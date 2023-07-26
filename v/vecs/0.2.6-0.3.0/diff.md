# Comparing `tmp/vecs-0.2.6.tar.gz` & `tmp/vecs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecs-0.2.6.tar", last modified: Thu Jun  1 18:47:16 2023, max compression
+gzip compressed data, was "vecs-0.3.0.tar", last modified: Wed Jul 26 14:05:20 2023, max compression
```

## Comparing `vecs-0.2.6.tar` & `vecs-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-06-01 18:47:16.811108 vecs-0.2.6/
--rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-06-01 18:47:16.811000 vecs-0.2.6/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)     2349 2023-05-19 14:53:34.000000 vecs-0.2.6/README.md
--rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-05-12 13:47:40.000000 vecs-0.2.6/pyproject.toml
--rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-06-01 18:47:16.811154 vecs-0.2.6/setup.cfg
--rw-r--r--   0 oliverrice   (501) staff       (20)     2222 2023-05-19 14:54:31.000000 vecs-0.2.6/setup.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-06-01 18:47:16.809141 vecs-0.2.6/src/
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-06-01 18:47:16.810318 vecs-0.2.6/src/vecs/
--rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-06-01 18:46:56.000000 vecs-0.2.6/src/vecs/__init__.py
--rw-r--r--   0 oliverrice   (501) staff       (20)     1917 2023-06-01 18:46:56.000000 vecs-0.2.6/src/vecs/client.py
--rw-r--r--   0 oliverrice   (501) staff       (20)    13736 2023-05-24 17:16:29.000000 vecs-0.2.6/src/vecs/collection.py
--rw-r--r--   0 oliverrice   (501) staff       (20)      491 2023-05-16 18:21:37.000000 vecs-0.2.6/src/vecs/exc.py
-drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-06-01 18:47:16.810849 vecs-0.2.6/src/vecs.egg-info/
--rw-r--r--   0 oliverrice   (501) staff       (20)      743 2023-06-01 18:47:16.000000 vecs-0.2.6/src/vecs.egg-info/PKG-INFO
--rw-r--r--   0 oliverrice   (501) staff       (20)      271 2023-06-01 18:47:16.000000 vecs-0.2.6/src/vecs.egg-info/SOURCES.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-06-01 18:47:16.000000 vecs-0.2.6/src/vecs.egg-info/dependency_links.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)      157 2023-06-01 18:47:16.000000 vecs-0.2.6/src/vecs.egg-info/requires.txt
--rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-06-01 18:47:16.000000 vecs-0.2.6/src/vecs.egg-info/top_level.txt
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-07-26 14:05:20.631950 vecs-0.3.0/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      724 2023-07-26 14:05:20.631847 vecs-0.3.0/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2711 2023-06-27 19:32:26.000000 vecs-0.3.0/README.md
+-rw-r--r--   0 oliverrice   (501) staff       (20)      154 2023-06-27 19:32:26.000000 vecs-0.3.0/pyproject.toml
+-rw-r--r--   0 oliverrice   (501) staff       (20)       38 2023-07-26 14:05:20.631990 vecs-0.3.0/setup.cfg
+-rw-r--r--   0 oliverrice   (501) staff       (20)     2256 2023-07-26 13:51:42.000000 vecs-0.3.0/setup.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-07-26 14:05:20.629010 vecs-0.3.0/src/
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-07-26 14:05:20.630533 vecs-0.3.0/src/vecs/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      390 2023-07-26 14:05:10.000000 vecs-0.3.0/src/vecs/__init__.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-07-26 14:05:20.631657 vecs-0.3.0/src/vecs/adapter/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      302 2023-07-26 13:51:42.000000 vecs-0.3.0/src/vecs/adapter/__init__.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     3269 2023-07-26 13:51:42.000000 vecs-0.3.0/src/vecs/adapter/base.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1668 2023-07-26 13:51:42.000000 vecs-0.3.0/src/vecs/adapter/noop.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     5041 2023-07-26 13:51:42.000000 vecs-0.3.0/src/vecs/adapter/text.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     6622 2023-07-26 13:51:42.000000 vecs-0.3.0/src/vecs/client.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)    26661 2023-07-26 13:51:42.000000 vecs-0.3.0/src/vecs/collection.py
+-rw-r--r--   0 oliverrice   (501) staff       (20)     1687 2023-07-26 13:51:42.000000 vecs-0.3.0/src/vecs/exc.py
+drwxr-xr-x   0 oliverrice   (501) staff       (20)        0 2023-07-26 14:05:20.631135 vecs-0.3.0/src/vecs.egg-info/
+-rw-r--r--   0 oliverrice   (501) staff       (20)      724 2023-07-26 14:05:20.000000 vecs-0.3.0/src/vecs.egg-info/PKG-INFO
+-rw-r--r--   0 oliverrice   (501) staff       (20)      375 2023-07-26 14:05:20.000000 vecs-0.3.0/src/vecs.egg-info/SOURCES.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        1 2023-07-26 14:05:20.000000 vecs-0.3.0/src/vecs.egg-info/dependency_links.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)      220 2023-07-26 14:05:20.000000 vecs-0.3.0/src/vecs.egg-info/requires.txt
+-rw-r--r--   0 oliverrice   (501) staff       (20)        5 2023-07-26 14:05:20.000000 vecs-0.3.0/src/vecs.egg-info/top_level.txt
```

### Comparing `vecs-0.2.6/PKG-INFO` & `vecs-0.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.2.6
+Version: 0.3.0
 Summary: pgvector client
 Home-page: https://github.com/supabase/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: text_embedding
 
 UNKNOWN
