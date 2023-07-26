# Comparing `tmp/DBLite3-0.1.4.1.tar.gz` & `tmp/DBLite3-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DBLite3-0.1.4.1.tar", last modified: Wed Jul 26 13:38:41 2023, max compression
+gzip compressed data, was "DBLite3-0.1.4.2.tar", last modified: Wed Jul 26 13:46:21 2023, max compression
```

## Comparing `DBLite3-0.1.4.1.tar` & `DBLite3-0.1.4.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:38:41.456197 DBLite3-0.1.4.1/
-drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:38:41.453808 DBLite3-0.1.4.1/DBLite3/
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      632 2023-07-26 13:36:30.000000 DBLite3-0.1.4.1/DBLite3/__init__.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4909 2023-07-26 11:43:04.000000 DBLite3-0.1.4.1/DBLite3/_alter.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    10323 2023-07-26 11:22:30.000000 DBLite3-0.1.4.1/DBLite3/_create.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4425 2023-07-26 11:43:04.000000 DBLite3-0.1.4.1/DBLite3/_delete.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     6030 2023-07-26 13:36:30.000000 DBLite3-0.1.4.1/DBLite3/_drop.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     6519 2023-07-26 11:22:30.000000 DBLite3-0.1.4.1/DBLite3/_exceptions.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    12637 2023-07-26 10:34:33.000000 DBLite3-0.1.4.1/DBLite3/_funcs.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4716 2023-07-26 11:22:30.000000 DBLite3-0.1.4.1/DBLite3/_insert.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     6675 2023-07-26 12:59:19.000000 DBLite3-0.1.4.1/DBLite3/_select.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4651 2023-07-26 11:22:30.000000 DBLite3-0.1.4.1/DBLite3/_update.py
-drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:38:41.454421 DBLite3-0.1.4.1/DBLite3.egg-info/
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    34413 2023-07-26 13:38:41.000000 DBLite3-0.1.4.1/DBLite3.egg-info/PKG-INFO
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      535 2023-07-26 13:38:41.000000 DBLite3-0.1.4.1/DBLite3.egg-info/SOURCES.txt
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)        1 2023-07-26 13:38:41.000000 DBLite3-0.1.4.1/DBLite3.egg-info/dependency_links.txt
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)        8 2023-07-26 13:38:41.000000 DBLite3-0.1.4.1/DBLite3.egg-info/top_level.txt
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1073 2023-07-20 13:51:31.000000 DBLite3-0.1.4.1/LICENSE.txt
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    34413 2023-07-26 13:38:41.456279 DBLite3-0.1.4.1/PKG-INFO
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    33377 2023-07-26 13:36:30.000000 DBLite3-0.1.4.1/README.md
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)       38 2023-07-26 13:38:41.456483 DBLite3-0.1.4.1/setup.cfg
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1340 2023-07-25 17:25:13.000000 DBLite3-0.1.4.1/setup.py
-drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:38:41.455922 DBLite3-0.1.4.1/tests/
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      745 2023-07-20 13:51:31.000000 DBLite3-0.1.4.1/tests/test_1_create.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      687 2023-07-20 13:51:31.000000 DBLite3-0.1.4.1/tests/test_2_insert.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      799 2023-07-20 13:51:31.000000 DBLite3-0.1.4.1/tests/test_3_update.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1060 2023-07-20 13:51:31.000000 DBLite3-0.1.4.1/tests/test_4_alter.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1040 2023-07-20 13:51:31.000000 DBLite3-0.1.4.1/tests/test_5_select.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      699 2023-07-20 13:51:31.000000 DBLite3-0.1.4.1/tests/test_6_delete.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      728 2023-07-20 13:51:31.000000 DBLite3-0.1.4.1/tests/test_7_drop.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     3584 2023-07-26 06:28:59.000000 DBLite3-0.1.4.1/tests/test_8_funcs.py
+drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:46:21.683870 DBLite3-0.1.4.2/
+drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:46:21.681506 DBLite3-0.1.4.2/DBLite3/
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      632 2023-07-26 13:46:06.000000 DBLite3-0.1.4.2/DBLite3/__init__.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4909 2023-07-26 11:43:04.000000 DBLite3-0.1.4.2/DBLite3/_alter.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    10323 2023-07-26 11:22:30.000000 DBLite3-0.1.4.2/DBLite3/_create.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4425 2023-07-26 11:43:04.000000 DBLite3-0.1.4.2/DBLite3/_delete.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     6030 2023-07-26 13:36:30.000000 DBLite3-0.1.4.2/DBLite3/_drop.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     6519 2023-07-26 11:22:30.000000 DBLite3-0.1.4.2/DBLite3/_exceptions.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    12637 2023-07-26 10:34:33.000000 DBLite3-0.1.4.2/DBLite3/_funcs.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4716 2023-07-26 11:22:30.000000 DBLite3-0.1.4.2/DBLite3/_insert.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     6675 2023-07-26 12:59:19.000000 DBLite3-0.1.4.2/DBLite3/_select.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4651 2023-07-26 11:22:30.000000 DBLite3-0.1.4.2/DBLite3/_update.py
+drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:46:21.682189 DBLite3-0.1.4.2/DBLite3.egg-info/
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    34418 2023-07-26 13:46:21.000000 DBLite3-0.1.4.2/DBLite3.egg-info/PKG-INFO
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      535 2023-07-26 13:46:21.000000 DBLite3-0.1.4.2/DBLite3.egg-info/SOURCES.txt
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)        1 2023-07-26 13:46:21.000000 DBLite3-0.1.4.2/DBLite3.egg-info/dependency_links.txt
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)        8 2023-07-26 13:46:21.000000 DBLite3-0.1.4.2/DBLite3.egg-info/top_level.txt
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1073 2023-07-20 13:51:31.000000 DBLite3-0.1.4.2/LICENSE.txt
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    34418 2023-07-26 13:46:21.683962 DBLite3-0.1.4.2/PKG-INFO
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    33377 2023-07-26 13:36:30.000000 DBLite3-0.1.4.2/README.md
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)       38 2023-07-26 13:46:21.684173 DBLite3-0.1.4.2/setup.cfg
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1337 2023-07-26 13:45:49.000000 DBLite3-0.1.4.2/setup.py
+drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:46:21.683596 DBLite3-0.1.4.2/tests/
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      745 2023-07-20 13:51:31.000000 DBLite3-0.1.4.2/tests/test_1_create.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      687 2023-07-20 13:51:31.000000 DBLite3-0.1.4.2/tests/test_2_insert.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      799 2023-07-20 13:51:31.000000 DBLite3-0.1.4.2/tests/test_3_update.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1060 2023-07-20 13:51:31.000000 DBLite3-0.1.4.2/tests/test_4_alter.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1040 2023-07-20 13:51:31.000000 DBLite3-0.1.4.2/tests/test_5_select.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      699 2023-07-20 13:51:31.000000 DBLite3-0.1.4.2/tests/test_6_delete.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      728 2023-07-20 13:51:31.000000 DBLite3-0.1.4.2/tests/test_7_drop.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     3584 2023-07-26 06:28:59.000000 DBLite3-0.1.4.2/tests/test_8_funcs.py
```

### Comparing `DBLite3-0.1.4.1/DBLite3/__init__.py` & `DBLite3-0.1.4.2/DBLite3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 # DBLite3 is NoSQL database.
 # DBLite3 could be used as simple DB for simple projects.
 # This DB creates file with file extension .json (JavaScript Object Notification).
 #
 # All information is stored in tables which contain collections.
 
 
