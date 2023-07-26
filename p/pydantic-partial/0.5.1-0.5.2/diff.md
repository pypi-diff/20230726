# Comparing `tmp/pydantic_partial-0.5.1.tar.gz` & `tmp/pydantic_partial-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_partial-0.5.1.tar", max compression
+gzip compressed data, was "pydantic_partial-0.5.2.tar", max compression
```

## Comparing `pydantic_partial-0.5.1.tar` & `pydantic_partial-0.5.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1077 2023-07-18 19:59:57.097087 pydantic_partial-0.5.1/LICENSE
--rw-r--r--   0        0        0     5597 2023-07-18 19:59:57.097087 pydantic_partial-0.5.1/README.md
--rw-r--r--   0        0        0       61 2023-07-18 19:59:57.101087 pydantic_partial-0.5.1/pydantic_partial/__init__.py
--rw-r--r--   0        0        0     2435 2023-07-18 19:59:57.101087 pydantic_partial-0.5.1/pydantic_partial/_compat.py
--rw-r--r--   0        0        0     5660 2023-07-18 19:59:57.101087 pydantic_partial-0.5.1/pydantic_partial/partial.py
--rw-r--r--   0        0        0        0 2023-07-18 19:59:57.101087 pydantic_partial-0.5.1/pydantic_partial/py.typed
--rw-r--r--   0        0        0     1034 2023-07-18 19:59:57.101087 pydantic_partial-0.5.1/pydantic_partial/utils.py
--rw-r--r--   0        0        0      915 2023-07-18 19:59:57.101087 pydantic_partial-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 pydantic_partial-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-26 06:28:45.900466 pydantic_partial-0.5.2/LICENSE
+-rw-r--r--   0        0        0     5597 2023-07-26 06:28:45.900466 pydantic_partial-0.5.2/README.md
+-rw-r--r--   0        0        0       61 2023-07-26 06:28:45.900466 pydantic_partial-0.5.2/pydantic_partial/__init__.py
+-rw-r--r--   0        0        0     2435 2023-07-26 06:28:45.900466 pydantic_partial-0.5.2/pydantic_partial/_compat.py
+-rw-r--r--   0        0        0     5660 2023-07-26 06:28:45.900466 pydantic_partial-0.5.2/pydantic_partial/partial.py
+-rw-r--r--   0        0        0        0 2023-07-26 06:28:45.900466 pydantic_partial-0.5.2/pydantic_partial/py.typed
+-rw-r--r--   0        0        0     1034 2023-07-26 06:28:45.900466 pydantic_partial-0.5.2/pydantic_partial/utils.py
+-rw-r--r--   0        0        0      915 2023-07-26 06:28:45.900466 pydantic_partial-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6318 1970-01-01 00:00:00.000000 pydantic_partial-0.5.2/PKG-INFO
```

### Comparing `pydantic_partial-0.5.1/LICENSE` & `pydantic_partial-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_partial-0.5.1/README.md` & `pydantic_partial-0.5.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pydantic-partial
 
 ## Installation
 
 Just use `pip install pydantic-partial` to install the library.
 
-**Note:** `pydantic-partial` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+**Note:** `pydantic-partial` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.x` (🥳) on
 Python `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
 using `tox`.
 
 ## About
 
 Create partial models from your normal pydantic models. Partial models will allow
 some or all fields to be optional and thus not be required when creating the model
```

### Comparing `pydantic_partial-0.5.1/pydantic_partial/_compat.py` & `pydantic_partial-0.5.2/pydantic_partial/_compat.py`

 * *Files identical despite different names*

### Comparing `pydantic_partial-0.5.1/pydantic_partial/partial.py` & `pydantic_partial-0.5.2/pydantic_partial/partial.py`

 * *Files identical despite different names*

### Comparing `pydantic_partial-0.5.1/pydantic_partial/utils.py` & `pydantic_partial-0.5.2/pydantic_partial/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_partial-0.5.1/pyproject.toml` & `pydantic_partial-0.5.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pydantic-partial"
-version = "0.5.1"
+version = "0.5.2"
 description = "Create partial models from your pydantic models. Partial models may allow None for certain or all fields."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-partial"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = ">=1.9.0,<2.1.0"
+pydantic = ">=1.9.0,<3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.1.2,<8.0.0"
 isort = "^5.10.1"
 mypy = ">=0.971,<2.0"
 flake8 = ">=5.0.4,<7.0.0"
 flake8-builtins = ">=1.5.3,<3.0.0"
```

### Comparing `pydantic_partial-0.5.1/PKG-INFO` & `pydantic_partial-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: pydantic-partial
-Version: 0.5.1
+Version: 0.5.2
 Summary: Create partial models from your pydantic models. Partial models may allow None for certain or all fields.
 Home-page: https://github.com/team23/pydantic-partial
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.9.0,<2.1.0)
+Requires-Dist: pydantic (>=1.9.0,<3.0.0)
 Project-URL: Repository, https://github.com/team23/pydantic-partial
 Description-Content-Type: text/markdown
 
 # pydantic-partial
 
 ## Installation
 
 Just use `pip install pydantic-partial` to install the library.
 
-**Note:** `pydantic-partial` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+**Note:** `pydantic-partial` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.x` (🥳) on
 Python `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
 using `tox`.
 
 ## About
 
 Create partial models from your normal pydantic models. Partial models will allow
 some or all fields to be optional and thus not be required when creating the model
```

