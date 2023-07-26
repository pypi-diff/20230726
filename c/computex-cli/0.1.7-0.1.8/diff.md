# Comparing `tmp/computex_cli-0.1.7.tar.gz` & `tmp/computex_cli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computex_cli-0.1.7.tar", max compression
+gzip compressed data, was "computex_cli-0.1.8.tar", max compression
```

## Comparing `computex_cli-0.1.7.tar` & `computex_cli-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1233 2023-07-21 20:22:34.791518 computex_cli-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/__init__.py
--rw-r--r--   0        0        0     8944 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/cli.py
--rw-r--r--   0        0        0      911 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/config.py
--rw-r--r--   0        0        0      161 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/exc.py
--rw-r--r--   0        0        0        0 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/services/__init__.py
--rw-r--r--   0        0        0      950 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/services/auth.py
--rw-r--r--   0        0        0     3065 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/services/deployments.py
--rw-r--r--   0        0        0     1912 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/services/service.py
--rw-r--r--   0        0        0     1236 2023-07-21 20:22:34.791518 computex_cli-0.1.7/cxcli/services/users.py
--rw-r--r--   0        0        0      773 2023-07-21 20:22:34.791518 computex_cli-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 computex_cli-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1233 2023-07-26 16:56:58.753727 computex_cli-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 16:56:58.753727 computex_cli-0.1.8/cxcli/__init__.py
+-rw-r--r--   0        0        0     9243 2023-07-26 16:56:58.753727 computex_cli-0.1.8/cxcli/cli.py
+-rw-r--r--   0        0        0      911 2023-07-26 16:56:58.753727 computex_cli-0.1.8/cxcli/config.py
+-rw-r--r--   0        0        0      161 2023-07-26 16:56:58.753727 computex_cli-0.1.8/cxcli/exc.py
+-rw-r--r--   0        0        0        0 2023-07-26 16:56:58.753727 computex_cli-0.1.8/cxcli/services/__init__.py
+-rw-r--r--   0        0        0      950 2023-07-26 16:56:58.753727 computex_cli-0.1.8/cxcli/services/auth.py
+-rw-r--r--   0        0        0     3137 2023-07-26 16:56:58.753727 computex_cli-0.1.8/cxcli/services/deployments.py
+-rw-r--r--   0        0        0     1912 2023-07-26 16:56:58.753727 computex_cli-0.1.8/cxcli/services/service.py
+-rw-r--r--   0        0        0     1236 2023-07-26 16:56:58.753727 computex_cli-0.1.8/cxcli/services/users.py
+-rw-r--r--   0        0        0      773 2023-07-26 16:56:58.757727 computex_cli-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1974 1970-01-01 00:00:00.000000 computex_cli-0.1.8/PKG-INFO
```

### Comparing `computex_cli-0.1.7/README.md` & `computex_cli-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.7/cxcli/cli.py` & `computex_cli-0.1.8/cxcli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,36 +131,41 @@
     "--gpu", default="A40", help="The type of GPU you'd like to use."
 )  # TODO: Add listing of SKUs
 # @click.option(
 #     "--cpu", default="intel_xeon_v3", help="The type of CPU you'd like to use."
 # )
 @click.option("--memory", default=4, help="Memory in GB to allocate.")
 @click.option("--replicas", default=1, help="Number of replicas to use.")
+@click.option(
+    "--model-image", default=None, help="Reference to a published model image."
+)
 @refresh_credentials
 def deploy(
     app,
     image,
     num_cpu_cores,
     num_gpu,
     gpu,
     # cpu,
     memory,
     replicas,
+    model_image,
 ):
     # TODO: Verify that image exists before deployment.
     r = UserServiceV1().get_registry_credentials()
     r = DeployRequest(
         app_name=app,
         container_image=f"{r.registry_host}/{r.registry_namespace}/{image}",
         num_cpu_cores=num_cpu_cores,
         num_gpu=num_gpu,
         gpu=gpu,
         # cpu_sku=cpu_sku,
         memory=memory,
         replicas=replicas,
+        model_image=model_image,
     )
     DeploymentServiceV1().deploy(r)
     click.echo("Your app has successfully deployed.")
 
 
 @cli.command()
 @click.option("--app", help="Your app's name.")
