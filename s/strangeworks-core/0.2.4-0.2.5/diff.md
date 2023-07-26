# Comparing `tmp/strangeworks_core-0.2.4.tar.gz` & `tmp/strangeworks_core-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_core-0.2.4.tar", max compression
+gzip compressed data, was "strangeworks_core-0.2.5.tar", max compression
```

## Comparing `strangeworks_core-0.2.4.tar` & `strangeworks_core-0.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      655 2023-07-25 15:12:12.228810 strangeworks_core-0.2.4/README.md
--rw-r--r--   0        0        0      914 2023-07-25 15:12:29.777008 strangeworks_core-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      109 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/__init__.py
--rw-r--r--   0        0        0       19 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/batch/__init__.py
--rw-r--r--   0        0        0    13604 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/batch/utils.py
--rw-r--r--   0        0        0       19 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/__init__.py
--rw-r--r--   0        0        0      647 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/base.py
--rw-r--r--   0        0        0     3340 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/config.py
--rw-r--r--   0        0        0      874 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/defaults.py
--rw-r--r--   0        0        0     1846 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/env.py
--rw-r--r--   0        0        0     6262 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/config/file.py
--rw-r--r--   0        0        0       19 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/errors/__init__.py
--rw-r--r--   0        0        0     2613 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/errors/error.py
--rw-r--r--   0        0        0       19 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/platform/__init__.py
--rw-r--r--   0        0        0     2457 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/platform/auth.py
--rw-r--r--   0        0        0     4880 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/platform/gql.py
--rw-r--r--   0        0        0    10844 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/platform/rest_client.py
--rw-r--r--   0        0        0     3275 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/platform/transport.py
--rw-r--r--   0        0        0       19 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/__init__.py
--rw-r--r--   0        0        0     3572 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/backend.py
--rw-r--r--   0        0        0      558 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/batch.py
--rw-r--r--   0        0        0     2024 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/file.py
--rw-r--r--   0        0        0      647 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/func.py
--rw-r--r--   0        0        0     6749 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/job.py
--rw-r--r--   0        0        0      760 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/machine.py
--rw-r--r--   0        0        0     1088 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/product.py
--rw-r--r--   0        0        0     2732 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/types/resource.py
--rw-r--r--   0        0        0      553 2023-07-25 15:12:12.232810 strangeworks_core-0.2.4/strangeworks_core/utils.py
--rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 strangeworks_core-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      655 2023-07-26 20:50:29.287334 strangeworks_core-0.2.5/README.md
+-rw-r--r--   0        0        0      914 2023-07-26 20:50:47.267563 strangeworks_core-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      109 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/__init__.py
+-rw-r--r--   0        0        0       19 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/batch/__init__.py
+-rw-r--r--   0        0        0    13789 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/batch/utils.py
+-rw-r--r--   0        0        0       19 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/config/__init__.py
+-rw-r--r--   0        0        0      647 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/config/base.py
+-rw-r--r--   0        0        0     3340 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/config/config.py
+-rw-r--r--   0        0        0      874 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/config/defaults.py
+-rw-r--r--   0        0        0     1846 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/config/env.py
+-rw-r--r--   0        0        0     6262 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/config/file.py
+-rw-r--r--   0        0        0       19 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/errors/__init__.py
+-rw-r--r--   0        0        0     2613 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/errors/error.py
+-rw-r--r--   0        0        0       19 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/platform/__init__.py
+-rw-r--r--   0        0        0     2457 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/platform/auth.py
+-rw-r--r--   0        0        0     4880 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/platform/gql.py
+-rw-r--r--   0        0        0    10844 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/platform/rest_client.py
+-rw-r--r--   0        0        0     3275 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/platform/transport.py
+-rw-r--r--   0        0        0       19 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/types/__init__.py
+-rw-r--r--   0        0        0     3572 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/types/backend.py
+-rw-r--r--   0        0        0      558 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/types/batch.py
+-rw-r--r--   0        0        0     2024 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/types/file.py
+-rw-r--r--   0        0        0      647 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/types/func.py
+-rw-r--r--   0        0        0     6749 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/types/job.py
+-rw-r--r--   0        0        0      760 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/types/machine.py
+-rw-r--r--   0        0        0     1088 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/types/product.py
+-rw-r--r--   0        0        0     2732 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/types/resource.py
+-rw-r--r--   0        0        0      553 2023-07-26 20:50:29.291334 strangeworks_core-0.2.5/strangeworks_core/utils.py
+-rw-r--r--   0        0        0     1464 1970-01-01 00:00:00.000000 strangeworks_core-0.2.5/PKG-INFO
```

### Comparing `strangeworks_core-0.2.4/README.md` & `strangeworks_core-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/pyproject.toml` & `strangeworks_core-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "strangeworks-core"
-version = "0.2.4"
+version = "0.2.5"
 
 description = "Strangeworks Core provides the infrastructure to interact with the platform."
 authors = ["Strange Devs <hello@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_core"}]
 license = "Apache-2.0"
