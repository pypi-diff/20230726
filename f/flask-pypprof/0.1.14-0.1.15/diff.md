# Comparing `tmp/flask_pypprof-0.1.14.tar.gz` & `tmp/flask_pypprof-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_pypprof-0.1.14.tar", max compression
+gzip compressed data, was "flask_pypprof-0.1.15.tar", max compression
```

## Comparing `flask_pypprof-0.1.14.tar` & `flask_pypprof-0.1.15.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/LICENSE
--rw-r--r--   0        0        0     1788 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/README.md
--rw-r--r--   0        0        0      333 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/flask_pypprof/__init__.py
--rw-r--r--   0        0        0     1408 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/flask_pypprof/handler.py
--rw-r--r--   0        0        0     1125 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/flask_pypprof/noop_routes.py
--rw-r--r--   0        0        0     1919 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/flask_pypprof/routes.py
--rw-r--r--   0        0        0      652 2023-07-18 17:48:50.618253 flask_pypprof-0.1.14/pyproject.toml
--rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 flask_pypprof-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 18:30:19.599544 flask_pypprof-0.1.15/LICENSE
+-rw-r--r--   0        0        0     1788 2023-07-26 18:30:19.599544 flask_pypprof-0.1.15/README.md
+-rw-r--r--   0        0        0      333 2023-07-26 18:30:19.599544 flask_pypprof-0.1.15/flask_pypprof/__init__.py
+-rw-r--r--   0        0        0     1408 2023-07-26 18:30:19.599544 flask_pypprof-0.1.15/flask_pypprof/handler.py
+-rw-r--r--   0        0        0     1125 2023-07-26 18:30:19.599544 flask_pypprof-0.1.15/flask_pypprof/noop_routes.py
+-rw-r--r--   0        0        0     1919 2023-07-26 18:30:19.599544 flask_pypprof-0.1.15/flask_pypprof/routes.py
+-rw-r--r--   0        0        0      652 2023-07-26 18:30:19.599544 flask_pypprof-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 flask_pypprof-0.1.15/PKG-INFO
```

### Comparing `flask_pypprof-0.1.14/LICENSE` & `flask_pypprof-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.14/README.md` & `flask_pypprof-0.1.15/README.md`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.14/flask_pypprof/handler.py` & `flask_pypprof-0.1.15/flask_pypprof/handler.py`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.14/flask_pypprof/noop_routes.py` & `flask_pypprof-0.1.15/flask_pypprof/noop_routes.py`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.14/flask_pypprof/routes.py` & `flask_pypprof-0.1.15/flask_pypprof/routes.py`

 * *Files identical despite different names*

### Comparing `flask_pypprof-0.1.14/pyproject.toml` & `flask_pypprof-0.1.15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "flask-pypprof"
-version = "v0.1.14"
+version = "v0.1.15"
 description = "Pypprof Flask wrapper"
 authors = ["Diego <diegolparra@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "flask_pypprof" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8 <3.11"
-flask = "^2.3.2"
+flask = "^2.1.3"
 
 zprofile = { version = "1.0.12", platform = "linux" }
 protobuf = { version = "^3.20", platform = "linux" }
 mprofile = { version = "0.0.15", platform = "linux" }
 pypprof = { version = "0.0.1", platform = "linux" }
 
 [tool.poetry.dev-dependencies]
```

### Comparing `flask_pypprof-0.1.14/PKG-INFO` & `flask_pypprof-0.1.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: flask-pypprof
-Version: 0.1.14
+Version: 0.1.15
 Summary: Pypprof Flask wrapper
 Author: Diego
 Author-email: diegolparra@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: flask (>=2.3.2,<3.0.0)
+Requires-Dist: flask (>=2.1.3,<3.0.0)
 Requires-Dist: mprofile (==0.0.15) ; sys_platform == "linux"
 Requires-Dist: protobuf (>=3.20,<4.0) ; sys_platform == "linux"
 Requires-Dist: pypprof (==0.0.1) ; sys_platform == "linux"
 Requires-Dist: zprofile (==1.0.12) ; sys_platform == "linux"
 Description-Content-Type: text/markdown
 
 # flask-pypprof
```

