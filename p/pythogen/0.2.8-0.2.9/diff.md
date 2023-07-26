# Comparing `tmp/pythogen-0.2.8.tar.gz` & `tmp/pythogen-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythogen-0.2.8.tar", max compression
+gzip compressed data, was "pythogen-0.2.9.tar", max compression
```

## Comparing `pythogen-0.2.8.tar` & `pythogen-0.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1069 2023-07-25 15:38:38.807537 pythogen-0.2.8/LICENSE
--rw-r--r--   0        0        0     2206 2023-07-25 15:38:38.807537 pythogen-0.2.8/README.md
--rw-r--r--   0        0        0     1650 2023-07-25 15:38:38.811537 pythogen-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/__init__.py
--rwxr-xr-x   0        0        0     1730 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/main.py
--rw-r--r--   0        0        0     7660 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/models.py
--rw-r--r--   0        0        0     2355 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/packager.py
--rw-r--r--   0        0        0      102 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/constants.py
--rw-r--r--   0        0        0     3307 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/document.py
--rw-r--r--   0        0        0      576 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/inline_schemas_aggregator.py
--rw-r--r--   0        0        0     3669 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/operations.py
--rw-r--r--   0        0        0     2132 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/parameters.py
--rw-r--r--   0        0        0     2437 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/paths.py
--rw-r--r--   0        0        0     1074 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/references.py
--rw-r--r--   0        0        0     3512 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/request_body.py
--rw-r--r--   0        0        0     1810 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/response.py
--rw-r--r--   0        0        0    17663 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/parsers/schemas.py
--rw-r--r--   0        0        0    10836 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/renderer.py
--rw-r--r--   0        0        0      286 2023-07-25 15:38:38.811537 pythogen-0.2.8/pythogen/settings.py
--rw-r--r--   0        0        0    10789 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client/main.j2
--rw-r--r--   0        0        0     4320 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client/method.j2
--rw-r--r--   0        0        0     2487 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client/operation_params_schemas.j2
--rw-r--r--   0        0        0     1471 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client/request-metrics.j2
--rw-r--r--   0        0        0       33 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client_package/init-py.j2
--rw-r--r--   0        0        0      312 2023-07-25 15:38:38.815537 pythogen-0.2.8/pythogen/templates/http_client_package/pyproject-toml.j2
--rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 pythogen-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-26 12:30:59.142498 pythogen-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2206 2023-07-26 12:30:59.142498 pythogen-0.2.9/README.md
+-rw-r--r--   0        0        0     1644 2023-07-26 12:30:59.146498 pythogen-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/__init__.py
+-rwxr-xr-x   0        0        0     1771 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/main.py
+-rw-r--r--   0        0        0     7660 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/models.py
+-rw-r--r--   0        0        0     2355 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/packager.py
+-rw-r--r--   0        0        0      102 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/parsers/constants.py
+-rw-r--r--   0        0        0     3307 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/parsers/document.py
+-rw-r--r--   0        0        0      576 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/parsers/inline_schemas_aggregator.py
+-rw-r--r--   0        0        0     3669 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/parsers/operations.py
+-rw-r--r--   0        0        0     2132 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/parsers/parameters.py
+-rw-r--r--   0        0        0     2437 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/parsers/paths.py
+-rw-r--r--   0        0        0     1074 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/parsers/references.py
+-rw-r--r--   0        0        0     3512 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/parsers/request_body.py
+-rw-r--r--   0        0        0     1810 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/parsers/response.py
+-rw-r--r--   0        0        0    17663 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/parsers/schemas.py
+-rw-r--r--   0        0        0    10836 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/renderer.py
+-rw-r--r--   0        0        0      286 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/settings.py
+-rw-r--r--   0        0        0    10789 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/templates/http_client/main.j2
+-rw-r--r--   0        0        0     4320 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/templates/http_client/method.j2
+-rw-r--r--   0        0        0     2487 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/templates/http_client/operation_params_schemas.j2
+-rw-r--r--   0        0        0     1471 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/templates/http_client/request-metrics.j2
+-rw-r--r--   0        0        0       33 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/templates/http_client_package/init-py.j2
+-rw-r--r--   0        0        0      312 2023-07-26 12:30:59.146498 pythogen-0.2.9/pythogen/templates/http_client_package/pyproject-toml.j2
+-rw-r--r--   0        0        0     3634 1970-01-01 00:00:00.000000 pythogen-0.2.9/PKG-INFO
```

### Comparing `pythogen-0.2.8/LICENSE` & `pythogen-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/README.md` & `pythogen-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pyproject.toml` & `pythogen-0.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythogen"
-version = "0.2.8"
+version = "0.2.9"
 description = "Generator of python HTTP-clients from OpenApi specification."
 homepage = "https://github.com/artsmolin/pythogen"
 repository = "https://github.com/artsmolin/pythogen"
 authors = [
     "Artur Smolin <artursmolin@outlook.com>",
     "Vladimir Vyazovetskov <erhosen@gmail.com>",
     "Evgeny Solomatin <solgenya@gmail.com>",
@@ -40,15 +40,15 @@
 autoflake = "^2.2.0"
 isort = "^5.12.0"
 pydantic = "^2.0.2"
 pytest-cov = "^4.1.0"
 openapi-spec-validator = "^0.6.0"
 
 [tool.poetry.scripts]
-pythogen = 'pythogen.entrypoint:run'
+pythogen = 'pythogen.main:run'
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 importlib-metadata = "^4.11.4"
 pre-commit = "^2.19.0"
```

### Comparing `pythogen-0.2.8/pythogen/main.py` & `pythogen-0.2.9/pythogen/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,9 +51,13 @@
         name=name,
         sync=sync,
         metrics=metrics,
         required_headers=headers.split(",") if headers else None,
     )
 
 
