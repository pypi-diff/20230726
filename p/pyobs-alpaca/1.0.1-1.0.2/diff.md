# Comparing `tmp/pyobs_alpaca-1.0.1.tar.gz` & `tmp/pyobs_alpaca-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobs_alpaca-1.0.1.tar", max compression
+gzip compressed data, was "pyobs_alpaca-1.0.2.tar", max compression
```

## Comparing `pyobs_alpaca-1.0.1.tar` & `pyobs_alpaca-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1099 2022-10-16 19:28:20.769863 pyobs_alpaca-1.0.1/LICENSE
--rw-r--r--   0        0        0      163 2022-10-16 19:28:20.773863 pyobs_alpaca-1.0.1/pyobs_alpaca/__init__.py
--rw-r--r--   0        0        0     6256 2022-10-16 19:28:20.773863 pyobs_alpaca-1.0.1/pyobs_alpaca/device.py
--rw-r--r--   0        0        0    10852 2022-10-16 19:28:20.773863 pyobs_alpaca-1.0.1/pyobs_alpaca/dome.py
--rw-r--r--   0        0        0     6569 2022-10-16 19:28:20.773863 pyobs_alpaca-1.0.1/pyobs_alpaca/focuser.py
--rw-r--r--   0        0        0    14593 2022-10-16 19:28:20.773863 pyobs_alpaca-1.0.1/pyobs_alpaca/telescope.py
--rw-r--r--   0        0        0      547 2022-10-16 19:28:20.773863 pyobs_alpaca-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      689 1970-01-01 00:00:00.000000 pyobs_alpaca-1.0.1/setup.py
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 pyobs_alpaca-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-07-26 19:21:52.993917 pyobs_alpaca-1.0.2/LICENSE
+-rw-r--r--   0        0        0      163 2023-07-26 19:21:52.993917 pyobs_alpaca-1.0.2/pyobs_alpaca/__init__.py
+-rw-r--r--   0        0        0     6256 2023-07-26 19:21:52.993917 pyobs_alpaca-1.0.2/pyobs_alpaca/device.py
+-rw-r--r--   0        0        0    10852 2023-07-26 19:21:52.993917 pyobs_alpaca-1.0.2/pyobs_alpaca/dome.py
+-rw-r--r--   0        0        0     6569 2023-07-26 19:21:52.993917 pyobs_alpaca-1.0.2/pyobs_alpaca/focuser.py
+-rw-r--r--   0        0        0    14593 2023-07-26 19:21:52.993917 pyobs_alpaca-1.0.2/pyobs_alpaca/telescope.py
+-rw-r--r--   0        0        0      547 2023-07-26 19:21:52.993917 pyobs_alpaca-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 pyobs_alpaca-1.0.2/PKG-INFO
```

### Comparing `pyobs_alpaca-1.0.1/LICENSE` & `pyobs_alpaca-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobs_alpaca-1.0.1/pyobs_alpaca/device.py` & `pyobs_alpaca-1.0.2/pyobs_alpaca/device.py`

 * *Files identical despite different names*

### Comparing `pyobs_alpaca-1.0.1/pyobs_alpaca/dome.py` & `pyobs_alpaca-1.0.2/pyobs_alpaca/dome.py`

 * *Files identical despite different names*

### Comparing `pyobs_alpaca-1.0.1/pyobs_alpaca/focuser.py` & `pyobs_alpaca-1.0.2/pyobs_alpaca/focuser.py`

 * *Files identical despite different names*

### Comparing `pyobs_alpaca-1.0.1/pyobs_alpaca/telescope.py` & `pyobs_alpaca-1.0.2/pyobs_alpaca/telescope.py`

 * *Files identical despite different names*

### Comparing `pyobs_alpaca-1.0.1/pyproject.toml` & `pyobs_alpaca-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "pyobs-alpaca"
-version = "1.0.1"
+version = "1.0.2"
 description = "pyobs module for ASCOM Alpaca"
 authors = ["Tim-Oliver Husser <thusser@uni-goettingen.de>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.11"
+python = ">=3.9,<3.12"
 numpy = "^1.22"
 single-source = "^0.2"
 pyobs-core="^1.0"
 
 [tool.poetry.dev-dependencies]
 black = "^21.12b0"
 pre-commit = "^2.16"
```

### Comparing `pyobs_alpaca-1.0.1/PKG-INFO` & `pyobs_alpaca-1.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyobs-alpaca
-Version: 1.0.1
+Version: 1.0.2
 Summary: pyobs module for ASCOM Alpaca
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: pyobs-core (>=1.0,<2.0)
 Requires-Dist: single-source (>=0.2,<0.3)
```

