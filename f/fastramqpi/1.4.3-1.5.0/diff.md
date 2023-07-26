# Comparing `tmp/fastramqpi-1.4.3.tar.gz` & `tmp/fastramqpi-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastramqpi-1.4.3.tar", max compression
+gzip compressed data, was "fastramqpi-1.5.0.tar", max compression
```

## Comparing `fastramqpi-1.4.3.tar` & `fastramqpi-1.5.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0        0        0        0 2023-06-02 13:35:23.336033 fastramqpi-1.4.3/LICENSES/
--rw-r--r--   0        0        0    15177 2023-06-02 13:35:23.336033 fastramqpi-1.4.3/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0     2932 2023-06-02 13:35:23.336033 fastramqpi-1.4.3/README.md
--rw-r--r--   0        0        0       85 2023-06-02 13:35:23.336033 fastramqpi-1.4.3/fastramqpi/__init__.py
--rw-r--r--   0        0        0     2206 2023-06-02 13:35:23.336033 fastramqpi-1.4.3/fastramqpi/config.py
--rw-r--r--   0        0        0     1144 2023-06-02 13:35:23.337033 fastramqpi-1.4.3/fastramqpi/context.py
--rw-r--r--   0        0        0     7100 2023-06-02 13:35:23.337033 fastramqpi-1.4.3/fastramqpi/fastapi.py
--rw-r--r--   0        0        0     1577 2023-06-02 13:35:23.337033 fastramqpi-1.4.3/fastramqpi/healthcheck.py
--rw-r--r--   0        0        0     3930 2023-06-02 13:35:23.337033 fastramqpi-1.4.3/fastramqpi/main.py
--rw-r--r--   0        0        0        0 2023-06-02 13:35:23.379037 fastramqpi-1.4.3/fastramqpi/py.typed
--rw-r--r--   0        0        0     1390 2023-06-02 13:35:36.797252 fastramqpi-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     3891 1970-01-01 00:00:00.000000 fastramqpi-1.4.3/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-07-26 15:18:33.939393 fastramqpi-1.5.0/LICENSES/
+-rw-r--r--   0        0        0    15177 2023-07-26 15:18:33.940393 fastramqpi-1.5.0/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0     6602 2023-07-26 15:18:33.940393 fastramqpi-1.5.0/README.md
+-rw-r--r--   0        0        0       85 2023-07-26 15:18:33.940393 fastramqpi-1.5.0/fastramqpi/__init__.py
+-rw-r--r--   0        0        0     2206 2023-07-26 15:18:33.940393 fastramqpi-1.5.0/fastramqpi/config.py
+-rw-r--r--   0        0        0     1298 2023-07-26 15:18:33.940393 fastramqpi-1.5.0/fastramqpi/context.py
+-rw-r--r--   0        0        0     1425 2023-07-26 15:18:33.941393 fastramqpi-1.5.0/fastramqpi/depends.py
+-rw-r--r--   0        0        0     7100 2023-07-26 15:18:33.941393 fastramqpi-1.5.0/fastramqpi/fastapi.py
+-rw-r--r--   0        0        0     1577 2023-07-26 15:18:33.941393 fastramqpi-1.5.0/fastramqpi/healthcheck.py
+-rw-r--r--   0        0        0     6935 2023-07-26 15:18:33.941393 fastramqpi-1.5.0/fastramqpi/main.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:18:33.985397 fastramqpi-1.5.0/fastramqpi/py.typed
+-rw-r--r--   0        0        0     1587 2023-07-26 15:18:46.849581 fastramqpi-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7561 1970-01-01 00:00:00.000000 fastramqpi-1.5.0/PKG-INFO
```

### Comparing `fastramqpi-1.4.3/LICENSES/MPL-2.0.txt` & `fastramqpi-1.5.0/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.3/fastramqpi/config.py` & `fastramqpi-1.5.0/fastramqpi/config.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.3/fastramqpi/context.py` & `fastramqpi-1.5.0/fastramqpi/context.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """FastRAMQPI Context."""
 from typing import Any
 from typing import AsyncContextManager
 from typing import Awaitable
 from typing import Callable
 from typing import TypedDict
 
+from authlib.integrations.httpx_client import AsyncOAuth2Client
 from fastapi import FastAPI
 from gql.client import AsyncClientSession
 from pydantic import BaseSettings
 from raclients.graph.client import GraphQLClient
 from raclients.modelclient.mo import ModelClient
 from ramqp.mo import MOAMQPSystem
 
@@ -26,11 +27,17 @@
     name: str
     settings: BaseSettings
     # The type is perfectly in order, but mypy cannot handle recursive types
     healthchecks: dict[str, HealthcheckFunction]  # type: ignore
     lifespan_managers: dict[int, set[AsyncContextManager]]
     app: FastAPI
     amqpsystem: MOAMQPSystem
+
+    # Legacy clients
     graphql_client: GraphQLClient
     graphql_session: AsyncClientSession
     model_client: ModelClient
+
+    # Authenticated HTTPX Client
+    mo_client: AsyncOAuth2Client
+
     user_context: dict[str, Any]
```

### Comparing `fastramqpi-1.4.3/fastramqpi/fastapi.py` & `fastramqpi-1.5.0/fastramqpi/fastapi.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.3/fastramqpi/healthcheck.py` & `fastramqpi-1.5.0/fastramqpi/healthcheck.py`

 * *Files identical despite different names*

### Comparing `fastramqpi-1.4.3/pyproject.toml` & `fastramqpi-1.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2019-2020 Magenta ApS
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "FastRAMQPI"
-version = "1.4.3"
+version = "1.5.0"
 description = "Rammearkitektur AMQP framework (FastAPI + RAMQP)"
 authors = ["Magenta ApS <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/FastRAMQPI"
 keywords = ["os2mo", "amqp"]
@@ -45,12 +45,17 @@
 python_version = "3.10"
 warn_return_any = "True"
 warn_unused_configs = "True"
 check_untyped_defs = "True"
 disallow_untyped_defs = "True"
 plugins = "pydantic.mypy"
 
+[[tool.mypy.overrides]]
+# The module seems to be missing library stubs or py.typed marker
+module = "authlib.integrations.httpx_client"
+ignore_missing_imports = true
+
 [tool.flake8]
-max-line-length = 88
+max-line-length = 999  # let black worry about that
 exclude = [
 ".git", "__pycache__", ".mypy_cache", ".pytest_cache", ".venv", ".gitlab"
 ]
```