```

### Comparing `vecs-0.2.6/README.md` & `vecs-0.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # vecs
 
 <p>
+    <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="Python version" height="18"></a>
+    <a href="https://github.com/supabase/vecs/actions">
+        <img src="https://github.com/supabase/vecs/workflows/tests/badge.svg" alt="test status" height="18">
+    </a>
+    <a href="https://github.com/supabase/vecs/actions">
+        <img src="https://github.com/supabase/vecs/workflows/pre-commit/badge.svg" alt="Pre-commit Status" height="18">
+    </a>
+</p>
 
 <p>
-    <a href="https://www.python.org/downloads/"><img src="https://img.shields.io/badge/python-3.7+-blue.svg" alt="Python version" height="18"></a>
     <a href="https://badge.fury.io/py/vecs"><img src="https://badge.fury.io/py/vecs.svg" alt="PyPI version" height="18"></a>
     <a href="https://github.com/supabase/vecs/blob/master/LICENSE"><img src="https://img.shields.io/pypi/l/markdown-subtemplate.svg" alt="License" height="18"></a>
     <a href="https://pypi.org/project/vecs/"><img src="https://img.shields.io/pypi/dm/vecs.svg" alt="Download count" height="18"></a>
 </p>
 
 ---
 
@@ -25,15 +32,15 @@
 
 Requires:
 
 - Python 3.7+
 
 You can install vecs using pip:
 
-```bash
+```sh
 pip install vecs
 ```
 
 ## Usage
 
 Visit the [quickstart guide](https://supabase.github.io/vecs/api/) for more complete info.
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
 # vecs
-[Python_version] [PyPI_version] [License] [Download_count]
+[Python_version] [test_status] [Pre-commit_Status]
+[PyPI_version] [License] [Download_count]
 --- **Documentation**: https://supabase.github.io/vecs/api/ **Source Code**:
 https://github.com/supabase/vecs --- `vecs` is a python client for managing and
 querying vector stores in PostgreSQL with the [pgvector extension](https://
 github.com/pgvector/pgvector). This guide will help you get started with using
 vecs. If you don't have a Postgres database with the pgvector ready, see
 [hosting](https://supabase.github.io/vecs/hosting/) for easy options. ##
-Installation Requires: - Python 3.7+ You can install vecs using pip: ```bash
-pip install vecs ``` ## Usage Visit the [quickstart guide](https://
+Installation Requires: - Python 3.7+ You can install vecs using pip: ```sh pip
+install vecs ``` ## Usage Visit the [quickstart guide](https://
 supabase.github.io/vecs/api/) for more complete info. ```python import vecs
 DB_CONNECTION = "postgresql://:@:/" # create vector store client vx =
 vecs.create_client(DB_CONNECTION) # create a collection of vectors with 3
 dimensions docs = vx.create_collection(name="docs", dimension=3) # add records
 to the *docs* collection docs.upsert( vectors=[ ( "vec0", # the vector's
 identifier [0.1, 0.2, 0.3], # the vector. list or np.array {"year": 1973} #
 associated metadata ), ( "vec1", [0.7, 0.8, 0.9], {"year": 2012} ) ] ) # index
```

### Comparing `vecs-0.2.6/setup.py` & `vecs-0.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import os
 import sys
 
 import setuptools
 
 PACKAGE_NAME = "vecs"
-MINIMUM_PYTHON_VERSION = (3, 7, 0, "", 0)
+MINIMUM_PYTHON_VERSION = (3, 8, 0, "", 0)
 
 
 def check_python_version():
     """Exit when the Python version is too low."""
     if sys.version_info < MINIMUM_PYTHON_VERSION:
         sys.exit(
             "At least Python {0}.{1}.{2} is required.".format(
@@ -38,14 +38,15 @@
 
 
 REQUIRES = [
     "pgvector==0.1.*",
     "sqlalchemy==2.*",
     "psycopg2-binary==2.9.*",
     "flupy==1.*",
+    "deprecated==1.2.*",
 ]
 
 
 setuptools.setup(
     name=read_package_variable("__project__"),
     version=read_package_variable("__version__"),
     description="pgvector client",
@@ -58,20 +59,20 @@
     license="MIT",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
     install_requires=REQUIRES,
     extras_require={
         "dev": ["pytest", "parse", "numpy", "pytest-cov"],
         "docs": ["mkdocs", "pygments", "pymdown-extensions", "pymarkdown"],
+        "text_embedding": ["sentence-transformers==2.*"],
     },
 )
```

### Comparing `vecs-0.2.6/src/vecs.egg-info/PKG-INFO` & `vecs-0.3.0/src/vecs.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: vecs
-Version: 0.2.6
+Version: 0.3.0
 Summary: pgvector client
 Home-page: https://github.com/supabase/vecs
 Author: Oliver Rice
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
 Provides-Extra: docs
+Provides-Extra: text_embedding
 
 UNKNOWN
```

