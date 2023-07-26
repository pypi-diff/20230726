# Comparing `tmp/PastebinReaderPy-0.9.10.tar.gz` & `tmp/PastebinReaderPy-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PastebinReaderPy-0.9.10.tar", last modified: Wed Jul 26 19:10:39 2023, max compression
+gzip compressed data, was "PastebinReaderPy-0.9.9.tar", last modified: Wed Jul 26 19:04:07 2023, max compression
```

## Comparing `PastebinReaderPy-0.9.10.tar` & `PastebinReaderPy-0.9.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:10:39.837591 PastebinReaderPy-0.9.10/
--rw-r--r--   0 artem      (502) staff       (20)     1218 2023-07-26 19:10:39.837020 PastebinReaderPy-0.9.10/PKG-INFO
-drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:10:39.834405 PastebinReaderPy-0.9.10/PastebinReaderPy.egg-info/
--rw-r--r--   0 artem      (502) staff       (20)     1218 2023-07-26 19:10:39.000000 PastebinReaderPy-0.9.10/PastebinReaderPy.egg-info/PKG-INFO
--rw-r--r--   0 artem      (502) staff       (20)      199 2023-07-26 19:10:39.000000 PastebinReaderPy-0.9.10/PastebinReaderPy.egg-info/SOURCES.txt
--rw-r--r--   0 artem      (502) staff       (20)        1 2023-07-26 19:10:39.000000 PastebinReaderPy-0.9.10/PastebinReaderPy.egg-info/dependency_links.txt
--rw-r--r--   0 artem      (502) staff       (20)        9 2023-07-26 19:10:39.000000 PastebinReaderPy-0.9.10/PastebinReaderPy.egg-info/top_level.txt
--rw-r--r--   0 artem      (502) staff       (20)      814 2023-07-26 19:02:16.000000 PastebinReaderPy-0.9.10/README.md
-drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:10:39.834901 PastebinReaderPy-0.9.10/pastebin/
--rw-r--r--   0 artem      (502) staff       (20)      464 2023-07-26 14:03:23.000000 PastebinReaderPy-0.9.10/pastebin/__init__.py
--rw-r--r--   0 artem      (502) staff       (20)       38 2023-07-26 19:10:39.837880 PastebinReaderPy-0.9.10/setup.cfg
--rw-r--r--   0 artem      (502) staff       (20)      592 2023-07-26 19:10:04.000000 PastebinReaderPy-0.9.10/setup.py
+drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:04:07.278130 PastebinReaderPy-0.9.9/
+-rw-r--r--   0 artem      (502) staff       (20)     1217 2023-07-26 19:04:07.278431 PastebinReaderPy-0.9.9/PKG-INFO
+drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:04:07.275739 PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/
+-rw-r--r--   0 artem      (502) staff       (20)     1217 2023-07-26 19:04:07.000000 PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/PKG-INFO
+-rw-r--r--   0 artem      (502) staff       (20)      209 2023-07-26 19:04:07.000000 PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/SOURCES.txt
+-rw-r--r--   0 artem      (502) staff       (20)        1 2023-07-26 19:04:07.000000 PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/dependency_links.txt
+-rw-r--r--   0 artem      (502) staff       (20)        9 2023-07-26 19:04:07.000000 PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/top_level.txt
+-rw-r--r--   0 artem      (502) staff       (20)      814 2023-07-26 19:02:16.000000 PastebinReaderPy-0.9.9/README.md
+drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:04:07.276277 PastebinReaderPy-0.9.9/pastebin/
+-rw-r--r--   0 artem      (502) staff       (20)      464 2023-07-26 14:03:23.000000 PastebinReaderPy-0.9.9/pastebin/__init__.py
+-rw-r--r--   0 artem      (502) staff       (20)       38 2023-07-26 19:04:07.279343 PastebinReaderPy-0.9.9/setup.cfg
+-rw-r--r--   0 artem      (502) staff       (20)      591 2023-07-26 19:02:30.000000 PastebinReaderPy-0.9.9/setup.py
```

### Comparing `PastebinReaderPy-0.9.10/PKG-INFO` & `PastebinReaderPy-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PastebinReaderPy
-Version: 0.9.10
+Version: 0.9.9
 Summary: Python Pastebin Library for reading and running pastes
 Author: Dolenko10.0Artem10.0
 Author-email: artemdolenko.ua@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `PastebinReaderPy-0.9.10/PastebinReaderPy.egg-info/PKG-INFO` & `PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PastebinReaderPy
-Version: 0.9.10
+Version: 0.9.9
 Summary: Python Pastebin Library for reading and running pastes
 Author: Dolenko10.0Artem10.0
 Author-email: artemdolenko.ua@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `PastebinReaderPy-0.9.10/README.md` & `PastebinReaderPy-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `PastebinReaderPy-0.9.10/setup.py` & `PastebinReaderPy-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open(r'README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='PastebinReaderPy',
-	version='0.9.10',
+	version='0.9.9',
 	author='Dolenko10.0Artem10.0',
 	author_email='artemdolenko.ua@gmail.com',
 	description='Python Pastebin Library for reading and running pastes',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	packages=['pastebin'],
 	classifiers=[
```

