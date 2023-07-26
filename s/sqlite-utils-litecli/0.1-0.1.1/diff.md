# Comparing `tmp/sqlite-utils-litecli-0.1.tar.gz` & `tmp/sqlite-utils-litecli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlite-utils-litecli-0.1.tar", last modified: Tue Jul 25 20:15:06 2023, max compression
+gzip compressed data, was "sqlite-utils-litecli-0.1.1.tar", last modified: Wed Jul 26 21:36:31 2023, max compression
```

## Comparing `sqlite-utils-litecli-0.1.tar` & `sqlite-utils-litecli-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:06.635244 sqlite-utils-litecli-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 20:14:46.000000 sqlite-utils-litecli-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-25 20:15:06.635244 sqlite-utils-litecli-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-25 20:14:46.000000 sqlite-utils-litecli-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 20:14:46.000000 sqlite-utils-litecli-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:15:06.635244 sqlite-utils-litecli-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:06.635244 sqlite-utils-litecli-0.1/sqlite_utils_litecli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-25 20:15:06.000000 sqlite-utils-litecli-0.1/sqlite_utils_litecli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 20:15:06.000000 sqlite-utils-litecli-0.1/sqlite_utils_litecli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:15:06.000000 sqlite-utils-litecli-0.1/sqlite_utils_litecli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 20:15:06.000000 sqlite-utils-litecli-0.1/sqlite_utils_litecli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 20:15:06.000000 sqlite-utils-litecli-0.1/sqlite_utils_litecli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 20:15:06.000000 sqlite-utils-litecli-0.1/sqlite_utils_litecli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-25 20:14:46.000000 sqlite-utils-litecli-0.1/sqlite_utils_litecli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:06.635244 sqlite-utils-litecli-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-25 20:14:46.000000 sqlite-utils-litecli-0.1/tests/test_litecli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:36:31.778224 sqlite-utils-litecli-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 21:36:16.000000 sqlite-utils-litecli-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-26 21:36:31.778224 sqlite-utils-litecli-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-26 21:36:16.000000 sqlite-utils-litecli-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-26 21:36:16.000000 sqlite-utils-litecli-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:36:31.778224 sqlite-utils-litecli-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:36:31.778224 sqlite-utils-litecli-0.1.1/sqlite_utils_litecli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-26 21:36:31.000000 sqlite-utils-litecli-0.1.1/sqlite_utils_litecli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-26 21:36:31.000000 sqlite-utils-litecli-0.1.1/sqlite_utils_litecli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:36:31.000000 sqlite-utils-litecli-0.1.1/sqlite_utils_litecli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 21:36:31.000000 sqlite-utils-litecli-0.1.1/sqlite_utils_litecli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 21:36:31.000000 sqlite-utils-litecli-0.1.1/sqlite_utils_litecli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 21:36:31.000000 sqlite-utils-litecli-0.1.1/sqlite_utils_litecli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-26 21:36:16.000000 sqlite-utils-litecli-0.1.1/sqlite_utils_litecli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:36:31.778224 sqlite-utils-litecli-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-26 21:36:16.000000 sqlite-utils-litecli-0.1.1/tests/test_litecli.py
```

### Comparing `sqlite-utils-litecli-0.1/LICENSE` & `sqlite-utils-litecli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlite-utils-litecli-0.1/PKG-INFO` & `sqlite-utils-litecli-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils-litecli
-Version: 0.1
+Version: 0.1.1
 Summary: Interactive shell using litecli
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/sqlite-utils-litecli
 Project-URL: Changelog, https://github.com/simonw/sqlite-utils-litecli/releases
 Project-URL: Issues, https://github.com/simonw/sqlite-utils-litecli/issues
 Project-URL: CI, https://github.com/simonw/sqlite-utils-litecli/actions
@@ -35,14 +35,16 @@
 ```bash
 sqlite-utils litecli data.db
 ```
 This will start a `litecli` interactive shell session.
 
 Custom SQL functions provided by other plugins will be available in the shell.
 
+<img src="https://raw.githubusercontent.com/simonw/sqlite-utils-litecli/main/screenshot.jpg" width="483" height="474" alt="Screenshot showing the plugin in action - it includes autocomplete of SQLite table names">
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd sqlite-utils-litecli
 python3 -m venv venv
 source venv/bin/activate
```

### Comparing `sqlite-utils-litecli-0.1/README.md` & `sqlite-utils-litecli-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 ```bash
 sqlite-utils litecli data.db
 ```
 This will start a `litecli` interactive shell session.
 
 Custom SQL functions provided by other plugins will be available in the shell.
 
+<img src="https://raw.githubusercontent.com/simonw/sqlite-utils-litecli/main/screenshot.jpg" width="483" height="474" alt="Screenshot showing the plugin in action - it includes autocomplete of SQLite table names">
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd sqlite-utils-litecli
 python3 -m venv venv
 source venv/bin/activate
@@ -35,8 +37,8 @@
 Now install the dependencies and test dependencies:
 ```bash
 pip install -e '.[test]'
 ```
 To run the tests:
 ```bash
 pytest
-```
+```
```

### Comparing `sqlite-utils-litecli-0.1/pyproject.toml` & `sqlite-utils-litecli-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sqlite-utils-litecli"
-version = "0.1"
+version = "0.1.1"
 description = "Interactive shell using litecli"
 readme = "README.md"
 authors = [{name = "Simon Willison"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
```

### Comparing `sqlite-utils-litecli-0.1/sqlite_utils_litecli.egg-info/PKG-INFO` & `sqlite-utils-litecli-0.1.1/sqlite_utils_litecli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlite-utils-litecli
-Version: 0.1
+Version: 0.1.1
 Summary: Interactive shell using litecli
 Author: Simon Willison
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/simonw/sqlite-utils-litecli
 Project-URL: Changelog, https://github.com/simonw/sqlite-utils-litecli/releases
 Project-URL: Issues, https://github.com/simonw/sqlite-utils-litecli/issues
 Project-URL: CI, https://github.com/simonw/sqlite-utils-litecli/actions
@@ -35,14 +35,16 @@
 ```bash
 sqlite-utils litecli data.db
 ```
 This will start a `litecli` interactive shell session.
 
 Custom SQL functions provided by other plugins will be available in the shell.
 
+<img src="https://raw.githubusercontent.com/simonw/sqlite-utils-litecli/main/screenshot.jpg" width="483" height="474" alt="Screenshot showing the plugin in action - it includes autocomplete of SQLite table names">
+
 ## Development
 
 To set up this plugin locally, first checkout the code. Then create a new virtual environment:
 ```bash
 cd sqlite-utils-litecli
 python3 -m venv venv
 source venv/bin/activate
```

### Comparing `sqlite-utils-litecli-0.1/sqlite_utils_litecli.py` & `sqlite-utils-litecli-0.1.1/sqlite_utils_litecli.py`

 * *Files identical despite different names*