-__version__ = '0.1.4.1'
+__version__ = '0.1.4.2'
 __author__ = "Alexander Nazimov"
 __git__ = '@macht1212'
 __email__ = 'nasimov.alexander@gmail.com'
```

### Comparing `DBLite3-0.1.4.1/DBLite3/_alter.py` & `DBLite3-0.1.4.2/DBLite3/_alter.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/DBLite3/_create.py` & `DBLite3-0.1.4.2/DBLite3/_create.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/DBLite3/_delete.py` & `DBLite3-0.1.4.2/DBLite3/_delete.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/DBLite3/_drop.py` & `DBLite3-0.1.4.2/DBLite3/_drop.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/DBLite3/_exceptions.py` & `DBLite3-0.1.4.2/DBLite3/_exceptions.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/DBLite3/_funcs.py` & `DBLite3-0.1.4.2/DBLite3/_funcs.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/DBLite3/_insert.py` & `DBLite3-0.1.4.2/DBLite3/_insert.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/DBLite3/_select.py` & `DBLite3-0.1.4.2/DBLite3/_select.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/DBLite3/_update.py` & `DBLite3-0.1.4.2/DBLite3/_update.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/DBLite3.egg-info/PKG-INFO` & `DBLite3-0.1.4.2/DBLite3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DBLite3
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: NoSQL database
 Home-page: https://github.com/macht1212/LiteDB/
