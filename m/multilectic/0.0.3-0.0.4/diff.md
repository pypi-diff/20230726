# Comparing `tmp/multilectic-0.0.3.tar.gz` & `tmp/multilectic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multilectic-0.0.3.tar", last modified: Wed Jul 26 18:59:34 2023, max compression
+gzip compressed data, was "multilectic-0.0.4.tar", last modified: Wed Jul 26 21:07:56 2023, max compression
```

## Comparing `multilectic-0.0.3.tar` & `multilectic-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 18:59:34.287180 multilectic-0.0.3/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-07-24 11:57:34.000000 multilectic-0.0.3/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      615 2023-07-26 18:59:34.283180 multilectic-0.0.3/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       67 2023-07-26 18:58:44.000000 multilectic-0.0.3/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      629 2023-07-26 18:58:44.000000 multilectic-0.0.3/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-26 18:59:34.287180 multilectic-0.0.3/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 18:59:34.283180 multilectic-0.0.3/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 18:59:34.283180 multilectic-0.0.3/src/multilectic/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      253 2023-07-26 18:58:44.000000 multilectic-0.0.3/src/multilectic/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      858 2023-07-26 18:42:54.000000 multilectic-0.0.3/src/multilectic/positions.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 18:59:34.283180 multilectic-0.0.3/src/multilectic.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      615 2023-07-26 18:59:34.000000 multilectic-0.0.3/src/multilectic.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      269 2023-07-26 18:59:34.000000 multilectic-0.0.3/src/multilectic.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-26 18:59:34.000000 multilectic-0.0.3/src/multilectic.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       12 2023-07-26 18:59:34.000000 multilectic-0.0.3/src/multilectic.egg-info/top_level.txt
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 18:59:34.283180 multilectic-0.0.3/tests/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      261 2023-07-26 18:32:54.000000 multilectic-0.0.3/tests/test_positions.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 21:07:56.906173 multilectic-0.0.4/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1074 2023-07-24 11:57:34.000000 multilectic-0.0.4/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      615 2023-07-26 21:07:56.906173 multilectic-0.0.4/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       67 2023-07-26 18:58:44.000000 multilectic-0.0.4/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      629 2023-07-26 21:03:50.000000 multilectic-0.0.4/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-26 21:07:56.906173 multilectic-0.0.4/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 21:07:56.902173 multilectic-0.0.4/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 21:07:56.906173 multilectic-0.0.4/src/multilectic/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      253 2023-07-26 18:58:44.000000 multilectic-0.0.4/src/multilectic/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      911 2023-07-26 21:06:14.000000 multilectic-0.0.4/src/multilectic/positions.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 21:07:56.906173 multilectic-0.0.4/src/multilectic.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      615 2023-07-26 21:07:56.000000 multilectic-0.0.4/src/multilectic.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      269 2023-07-26 21:07:56.000000 multilectic-0.0.4/src/multilectic.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-26 21:07:56.000000 multilectic-0.0.4/src/multilectic.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       12 2023-07-26 21:07:56.000000 multilectic-0.0.4/src/multilectic.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 21:07:56.906173 multilectic-0.0.4/tests/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      261 2023-07-26 18:32:54.000000 multilectic-0.0.4/tests/test_positions.py
```

### Comparing `multilectic-0.0.3/LICENSE` & `multilectic-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multilectic-0.0.3/PKG-INFO` & `multilectic-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilectic
-Version: 0.0.3
+Version: 0.0.4
 Summary: The multilogue philosophy with more than two 'truths'
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilectic/multilectic
 Project-URL: Bug Tracker, https://github.com/multilectic/multilectic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multilectic-0.0.3/pyproject.toml` & `multilectic-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "multilectic"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "The multilogue philosophy with more than two 'truths'"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `multilectic-0.0.3/src/multilectic/positions.py` & `multilectic-0.0.4/src/multilectic/positions.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 """Copyright (c) Alexander Fedotov.
 This source code is licensed under the license found in the
 LICENSE file in the root directory of this source tree.
 """
 from typing import List, Dict
 
 
-class Position:
+class Position(object):
     """ A position in a multilogue discussion. """
     thesis: str                 = ""
     antithesis: str             = ""
     conversation: List[Dict]    = []  # The course of conversation, sequence of statements.
 
     def __init__(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
+            super(Position, self).__init__()
 
     def __call__(self, *args, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
         return self
 
     def __repr__(self):
```

### Comparing `multilectic-0.0.3/src/multilectic.egg-info/PKG-INFO` & `multilectic-0.0.4/src/multilectic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilectic
-Version: 0.0.3
+Version: 0.0.4
 Summary: The multilogue philosophy with more than two 'truths'
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilectic/multilectic
 Project-URL: Bug Tracker, https://github.com/multilectic/multilectic/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

