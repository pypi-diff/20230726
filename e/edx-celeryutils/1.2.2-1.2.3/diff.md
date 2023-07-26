# Comparing `tmp/edx-celeryutils-1.2.2.tar.gz` & `tmp/edx-celeryutils-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-celeryutils-1.2.2.tar", last modified: Thu Jan 19 09:58:48 2023, max compression
+gzip compressed data, was "edx-celeryutils-1.2.3.tar", last modified: Wed Jul 26 12:21:19 2023, max compression
```

## Comparing `edx-celeryutils-1.2.2.tar` & `edx-celeryutils-1.2.3.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:48.284820 edx-celeryutils-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     3105 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      248 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     6554 2023-01-19 09:58:48.284820 edx-celeryutils-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:48.284820 edx-celeryutils-1.2.2/celery_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)      231 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/logged_task.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:48.284820 edx-celeryutils-1.2.2/celery_utils/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:48.284820 edx-celeryutils-1.2.2/celery_utils/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/management/commands/cleanup_resolved_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1377 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/management/commands/reapply_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:48.284820 edx-celeryutils-1.2.2/celery_utils/management/commands/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/management/commands/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/management/commands/tests/test_cleanup_resolved_tasks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/management/commands/tests/test_reapply_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:48.284820 edx-celeryutils-1.2.2/celery_utils/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      339 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/migrations/0002_chordable_django_backend.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1946 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/persist_on_failure.py
--rw-r--r--   0 runner    (1001) docker     (122)      535 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/celery_utils/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:48.284820 edx-celeryutils-1.2.2/edx_celeryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6554 2023-01-19 09:58:48.000000 edx-celeryutils-1.2.2/edx_celeryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-01-19 09:58:48.000000 edx-celeryutils-1.2.2/edx_celeryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-19 09:58:48.000000 edx-celeryutils-1.2.2/edx_celeryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-19 09:58:48.000000 edx-celeryutils-1.2.2/edx_celeryutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-01-19 09:58:48.000000 edx-celeryutils-1.2.2/edx_celeryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-01-19 09:58:48.000000 edx-celeryutils-1.2.2/edx_celeryutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-19 09:58:48.284820 edx-celeryutils-1.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-01-19 09:58:48.284820 edx-celeryutils-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     5114 2023-01-19 09:58:43.000000 edx-celeryutils-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     3301 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10702 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      248 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     6676 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2609 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/celery_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1586 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/logged_task.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/celery_utils/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/celery_utils/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1988 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/management/commands/cleanup_resolved_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1377 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/management/commands/reapply_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/celery_utils/management/commands/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/management/commands/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/management/commands/tests/test_cleanup_resolved_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3406 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/management/commands/tests/test_reapply_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/celery_utils/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1382 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/migrations/0002_chordable_django_backend.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1946 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1965 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/persist_on_failure.py
+-rw-r--r--   0 runner    (1001) docker     (122)      535 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/celery_utils/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/edx_celeryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6676 2023-07-26 12:21:19.000000 edx-celeryutils-1.2.3/edx_celeryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1097 2023-07-26 12:21:19.000000 edx-celeryutils-1.2.3/edx_celeryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 12:21:19.000000 edx-celeryutils-1.2.3/edx_celeryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 12:21:19.000000 edx-celeryutils-1.2.3/edx_celeryutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-26 12:21:19.000000 edx-celeryutils-1.2.3/edx_celeryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-07-26 12:21:19.000000 edx-celeryutils-1.2.3/edx_celeryutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     5190 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 12:21:19.343104 edx-celeryutils-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/tests/test_logged_task.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2683 2023-07-26 12:21:14.000000 edx-celeryutils-1.2.3/tests/test_persist_on_failure.py
```

### Comparing `edx-celeryutils-1.2.2/CHANGELOG.rst` & `edx-celeryutils-1.2.3/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,22 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
-*
+
+
+
+[1.2.3] - 2023-06-15
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Support added for Django 4.2.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
 
 [1.2.2] - 2022-01-24
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Removed future package dependency.
 
 [1.2.1] - 2022-01-24
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `edx-celeryutils-1.2.2/LICENSE.txt` & `edx-celeryutils-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/PKG-INFO` & `edx-celeryutils-1.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: edx-celeryutils
-Version: 1.2.2
+Version: 1.2.3
 Summary: Code to support working with celery
 Home-page: https://github.com/openedx/edx-celeryutils
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
 License-File: AUTHORS
@@ -83,18 +84,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -117,15 +115,22 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
-*
+
+
+
+[1.2.3] - 2023-06-15
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Support added for Django 4.2.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
 
 [1.2.2] - 2022-01-24
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Removed future package dependency.
 
 [1.2.1] - 2022-01-24
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -215,9 +220,7 @@
 
 Initial release
 
 Contains two task base classes:
 
 * LoggedTask - Reports extra logging info 1) when a task is submitted to the task service (for tracking task latency) and 2) when the task retries, it surfaces information about the raised exception.
 * PersistOnFailureTask - Stores a record of failed tasks that can later be retried.
-
-
```

