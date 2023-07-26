# Comparing `tmp/testmhdbAPI-1.4.tar.gz` & `tmp/testmhdbAPI-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/testmhdbAPI-1.4.tar", last modified: Wed Jul 26 00:06:40 2023, max compression
+gzip compressed data, was "dist/testmhdbAPI-1.5.tar", last modified: Wed Jul 26 00:17:58 2023, max compression
```

## Comparing `testmhdbAPI-1.4.tar` & `testmhdbAPI-1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:06:40.000000 testmhdbAPI-1.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:06:40.000000 testmhdbAPI-1.4/machbaseAPI/
--rw-r--r--   0 root         (0) root         (0)    15368 2023-07-24 01:22:08.000000 testmhdbAPI-1.4/machbaseAPI/machbaseAPI.py
--rw-r--r--   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.4/machbaseAPI/libmachbaseAPI.so
--rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 01:22:08.000000 testmhdbAPI-1.4/machbaseAPI/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.4/libmachbaseAPI.so
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 00:04:34.000000 testmhdbAPI-1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 00:06:40.000000 testmhdbAPI-1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1259 2023-07-26 00:06:10.000000 testmhdbAPI-1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:06:40.000000 testmhdbAPI-1.4/testmhdbAPI.egg-info/
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 00:06:39.000000 testmhdbAPI-1.4/testmhdbAPI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:06:39.000000 testmhdbAPI-1.4/testmhdbAPI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-26 00:06:39.000000 testmhdbAPI-1.4/testmhdbAPI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 00:06:39.000000 testmhdbAPI-1.4/testmhdbAPI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 01:22:08.000000 testmhdbAPI-1.4/README
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 00:06:40.000000 testmhdbAPI-1.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:17:58.000000 testmhdbAPI-1.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:17:58.000000 testmhdbAPI-1.5/machbaseAPI/
+-rw-r--r--   0 root         (0) root         (0)    15273 2023-07-26 00:17:07.000000 testmhdbAPI-1.5/machbaseAPI/machbaseAPI.py
+-rw-r--r--   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.5/machbaseAPI/libmachbaseAPI.so
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 01:22:08.000000 testmhdbAPI-1.5/machbaseAPI/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.5/libmachbaseAPI.so
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 00:04:34.000000 testmhdbAPI-1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 00:17:58.000000 testmhdbAPI-1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-26 00:16:45.000000 testmhdbAPI-1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:17:58.000000 testmhdbAPI-1.5/testmhdbAPI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 00:17:58.000000 testmhdbAPI-1.5/testmhdbAPI.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:17:58.000000 testmhdbAPI-1.5/testmhdbAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-26 00:17:58.000000 testmhdbAPI-1.5/testmhdbAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 00:17:58.000000 testmhdbAPI-1.5/testmhdbAPI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 01:22:08.000000 testmhdbAPI-1.5/README
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 00:17:58.000000 testmhdbAPI-1.5/PKG-INFO
```

### Comparing `testmhdbAPI-1.4/machbaseAPI/machbaseAPI.py` & `testmhdbAPI-1.5/machbaseAPI/machbaseAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,21 +8,19 @@
 import os
 import ctypes
 import time
 import unittest
 import json
 import re
 import sys, errno
-from distutils.sysconfig import get_python_lib
 
 gCharset = 'UTF-8'
 
 class machbaseAPI(object):
-    _PATH = get_python_lib()
-    sofile = _PATH+'/machbaseAPI/libmachbaseAPI.so'
+    sofile = 'libmachbaseAPI.so'
     clib = ctypes.CDLL(sofile)
     clib.openDB.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_uint32]
     clib.openDB.restype = ctypes.c_void_p
     clib.openDBEx.argtypes = [ctypes.c_char_p, ctypes.c_char_p, ctypes.c_char_p, ctypes.c_uint32, ctypes.c_char_p]
     clib.openDBEx.restype = ctypes.c_void_p
     clib.closeDB.argtypes = [ctypes.c_void_p,]
     clib.closeDB.restypes = ctypes.c_int
```

### Comparing `testmhdbAPI-1.4/machbaseAPI/libmachbaseAPI.so` & `testmhdbAPI-1.5/machbaseAPI/libmachbaseAPI.so`

 * *Files identical despite different names*

### Comparing `testmhdbAPI-1.4/libmachbaseAPI.so` & `testmhdbAPI-1.5/libmachbaseAPI.so`

 * *Files identical despite different names*

### Comparing `testmhdbAPI-1.4/setup.py` & `testmhdbAPI-1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import os, re, shutil, zipfile, platform, sys
 from setuptools import setup, find_packages
 from distutils.sysconfig import get_python_lib
 
 setup(
     name='testmhdbAPI',
-    version='1.4',
+    version='1.5',
     description='Machbase-Python3-API',
     long_description='Python3 module for Machbase',
     url='http://www.machbase.com',
     author='machbase',
     author_email='support@machbase.com',
     platforms='LINUX',
     packages=find_packages(),
```

