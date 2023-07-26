# Comparing `tmp/echoss_query-0.0.3.tar.gz` & `tmp/echoss_query-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echoss_query-0.0.3.tar", last modified: Wed Jul 26 02:42:02 2023, max compression
+gzip compressed data, was "echoss_query-0.0.4.tar", last modified: Wed Jul 26 02:58:29 2023, max compression
```

## Comparing `echoss_query-0.0.3.tar` & `echoss_query-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:42:02.676297 echoss_query-0.0.3/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2813 2023-07-26 02:42:02.676297 echoss_query-0.0.3/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2481 2023-07-26 01:53:50.000000 echoss_query-0.0.3/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:42:02.676297 echoss_query-0.0.3/echoss_query/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-07-26 02:40:36.000000 echoss_query-0.0.3/echoss_query/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:42:02.676297 echoss_query-0.0.3/echoss_query.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2813 2023-07-26 02:42:02.000000 echoss_query-0.0.3/echoss_query.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      187 2023-07-26 02:42:02.000000 echoss_query-0.0.3/echoss_query.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-26 02:42:02.000000 echoss_query-0.0.3/echoss_query.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-07-26 02:42:02.000000 echoss_query-0.0.3/echoss_query.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-26 02:42:02.676297 echoss_query-0.0.3/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2023-07-26 02:41:39.000000 echoss_query-0.0.3/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:58:29.634132 echoss_query-0.0.4/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2813 2023-07-26 02:58:29.634132 echoss_query-0.0.4/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2481 2023-07-26 01:53:50.000000 echoss_query-0.0.4/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:58:29.634132 echoss_query-0.0.4/echoss_query/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      131 2023-07-26 02:40:36.000000 echoss_query-0.0.4/echoss_query/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:58:29.634132 echoss_query-0.0.4/echoss_query/project_control/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-07-26 02:39:42.000000 echoss_query-0.0.4/echoss_query/project_control/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8840 2023-07-26 01:53:50.000000 echoss_query-0.0.4/echoss_query/project_control/project_generator.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:58:29.634132 echoss_query-0.0.4/echoss_query/query/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       80 2023-07-26 02:47:18.000000 echoss_query-0.0.4/echoss_query/query/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25846 2023-07-26 01:53:50.000000 echoss_query-0.0.4/echoss_query/query/echoss_query.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 02:58:29.634132 echoss_query-0.0.4/echoss_query.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2813 2023-07-26 02:58:29.000000 echoss_query-0.0.4/echoss_query.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      344 2023-07-26 02:58:29.000000 echoss_query-0.0.4/echoss_query.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-26 02:58:29.000000 echoss_query-0.0.4/echoss_query.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-07-26 02:58:29.000000 echoss_query-0.0.4/echoss_query.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-26 02:58:29.634132 echoss_query-0.0.4/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      740 2023-07-26 02:58:27.000000 echoss_query-0.0.4/setup.py
```

### Comparing `echoss_query-0.0.3/PKG-INFO` & `echoss_query-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoss_query
-Version: 0.0.3
+Version: 0.0.4
 Summary: echoss AI Bigdata Solution - Query Package
 Home-page: 
 Author: incheolshin
 Author-email: incheolshin@12cm.co.kr
 Requires: pandas
 Requires: pymongo
 Requires: PyMySQL
```

### Comparing `echoss_query-0.0.3/README.md` & `echoss_query-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `echoss_query-0.0.3/echoss_query.egg-info/PKG-INFO` & `echoss_query-0.0.4/echoss_query.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echoss-query
-Version: 0.0.3
+Version: 0.0.4
 Summary: echoss AI Bigdata Solution - Query Package
 Home-page: 
 Author: incheolshin
 Author-email: incheolshin@12cm.co.kr
 Requires: pandas
 Requires: pymongo
 Requires: PyMySQL
```

### Comparing `echoss_query-0.0.3/setup.py` & `echoss_query-0.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-from setuptools import setup, Extension
+from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-print(long_description)
+
+package_name = "echoss_query"
+
+packages = [
+    package
+    for package in find_packages(where=".")
+    if package == package_name or package.startswith(package_name + ".")
+]
+
 setup(
     name='echoss_query',
-    version='0.0.3',
-    packages=['echoss_query'],
+    version='0.0.4',
     url='',
     requires=['pandas','pymongo','PyMySQL','PyYAML','opensearch'],
     license='',
     author='incheolshin',
     author_email='incheolshin@12cm.co.kr',
     description='echoss AI Bigdata Solution - Query Package',
     long_description=long_description,
     long_description_content_type='text/markdown',
+    packages=find_packages(),
     package_data={},
     python_requires= '>3.7',
 )
```

