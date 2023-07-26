# Comparing `tmp/fyndata-django-accounts-0.6.1.tar.gz` & `tmp/fyndata-django-accounts-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyndata-django-accounts-0.6.1.tar", last modified: Tue Jun 13 13:44:14 2023, max compression
+gzip compressed data, was "fyndata-django-accounts-0.7.0.tar", last modified: Wed Jul 26 15:25:43 2023, max compression
```

## Comparing `fyndata-django-accounts-0.6.1.tar` & `fyndata-django-accounts-0.7.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.470327 fyndata-django-accounts-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-13 13:44:14.470327 fyndata-django-accounts-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.466328 fyndata-django-accounts-0.6.1/fd_dj_accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/auth_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/base_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.466328 fyndata-django-accounts-0.6.1/fd_dj_accounts/management/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.466328 fyndata-django-accounts-0.6.1/fd_dj_accounts/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/management/commands/createsuperuser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.466328 fyndata-django-accounts-0.6.1/fd_dj_accounts/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/fd_dj_accounts/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.470327 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-06-13 13:44:14.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 13:44:14.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:44:14.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:44:13.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 13:44:14.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 13:44:14.000000 fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-13 13:44:14.474328 fyndata-django-accounts-0.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:44:14.470327 fyndata-django-accounts-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_auth_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 13:43:45.000000 fyndata-django-accounts-0.6.1/tests/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:25:43.351387 fyndata-django-accounts-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-07-26 15:25:43.351387 fyndata-django-accounts-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:25:43.347386 fyndata-django-accounts-0.7.0/fd_dj_accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/auth_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/base_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:25:43.347386 fyndata-django-accounts-0.7.0/fd_dj_accounts/management/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:25:43.347386 fyndata-django-accounts-0.7.0/fd_dj_accounts/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7970 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/management/commands/createsuperuser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:25:43.347386 fyndata-django-accounts-0.7.0/fd_dj_accounts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/fd_dj_accounts/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:25:43.351387 fyndata-django-accounts-0.7.0/fyndata_django_accounts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10106 2023-07-26 15:25:43.000000 fyndata-django-accounts-0.7.0/fyndata_django_accounts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-26 15:25:43.000000 fyndata-django-accounts-0.7.0/fyndata_django_accounts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:25:43.000000 fyndata-django-accounts-0.7.0/fyndata_django_accounts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:25:42.000000 fyndata-django-accounts-0.7.0/fyndata_django_accounts.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 15:25:43.000000 fyndata-django-accounts-0.7.0/fyndata_django_accounts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 15:25:43.000000 fyndata-django-accounts-0.7.0/fyndata_django_accounts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-26 15:25:43.351387 fyndata-django-accounts-0.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3059 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:25:43.351387 fyndata-django-accounts-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/tests/test_auth_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/tests/test_factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-26 15:25:21.000000 fyndata-django-accounts-0.7.0/tests/test_signals.py
```

### Comparing `fyndata-django-accounts-0.6.1/CONTRIBUTING.rst` & `fyndata-django-accounts-0.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/HISTORY.rst` & `fyndata-django-accounts-0.7.0/HISTORY.rst`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,29 @@
 
 History
 -------
 
 unreleased (YYYY-MM-DD)
 +++++++++++++++++++++++
 
+0.7.0 (2023-06-09)
+++++++++++++++++++
+
+- (PR #242, 2023-07-10) Add improved `__repr__()` to `User` model
+- (PR #243, 2023-07-10) Fix broken Make task `docker-compose-run-test`
+- (PR #241, 2023-07-10) chore: Bump codecov/codecov-action from 3.1.2 to 3.1.4
+- (PR #244, 2023-07-14) chore: Bump actions/setup-python from 4.5.0 to 4.7.0
+- (PR #231, 2023-07-14) chore(deps): Bump flake8 from 3.8.4 to 6.0.0
+- (PR #240, 2023-07-14) chore: Bump actions/checkout from 3.3.0 to 3.5.3
+- (PR #237, 2023-07-14) chore: Bump actions/dependency-review-action from 3.0.4 to 3.0.6
+- (PR #235, 2023-07-14) chore(deps): Bump coverage from 7.2.1 to 7.2.7
+- (PR #247, 2023-07-25) chore(deps): Bump mypy from 1.1.1 to 1.4.1
+- (PR #246, 2023-07-25) chore(deps): Bump setuptools from 67.6.0 to 68.0.0
+- (PR #245, 2023-07-25) chore(deps): Bump twine from 4.0.1 to 4.0.2
+
 0.6.1 (2023-06-09)
 ++++++++++++++++++
 
 - (PR #228, 2023-04-04) Add Git commit linter
 - (PR #225, 2023-04-05) Bump wheel from 0.38.4 to 0.40.0
 - (PR #227, 2023-05-23) chore(deps): Bump actions/dependency-review-action from 3.0.3 to 3.0.4
 - (PR #234, 2023-06-05) Add Codecov to CI workflow
```

