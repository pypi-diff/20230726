# Comparing `tmp/aes_pkcs5-1.0.1.tar.gz` & `tmp/aes_pkcs5-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aes_pkcs5-1.0.1.tar", last modified: Sun Jan 22 03:12:12 2023, max compression
+gzip compressed data, was "aes_pkcs5-1.0.2.tar", last modified: Wed Jul 26 17:53:34 2023, max compression
```

## Comparing `aes_pkcs5-1.0.1.tar` & `aes_pkcs5-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 03:12:12.024738 aes_pkcs5-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-01-22 03:11:56.000000 aes_pkcs5-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-01-22 03:12:12.024738 aes_pkcs5-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-22 03:11:56.000000 aes_pkcs5-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 03:12:12.024738 aes_pkcs5-1.0.1/aes_pkcs5/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-22 03:11:56.000000 aes_pkcs5-1.0.1/aes_pkcs5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 03:12:12.024738 aes_pkcs5-1.0.1/aes_pkcs5/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-01-22 03:11:56.000000 aes_pkcs5-1.0.1/aes_pkcs5/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-01-22 03:11:56.000000 aes_pkcs5-1.0.1/aes_pkcs5/algorithms/aes_cbc_pkcs5_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-01-22 03:11:56.000000 aes_pkcs5-1.0.1/aes_pkcs5/algorithms/aes_ecb_pkcs5_padding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-22 03:12:12.024738 aes_pkcs5-1.0.1/aes_pkcs5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-01-22 03:12:12.000000 aes_pkcs5-1.0.1/aes_pkcs5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-01-22 03:12:12.000000 aes_pkcs5-1.0.1/aes_pkcs5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-22 03:12:12.000000 aes_pkcs5-1.0.1/aes_pkcs5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-22 03:12:12.000000 aes_pkcs5-1.0.1/aes_pkcs5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-22 03:12:12.000000 aes_pkcs5-1.0.1/aes_pkcs5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-22 03:12:12.024738 aes_pkcs5-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-01-22 03:11:56.000000 aes_pkcs5-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:53:34.639340 aes_pkcs5-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-26 17:53:16.000000 aes_pkcs5-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-26 17:53:34.639340 aes_pkcs5-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-26 17:53:16.000000 aes_pkcs5-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:53:34.639340 aes_pkcs5-1.0.2/aes_pkcs5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:53:16.000000 aes_pkcs5-1.0.2/aes_pkcs5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:53:34.639340 aes_pkcs5-1.0.2/aes_pkcs5/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-26 17:53:16.000000 aes_pkcs5-1.0.2/aes_pkcs5/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-26 17:53:16.000000 aes_pkcs5-1.0.2/aes_pkcs5/algorithms/aes_cbc_pkcs5_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-26 17:53:16.000000 aes_pkcs5-1.0.2/aes_pkcs5/algorithms/aes_ecb_pkcs5_padding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:53:34.639340 aes_pkcs5-1.0.2/aes_pkcs5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-26 17:53:34.000000 aes_pkcs5-1.0.2/aes_pkcs5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-26 17:53:34.000000 aes_pkcs5-1.0.2/aes_pkcs5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:53:34.000000 aes_pkcs5-1.0.2/aes_pkcs5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 17:53:34.000000 aes_pkcs5-1.0.2/aes_pkcs5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 17:53:34.000000 aes_pkcs5-1.0.2/aes_pkcs5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-26 17:53:34.639340 aes_pkcs5-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-26 17:53:16.000000 aes_pkcs5-1.0.2/setup.py
```

### Comparing `aes_pkcs5-1.0.1/LICENSE` & `aes_pkcs5-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aes_pkcs5-1.0.1/PKG-INFO` & `aes_pkcs5-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: aes_pkcs5
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implementation of AES with CBC/ECB mode and padding scheme PKCS5
 Home-page: https://github.com/Laerte/aes_pkcs5
 Author: Laerte Pereira
 Author-email: hi@laerte.dev
-License: BSD
+License: BSD License
 Project-URL: Documentation, https://aes-pkcs5.readthedocs.io
 Project-URL: Source, https://github.com/Laerte/aes_pkcs5
 Project-URL: Tracker, https://github.com/Laerte/aes_pkcs5/issues
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
 AESPKCS5
 ========
 
@@ -47,15 +46,15 @@
     
 
 Python implementation of AES with CBC/ECB mode and padding scheme PKCS5.
 
 ============
 Requirements
 ============
-* Python 3.7+
+* Python 3.8+
 
 Install
 =======
 You can install AESPKCS5 from PyPI with::
 
     pip install aes-pkcs5
```

### Comparing `aes_pkcs5-1.0.1/README.rst` & `aes_pkcs5-1.0.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     
 
 Python implementation of AES with CBC/ECB mode and padding scheme PKCS5.
 
 ============
 Requirements
 ============
-* Python 3.7+
+* Python 3.8+
 
 Install
 =======
 You can install AESPKCS5 from PyPI with::
 
     pip install aes-pkcs5
```

### Comparing `aes_pkcs5-1.0.1/aes_pkcs5/algorithms/__init__.py` & `aes_pkcs5-1.0.2/aes_pkcs5/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `aes_pkcs5-1.0.1/aes_pkcs5/algorithms/aes_cbc_pkcs5_padding.py` & `aes_pkcs5-1.0.2/aes_pkcs5/algorithms/aes_cbc_pkcs5_padding.py`

 * *Files identical despite different names*

### Comparing `aes_pkcs5-1.0.1/aes_pkcs5/algorithms/aes_ecb_pkcs5_padding.py` & `aes_pkcs5-1.0.2/aes_pkcs5/algorithms/aes_ecb_pkcs5_padding.py`

 * *Files identical despite different names*

### Comparing `aes_pkcs5-1.0.1/aes_pkcs5.egg-info/PKG-INFO` & `aes_pkcs5-1.0.2/aes_pkcs5.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 Metadata-Version: 2.1
 Name: aes-pkcs5
-Version: 1.0.1
+Version: 1.0.2
 Summary: Implementation of AES with CBC/ECB mode and padding scheme PKCS5
 Home-page: https://github.com/Laerte/aes_pkcs5
 Author: Laerte Pereira
 Author-email: hi@laerte.dev
-License: BSD
+License: BSD License
 Project-URL: Documentation, https://aes-pkcs5.readthedocs.io
 Project-URL: Source, https://github.com/Laerte/aes_pkcs5
 Project-URL: Tracker, https://github.com/Laerte/aes_pkcs5/issues
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
 AESPKCS5
 ========
 
@@ -47,15 +46,15 @@
     
 
 Python implementation of AES with CBC/ECB mode and padding scheme PKCS5.
 
 ============
 Requirements
 ============
-* Python 3.7+
+* Python 3.8+
 
 Install
 =======
 You can install AESPKCS5 from PyPI with::
 
     pip install aes-pkcs5
```

