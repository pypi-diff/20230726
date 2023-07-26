# Comparing `tmp/dj_maintenance-0.2.5.tar.gz` & `tmp/dj_maintenance-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_maintenance-0.2.5.tar", last modified: Wed Jul 26 08:39:05 2023, max compression
+gzip compressed data, was "dj_maintenance-0.2.6.tar", last modified: Wed Jul 26 18:28:17 2023, max compression
```

## Comparing `dj_maintenance-0.2.5.tar` & `dj_maintenance-0.2.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.355624 dj_maintenance-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 08:39:05.355624 dj_maintenance-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.351624 dj_maintenance-0.2.5/dj_maintenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.351624 dj_maintenance-0.2.5/dj_maintenance/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.347624 dj_maintenance-0.2.5/dj_maintenance/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.347624 dj_maintenance-0.2.5/dj_maintenance/static/dj-maintenance/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.351624 dj_maintenance-0.2.5/dj_maintenance/static/dj-maintenance/images/
--rw-r--r--   0 runner    (1001) docker     (123)  3843590 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/static/dj-maintenance/images/maintenance.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.347624 dj_maintenance-0.2.5/dj_maintenance/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.355624 dj_maintenance-0.2.5/dj_maintenance/templates/dj_maintenance/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/templates/dj_maintenance/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.351624 dj_maintenance-0.2.5/dj_maintenance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 08:39:05.000000 dj_maintenance-0.2.5/dj_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-26 08:39:05.000000 dj_maintenance-0.2.5/dj_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:39:05.000000 dj_maintenance-0.2.5/dj_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 08:39:05.000000 dj_maintenance-0.2.5/dj_maintenance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 08:39:05.000000 dj_maintenance-0.2.5/dj_maintenance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-26 08:39:05.355624 dj_maintenance-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:17.980287 dj_maintenance-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-26 18:28:17.980287 dj_maintenance-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:17.976287 dj_maintenance-0.2.6/dj_maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/dj_maintenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/dj_maintenance/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/dj_maintenance/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:17.976287 dj_maintenance-0.2.6/dj_maintenance/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/dj_maintenance/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/dj_maintenance/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:17.972287 dj_maintenance-0.2.6/dj_maintenance/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:17.972287 dj_maintenance-0.2.6/dj_maintenance/static/dj-maintenance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:17.976287 dj_maintenance-0.2.6/dj_maintenance/static/dj-maintenance/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  3843590 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/dj_maintenance/static/dj-maintenance/images/maintenance.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:17.972287 dj_maintenance-0.2.6/dj_maintenance/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:17.980287 dj_maintenance-0.2.6/dj_maintenance/templates/dj_maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/dj_maintenance/templates/dj_maintenance/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/dj_maintenance/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/dj_maintenance/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/dj_maintenance/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:28:17.976287 dj_maintenance-0.2.6/dj_maintenance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-26 18:28:17.000000 dj_maintenance-0.2.6/dj_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-26 18:28:17.000000 dj_maintenance-0.2.6/dj_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:28:17.000000 dj_maintenance-0.2.6/dj_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 18:28:17.000000 dj_maintenance-0.2.6/dj_maintenance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 18:28:17.000000 dj_maintenance-0.2.6/dj_maintenance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-26 18:28:17.980287 dj_maintenance-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-26 18:28:04.000000 dj_maintenance-0.2.6/setup.py
```

### Comparing `dj_maintenance-0.2.5/LICENSE` & `dj_maintenance-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.5/PKG-INFO` & `dj_maintenance-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: dj_maintenance
-Version: 0.2.5
+Version: 0.2.6
 Summary: A django app to conduct sheduled maintenance.
 Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
 Author-email: admin@ayumefrancis.com
 License: BSD-3-Clause
+Project-URL: Homepage, https://djmaintenance.ayumefrancis.com
+Project-URL: Source Code, https://github.com/ayudmin/dj_maintenance
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `dj_maintenance-0.2.5/dj_maintenance/static/dj-maintenance/images/maintenance.gif` & `dj_maintenance-0.2.6/dj_maintenance/static/dj-maintenance/images/maintenance.gif`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.5/dj_maintenance/templates/dj_maintenance/index.html` & `dj_maintenance-0.2.6/dj_maintenance/templates/dj_maintenance/index.html`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.5/dj_maintenance.egg-info/PKG-INFO` & `dj_maintenance-0.2.6/dj_maintenance.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: dj-maintenance
-Version: 0.2.5
+Version: 0.2.6
 Summary: A django app to conduct sheduled maintenance.
 Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
 Author-email: admin@ayumefrancis.com
 License: BSD-3-Clause
+Project-URL: Homepage, https://djmaintenance.ayumefrancis.com
+Project-URL: Source Code, https://github.com/ayudmin/dj_maintenance
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `dj_maintenance-0.2.5/dj_maintenance.egg-info/SOURCES.txt` & `dj_maintenance-0.2.6/dj_maintenance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.5/setup.cfg` & `dj_maintenance-0.2.6/setup.cfg`

 * *Files identical despite different names*