### Comparing `fyndata-django-accounts-0.6.1/LICENSE` & `fyndata-django-accounts-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/PKG-INFO` & `fyndata-django-accounts-0.7.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyndata-django-accounts
-Version: 0.6.1
+Version: 0.7.0
 Summary: Reusable Django app to replace the default Django user (account) model.
 Home-page: https://github.com/fyndata/fyndata-django-accounts
 Author: Fyndata (Fynpal SpA)
 Author-email: no-reply@fyndata.com
 License: MIT
 Keywords: fyndata-django-accounts
 Classifier: Development Status :: 3 - Alpha
@@ -143,14 +143,29 @@
 
 History
 -------
 
 unreleased (YYYY-MM-DD)
 +++++++++++++++++++++++
 
+0.7.0 (2023-06-09)
+++++++++++++++++++
+
+- (PR #242, 2023-07-10) Add improved `__repr__()` to `User` model
+- (PR #243, 2023-07-10) Fix broken Make task `docker-compose-run-test`
+- (PR #241, 2023-07-10) chore: Bump codecov/codecov-action from 3.1.2 to 3.1.4
+- (PR #244, 2023-07-14) chore: Bump actions/setup-python from 4.5.0 to 4.7.0
+- (PR #231, 2023-07-14) chore(deps): Bump flake8 from 3.8.4 to 6.0.0
+- (PR #240, 2023-07-14) chore: Bump actions/checkout from 3.3.0 to 3.5.3
+- (PR #237, 2023-07-14) chore: Bump actions/dependency-review-action from 3.0.4 to 3.0.6
+- (PR #235, 2023-07-14) chore(deps): Bump coverage from 7.2.1 to 7.2.7
+- (PR #247, 2023-07-25) chore(deps): Bump mypy from 1.1.1 to 1.4.1
+- (PR #246, 2023-07-25) chore(deps): Bump setuptools from 67.6.0 to 68.0.0
+- (PR #245, 2023-07-25) chore(deps): Bump twine from 4.0.1 to 4.0.2
+
 0.6.1 (2023-06-09)
 ++++++++++++++++++
 
 - (PR #228, 2023-04-04) Add Git commit linter
 - (PR #225, 2023-04-05) Bump wheel from 0.38.4 to 0.40.0
 - (PR #227, 2023-05-23) chore(deps): Bump actions/dependency-review-action from 3.0.3 to 3.0.4
 - (PR #234, 2023-06-05) Add Codecov to CI workflow
```

### Comparing `fyndata-django-accounts-0.6.1/README.rst` & `fyndata-django-accounts-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/fd_dj_accounts/__init__.py` & `fyndata-django-accounts-0.7.0/fd_dj_accounts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,11 +94,11 @@
     https://docs.djangoproject.com/en/2.1/topics/auth/customizing/#specifying-a-custom-user-model
     https://docs.djangoproject.com/en/2.1/ref/contrib/auth/#django.contrib.auth.models.User
 
 
 """
 
 
-__version__ = '0.6.1'
+__version__ = '0.7.0'
 
 
 default_app_config = 'fd_dj_accounts.apps.AccountsAppConfig'
```

### Comparing `fyndata-django-accounts-0.6.1/fd_dj_accounts/apps.py` & `fyndata-django-accounts-0.7.0/fd_dj_accounts/apps.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/fd_dj_accounts/auth_backends.py` & `fyndata-django-accounts-0.7.0/fd_dj_accounts/auth_backends.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/fd_dj_accounts/base_models.py` & `fyndata-django-accounts-0.7.0/fd_dj_accounts/base_models.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/fd_dj_accounts/management/__init__.py` & `fyndata-django-accounts-0.7.0/fd_dj_accounts/management/__init__.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/fd_dj_accounts/management/commands/createsuperuser.py` & `fyndata-django-accounts-0.7.0/fd_dj_accounts/management/commands/createsuperuser.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/fd_dj_accounts/migrations/0001_initial.py` & `fyndata-django-accounts-0.7.0/fd_dj_accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/fd_dj_accounts/models.py` & `fyndata-django-accounts-0.7.0/fd_dj_accounts/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -114,14 +114,15 @@
 
     Extra customizations (besides those in the parent class):
     - New field ``created_by``.
     - Change field `id`: UUID instead of int.
     - Override :meth:`save` to make sure full validation is performed before
       each and every save (including creation).
     - Custom model manager.
+    - Custom :meth:`__repr__` that includes the user’s ``id`` in addition to the username.
 
     .. seealso:: :class:`AnonymousUser`.
 
     """
 
     # Explicit override of auto-generated integer model field 'id' (primary key).
     id = models.UUIDField(
@@ -142,14 +143,24 @@
 
     class Meta:
         abstract = False
 
         verbose_name = 'user'
         verbose_name_plural = 'users'
 
+    def __repr__(self) -> str:
+        # fmt: off
+        return (
+            f"<{self.__class__.__name__}("
+            f"id={self.id!r},"
+            f" {self.USERNAME_FIELD}={self.get_username()!r}"
+            f")>"
+        )
+        # fmt: on
+
     def save(self, *args: Any, **kwargs: Any) -> None:
         """Call :meth:`full_clean` before saving."""
         self.full_clean()
         super().save(*args, **kwargs)
 
 
 class AnonymousUser(base_models.AnonymousUser):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fyndata-django-accounts-0.6.1/fd_dj_accounts/urls.py` & `fyndata-django-accounts-0.7.0/fd_dj_accounts/urls.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/PKG-INFO` & `fyndata-django-accounts-0.7.0/fyndata_django_accounts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyndata-django-accounts
-Version: 0.6.1
+Version: 0.7.0
 Summary: Reusable Django app to replace the default Django user (account) model.
 Home-page: https://github.com/fyndata/fyndata-django-accounts
 Author: Fyndata (Fynpal SpA)
 Author-email: no-reply@fyndata.com
 License: MIT
 Keywords: fyndata-django-accounts
 Classifier: Development Status :: 3 - Alpha
@@ -143,14 +143,29 @@
 
 History
 -------
 
 unreleased (YYYY-MM-DD)
 +++++++++++++++++++++++
 
+0.7.0 (2023-06-09)
+++++++++++++++++++
+
+- (PR #242, 2023-07-10) Add improved `__repr__()` to `User` model
+- (PR #243, 2023-07-10) Fix broken Make task `docker-compose-run-test`
+- (PR #241, 2023-07-10) chore: Bump codecov/codecov-action from 3.1.2 to 3.1.4
+- (PR #244, 2023-07-14) chore: Bump actions/setup-python from 4.5.0 to 4.7.0
+- (PR #231, 2023-07-14) chore(deps): Bump flake8 from 3.8.4 to 6.0.0
+- (PR #240, 2023-07-14) chore: Bump actions/checkout from 3.3.0 to 3.5.3
+- (PR #237, 2023-07-14) chore: Bump actions/dependency-review-action from 3.0.4 to 3.0.6
+- (PR #235, 2023-07-14) chore(deps): Bump coverage from 7.2.1 to 7.2.7
+- (PR #247, 2023-07-25) chore(deps): Bump mypy from 1.1.1 to 1.4.1
+- (PR #246, 2023-07-25) chore(deps): Bump setuptools from 67.6.0 to 68.0.0
+- (PR #245, 2023-07-25) chore(deps): Bump twine from 4.0.1 to 4.0.2
+
 0.6.1 (2023-06-09)
 ++++++++++++++++++
 
 - (PR #228, 2023-04-04) Add Git commit linter
 - (PR #225, 2023-04-05) Bump wheel from 0.38.4 to 0.40.0
 - (PR #227, 2023-05-23) chore(deps): Bump actions/dependency-review-action from 3.0.3 to 3.0.4
 - (PR #234, 2023-06-05) Add Codecov to CI workflow
```

### Comparing `fyndata-django-accounts-0.6.1/fyndata_django_accounts.egg-info/SOURCES.txt` & `fyndata-django-accounts-0.7.0/fyndata_django_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/setup.cfg` & `fyndata-django-accounts-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/setup.py` & `fyndata-django-accounts-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/tests/test_apps.py` & `fyndata-django-accounts-0.7.0/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/tests/test_auth_backends.py` & `fyndata-django-accounts-0.7.0/tests/test_auth_backends.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/tests/test_factories.py` & `fyndata-django-accounts-0.7.0/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/tests/test_management.py` & `fyndata-django-accounts-0.7.0/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `fyndata-django-accounts-0.6.1/tests/test_models.py` & `fyndata-django-accounts-0.7.0/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from uuid import UUID
+
 from django.test import SimpleTestCase, TestCase
 
 from fd_dj_accounts.models import AnonymousUser, User, UserManager, get_or_create_system_user
 
 
 class FunctionsTestCase(TestCase):
 
@@ -79,14 +81,27 @@
                 email_address='test@test.com',
                 password='test', is_staff=False,
             )
 
 
 class UserTestCase(TestCase):
 
+    def test_repr(self) -> None:
+        user = User(
+            id=UUID('12caf218-0001-45d4-b4df-44ff87f19989'),
+            email_address='user@example.com',
+        )
+        self.assertEqual(
+            repr(user),
+            "<User("
+            "id=UUID('12caf218-0001-45d4-b4df-44ff87f19989'),"
+            " email_address='user@example.com'"
+            ")>"
+        )
+
     def test_model_manager(self):  # type: ignore
         self.assertIsInstance(User.objects, UserManager)
 
     def test_clean_normalize_email_address_as_username(self):  # type: ignore
         # Unicode characters that look the same but are different ones.
         email_address_original_ohm = 'iamtheΩ@example.com'  # U+2126 OHM SIGN
         email_address_normalized_omega = 'iamtheΩ@example.com'  # U+03A9 GREEK CAPITAL LETTER OMEGA
```

### Comparing `fyndata-django-accounts-0.6.1/tests/test_signals.py` & `fyndata-django-accounts-0.7.0/tests/test_signals.py`

 * *Files identical despite different names*

