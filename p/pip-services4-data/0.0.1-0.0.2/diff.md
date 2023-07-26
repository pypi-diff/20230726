# Comparing `tmp/pip_services4_data-0.0.1.tar.gz` & `tmp/pip_services4_data-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_data-0.0.1.tar", last modified: Tue Jul 25 23:38:18 2023, max compression
+gzip compressed data, was "pip_services4_data-0.0.2.tar", last modified: Wed Jul 26 00:16:01 2023, max compression
```

## Comparing `pip_services4_data-0.0.1.tar` & `pip_services4_data-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 23:38:18.670011 pip_services4_data-0.0.1/
--rw-rw-rw-   0        0        0      297 2023-07-25 23:10:37.000000 pip_services4_data-0.0.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1076 2020-12-11 04:36:42.000000 pip_services4_data-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       54 2020-12-11 04:36:42.000000 pip_services4_data-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2490 2023-07-25 23:38:18.671015 pip_services4_data-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1574 2023-07-25 23:11:05.000000 pip_services4_data-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 23:38:18.670011 pip_services4_data-0.0.1/pip_services4_data.egg-info/
--rw-rw-rw-   0        0        0     2490 2023-07-25 23:38:18.000000 pip_services4_data-0.0.1/pip_services4_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-07-25 23:38:18.000000 pip_services4_data-0.0.1/pip_services4_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 23:38:18.000000 pip_services4_data-0.0.1/pip_services4_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-25 23:38:18.000000 pip_services4_data-0.0.1/pip_services4_data.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 23:38:18.000000 pip_services4_data-0.0.1/pip_services4_data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 23:38:18.000000 pip_services4_data-0.0.1/pip_services4_data.egg-info/zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-25 23:38:18.676077 pip_services4_data-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1587 2023-07-25 23:11:42.000000 pip_services4_data-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:16:01.311191 pip_services4_data-0.0.2/
+-rw-rw-rw-   0        0        0      297 2023-07-25 23:10:37.000000 pip_services4_data-0.0.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1076 2020-12-11 04:36:42.000000 pip_services4_data-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-12-11 04:36:42.000000 pip_services4_data-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2490 2023-07-26 00:16:01.311191 pip_services4_data-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1574 2023-07-25 23:11:05.000000 pip_services4_data-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 00:16:01.310190 pip_services4_data-0.0.2/pip_services4_data.egg-info/
+-rw-rw-rw-   0        0        0     2490 2023-07-26 00:16:01.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-07-26 00:16:01.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 00:16:01.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-07-26 00:16:01.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 00:16:01.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-25 23:38:18.000000 pip_services4_data-0.0.2/pip_services4_data.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-26 00:16:01.313192 pip_services4_data-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1587 2023-07-26 00:15:45.000000 pip_services4_data-0.0.2/setup.py
```

### Comparing `pip_services4_data-0.0.1/LICENSE` & `pip_services4_data-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_data-0.0.1/PKG-INFO` & `pip_services4_data-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_data
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data processing and persistence components for Pip.Services in Python
 Home-page: http://github.com/pip-services3-python/pip-services4-data-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_data-0.0.1/README.md` & `pip_services4_data-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pip_services4_data-0.0.1/pip_services4_data.egg-info/PKG-INFO` & `pip_services4_data-0.0.2/pip_services4_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-services4-data
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data processing and persistence components for Pip.Services in Python
 Home-page: http://github.com/pip-services3-python/pip-services4-data-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_data-0.0.1/setup.py` & `pip_services4_data-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 try:
     readme = open('readme.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_data',
-    version='0.0.1',
+    version='0.0.2',
     url='http://github.com/pip-services3-python/pip-services4-data-python',
     license='MIT',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     description='Data processing and persistence components for Pip.Services in Python',
     long_description=readme,
     long_description_content_type="text/markdown",
```

