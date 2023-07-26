# Comparing `tmp/seveno-pyutil-0.8.3.tar.gz` & `tmp/seveno-pyutil-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seveno-pyutil-0.8.3.tar", last modified: Mon Jun 26 06:11:35 2023, max compression
+gzip compressed data, was "seveno-pyutil-0.8.4.tar", last modified: Wed Jul 26 13:07:08 2023, max compression
```

## Comparing `seveno-pyutil-0.8.3.tar` & `seveno-pyutil-0.8.4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.325964 seveno-pyutil-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-26 06:11:35.325964 seveno-pyutil-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/_static/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/examples_and_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 06:11:35.325964 seveno-pyutil-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.317964 seveno-pyutil-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/src/seveno_pyutil/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/benchmarking_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/collections_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/datetime_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/error_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/file_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/pretty_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16041 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/sql_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/metaprogramming_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/os_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/src/seveno_pyutil/string_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.321964 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-26 06:11:35.000000 seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.325964 seveno-pyutil-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/benchmarking_utilities_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/collections_utilities_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/datetime_utilities_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/error_utilities_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/file_utilities_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 06:11:35.325964 seveno-pyutil-0.8.3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/metaprograming_helpers_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/string_utilities_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 06:11:23.000000 seveno-pyutil-0.8.3/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.357502 seveno-pyutil-0.8.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.361502 seveno-pyutil-0.8.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/_static/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.361502 seveno-pyutil-0.8.4/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/examples_and_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.357502 seveno-pyutil-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.361502 seveno-pyutil-0.8.4/src/seveno_pyutil/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/benchmarking_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/collections_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/datetime_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/error_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/file_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/pretty_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/sql_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/metaprogramming_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/os_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/src/seveno_pyutil/string_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.361502 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 13:07:08.000000 seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/benchmarking_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/collections_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/datetime_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/error_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/file_utilities_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:07:08.365502 seveno-pyutil-0.8.4/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/metaprograming_helpers_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/string_utilities_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-26 13:06:54.000000 seveno-pyutil-0.8.4/tests/test_helpers.py
```

### Comparing `seveno-pyutil-0.8.3/CHANGELOG.md` & `seveno-pyutil-0.8.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.8.4 (2023-07-26)
+
+- fix: don't rely on json to be able to encode SQL parameters
+
 ## 0.8.3 (2023-06-26)
 
 - build: added GitHub action for publishing releases to PyPi
 
 ## 0.8.2 (2023-06-07)
 
 - feat: prettier format for multiline SQL in SQLFilter
```

### Comparing `seveno-pyutil-0.8.3/LICENSE` & `seveno-pyutil-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/PKG-INFO` & `seveno-pyutil-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seveno-pyutil
-Version: 0.8.3
+Version: 0.8.4
 Summary: Various unsorted Python utilities
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/seveno_pyutil
 Project-URL: Documentation, https://seveno-pyutil.readthedocs.io/en/latest/
 Keywords: utilities
 Platform: any
```

### Comparing `seveno-pyutil-0.8.3/README.md` & `seveno-pyutil-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/docs/CHANGELOG.md` & `seveno-pyutil-0.8.4/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 0.8.4 (2023-07-26)
+
+- fix: don't rely on json to be able to encode SQL parameters
+
 ## 0.8.3 (2023-06-26)
 
 - build: added GitHub action for publishing releases to PyPi
 
 ## 0.8.2 (2023-06-07)
 
 - feat: prettier format for multiline SQL in SQLFilter
```

### Comparing `seveno-pyutil-0.8.3/docs/Makefile` & `seveno-pyutil-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/docs/api.rst` & `seveno-pyutil-0.8.4/docs/api.rst`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/docs/conf.py` & `seveno-pyutil-0.8.4/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from datetime import datetime
 
 author = "tadams42"
 project = "seveno-pyutil"
 copyright = (
     ", ".join(str(y) for y in range(2017, datetime.now().year + 1)) + ", " + author
 )
-release = "0.8.3"
+release = "0.8.4"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
```

### Comparing `seveno-pyutil-0.8.3/docs/examples_and_usage.rst` & `seveno-pyutil-0.8.4/docs/examples_and_usage.rst`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/docs/make.bat` & `seveno-pyutil-0.8.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/pyproject.toml` & `seveno-pyutil-0.8.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=65", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "seveno-pyutil"
-version = "0.8.3"
+version = "0.8.4"
 description = "Various unsorted Python utilities"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
 	"Development Status :: 4 - Beta",
 	"Intended Audience :: Developers",
 	"License :: OSI Approved :: MIT License",
@@ -39,31 +39,15 @@
 
 [project.urls]
 Source = "https://github.com/tadams42/seveno_pyutil"
 Documentation = "https://seveno-pyutil.readthedocs.io/en/latest/"
 
 
 [project.optional-dependencies]
