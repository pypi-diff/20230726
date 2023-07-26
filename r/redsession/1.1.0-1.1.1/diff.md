# Comparing `tmp/redsession-1.1.0.tar.gz` & `tmp/redsession-1.1.1.tar.gz`

## Comparing `redsession-1.1.0.tar` & `redsession-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 redsession-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 redsession-1.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 redsession-1.1.0/requirements-docs.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 redsession-1.1.0/requirements-tests.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 redsession-1.1.0/requirements.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 redsession-1.1.0/redsession/__init__.py
--rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 redsession-1.1.0/redsession/middleware.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 redsession-1.1.0/redsession/backend/__init__.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 redsession-1.1.0/redsession/backend/base.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 redsession-1.1.0/redsession/backend/redis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redsession-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 redsession-1.1.0/tests/test_session.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 redsession-1.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 redsession-1.1.0/LICENSE.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 redsession-1.1.0/README.rst
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 redsession-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 redsession-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 redsession-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 redsession-1.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 redsession-1.1.1/requirements-docs.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 redsession-1.1.1/requirements-tests.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 redsession-1.1.1/requirements.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 redsession-1.1.1/redsession/__init__.py
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 redsession-1.1.1/redsession/middleware.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 redsession-1.1.1/redsession/backend/__init__.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 redsession-1.1.1/redsession/backend/base.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 redsession-1.1.1/redsession/backend/redis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redsession-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3872 2020-02-02 00:00:00.000000 redsession-1.1.1/tests/test_session.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 redsession-1.1.1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 redsession-1.1.1/LICENSE.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 redsession-1.1.1/README.rst
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 redsession-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 redsession-1.1.1/PKG-INFO
```

### Comparing `redsession-1.1.0/.pre-commit-config.yaml` & `redsession-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `redsession-1.1.0/.readthedocs.yaml` & `redsession-1.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `redsession-1.1.0/redsession/middleware.py` & `redsession-1.1.1/redsession/middleware.py`

 * *Files identical despite different names*

### Comparing `redsession-1.1.0/redsession/backend/base.py` & `redsession-1.1.1/redsession/backend/base.py`

 * *Files identical despite different names*

### Comparing `redsession-1.1.0/redsession/backend/redis.py` & `redsession-1.1.1/redsession/backend/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class RedisBackend(BaseAsyncBackend):
     """
     This class is used to connect and interact with Redis.
 
     Args:
-        redis (:class:`redis.asyncio.Redis`): Redis client.
+        redis (:obj:`redis.asyncio.Redis`): Async Redis client.
     """
 
     def __init__(self, redis: "Redis[Any]") -> None:
         self.redis = redis
 
     async def get(self, key: str) -> Optional[Dict[str, Any]]:
         data = await self.redis.get(key)
```

### Comparing `redsession-1.1.0/tests/test_session.py` & `redsession-1.1.1/tests/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import pytest
-
-from starlette.requests import Request
-from starlette.testclient import TestClient
-from starlette.responses import JSONResponse
-from starlette.applications import Starlette
-
 from httpx import Cookies
 from fakeredis import aioredis
+from starlette.applications import Starlette
+from starlette.requests import Request
+from starlette.responses import JSONResponse
+from starlette.testclient import TestClient
 
 from redsession import ServerSessionMiddleware
 from redsession.backend import RedisBackend
 
 
 async def set_session(request: Request):
     request.session.update({"id": 1})
```

### Comparing `redsession-1.1.0/LICENSE.md` & `redsession-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redsession-1.1.0/README.rst` & `redsession-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `redsession-1.1.0/pyproject.toml` & `redsession-1.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "redsession"
 authors = [{ name = "TheJecksMan" }]
-description = "Simple and fastest library for Redis server sessions"
+description = "Simple and fast server session middleware for FastAPI and Starlette"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = "MIT"
 classifiers = [
     "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -30,15 +29,31 @@
     "itsdangerous>=2.1.2",
     "redis[hiredis]>=4.6.0",
     "orjson>=3.9.0",
 ]
 
 [project.urls]
 Repository = "https://github.com/TheJecksMan/red-session"
+Issues = "https://github.com/TheJecksMan/red-session/issues"
 Docs = "https://red-session.readthedocs.io/en/stable/"
 
-
 [tool.hatch.version]
 path = "redsession/__init__.py"
 
 [tool.hatch.build.targets.sdist]
 exclude = ["/.github", "/docs", "/examples"]
+
+[tool.mypy]
+strict = true
+
+[tool.ruff]
+select = [
+    "E", # pycodestyle errors
+    "W", # pycodestyle warnings
+    "F", # pyflakes
+    "I", # isort
+    "B", # flake8-bugbear
+]
+
+[tool.ruff.per-file-ignores]
+"examples/fastapi.py" = ["I001"]
+"examples/starlette.py" = ["I001"]
```

### Comparing `redsession-1.1.0/PKG-INFO` & `redsession-1.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: redsession
-Version: 1.1.0
-Summary: Simple and fastest library for Redis server sessions
+Version: 1.1.1
+Summary: Simple and fast server session middleware for FastAPI and Starlette
 Project-URL: Repository, https://github.com/TheJecksMan/red-session
+Project-URL: Issues, https://github.com/TheJecksMan/red-session/issues
 Project-URL: Docs, https://red-session.readthedocs.io/en/stable/
 Author: TheJecksMan
 License-Expression: MIT
 License-File: LICENSE.md
-Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: FastAPI
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
```

