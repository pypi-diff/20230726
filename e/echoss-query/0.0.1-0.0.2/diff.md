# Comparing `tmp/echoss_query-0.0.1.tar.gz` & `tmp/echoss_query-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoss_query-0.0.1.tar", last modified: Wed Jul 26 02:28:30 2023, max compression
+gzip compressed data, was "echoss_query-0.0.2.tar", last modified: Wed Jul 26 02:34:39 2023, max compression
```

## Comparing `echoss_query-0.0.1.tar` & `echoss_query-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:28:30.468254 echoss_query-0.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2813 2023-07-26 02:28:30.468254 echoss_query-0.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2481 2023-07-26 01:53:50.000000 echoss_query-0.0.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:28:30.468254 echoss_query-0.0.1/echoss_query/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      162 2023-07-26 01:53:50.000000 echoss_query-0.0.1/echoss_query/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:28:30.468254 echoss_query-0.0.1/echoss_query.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2813 2023-07-26 02:28:30.000000 echoss_query-0.0.1/echoss_query.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      187 2023-07-26 02:28:30.000000 echoss_query-0.0.1/echoss_query.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-26 02:28:30.000000 echoss_query-0.0.1/echoss_query.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-07-26 02:28:30.000000 echoss_query-0.0.1/echoss_query.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-26 02:28:30.468254 echoss_query-0.0.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2023-07-26 02:28:28.000000 echoss_query-0.0.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:34:39.669936 echoss_query-0.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2813 2023-07-26 02:34:39.669936 echoss_query-0.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2481 2023-07-26 01:53:50.000000 echoss_query-0.0.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:34:39.669936 echoss_query-0.0.2/echoss_query/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      160 2023-07-26 02:32:29.000000 echoss_query-0.0.2/echoss_query/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:34:39.669936 echoss_query-0.0.2/echoss_query.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2813 2023-07-26 02:34:39.000000 echoss_query-0.0.2/echoss_query.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      187 2023-07-26 02:34:39.000000 echoss_query-0.0.2/echoss_query.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-26 02:34:39.000000 echoss_query-0.0.2/echoss_query.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-07-26 02:34:39.000000 echoss_query-0.0.2/echoss_query.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-26 02:34:39.669936 echoss_query-0.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2023-07-26 02:34:34.000000 echoss_query-0.0.2/setup.py
```

### Comparing `echoss_query-0.0.1/PKG-INFO` & `echoss_query-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoss_query
-Version: 0.0.1
+Version: 0.0.2
 Summary: echoss AI Bigdata Solution - Query Package
 Home-page: 
 Author: incheolshin
 Author-email: incheolshin@12cm.co.kr
 Requires: pandas
 Requires: pymongo
 Requires: PyMySQL
```

### Comparing `echoss_query-0.0.1/README.md` & `echoss_query-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `echoss_query-0.0.1/echoss_query.egg-info/PKG-INFO` & `echoss_query-0.0.2/echoss_query.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoss-query
-Version: 0.0.1
+Version: 0.0.2
 Summary: echoss AI Bigdata Solution - Query Package
 Home-page: 
 Author: incheolshin
 Author-email: incheolshin@12cm.co.kr
 Requires: pandas
 Requires: pymongo
 Requires: PyMySQL
```

### Comparing `echoss_query-0.0.1/setup.py` & `echoss_query-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, Extension
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 print(long_description)
 setup(
     name='echoss_query',
-    version='0.0.1',
+    version='0.0.2',
     packages=['echoss_query'],
     url='',
     requires=['pandas','pymongo','PyMySQL','PyYAML','opensearch'],
     license='',
     author='incheolshin',
     author_email='incheolshin@12cm.co.kr',
     description='echoss AI Bigdata Solution - Query Package',
```

