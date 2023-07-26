# Comparing `tmp/extend_orfs_pyranges-0.1.0.tar.gz` & `tmp/extend_orfs_pyranges-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extend_orfs_pyranges-0.1.0.tar", last modified: Wed Jul 26 09:49:24 2023, max compression
+gzip compressed data, was "extend_orfs_pyranges-0.1.1.tar", last modified: Wed Jul 26 10:23:50 2023, max compression
```

## Comparing `extend_orfs_pyranges-0.1.0.tar` & `extend_orfs_pyranges-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:49:24.314982 extend_orfs_pyranges-0.1.0/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-26 09:49:24.314982 extend_orfs_pyranges-0.1.0/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      340 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.0/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.0/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      868 2023-07-26 09:49:24.314982 extend_orfs_pyranges-0.1.0/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.0/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:49:24.314982 extend_orfs_pyranges-0.1.0/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:49:24.314982 extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       80 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    23390 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges/extend_orfs_pyranges.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 09:49:24.314982 extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-26 09:49:24.000000 extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      405 2023-07-26 09:49:24.000000 extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-26 09:49:24.000000 extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       63 2023-07-26 09:49:24.000000 extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       21 2023-07-26 09:49:24.000000 extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:23:50.703333 extend_orfs_pyranges-0.1.1/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-26 10:23:50.703333 extend_orfs_pyranges-0.1.1/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      340 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.1/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.1/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      868 2023-07-26 10:23:50.703333 extend_orfs_pyranges-0.1.1/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.1/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:23:50.703333 extend_orfs_pyranges-0.1.1/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:23:50.703333 extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       80 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-26 10:22:40.000000 extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    23390 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges/extend_orfs_pyranges.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 10:23:50.703333 extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-26 10:23:50.000000 extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      405 2023-07-26 10:23:50.000000 extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-26 10:23:50.000000 extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       63 2023-07-26 10:23:50.000000 extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       21 2023-07-26 10:23:50.000000 extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges.egg-info/top_level.txt
```

### Comparing `extend_orfs_pyranges-0.1.0/PKG-INFO` & `extend_orfs_pyranges-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extend_orfs_pyranges
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fork of Joan Pallares extend_orf based on pyranges
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti and Joan Pallares
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `extend_orfs_pyranges-0.1.0/setup.cfg` & `extend_orfs_pyranges-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges/extend_orfs_pyranges.py` & `extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges/extend_orfs_pyranges.py`

 * *Files identical despite different names*

### Comparing `extend_orfs_pyranges-0.1.0/src/extend_orfs_pyranges.egg-info/PKG-INFO` & `extend_orfs_pyranges-0.1.1/src/extend_orfs_pyranges.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extend-orfs-pyranges
-Version: 0.1.0
+Version: 0.1.1
 Summary: Fork of Joan Pallares extend_orf based on pyranges
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti and Joan Pallares
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

