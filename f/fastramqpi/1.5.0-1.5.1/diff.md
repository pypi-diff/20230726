# Comparing `tmp/fastramqpi-1.5.0.tar.gz` & `tmp/fastramqpi-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastramqpi-1.5.0.tar", max compression
+gzip compressed data, was "fastramqpi-1.5.1.tar", max compression
```

## Comparing `fastramqpi-1.5.0.tar` & `fastramqpi-1.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0        0        0        0 2023-07-26 15:18:33.939393 fastramqpi-1.5.0/LICENSES/
--rw-r--r--   0        0        0    15177 2023-07-26 15:18:33.940393 fastramqpi-1.5.0/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     6602 2023-07-26 15:18:33.940393 fastramqpi-1.5.0/README.md
--rw-r--r--   0        0        0       85 2023-07-26 15:18:33.940393 fastramqpi-1.5.0/fastramqpi/__init__.py
--rw-r--r--   0        0        0     2206 2023-07-26 15:18:33.940393 fastramqpi-1.5.0/fastramqpi/config.py
--rw-r--r--   0        0        0     1298 2023-07-26 15:18:33.940393 fastramqpi-1.5.0/fastramqpi/context.py
--rw-r--r--   0        0        0     1425 2023-07-26 15:18:33.941393 fastramqpi-1.5.0/fastramqpi/depends.py
--rw-r--r--   0        0        0     7100 2023-07-26 15:18:33.941393 fastramqpi-1.5.0/fastramqpi/fastapi.py
--rw-r--r--   0        0        0     1577 2023-07-26 15:18:33.941393 fastramqpi-1.5.0/fastramqpi/healthcheck.py
--rw-r--r--   0        0        0     6935 2023-07-26 15:18:33.941393 fastramqpi-1.5.0/fastramqpi/main.py
--rw-r--r--   0        0        0        0 2023-07-26 15:18:33.985397 fastramqpi-1.5.0/fastramqpi/py.typed
--rw-r--r--   0        0        0     1587 2023-07-26 15:18:46.849581 fastramqpi-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     7561 1970-01-01 00:00:00.000000 fastramqpi-1.5.0/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-07-26 15:20:45.429331 fastramqpi-1.5.1/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-07-26 15:20:45.430331 fastramqpi-1.5.1/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     6602 2023-07-26 15:20:45.430331 fastramqpi-1.5.1/README.md
+-rw-r--r--   0        0        0       85 2023-07-26 15:20:45.430331 fastramqpi-1.5.1/fastramqpi/__init__.py
+-rw-r--r--   0        0        0     2206 2023-07-26 15:20:45.430331 fastramqpi-1.5.1/fastramqpi/config.py
+-rw-r--r--   0        0        0     1298 2023-07-26 15:20:45.430331 fastramqpi-1.5.1/fastramqpi/context.py
+-rw-r--r--   0        0        0     1425 2023-07-26 15:20:45.431331 fastramqpi-1.5.1/fastramqpi/depends.py
+-rw-r--r--   0        0        0     7150 2023-07-26 15:20:45.431331 fastramqpi-1.5.1/fastramqpi/fastapi.py
+-rw-r--r--   0        0        0     1577 2023-07-26 15:20:45.431331 fastramqpi-1.5.1/fastramqpi/healthcheck.py
+-rw-r--r--   0        0        0     6935 2023-07-26 15:20:45.431331 fastramqpi-1.5.1/fastramqpi/main.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:20:45.477335 fastramqpi-1.5.1/fastramqpi/py.typed
+-rw-r--r--   0        0        0     1587 2023-07-26 15:20:59.364335 fastramqpi-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7561 1970-01-01 00:00:00.000000 fastramqpi-1.5.1/PKG-INFO
```

### Comparing `fastramqpi-1.5.0/LICENSES/MPL-2.0.txt` & `fastramqpi-1.5.1/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.0/README.md` & `fastramqpi-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.0/fastramqpi/config.py` & `fastramqpi-1.5.1/fastramqpi/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.0/fastramqpi/context.py` & `fastramqpi-1.5.1/fastramqpi/context.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.0/fastramqpi/depends.py` & `fastramqpi-1.5.1/fastramqpi/depends.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.0/fastramqpi/fastapi.py` & `fastramqpi-1.5.1/fastramqpi/fastapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,30 +64,31 @@
 @fastapi_router.get("/")
 async def index(request: Request) -> dict[str, str]:
     """Endpoint to return name of integration."""
     context: dict[str, Any] = request.app.state.context
     return {"name": context["name"]}
 
 
-@fastapi_router.get("/health/live", status_code=HTTP_204_NO_CONTENT)
-async def liveness() -> None:
-    """Endpoint to be used as a liveness probe for Kubernetes."""
+@fastapi_router.get("/health/ready", status_code=HTTP_204_NO_CONTENT)
+async def readiness() -> None:
+    """Endpoint to be used as a readiness probe for Kubernetes."""
+    # TODO: Remove once everyone is using v1.4.3+
     return None
 
 
 @fastapi_router.get(
-    "/health/ready",
+    "/health/live",
     status_code=HTTP_204_NO_CONTENT,
     responses={
         "204": {"description": "Ready"},
         "503": {"description": "Not ready"},
     },
 )
-async def readiness(request: Request, response: Response) -> Response:
-    """Endpoint to be used as a readiness probe for Kubernetes."""
+async def liveness(request: Request, response: Response) -> Response:
+    """Endpoint to be used as a liveness probe for Kubernetes."""
     response.status_code = HTTP_204_NO_CONTENT
 
     context: dict[str, Any] = request.app.state.context
     healthchecks = context["healthchecks"]
     all_ready = True
     try:
         for name, healthcheck in healthchecks.items():
```

### Comparing `fastramqpi-1.5.0/fastramqpi/healthcheck.py` & `fastramqpi-1.5.1/fastramqpi/healthcheck.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.0/fastramqpi/main.py` & `fastramqpi-1.5.1/fastramqpi/main.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.5.0/pyproject.toml` & `fastramqpi-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "FastRAMQPI"
-version = "1.5.0"
+version = "1.5.1"
 description = "Rammearkitektur AMQP framework (FastAPI + RAMQP)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/FastRAMQPI"
 keywords = ["os2mo", "amqp"]
```

### Comparing `fastramqpi-1.5.0/PKG-INFO` & `fastramqpi-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastramqpi
-Version: 1.5.0
+Version: 1.5.1
 Summary: Rammearkitektur AMQP framework (FastAPI + RAMQP)
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,amqp
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
```

