# Comparing `tmp/PastebinReaderPy-0.9.9.tar.gz` & `tmp/PastebinReaderPy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PastebinReaderPy-0.9.9.tar", last modified: Wed Jul 26 19:04:07 2023, max compression
+gzip compressed data, was "PastebinReaderPy-1.0.0.tar", last modified: Wed Jul 26 19:15:00 2023, max compression
```

## Comparing `PastebinReaderPy-0.9.9.tar` & `PastebinReaderPy-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:04:07.278130 PastebinReaderPy-0.9.9/
--rw-r--r--   0 artem      (502) staff       (20)     1217 2023-07-26 19:04:07.278431 PastebinReaderPy-0.9.9/PKG-INFO
-drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:04:07.275739 PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/
--rw-r--r--   0 artem      (502) staff       (20)     1217 2023-07-26 19:04:07.000000 PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/PKG-INFO
--rw-r--r--   0 artem      (502) staff       (20)      209 2023-07-26 19:04:07.000000 PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/SOURCES.txt
--rw-r--r--   0 artem      (502) staff       (20)        1 2023-07-26 19:04:07.000000 PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/dependency_links.txt
--rw-r--r--   0 artem      (502) staff       (20)        9 2023-07-26 19:04:07.000000 PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/top_level.txt
--rw-r--r--   0 artem      (502) staff       (20)      814 2023-07-26 19:02:16.000000 PastebinReaderPy-0.9.9/README.md
-drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:04:07.276277 PastebinReaderPy-0.9.9/pastebin/
--rw-r--r--   0 artem      (502) staff       (20)      464 2023-07-26 14:03:23.000000 PastebinReaderPy-0.9.9/pastebin/__init__.py
--rw-r--r--   0 artem      (502) staff       (20)       38 2023-07-26 19:04:07.279343 PastebinReaderPy-0.9.9/setup.cfg
--rw-r--r--   0 artem      (502) staff       (20)      591 2023-07-26 19:02:30.000000 PastebinReaderPy-0.9.9/setup.py
+drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:15:00.362338 PastebinReaderPy-1.0.0/
+-rw-r--r--   0 artem      (502) staff       (20)     1224 2023-07-26 19:15:00.361715 PastebinReaderPy-1.0.0/PKG-INFO
+drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:15:00.359516 PastebinReaderPy-1.0.0/PastebinReaderPy.egg-info/
+-rw-r--r--   0 artem      (502) staff       (20)     1224 2023-07-26 19:15:00.000000 PastebinReaderPy-1.0.0/PastebinReaderPy.egg-info/PKG-INFO
+-rw-r--r--   0 artem      (502) staff       (20)      206 2023-07-26 19:15:00.000000 PastebinReaderPy-1.0.0/PastebinReaderPy.egg-info/SOURCES.txt
+-rw-r--r--   0 artem      (502) staff       (20)        1 2023-07-26 19:15:00.000000 PastebinReaderPy-1.0.0/PastebinReaderPy.egg-info/dependency_links.txt
+-rw-r--r--   0 artem      (502) staff       (20)       16 2023-07-26 19:15:00.000000 PastebinReaderPy-1.0.0/PastebinReaderPy.egg-info/top_level.txt
+-rw-r--r--   0 artem      (502) staff       (20)      821 2023-07-26 19:14:52.000000 PastebinReaderPy-1.0.0/README.md
+drwxr-xr-x   0 artem      (502) staff       (20)        0 2023-07-26 19:15:00.360015 PastebinReaderPy-1.0.0/pastebin_reader/
+-rw-r--r--   0 artem      (502) staff       (20)      464 2023-07-26 14:03:23.000000 PastebinReaderPy-1.0.0/pastebin_reader/__init__.py
+-rw-r--r--   0 artem      (502) staff       (20)       38 2023-07-26 19:15:00.362575 PastebinReaderPy-1.0.0/setup.cfg
+-rw-r--r--   0 artem      (502) staff       (20)      598 2023-07-26 19:14:26.000000 PastebinReaderPy-1.0.0/setup.py
```

### Comparing `PastebinReaderPy-0.9.9/PKG-INFO` & `PastebinReaderPy-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PastebinReaderPy
-Version: 0.9.9
+Version: 1.0.0
 Summary: Python Pastebin Library for reading and running pastes
 Author: Dolenko10.0Artem10.0
 Author-email: artemdolenko.ua@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -29,15 +29,15 @@
    - _This function return paste's varible_
 3. run_paste(paste_id:str) -> None
    - _This function run paste's python code_
 
 ### Usage
 ```
 
->>> import pastebin as pr
+>>> import pastebin_reader as pr
 >>> pr.read_paste('uQS3TJgS') # for reading example id = uQS3TJgS
 '{\n    "English": "en",\n    "Chinese": "zh",\n    "Ukrainian": "uk",\n    "Polish": "pl"\n}'
 >>> pr.read_var_paste('uQS3TJgS')
 {'English': 'en', 'Chinese': 'zh', 'Ukrainian': 'uk', 'Polish': 'pl'}
 >>> pr.run_paste('tLDZ9p7w') # for running example id = tLDZ9p7w
 Hello, World!
```

