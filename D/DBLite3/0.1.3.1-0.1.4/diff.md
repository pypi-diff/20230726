# Comparing `tmp/DBLite3-0.1.3.1.tar.gz` & `tmp/DBLite3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DBLite3-0.1.3.1.tar", last modified: Wed Jul 19 22:27:10 2023, max compression
+gzip compressed data, was "DBLite3-0.1.4.tar", last modified: Wed Jul 26 13:02:07 2023, max compression
```

## Comparing `DBLite3-0.1.3.1.tar` & `DBLite3-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-19 22:27:10.750603 DBLite3-0.1.3.1/
-drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-19 22:27:10.747890 DBLite3-0.1.3.1/DBLite3/
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      600 2023-07-19 22:27:07.000000 DBLite3-0.1.3.1/DBLite3/__init__.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1585 2023-07-19 22:27:07.000000 DBLite3-0.1.3.1/DBLite3/_alter.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     2456 2023-07-19 22:27:07.000000 DBLite3-0.1.3.1/DBLite3/_create.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1311 2023-07-19 22:27:07.000000 DBLite3-0.1.3.1/DBLite3/_delete.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1385 2023-07-19 22:27:07.000000 DBLite3-0.1.3.1/DBLite3/_drop.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)       89 2023-07-19 12:06:19.000000 DBLite3-0.1.3.1/DBLite3/_exceptions.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     2697 2023-07-19 20:27:58.000000 DBLite3-0.1.3.1/DBLite3/_funcs.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     2110 2023-07-19 22:27:07.000000 DBLite3-0.1.3.1/DBLite3/_insert.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     2241 2023-07-19 22:27:07.000000 DBLite3-0.1.3.1/DBLite3/_select.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1529 2023-07-19 22:27:07.000000 DBLite3-0.1.3.1/DBLite3/_update.py
-drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-19 22:27:10.748543 DBLite3-0.1.3.1/DBLite3.egg-info/
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    13009 2023-07-19 22:27:10.000000 DBLite3-0.1.3.1/DBLite3.egg-info/PKG-INFO
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      513 2023-07-19 22:27:10.000000 DBLite3-0.1.3.1/DBLite3.egg-info/SOURCES.txt
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)        1 2023-07-19 22:27:10.000000 DBLite3-0.1.3.1/DBLite3.egg-info/dependency_links.txt
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)        8 2023-07-19 22:27:10.000000 DBLite3-0.1.3.1/DBLite3.egg-info/top_level.txt
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1073 2023-07-12 12:06:01.000000 DBLite3-0.1.3.1/LICENSE.txt
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    13009 2023-07-19 22:27:10.750715 DBLite3-0.1.3.1/PKG-INFO
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    11958 2023-07-19 22:27:07.000000 DBLite3-0.1.3.1/README.md
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)       38 2023-07-19 22:27:10.751027 DBLite3-0.1.3.1/setup.cfg
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1356 2023-07-19 22:27:07.000000 DBLite3-0.1.3.1/setup.py
-drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-19 22:27:10.750370 DBLite3-0.1.3.1/tests/
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      745 2023-07-19 20:31:38.000000 DBLite3-0.1.3.1/tests/test_1_create.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      687 2023-07-19 20:34:06.000000 DBLite3-0.1.3.1/tests/test_2_insert.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      799 2023-07-19 20:34:06.000000 DBLite3-0.1.3.1/tests/test_3_update.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1060 2023-07-19 20:39:08.000000 DBLite3-0.1.3.1/tests/test_4_alter.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1040 2023-07-19 20:35:03.000000 DBLite3-0.1.3.1/tests/test_5_select.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      699 2023-07-19 20:39:47.000000 DBLite3-0.1.3.1/tests/test_6_delete.py
--rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      728 2023-07-19 20:46:39.000000 DBLite3-0.1.3.1/tests/test_7_drop.py
+drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:02:07.618768 DBLite3-0.1.4/
+drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:02:07.616087 DBLite3-0.1.4/DBLite3/
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      630 2023-07-25 17:25:13.000000 DBLite3-0.1.4/DBLite3/__init__.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4909 2023-07-26 11:43:04.000000 DBLite3-0.1.4/DBLite3/_alter.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    10323 2023-07-26 11:22:30.000000 DBLite3-0.1.4/DBLite3/_create.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4425 2023-07-26 11:43:04.000000 DBLite3-0.1.4/DBLite3/_delete.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1831 2023-07-26 10:34:33.000000 DBLite3-0.1.4/DBLite3/_drop.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     6519 2023-07-26 11:22:30.000000 DBLite3-0.1.4/DBLite3/_exceptions.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    12637 2023-07-26 10:34:33.000000 DBLite3-0.1.4/DBLite3/_funcs.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4716 2023-07-26 11:22:30.000000 DBLite3-0.1.4/DBLite3/_insert.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     6675 2023-07-26 12:59:19.000000 DBLite3-0.1.4/DBLite3/_select.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     4651 2023-07-26 11:22:30.000000 DBLite3-0.1.4/DBLite3/_update.py
+drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:02:07.616923 DBLite3-0.1.4/DBLite3.egg-info/
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    13422 2023-07-26 13:02:07.000000 DBLite3-0.1.4/DBLite3.egg-info/PKG-INFO
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      535 2023-07-26 13:02:07.000000 DBLite3-0.1.4/DBLite3.egg-info/SOURCES.txt
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)        1 2023-07-26 13:02:07.000000 DBLite3-0.1.4/DBLite3.egg-info/dependency_links.txt
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)        8 2023-07-26 13:02:07.000000 DBLite3-0.1.4/DBLite3.egg-info/top_level.txt
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1073 2023-07-20 13:51:31.000000 DBLite3-0.1.4/LICENSE.txt
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    13422 2023-07-26 13:02:07.618858 DBLite3-0.1.4/PKG-INFO
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)    12390 2023-07-25 17:25:13.000000 DBLite3-0.1.4/README.md
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)       38 2023-07-26 13:02:07.619192 DBLite3-0.1.4/setup.cfg
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1340 2023-07-25 17:25:13.000000 DBLite3-0.1.4/setup.py
+drwxr-xr-x   0 xeniakhrustaleva   (501) staff       (20)        0 2023-07-26 13:02:07.618473 DBLite3-0.1.4/tests/
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      745 2023-07-20 13:51:31.000000 DBLite3-0.1.4/tests/test_1_create.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      687 2023-07-20 13:51:31.000000 DBLite3-0.1.4/tests/test_2_insert.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      799 2023-07-20 13:51:31.000000 DBLite3-0.1.4/tests/test_3_update.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1060 2023-07-20 13:51:31.000000 DBLite3-0.1.4/tests/test_4_alter.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     1040 2023-07-20 13:51:31.000000 DBLite3-0.1.4/tests/test_5_select.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      699 2023-07-20 13:51:31.000000 DBLite3-0.1.4/tests/test_6_delete.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)      728 2023-07-20 13:51:31.000000 DBLite3-0.1.4/tests/test_7_drop.py
+-rw-r--r--   0 xeniakhrustaleva   (501) staff       (20)     3584 2023-07-26 06:28:59.000000 DBLite3-0.1.4/tests/test_8_funcs.py
```

### Comparing `DBLite3-0.1.3.1/DBLite3/__init__.py` & `DBLite3-0.1.4/DBLite3/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from DBLite3._create import *
 from DBLite3._insert import *
 from DBLite3._update import *
 from DBLite3._drop import *
 from DBLite3._alter import *
 from DBLite3._delete import *
 from DBLite3._select import *
