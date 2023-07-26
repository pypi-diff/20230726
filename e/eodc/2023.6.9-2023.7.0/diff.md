# Comparing `tmp/eodc-2023.6.9.tar.gz` & `tmp/eodc-2023.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.6.9.tar", max compression
+gzip compressed data, was "eodc-2023.7.0.tar", max compression
```

## Comparing `eodc-2023.6.9.tar` & `eodc-2023.7.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-06-29 11:54:54.077811 eodc-2023.6.9/README.md
--rw-r--r--   0        0        0      213 2023-06-29 11:54:54.077811 eodc-2023.6.9/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-29 11:54:54.077811 eodc-2023.6.9/eodc/dask.py
--rw-r--r--   0        0        0    11584 2023-06-29 11:54:54.077811 eodc-2023.6.9/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-06-29 11:54:54.077811 eodc-2023.6.9/eodc/settings.py
--rw-r--r--   0        0        0     1207 2023-06-29 11:54:54.077811 eodc-2023.6.9/pyproject.toml
--rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 eodc-2023.6.9/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-07-26 10:46:33.693857 eodc-2023.7.0/README.md
+-rw-r--r--   0        0        0      120 2023-07-26 10:46:33.693857 eodc-2023.7.0/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-07-26 10:46:33.693857 eodc-2023.7.0/eodc/dask.py
+-rw-r--r--   0        0        0    11843 2023-07-26 10:46:33.693857 eodc-2023.7.0/eodc/faas.py
+-rw-r--r--   0        0        0      537 2023-07-26 10:46:33.693857 eodc-2023.7.0/eodc/settings.py
+-rw-r--r--   0        0        0     1198 2023-07-26 10:46:33.693857 eodc-2023.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 eodc-2023.7.0/PKG-INFO
```

### Comparing `eodc-2023.6.9/README.md` & `eodc-2023.7.0/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.9/eodc/dask.py` & `eodc-2023.7.0/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.9/eodc/faas.py` & `eodc-2023.7.0/eodc/faas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,23 @@
 import json
 import logging
 import re
+import time
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
-from time import sleep
 from typing import Optional
+from urllib.parse import urljoin
 
-import argo_workflows
-from argo_workflows.api import workflow_service_api
-from argo_workflows.model.io_argoproj_workflow_v1alpha1_arguments import (
-    IoArgoprojWorkflowV1alpha1Arguments,
-)
-from argo_workflows.model.io_argoproj_workflow_v1alpha1_parameter import (
-    IoArgoprojWorkflowV1alpha1Parameter,
-)
-from argo_workflows.model.io_argoproj_workflow_v1alpha1_workflow import (
-    IoArgoprojWorkflowV1alpha1Workflow,
-)
-from argo_workflows.model.io_argoproj_workflow_v1alpha1_workflow_create_request import (
-    IoArgoprojWorkflowV1alpha1WorkflowCreateRequest,
-)
-from argo_workflows.model.io_argoproj_workflow_v1alpha1_workflow_spec import (
-    IoArgoprojWorkflowV1alpha1WorkflowSpec,
-)
-from argo_workflows.model.io_argoproj_workflow_v1alpha1_workflow_stop_request import (
-    IoArgoprojWorkflowV1alpha1WorkflowStopRequest,
-)
-from argo_workflows.model.io_argoproj_workflow_v1alpha1_workflow_template_ref import (
-    IoArgoprojWorkflowV1alpha1WorkflowTemplateRef,
-)
-from argo_workflows.model.object_meta import ObjectMeta
+import requests
 from force_processor_bindings.model import ForceParameters, ForceResMergeOptions  # noqa
