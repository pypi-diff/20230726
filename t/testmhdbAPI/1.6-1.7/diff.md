# Comparing `tmp/testmhdbAPI-1.6.tar.gz` & `tmp/testmhdbAPI-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/testmhdbAPI-1.6.tar", last modified: Wed Jul 26 00:28:34 2023, max compression
+gzip compressed data, was "dist/testmhdbAPI-1.7.tar", last modified: Wed Jul 26 00:46:57 2023, max compression
```

## Comparing `testmhdbAPI-1.6.tar` & `testmhdbAPI-1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:28:34.000000 testmhdbAPI-1.6/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:28:34.000000 testmhdbAPI-1.6/machbaseAPI/
--rw-r--r--   0 root         (0) root         (0)    15275 2023-07-26 00:28:14.000000 testmhdbAPI-1.6/machbaseAPI/machbaseAPI.py
--rw-r--r--   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.6/machbaseAPI/libmachbaseAPI.so
--rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 01:22:08.000000 testmhdbAPI-1.6/machbaseAPI/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.6/libmachbaseAPI.so
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 00:04:34.000000 testmhdbAPI-1.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 00:28:34.000000 testmhdbAPI-1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1259 2023-07-26 00:28:18.000000 testmhdbAPI-1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:28:34.000000 testmhdbAPI-1.6/testmhdbAPI.egg-info/
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 00:28:34.000000 testmhdbAPI-1.6/testmhdbAPI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:28:34.000000 testmhdbAPI-1.6/testmhdbAPI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-26 00:28:34.000000 testmhdbAPI-1.6/testmhdbAPI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 00:28:34.000000 testmhdbAPI-1.6/testmhdbAPI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 01:22:08.000000 testmhdbAPI-1.6/README
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 00:28:34.000000 testmhdbAPI-1.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:46:57.000000 testmhdbAPI-1.7/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:46:57.000000 testmhdbAPI-1.7/machbaseAPI/
+-rw-r--r--   0 root         (0) root         (0)    15302 2023-07-26 00:46:13.000000 testmhdbAPI-1.7/machbaseAPI/machbaseAPI.py
+-rw-r--r--   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.7/machbaseAPI/libmachbaseAPI.so
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 01:22:08.000000 testmhdbAPI-1.7/machbaseAPI/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.7/libmachbaseAPI.so
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 00:04:34.000000 testmhdbAPI-1.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 00:46:57.000000 testmhdbAPI-1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-26 00:46:18.000000 testmhdbAPI-1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:46:57.000000 testmhdbAPI-1.7/testmhdbAPI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 00:46:57.000000 testmhdbAPI-1.7/testmhdbAPI.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:46:57.000000 testmhdbAPI-1.7/testmhdbAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-26 00:46:57.000000 testmhdbAPI-1.7/testmhdbAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 00:46:57.000000 testmhdbAPI-1.7/testmhdbAPI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 01:22:08.000000 testmhdbAPI-1.7/README
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 00:46:57.000000 testmhdbAPI-1.7/PKG-INFO
```

### Comparing `testmhdbAPI-1.6/machbaseAPI/machbaseAPI.py` & `testmhdbAPI-1.7/machbaseAPI/machbaseAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import json
 import re
 import sys, errno
 
 gCharset = 'UTF-8'
 
 class machbaseAPI(object):
-    sofile = './libmachbaseAPI.so'
+    sofile = os.path.dirname(__file__) + '/libmachbaseAPI.so'
     clib = ctypes.CDLL(sofile)
     clib.openDB.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_uint32]
     clib.openDB.restype = ctypes.c_void_p
     clib.openDBEx.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_uint32, ctypes.c_char_p]
     clib.openDBEx.restype = ctypes.c_void_p
     clib.closeDB.argtypes = [ctypes.c_void_p,]
     clib.closeDB.restypes = ctypes.c_int
```

### Comparing `testmhdbAPI-1.6/machbaseAPI/libmachbaseAPI.so` & `testmhdbAPI-1.7/machbaseAPI/libmachbaseAPI.so`

 * *Files identical despite different names*

### Comparing `testmhdbAPI-1.6/libmachbaseAPI.so` & `testmhdbAPI-1.7/libmachbaseAPI.so`

 * *Files identical despite different names*

### Comparing `testmhdbAPI-1.6/setup.py` & `testmhdbAPI-1.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import os, re, shutil, zipfile, platform, sys
 from setuptools import setup, find_packages
 from distutils.sysconfig import get_python_lib
 
 setup(
     name='testmhdbAPI',
-    version='1.6',
+    version='1.7',
     description='Machbase-Python3-API',
     long_description='Python3 module for Machbase',
     url='http://www.machbase.com',
     author='machbase',
     author_email='support@machbase.com',
     platforms='LINUX',
     packages=find_packages(),
```