```

### Comparing `strangeworks_core-0.2.4/strangeworks_core/batch/utils.py` & `strangeworks_core-0.2.5/strangeworks_core/batch/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,19 @@
         parsed = ast.parse(func_source)
         for node in ast.iter_child_nodes(parsed):
             if isinstance(node, ast.FunctionDef) and node.name == func_name:
                 decorator_index = None
                 for index, decorator in enumerate(node.decorator_list):
                     id = None
                     if isinstance(decorator, ast.Call):
-                        id = decorator.func.id
+                        f = decorator.func
+                        if isinstance(f, ast.Name):
+                            id = f.id
+                        elif isinstance(f, ast.Attribute):
+                            id = f.attr
                     elif isinstance(decorator, ast.Name):
                         id = decorator.id
 
                     if id and id == decorator_name:
                         decorator_index = index
                         break
                 if decorator_index is not None:
```

### Comparing `strangeworks_core-0.2.4/strangeworks_core/config/base.py` & `strangeworks_core-0.2.5/strangeworks_core/config/base.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/config/config.py` & `strangeworks_core-0.2.5/strangeworks_core/config/config.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/config/defaults.py` & `strangeworks_core-0.2.5/strangeworks_core/config/defaults.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/config/env.py` & `strangeworks_core-0.2.5/strangeworks_core/config/env.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/config/file.py` & `strangeworks_core-0.2.5/strangeworks_core/config/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/errors/error.py` & `strangeworks_core-0.2.5/strangeworks_core/errors/error.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/platform/auth.py` & `strangeworks_core-0.2.5/strangeworks_core/platform/auth.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/platform/gql.py` & `strangeworks_core-0.2.5/strangeworks_core/platform/gql.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/platform/rest_client.py` & `strangeworks_core-0.2.5/strangeworks_core/platform/rest_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/platform/transport.py` & `strangeworks_core-0.2.5/strangeworks_core/platform/transport.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/types/backend.py` & `strangeworks_core-0.2.5/strangeworks_core/types/backend.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/types/batch.py` & `strangeworks_core-0.2.5/strangeworks_core/types/batch.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/types/file.py` & `strangeworks_core-0.2.5/strangeworks_core/types/file.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/types/func.py` & `strangeworks_core-0.2.5/strangeworks_core/types/func.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/types/job.py` & `strangeworks_core-0.2.5/strangeworks_core/types/job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/types/machine.py` & `strangeworks_core-0.2.5/strangeworks_core/types/machine.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/types/product.py` & `strangeworks_core-0.2.5/strangeworks_core/types/product.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/types/resource.py` & `strangeworks_core-0.2.5/strangeworks_core/types/resource.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/strangeworks_core/utils.py` & `strangeworks_core-0.2.5/strangeworks_core/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_core-0.2.4/PKG-INFO` & `strangeworks_core-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-core
-Version: 0.2.4
+Version: 0.2.5
 Summary: Strangeworks Core provides the infrastructure to interact with the platform.
 License: Apache-2.0
 Author: Strange Devs
 Author-email: hello@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

