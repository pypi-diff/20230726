# Comparing `tmp/juviz-app-0.1.0.tar.gz` & `tmp/juviz-app-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "juviz-app-0.1.0.tar", last modified: Mon Jul 24 12:04:32 2023, max compression
+gzip compressed data, was "juviz-app-0.1.1.tar", last modified: Wed Jul 26 11:14:22 2023, max compression
```

## Comparing `juviz-app-0.1.0.tar` & `juviz-app-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:04:32.952190 juviz-app-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-24 12:04:17.000000 juviz-app-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-24 12:04:32.952190 juviz-app-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-24 12:04:17.000000 juviz-app-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:04:32.952190 juviz-app-0.1.0/juviz/
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-24 12:04:17.000000 juviz-app-0.1.0/juviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:04:32.952190 juviz-app-0.1.0/juviz/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-24 12:04:17.000000 juviz-app-0.1.0/juviz/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:04:32.952190 juviz-app-0.1.0/juviz/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-24 12:04:17.000000 juviz-app-0.1.0/juviz/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-24 12:04:17.000000 juviz-app-0.1.0/juviz/widgets/juviz_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 12:04:32.952190 juviz-app-0.1.0/juviz_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-24 12:04:32.000000 juviz-app-0.1.0/juviz_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-24 12:04:32.000000 juviz-app-0.1.0/juviz_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 12:04:32.000000 juviz-app-0.1.0/juviz_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 12:04:32.000000 juviz-app-0.1.0/juviz_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 12:04:32.000000 juviz-app-0.1.0/juviz_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-24 12:04:32.952190 juviz-app-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 12:04:17.000000 juviz-app-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:14:22.479249 juviz-app-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-26 11:14:12.000000 juviz-app-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-26 11:14:22.479249 juviz-app-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 11:14:12.000000 juviz-app-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:14:22.479249 juviz-app-0.1.1/juviz/
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-07-26 11:14:12.000000 juviz-app-0.1.1/juviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:14:22.479249 juviz-app-0.1.1/juviz/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-26 11:14:12.000000 juviz-app-0.1.1/juviz/assets/FZJ_Logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-26 11:14:12.000000 juviz-app-0.1.1/juviz/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:14:22.479249 juviz-app-0.1.1/juviz/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-26 11:14:12.000000 juviz-app-0.1.1/juviz/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-07-26 11:14:12.000000 juviz-app-0.1.1/juviz/widgets/juviz_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:14:22.479249 juviz-app-0.1.1/juviz_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-26 11:14:22.000000 juviz-app-0.1.1/juviz_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-26 11:14:22.000000 juviz-app-0.1.1/juviz_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:14:22.000000 juviz-app-0.1.1/juviz_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 11:14:22.000000 juviz-app-0.1.1/juviz_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 11:14:22.000000 juviz-app-0.1.1/juviz_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-26 11:14:22.479249 juviz-app-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:14:12.000000 juviz-app-0.1.1/setup.py
```

### Comparing `juviz-app-0.1.0/LICENSE` & `juviz-app-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `juviz-app-0.1.0/PKG-INFO` & `juviz-app-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juviz-app
-Version: 0.1.0
+Version: 0.1.1
 Summary: Default trame App for JuViz
 Author: Jonathan Windgassen
 Author-email: j.windgassen@fz-juelich.de
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Web Environment
```

### Comparing `juviz-app-0.1.0/juviz/__init__.py` & `juviz-app-0.1.1/juviz/__init__.py`

 * *Files identical despite different names*

### Comparing `juviz-app-0.1.0/juviz/widgets/__init__.py` & `juviz-app-0.1.1/juviz/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `juviz-app-0.1.0/juviz/widgets/juviz_controller.py` & `juviz-app-0.1.1/juviz/widgets/juviz_controller.py`

 * *Files identical despite different names*

### Comparing `juviz-app-0.1.0/juviz_app.egg-info/PKG-INFO` & `juviz-app-0.1.1/juviz_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: juviz-app
-Version: 0.1.0
+Version: 0.1.1
 Summary: Default trame App for JuViz
 Author: Jonathan Windgassen
 Author-email: j.windgassen@fz-juelich.de
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Environment :: Web Environment
```

### Comparing `juviz-app-0.1.0/setup.cfg` & `juviz-app-0.1.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = juviz-app
-version = 0.1.0
+version = 0.1.1
 description = Default trame App for JuViz
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Jonathan Windgassen
 author_email = j.windgassen@fz-juelich.de
 license = BSD License
 classifiers = 
@@ -25,14 +25,17 @@
 
 [options]
 packages = find:
 include_package_data = True
 install_requires = 
 	pv_visualizer
 
+[options.package_data]
+juviz.assets = *.svg
+
 [semantic_release]
 version_pattern = setup.cfg:version = (\d+\.\d+\.\d+)
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

