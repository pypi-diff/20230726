# Comparing `tmp/pydantic_changedetect-0.5.0.tar.gz` & `tmp/pydantic_changedetect-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_changedetect-0.5.0.tar", max compression
+gzip compressed data, was "pydantic_changedetect-0.5.1.tar", max compression
```

## Comparing `pydantic_changedetect-0.5.0.tar` & `pydantic_changedetect-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-07-17 07:40:50.942068 pydantic_changedetect-0.5.0/LICENSE
--rw-r--r--   0        0        0     2827 2023-07-17 07:38:10.198156 pydantic_changedetect-0.5.0/README.md
--rw-r--r--   0        0        0       47 2022-08-31 20:08:26.918750 pydantic_changedetect-0.5.0/pydantic_changedetect/__init__.py
--rw-r--r--   0        0        0     1232 2023-07-16 18:05:16.681505 pydantic_changedetect-0.5.0/pydantic_changedetect/_compat.py
--rw-r--r--   0        0        0    21933 2023-07-17 07:36:59.214165 pydantic_changedetect-0.5.0/pydantic_changedetect/changedetect.py
--rw-r--r--   0        0        0        0 2022-09-23 05:50:27.111492 pydantic_changedetect-0.5.0/pydantic_changedetect/py.typed
--rw-r--r--   0        0        0     2621 2023-07-17 07:35:19.623327 pydantic_changedetect-0.5.0/pydantic_changedetect/utils.py
--rw-r--r--   0        0        0      906 2023-07-17 07:41:48.213670 pydantic_changedetect-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 pydantic_changedetect-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-26 06:28:17.798095 pydantic_changedetect-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2827 2023-07-26 06:28:17.798095 pydantic_changedetect-0.5.1/README.md
+-rw-r--r--   0        0        0       47 2023-07-26 06:28:17.798095 pydantic_changedetect-0.5.1/pydantic_changedetect/__init__.py
+-rw-r--r--   0        0        0     1232 2023-07-26 06:28:17.798095 pydantic_changedetect-0.5.1/pydantic_changedetect/_compat.py
+-rw-r--r--   0        0        0    21933 2023-07-26 06:28:17.798095 pydantic_changedetect-0.5.1/pydantic_changedetect/changedetect.py
+-rw-r--r--   0        0        0        0 2023-07-26 06:28:17.798095 pydantic_changedetect-0.5.1/pydantic_changedetect/py.typed
+-rw-r--r--   0        0        0     2621 2023-07-26 06:28:17.798095 pydantic_changedetect-0.5.1/pydantic_changedetect/utils.py
+-rw-r--r--   0        0        0      906 2023-07-26 06:28:17.802095 pydantic_changedetect-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3594 1970-01-01 00:00:00.000000 pydantic_changedetect-0.5.1/PKG-INFO
```

### Comparing `pydantic_changedetect-0.5.0/LICENSE` & `pydantic_changedetect-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.5.0/README.md` & `pydantic_changedetect-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Pydantic change detection
 
 ## Installation
 
 Just use `pip install pydantic-changedetect` to install the library.
 
-**Note:** `pydantic-changedetect` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+**Note:** `pydantic-changedetect` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.x` (🥳) on
 Python `3.8`, `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
 using `tox`.
 
 ## About
 
 When working with database models it is pretty common to want to detect changes
 to the model attributes. The `ChangeDetectionMixin` just provides this mechanism
```

### Comparing `pydantic_changedetect-0.5.0/pydantic_changedetect/_compat.py` & `pydantic_changedetect-0.5.1/pydantic_changedetect/_compat.py`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.5.0/pydantic_changedetect/changedetect.py` & `pydantic_changedetect-0.5.1/pydantic_changedetect/changedetect.py`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.5.0/pydantic_changedetect/utils.py` & `pydantic_changedetect-0.5.1/pydantic_changedetect/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_changedetect-0.5.0/pyproject.toml` & `pydantic_changedetect-0.5.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pydantic-changedetect"
-version = "0.5.0"
+version = "0.5.1"
 description = "Extend pydantic models to also detect and record changes made to the model attributes."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-changedetect"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pydantic = ">=1.9.0,<2.1.0"
+pydantic = ">=1.9.0,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.1.2,<8.0.0"
 isort = "^5.10.1"
 mypy = ">=0.971,<2.0"
 flake8 = ">=5.0.4,<7.0.0"
 flake8-builtins = ">=1.5.3,<3.0.0"
```

### Comparing `pydantic_changedetect-0.5.0/PKG-INFO` & `pydantic_changedetect-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pydantic-changedetect
-Version: 0.5.0
+Version: 0.5.1
 Summary: Extend pydantic models to also detect and record changes made to the model attributes.
 Home-page: https://github.com/team23/pydantic-changedetect
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.9.0,<2.1.0)
+Requires-Dist: pydantic (>=1.9.0,<3.0.0)
 Project-URL: Repository, https://github.com/team23/pydantic-changedetect
 Description-Content-Type: text/markdown
 
 # Pydantic change detection
 
 ## Installation
 
 Just use `pip install pydantic-changedetect` to install the library.
 
-**Note:** `pydantic-changedetect` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+**Note:** `pydantic-changedetect` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.x` (🥳) on
 Python `3.8`, `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
 using `tox`.
 
 ## About
 
 When working with database models it is pretty common to want to detect changes
 to the model attributes. The `ChangeDetectionMixin` just provides this mechanism
```

