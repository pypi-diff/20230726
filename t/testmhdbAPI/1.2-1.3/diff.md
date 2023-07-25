# Comparing `tmp/testmhdbAPI-1.2.tar.gz` & `tmp/testmhdbAPI-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/testmhdbAPI-1.2.tar", last modified: Tue Jul 25 07:40:59 2023, max compression
+gzip compressed data, was "dist/testmhdbAPI-1.3.tar", last modified: Tue Jul 25 23:48:10 2023, max compression
```

## Comparing `testmhdbAPI-1.2.tar` & `testmhdbAPI-1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/machbaseAPI/
--rw-r--r--   0 root         (0) root         (0)    15368 2023-07-24 01:22:08.000000 testmhdbAPI-1.2/machbaseAPI/machbaseAPI.py
--rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 01:22:08.000000 testmhdbAPI-1.2/machbaseAPI/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.2/libmachbaseAPI.so
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-24 01:22:08.000000 testmhdbAPI-1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1204 2023-07-25 07:38:34.000000 testmhdbAPI-1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/testmhdbAPI.egg-info/
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/testmhdbAPI.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/testmhdbAPI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      236 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/testmhdbAPI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/testmhdbAPI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 01:22:08.000000 testmhdbAPI-1.2/README
--rw-r--r--   0 root         (0) root         (0)      263 2023-07-25 07:40:59.000000 testmhdbAPI-1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/machbaseAPI/
+-rw-r--r--   0 root         (0) root         (0)    15368 2023-07-24 01:22:08.000000 testmhdbAPI-1.3/machbaseAPI/machbaseAPI.py
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-24 01:22:08.000000 testmhdbAPI-1.3/machbaseAPI/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    32608 2023-07-24 01:33:27.000000 testmhdbAPI-1.3/libmachbaseAPI.so
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-24 01:22:08.000000 testmhdbAPI-1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-07-25 23:47:58.000000 testmhdbAPI-1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/testmhdbAPI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/testmhdbAPI.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/testmhdbAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      236 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/testmhdbAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/testmhdbAPI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      155 2023-07-24 01:22:08.000000 testmhdbAPI-1.3/README
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-25 23:48:10.000000 testmhdbAPI-1.3/PKG-INFO
```

### Comparing `testmhdbAPI-1.2/machbaseAPI/machbaseAPI.py` & `testmhdbAPI-1.3/machbaseAPI/machbaseAPI.py`

 * *Files identical despite different names*

### Comparing `testmhdbAPI-1.2/libmachbaseAPI.so` & `testmhdbAPI-1.3/libmachbaseAPI.so`

 * *Files identical despite different names*