### Comparing `PastebinReaderPy-0.9.9/PastebinReaderPy.egg-info/PKG-INFO` & `PastebinReaderPy-1.0.0/PastebinReaderPy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PastebinReaderPy
-Version: 0.9.9
+Version: 1.0.0
 Summary: Python Pastebin Library for reading and running pastes
 Author: Dolenko10.0Artem10.0
 Author-email: artemdolenko.ua@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -29,15 +29,15 @@
    - _This function return paste's varible_
 3. run_paste(paste_id:str) -> None
    - _This function run paste's python code_
 
 ### Usage
 ```
 
->>> import pastebin as pr
+>>> import pastebin_reader as pr
 >>> pr.read_paste('uQS3TJgS') # for reading example id = uQS3TJgS
 '{\n    "English": "en",\n    "Chinese": "zh",\n    "Ukrainian": "uk",\n    "Polish": "pl"\n}'
 >>> pr.read_var_paste('uQS3TJgS')
 {'English': 'en', 'Chinese': 'zh', 'Ukrainian': 'uk', 'Polish': 'pl'}
 >>> pr.run_paste('tLDZ9p7w') # for running example id = tLDZ9p7w
 Hello, World!
```

### Comparing `PastebinReaderPy-0.9.9/README.md` & `PastebinReaderPy-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
    - _This function return paste's varible_
 3. run_paste(paste_id:str) -> None
    - _This function run paste's python code_
 
 ### Usage
 ```
 
->>> import pastebin as pr
+>>> import pastebin_reader as pr
 >>> pr.read_paste('uQS3TJgS') # for reading example id = uQS3TJgS
 '{\n    "English": "en",\n    "Chinese": "zh",\n    "Ukrainian": "uk",\n    "Polish": "pl"\n}'
 >>> pr.read_var_paste('uQS3TJgS')
 {'English': 'en', 'Chinese': 'zh', 'Ukrainian': 'uk', 'Polish': 'pl'}
 >>> pr.run_paste('tLDZ9p7w') # for running example id = tLDZ9p7w
 Hello, World!
```

### Comparing `PastebinReaderPy-0.9.9/setup.py` & `PastebinReaderPy-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 with open(r'README.md', 'r', encoding='utf-8') as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name='PastebinReaderPy',
-	version='0.9.9',
+	version='1.0.0',
 	author='Dolenko10.0Artem10.0',
 	author_email='artemdolenko.ua@gmail.com',
 	description='Python Pastebin Library for reading and running pastes',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
-	packages=['pastebin'],
+	packages=['pastebin_reader'],
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: MIT License",
 		"Operating System :: OS Independent",
 	],
 	python_requires='>=3.6',
 )
```

