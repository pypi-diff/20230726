# Comparing `tmp/dj_maintenance-0.2.4.tar.gz` & `tmp/dj_maintenance-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_maintenance-0.2.4.tar", last modified: Tue Jul 25 11:41:12 2023, max compression
+gzip compressed data, was "dj_maintenance-0.2.5.tar", last modified: Wed Jul 26 08:39:05 2023, max compression
```

## Comparing `dj_maintenance-0.2.4.tar` & `dj_maintenance-0.2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:41:12.742154 dj_maintenance-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-25 11:41:12.742154 dj_maintenance-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:41:12.734154 dj_maintenance-0.2.4/dj_maintenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/dj_maintenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/dj_maintenance/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/dj_maintenance/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:41:12.738154 dj_maintenance-0.2.4/dj_maintenance/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/dj_maintenance/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/dj_maintenance/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:41:12.730154 dj_maintenance-0.2.4/dj_maintenance/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:41:12.730154 dj_maintenance-0.2.4/dj_maintenance/static/dj-maintenance/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:41:12.738154 dj_maintenance-0.2.4/dj_maintenance/static/dj-maintenance/images/
--rw-r--r--   0 runner    (1001) docker     (123)  3843590 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/dj_maintenance/static/dj-maintenance/images/maintenance.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:41:12.730154 dj_maintenance-0.2.4/dj_maintenance/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:41:12.742154 dj_maintenance-0.2.4/dj_maintenance/templates/dj_maintenance/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/dj_maintenance/templates/dj_maintenance/index.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/dj_maintenance/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/dj_maintenance/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/dj_maintenance/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:41:12.738154 dj_maintenance-0.2.4/dj_maintenance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-25 11:41:12.000000 dj_maintenance-0.2.4/dj_maintenance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-25 11:41:12.000000 dj_maintenance-0.2.4/dj_maintenance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:41:12.000000 dj_maintenance-0.2.4/dj_maintenance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 11:41:12.000000 dj_maintenance-0.2.4/dj_maintenance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 11:41:12.000000 dj_maintenance-0.2.4/dj_maintenance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-25 11:41:12.742154 dj_maintenance-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-25 11:40:59.000000 dj_maintenance-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.355624 dj_maintenance-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 08:39:05.355624 dj_maintenance-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.351624 dj_maintenance-0.2.5/dj_maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.351624 dj_maintenance-0.2.5/dj_maintenance/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.347624 dj_maintenance-0.2.5/dj_maintenance/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.347624 dj_maintenance-0.2.5/dj_maintenance/static/dj-maintenance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.351624 dj_maintenance-0.2.5/dj_maintenance/static/dj-maintenance/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  3843590 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/static/dj-maintenance/images/maintenance.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.347624 dj_maintenance-0.2.5/dj_maintenance/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.355624 dj_maintenance-0.2.5/dj_maintenance/templates/dj_maintenance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/templates/dj_maintenance/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/dj_maintenance/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:05.351624 dj_maintenance-0.2.5/dj_maintenance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-26 08:39:05.000000 dj_maintenance-0.2.5/dj_maintenance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-26 08:39:05.000000 dj_maintenance-0.2.5/dj_maintenance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:39:05.000000 dj_maintenance-0.2.5/dj_maintenance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 08:39:05.000000 dj_maintenance-0.2.5/dj_maintenance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 08:39:05.000000 dj_maintenance-0.2.5/dj_maintenance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-26 08:39:05.355624 dj_maintenance-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-26 08:38:50.000000 dj_maintenance-0.2.5/setup.py
```

### Comparing `dj_maintenance-0.2.4/LICENSE` & `dj_maintenance-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.4/PKG-INFO` & `dj_maintenance-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_maintenance
-Version: 0.2.4
+Version: 0.2.5
 Summary: A django app to conduct sheduled maintenance.
 Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
 Author-email: admin@ayumefrancis.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj_maintenance-0.2.4/README.rst` & `dj_maintenance-0.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.4/dj_maintenance/static/dj-maintenance/images/maintenance.gif` & `dj_maintenance-0.2.5/dj_maintenance/static/dj-maintenance/images/maintenance.gif`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.4/dj_maintenance/templates/dj_maintenance/index.html` & `dj_maintenance-0.2.5/dj_maintenance/templates/dj_maintenance/index.html`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <html lang="en">
 <head>
     {% load static %}
     <meta charset="UTF-8">
     <meta name="viewport"
           content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
     <meta http-equiv="X-UA-Compatible" content="ie=edge">
-    <title>sspaynow</title>
+    <title>{% if domain %}{{ domain }}{% else %} 503{% endif %} | Unavailable</title>
 </head>
 <style>
     html, body {
         height: 100%;
         font-family: monospace;
         background: #80808003;
     }
@@ -33,19 +33,24 @@
     h3 {
         margin-bottom: 8em;
     }
     p {
         font-size: 12px;
         font-weight: 600;
     }
+
+
+
 </style>
 <body>
-    <section class="alert">
-        <h1><underline>website Under maintenance</underline></h1>
-        <p>Our website is currently undergoing <span style="color: green;">sheduled maintenance</span></p>
-        <p>We should be back shortly. Thank you for your patience</p>
-        <img src="{% static 'dj-maintenance/images/maintenance.gif' %}" width="500"  alt="">
-        <h3>Application Id: DA-11542</h3>
-    </section>
+<section class="alert">
+    <h1>
+        <underline>website Under maintenance</underline>
+    </h1>
+    <p>Our website is currently undergoing <span style="color: green;">sheduled maintenance</span></p>
+    <p>We should be back shortly. Thank you for your patience</p>
+    <img src="{% static 'dj-maintenance/images/maintenance.gif' %}" width="500" alt="">
+    <h3>Application Id: DA-11542</h3>
+</section>
 
 </body>
 </html>
```

### Comparing `dj_maintenance-0.2.4/dj_maintenance.egg-info/PKG-INFO` & `dj_maintenance-0.2.5/dj_maintenance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-maintenance
-Version: 0.2.4
+Version: 0.2.5
 Summary: A django app to conduct sheduled maintenance.
 Home-page: https://djmaintenance.ayumefrancis.com/
 Author: Ayume Francis
 Author-email: admin@ayumefrancis.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj_maintenance-0.2.4/dj_maintenance.egg-info/SOURCES.txt` & `dj_maintenance-0.2.5/dj_maintenance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_maintenance-0.2.4/setup.cfg` & `dj_maintenance-0.2.5/setup.cfg`

 * *Files identical despite different names*

