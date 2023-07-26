# Comparing `tmp/imp_toolkit_logs-0.1.3.tar.gz` & `tmp/imp_toolkit_logs-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imp_toolkit_logs-0.1.3.tar", max compression
+gzip compressed data, was "imp_toolkit_logs-0.1.4.tar", max compression
```

## Comparing `imp_toolkit_logs-0.1.3.tar` & `imp_toolkit_logs-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0       30 2023-07-25 22:38:08.817338 imp_toolkit_logs-0.1.3/README.md
--rw-r--r--   0        0        0      380 2023-07-25 22:22:12.036888 imp_toolkit_logs-0.1.3/imp/main.py
--rw-r--r--   0        0        0      656 2023-07-26 03:00:09.406587 imp_toolkit_logs-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 imp_toolkit_logs-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-07-25 22:38:08.817338 imp_toolkit_logs-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 03:02:56.043811 imp_toolkit_logs-0.1.4/imp/__init__.py
+-rw-r--r--   0        0        0      380 2023-07-25 22:22:12.036888 imp_toolkit_logs-0.1.4/imp/main.py
+-rw-r--r--   0        0        0      656 2023-07-26 03:04:09.218783 imp_toolkit_logs-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 imp_toolkit_logs-0.1.4/PKG-INFO
```

### Comparing `imp_toolkit_logs-0.1.3/pyproject.toml` & `imp_toolkit_logs-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "imp-toolkit-logs"
-version = "0.1.3"
+version = "0.1.4"
 description = "toolkit imp"
 authors = ["Johan Bustos <johan.bustosm@gmail.com>"]
 readme = "README.md"
 packages = [{include = "imp"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `imp_toolkit_logs-0.1.3/PKG-INFO` & `imp_toolkit_logs-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imp-toolkit-logs
-Version: 0.1.3
+Version: 0.1.4
 Summary: toolkit imp
 Author: Johan Bustos
 Author-email: johan.bustosm@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

