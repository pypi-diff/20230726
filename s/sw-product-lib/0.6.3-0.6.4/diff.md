# Comparing `tmp/sw_product_lib-0.6.3.tar.gz` & `tmp/sw_product_lib-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw_product_lib-0.6.3.tar", max compression
+gzip compressed data, was "sw_product_lib-0.6.4.tar", max compression
```

## Comparing `sw_product_lib-0.6.3.tar` & `sw_product_lib-0.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1097 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/pyproject.toml
--rw-r--r--   0        0        0       87 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/client/__init__.py
--rw-r--r--   0        0        0    10691 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/client/backend.py
--rw-r--r--   0        0        0     3885 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/client/billing.py
--rw-r--r--   0        0        0     7180 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/client/job.py
--rw-r--r--   0        0        0     2186 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/client/resource.py
--rw-r--r--   0        0        0        0 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/platform/__init__.py
--rw-r--r--   0        0        0      331 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/platform/gql.py
--rw-r--r--   0        0        0    27535 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/service.py
--rw-r--r--   0        0        0     2239 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/types/batch_job.py
--rw-r--r--   0        0        0    23167 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/types/job.py
--rw-r--r--   0        0        0     8702 2023-06-09 14:55:14.450120 sw_product_lib-0.6.3/sw_product_lib/types/resource.py
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 sw_product_lib-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-07-26 15:06:29.174447 sw_product_lib-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0       87 2023-07-26 15:06:29.174447 sw_product_lib-0.6.4/sw_product_lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:06:29.174447 sw_product_lib-0.6.4/sw_product_lib/client/__init__.py
+-rw-r--r--   0        0        0    10691 2023-07-26 15:06:29.174447 sw_product_lib-0.6.4/sw_product_lib/client/backend.py
+-rw-r--r--   0        0        0     3885 2023-07-26 15:06:29.174447 sw_product_lib-0.6.4/sw_product_lib/client/billing.py
+-rw-r--r--   0        0        0     7180 2023-07-26 15:06:29.174447 sw_product_lib-0.6.4/sw_product_lib/client/job.py
+-rw-r--r--   0        0        0     2186 2023-07-26 15:06:29.178447 sw_product_lib-0.6.4/sw_product_lib/client/resource.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:06:29.178447 sw_product_lib-0.6.4/sw_product_lib/platform/__init__.py
+-rw-r--r--   0        0        0      331 2023-07-26 15:06:29.178447 sw_product_lib-0.6.4/sw_product_lib/platform/gql.py
+-rw-r--r--   0        0        0    27719 2023-07-26 15:06:29.178447 sw_product_lib-0.6.4/sw_product_lib/service.py
+-rw-r--r--   0        0        0     2416 2023-07-26 15:06:29.178447 sw_product_lib-0.6.4/sw_product_lib/types/batch_job.py
+-rw-r--r--   0        0        0    23167 2023-07-26 15:06:29.178447 sw_product_lib-0.6.4/sw_product_lib/types/job.py
+-rw-r--r--   0        0        0     8702 2023-07-26 15:06:29.178447 sw_product_lib-0.6.4/sw_product_lib/types/resource.py
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 sw_product_lib-0.6.4/PKG-INFO
```

### Comparing `sw_product_lib-0.6.3/pyproject.toml` & `sw_product_lib-0.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 per-file-ignores = [
     "__init__.py:F401",
     "./docs/*:E402"
 ]
 
 [tool.poetry]
 name = "sw-product-lib"