@@ -184,41 +189,46 @@
 @click.option(
     "--min-scale", default=0, help="Minimum concurrent serverless invocations."
 )
 @click.option(
     "--max-scale", default=1, help="Maximum concurrent serverless invocations."
 )
 @click.option("--public", is_flag=True, default=False)
+@click.option(
+    "--model-image", default=None, help="Reference to a published model image."
+)
 @refresh_credentials
 def deploy_serverless(
     app: str,
     image: str,
     num_cpu_cores: int,
     num_gpu: int,
     gpu: str,
     # cpu: str,
     memory: int,
     concurrency: int,
     min_scale: int,
     max_scale: int,
     public: bool,
+    model_image: str,
 ):
     # TODO: Verify that image exists before deployment.
     r = UserServiceV1().get_registry_credentials()
     r = DeployServerlessRequest(
         app_name=app,
         container_image=f"{r.registry_host}/{r.registry_namespace}/{image}",
         num_cpu_cores=num_cpu_cores,
         num_gpu=num_gpu,
         gpu=gpu,
         # cpu_sku=cpu_sku,
         memory=memory,
         concurrency=concurrency,
         min_scale=min_scale,
         max_scale=max_scale,
+        model_image=model_image,
     )
     DeploymentServiceV1().deploy_serverless(r, is_public=public)
     click.echo("Your app has successfully deployed.")
 
 
 @cli.command()
 @refresh_credentials
```

### Comparing `computex_cli-0.1.7/cxcli/config.py` & `computex_cli-0.1.8/cxcli/config.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.7/cxcli/services/auth.py` & `computex_cli-0.1.8/cxcli/services/auth.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.7/cxcli/services/deployments.py` & `computex_cli-0.1.8/cxcli/services/deployments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Optional
 
 from pydantic import BaseModel
 
 from .service import CoreApiService
 
 
 class DeployRequest(BaseModel):
@@ -11,28 +11,30 @@
     num_cpu_cores: int
     num_gpu: int
     # TODO: Share SKU enums from main repo.
     gpu: str
     # cpu: str
     memory: int
     replicas: int
+    model_image: Optional[str]
 
 
 class DeployServerlessRequest(BaseModel):
     app_name: str
     container_image: str
     num_cpu_cores: int
     num_gpu: int
     # TODO: Share SKU enums from main repo.
     gpu: str
     # cpu: str
     memory: int
     concurrency: int = 1
     min_scale: int = 0
     max_scale: int = 10
+    model_image: Optional[str]
 
 
 class DeployResponse(BaseModel):
     app_name: str
 
 
 class DeleteResponse(BaseModel):
```

### Comparing `computex_cli-0.1.7/cxcli/services/service.py` & `computex_cli-0.1.8/cxcli/services/service.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.7/cxcli/services/users.py` & `computex_cli-0.1.8/cxcli/services/users.py`

 * *Files identical despite different names*

### Comparing `computex_cli-0.1.7/pyproject.toml` & `computex_cli-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "computex-cli"
-version = "0.1.7"
+version = "0.1.8"
 description = "ComputeX CLI tool"
 authors = ["Abate De Mey <abate@computex.ai>"]
 readme = "README.md"
 packages = [{include = "cxcli"}]
 include = ["pyproject.toml"]
 
 [tool.poetry.dependencies]
```

### Comparing `computex_cli-0.1.7/PKG-INFO` & `computex_cli-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: computex-cli
-Version: 0.1.7
+Version: 0.1.8
 Summary: ComputeX CLI tool
 Author: Abate De Mey
 Author-email: abate@computex.ai
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