-Download-URL: https://github.com/macht1212/LiteDB/archive/0.1.4.1.tar.gz
+Download-URL: https://github.com/macht1212/LiteDB/dist/DBLite3-0.1.4.2.tar.gz
 Author: Alexander Nazimov
 Author-email: nasimov.alexander@gmail.com
 License: MIT license
 Keywords: database,nosql,litedb,json
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DBLite3-0.1.4.1/DBLite3.egg-info/SOURCES.txt` & `DBLite3-0.1.4.2/DBLite3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/LICENSE.txt` & `DBLite3-0.1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/PKG-INFO` & `DBLite3-0.1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: DBLite3
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: NoSQL database
 Home-page: https://github.com/macht1212/LiteDB/
-Download-URL: https://github.com/macht1212/LiteDB/archive/0.1.4.1.tar.gz
+Download-URL: https://github.com/macht1212/LiteDB/dist/DBLite3-0.1.4.2.tar.gz
 Author: Alexander Nazimov
 Author-email: nasimov.alexander@gmail.com
 License: MIT license
 Keywords: database,nosql,litedb,json
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DBLite3-0.1.4.1/README.md` & `DBLite3-0.1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/setup.py` & `DBLite3-0.1.4.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     version=__version__,
     author=__author__,
     author_email=__email__,
     description="NoSQL database",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/macht1212/LiteDB/",
-    download_url="https://github.com/macht1212/LiteDB/archive/{}.tar.gz".format(__version__),
+    download_url=f"https://github.com/macht1212/LiteDB/dist/DBLite3-{__version__}.tar.gz",
     packages=['DBLite3'],
     package_data={'DBLite3': ['__init__.py']},
     keywords=['database', 'nosql', 'litedb', 'json'],
     license="MIT license",
     python_requires=">=3.9",
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `DBLite3-0.1.4.1/tests/test_1_create.py` & `DBLite3-0.1.4.2/tests/test_1_create.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/tests/test_2_insert.py` & `DBLite3-0.1.4.2/tests/test_2_insert.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/tests/test_3_update.py` & `DBLite3-0.1.4.2/tests/test_3_update.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/tests/test_4_alter.py` & `DBLite3-0.1.4.2/tests/test_4_alter.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/tests/test_5_select.py` & `DBLite3-0.1.4.2/tests/test_5_select.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/tests/test_6_delete.py` & `DBLite3-0.1.4.2/tests/test_6_delete.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/tests/test_7_drop.py` & `DBLite3-0.1.4.2/tests/test_7_drop.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.4.1/tests/test_8_funcs.py` & `DBLite3-0.1.4.2/tests/test_8_funcs.py`

 * *Files identical despite different names*