-from DBLite3._exceptions import CreationError
+from DBLite3._exceptions import *
 from DBLite3._funcs import *
 
-
 # DBLite3 is NoSQL database.
 # DBLite3 could be used as simple DB for simple projects.
 # This DB creates file with file extension .json (JavaScript Object Notification).
 #
 # All information is stored in tables which contain collections.
 
 
-__version__ = '0.1.3.1'
-__author__ = "Alexander Nazimov (GitHub @macht1212)"
+__version__ = '0.1.4'
+__author__ = "Alexander Nazimov"
+__git__ = '@macht1212'
+__email__ = 'nasimov.alexander@gmail.com'
```

### Comparing `DBLite3-0.1.3.1/DBLite3/_delete.py` & `DBLite3-0.1.4/DBLite3/_drop.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,50 @@
-from DBLite3._funcs import _open_db, _save_db, _get_value_index
+import os
 
+from DBLite3._exceptions import DropError
+from DBLite3._funcs import _open_db, _save_db, _db_exists, _does_collection_exists, _object_exists
 
-def delete_value(db_name: str, collection: str, object: str, id: int) -> None:
+
+def drop_db(db_name: str) -> None:
+    """
+    The function deletes the database. IMPORTANT! Using this feature will result in data loss
+    :param db_name: the name of the database to be dropped
+    :return: None
+    """
+    if _db_exists(db_name=db_name):
+        os.remove(f'{db_name}.json')
+        return
+    else:
+        raise DropError(f'Database {db_name} does not exist.')
+
+
+def drop_collection(db_name: str, collection: str) -> None:
     """
-    The function deletes a value by its index
-    :param db_name: The name of the database to delete values to
-    :param collection: The name of the collection to delete values to
-    :param object: The name of the object to delete values to
-    :param id: ID of the value to delete
+    The function deletes the table from database. IMPORTANT! Using this feature will result in data loss
+    :param db_name: the name of the database to be modified
+    :param collection: the name of the collection to be dropped
     :return: None
     """
