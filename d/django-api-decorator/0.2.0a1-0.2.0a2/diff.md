# Comparing `tmp/django_api_decorator-0.2.0a1.tar.gz` & `tmp/django_api_decorator-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_api_decorator-0.2.0a1.tar", max compression
+gzip compressed data, was "django_api_decorator-0.2.0a2.tar", max compression
```

## Comparing `django_api_decorator-0.2.0a1.tar` & `django_api_decorator-0.2.0a2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-07-18 10:44:42.553767 django_api_decorator-0.2.0a1/LICENSE
--rw-r--r--   0        0        0      373 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/README.md
--rw-r--r--   0        0        0        0 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/__init__.py
--rw-r--r--   0        0        0      390 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/apps.py
--rw-r--r--   0        0        0    12218 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/decorators.py
--rw-r--r--   0        0        0        0 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/management/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/management/commands/generate_api_schemas.py
--rw-r--r--   0        0        0     8958 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/openapi.py
--rw-r--r--   0        0        0        0 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/py.typed
--rw-r--r--   0        0        0     1552 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/schema_file.py
--rw-r--r--   0        0        0     1037 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/types.py
--rw-r--r--   0        0        0     1993 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/django_api_decorator/utils.py
--rw-r--r--   0        0        0     1074 2023-07-18 10:44:42.557767 django_api_decorator-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 django_api_decorator-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0      373 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/__init__.py
+-rw-r--r--   0        0        0      390 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/apps.py
+-rw-r--r--   0        0        0    12218 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/decorators.py
+-rw-r--r--   0        0        0        0 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/management/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/management/commands/generate_api_schemas.py
+-rw-r--r--   0        0        0     9000 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/openapi.py
+-rw-r--r--   0        0        0        0 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/py.typed
+-rw-r--r--   0        0        0     1552 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/schema_file.py
+-rw-r--r--   0        0        0     1037 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/types.py
+-rw-r--r--   0        0        0     1993 2023-07-26 11:02:11.520817 django_api_decorator-0.2.0a2/django_api_decorator/utils.py
+-rw-r--r--   0        0        0     1074 2023-07-26 11:02:11.524817 django_api_decorator-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1033 1970-01-01 00:00:00.000000 django_api_decorator-0.2.0a2/PKG-INFO
```

### Comparing `django_api_decorator-0.2.0a1/LICENSE` & `django_api_decorator-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a1/django_api_decorator/decorators.py` & `django_api_decorator-0.2.0a2/django_api_decorator/decorators.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a1/django_api_decorator/management/commands/generate_api_schemas.py` & `django_api_decorator-0.2.0a2/django_api_decorator/management/commands/generate_api_schemas.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a1/django_api_decorator/openapi.py` & `django_api_decorator-0.2.0a2/django_api_decorator/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dataclasses
 import logging
 import re
+import textwrap
 from collections.abc import Callable, Sequence
 from typing import Any, cast
 
 import pydantic
 from django.http import HttpResponse
 from django.urls.resolvers import RoutePattern, URLPattern, URLResolver
 from pydantic_core import PydanticUndefined
@@ -134,35 +135,35 @@
     path, parameters = django_path_to_openapi_url_and_parameters(resolved_url)
 
     for name, field in api_meta.query_params_model.model_fields.items():
         schema = pydantic.TypeAdapter(field.annotation).json_schema(
             ref_template=schema_ref
         )
         schema = to_ref_if_object(schema)
+        if field.default != PydanticUndefined:
+            schema["default"] = field.default
 
         param = {
             "name": field.alias or name,
             "in": "query",
             "required": field.is_required(),
             "schema": schema,
         }
-        if field.default != PydanticUndefined:
-            param["default"] = field.default
         parameters.append(param)
 
     # Assuming standard django folder structure with [project name]/[app name]/....
     app_name = callback.__module__.split(".")[1]
 
     paths = {
         path: {
             api_meta.method.lower(): {
                 "operationId": view_name,
                 # Note: We could consider allowing users to pass a description into
                 # @api() instead of using the function docstring.
-                "description": callback.__doc__ or "",
+                "description": textwrap.dedent(callback.__doc__ or "").strip(),
                 # Tags are useful for grouping operations in codegen
                 "tags": [app_name],
                 "parameters": parameters,
                 **request_body,
                 "responses": {
                     api_meta.response_status: {
                         "description": "",
@@ -257,15 +258,15 @@
             if path in api_paths:
                 # Merge operations that have the same URL but different http methods
                 api_paths[path].update(val)
             else:
                 api_paths[path] = val
 
     api_spec = {
-        "openapi": "3.0.0",
+        "openapi": "3.1.0",
         "info": {"title": "API overview", "version": "0.0.1"},
         "paths": api_paths,
         "components": {"schemas": api_components},
     }
 
     logger.info(
         "Generated %s paths and %s schemas", len(api_paths), len(api_components)
```

### Comparing `django_api_decorator-0.2.0a1/django_api_decorator/schema_file.py` & `django_api_decorator-0.2.0a2/django_api_decorator/schema_file.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a1/django_api_decorator/types.py` & `django_api_decorator-0.2.0a2/django_api_decorator/types.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a1/django_api_decorator/utils.py` & `django_api_decorator-0.2.0a2/django_api_decorator/utils.py`

 * *Files identical despite different names*

### Comparing `django_api_decorator-0.2.0a1/pyproject.toml` & `django_api_decorator-0.2.0a2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-api-decorator"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = "A collection of tools to build function based Django APIs"
 authors = ["Oda <tech@oda.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kolonialno/django-api-decorator"
 repository = "https://github.com/kolonialno/django-api-decorator"
 packages = [{include = "django_api_decorator"}]
```

### Comparing `django_api_decorator-0.2.0a1/PKG-INFO` & `django_api_decorator-0.2.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-api-decorator
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: A collection of tools to build function based Django APIs
 Home-page: https://github.com/kolonialno/django-api-decorator
 License: MIT
 Author: Oda
 Author-email: tech@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

