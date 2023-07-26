# Comparing `tmp/imp_toolkit_logs-0.1.1.tar.gz` & `tmp/imp_toolkit_logs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imp_toolkit_logs-0.1.1.tar", max compression
+gzip compressed data, was "imp_toolkit_logs-0.1.2.tar", max compression
```

## Comparing `imp_toolkit_logs-0.1.1.tar` & `imp_toolkit_logs-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       30 2023-07-25 22:38:08.817338 imp_toolkit_logs-0.1.1/README.md
--rw-r--r--   0        0        0      380 2023-07-25 22:22:12.036888 imp_toolkit_logs-0.1.1/imp/main.py
--rw-r--r--   0        0        0      650 2023-07-25 23:20:22.496345 imp_toolkit_logs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 imp_toolkit_logs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-07-25 22:38:08.817338 imp_toolkit_logs-0.1.2/README.md
+-rw-r--r--   0        0        0      380 2023-07-25 22:22:12.036888 imp_toolkit_logs-0.1.2/imp/main.py
+-rw-r--r--   0        0        0      650 2023-07-26 02:54:53.764877 imp_toolkit_logs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 imp_toolkit_logs-0.1.2/PKG-INFO
```

### Comparing `imp_toolkit_logs-0.1.1/pyproject.toml` & `imp_toolkit_logs-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "imp-toolkit-logs"
-version = "0.1.1"
+version = "0.1.2"
 description = "toolkit imp"
 authors = ["Johan Bustos <johan.bustosm@gmail.com>"]
 readme = "README.md"
 packages = [{include = "imp"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 gitpython = "^3.1.32"
 click = "^8.1.6"
 
 [tool.poetry.scripts]
-imp = "imp:main"
+imp = "imp.main"
 
 [build-system]
 requires = ["setuptools","wheel","poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [pypi]
   username = "Johanbustos"
```

### Comparing `imp_toolkit_logs-0.1.1/PKG-INFO` & `imp_toolkit_logs-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imp-toolkit-logs
-Version: 0.1.1
+Version: 0.1.2
 Summary: toolkit imp
 Author: Johan Bustos
 Author-email: johan.bustosm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

