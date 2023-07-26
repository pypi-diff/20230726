# Comparing `tmp/pydantic_apply-0.5.4.tar.gz` & `tmp/pydantic_apply-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_apply-0.5.4.tar", max compression
+gzip compressed data, was "pydantic_apply-0.5.5.tar", max compression
```

## Comparing `pydantic_apply-0.5.4.tar` & `pydantic_apply-0.5.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1078 2023-07-18 19:21:19.949882 pydantic_apply-0.5.4/LICENSE
--rw-r--r--   0        0        0     2258 2023-07-18 19:21:19.949882 pydantic_apply-0.5.4/README.md
--rw-r--r--   0        0        0       35 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pydantic_apply/__init__.py
--rw-r--r--   0        0        0     2453 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pydantic_apply/_compat.py
--rw-r--r--   0        0        0     5153 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pydantic_apply/apply.py
--rw-r--r--   0        0        0        0 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pydantic_apply/py.typed
--rw-r--r--   0        0        0      821 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pydantic_apply/utils.py
--rw-r--r--   0        0        0      849 2023-07-18 19:21:19.953882 pydantic_apply-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 pydantic_apply-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-26 06:28:04.118071 pydantic_apply-0.5.5/LICENSE
+-rw-r--r--   0        0        0     2258 2023-07-26 06:28:04.118071 pydantic_apply-0.5.5/README.md
+-rw-r--r--   0        0        0       35 2023-07-26 06:28:04.118071 pydantic_apply-0.5.5/pydantic_apply/__init__.py
+-rw-r--r--   0        0        0     2453 2023-07-26 06:28:04.118071 pydantic_apply-0.5.5/pydantic_apply/_compat.py
+-rw-r--r--   0        0        0     5153 2023-07-26 06:28:04.118071 pydantic_apply-0.5.5/pydantic_apply/apply.py
+-rw-r--r--   0        0        0        0 2023-07-26 06:28:04.118071 pydantic_apply-0.5.5/pydantic_apply/py.typed
+-rw-r--r--   0        0        0      821 2023-07-26 06:28:04.118071 pydantic_apply-0.5.5/pydantic_apply/utils.py
+-rw-r--r--   0        0        0      849 2023-07-26 06:28:04.118071 pydantic_apply-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 pydantic_apply-0.5.5/PKG-INFO
```

### Comparing `pydantic_apply-0.5.4/LICENSE` & `pydantic_apply-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.4/README.md` & `pydantic_apply-0.5.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pydantic-apply
 
 ## Installation
 
 Just use `pip install pydantic-apply` to install the library.
 
-**Note:** `pydantic-apply` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+**Note:** `pydantic-apply` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.x` (🥳) on
 Python `3.8`, `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
 using `tox`.
 
 ## About
 
 With `pydantic-apply` you can apply changes to your pydantic models by using
 the `ApplyModelMixin` it provides:
```

### Comparing `pydantic_apply-0.5.4/pydantic_apply/_compat.py` & `pydantic_apply-0.5.5/pydantic_apply/_compat.py`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.4/pydantic_apply/apply.py` & `pydantic_apply-0.5.5/pydantic_apply/apply.py`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.4/pydantic_apply/utils.py` & `pydantic_apply-0.5.5/pydantic_apply/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.5.4/pyproject.toml` & `pydantic_apply-0.5.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "pydantic-apply"
-version = "0.5.4"
+version = "0.5.5"
 description = "Apply changes as patches to pydanic models."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-apply"
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

### Comparing `pydantic_apply-0.5.4/PKG-INFO` & `pydantic_apply-0.5.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: pydantic-apply
-Version: 0.5.4
+Version: 0.5.5
 Summary: Apply changes as patches to pydanic models.
 Home-page: https://github.com/team23/pydantic-apply
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
 Project-URL: Repository, https://github.com/team23/pydantic-apply
 Description-Content-Type: text/markdown
 
 # pydantic-apply
 
 ## Installation
 
 Just use `pip install pydantic-apply` to install the library.
 
-**Note:** `pydantic-apply` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+**Note:** `pydantic-apply` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.x` (🥳) on
 Python `3.8`, `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
 using `tox`.
 
 ## About
 
 With `pydantic-apply` you can apply changes to your pydantic models by using
 the `ApplyModelMixin` it provides:
```

