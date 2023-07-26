# Comparing `tmp/testmhdbAPI-1.3.tar.gz` & `tmp/testmhdbAPI-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/testmhdbAPI-1.3.tar", last modified: Tue Jul 25 23:48:10 2023, max compression
+gzip compressed data, was "dist/testmhdbAPI-1.4.tar", last modified: Wed Jul 26 00:06:40 2023, max compression
```

## Comparing `testmhdbAPI-1.3.tar` & `testmhdbAPI-1.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/machbaseAPI/
--rw-r--r--   0 root         (0) root         (0)    15368 2023-07-24 01:22:08.000000 testmhdbAPI-1.3/machbaseAPI/machbaseAPI.py
--rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 01:22:08.000000 testmhdbAPI-1.3/machbaseAPI/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.3/libmachbaseAPI.so
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-24 01:22:08.000000 testmhdbAPI-1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1248 2023-07-25 23:47:58.000000 testmhdbAPI-1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/testmhdbAPI.egg-info/
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/testmhdbAPI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/testmhdbAPI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      236 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/testmhdbAPI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/testmhdbAPI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 01:22:08.000000 testmhdbAPI-1.3/README
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:06:40.000000 testmhdbAPI-1.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:06:40.000000 testmhdbAPI-1.4/machbaseAPI/
+-rw-r--r--   0 root         (0) root         (0)    15368 2023-07-24 01:22:08.000000 testmhdbAPI-1.4/machbaseAPI/machbaseAPI.py
+-rw-r--r--   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.4/machbaseAPI/libmachbaseAPI.so
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 01:22:08.000000 testmhdbAPI-1.4/machbaseAPI/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.4/libmachbaseAPI.so
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 00:04:34.000000 testmhdbAPI-1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 00:06:40.000000 testmhdbAPI-1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-07-26 00:06:10.000000 testmhdbAPI-1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 00:06:40.000000 testmhdbAPI-1.4/testmhdbAPI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 00:06:39.000000 testmhdbAPI-1.4/testmhdbAPI.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 00:06:39.000000 testmhdbAPI-1.4/testmhdbAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-26 00:06:39.000000 testmhdbAPI-1.4/testmhdbAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 00:06:39.000000 testmhdbAPI-1.4/testmhdbAPI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 01:22:08.000000 testmhdbAPI-1.4/README
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 00:06:40.000000 testmhdbAPI-1.4/PKG-INFO
```

### Comparing `testmhdbAPI-1.3/machbaseAPI/machbaseAPI.py` & `testmhdbAPI-1.4/machbaseAPI/machbaseAPI.py`

 * *Files identical despite different names*

### Comparing `testmhdbAPI-1.3/libmachbaseAPI.so` & `testmhdbAPI-1.4/machbaseAPI/libmachbaseAPI.so`

 * *Files identical despite different names*

### Comparing `testmhdbAPI-1.3/setup.py` & `testmhdbAPI-1.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 
 import os, re, shutil, zipfile, platform, sys
 from setuptools import setup, find_packages
 from distutils.sysconfig import get_python_lib
 
 setup(
     name='testmhdbAPI',
-    version='1.3',
+    version='1.4',
     description='Machbase-Python3-API',
     long_description='Python3 module for Machbase',
     url='http://www.machbase.com',
     author='machbase',
     author_email='support@machbase.com',
     platforms='LINUX',
     packages=find_packages(),
-    package_data={"":['*.so']}
+    package_data={"machbaseAPI":['*.so']}
 )
 
 args = sys.argv
 p = platform.system()
 
 if p == 'Windows' and args[1] == 'install':
     os.chdir(get_python_lib())
```

