# Comparing `tmp/python_injection-0.2.2.tar.gz` & `tmp/python_injection-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_injection-0.2.2.tar", max compression
+gzip compressed data, was "python_injection-0.2.3.tar", max compression
```

## Comparing `python_injection-0.2.2.tar` & `python_injection-0.2.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2538 2023-07-16 12:05:40.851462 python_injection-0.2.2/README.md
--rw-r--r--   0        0        0       38 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/__init__.py
--rw-r--r--   0        0        0     4038 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/core.py
--rw-r--r--   0        0        0      340 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/core.pyi
--rw-r--r--   0        0        0       39 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/exceptions.py
--rw-r--r--   0        0        0      461 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/utils.py
--rw-r--r--   0        0        0       81 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/utils.pyi
--rw-r--r--   0        0        0      561 2023-07-16 12:06:03.571627 python_injection-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 python_injection-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2538 2023-07-26 13:19:25.496965 python_injection-0.2.3/README.md
+-rw-r--r--   0        0        0       38 2023-07-26 13:19:25.496965 python_injection-0.2.3/injection/__init__.py
+-rw-r--r--   0        0        0     4042 2023-07-26 13:19:25.496965 python_injection-0.2.3/injection/core.py
+-rw-r--r--   0        0        0      340 2023-07-26 13:19:25.496965 python_injection-0.2.3/injection/core.pyi
+-rw-r--r--   0        0        0       39 2023-07-26 13:19:25.496965 python_injection-0.2.3/injection/exceptions.py
+-rw-r--r--   0        0        0      461 2023-07-26 13:19:25.496965 python_injection-0.2.3/injection/utils.py
+-rw-r--r--   0        0        0       81 2023-07-26 13:19:25.496965 python_injection-0.2.3/injection/utils.pyi
+-rw-r--r--   0        0        0      561 2023-07-26 13:19:47.569111 python_injection-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 python_injection-0.2.3/PKG-INFO
```

### Comparing `python_injection-0.2.2/README.md` & `python_injection-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `python_injection-0.2.2/injection/core.py` & `python_injection-0.2.3/injection/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             signature = inspect.signature(function)
             arguments = signature.bind_partial(*args, **kwargs).arguments
             args = []
             kwargs = {}
 
             for name, parameter in signature.parameters.items():
                 try:
-                    value = arguments[name]
+                    value = arguments.pop(name)
                 except KeyError:
                     try:
                         value = get_instance(parameter.annotation)
                     except NoInjectable:
                         continue
 
                 match parameter.kind:
```

### Comparing `python_injection-0.2.2/pyproject.toml` & `python_injection-0.2.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-injection"
-version = "0.2.2"
+version = "0.2.3"
 description = "Fast and easy dependency injection framework."
 authors = ["remimd"]
 keywords = ["dependencies", "inject", "injection"]
 license = "MIT"
 packages = [{ include = "injection" }]
 readme = "README.md"
 repository = "https://github.com/soon-app/injection"
```

### Comparing `python_injection-0.2.2/PKG-INFO` & `python_injection-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-injection
-Version: 0.2.2
+Version: 0.2.3
 Summary: Fast and easy dependency injection framework.
 Home-page: https://github.com/soon-app/injection
 License: MIT
 Keywords: dependencies,inject,injection
 Author: remimd
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
```

