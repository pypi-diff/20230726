# Comparing `tmp/botocore-a-la-carte-internetmonitor-1.31.8.tar.gz` & `tmp/botocore-a-la-carte-internetmonitor-1.31.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-internetmonitor-1.31.8.tar", last modified: Fri Jul 21 01:21:28 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-internetmonitor-1.31.9.tar", last modified: Sat Jul 22 01:20:30 2023, max compression
```

## Comparing `botocore-a-la-carte-internetmonitor-1.31.8.tar` & `botocore-a-la-carte-internetmonitor-1.31.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:28.031050 botocore-a-la-carte-internetmonitor-1.31.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:27.000000 botocore-a-la-carte-internetmonitor-1.31.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-21 01:21:28.031050 botocore-a-la-carte-internetmonitor-1.31.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:28.031050 botocore-a-la-carte-internetmonitor-1.31.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:28.031050 botocore-a-la-carte-internetmonitor-1.31.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:28.031050 botocore-a-la-carte-internetmonitor-1.31.8/botocore/data/internetmonitor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:28.031050 botocore-a-la-carte-internetmonitor-1.31.8/botocore/data/internetmonitor/2021-06-03/
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-21 01:21:06.000000 botocore-a-la-carte-internetmonitor-1.31.8/botocore/data/internetmonitor/2021-06-03/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-21 01:21:06.000000 botocore-a-la-carte-internetmonitor-1.31.8/botocore/data/internetmonitor/2021-06-03/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    58576 2023-07-21 01:21:06.000000 botocore-a-la-carte-internetmonitor-1.31.8/botocore/data/internetmonitor/2021-06-03/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-21 01:21:06.000000 botocore-a-la-carte-internetmonitor-1.31.8/botocore/data/internetmonitor/2021-06-03/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:28.031050 botocore-a-la-carte-internetmonitor-1.31.8/botocore_a_la_carte_internetmonitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-21 01:21:28.000000 botocore-a-la-carte-internetmonitor-1.31.8/botocore_a_la_carte_internetmonitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-21 01:21:28.000000 botocore-a-la-carte-internetmonitor-1.31.8/botocore_a_la_carte_internetmonitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:28.000000 botocore-a-la-carte-internetmonitor-1.31.8/botocore_a_la_carte_internetmonitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:28.000000 botocore-a-la-carte-internetmonitor-1.31.8/botocore_a_la_carte_internetmonitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:28.031050 botocore-a-la-carte-internetmonitor-1.31.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-21 01:21:27.000000 botocore-a-la-carte-internetmonitor-1.31.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:30.421003 botocore-a-la-carte-internetmonitor-1.31.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-22 01:20:30.000000 botocore-a-la-carte-internetmonitor-1.31.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-22 01:20:30.421003 botocore-a-la-carte-internetmonitor-1.31.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:30.421003 botocore-a-la-carte-internetmonitor-1.31.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:30.421003 botocore-a-la-carte-internetmonitor-1.31.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:30.421003 botocore-a-la-carte-internetmonitor-1.31.9/botocore/data/internetmonitor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:30.421003 botocore-a-la-carte-internetmonitor-1.31.9/botocore/data/internetmonitor/2021-06-03/
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-22 01:20:09.000000 botocore-a-la-carte-internetmonitor-1.31.9/botocore/data/internetmonitor/2021-06-03/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-22 01:20:09.000000 botocore-a-la-carte-internetmonitor-1.31.9/botocore/data/internetmonitor/2021-06-03/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58576 2023-07-22 01:20:09.000000 botocore-a-la-carte-internetmonitor-1.31.9/botocore/data/internetmonitor/2021-06-03/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-22 01:20:09.000000 botocore-a-la-carte-internetmonitor-1.31.9/botocore/data/internetmonitor/2021-06-03/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:30.421003 botocore-a-la-carte-internetmonitor-1.31.9/botocore_a_la_carte_internetmonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-22 01:20:30.000000 botocore-a-la-carte-internetmonitor-1.31.9/botocore_a_la_carte_internetmonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-22 01:20:30.000000 botocore-a-la-carte-internetmonitor-1.31.9/botocore_a_la_carte_internetmonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:20:30.000000 botocore-a-la-carte-internetmonitor-1.31.9/botocore_a_la_carte_internetmonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:20:30.000000 botocore-a-la-carte-internetmonitor-1.31.9/botocore_a_la_carte_internetmonitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:20:30.421003 botocore-a-la-carte-internetmonitor-1.31.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-22 01:20:30.000000 botocore-a-la-carte-internetmonitor-1.31.9/setup.py
```

### Comparing `botocore-a-la-carte-internetmonitor-1.31.8/LICENSE.txt` & `botocore-a-la-carte-internetmonitor-1.31.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-internetmonitor-1.31.8/PKG-INFO` & `botocore-a-la-carte-internetmonitor-1.31.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-internetmonitor
-Version: 1.31.8
+Version: 1.31.9
 Summary: internetmonitor data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-internetmonitor-1.31.8/botocore/data/internetmonitor/2021-06-03/endpoint-rule-set-1.json` & `botocore-a-la-carte-internetmonitor-1.31.9/botocore/data/internetmonitor/2021-06-03/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-internetmonitor-1.31.8/botocore/data/internetmonitor/2021-06-03/service-2.json` & `botocore-a-la-carte-internetmonitor-1.31.9/botocore/data/internetmonitor/2021-06-03/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-internetmonitor-1.31.8/botocore_a_la_carte_internetmonitor.egg-info/PKG-INFO` & `botocore-a-la-carte-internetmonitor-1.31.9/botocore_a_la_carte_internetmonitor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-internetmonitor
-Version: 1.31.8
+Version: 1.31.9
 Summary: internetmonitor data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-internetmonitor-1.31.8/setup.py` & `botocore-a-la-carte-internetmonitor-1.31.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-internetmonitor',
-    version="1.31.8",
+    version="1.31.9",
     description='internetmonitor data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/internetmonitor/*/*.json'],
```