+def run() -> None:
+    typer.run(main)
+
+
 if __name__ == '__main__':
     app()
```

### Comparing `pythogen-0.2.8/pythogen/models.py` & `pythogen-0.2.9/pythogen/models.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/packager.py` & `pythogen-0.2.9/pythogen/packager.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/parsers/document.py` & `pythogen-0.2.9/pythogen/parsers/document.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/parsers/inline_schemas_aggregator.py` & `pythogen-0.2.9/pythogen/parsers/inline_schemas_aggregator.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/parsers/operations.py` & `pythogen-0.2.9/pythogen/parsers/operations.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/parsers/parameters.py` & `pythogen-0.2.9/pythogen/parsers/parameters.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/parsers/paths.py` & `pythogen-0.2.9/pythogen/parsers/paths.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/parsers/references.py` & `pythogen-0.2.9/pythogen/parsers/references.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/parsers/request_body.py` & `pythogen-0.2.9/pythogen/parsers/request_body.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/parsers/response.py` & `pythogen-0.2.9/pythogen/parsers/response.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/parsers/schemas.py` & `pythogen-0.2.9/pythogen/parsers/schemas.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/renderer.py` & `pythogen-0.2.9/pythogen/renderer.py`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/templates/http_client/main.j2` & `pythogen-0.2.9/pythogen/templates/http_client/main.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/templates/http_client/method.j2` & `pythogen-0.2.9/pythogen/templates/http_client/method.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/templates/http_client/operation_params_schemas.j2` & `pythogen-0.2.9/pythogen/templates/http_client/operation_params_schemas.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/pythogen/templates/http_client/request-metrics.j2` & `pythogen-0.2.9/pythogen/templates/http_client/request-metrics.j2`

 * *Files identical despite different names*

### Comparing `pythogen-0.2.8/PKG-INFO` & `pythogen-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythogen
-Version: 0.2.8
+Version: 0.2.9
 Summary: Generator of python HTTP-clients from OpenApi specification.
 Home-page: https://github.com/artsmolin/pythogen
 License: MIT
 Keywords: openapi,openapi-generator,swagger,http-client,generator
 Author: Artur Smolin
 Author-email: artursmolin@outlook.com
 Requires-Python: >=3.10,<4.0
```