-version = "0.6.3"
+version = "0.6.4"
 description = "Python library for Strangeworks products to interact with the Strangeworks Platform"
 authors = ["Strangeworks Devs <hello@strangeworks.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 rich = "^12.4.4"
 gql = "^3.4.1"
 sgqlc = "^16.0"
 aiofiles = "^0.8.0"
 fastapi = "^0.85.0"
 python-jose = {extras = ["cryptography"], version = "^3.3.0"}
-strangeworks-core = "^0.2.1"
+strangeworks-core = "^0.2.4"
 deprecated = "^1.2.13"
 
 
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^5.0.4"
 pre-commit = "^2.20.0"
```

### Comparing `sw_product_lib-0.6.3/sw_product_lib/client/backend.py` & `sw_product_lib-0.6.4/sw_product_lib/client/backend.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.3/sw_product_lib/client/billing.py` & `sw_product_lib-0.6.4/sw_product_lib/client/billing.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.3/sw_product_lib/client/job.py` & `sw_product_lib-0.6.4/sw_product_lib/client/job.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.3/sw_product_lib/client/resource.py` & `sw_product_lib-0.6.4/sw_product_lib/client/resource.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.3/sw_product_lib/service.py` & `sw_product_lib-0.6.4/sw_product_lib/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import requests
 from deprecated import deprecated
 from fastapi import Request
 from jose import jwt
 from strangeworks_core.errors.error import StrangeworksError
 from strangeworks_core.platform import auth
 from strangeworks_core.platform.gql import API, APIInfo
+from strangeworks_core.types.batch import Options
 from strangeworks_core.types.func import Func
 from strangeworks_core.types.job import Status as JobStatus
 from strangeworks_core.types.machine import Accelerator, Machine
 
 from sw_product_lib.client import backend, billing, resource
 from sw_product_lib.client.billing import BillingTransaction
 from sw_product_lib.platform.gql import ProductAPI
@@ -837,14 +838,15 @@
     fargs: tuple = (),
     fkwargs: dict[str, Any] = {},
     machine: Machine = Machine(),
     accelerator: Optional[Accelerator] = None,
     requirements_path: Optional[str] = None,
     job_slug: Optional[str] = None,
     workspace_member_slug: Optional[str] = None,
+    options: Optional[Options] = None,
 ) -> str:
     """
     Create a batch job.
 
     Parameters
     ----------
     ctx: RequestContext
@@ -861,14 +863,16 @@
         An accelerator to use.
     requirements_path: Optional[str]
         The path to the requirements file.
     job_slug: Optional[str]
         The slug of the job.
     workspace_member_slug: Optional[str]
         The slug of the workspace member.
+    options: Optional[Options]
+        The options for the batch job.
 
     Returns
     -------
     batch_job_slug: str
         The slug of the batch job.
 
     """
@@ -882,8 +886,9 @@
         resource_slug=ctx.resource_slug,
         decorator_name="",
         func=f,
         machine=machine,
         accelerator=accelerator,
         job_slug=job_slug,
         workspace_member_slug=workspace_member_slug,
+        options=options,
     )
```

### Comparing `sw_product_lib-0.6.3/sw_product_lib/types/batch_job.py` & `sw_product_lib-0.6.4/sw_product_lib/types/batch_job.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import Optional
 
 from strangeworks_core.batch.utils import send_batch_request
 from strangeworks_core.platform.gql import API, Operation
+from strangeworks_core.types.batch import Options
 from strangeworks_core.types.func import Func
 from strangeworks_core.types.machine import Accelerator, Machine
 
 
 def new(
     api: API,
     resource_slug: str,
     decorator_name: str,
     func: Func,
     machine: Optional[Machine] = None,
     accelerator: Optional[Accelerator] = None,
     job_slug: Optional[str] = None,
     workspace_member_slug: Optional[str] = None,
+    options: Optional[Options] = None,
     **kwargs
 ) -> str:
     """
     Create a new batch job.
 
     Parameters
     ----------
@@ -34,14 +36,16 @@
         The machine to run the job on.
     accelerator : Optional[Accelerator]
         The accelerator to run the job on.
     job_slug : Optional[str]
         The job slug. Associate the batch job with a strangeworks job.
     workspace_member_slug : Optional[str]
         The workspace member slug. Associate the batch job with a workspace member.
+    options : Optional[Options]
+        The batch job options.
     **kwargs: dict
         Additional keyword arguments.
 
     Returns
     -------
     batch_job_slug: str
 
@@ -76,9 +80,10 @@
         decorator_name,
         func,
         machine,
         accelerator,
         resource_slug=resource_slug,
         job_slug=job_slug,
         workspace_member_slug=workspace_member_slug,
+        options=options,
         **kwargs
     )
```

### Comparing `sw_product_lib-0.6.3/sw_product_lib/types/job.py` & `sw_product_lib-0.6.4/sw_product_lib/types/job.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.3/sw_product_lib/types/resource.py` & `sw_product_lib-0.6.4/sw_product_lib/types/resource.py`

 * *Files identical despite different names*

### Comparing `sw_product_lib-0.6.3/PKG-INFO` & `sw_product_lib-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw-product-lib
-Version: 0.6.3
+Version: 0.6.4
 Summary: Python library for Strangeworks products to interact with the Strangeworks Platform
 License: Apache-2.0
 Author: Strangeworks Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -14,8 +14,8 @@
 Requires-Dist: aiofiles (>=0.8.0,<0.9.0)
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: fastapi (>=0.85.0,<0.86.0)
 Requires-Dist: gql (>=3.4.1,<4.0.0)
 Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
 Requires-Dist: sgqlc (>=16.0,<17.0)
-Requires-Dist: strangeworks-core (>=0.2.1,<0.3.0)
+Requires-Dist: strangeworks-core (>=0.2.4,<0.3.0)
```

