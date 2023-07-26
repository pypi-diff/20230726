# Comparing `tmp/pydantic-loggings-1.3.0.tar.gz` & `tmp/pydantic-loggings-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-1.3.0.tar", last modified: Sat Jul 15 07:37:12 2023, max compression
+gzip compressed data, was "pydantic-loggings-1.6.0.tar", last modified: Wed Jul 26 18:22:25 2023, max compression
```

## Comparing `pydantic-loggings-1.3.0.tar` & `pydantic-loggings-1.6.0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/
--rw-r--r--   0 root         (0) root         (0)     3119 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2313 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)     2508 2023-07-15 07:37:02.000000 pydantic-loggings-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.626620 pydantic-loggings-1.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.626620 pydantic-loggings-1.3.0/src/pydantic_loggings/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/src/pydantic_loggings/base/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/loggings.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/loggings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/src/pydantic_loggings/rich/
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/rich/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/rich/handlers.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/rich/loggers.py
--rw-r--r--   0 root         (0) root         (0)      454 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/rich/loggings.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/types_.py
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3119 2023-07-15 07:37:12.000000 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-15 07:37:12.000000 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 07:37:12.000000 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-15 07:37:12.000000 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-15 07:37:12.000000 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.551401 pydantic-loggings-1.6.0/
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-07-26 18:22:25.551401 pydantic-loggings-1.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-07-26 18:22:16.000000 pydantic-loggings-1.6.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 18:22:25.551401 pydantic-loggings-1.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.543401 pydantic-loggings-1.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.543401 pydantic-loggings-1.6.0/src/pydantic_loggings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.547401 pydantic-loggings-1.6.0/src/pydantic_loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/loggings.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.547401 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/loggings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.551401 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/filters.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/loggings.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/types_.py
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.547401 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-07-26 18:22:25.000000 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-07-26 18:22:25.000000 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 18:22:25.000000 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-26 18:22:25.000000 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 18:22:25.000000 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/top_level.txt
```

### Comparing `pydantic-loggings-1.3.0/PKG-INFO` & `pydantic-loggings-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 1.3.0
+Version: 1.6.0
 Summary: Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-loggings
 Project-URL: Source, https://github.com/m9810223/pydantic-loggings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 2
 Classifier: Environment :: Console
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: rich
 
 # Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 
 [![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
 
 ## Installation
```

### Comparing `pydantic-loggings-1.3.0/README.md` & `pydantic-loggings-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.3.0/pyproject.toml` & `pydantic-loggings-1.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,90 @@
 [project.urls]
 Homepage = "https://github.com/m9810223/pydantic-loggings"
 Source = "https://github.com/m9810223/pydantic-loggings"
 
+
 [project]
 name = "pydantic-loggings"
 description = "Configure 🎁 Your 🤗 Python 🐍 Logging 📝"
-version = "1.3.0"
-authors = [
-  { name = "m9810223", email = "m9810223@gmail.com" },
-]
+version = "1.6.0"
+authors = [{ name = "m9810223", email = "m9810223@gmail.com" }]
 requires-python = ">=3.9"
 readme = "README.md"
-
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3 :: Only",
   "Typing :: Typed",
   "Framework :: Pydantic",
   "Framework :: Pydantic :: 2",
   "Environment :: Console",
 ]
+dependencies = ["pydantic>=2.0", "pydantic-settings>=2.0"]
 
-dependencies = [
-  "pydantic>=2.0",
-  "pydantic-settings>=2.0",
-]
-
-[tool.semantic_release] # https://python-semantic-release.readthedocs.io/en/latest/configuration.html
-build_command = "pip install pdm && pdm build"
-upload_to_repository = true
-upload_to_release = false
-version_toml = "pyproject.toml:project.version"
-changelog_file = "./misc/CHANGELOG.md"
-
-[tool.pdm.scripts]
-debug = { composite = ["dev"], env = { DEBUG = '1' } }
-dev = "python dev.py"
+[project.optional-dependencies]
+rich = ["rich>=13.4.2"]
 
 [tool.pdm.dev-dependencies]
 dev = [
   "pytest>=7.4.0",
   "pyright>=1.1.316",
   "pytest-cov>=4.1.0",
   "hypothesis>=6.80.0",
   "pytest-xdist>=3.3.1",
   "pytest-mock>=3.11.1",
-  "rich>=13.4.2",
 ]
 
+
+[tool.semantic_release] # https://python-semantic-release.readthedocs.io/en/latest/configuration.html
+build_command = "pip install pdm && pdm build"
+upload_to_vcs_release = false
+version_toml = ["pyproject.toml:project.version"]
+changelog_file = "./misc/CHANGELOG.md"
+
+
+[tool.pdm.scripts]
+debug = { composite = ["dev"], env = { DEBUG = '1' } }
+dev = "python dev.py"
+
+
 [tool.black] # https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html
 skip-string-normalization = 1
 
+
 [tool.ruff]
 extend-select = [
-  "W", # pycodestyle Warning
-  "I", # isort
-  "N", # pep8-naming
-  "S", # flake8-bandit
+  "W",   # pycodestyle Warning
+  "I",   # isort
+  "N",   # pep8-naming
+  "S",   # flake8-bandit
   "PTH", # flake8-use-pathlib
   "PGH", # pygrep-hooks
   "TRY", # tryceratops
 ]
 ignore = [
-  "E501", # line-too-long
-  "S101", # Use of `assert` detected
+  "E501",   # line-too-long
+  "S101",   # Use of `assert` detected
   "TRY003", # raise-vanilla-args  # "TRY400", # error-instead-of-exception
 ]
 
 [tool.ruff.isort] # https://beta.ruff.rs/docs/settings/#isort
 force-single-line = true
 lines-after-imports = 2
 
+
 [tool.mypy]
 ignore_missing_imports = true
 
+
 [tool.pytest.ini_options]
 addopts = "--exitfirst --failed-first -r fEsxXp --disable-warnings --showlocals --tb=short --cov=src --cov-report=term --cov-report=html:./htmlcov"
 # https://docs.pytest.org/en/stable/reference/reference.html
 # https://docs.pytest.org/en/stable/explanation/goodpractices.html
 # https://docs.pytest.org/en/stable/example/pythoncollection.html
 
+
 [tool.coverage.run] # https://coverage.readthedocs.io/en/stable/config.html
 omit = ["__init__.py"]
```

### Comparing `pydantic-loggings-1.3.0/src/pydantic_loggings/base/loggings.py` & `pydantic-loggings-1.6.0/src/pydantic_loggings/base/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.3.0/src/pydantic_loggings/mixins.py` & `pydantic-loggings-1.6.0/src/pydantic_loggings/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/formatters.py` & `pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/handlers.py` & `pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/loggers.py` & `pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/loggers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/loggings.py` & `pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.3.0/src/pydantic_loggings/rich/handlers.py` & `pydantic-loggings-1.6.0/src/pydantic_loggings/rich/handlers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import logging
 import typing as t
 
-import rich.logging
 from pydantic import Field
 
 from .. import not_set
 from .. import utils
-
-
-rich.logging.RichHandler
+from .formatters import Formatter
 
 
 class Handler(not_set.Handler):
     NAME: t.ClassVar[str] = 'rich'
     class_: str = Field(default='rich.logging.RichHandler', alias='()')
     level: t.Optional[str] = utils.get_level_name(logging.DEBUG)
+    formatter: t.Optional[str] = Formatter.NAME
     #
     omit_repeated_times: t.Optional[bool] = False
     log_time_format: t.Optional[str] = '%m-%d %H:%M:%S'
     show_path: t.Optional[bool] = False
     keywords: t.Optional[list[str]] = []
```

### Comparing `pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/PKG-INFO` & `pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 1.3.0
+Version: 1.6.0
 Summary: Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-loggings
 Project-URL: Source, https://github.com/m9810223/pydantic-loggings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
 Classifier: Framework :: Pydantic
 Classifier: Framework :: Pydantic :: 2
 Classifier: Environment :: Console
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: rich
 
 # Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 
 [![PyPI](https://img.shields.io/pypi/v/pydantic-loggings)](https://pypi.org/project/pydantic-loggings/)
 
 ## Installation
```

### Comparing `pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,10 +18,12 @@
 src/pydantic_loggings/not_set/__init__.py
 src/pydantic_loggings/not_set/filters.py
 src/pydantic_loggings/not_set/formatters.py
 src/pydantic_loggings/not_set/handlers.py
 src/pydantic_loggings/not_set/loggers.py
 src/pydantic_loggings/not_set/loggings.py
 src/pydantic_loggings/rich/__init__.py
+src/pydantic_loggings/rich/filters.py
+src/pydantic_loggings/rich/formatters.py
 src/pydantic_loggings/rich/handlers.py
 src/pydantic_loggings/rich/loggers.py
 src/pydantic_loggings/rich/loggings.py
```

