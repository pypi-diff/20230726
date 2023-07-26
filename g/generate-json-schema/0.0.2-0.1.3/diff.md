# Comparing `tmp/generate-json-schema-0.0.2.tar.gz` & `tmp/generate-json-schema-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generate-json-schema-0.0.2.tar", last modified: Wed Jul 26 18:57:22 2023, max compression
+gzip compressed data, was "generate-json-schema-0.1.3.tar", last modified: Wed Jul 26 19:00:04 2023, max compression
```

## Comparing `generate-json-schema-0.0.2.tar` & `generate-json-schema-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-26 18:57:22.695479 generate-json-schema-0.0.2/
--rw-r--r--   0 fernnando   (501) staff       (20)     1233 2023-07-26 18:57:22.695104 generate-json-schema-0.0.2/PKG-INFO
--rw-r--r--   0 fernnando   (501) staff       (20)      520 2023-07-26 18:54:14.000000 generate-json-schema-0.0.2/README.rst
-drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-26 18:57:22.693022 generate-json-schema-0.0.2/generate_json_schema.egg-info/
--rw-r--r--   0 fernnando   (501) staff       (20)     1233 2023-07-26 18:57:22.000000 generate-json-schema-0.0.2/generate_json_schema.egg-info/PKG-INFO
--rw-r--r--   0 fernnando   (501) staff       (20)      234 2023-07-26 18:57:22.000000 generate-json-schema-0.0.2/generate_json_schema.egg-info/SOURCES.txt
--rw-r--r--   0 fernnando   (501) staff       (20)        1 2023-07-26 18:57:22.000000 generate-json-schema-0.0.2/generate_json_schema.egg-info/dependency_links.txt
--rw-r--r--   0 fernnando   (501) staff       (20)       22 2023-07-26 18:57:22.000000 generate-json-schema-0.0.2/generate_json_schema.egg-info/top_level.txt
--rw-r--r--   0 fernnando   (501) staff       (20)       38 2023-07-26 18:57:22.695611 generate-json-schema-0.0.2/setup.cfg
--rw-r--r--   0 fernnando   (501) staff       (20)     1763 2023-07-26 18:56:45.000000 generate-json-schema-0.0.2/setup.py
-drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-26 18:57:22.694094 generate-json-schema-0.0.2/src/
--rw-r--r--   0 fernnando   (501) staff       (20)        0 2023-07-25 18:41:19.000000 generate-json-schema-0.0.2/src/__init__.py
--rw-r--r--   0 fernnando   (501) staff       (20)     2056 2023-07-26 13:48:52.000000 generate-json-schema-0.0.2/src/generate_schema.py
+drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-26 19:00:04.166418 generate-json-schema-0.1.3/
+-rw-r--r--   0 fernnando   (501) staff       (20)     1234 2023-07-26 19:00:04.165785 generate-json-schema-0.1.3/PKG-INFO
+-rw-r--r--   0 fernnando   (501) staff       (20)      522 2023-07-26 18:59:42.000000 generate-json-schema-0.1.3/README.rst
+drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-26 19:00:04.163607 generate-json-schema-0.1.3/generate_json_schema.egg-info/
+-rw-r--r--   0 fernnando   (501) staff       (20)     1234 2023-07-26 19:00:04.000000 generate-json-schema-0.1.3/generate_json_schema.egg-info/PKG-INFO
+-rw-r--r--   0 fernnando   (501) staff       (20)      234 2023-07-26 19:00:04.000000 generate-json-schema-0.1.3/generate_json_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 fernnando   (501) staff       (20)        1 2023-07-26 19:00:04.000000 generate-json-schema-0.1.3/generate_json_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 fernnando   (501) staff       (20)       22 2023-07-26 19:00:04.000000 generate-json-schema-0.1.3/generate_json_schema.egg-info/top_level.txt
+-rw-r--r--   0 fernnando   (501) staff       (20)       38 2023-07-26 19:00:04.167612 generate-json-schema-0.1.3/setup.cfg
+-rw-r--r--   0 fernnando   (501) staff       (20)     1763 2023-07-26 18:58:32.000000 generate-json-schema-0.1.3/setup.py
+drwxr-xr-x   0 fernnando   (501) staff       (20)        0 2023-07-26 19:00:04.164424 generate-json-schema-0.1.3/src/
+-rw-r--r--   0 fernnando   (501) staff       (20)        0 2023-07-25 18:41:19.000000 generate-json-schema-0.1.3/src/__init__.py
+-rw-r--r--   0 fernnando   (501) staff       (20)     2056 2023-07-26 13:48:52.000000 generate-json-schema-0.1.3/src/generate_schema.py
```

### Comparing `generate-json-schema-0.0.2/PKG-INFO` & `generate-json-schema-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-json-schema
-Version: 0.0.2
+Version: 0.1.3
 Summary: Json Schema Generator
 Home-page: https://github.com/fernandotoledomoreira/json-schema-generator
 Author: Fernando Toledo Moreira
 Author-email: fernandotoledomoreira@gmail.com
 Keywords: json schema generator development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Installation
 ============
 
 To install the Json Schema Generator, use pip:
 
 .. code-block:: bash
 
-    pip install jsonschemagenerator
+    pip install generate-json-schema
 
 Usage
 =====
 
 To use the Json Schema Generator, import the module and utilize the function `generate_json_schema`:
 
 .. code-block:: python
```

### Comparing `generate-json-schema-0.0.2/README.rst` & `generate-json-schema-0.1.3/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Json Schema Generator
-====================
+=====================
 
 Installation
 ============
 
 To install the Json Schema Generator, use pip:
 
 .. code-block:: bash
 
-    pip install jsonschemagenerator
+    pip install generate-json-schema
 
 Usage
 =====
 
 To use the Json Schema Generator, import the module and utilize the function `generate_json_schema`:
 
 .. code-block:: python
```

### Comparing `generate-json-schema-0.0.2/generate_json_schema.egg-info/PKG-INFO` & `generate-json-schema-0.1.3/generate_json_schema.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generate-json-schema
-Version: 0.0.2
+Version: 0.1.3
 Summary: Json Schema Generator
 Home-page: https://github.com/fernandotoledomoreira/json-schema-generator
 Author: Fernando Toledo Moreira
 Author-email: fernandotoledomoreira@gmail.com
 Keywords: json schema generator development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Installation
 ============
 
 To install the Json Schema Generator, use pip:
 
 .. code-block:: bash
 
-    pip install jsonschemagenerator
+    pip install generate-json-schema
 
 Usage
 =====
 
 To use the Json Schema Generator, import the module and utilize the function `generate_json_schema`:
 
 .. code-block:: python
```

### Comparing `generate-json-schema-0.0.2/setup.py` & `generate-json-schema-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2023 Your Name <fernandotoledomoreira@gmail.com>
 
 import os
 from setuptools import setup
 
 # Library Information
 NAME = 'generate-json-schema'
-VERSION = '0.0.2'
+VERSION = '0.1.3'
 AUTHOR = 'Fernando Toledo Moreira'
 AUTHOR_EMAIL = 'fernandotoledomoreira@gmail.com'
 URL = 'https://github.com/fernandotoledomoreira/json-schema-generator'
 
 # Minimum Python version required for the library
 PYTHON_REQUIRES = '>=3.6'
```

### Comparing `generate-json-schema-0.0.2/src/generate_schema.py` & `generate-json-schema-0.1.3/src/generate_schema.py`

 * *Files identical despite different names*

