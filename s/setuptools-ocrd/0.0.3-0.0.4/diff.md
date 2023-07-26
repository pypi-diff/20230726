# Comparing `tmp/setuptools_ocrd-0.0.3.tar.gz` & `tmp/setuptools_ocrd-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools_ocrd-0.0.3.tar", last modified: Wed Jul 26 12:57:15 2023, max compression
+gzip compressed data, was "setuptools_ocrd-0.0.4.tar", last modified: Wed Jul 26 16:51:20 2023, max compression
```

## Comparing `setuptools_ocrd-0.0.3.tar` & `setuptools_ocrd-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 12:57:15.079453 setuptools_ocrd-0.0.3/
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)    11333 2023-07-19 16:25:42.000000 setuptools_ocrd-0.0.3/LICENSE
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)    13986 2023-07-26 12:57:15.070456 setuptools_ocrd-0.0.3/PKG-INFO
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      429 2023-07-24 20:19:40.000000 setuptools_ocrd-0.0.3/README.md
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      909 2023-07-25 11:20:37.000000 setuptools_ocrd-0.0.3/pyproject.toml
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-19 16:28:52.000000 setuptools_ocrd-0.0.3/requirements.txt
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)       38 2023-07-26 12:57:15.079630 setuptools_ocrd-0.0.3/setup.cfg
-drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 12:57:14.996396 setuptools_ocrd-0.0.3/setuptools_ocrd/
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      155 2023-07-24 19:04:24.000000 setuptools_ocrd-0.0.3/setuptools_ocrd/__init__.py
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      175 2023-07-19 17:27:14.000000 setuptools_ocrd-0.0.3/setuptools_ocrd/__main__.py
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      247 2023-07-24 19:20:53.000000 setuptools_ocrd-0.0.3/setuptools_ocrd/_get_version.py
-drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 12:57:15.064066 setuptools_ocrd-0.0.3/setuptools_ocrd/_integration/
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-24 18:42:24.000000 setuptools_ocrd-0.0.3/setuptools_ocrd/_integration/__init__.py
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      581 2023-07-25 11:45:07.000000 setuptools_ocrd-0.0.3/setuptools_ocrd/_integration/setuptools.py
-drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 12:57:15.053729 setuptools_ocrd-0.0.3/setuptools_ocrd.egg-info/
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)    13986 2023-07-26 12:57:14.000000 setuptools_ocrd-0.0.3/setuptools_ocrd.egg-info/PKG-INFO
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      419 2023-07-26 12:57:14.000000 setuptools_ocrd-0.0.3/setuptools_ocrd.egg-info/SOURCES.txt
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)        1 2023-07-26 12:57:14.000000 setuptools_ocrd-0.0.3/setuptools_ocrd.egg-info/dependency_links.txt
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      115 2023-07-26 12:57:14.000000 setuptools_ocrd-0.0.3/setuptools_ocrd.egg-info/entry_points.txt
--rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)       16 2023-07-26 12:57:14.000000 setuptools_ocrd-0.0.3/setuptools_ocrd.egg-info/top_level.txt
+drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 16:51:20.397393 setuptools_ocrd-0.0.4/
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)    11333 2023-07-19 16:25:42.000000 setuptools_ocrd-0.0.4/LICENSE
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      926 2023-07-26 16:51:20.394406 setuptools_ocrd-0.0.4/PKG-INFO
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      324 2023-07-26 13:35:37.000000 setuptools_ocrd-0.0.4/README.md
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      876 2023-07-26 16:46:01.000000 setuptools_ocrd-0.0.4/pyproject.toml
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-19 16:28:52.000000 setuptools_ocrd-0.0.4/requirements.txt
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)       38 2023-07-26 16:51:20.398393 setuptools_ocrd-0.0.4/setup.cfg
+drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 16:51:20.334530 setuptools_ocrd-0.0.4/setuptools_ocrd/
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      155 2023-07-24 19:04:24.000000 setuptools_ocrd-0.0.4/setuptools_ocrd/__init__.py
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      175 2023-07-19 17:27:14.000000 setuptools_ocrd-0.0.4/setuptools_ocrd/__main__.py
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      247 2023-07-24 19:20:53.000000 setuptools_ocrd-0.0.4/setuptools_ocrd/_get_version.py
+drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 16:51:20.388458 setuptools_ocrd-0.0.4/setuptools_ocrd/_integration/
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-24 18:42:24.000000 setuptools_ocrd-0.0.4/setuptools_ocrd/_integration/__init__.py
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      581 2023-07-25 11:45:07.000000 setuptools_ocrd-0.0.4/setuptools_ocrd/_integration/setuptools.py
+drwxr-xr-x   0 b-mg106   (1000) b-mg106   (1000)        0 2023-07-26 16:51:20.378455 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      926 2023-07-26 16:51:20.000000 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/PKG-INFO
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      419 2023-07-26 16:51:20.000000 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/SOURCES.txt
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)        1 2023-07-26 16:51:20.000000 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/dependency_links.txt
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)      115 2023-07-26 16:51:20.000000 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/entry_points.txt
+-rw-r--r--   0 b-mg106   (1000) b-mg106   (1000)       16 2023-07-26 16:51:20.000000 setuptools_ocrd-0.0.4/setuptools_ocrd.egg-info/top_level.txt
```

### Comparing `setuptools_ocrd-0.0.3/LICENSE` & `setuptools_ocrd-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools_ocrd-0.0.3/pyproject.toml` & `setuptools_ocrd-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "setuptools_ocrd"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name = "Mike Gerber", email = "mike.gerber@sbb.spk-berlin.de"},
 ]
 description = "Manage your package version through ocrd-tool.json"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["ocr-d", "setuptools"]
-license = {file = "LICENSE"}
 classifiers = [
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Build Tools",
 ]
 dynamic = ["dependencies"]
```

### Comparing `setuptools_ocrd-0.0.3/setuptools_ocrd/_integration/setuptools.py` & `setuptools_ocrd-0.0.4/setuptools_ocrd/_integration/setuptools.py`

 * *Files identical despite different names*

