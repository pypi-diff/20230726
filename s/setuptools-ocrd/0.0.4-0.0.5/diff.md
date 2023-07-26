# Comparing `tmp/setuptools_ocrd-0.0.4.tar.gz` & `tmp/setuptools_ocrd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools_ocrd-0.0.4.tar", last modified: Wed Jul 26 16:51:20 2023, max compression
+gzip compressed data, was "setuptools_ocrd-0.0.5.tar", last modified: Wed Jul 26 17:49:40 2023, max compression
```

## Comparing `setuptools_ocrd-0.0.4.tar` & `setuptools_ocrd-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 16:51:20.397393 setuptools_ocrd-0.0.4/
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)    11333 2023-07-19 16:25:42.000000 setuptools_ocrd-0.0.4/LICENSE
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      926 2023-07-26 16:51:20.394406 setuptools_ocrd-0.0.4/PKG-INFO
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      324 2023-07-26 13:35:37.000000 setuptools_ocrd-0.0.4/README.md
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      876 2023-07-26 16:46:01.000000 setuptools_ocrd-0.0.4/pyproject.toml
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-19 16:28:52.000000 setuptools_ocrd-0.0.4/requirements.txt
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)       38 2023-07-26 16:51:20.398393 setuptools_ocrd-0.0.4/setup.cfg
-drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 16:51:20.334530 setuptools_ocrd-0.0.4/setuptools_ocrd/
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      155 2023-07-24 19:04:24.000000 setuptools_ocrd-0.0.4/setuptools_ocrd/__init__.py
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      175 2023-07-19 17:27:14.000000 setuptools_ocrd-0.0.4/setuptools_ocrd/__main__.py
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      247 2023-07-24 19:20:53.000000 setuptools_ocrd-0.0.4/setuptools_ocrd/_get_version.py
-drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 16:51:20.388458 setuptools_ocrd-0.0.4/setuptools_ocrd/_integration/
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-24 18:42:24.000000 setuptools_ocrd-0.0.4/setuptools_ocrd/_integration/__init__.py
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      581 2023-07-25 11:45:07.000000 setuptools_ocrd-0.0.4/setuptools_ocrd/_integration/setuptools.py
-drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 16:51:20.378455 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      926 2023-07-26 16:51:20.000000 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/PKG-INFO
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      419 2023-07-26 16:51:20.000000 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/SOURCES.txt
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)        1 2023-07-26 16:51:20.000000 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/dependency_links.txt
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      115 2023-07-26 16:51:20.000000 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/entry_points.txt
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)       16 2023-07-26 16:51:20.000000 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:49:40.399991 setuptools_ocrd-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-07-26 17:49:32.000000 setuptools_ocrd-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-26 17:49:40.399991 setuptools_ocrd-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-26 17:49:32.000000 setuptools_ocrd-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-26 17:49:32.000000 setuptools_ocrd-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:49:32.000000 setuptools_ocrd-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:49:40.399991 setuptools_ocrd-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:49:40.399991 setuptools_ocrd-0.0.5/setuptools_ocrd/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-26 17:49:32.000000 setuptools_ocrd-0.0.5/setuptools_ocrd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-26 17:49:32.000000 setuptools_ocrd-0.0.5/setuptools_ocrd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-26 17:49:32.000000 setuptools_ocrd-0.0.5/setuptools_ocrd/_get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:49:40.399991 setuptools_ocrd-0.0.5/setuptools_ocrd/_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:49:32.000000 setuptools_ocrd-0.0.5/setuptools_ocrd/_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-26 17:49:32.000000 setuptools_ocrd-0.0.5/setuptools_ocrd/_integration/setuptools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:49:40.399991 setuptools_ocrd-0.0.5/setuptools_ocrd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-26 17:49:40.000000 setuptools_ocrd-0.0.5/setuptools_ocrd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-26 17:49:40.000000 setuptools_ocrd-0.0.5/setuptools_ocrd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:49:40.000000 setuptools_ocrd-0.0.5/setuptools_ocrd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-26 17:49:40.000000 setuptools_ocrd-0.0.5/setuptools_ocrd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 17:49:40.000000 setuptools_ocrd-0.0.5/setuptools_ocrd.egg-info/top_level.txt
```

### Comparing `setuptools_ocrd-0.0.4/LICENSE` & `setuptools_ocrd-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools_ocrd-0.0.4/PKG-INFO` & `setuptools_ocrd-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools_ocrd
-Version: 0.0.4
+Version: 0.0.5
 Summary: Manage your package version through ocrd-tool.json
 Author-email: Mike Gerber <mike.gerber@sbb.spk-berlin.de>
 Keywords: ocr-d,setuptools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -24,7 +24,10 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools-ocrd"]
 
 [project]
 # ... any other options ...
 dynamic = ["version"]
 ```
+
+## Developer information
+*Please refer to [README-DEV.md](README-DEV.md).*
```

### Comparing `setuptools_ocrd-0.0.4/pyproject.toml` & `setuptools_ocrd-0.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "setuptools_ocrd"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     {name = "Mike Gerber", email = "mike.gerber@sbb.spk-berlin.de"},
 ]
 description = "Manage your package version through ocrd-tool.json"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["ocr-d", "setuptools"]
```

### Comparing `setuptools_ocrd-0.0.4/setuptools_ocrd/_integration/setuptools.py` & `setuptools_ocrd-0.0.5/setuptools_ocrd/_integration/setuptools.py`

 * *Files identical despite different names*

### Comparing `setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/PKG-INFO` & `setuptools_ocrd-0.0.5/setuptools_ocrd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-ocrd
-Version: 0.0.4
+Version: 0.0.5
 Summary: Manage your package version through ocrd-tool.json
 Author-email: Mike Gerber <mike.gerber@sbb.spk-berlin.de>
 Keywords: ocr-d,setuptools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -24,7 +24,10 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools-ocrd"]
 
 [project]
 # ... any other options ...
 dynamic = ["version"]
 ```
+
+## Developer information
+*Please refer to [README-DEV.md](README-DEV.md).*
```

