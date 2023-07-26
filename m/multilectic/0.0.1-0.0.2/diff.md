# Comparing `tmp/multilectic-0.0.1.tar.gz` & `tmp/multilectic-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multilectic-0.0.1.tar", last modified: Mon Jul 24 12:11:11 2023, max compression
+gzip compressed data, was "multilectic-0.0.2.tar", last modified: Wed Jul 26 18:47:29 2023, max compression
```

## Comparing `multilectic-0.0.1.tar` & `multilectic-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-24 12:11:11.117402 multilectic-0.0.1/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-07-24 11:57:34.000000 multilectic-0.0.1/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      617 2023-07-24 12:11:11.117402 multilectic-0.0.1/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       69 2023-07-24 12:08:05.000000 multilectic-0.0.1/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      629 2023-07-24 12:05:32.000000 multilectic-0.0.1/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-24 12:11:11.117402 multilectic-0.0.1/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-24 12:11:11.113402 multilectic-0.0.1/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-24 12:11:11.113402 multilectic-0.0.1/src/multilectic/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-07-24 11:57:34.000000 multilectic-0.0.1/src/multilectic/__init__.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-24 12:11:11.117402 multilectic-0.0.1/src/multilectic.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      617 2023-07-24 12:11:11.000000 multilectic-0.0.1/src/multilectic.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      216 2023-07-24 12:11:11.000000 multilectic-0.0.1/src/multilectic.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-24 12:11:11.000000 multilectic-0.0.1/src/multilectic.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       12 2023-07-24 12:11:11.000000 multilectic-0.0.1/src/multilectic.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 18:47:29.890436 multilectic-0.0.2/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-07-24 11:57:34.000000 multilectic-0.0.2/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      617 2023-07-26 18:47:29.890436 multilectic-0.0.2/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       69 2023-07-24 12:08:05.000000 multilectic-0.0.2/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      629 2023-07-26 18:20:10.000000 multilectic-0.0.2/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-26 18:47:29.890436 multilectic-0.0.2/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 18:47:29.886436 multilectic-0.0.2/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 18:47:29.890436 multilectic-0.0.2/src/multilectic/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-07-24 11:57:34.000000 multilectic-0.0.2/src/multilectic/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      858 2023-07-26 18:42:54.000000 multilectic-0.0.2/src/multilectic/positions.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 18:47:29.890436 multilectic-0.0.2/src/multilectic.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      617 2023-07-26 18:47:29.000000 multilectic-0.0.2/src/multilectic.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      269 2023-07-26 18:47:29.000000 multilectic-0.0.2/src/multilectic.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-26 18:47:29.000000 multilectic-0.0.2/src/multilectic.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       12 2023-07-26 18:47:29.000000 multilectic-0.0.2/src/multilectic.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 18:47:29.890436 multilectic-0.0.2/tests/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      261 2023-07-26 18:32:54.000000 multilectic-0.0.2/tests/test_positions.py
```

### Comparing `multilectic-0.0.1/LICENSE` & `multilectic-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multilectic-0.0.1/PKG-INFO` & `multilectic-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilectic
-Version: 0.0.1
+Version: 0.0.2
 Summary: The multilogue philosophy with more than two 'truths'
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilectic/multilectic
 Project-URL: Bug Tracker, https://github.com/multilectic/multilectic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multilectic-0.0.1/pyproject.toml` & `multilectic-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "multilectic"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "The multilogue philosophy with more than two 'truths'"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `multilectic-0.0.1/src/multilectic.egg-info/PKG-INFO` & `multilectic-0.0.2/src/multilectic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilectic
-Version: 0.0.1
+Version: 0.0.2
 Summary: The multilogue philosophy with more than two 'truths'
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilectic/multilectic
 Project-URL: Bug Tracker, https://github.com/multilectic/multilectic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

