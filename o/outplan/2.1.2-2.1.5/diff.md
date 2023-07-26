# Comparing `tmp/outplan-2.1.2.tar.gz` & `tmp/outplan-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/outplan-2.1.2.tar", last modified: Tue Jul 18 11:15:46 2023, max compression
+gzip compressed data, was "/home/runner/work/outplan/outplan/dist/tmpstm6vr64/outplan-2.1.5.tar", last modified: Wed Jul 26 09:34:46 2023, max compression
```

## Comparing `outplan-2.1.2.tar` & `outplan-2.1.5.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-18 11:15:46.000000 outplan-2.1.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1067 2023-07-18 11:14:46.000000 outplan-2.1.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1742 2023-07-18 11:15:46.000000 outplan-2.1.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1045 2023-07-18 11:14:46.000000 outplan-2.1.2/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan/
--rw-rw-r--   0 travis    (2000) travis    (2000)      300 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12861 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      256 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/const.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      195 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14078 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/experiment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1952 2023-07-18 11:14:46.000000 outplan-2.1.2/outplan/local.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1742 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      366 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       82 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-07-18 11:15:46.000000 outplan-2.1.2/outplan.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      228 2023-07-18 11:14:46.000000 outplan-2.1.2/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-07-18 11:15:46.000000 outplan-2.1.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1258 2023-07-18 11:14:46.000000 outplan-2.1.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-07-18 11:15:46.000000 outplan-2.1.2/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)    28361 2023-07-18 11:14:46.000000 outplan-2.1.2/tests/test_experiment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1416 2023-07-18 11:14:46.000000 outplan-2.1.2/tests/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:34:46.000000 outplan-2.1.5/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-07-26 09:34:46.000000 outplan-2.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-07-26 09:34:33.000000 outplan-2.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1258 2023-07-26 09:34:33.000000 outplan-2.1.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-07-26 09:34:46.000000 outplan-2.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:34:46.000000 outplan-2.1.5/outplan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 09:34:46.000000 outplan-2.1.5/outplan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      321 2023-07-26 09:34:46.000000 outplan-2.1.5/outplan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-07-26 09:34:46.000000 outplan-2.1.5/outplan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-07-26 09:34:46.000000 outplan-2.1.5/outplan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-07-26 09:34:46.000000 outplan-2.1.5/outplan.egg-info/requires.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 09:34:46.000000 outplan-2.1.5/outplan/
+-rw-r--r--   0 runner    (1001) docker     (122)    12861 2023-07-26 09:34:33.000000 outplan-2.1.5/outplan/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-07-26 09:34:33.000000 outplan-2.1.5/outplan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1952 2023-07-26 09:34:33.000000 outplan-2.1.5/outplan/local.py
+-rw-r--r--   0 runner    (1001) docker     (122)      195 2023-07-26 09:34:33.000000 outplan-2.1.5/outplan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14078 2023-07-26 09:34:33.000000 outplan-2.1.5/outplan/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-07-26 09:34:33.000000 outplan-2.1.5/outplan/const.py
+-rw-r--r--   0 runner    (1001) docker     (122)      228 2023-07-26 09:34:33.000000 outplan-2.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1045 2023-07-26 09:34:33.000000 outplan-2.1.5/README.md
```

### Comparing `outplan-2.1.2/LICENSE` & `outplan-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `outplan-2.1.2/PKG-INFO` & `outplan-2.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: outplan
-Version: 2.1.2
+Version: 2.1.5
 Summary: Support nested experiment/namespace base on Facebook Planout
 Home-page: https://github.com/xiachufang/outplan
 Author: x1ah
 Author-email: gaoxiaoqiang@xiachufang.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -62,7 +63,9 @@
 # run test
 make test
 
 # commit
 pip install pre-commit
 # and commit here
 ```
+
+
```

### Comparing `outplan-2.1.2/README.md` & `outplan-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `outplan-2.1.2/outplan/client.py` & `outplan-2.1.5/outplan/client.py`

 * *Files identical despite different names*

### Comparing `outplan-2.1.2/outplan/experiment.py` & `outplan-2.1.5/outplan/experiment.py`

 * *Files identical despite different names*

### Comparing `outplan-2.1.2/outplan/local.py` & `outplan-2.1.5/outplan/local.py`

 * *Files identical despite different names*

### Comparing `outplan-2.1.2/outplan.egg-info/PKG-INFO` & `outplan-2.1.5/outplan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: outplan
-Version: 2.1.2
+Version: 2.1.5
 Summary: Support nested experiment/namespace base on Facebook Planout
 Home-page: https://github.com/xiachufang/outplan
 Author: x1ah
 Author-email: gaoxiaoqiang@xiachufang.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
@@ -62,7 +63,9 @@
 # run test
 make test
 
 # commit
 pip install pre-commit
 # and commit here
 ```
+
+
```

### Comparing `outplan-2.1.2/setup.py` & `outplan-2.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with io.open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="outplan",
-    version="2.1.2",
+    version="2.1.5",
     description="Support nested experiment/namespace base on Facebook Planout",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xiachufang/outplan",
     author="x1ah",
     author_email="gaoxiaoqiang@xiachufang.com",
     packages=find_packages(exclude=["docs", "tests*"]),
```

