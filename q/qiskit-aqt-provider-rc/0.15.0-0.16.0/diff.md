# Comparing `tmp/qiskit_aqt_provider_rc-0.15.0.tar.gz` & `tmp/qiskit_aqt_provider_rc-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_aqt_provider_rc-0.15.0.tar", max compression
+gzip compressed data, was "qiskit_aqt_provider_rc-0.16.0.tar", max compression
```

## Comparing `qiskit_aqt_provider_rc-0.15.0.tar` & `qiskit_aqt_provider_rc-0.16.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     3214 2023-06-22 14:50:37.327675 qiskit_aqt_provider_rc-0.15.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0    14035 2023-06-22 14:50:37.327675 qiskit_aqt_provider_rc-0.15.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11416 2023-06-22 14:50:37.327675 qiskit_aqt_provider_rc-0.15.0/LICENSE.txt
--rw-r--r--   0        0        0     1467 2023-06-22 14:50:37.327675 qiskit_aqt_provider_rc-0.15.0/README.md
--rw-r--r--   0        0        0     6144 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/pyproject.toml
--rw-r--r--   0        0        0      562 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/__init__.py
--rw-r--r--   0        0        0     8241 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/api_models.py
--rw-r--r--   0        0        0    12734 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/api_models_generated.py
--rw-r--r--   0        0        0    16481 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_job.py
--rw-r--r--   0        0        0     2704 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_options.py
--rw-r--r--   0        0        0     8824 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_provider.py
--rw-r--r--   0        0        0    12462 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_resource.py
--rw-r--r--   0        0        0     3425 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/circuit_to_aqt.py
--rw-r--r--   0        0        0      564 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/__init__.py
--rw-r--r--   0        0        0     2476 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/estimator.py
--rw-r--r--   0        0        0     2286 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/sampler.py
--rw-r--r--   0        0        0        0 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/py.typed
--rw-r--r--   0        0        0      587 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/__init__.py
--rw-r--r--   0        0        0     1884 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/circuits.py
--rw-r--r--   0        0        0     2703 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/fixtures.py
--rw-r--r--   0        0        0     6970 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/resources.py
--rw-r--r--   0        0        0     1259 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/timeout.py
--rw-r--r--   0        0        0     7323 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/transpiler_plugin.py
--rw-r--r--   0        0        0     1838 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/utils.py
--rw-r--r--   0        0        0     1040 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/versions.py
--rw-r--r--   0        0        0        0 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/__init__.py
--rw-r--r--   0        0        0     3822 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_api_models.py
--rw-r--r--   0        0        0     6142 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_circuit_to_aqt.py
--rw-r--r--   0        0        0    13208 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_execution.py
--rw-r--r--   0        0        0     2121 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_options.py
--rw-r--r--   0        0        0     6630 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_primitives.py
--rw-r--r--   0        0        0     5139 2023-06-22 14:50:37.331675 qiskit_aqt_provider_rc-0.15.0/test/test_provider.py
--rw-r--r--   0        0        0    11103 2023-06-22 14:50:37.335675 qiskit_aqt_provider_rc-0.15.0/test/test_resource.py
--rw-r--r--   0        0        0     8668 2023-06-22 14:50:37.335675 qiskit_aqt_provider_rc-0.15.0/test/test_transpilation.py
--rw-r--r--   0        0        0     1063 2023-06-22 14:50:37.335675 qiskit_aqt_provider_rc-0.15.0/test/test_utils.py
--rw-r--r--   0        0        0     2921 1970-01-01 00:00:00.000000 qiskit_aqt_provider_rc-0.15.0/PKG-INFO
+-rw-r--r--   0        0        0     3214 2023-07-26 12:49:02.878883 qiskit_aqt_provider_rc-0.16.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0    14035 2023-07-26 12:49:02.878883 qiskit_aqt_provider_rc-0.16.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11416 2023-07-26 12:49:02.878883 qiskit_aqt_provider_rc-0.16.0/LICENSE.txt
+-rw-r--r--   0        0        0     1467 2023-07-26 12:49:02.878883 qiskit_aqt_provider_rc-0.16.0/README.md
+-rw-r--r--   0        0        0     6352 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/pyproject.toml
+-rw-r--r--   0        0        0      562 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/__init__.py
+-rw-r--r--   0        0        0     8241 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/api_models.py
+-rw-r--r--   0        0        0    12734 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/api_models_generated.py
+-rw-r--r--   0        0        0    16481 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/aqt_job.py
+-rw-r--r--   0        0        0     2704 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/aqt_options.py
+-rw-r--r--   0        0        0     8995 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/aqt_provider.py
+-rw-r--r--   0        0        0    12366 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/aqt_resource.py
+-rw-r--r--   0        0        0     3425 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/circuit_to_aqt.py
+-rw-r--r--   0        0        0      616 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/primitives/__init__.py
+-rw-r--r--   0        0        0     2476 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/primitives/estimator.py
+-rw-r--r--   0        0        0     2286 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/primitives/sampler.py
+-rw-r--r--   0        0        0        0 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/py.typed
+-rw-r--r--   0        0        0      587 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/test/__init__.py
+-rw-r--r--   0        0        0     1884 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/test/circuits.py
+-rw-r--r--   0        0        0     2703 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/test/fixtures.py
+-rw-r--r--   0        0        0     6970 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/test/resources.py
+-rw-r--r--   0        0        0     1259 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/test/timeout.py
+-rw-r--r--   0        0        0     7323 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/transpiler_plugin.py
+-rw-r--r--   0        0        0     1838 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/utils.py
+-rw-r--r--   0        0        0     1040 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/versions.py
+-rw-r--r--   0        0        0        0 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/test/__init__.py
+-rw-r--r--   0        0        0     3822 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/test/test_api_models.py
+-rw-r--r--   0        0        0     6142 2023-07-26 12:49:02.882883 qiskit_aqt_provider_rc-0.16.0/test/test_circuit_to_aqt.py
+-rw-r--r--   0        0        0    13208 2023-07-26 12:49:02.886883 qiskit_aqt_provider_rc-0.16.0/test/test_execution.py
+-rw-r--r--   0        0        0     2121 2023-07-26 12:49:02.886883 qiskit_aqt_provider_rc-0.16.0/test/test_options.py
+-rw-r--r--   0        0        0     6630 2023-07-26 12:49:02.886883 qiskit_aqt_provider_rc-0.16.0/test/test_primitives.py
+-rw-r--r--   0        0        0     5412 2023-07-26 12:49:02.886883 qiskit_aqt_provider_rc-0.16.0/test/test_provider.py
+-rw-r--r--   0        0        0    11103 2023-07-26 12:49:02.886883 qiskit_aqt_provider_rc-0.16.0/test/test_resource.py
+-rw-r--r--   0        0        0     8668 2023-07-26 12:49:02.886883 qiskit_aqt_provider_rc-0.16.0/test/test_transpilation.py
+-rw-r--r--   0        0        0     1063 2023-07-26 12:49:02.886883 qiskit_aqt_provider_rc-0.16.0/test/test_utils.py
+-rw-r--r--   0        0        0     3037 1970-01-01 00:00:00.000000 qiskit_aqt_provider_rc-0.16.0/PKG-INFO
```

### Comparing `qiskit_aqt_provider_rc-0.15.0/CODE_OF_CONDUCT.md` & `qiskit_aqt_provider_rc-0.16.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/CONTRIBUTING.md` & `qiskit_aqt_provider_rc-0.16.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/LICENSE.txt` & `qiskit_aqt_provider_rc-0.16.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/README.md` & `qiskit_aqt_provider_rc-0.16.0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/pyproject.toml` & `qiskit_aqt_provider_rc-0.16.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qiskit-aqt-provider-rc"
-version = "0.15.0"
+version = "0.16.0"
 description = "Qiskit provider for AQT backends"
 authors = ["Qiskit Development Team", "Alpine Quantum Technologies GmbH"]
 repository = "https://github.com/alpine-quantum-technologies/qiskit-aqt-provider-rc/"
 readme = "README.md"
 license = "Apache-2.0"
 classifiers=[
         "Intended Audience :: Developers",
@@ -44,53 +44,57 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 
 httpx = ">=0.24.0"
 pydantic = ">=1.10.8,<2"
 python-dotenv = ">=1"
 qiskit-aer = ">=0.11"
+qiskit-optimization = { version = ">=0.5.0", optional = true }
 qiskit-terra = ">=0.23.3,!=0.24.0"
 tabulate = ">=0.9.0"
 tqdm = ">=4"
 tweedledum = { version = ">=1", optional = true }
 typing-extensions = ">=4.0.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
+black = "^23.7.0"
 coverage = "^7.2.1"
-datamodel-code-generator = "^0.19.0"
-hypothesis = "^6.70.0"
+datamodel-code-generator = "^0.21.2"
+hypothesis = "^6.82.0"
 ipykernel = "^6.22.0"
 jupyter-sphinx = "^0.4.0"
-mistletoe = "^1.0.1"
-mypy = "=1.3.0"
+mistletoe = "^1.1.0"
+mypy = "=1.4.1"
 poethepoet = "^0.18.1"
 polyfactory = "^2.0.0"
 pre-commit = "^3.1.1"
-pyproject-fmt = "^0.9.2"
-pyright = "=1.1.308"
+pyproject-fmt = "^0.13.0"
 pytest = ">=7"
 pytest-httpx = "^0.22.0"
 pytest-sugar = "^0.9.6"
 qiskit-experiments = "^0.4.0"
 qiskit-sphinx-theme = ">=1.7.0"
 qiskit-terra = {version = ">=0.23.2", extras = ["visualization"]}
-ruff = "^0.0.267"
+ruff = "^0.0.280"
 sphinx = "^6"
 sympy = "^1.11.1"
 typer = "^0.7.0"
 types-requests = "^2.28.11"
 types-setuptools = "^65.7.0"
 types-tabulate = "^0.9.0.1"
 types-tqdm = "^4.65.0.1"
 
 [tool.poetry.extras]
-examples = [
+# dependencies for examples that are not compatible with recent Python versions
+examples-problematic = [
     "tweedledum"
 ]
+examples = [
+    "qiskit-optimization"
+]
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = [
   "poetry-core>=1",
 ]
 
@@ -204,15 +208,16 @@
 dynamic_context = "test_function"
 
 [tool.coverage.report]
 fail_under = 98
 
 [tool.poe.tasks.test]
 shell = """
-coverage run ${cov_opts} -m pytest
+set -eu
+coverage run ${cov_opts} -m pytest --hypothesis-profile=ci
 coverage report
 """
 
 [[tool.poe.tasks.test.args]]
 name = "cov_opts"
 default = ""
```

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/__init__.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/api_models.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/api_models.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/api_models_generated.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/api_models_generated.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_job.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/aqt_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_options.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/aqt_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_provider.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/aqt_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 
 import contextlib
 import os
 import re
+import warnings
 from collections import defaultdict
 from dataclasses import dataclass
 from operator import attrgetter
 from pathlib import Path
 from typing import (
     DefaultDict,
     Dict,
@@ -40,14 +41,18 @@
 from qiskit_aqt_provider import api_models
 
 from .aqt_resource import AQTResource, OfflineSimulatorResource
 
 StrPath: TypeAlias = Union[str, Path]
 
 
+class NoTokenWarning(UserWarning):
+    """Warning emitted when a provider is initialized with no access token."""
+
+
 @dataclass(frozen=True)
 class OfflineSimulator:
     """Description of an offline simulator."""
 
     id: str
     """Unique identifier of the simulator."""
 
@@ -172,20 +177,24 @@
         if load_dotenv or dotenv_path is not None:
             dotenv.load_dotenv(dotenv_path)
 
         portal_base_url = os.environ.get("AQT_PORTAL_URL", AQTProvider.DEFAULT_PORTAL_URL)
         self.portal_url = f"{portal_base_url}/api/v1"
 
         if access_token is None:
-            env_token = os.environ.get("AQT_TOKEN")
-            if env_token is None:
-                raise ValueError("No access token provided. Use 'AQT_TOKEN' environment variable.")
-            self.access_token = env_token
+            self.access_token = os.environ.get("AQT_TOKEN", "")
         else:
             self.access_token = access_token
+
+        if not self.access_token:
+            warnings.warn(
+                "No access token provided: access is restricted to the 'default' workspace.",
+                NoTokenWarning,
+            )
+
         self.name = "aqt_provider"
 
     @property
     def _http_client(self) -> httpx.Client:
         """HTTP client for communicating with the AQT cloud service."""
         return api_models.http_client(base_url=self.portal_url, token=self.access_token)
```

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/aqt_resource.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/aqt_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,34 +149,30 @@
         """
         resp = self._http_client.get(f"/result/{job_id}")
         resp.raise_for_status()
         return api_models.Response.parse_obj(resp.json())
 
     def configuration(self) -> BackendConfiguration:
         warnings.warn(
-            (
-                "The configuration() method is deprecated and will be removed in a "
-                "future release. Instead you should access these attributes directly "
-                "off the object or via the .target attribute. You can refer to qiskit "
-                "backend interface transition guide for the exact changes: "
-                "https://qiskit.org/documentation/apidoc/providers.html#backendv1-backendv2"
-            ),
+            "The configuration() method is deprecated and will be removed in a "
+            "future release. Instead you should access these attributes directly "
+            "off the object or via the .target attribute. You can refer to qiskit "
+            "backend interface transition guide for the exact changes: "
+            "https://qiskit.org/documentation/apidoc/providers.html#backendv1-backendv2",
             DeprecationWarning,
         )
         return self._configuration
 
     def properties(self) -> None:
         warnings.warn(  # pragma: no cover
-            (
-                "The properties() method is deprecated and will be removed in a "
-                "future release. Instead you should access these attributes directly "
-                "off the object or via the .target attribute. You can refer to qiskit "
-                "backend interface transition guide for the exact changes: "
-                "https://qiskit.org/documentation/apidoc/providers.html#backendv1-backendv2"
-            ),
+            "The properties() method is deprecated and will be removed in a "
+            "future release. Instead you should access these attributes directly "
+            "off the object or via the .target attribute. You can refer to qiskit "
+            "backend interface transition guide for the exact changes: "
+            "https://qiskit.org/documentation/apidoc/providers.html#backendv1-backendv2",
             DeprecationWarning,
         )
 
     @property
     def max_circuits(self) -> int:
         return 2000
```

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/circuit_to_aqt.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/circuit_to_aqt.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/__init__.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/primitives/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,10 +6,11 @@
 # obtain a copy of this license in the LICENSE.txt file in the root directory
 # of this source tree or at http://www.apache.org/licenses/LICENSE-2.0.
 #
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
+from .estimator import AQTEstimator
 from .sampler import AQTSampler
 
-__all__ = ["AQTSampler"]
+__all__ = ["AQTEstimator", "AQTSampler"]
```

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/estimator.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/primitives/estimator.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/primitives/sampler.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/primitives/sampler.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/__init__.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/circuits.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/test/circuits.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/fixtures.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/test/fixtures.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/resources.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/test/resources.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/test/timeout.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/test/timeout.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/transpiler_plugin.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/transpiler_plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/utils.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/qiskit_aqt_provider/versions.py` & `qiskit_aqt_provider_rc-0.16.0/qiskit_aqt_provider/versions.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/test/test_api_models.py` & `qiskit_aqt_provider_rc-0.16.0/test/test_api_models.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/test/test_circuit_to_aqt.py` & `qiskit_aqt_provider_rc-0.16.0/test/test_circuit_to_aqt.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/test/test_execution.py` & `qiskit_aqt_provider_rc-0.16.0/test/test_execution.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/test/test_options.py` & `qiskit_aqt_provider_rc-0.16.0/test/test_options.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/test/test_primitives.py` & `qiskit_aqt_provider_rc-0.16.0/test/test_primitives.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/test/test_provider.py` & `qiskit_aqt_provider_rc-0.16.0/test/test_provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from unittest import mock
 from urllib.parse import urlparse
 
 import pytest
 from pytest_httpx import HTTPXMock
 
 from qiskit_aqt_provider import api_models, api_models_generated
-from qiskit_aqt_provider.aqt_provider import OFFLINE_SIMULATORS, AQTProvider
+from qiskit_aqt_provider.aqt_provider import OFFLINE_SIMULATORS, AQTProvider, NoTokenWarning
 
 
 def test_default_portal_url() -> None:
     """Check that by default, the portal url is that of the class variable."""
     with mock.patch.object(os, "environ", {}):
         aqt = AQTProvider("my-token")
 
@@ -93,19 +93,27 @@
     dotenv_path.write_text(f'AQT_TOKEN = "{env_token}"')
 
     with mock.patch.object(os, "environ", {}):
         aqt = AQTProvider(dotenv_path=dotenv_path)
         assert aqt.access_token == env_token
 
 
-def test_autoload_env_deactivated() -> None:
-    """Check that auto-loading the environment can be deactivated."""
+def test_default_to_empty_token() -> None:
+    """Check that if no token is passed and AQT_TOKEN is not found in the environment,
+    the access token is set to an empty string.
+
+    In this case, the only accessible workspace is the default workspace.
+    """
     with mock.patch.object(os, "environ", {}):
-        with pytest.raises(ValueError, match="No access token provided"):
-            AQTProvider(load_dotenv=False)
+        with pytest.warns(NoTokenWarning, match="No access token provided"):
+            aqt = AQTProvider(load_dotenv=False)
+
+        assert aqt.access_token == ""
+
+    assert list(aqt.backends().by_workspace()) == ["default"]
 
 
 def test_remote_workspaces_table(httpx_mock: HTTPXMock) -> None:
     """Check that the AQTProvider.backends() methods can fetch a list of available
     workspaces and associated resources over HTTP.
 
     Check that the offline simulators are added if they match the search criteria.
```

### Comparing `qiskit_aqt_provider_rc-0.15.0/test/test_resource.py` & `qiskit_aqt_provider_rc-0.16.0/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/test/test_transpilation.py` & `qiskit_aqt_provider_rc-0.16.0/test/test_transpilation.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/test/test_utils.py` & `qiskit_aqt_provider_rc-0.16.0/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit_aqt_provider_rc-0.15.0/PKG-INFO` & `qiskit_aqt_provider_rc-0.16.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-aqt-provider-rc
-Version: 0.15.0
+Version: 0.16.0
 Summary: Qiskit provider for AQT backends
 Home-page: https://github.com/alpine-quantum-technologies/qiskit-aqt-provider-rc/
 License: Apache-2.0
 Keywords: qiskit,sdk,quantum
 Author: Qiskit Development Team
 Requires-Python: >=3.8,<3.12
 Classifier: Intended Audience :: Developers
@@ -17,22 +17,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Provides-Extra: examples
+Provides-Extra: examples-problematic
 Requires-Dist: httpx (>=0.24.0)
 Requires-Dist: pydantic (>=1.10.8,<2)
 Requires-Dist: python-dotenv (>=1)
 Requires-Dist: qiskit-aer (>=0.11)
+Requires-Dist: qiskit-optimization (>=0.5.0) ; extra == "examples"
 Requires-Dist: qiskit-terra (>=0.23.3,!=0.24.0)
 Requires-Dist: tabulate (>=0.9.0)
 Requires-Dist: tqdm (>=4)
-Requires-Dist: tweedledum (>=1) ; extra == "examples"
+Requires-Dist: tweedledum (>=1) ; extra == "examples-problematic"
 Requires-Dist: typing-extensions (>=4.0.0)
 Project-URL: Repository, https://github.com/alpine-quantum-technologies/qiskit-aqt-provider-rc/
 Description-Content-Type: text/markdown
 
 # Qiskit AQT Provider
 
 [![Latest release](https://img.shields.io/pypi/v/qiskit-aqt-provider-rc.svg)](https://pypi.python.org/pypi/qiskit-aqt-provider-rc)
```

