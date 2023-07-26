# Comparing `tmp/hyfi_template-0.6.3.tar.gz` & `tmp/hyfi_template-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.6.3.tar", max compression
+gzip compressed data, was "hyfi_template-0.6.4.tar", max compression
```

## Comparing `hyfi_template-0.6.3.tar` & `hyfi_template-0.6.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-07-25 00:24:02.543715 hyfi_template-0.6.3/LICENSE
--rw-r--r--   0        0        0     2215 2023-07-25 00:24:02.543715 hyfi_template-0.6.3/README.md
--rw-r--r--   0        0        0     2946 2023-07-25 00:24:28.507847 hyfi_template-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      180 2023-07-25 00:24:02.543715 hyfi_template-0.6.3/src/hyfit/__cli__.py
--rw-r--r--   0        0        0      473 2023-07-25 00:24:02.543715 hyfi_template-0.6.3/src/hyfit/__init__.py
--rw-r--r--   0        0        0       22 2023-07-25 00:24:28.467846 hyfi_template-0.6.3/src/hyfit/_version.py
--rw-r--r--   0        0        0        0 2023-07-25 00:24:02.543715 hyfi_template-0.6.3/src/hyfit/conf/__init__.py
--rw-r--r--   0        0        0      206 2023-07-25 00:24:02.543715 hyfi_template-0.6.3/src/hyfit/conf/about/hyfit.yaml
--rw-r--r--   0        0        0        0 2023-07-25 00:24:02.543715 hyfi_template-0.6.3/src/hyfit/py.typed
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 hyfi_template-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-26 19:08:19.088398 hyfi_template-0.6.4/LICENSE
+-rw-r--r--   0        0        0     2215 2023-07-26 19:08:19.088398 hyfi_template-0.6.4/README.md
+-rw-r--r--   0        0        0     2947 2023-07-26 19:08:49.113191 hyfi_template-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-07-26 19:08:19.092398 hyfi_template-0.6.4/src/hyfit/__cli__.py
+-rw-r--r--   0        0        0      473 2023-07-26 19:08:19.092398 hyfi_template-0.6.4/src/hyfit/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-26 19:08:49.065189 hyfi_template-0.6.4/src/hyfit/_version.py
+-rw-r--r--   0        0        0        0 2023-07-26 19:08:19.092398 hyfi_template-0.6.4/src/hyfit/conf/__init__.py
+-rw-r--r--   0        0        0      206 2023-07-26 19:08:19.092398 hyfi_template-0.6.4/src/hyfit/conf/about/hyfit.yaml
+-rw-r--r--   0        0        0        0 2023-07-26 19:08:19.092398 hyfi_template-0.6.4/src/hyfit/py.typed
+-rw-r--r--   0        0        0     2888 1970-01-01 00:00:00.000000 hyfi_template-0.6.4/PKG-INFO
```

### Comparing `hyfi_template-0.6.3/LICENSE` & `hyfi_template-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.6.3/README.md` & `hyfi_template-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.6.3/pyproject.toml` & `hyfi_template-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.6.3"
+version = "0.6.4"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-template"
 readme = "README.md"
 packages = [{ include = "hyfit", from = "src" }]
 
 [tool.poetry.scripts]
 hyfit = 'hyfit.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^1.9.3"
+hyfi = "^1.11.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `hyfi_template-0.6.3/PKG-INFO` & `hyfi_template-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.6.3
+Version: 0.6.4
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=1.9.3,<2.0.0)
+Requires-Dist: hyfi (>=1.11.0,<2.0.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi-template
 Description-Content-Type: text/markdown
 
 # HyFI Template
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