-dev = [
-	"black",
-	"bump2version",
-	"check-manifest",
-	"coverage",
-	"factory-boy",
-	"faker",
-	"furo",
-	"ipython",
-	"isort",
-	"myst-parser",
-	"pytest-spec",
-	"pytest",
-	"sphinx-copybutton",
-	"sphinx",
-	"twine",
-]
+dev = ["black", "bump2version", "ipython", "isort", "rich", "pre-commit"]
 docs = ["furo", "myst-parser", "sphinx", "sphinx-copybutton"]
 tests = [
 	"check-manifest",
 	"pytest",
 	"coverage",
 	"factory-boy",
 	"faker",
```

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/__init__.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 
 import logging
 
 from .benchmarking_utilities import Stopwatch
 from .collections_utilities import in_batches
 from .datetime_utilities import ensure_tzinfo, iter_year_month
 from .error_utilities import ExceptionsAsErrors, add_error_to
```

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/benchmarking_utilities.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/benchmarking_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/collections_utilities.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/collections_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/datetime_utilities.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/datetime_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/error_utilities.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/error_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/file_utilities.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/file_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/pretty_formatter.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/pretty_formatter.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/sql_filter.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/sql_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from __future__ import annotations
 
 import enum
+import json
 import logging
 import timeit
 from dataclasses import dataclass, field
 from datetime import date, datetime, timedelta
+from decimal import Decimal
+from pathlib import Path
 from typing import TYPE_CHECKING, Callable, ClassVar, Final
+from uuid import UUID
 
 import pygments
 import sqlparse
 
 # from pygments.formatters import TerminalTrueColorFormatter
 from pygments.formatters import Terminal256Formatter
 from pygments.lexers import SqlLexer
 
-try:
-    import simplejson as json
-except Exception:
-    import json
-
 HAS_FLASK = False
 try:
     import flask
 
     HAS_FLASK = True
 except Exception:
     pass
@@ -399,15 +398,15 @@
         sql: str = statement or ""
 
         sql = self._maybe_multiline(sql)
         sql = self._maybe_colorized(sql)
 
         if parameters:
             params_dict = parameters
-            params = json.dumps(params_dict, cls=JsonEncoder).strip()
+            params = json.dumps(params_dict, cls=JSONEncoder).strip()
         else:
             params_dict = {}
             params = ""
 
         if self.colorize_queries and params:
             params = pygments.highlight(
                 params,
@@ -482,14 +481,19 @@
                 data[cls._KEY_SQL_CUMULATIVE_DURATION] += statement_duration
                 data[cls._KEY_SQL_COUNT] += 1
 
             except Exception:
                 lgr.error("Failed to collect SQL statistics!", exc_info=True)
 
 
-class JsonEncoder(json.JSONEncoder):
-    def default(self, o):
-        if isinstance(o, (date, datetime)):
-            return o.isoformat()
-        if isinstance(o, enum.Enum):
-            return o.name
-        return super().default(o)
+class JSONEncoder(json.JSONEncoder):
+    _DATES_TIMES = (date, datetime)
+
+    def default(self, obj):
+        if isinstance(obj, self._DATES_TIMES):
+            return obj.isoformat()
+        elif isinstance(obj, enum.Enum):
+            return obj.name
+        elif isinstance(obj, (UUID, Decimal, Path)):
+            return str(obj)
+        # return json.JSONEncoder.default(self, obj)
+        return str(obj)
```

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/standard_metadata_filter.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/logging_utilities/utilities.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/logging_utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/metaprogramming_helpers.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/metaprogramming_helpers.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil/os_utilities.py` & `seveno-pyutil-0.8.4/src/seveno_pyutil/os_utilities.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/PKG-INFO` & `seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seveno-pyutil
-Version: 0.8.3
+Version: 0.8.4
 Summary: Various unsorted Python utilities
 Author-email: Tomislav Adamic <tomislav.adamic@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/tadams42/seveno_pyutil
 Project-URL: Documentation, https://seveno-pyutil.readthedocs.io/en/latest/
 Keywords: utilities
 Platform: any
```

### Comparing `seveno-pyutil-0.8.3/src/seveno_pyutil.egg-info/SOURCES.txt` & `seveno-pyutil-0.8.4/src/seveno_pyutil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/tests/collections_utilities_spec.py` & `seveno-pyutil-0.8.4/tests/collections_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/tests/datetime_utilities_spec.py` & `seveno-pyutil-0.8.4/tests/datetime_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/tests/error_utilities_spec.py` & `seveno-pyutil-0.8.4/tests/error_utilities_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/tests/metaprograming_helpers_spec.py` & `seveno-pyutil-0.8.4/tests/metaprograming_helpers_spec.py`

 * *Files identical despite different names*

### Comparing `seveno-pyutil-0.8.3/tests/string_utilities_spec.py` & `seveno-pyutil-0.8.4/tests/string_utilities_spec.py`

 * *Files identical despite different names*

