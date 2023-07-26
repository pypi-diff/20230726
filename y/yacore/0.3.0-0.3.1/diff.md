# Comparing `tmp/yacore-0.3.0.tar.gz` & `tmp/yacore-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yacore-0.3.0.tar", last modified: Mon Jul 24 18:53:50 2023, max compression
+gzip compressed data, was "yacore-0.3.1.tar", last modified: Tue Jul 25 19:57:43 2023, max compression
```

## Comparing `yacore-0.3.0.tar` & `yacore-0.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:50.449345 yacore-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-24 18:53:32.000000 yacore-0.3.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-24 18:53:32.000000 yacore-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-24 18:53:50.449345 yacore-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-24 18:53:32.000000 yacore-0.3.0/history.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-24 18:53:32.000000 yacore-0.3.0/license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-24 18:53:32.000000 yacore-0.3.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-24 18:53:32.000000 yacore-0.3.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:53:50.449345 yacore-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-24 18:53:32.000000 yacore-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:50.445345 yacore-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-24 18:53:32.000000 yacore-0.3.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-24 18:53:32.000000 yacore-0.3.0/tests/test_db_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-24 18:53:32.000000 yacore-0.3.0/tests/test_deepmerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-24 18:53:32.000000 yacore-0.3.0/tests/test_executors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-24 18:53:32.000000 yacore-0.3.0/tests/test_net_http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:50.445345 yacore-0.3.0/yacore/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:50.445345 yacore-0.3.0/yacore/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:50.445345 yacore-0.3.0/yacore/db/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/db/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/db/postgresql/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/db/postgresql/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/injector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:50.445345 yacore-0.3.0/yacore/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/log/loguru.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/log/stdlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:50.445345 yacore-0.3.0/yacore/net/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:50.449345 yacore-0.3.0/yacore/net/http/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/net/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/net/http/server.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 18:53:32.000000 yacore-0.3.0/yacore/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:53:50.445345 yacore-0.3.0/yacore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-24 18:53:50.000000 yacore-0.3.0/yacore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-24 18:53:50.000000 yacore-0.3.0/yacore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:53:50.000000 yacore-0.3.0/yacore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-24 18:53:50.000000 yacore-0.3.0/yacore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-24 18:53:50.000000 yacore-0.3.0/yacore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 18:53:50.000000 yacore-0.3.0/yacore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:43.088769 yacore-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 19:57:24.000000 yacore-0.3.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 19:57:24.000000 yacore-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-25 19:57:43.084769 yacore-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-25 19:57:24.000000 yacore-0.3.1/history.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-25 19:57:24.000000 yacore-0.3.1/license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-25 19:57:24.000000 yacore-0.3.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-25 19:57:24.000000 yacore-0.3.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:57:43.088769 yacore-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-25 19:57:24.000000 yacore-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:43.084769 yacore-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-25 19:57:24.000000 yacore-0.3.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-07-25 19:57:24.000000 yacore-0.3.1/tests/test_db_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-25 19:57:24.000000 yacore-0.3.1/tests/test_deepmerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-25 19:57:24.000000 yacore-0.3.1/tests/test_executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-07-25 19:57:24.000000 yacore-0.3.1/tests/test_net_http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:43.084769 yacore-0.3.1/yacore/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:43.084769 yacore-0.3.1/yacore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:43.084769 yacore-0.3.1/yacore/db/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/db/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/db/postgresql/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8181 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/db/postgresql/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/injector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:43.084769 yacore-0.3.1/yacore/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/log/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/log/stdlib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:43.084769 yacore-0.3.1/yacore/net/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:43.084769 yacore-0.3.1/yacore/net/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/net/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/net/http/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 19:57:24.000000 yacore-0.3.1/yacore/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:57:43.084769 yacore-0.3.1/yacore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-25 19:57:43.000000 yacore-0.3.1/yacore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 19:57:43.000000 yacore-0.3.1/yacore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:57:43.000000 yacore-0.3.1/yacore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 19:57:43.000000 yacore-0.3.1/yacore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-25 19:57:43.000000 yacore-0.3.1/yacore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 19:57:43.000000 yacore-0.3.1/yacore.egg-info/top_level.txt
```

### Comparing `yacore-0.3.0/PKG-INFO` & `yacore-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yacore
-Version: 0.3.0
+Version: 0.3.1
 Summary: yet another core library
 Home-page: https://github.com/pohmelie/yacore
 Author: pohmelie
 Author-email: multisosnooley@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yacore-0.3.0/history.md` & `yacore-0.3.1/history.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+# 0.3.1 (25-07-2023)
+- fix `importlib.resources` deprication warning
+
 # 0.3.0 (24-07-2023)
 - add top-level imports from 3rd party libraries
 
 # 0.2.0 (22-07-2023)
 - target python version changed to `>= 3.11`
 - log/loguru: fix `InterceptHandler` for python 3.11
 - dev: use `ruff` linter instead of `flake8`
```

### Comparing `yacore-0.3.0/license.txt` & `yacore-0.3.1/license.txt`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/readme.md` & `yacore-0.3.1/readme.md`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/setup.py` & `yacore-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/tests/conftest.py` & `yacore-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/tests/test_db_postgresql.py` & `yacore-0.3.1/tests/test_db_postgresql.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/tests/test_deepmerge.py` & `yacore-0.3.1/tests/test_deepmerge.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/tests/test_executors.py` & `yacore-0.3.1/tests/test_executors.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/tests/test_net_http.py` & `yacore-0.3.1/tests/test_net_http.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/yacore/db/postgresql/fixtures.py` & `yacore-0.3.1/yacore/db/postgresql/fixtures.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/yacore/db/postgresql/postgresql.py` & `yacore-0.3.1/yacore/db/postgresql/postgresql.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/yacore/executors.py` & `yacore-0.3.1/yacore/executors.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/yacore/log/loguru.py` & `yacore-0.3.1/yacore/log/loguru.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/yacore/log/stdlib.py` & `yacore-0.3.1/yacore/log/stdlib.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/yacore/net/http/client.py` & `yacore-0.3.1/yacore/net/http/client.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/yacore/net/http/server.py` & `yacore-0.3.1/yacore/net/http/server.py`

 * *Files identical despite different names*

### Comparing `yacore-0.3.0/yacore.egg-info/PKG-INFO` & `yacore-0.3.1/yacore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yacore
-Version: 0.3.0
+Version: 0.3.1
 Summary: yet another core library
 Home-page: https://github.com/pohmelie/yacore
 Author: pohmelie
 Author-email: multisosnooley@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yacore-0.3.0/yacore.egg-info/SOURCES.txt` & `yacore-0.3.1/yacore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

