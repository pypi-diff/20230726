# Comparing `tmp/pympc-1.1.0.tar.gz` & `tmp/pympc-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pympc-1.1.0.tar", last modified: Wed Jul 26 12:09:34 2023, max compression
+gzip compressed data, was "dist/pympc-1.1.1.tar", last modified: Wed Jul 26 12:14:13 2023, max compression
```

## Comparing `pympc-1.1.0.tar` & `pympc-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:09:34.000000 pympc-1.1.0/
--rw-rw-r--   0 jdl       (1000) jdl       (1000)    32422 2019-09-12 12:07:32.000000 pympc-1.1.0/LICENSE.txt
--rw-r--r--   0 jdl       (1000) jdl       (1000)     7286 2023-07-26 12:09:34.000000 pympc-1.1.0/PKG-INFO
--rw-r--r--   0 jdl       (1000) jdl       (1000)     6939 2023-07-25 17:00:47.000000 pympc-1.1.0/README.md
-drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc/
--rw-r--r--   0 jdl       (1000) jdl       (1000)      150 2023-07-26 12:08:44.000000 pympc-1.1.0/pympc/__init__.py
-drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc/data/
--rw-r--r--   0 jdl       (1000) jdl       (1000)    84540 2022-03-04 16:22:51.000000 pympc-1.1.0/pympc/data/obs_codes.npy
--rw-r--r--   0 jdl       (1000) jdl       (1000)    26650 2023-04-21 16:04:55.000000 pympc-1.1.0/pympc/pympc.py
-drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/
--rw-rw-r--   0 jdl       (1000) jdl       (1000)     7286 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/PKG-INFO
--rw-rw-r--   0 jdl       (1000) jdl       (1000)      310 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/SOURCES.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)        1 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/dependency_links.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)       67 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/entry_points.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)       56 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/requires.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)       11 2023-07-26 12:09:34.000000 pympc-1.1.0/pympc.egg-info/top_level.txt
--rw-rw-r--   0 jdl       (1000) jdl       (1000)      113 2023-07-26 12:09:34.000000 pympc-1.1.0/setup.cfg
--rw-r--r--   0 jdl       (1000) jdl       (1000)      764 2023-07-26 11:58:35.000000 pympc-1.1.0/setup.py
-drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:09:34.000000 pympc-1.1.0/test/
--rw-r--r--   0 jdl       (1000) jdl       (1000)        0 2021-04-01 14:53:21.000000 pympc-1.1.0/test/__init__.py
--rw-r--r--   0 jdl       (1000) jdl       (1000)     8914 2023-07-26 12:08:44.000000 pympc-1.1.0/test/test_pympc.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:14:13.000000 pympc-1.1.1/
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)    32422 2019-09-12 12:07:32.000000 pympc-1.1.1/LICENSE.txt
+-rw-r--r--   0 jdl       (1000) jdl       (1000)     7286 2023-07-26 12:14:13.000000 pympc-1.1.1/PKG-INFO
+-rw-r--r--   0 jdl       (1000) jdl       (1000)     6939 2023-07-25 17:00:47.000000 pympc-1.1.1/README.md
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:14:13.000000 pympc-1.1.1/pympc/
+-rw-r--r--   0 jdl       (1000) jdl       (1000)      150 2023-07-26 12:12:04.000000 pympc-1.1.1/pympc/__init__.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:14:13.000000 pympc-1.1.1/pympc/data/
+-rw-r--r--   0 jdl       (1000) jdl       (1000)    84540 2022-03-04 16:22:51.000000 pympc-1.1.1/pympc/data/obs_codes.npy
+-rw-r--r--   0 jdl       (1000) jdl       (1000)    26650 2023-04-21 16:04:55.000000 pympc-1.1.1/pympc/pympc.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:14:13.000000 pympc-1.1.1/pympc.egg-info/
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)     7286 2023-07-26 12:14:12.000000 pympc-1.1.1/pympc.egg-info/PKG-INFO
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)      310 2023-07-26 12:14:12.000000 pympc-1.1.1/pympc.egg-info/SOURCES.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)        1 2023-07-26 12:14:12.000000 pympc-1.1.1/pympc.egg-info/dependency_links.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)       67 2023-07-26 12:14:12.000000 pympc-1.1.1/pympc.egg-info/entry_points.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)       56 2023-07-26 12:14:12.000000 pympc-1.1.1/pympc.egg-info/requires.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)       11 2023-07-26 12:14:12.000000 pympc-1.1.1/pympc.egg-info/top_level.txt
+-rw-rw-r--   0 jdl       (1000) jdl       (1000)      113 2023-07-26 12:14:13.000000 pympc-1.1.1/setup.cfg
+-rw-r--r--   0 jdl       (1000) jdl       (1000)      764 2023-07-26 11:58:35.000000 pympc-1.1.1/setup.py
+drwxr-xr-x   0 jdl       (1000) jdl       (1000)        0 2023-07-26 12:14:13.000000 pympc-1.1.1/test/
+-rw-r--r--   0 jdl       (1000) jdl       (1000)        0 2021-04-01 14:53:21.000000 pympc-1.1.1/test/__init__.py
+-rw-r--r--   0 jdl       (1000) jdl       (1000)     8914 2023-07-26 12:08:44.000000 pympc-1.1.1/test/test_pympc.py
```

### Comparing `pympc-1.1.0/LICENSE.txt` & `pympc-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pympc-1.1.0/PKG-INFO` & `pympc-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympc
-Version: 1.1.0
+Version: 1.1.1
 Summary: minor planet checking
 Home-page: https://github.com/lyalpha/pympc
 Author: Joe Lyman
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `pympc-1.1.0/README.md` & `pympc-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pympc-1.1.0/pympc/data/obs_codes.npy` & `pympc-1.1.1/pympc/data/obs_codes.npy`

 * *Files identical despite different names*

### Comparing `pympc-1.1.0/pympc/pympc.py` & `pympc-1.1.1/pympc/pympc.py`

 * *Files identical despite different names*

### Comparing `pympc-1.1.0/pympc.egg-info/PKG-INFO` & `pympc-1.1.1/pympc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympc
-Version: 1.1.0
+Version: 1.1.1
 Summary: minor planet checking
 Home-page: https://github.com/lyalpha/pympc
 Author: Joe Lyman
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `pympc-1.1.0/setup.py` & `pympc-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pympc-1.1.0/test/test_pympc.py` & `pympc-1.1.1/test/test_pympc.py`

 * *Files identical despite different names*

