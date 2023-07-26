# Comparing `tmp/configula-0.5.2.tar.gz` & `tmp/configula-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configula-0.5.2.tar", max compression
+gzip compressed data, was "configula-0.5.3.tar", max compression
```

## Comparing `configula-0.5.2.tar` & `configula-0.5.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    10231 2022-12-11 05:47:17.378858 configula-0.5.2/LICENSE
--rw-r--r--   0        0        0     1920 2022-12-11 05:47:17.378858 configula-0.5.2/README.md
--rw-r--r--   0        0        0      276 2022-12-11 05:47:17.378858 configula-0.5.2/changelog.md
--rw-r--r--   0        0        0       33 2022-12-11 05:47:17.378858 configula-0.5.2/configula/__init__.py
--rw-r--r--   0        0        0     7734 2022-12-11 05:47:17.378858 configula-0.5.2/configula/configula.py
--rw-r--r--   0        0        0     1273 2022-12-11 05:47:17.378858 configula-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2698 1970-01-01 00:00:00.000000 configula-0.5.2/setup.py
--rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 configula-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    10231 2023-07-26 13:00:54.273795 configula-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1920 2023-07-26 13:00:54.273795 configula-0.5.3/README.md
+-rw-r--r--   0        0        0      276 2023-07-26 13:00:54.273795 configula-0.5.3/changelog.md
+-rw-r--r--   0        0        0       33 2023-07-26 13:00:54.273795 configula-0.5.3/configula/__init__.py
+-rw-r--r--   0        0        0     7734 2023-07-26 13:00:54.273795 configula-0.5.3/configula/configula.py
+-rw-r--r--   0        0        0     1273 2023-07-26 13:00:54.273795 configula-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 configula-0.5.3/PKG-INFO
```

### Comparing `configula-0.5.2/LICENSE` & `configula-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `configula-0.5.2/README.md` & `configula-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `configula-0.5.2/configula/configula.py` & `configula-0.5.3/configula/configula.py`

 * *Files identical despite different names*

### Comparing `configula-0.5.2/pyproject.toml` & `configula-0.5.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configula"
-version = "0.5.2"
+version = "0.5.3"
 description = "Merges configuration from toml file and environment variables"
 authors = ["Eugen Ciur <eugen@papermerge.com>"]
 maintainers = ["Eugen Ciur <eugen@papermerge.com>"]
 license = "Apache-2.0"
 include = ["LICENSE", "changelog.md", "README.md"]
 readme = "README.md"
 classifiers = [
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.10"
 ]
 homepage = "https://github.com/papermerge/configula"
 repository = "https://github.com/papermerge/configula"
 keywords = ["configurations", "config", "environment variables", "toml"]
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.11"
+python = ">=3.8, <3.12"
 tomlkit = "^0.7.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 pycodestyle = "^2.8.0"
 taskipy = "^1.10.2"
```

### Comparing `configula-0.5.2/PKG-INFO` & `configula-0.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: configula
-Version: 0.5.2
+Version: 0.5.3
 Summary: Merges configuration from toml file and environment variables
 Home-page: https://github.com/papermerge/configula
 License: Apache-2.0
 Keywords: configurations,config,environment variables,toml
 Author: Eugen Ciur
 Author-email: eugen@papermerge.com
 Maintainer: Eugen Ciur
 Maintainer-email: eugen@papermerge.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: tomlkit (>=0.7.2,<0.8.0)
 Project-URL: Repository, https://github.com/papermerge/configula
 Description-Content-Type: text/markdown
 
 # Configula
 
 Creates a single configuration by merging settings defined in:
```