-    index = _get_value_index(db_name=db_name, collection=collection, object=object, id=id)
     DATABASE = _open_db(db_name=db_name)
-    if len(DATABASE[collection][object]['values']) == 1:
-        DATABASE[collection][object]['values'] = None
+    if _does_collection_exists(collection=collection, DB=DATABASE):
+        del (DATABASE[collection])
+        _save_db(db_name=db_name, DB=DATABASE)
+        return
     else:
-        del (DATABASE[collection][object]['values'][index])
-    _save_db(db_name=db_name, DB=DATABASE)
+        raise DropError(f'Collection {collection} does not exist.')
 
 
-def delete_all_values(db_name: str, collection: str, object: str) -> None:
+def drop_object(db_name: str, collection: str, object: str) -> None:
     """
-    The function deletes all values from database
-    :param db_name: The name of the database to delete values to
-    :param collection: The name of the collection to delete values to
-    :param object: The name of the object to delete values to
+    The function deletes the collection from database. IMPORTANT! Using this feature will result in data loss
+    :param db_name: the name of the database to be modified
+    :param collection: the name of the collection to be modified
+    :param object: the name of the object to be dropped
     :return: None
     """
     DATABASE = _open_db(db_name=db_name)
-    DATABASE[collection][object]['values'] = None
-    _save_db(db_name=db_name, DB=DATABASE)
+    if _object_exists(collection=collection, object=object, DB=DATABASE):
+        del (DATABASE[collection][object])
+        _save_db(db_name=db_name, DB=DATABASE)
+        return
+    else:
+        raise DropError(f'Object {object} does not exist.')
```

### Comparing `DBLite3-0.1.3.1/DBLite3.egg-info/PKG-INFO` & `DBLite3-0.1.4/DBLite3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: DBLite3
-Version: 0.1.3.1
+Version: 0.1.4
 Summary: NoSQL database
 Home-page: https://github.com/macht1212/LiteDB/
-Download-URL: https://github.com/macht1212/LiteDB/archive/0.1.3.1.tar.gz
-Author: Alexander Nazimov (GitHub @macht1212)
+Download-URL: https://github.com/macht1212/LiteDB/archive/0.1.4.tar.gz
+Author: Alexander Nazimov
 Author-email: nasimov.alexander@gmail.com
 License: MIT license
