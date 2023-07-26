# Comparing `tmp/aiohttp_deps-0.3.0.tar.gz` & `tmp/aiohttp_deps-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_deps-0.3.0.tar", max compression
+gzip compressed data, was "aiohttp_deps-0.3.1.tar", max compression
```

## Comparing `aiohttp_deps-0.3.0.tar` & `aiohttp_deps-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/LICENSE
--rw-r--r--   0        0        0     9687 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/README.md
--rw-r--r--   0        0        0      539 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/__init__.py
--rw-r--r--   0        0        0     3265 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/initializer.py
--rw-r--r--   0        0        0        0 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/py.typed
--rw-r--r--   0        0        0     1250 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/router.py
--rw-r--r--   0        0        0      898 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/router.pyi
--rw-r--r--   0        0        0    11067 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/swagger.py
--rw-r--r--   0        0        0    10950 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/utils.py
--rw-r--r--   0        0        0     1385 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/aiohttp_deps/view.py
--rw-r--r--   0        0        0     1784 2023-07-25 18:14:04.763046 aiohttp_deps-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    10841 1970-01-01 00:00:00.000000 aiohttp_deps-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/LICENSE
+-rw-r--r--   0        0        0     9687 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/README.md
+-rw-r--r--   0        0        0      539 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/__init__.py
+-rw-r--r--   0        0        0     3265 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/initializer.py
+-rw-r--r--   0        0        0        0 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/py.typed
+-rw-r--r--   0        0        0     1250 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/router.py
+-rw-r--r--   0        0        0      898 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/router.pyi
+-rw-r--r--   0        0        0    12061 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/swagger.py
+-rw-r--r--   0        0        0    10950 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/utils.py
+-rw-r--r--   0        0        0     1385 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/aiohttp_deps/view.py
+-rw-r--r--   0        0        0     1784 2023-07-26 11:11:47.779408 aiohttp_deps-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    10841 1970-01-01 00:00:00.000000 aiohttp_deps-0.3.1/PKG-INFO
```

### Comparing `aiohttp_deps-0.3.0/LICENSE` & `aiohttp_deps-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.0/README.md` & `aiohttp_deps-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.0/aiohttp_deps/__init__.py` & `aiohttp_deps-0.3.1/aiohttp_deps/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.0/aiohttp_deps/initializer.py` & `aiohttp_deps-0.3.1/aiohttp_deps/initializer.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.0/aiohttp_deps/router.py` & `aiohttp_deps-0.3.1/aiohttp_deps/router.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.0/aiohttp_deps/router.pyi` & `aiohttp_deps-0.3.1/aiohttp_deps/router.pyi`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.0/aiohttp_deps/swagger.py` & `aiohttp_deps-0.3.1/aiohttp_deps/swagger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import inspect
 from collections import defaultdict
 from logging import getLogger
-from typing import Any, Awaitable, Callable, Dict, Optional, TypeVar, get_type_hints
+from typing import (
+    Any,
+    Awaitable,
+    Callable,
+    Dict,
+    Optional,
+    Tuple,
+    TypeVar,
+    get_type_hints,
+)
 
 import pydantic
 from aiohttp import web
 from deepmerge import always_merger
 from taskiq_dependencies import DependencyGraph
 
 from aiohttp_deps.initializer import InjectableFuncHandler, InjectableViewHandler
 from aiohttp_deps.utils import Form, Header, Json, Path, Query
 
 _T = TypeVar("_T")  # noqa: WPS111
 
+REF_TEMPLATE = "#/components/schemas/{model}"
 SCHEMA_KEY = "openapi_schema"
 SWAGGER_HTML_TEMPALTE = """
 <html lang="en">
 
 <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1" />
@@ -71,30 +81,34 @@
     def dummy(_var: annotation.annotation) -> None:  # type: ignore
         """Dummy function to use for type resolution."""
 
     var = get_type_hints(dummy).get("_var")
     return var == Optional[var]
 
 
-def _add_route_def(  # noqa: C901, WPS210
+def _add_route_def(  # noqa: C901, WPS210, WPS211
     openapi_schema: Dict[str, Any],
     route: web.ResourceRoute,
     method: str,
     graph: DependencyGraph,
     extra_openapi: Dict[str, Any],
+    extra_openapi_schemas: Dict[str, Any],
 ) -> None:
     route_info: Dict[str, Any] = {
         "description": inspect.getdoc(graph.target),
         "responses": {},
         "parameters": [],
     }
     if route.resource is None:  # pragma: no cover
         return
 
-    params: Dict[tuple[str, str], Any] = {}
+    if extra_openapi_schemas:
+        openapi_schema["components"]["schemas"].update(extra_openapi_schemas)
+
+    params: Dict[Tuple[str, str], Any] = {}
 
     def _insert_in_params(data: Dict[str, Any]) -> None:
         element = params.get((data["name"], data["in"]))
         if element is None:
             params[(data["name"], data["in"])] = data
             return
         element["required"] = element.get("required") or data.get("required")
@@ -110,17 +124,17 @@
                 content_type = "application/x-www-form-urlencoded"
             if (
                 dependency.signature
                 and dependency.signature.annotation != inspect.Parameter.empty
             ):
                 input_schema = pydantic.TypeAdapter(
                     dependency.signature.annotation,
-                ).json_schema()
+                ).json_schema(ref_template=REF_TEMPLATE)
                 openapi_schema["components"]["schemas"].update(
-                    input_schema.pop("definitions", {}),
+                    input_schema.pop("$defs", {}),
                 )
                 route_info["requestBody"] = {
                     "content": {content_type: {"schema": input_schema}},
                 }
             else:
                 route_info["requestBody"] = {
                     "content": {content_type: {}},
@@ -212,46 +226,55 @@
                 continue
             if isinstance(route._handler, InjectableFuncHandler):
                 extra_openapi = getattr(
                     route._handler.original_handler,
                     "__extra_openapi__",
                     {},
                 )
+                extra_schemas = getattr(
+                    route._handler.original_handler,
+                    "__extra_openapi_schemas__",
+                    {},
+                )
                 try:
                     _add_route_def(
                         openapi_schema,
                         route,  # type: ignore
                         route.method,
                         route._handler.graph,
                         extra_openapi=extra_openapi,
+                        extra_openapi_schemas=extra_schemas,
                     )
                 except Exception as exc:  # pragma: no cover
                     logger.warn(
                         "Cannot add route info: %s",
                         exc,
                         exc_info=True,
                     )
 
             elif isinstance(route._handler, InjectableViewHandler):
                 for key, graph in route._handler.graph_map.items():
                     extra_openapi = getattr(
-                        getattr(
-                            route._handler.original_handler,
-                            key,
-                        ),
+                        getattr(route._handler.original_handler, key),
                         "__extra_openapi__",
                         {},
                     )
+                    extra_schemas = getattr(
+                        getattr(route._handler.original_handler, key),
+                        "__extra_openapi_schemas__",
+                        {},
+                    )
                     try:
                         _add_route_def(
                             openapi_schema,
                             route,  # type: ignore
                             key,
                             graph,
                             extra_openapi=extra_openapi,
+                            extra_openapi_schemas=extra_schemas,
                         )
                     except Exception as exc:  # pragma: no cover
                         logger.warn(
                             "Cannot add route info: %s",
                             exc,
                             exc_info=True,
                         )
@@ -311,20 +334,24 @@
     :param description: Response's description.
 
     :returns: decorator that modifies your function.
     """
 
     def decorator(func: _T) -> _T:
         openapi = getattr(func, "__extra_openapi__", {})
+        openapi_schemas = getattr(func, "__extra_openapi_schemas__", {})
         adapter: "pydantic.TypeAdapter[Any]" = pydantic.TypeAdapter(model)
         responses = openapi.get("responses", {})
         status_response = responses.get(status, {})
         if not status_response:
             status_response["description"] = description
         status_response["content"] = status_response.get("content", {})
-        status_response["content"][content_type] = {"schema": adapter.json_schema()}
+        response_schema = adapter.json_schema(ref_template=REF_TEMPLATE)
+        openapi_schemas.update(response_schema.pop("$defs", {}))
+        status_response["content"][content_type] = {"schema": response_schema}
         responses[status] = status_response
         openapi["responses"] = responses
         func.__extra_openapi__ = openapi  # type: ignore
+        func.__extra_openapi_schemas__ = openapi_schemas  # type: ignore
         return func
 
     return decorator
```

### Comparing `aiohttp_deps-0.3.0/aiohttp_deps/utils.py` & `aiohttp_deps-0.3.1/aiohttp_deps/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.0/aiohttp_deps/view.py` & `aiohttp_deps-0.3.1/aiohttp_deps/view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_deps-0.3.0/pyproject.toml` & `aiohttp_deps-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "aiohttp-deps"
 description = "Dependency injection for AioHTTP"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.3.0"
+version = "0.3.1"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `aiohttp_deps-0.3.0/PKG-INFO` & `aiohttp_deps-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-deps
-Version: 0.3.0
+Version: 0.3.1
 Summary: Dependency injection for AioHTTP
 Home-page: https://github.com/taskiq-python/aiohttp-deps
 License: LICENSE
 Keywords: aiohttp,taskiq-dependencies
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
```

