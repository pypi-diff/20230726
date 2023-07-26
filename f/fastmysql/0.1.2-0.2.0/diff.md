# Comparing `tmp/fastmysql-0.1.2.tar.gz` & `tmp/fastmysql-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmysql-0.1.2.tar", last modified: Mon Jul 24 10:48:10 2023, max compression
+gzip compressed data, was "fastmysql-0.2.0.tar", last modified: Wed Jul 26 06:52:10 2023, max compression
```

## Comparing `fastmysql-0.1.2.tar` & `fastmysql-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 10:48:10.538402 fastmysql-0.1.2/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-24 10:48:10.538282 fastmysql-0.1.2/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.1.2/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 10:48:10.536602 fastmysql-0.1.2/fastmysql/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      208 2023-02-22 07:55:41.000000 fastmysql-0.1.2/fastmysql/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    47563 2023-07-24 10:45:49.000000 fastmysql-0.1.2/fastmysql/fastmysql.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-24 10:48:10.538063 fastmysql-0.1.2/fastmysql.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-24 10:48:10.000000 fastmysql-0.1.2/fastmysql.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      227 2023-07-24 10:48:10.000000 fastmysql-0.1.2/fastmysql.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-24 10:48:10.000000 fastmysql-0.1.2/fastmysql.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      131 2023-07-24 10:48:10.000000 fastmysql-0.1.2/fastmysql.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-24 10:48:10.000000 fastmysql-0.1.2/fastmysql.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-24 10:48:10.538441 fastmysql-0.1.2/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1076 2023-07-24 10:47:46.000000 fastmysql-0.1.2/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 06:52:10.147163 fastmysql-0.2.0/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 06:52:10.147045 fastmysql-0.2.0/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1442 2023-02-22 07:55:41.000000 fastmysql-0.2.0/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 06:52:10.145950 fastmysql-0.2.0/fastmysql/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      238 2023-07-26 03:48:57.000000 fastmysql-0.2.0/fastmysql/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    47563 2023-07-24 10:45:49.000000 fastmysql-0.2.0/fastmysql/fastmysql.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    25482 2023-07-26 06:51:37.000000 fastmysql-0.2.0/fastmysql/fastmysql_test.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2023-07-26 06:52:10.146869 fastmysql-0.2.0/fastmysql.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1775 2023-07-26 06:52:10.000000 fastmysql-0.2.0/fastmysql.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      255 2023-07-26 06:52:10.000000 fastmysql-0.2.0/fastmysql.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2023-07-26 06:52:10.000000 fastmysql-0.2.0/fastmysql.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      146 2023-07-26 06:52:10.000000 fastmysql-0.2.0/fastmysql.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       10 2023-07-26 06:52:10.000000 fastmysql-0.2.0/fastmysql.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2023-07-26 06:52:10.147209 fastmysql-0.2.0/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1102 2023-07-26 06:51:37.000000 fastmysql-0.2.0/setup.py
```

### Comparing `fastmysql-0.1.2/PKG-INFO` & `fastmysql-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.1.2
+Version: 0.2.0
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.1.2/README.md` & `fastmysql-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fastmysql-0.1.2/fastmysql/fastmysql.py` & `fastmysql-0.2.0/fastmysql/fastmysql.py`

 * *Files identical despite different names*

### Comparing `fastmysql-0.1.2/fastmysql.egg-info/PKG-INFO` & `fastmysql-0.2.0/fastmysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastmysql
-Version: 0.1.2
+Version: 0.2.0
 Summary: make it easy to use pymysql
 Home-page: https://gitee.com/ZeroSeeker/fastmysql
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `fastmysql-0.1.2/setup.py` & `fastmysql-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fastmysql",
-    version="0.1.2",
+    version="0.2.0",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     description="make it easy to use pymysql",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/ZeroSeeker/fastmysql",
     packages=setuptools.find_packages(),
@@ -31,10 +31,11 @@
         'numpy>=1.19.5',
         'pandas>=1.3.5',
         'PyMySQL==1.0.2',
         'python-dateutil==2.8.2',
         'pytz==2022.1',
         'showlog>=0.0.6',
         'six==1.16.0',
-        'tqdm==4.61.2'
+        'tqdm==4.61.2',
+        'DBUtils==3.0.3'
     ]
 )
```