-Keywords: database,nosql,litedb
+Keywords: database,nosql,litedb,json
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -22,15 +22,16 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # ![Icon](img/icon.svg) DBLite3
-![Static Badge](https://img.shields.io/badge/LiteDB-v0.1.1-blue)
+
+![Static Badge](https://img.shields.io/badge/LiteDB-v0.1.4-blue)
 
 
 DBLite3 is NoSQL database.
 DBLite3 could be used as simple DB for simple projects.
 This DB creates file with file extension **.json** (JavaScript Object Notification).
 
 ## Documentation
@@ -407,21 +408,31 @@
 
 Install my-project with pip
 
 ```bash
   pip install DBLite3
 ```
 
+
+## RoadMap
+* Add a few variants of inserts (one-in-one, one-in-many, many-to-one, many-to-many)
+* Add description field to *.create_db* method (optional)
+* Add restrictions to values (uniqueness, insertion restriction, data type restriction)
+* Using any data encryption library, implement a secure way to work with the database
+* Add the ability to select values from all collections and objects together and compare
+
+
+
 ## Authors
 
 - [@macht1212](https://www.github.com/macht1212) Alexander Nazimov
 
 
 ## License
 
 [MIT](https://github.com/macht1212/LiteDB/blob/0711686a88e82182ed37199da73cea1b7595a75d/LICENSE.txt)
 
 
-## Lessons Learned
+[//]: # (## Lessons Learned)
```

### Comparing `DBLite3-0.1.3.1/DBLite3.egg-info/SOURCES.txt` & `DBLite3-0.1.4/DBLite3.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 DBLite3.egg-info/top_level.txt
 tests/test_1_create.py
 tests/test_2_insert.py
 tests/test_3_update.py
 tests/test_4_alter.py
 tests/test_5_select.py
 tests/test_6_delete.py
-tests/test_7_drop.py
+tests/test_7_drop.py
+tests/test_8_funcs.py
```

### Comparing `DBLite3-0.1.3.1/LICENSE.txt` & `DBLite3-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.3.1/PKG-INFO` & `DBLite3-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: DBLite3
-Version: 0.1.3.1
+Version: 0.1.4
 Summary: NoSQL database
 Home-page: https://github.com/macht1212/LiteDB/
-Download-URL: https://github.com/macht1212/LiteDB/archive/0.1.3.1.tar.gz
-Author: Alexander Nazimov (GitHub @macht1212)
+Download-URL: https://github.com/macht1212/LiteDB/archive/0.1.4.tar.gz
+Author: Alexander Nazimov
 Author-email: nasimov.alexander@gmail.com
 License: MIT license
-Keywords: database,nosql,litedb
+Keywords: database,nosql,litedb,json
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -22,15 +22,16 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # ![Icon](img/icon.svg) DBLite3
-![Static Badge](https://img.shields.io/badge/LiteDB-v0.1.1-blue)
+
+![Static Badge](https://img.shields.io/badge/LiteDB-v0.1.4-blue)
 
 
 DBLite3 is NoSQL database.
 DBLite3 could be used as simple DB for simple projects.
 This DB creates file with file extension **.json** (JavaScript Object Notification).
 
 ## Documentation
@@ -407,21 +408,31 @@
 
 Install my-project with pip
 
 ```bash
   pip install DBLite3
 ```
 
+
+## RoadMap
+* Add a few variants of inserts (one-in-one, one-in-many, many-to-one, many-to-many)
+* Add description field to *.create_db* method (optional)
+* Add restrictions to values (uniqueness, insertion restriction, data type restriction)
+* Using any data encryption library, implement a secure way to work with the database
+* Add the ability to select values from all collections and objects together and compare
+
+
+
 ## Authors
 
 - [@macht1212](https://www.github.com/macht1212) Alexander Nazimov
 
 
 ## License
 
 [MIT](https://github.com/macht1212/LiteDB/blob/0711686a88e82182ed37199da73cea1b7595a75d/LICENSE.txt)
 
 
-## Lessons Learned
+[//]: # (## Lessons Learned)
```

### Comparing `DBLite3-0.1.3.1/README.md` & `DBLite3-0.1.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 # ![Icon](img/icon.svg) DBLite3
-![Static Badge](https://img.shields.io/badge/LiteDB-v0.1.1-blue)
+
+![Static Badge](https://img.shields.io/badge/LiteDB-v0.1.4-blue)
 
 
 DBLite3 is NoSQL database.
 DBLite3 could be used as simple DB for simple projects.
 This DB creates file with file extension **.json** (JavaScript Object Notification).
 
 ## Documentation
@@ -381,21 +382,31 @@
 
 Install my-project with pip
 
 ```bash
   pip install DBLite3
 ```
 
+
+## RoadMap
+* Add a few variants of inserts (one-in-one, one-in-many, many-to-one, many-to-many)
+* Add description field to *.create_db* method (optional)
+* Add restrictions to values (uniqueness, insertion restriction, data type restriction)
+* Using any data encryption library, implement a secure way to work with the database
+* Add the ability to select values from all collections and objects together and compare
+
+
+
 ## Authors
 
 - [@macht1212](https://www.github.com/macht1212) Alexander Nazimov
 
 
 ## License
 
 [MIT](https://github.com/macht1212/LiteDB/blob/0711686a88e82182ed37199da73cea1b7595a75d/LICENSE.txt)
 
 
-## Lessons Learned
+[//]: # (## Lessons Learned)
```

### Comparing `DBLite3-0.1.3.1/setup.py` & `DBLite3-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from setuptools import setup, find_packages
-from DBLite3 import __version__, __author__
+from setuptools import setup
+from DBLite3 import __version__, __author__, __email__
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="DBLite3",
     version=__version__,
     author=__author__,
-    author_email='nasimov.alexander@gmail.com',
+    author_email=__email__,
     description="NoSQL database",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/macht1212/LiteDB/",
     download_url="https://github.com/macht1212/LiteDB/archive/{}.tar.gz".format(__version__),
     packages=['DBLite3'],
     package_data={'DBLite3': ['__init__.py']},
-    keywords=['database', 'nosql', 'litedb'],
+    keywords=['database', 'nosql', 'litedb', 'json'],
     license="MIT license",
     python_requires=">=3.9",
     classifiers=[
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `DBLite3-0.1.3.1/tests/test_1_create.py` & `DBLite3-0.1.4/tests/test_1_create.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.3.1/tests/test_2_insert.py` & `DBLite3-0.1.4/tests/test_2_insert.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.3.1/tests/test_3_update.py` & `DBLite3-0.1.4/tests/test_3_update.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.3.1/tests/test_4_alter.py` & `DBLite3-0.1.4/tests/test_4_alter.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.3.1/tests/test_5_select.py` & `DBLite3-0.1.4/tests/test_5_select.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.3.1/tests/test_6_delete.py` & `DBLite3-0.1.4/tests/test_6_delete.py`

 * *Files identical despite different names*

### Comparing `DBLite3-0.1.3.1/tests/test_7_drop.py` & `DBLite3-0.1.4/tests/test_7_drop.py`

 * *Files identical despite different names*

