# Comparing `tmp/KDEpy-1.1.4.tar.gz` & `tmp/KDEpy-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KDEpy-1.1.4.tar", last modified: Wed Jul 12 06:26:29 2023, max compression
+gzip compressed data, was "KDEpy-1.1.5.tar", last modified: Wed Jul 26 19:07:26 2023, max compression
```

## Comparing `KDEpy-1.1.4.tar` & `KDEpy-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-12 06:26:29.206738 KDEpy-1.1.4/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-12 06:26:29.203098 KDEpy-1.1.4/KDEpy/
--rw-r--r--   0 runner     (501) staff       (20)     8718 2023-07-12 06:22:34.000000 KDEpy-1.1.4/KDEpy/BaseKDE.py
--rw-r--r--   0 runner     (501) staff       (20)     8259 2023-07-12 06:22:34.000000 KDEpy-1.1.4/KDEpy/FFTKDE.py
--rw-r--r--   0 runner     (501) staff       (20)     5036 2023-07-12 06:22:34.000000 KDEpy-1.1.4/KDEpy/NaiveKDE.py
--rw-r--r--   0 runner     (501) staff       (20)     6884 2023-07-12 06:22:34.000000 KDEpy-1.1.4/KDEpy/TreeKDE.py
--rw-r--r--   0 runner     (501) staff       (20)      298 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    16130 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/binning.py
--rw-r--r--   0 runner     (501) staff       (20)    10045 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/bw_selection.py
--rw-r--r--   0 runner     (501) staff       (20)   896080 2023-07-12 06:23:43.000000 KDEpy-1.1.4/KDEpy/cutils.c
--rw-r--r--   0 runner     (501) staff       (20)    14713 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/cutils.pyx
--rw-r--r--   0 runner     (501) staff       (20)    10297 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/kernel_funcs.py
--rw-r--r--   0 runner     (501) staff       (20)     3809 2023-07-12 06:22:35.000000 KDEpy-1.1.4/KDEpy/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-12 06:26:29.205568 KDEpy-1.1.4/KDEpy.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     6930 2023-07-12 06:26:29.000000 KDEpy-1.1.4/KDEpy.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      391 2023-07-12 06:26:29.000000 KDEpy-1.1.4/KDEpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-12 06:26:29.000000 KDEpy-1.1.4/KDEpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)      163 2023-07-12 06:26:29.000000 KDEpy-1.1.4/KDEpy.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)       13 2023-07-12 06:26:29.000000 KDEpy-1.1.4/KDEpy.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1499 2023-07-12 06:22:35.000000 KDEpy-1.1.4/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       48 2023-07-12 06:22:35.000000 KDEpy-1.1.4/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     6930 2023-07-12 06:26:29.206322 KDEpy-1.1.4/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     4563 2023-07-12 06:22:35.000000 KDEpy-1.1.4/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1034 2023-07-12 06:22:37.000000 KDEpy-1.1.4/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-12 06:26:29.206846 KDEpy-1.1.4/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      575 2023-07-12 06:22:37.000000 KDEpy-1.1.4/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-26 19:07:26.364772 KDEpy-1.1.5/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-26 19:07:26.351938 KDEpy-1.1.5/KDEpy/
+-rw-r--r--   0 runner     (501) staff       (20)     8718 2023-07-26 19:01:32.000000 KDEpy-1.1.5/KDEpy/BaseKDE.py
+-rw-r--r--   0 runner     (501) staff       (20)     8259 2023-07-26 19:01:32.000000 KDEpy-1.1.5/KDEpy/FFTKDE.py
+-rw-r--r--   0 runner     (501) staff       (20)     5036 2023-07-26 19:01:32.000000 KDEpy-1.1.5/KDEpy/NaiveKDE.py
+-rw-r--r--   0 runner     (501) staff       (20)     6884 2023-07-26 19:01:33.000000 KDEpy-1.1.5/KDEpy/TreeKDE.py
+-rw-r--r--   0 runner     (501) staff       (20)      298 2023-07-26 19:01:33.000000 KDEpy-1.1.5/KDEpy/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    16130 2023-07-26 19:01:33.000000 KDEpy-1.1.5/KDEpy/binning.py
+-rw-r--r--   0 runner     (501) staff       (20)    10045 2023-07-26 19:01:33.000000 KDEpy-1.1.5/KDEpy/bw_selection.py
+-rw-r--r--   0 runner     (501) staff       (20)   896080 2023-07-26 19:04:01.000000 KDEpy-1.1.5/KDEpy/cutils.c
+-rw-r--r--   0 runner     (501) staff       (20)    14713 2023-07-26 19:01:33.000000 KDEpy-1.1.5/KDEpy/cutils.pyx
+-rw-r--r--   0 runner     (501) staff       (20)    10297 2023-07-26 19:01:33.000000 KDEpy-1.1.5/KDEpy/kernel_funcs.py
+-rw-r--r--   0 runner     (501) staff       (20)     3809 2023-07-26 19:01:34.000000 KDEpy-1.1.5/KDEpy/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2023-07-26 19:07:26.363542 KDEpy-1.1.5/KDEpy.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     6930 2023-07-26 19:07:26.000000 KDEpy-1.1.5/KDEpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      391 2023-07-26 19:07:26.000000 KDEpy-1.1.5/KDEpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2023-07-26 19:07:26.000000 KDEpy-1.1.5/KDEpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)      173 2023-07-26 19:07:26.000000 KDEpy-1.1.5/KDEpy.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)       13 2023-07-26 19:07:26.000000 KDEpy-1.1.5/KDEpy.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1499 2023-07-26 19:01:34.000000 KDEpy-1.1.5/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       48 2023-07-26 19:01:34.000000 KDEpy-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     6930 2023-07-26 19:07:26.364332 KDEpy-1.1.5/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     4563 2023-07-26 19:01:34.000000 KDEpy-1.1.5/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1056 2023-07-26 19:01:36.000000 KDEpy-1.1.5/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)       38 2023-07-26 19:07:26.364877 KDEpy-1.1.5/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      575 2023-07-26 19:01:37.000000 KDEpy-1.1.5/setup.py
```

### Comparing `KDEpy-1.1.4/KDEpy/BaseKDE.py` & `KDEpy-1.1.5/KDEpy/BaseKDE.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/KDEpy/FFTKDE.py` & `KDEpy-1.1.5/KDEpy/FFTKDE.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/KDEpy/NaiveKDE.py` & `KDEpy-1.1.5/KDEpy/NaiveKDE.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/KDEpy/TreeKDE.py` & `KDEpy-1.1.5/KDEpy/TreeKDE.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/KDEpy/binning.py` & `KDEpy-1.1.5/KDEpy/binning.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/KDEpy/bw_selection.py` & `KDEpy-1.1.5/KDEpy/bw_selection.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/KDEpy/cutils.c` & `KDEpy-1.1.5/KDEpy/cutils.c`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/KDEpy/cutils.pyx` & `KDEpy-1.1.5/KDEpy/cutils.pyx`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/KDEpy/kernel_funcs.py` & `KDEpy-1.1.5/KDEpy/kernel_funcs.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/KDEpy/utils.py` & `KDEpy-1.1.5/KDEpy/utils.py`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/KDEpy.egg-info/PKG-INFO` & `KDEpy-1.1.5/KDEpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KDEpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: Kernel Density Estimation in Python.
 Author-email: tommyod <tommy.odland@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Tommy Odland
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `KDEpy-1.1.4/LICENSE` & `KDEpy-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/PKG-INFO` & `KDEpy-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KDEpy
-Version: 1.1.4
+Version: 1.1.5
 Summary: Kernel Density Estimation in Python.
 Author-email: tommyod <tommy.odland@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Tommy Odland
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `KDEpy-1.1.4/README.md` & `KDEpy-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `KDEpy-1.1.4/pyproject.toml` & `KDEpy-1.1.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "KDEpy"
-version = "1.1.4"
+version = "1.1.5"
 dependencies = [
-    "numpy>=1.14.2",
-    "scipy>=1.0.1",
+    "numpy>=1.14.2,<2.0",
+    "scipy>=1.0.1,<2.0",
     "matplotlib>=2.2.2",
 ]
 description = "Kernel Density Estimation in Python."
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
   {name = "tommyod", email = "tommy.odland@gmail.com"},
 ]
@@ -36,9 +36,9 @@
 ]
 lint = [
   "black",
   "flake8>=3.5.0",
 ]
 
 [build-system]
-requires = ["setuptools>=45", "wheel", "cython>=0.29", "numpy>=1.14.2"]
+requires = ["setuptools>=45", "wheel", "cython>=0.29,<1.0.0", "numpy>=1.14.2,<2.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `KDEpy-1.1.4/setup.py` & `KDEpy-1.1.5/setup.py`

 * *Files identical despite different names*