### Comparing `edx-celeryutils-1.2.2/README.rst` & `edx-celeryutils-1.2.3/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -61,18 +61,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
```

### Comparing `edx-celeryutils-1.2.2/celery_utils/logged_task.py` & `edx-celeryutils-1.2.3/celery_utils/logged_task.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/celery_utils/management/commands/cleanup_resolved_tasks.py` & `edx-celeryutils-1.2.3/celery_utils/management/commands/cleanup_resolved_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/celery_utils/management/commands/reapply_tasks.py` & `edx-celeryutils-1.2.3/celery_utils/management/commands/reapply_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/celery_utils/management/commands/tests/test_cleanup_resolved_tasks.py` & `edx-celeryutils-1.2.3/celery_utils/management/commands/tests/test_cleanup_resolved_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/celery_utils/management/commands/tests/test_reapply_tasks.py` & `edx-celeryutils-1.2.3/celery_utils/management/commands/tests/test_reapply_tasks.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/celery_utils/migrations/0001_initial.py` & `edx-celeryutils-1.2.3/celery_utils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/celery_utils/models.py` & `edx-celeryutils-1.2.3/celery_utils/models.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/celery_utils/persist_on_failure.py` & `edx-celeryutils-1.2.3/celery_utils/persist_on_failure.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/celery_utils/tasks.py` & `edx-celeryutils-1.2.3/celery_utils/tasks.py`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/edx_celeryutils.egg-info/PKG-INFO` & `edx-celeryutils-1.2.3/edx_celeryutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: edx-celeryutils
-Version: 1.2.2
+Version: 1.2.3
 Summary: Code to support working with celery
 Home-page: https://github.com/openedx/edx-celeryutils
 Author: edX
 Author-email: oscm@edx.org
 License: Apache 2.0
 Keywords: Django edx
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 License-File: LICENSE.txt
 License-File: AUTHORS
@@ -83,18 +84,15 @@
 Please see ``LICENSE.txt`` for details.
 
 How To Contribute
 -----------------
 
 Contributions are very welcome.
 
-Please read `How To Contribute <https://github.com/openedx/edx-platform/blob/master/CONTRIBUTING.rst>`_ for details.
-
-Even though they were written with ``edx-platform`` in mind, the guidelines
-should be followed for Open edX code in general.
+Please read `How To Contribute <https://github.com/openedx/.github/blob/master/CONTRIBUTING.md>`_ for details.
 
 Reporting Security Issues
 -------------------------
 
 Please do not report security issues in public. Please email security@edx.org.
 
 Getting Help
@@ -117,15 +115,22 @@
 
    This project adheres to Semantic Versioning (http://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 ~~~~~~~~~~
-*
+
+
+
+[1.2.3] - 2023-06-15
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+* Support added for Django 4.2.
+* Switch from ``edx-sphinx-theme`` to ``sphinx-book-theme`` since the former is
+  deprecated
 
 [1.2.2] - 2022-01-24
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 * Removed future package dependency.
 
 [1.2.1] - 2022-01-24
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
@@ -215,9 +220,7 @@
 
 Initial release
 
 Contains two task base classes:
 
 * LoggedTask - Reports extra logging info 1) when a task is submitted to the task service (for tracking task latency) and 2) when the task retries, it surfaces information about the raised exception.
 * PersistOnFailureTask - Stores a record of failed tasks that can later be retried.
-
-
```

### Comparing `edx-celeryutils-1.2.2/edx_celeryutils.egg-info/SOURCES.txt` & `edx-celeryutils-1.2.3/edx_celeryutils.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,8 +25,10 @@
 edx_celeryutils.egg-info/PKG-INFO
 edx_celeryutils.egg-info/SOURCES.txt
 edx_celeryutils.egg-info/dependency_links.txt
 edx_celeryutils.egg-info/not-zip-safe
 edx_celeryutils.egg-info/requires.txt
 edx_celeryutils.egg-info/top_level.txt
 requirements/base.in
-requirements/constraints.txt
+requirements/constraints.txt
+tests/test_logged_task.py
+tests/test_persist_on_failure.py
```

### Comparing `edx-celeryutils-1.2.2/requirements/constraints.txt` & `edx-celeryutils-1.2.3/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `edx-celeryutils-1.2.2/setup.py` & `edx-celeryutils-1.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,16 @@
     zip_safe=False,
     keywords='Django edx',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Framework :: Django',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
 )
```