+from hera.exceptions import NotFound, exception_from_server_response
+from hera.workflows import Parameter, Workflow, WorkflowsService
+from hera.workflows.models import WorkflowStopRequest, WorkflowTemplateRef
+from hera.workflows.service import valid_host_scheme
 from openeo_executor_bindings.model import OpenEOExecutorParameters
 from pystac import Collection, Item
 from sen2like_processor_bindings.model import BoundingBox as Sen2LikeBoundingBox  # noqa
 from sen2like_processor_bindings.model import (  # noqa
     Sen2LikeParameters,
     sen2like_options,
 )
@@ -68,113 +50,141 @@
 
 class FaasProcessorBase(ABC):
     @classmethod
     def get_instance(cls, processor_details):
         return cls(processor_details=processor_details)
 
     def __init__(self, processor_details: FaasProcessorDetails) -> None:
-        self.configuration = argo_workflows.Configuration(host=settings.FAAS_URL)
-        self.configuration.verify_ssl = False
-
-        self.api_client = argo_workflows.ApiClient(self.configuration)
-        self.api_instance_workflows = workflow_service_api.WorkflowServiceApi(
-            self.api_client
+        # The URL for hera needs to end with a slash,
+        # otherwise urlparse cuts the `/dev` part
+        host = (
+            settings.FAAS_URL + "/"
+            if not settings.FAAS_URL.endswith("/")
+            else settings.FAAS_URL
+        )
+        self.workflows_service = WorkflowsService(
+            host=host, verify_ssl=False, namespace=settings.NAMESPACE
         )
+
         self.processor_details = processor_details
-        # TODO: Check here that this workflow template even exists on the server
+        try:
+            self.workflows_service.get_info()
+        except ConnectionError:
+            raise Exception(
+                f"Could not establish connection to argo workflows server "
+                f"at {settings.FAAS_URL} in namespace {settings.NAMESPACE}"
+            )
+
+        try:
+            self.workflows_service.get_workflow_template(
+                processor_details.workflow_template_name, namespace=settings.NAMESPACE
+            )
+        except NotFound:
+            raise Exception(
+                f"Could not initialise faas module {self.processor_details.name} as the"
+                f" workflow template {self.processor_details.workflow_template_name} "
+                f"could not be found in namespace {settings.NAMESPACE}"
+            )
 
     def submit_workflow(self, **kwargs):
         if (
             "user_id" in kwargs
             and re.match(LABEL_VALIDATION_REGEX, kwargs["user_id"]) is None
         ):
             raise ValueError("invalid user_id")
         if (
             "job_id" in kwargs
             and re.match(LABEL_VALIDATION_REGEX, kwargs["job_id"]) is None
         ):
             raise ValueError("invalid user_id")
 
-        parameters = [
-            IoArgoprojWorkflowV1alpha1Parameter(name=k, value=v)
-            for k, v in kwargs.items()
-        ]
+        arguments = [Parameter(name=k, value=v) for k, v in kwargs.items()]
 
-        manifest = IoArgoprojWorkflowV1alpha1Workflow(
-            metadata=ObjectMeta(
-                generate_name=f"{self.processor_details.name.lower()}-"
+        workflow = Workflow(
+            workflow_template_ref=WorkflowTemplateRef(
+                name=self.processor_details.workflow_template_name
             ),
-            spec=IoArgoprojWorkflowV1alpha1WorkflowSpec(
-                workflow_template_ref=IoArgoprojWorkflowV1alpha1WorkflowTemplateRef(
-                    name=self.processor_details.workflow_template_name
-                ),
-                arguments=IoArgoprojWorkflowV1alpha1Arguments(parameters=parameters),
-            ),
-        )
-
-        created_workflow = self.api_instance_workflows.create_workflow(
+            workflows_service=self.workflows_service,
             namespace=settings.NAMESPACE,
-            body=IoArgoprojWorkflowV1alpha1WorkflowCreateRequest(workflow=manifest),
-            _check_return_type=False,
+            generate_name=f"{self.processor_details.name}-",
+            arguments=arguments,
         )
-
-        workflow_name = created_workflow.metadata.get("name")
+        workflow.create()
 
         logger.info(
-            f"Submitted {self.processor_details.name.upper()} workflow: {workflow_name}"
+            f"Submitted {self.processor_details.name.upper()} workflow: {workflow.name}"
         )
-        return workflow_name
+        return workflow.name
 
-    def get_workflow_status(self, workflow_name: str) -> dict:
-        status = self.api_instance_workflows.get_workflow(
-            namespace=settings.NAMESPACE,
-            name=workflow_name,
-            fields="status.phase,status.finishedAt,status.startedAt",
-            _check_return_type=False,
-        ).get("status", {})
-        return status
-
-    def wait_for_completion(self, workflow_name: str) -> None:
-        """Repeatedly query workflow status until it changes to a completed state"""
-
-        while (status := self.get_workflow_status(workflow_name)).get(
-            "finishedAt"
-        ) is None:
-            logger.info("Workflow still running, sleeping 30 seconds")
-            sleep(30)
-        logger.info(f"Workflow completed with status {status.get('phase')}.")
-
-        if status.get("phase") in ("Failed", "Error"):
-            raise ValueError(
-                f"Workflow {workflow_name} ended with status {status.get('phase')}"
+    def wait_for_completion(self, workflow_name, poll_interval=30):
+        wf = self.workflows_service.get_workflow(
+            workflow_name, namespace=settings.NAMESPACE
+        )
+
+        # keep polling for workflow status until completed,
+        # at the interval dictated by the user
+        while wf.status.phase in ("Pending", "Running"):
+            time.sleep(poll_interval)
+            wf = self.workflows_service.get_workflow(
+                wf.metadata.name, namespace=settings.NAMESPACE
             )
+        return wf
+
+    def get_workflow_status(self, workflow_name: str) -> dict:
+        # TODO: Limit this response to only the required fields
+        workflow_response = self.workflows_service.get_workflow(
+            name=workflow_name, namespace=settings.NAMESPACE
+        )
+        return dict(workflow_response.status)
 
     def stop_workflow(self, name):
-        body = IoArgoprojWorkflowV1alpha1WorkflowStopRequest()
-        self.api_instance_workflows.stop_workflow(settings.NAMESPACE, name, body=body)
-        logger.info(f"Successfully stopped workflow {name}.")
+        req = WorkflowStopRequest(name=name, namespace=settings.NAMESPACE)
+        try:
+            self.workflows_service.stop_workflow(
+                name, req=req, namespace=settings.NAMESPACE
+            )
+            logger.info(f"Successfully stopped workflow {name}.")
+        except NotFound:
+            logger.warning(f"Could not stop workflow {name}.")
 
     def get_logs(self, workflow_name) -> list[str]:
-        # The .workflow_logs client method seems semi-broken:
-        # https://github.com/argoproj/argo-workflows/issues/7781
-        # Therefore this workaround is necessary!
-        raw_logs = (
-            self.api_instance_workflows.workflow_logs(
-                settings.NAMESPACE,
-                workflow_name,
-                log_options_container="main",
-                #  log_options_follow=True,
-                _check_return_type=False,
-                _preload_content=False,
-            )
-            .read()
-            .decode("utf-8")
-            .splitlines()
+        assert valid_host_scheme(
+            self.workflows_service.host
+        ), "The host scheme is required for service usage"
+        resp = requests.get(
+            url=urljoin(
+                self.workflows_service.host, "api/v1/workflows/{namespace}/{name}/log"
+            ).format(name=workflow_name, namespace=settings.NAMESPACE),
+            params={
+                "podName": None,
+                "logOptions.container": "main",
+                "logOptions.follow": None,
+                "logOptions.previous": None,
+                "logOptions.sinceSeconds": None,
+                "logOptions.sinceTime.seconds": None,
+                "logOptions.sinceTime.nanos": None,
+                "logOptions.timestamps": None,
+                "logOptions.tailLines": None,
+                "logOptions.limitBytes": None,
+                "logOptions.insecureSkipTLSVerifyBackend": None,
+                "grep": None,
+                "selector": None,
+            },
+            headers={"Authorization": f"Bearer {self.workflows_service.token}"},
+            data=None,
+            verify=self.workflows_service.verify_ssl,
         )
-        return [json.loads(log)["result"]["content"] for log in raw_logs]
+
+        if resp.ok:
+            raw_logs = resp.content.decode("utf8").split("\n")
+            return [
+                json.loads(log)["result"]["content"] for log in raw_logs if log != ""
+            ]
+
+        raise exception_from_server_response(resp)
 
     @abstractmethod
     def get_output_stac_items(self):
         raise NotImplementedError()
 
 
 class Force(FaasProcessorBase):
@@ -255,31 +265,29 @@
             for link in openeo_output_collection.get_item_links()
         ]
 
         return stac_items
 
     def _get_workflows_for_job_id(
         self, openeo_job_id, filter_workflow_status_phase: Optional[tuple[str]] = None
-    ):
+    ) -> list[Workflow]:
         # filter_workflow_status_phase wants to be an iterable
         # of strings like ("Running", "Pending")
-
-        workflows_with_label = self.api_instance_workflows.list_workflows(
+        workflows = self.workflows_service.list_workflows(
             namespace=settings.NAMESPACE,
-            list_options_label_selector=f"openeo_job_id={openeo_job_id}",
+            label_selector=f"openeo_job_id={openeo_job_id}",
         ).items
-
         if filter_workflow_status_phase is not None:
             workflows_with_label_filtered = [
                 workflow
-                for workflow in workflows_with_label
+                for workflow in workflows
                 if workflow.status.phase in filter_workflow_status_phase
             ]
         else:
-            workflows_with_label_filtered = workflows_with_label
+            workflows_with_label_filtered = workflows
         return workflows_with_label_filtered
 
     def stop_openeo_job(self, openeo_job_id):
         associated_unfinished_workflows = self._get_workflows_for_job_id(
             openeo_job_id=openeo_job_id,
             filter_workflow_status_phase=("Running", "Pending"),
         )
```

### Comparing `eodc-2023.6.9/pyproject.toml` & `eodc-2023.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.6.9"
+version = "2023.7.0"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -19,22 +19,22 @@
 
 packages = [{include = "eodc"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 requests = "^2.28.2"
 pydantic = "^1.10.7"
-argo-workflows = "6.3.9"
 dask-gateway = "^2022.11.0"
-eodc-faas-force = "^2023.6.2"
+eodc-faas-force = "^2023.7.1"
 eodc-faas-sen2like = "^2023.6.2"
 eodc-faas-openeo = "^2023.6.8"
 pystac = "^1.7.3"
 eodc-faas-snap = "^2023.6.2"
 pyproj = "^3.6.0"
+hera = "^5.5.2"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.0"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 ipykernel = "^6.22.0"
```

### Comparing `eodc-2023.6.9/PKG-INFO` & `eodc-2023.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.6.9
+Version: 2023.7.0
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
@@ -12,20 +12,20 @@
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: argo-workflows (==6.3.9)
 Requires-Dist: dask-gateway (>=2022.11.0,<2023.0.0)
-Requires-Dist: eodc-faas-force (>=2023.6.2,<2024.0.0)
+Requires-Dist: eodc-faas-force (>=2023.7.1,<2024.0.0)
 Requires-Dist: eodc-faas-openeo (>=2023.6.8,<2024.0.0)
 Requires-Dist: eodc-faas-sen2like (>=2023.6.2,<2024.0.0)
 Requires-Dist: eodc-faas-snap (>=2023.6.2,<2024.0.0)
+Requires-Dist: hera (>=5.5.2,<6.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyproj (>=3.6.0,<4.0.0)
 Requires-Dist: pystac (>=1.7.3,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/eodcgmbh/eodc-sdk
 Description-Content-Type: text/markdown
```

