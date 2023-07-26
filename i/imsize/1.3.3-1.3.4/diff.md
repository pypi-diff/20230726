# Comparing `tmp/imsize-1.3.3.tar.gz` & `tmp/imsize-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsize-1.3.3.tar", last modified: Wed Jul 26 13:51:22 2023, max compression
+gzip compressed data, was "imsize-1.3.4.tar", last modified: Wed Jul 26 15:10:15 2023, max compression
```

## Comparing `imsize-1.3.3.tar` & `imsize-1.3.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 13:51:22.401034 imsize-1.3.3/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imsize-1.3.3/LICENSE
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     2294 2023-07-26 13:51:22.401034 imsize-1.3.3/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      589 2023-03-13 15:45:56.000000 imsize-1.3.3/README.md
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      619 2023-07-26 13:28:36.000000 imsize-1.3.3/pyproject.toml
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-07-26 13:51:22.405034 imsize-1.3.3/setup.cfg
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 13:51:22.401034 imsize-1.3.3/src/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15567 2023-03-13 15:45:56.000000 imsize-1.3.3/src/argv.py
--rwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)     4052 2023-07-26 13:25:19.000000 imsize-1.3.3/src/consoleapp.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     2760 2023-03-13 15:45:56.000000 imsize-1.3.3/src/exrhdr.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 13:51:22.401034 imsize-1.3.3/src/imsize.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     2294 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      342 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       43 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/entry_points.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       57 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       44 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/top_level.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    14958 2023-07-26 13:23:53.000000 imsize-1.3.3/src/imsize.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1785 2023-03-13 15:45:56.000000 imsize-1.3.3/src/pfmhdr.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1733 2023-03-13 15:45:56.000000 imsize-1.3.3/src/pnmhdr.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 13:51:22.401034 imsize-1.3.3/test/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4919 2023-03-13 15:45:57.000000 imsize-1.3.3/test/test_read.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 15:10:15.898594 imsize-1.3.4/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imsize-1.3.4/LICENSE
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     2294 2023-07-26 15:10:15.898594 imsize-1.3.4/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      589 2023-03-13 15:45:56.000000 imsize-1.3.4/README.md
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 15:10:15.898594 imsize-1.3.4/imsize/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      194 2023-07-26 14:58:43.000000 imsize-1.3.4/imsize/__init__.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15567 2023-03-13 15:45:56.000000 imsize-1.3.4/imsize/argv.py
+-rwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)     4052 2023-07-26 14:56:53.000000 imsize-1.3.4/imsize/consoleapp.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     2760 2023-03-13 15:45:56.000000 imsize-1.3.4/imsize/exrhdr.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    14800 2023-07-26 15:06:32.000000 imsize-1.3.4/imsize/imsize.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1785 2023-03-13 15:45:56.000000 imsize-1.3.4/imsize/pfmhdr.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1733 2023-03-13 15:45:56.000000 imsize-1.3.4/imsize/pnmhdr.py
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       22 2023-07-26 14:58:57.000000 imsize-1.3.4/imsize/version.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 15:10:15.898594 imsize-1.3.4/imsize.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     2294 2023-07-26 15:10:15.000000 imsize-1.3.4/imsize.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      373 2023-07-26 15:10:15.000000 imsize-1.3.4/imsize.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-07-26 15:10:15.000000 imsize-1.3.4/imsize.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       50 2023-07-26 15:10:15.000000 imsize-1.3.4/imsize.egg-info/entry_points.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       57 2023-07-26 15:10:15.000000 imsize-1.3.4/imsize.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        7 2023-07-26 15:10:15.000000 imsize-1.3.4/imsize.egg-info/top_level.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      626 2023-07-26 14:46:18.000000 imsize-1.3.4/pyproject.toml
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-07-26 15:10:15.898594 imsize-1.3.4/setup.cfg
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 15:10:15.898594 imsize-1.3.4/test/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4919 2023-03-13 15:45:57.000000 imsize-1.3.4/test/test_read.py
```

### Comparing `imsize-1.3.3/LICENSE` & `imsize-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imsize-1.3.3/PKG-INFO` & `imsize-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsize
-Version: 1.3.3
+Version: 1.3.4
 Summary: Lightning-fast extraction of image dimensions & bit depth.
 Author-email: Tomi Aarnio <tomi.p.aarnio@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Tomi Aarnio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `imsize-1.3.3/README.md` & `imsize-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `imsize-1.3.3/pyproject.toml` & `imsize-1.3.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "imsize"
-version = "1.3.3"
+version = "1.3.4"
 description="Lightning-fast extraction of image dimensions & bit depth."
 authors = [{name = "Tomi Aarnio", email = "tomi.p.aarnio@gmail.com"}]
 readme = "README.md"
 requires-python = ">= 3.8"
 license = {file = "LICENSE"}
 classifiers = [
   "Programming Language :: Python :: 3",
@@ -18,8 +18,8 @@
   "rawpy >= 0.16.0"
 ]
 
 [project.urls]
 Homepage = "http://github.com/toaarnio/imsize"
 
 [project.scripts]
-imsize = "consoleapp:main"
+imsize = "imsize.consoleapp:main"
```

### Comparing `imsize-1.3.3/src/argv.py` & `imsize-1.3.4/imsize/argv.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.3/src/consoleapp.py` & `imsize-1.3.4/imsize/consoleapp.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.3/src/exrhdr.py` & `imsize-1.3.4/imsize/exrhdr.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.3/src/imsize.egg-info/PKG-INFO` & `imsize-1.3.4/imsize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsize
-Version: 1.3.3
+Version: 1.3.4
 Summary: Lightning-fast extraction of image dimensions & bit depth.
 Author-email: Tomi Aarnio <tomi.p.aarnio@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Tomi Aarnio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `imsize-1.3.3/src/imsize.py` & `imsize-1.3.4/imsize/imsize.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,20 +26,14 @@
     from imsize import exrhdr   # local import: exrhdr.py
 except ImportError:
     # stand-alone mode
     import pnmhdr
     import pfmhdr
     import exrhdr
 
-# Fetch version number from pyproject.toml
-
-import importlib.metadata  # built-in library
-
-__version__ = importlib.metadata.version(__package__ or __name__)
-
 
 ######################################################################################
 #
 #  P U B L I C   A P I
 #
 ######################################################################################
```

### Comparing `imsize-1.3.3/src/pfmhdr.py` & `imsize-1.3.4/imsize/pfmhdr.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.3/src/pnmhdr.py` & `imsize-1.3.4/imsize/pnmhdr.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.3/test/test_read.py` & `imsize-1.3.4/test/test_read.py`

 * *Files identical despite different names*

