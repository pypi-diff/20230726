# Comparing `tmp/edx-completion-4.2.1.tar.gz` & `tmp/edx-completion-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-completion-4.2.1.tar", last modified: Wed Apr 26 14:44:47 2023, max compression
+gzip compressed data, was "edx-completion-4.3.0.tar", last modified: Wed Jul 26 13:38:09 2023, max compression
```

## Comparing `edx-completion-4.2.1.tar` & `edx-completion-4.3.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.952363 edx-completion-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (122)     8091 2023-04-26 14:44:41.000000 edx-completion-4.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-04-26 14:44:41.000000 edx-completion-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      230 2023-04-26 14:44:41.000000 edx-completion-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    13239 2023-04-26 14:44:47.952363 edx-completion-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4426 2023-04-26 14:44:41.000000 edx-completion-4.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.944363 edx-completion-4.2.1/completion/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.944363 edx-completion-4.2.1/completion/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.944363 edx-completion-4.2.1/completion/api/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.948363 edx-completion-4.2.1/completion/api/v1/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.948363 edx-completion-4.2.1/completion/api/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/v1/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     9219 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/api/v1/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)      438 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.948363 edx-completion-4.2.1/completion/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      312 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/migrations/0002_auto_20180125_1510.py
--rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/migrations/0003_learning_context.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12622 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     8289 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/services.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.948363 edx-completion-4.2.1/completion/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/settings/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.948363 edx-completion-4.2.1/completion/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)     9545 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      927 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      924 2023-04-26 14:44:41.000000 edx-completion-4.2.1/completion/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.952363 edx-completion-4.2.1/edx_completion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13239 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       65 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      127 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-26 14:44:47.000000 edx-completion-4.2.1/edx_completion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 14:44:47.952363 edx-completion-4.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-04-26 14:44:41.000000 edx-completion-4.2.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-04-26 14:44:41.000000 edx-completion-4.2.1/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      526 2023-04-26 14:44:41.000000 edx-completion-4.2.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-04-26 14:44:47.952363 edx-completion-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5373 2023-04-26 14:44:41.000000 edx-completion-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.703159 edx-completion-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     8192 2023-07-26 13:38:01.000000 edx-completion-4.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    34520 2023-07-26 13:38:01.000000 edx-completion-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      230 2023-07-26 13:38:01.000000 edx-completion-4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    13340 2023-07-26 13:38:09.703159 edx-completion-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4426 2023-07-26 13:38:01.000000 edx-completion-4.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.695159 edx-completion-4.3.0/completion/
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.695159 edx-completion-4.3.0/completion/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1635 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/api/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.699159 edx-completion-4.3.0/completion/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/api/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/api/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.699159 edx-completion-4.3.0/completion/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/api/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.699159 edx-completion-4.3.0/completion/api/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/api/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/api/v1/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9219 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/api/v1/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1156 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)      438 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.699159 edx-completion-4.3.0/completion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/migrations/0002_auto_20180125_1510.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1309 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/migrations/0003_learning_context.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12622 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8289 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/services.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.699159 edx-completion-4.3.0/completion/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/settings/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3775 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.699159 edx-completion-4.3.0/completion/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9545 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1511 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      927 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-07-26 13:38:01.000000 edx-completion-4.3.0/completion/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.703159 edx-completion-4.3.0/edx_completion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13340 2023-07-26 13:38:09.000000 edx-completion-4.3.0/edx_completion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1275 2023-07-26 13:38:09.000000 edx-completion-4.3.0/edx_completion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 13:38:09.000000 edx-completion-4.3.0/edx_completion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-07-26 13:38:09.000000 edx-completion-4.3.0/edx_completion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 13:38:09.000000 edx-completion-4.3.0/edx_completion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-26 13:38:09.000000 edx-completion-4.3.0/edx_completion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-26 13:38:09.000000 edx-completion-4.3.0/edx_completion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 13:38:09.703159 edx-completion-4.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-07-26 13:38:01.000000 edx-completion-4.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-26 13:38:01.000000 edx-completion-4.3.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-07-26 13:38:01.000000 edx-completion-4.3.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-26 13:38:09.703159 edx-completion-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5373 2023-07-26 13:38:01.000000 edx-completion-4.3.0/setup.py
```

### Comparing `edx-completion-4.2.1/CHANGELOG.rst` & `edx-completion-4.3.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,18 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[4.3.0]- 2023-07-26
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Added support for Django 4.2
+
 [4.2.1]- 2023-04-26
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Support ``get_child_blocks`` along with ``get_child_descriptors``.
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [4.1.0]- 2021-07-19
```

### Comparing `edx-completion-4.2.1/LICENSE` & `edx-completion-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/PKG-INFO` & `edx-completion-4.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-completion
-Version: 4.2.1
+Version: 4.3.0
 Summary: A library for tracking completion of blocks by learners in edX courses.
 Home-page: https://github.com/openedx/completion
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
@@ -140,14 +140,18 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[4.3.0]- 2023-07-26
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Added support for Django 4.2
+
 [4.2.1]- 2023-04-26
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Support ``get_child_blocks`` along with ``get_child_descriptors``.
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [4.1.0]- 2021-07-19
```

### Comparing `edx-completion-4.2.1/README.rst` & `edx-completion-4.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/api/permissions.py` & `edx-completion-4.3.0/completion/api/permissions.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/api/tests/test_permissions.py` & `edx-completion-4.3.0/completion/api/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/api/v1/urls.py` & `edx-completion-4.3.0/completion/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/api/v1/views.py` & `edx-completion-4.3.0/completion/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/apps.py` & `edx-completion-4.3.0/completion/apps.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/handlers.py` & `edx-completion-4.3.0/completion/handlers.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/migrations/0001_initial.py` & `edx-completion-4.3.0/completion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/migrations/0003_learning_context.py` & `edx-completion-4.3.0/completion/migrations/0003_learning_context.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/models.py` & `edx-completion-4.3.0/completion/models.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/services.py` & `edx-completion-4.3.0/completion/services.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/settings/common.py` & `edx-completion-4.3.0/completion/settings/common.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/test_utils.py` & `edx-completion-4.3.0/completion/test_utils.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/tests/test_models.py` & `edx-completion-4.3.0/completion/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/tests/test_services.py` & `edx-completion-4.3.0/completion/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/tests/test_utilities.py` & `edx-completion-4.3.0/completion/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/utilities.py` & `edx-completion-4.3.0/completion/utilities.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/completion/waffle.py` & `edx-completion-4.3.0/completion/waffle.py`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/edx_completion.egg-info/PKG-INFO` & `edx-completion-4.3.0/edx_completion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-completion
-Version: 4.2.1
+Version: 4.3.0
 Summary: A library for tracking completion of blocks by learners in edX courses.
 Home-page: https://github.com/openedx/completion
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL 3.0
 Keywords: Django edx
 Classifier: Development Status :: 3 - Alpha
@@ -140,14 +140,18 @@
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
 
+[4.3.0]- 2023-07-26
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Added support for Django 4.2
+
 [4.2.1]- 2023-04-26
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Support ``get_child_blocks`` along with ``get_child_descriptors``.
 * Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
   deprecated
 
 [4.1.0]- 2021-07-19
```

### Comparing `edx-completion-4.2.1/edx_completion.egg-info/SOURCES.txt` & `edx-completion-4.3.0/edx_completion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/requirements/constraints.txt` & `edx-completion-4.3.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/requirements/test.in` & `edx-completion-4.3.0/requirements/test.in`

 * *Files identical despite different names*

### Comparing `edx-completion-4.2.1/setup.py` & `edx-completion-4.3.0/setup.py`

 * *Files identical despite different names*

