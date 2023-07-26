# Comparing `tmp/mcqgen-0.1.4.tar.gz` & `tmp/mcqgen-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqgen-0.1.4.tar", last modified: Wed Jul 26 00:13:44 2023, max compression
+gzip compressed data, was "mcqgen-1.0.0.tar", last modified: Wed Jul 26 00:29:31 2023, max compression
```

## Comparing `mcqgen-0.1.4.tar` & `mcqgen-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:13:44.112968 mcqgen-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 00:13:41.000000 mcqgen-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-26 00:13:44.112968 mcqgen-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-26 00:13:41.000000 mcqgen-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:13:44.112968 mcqgen-0.1.4/mcqgen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:13:41.000000 mcqgen-0.1.4/mcqgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-26 00:13:41.000000 mcqgen-0.1.4/mcqgen/mcqgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:13:44.112968 mcqgen-0.1.4/mcqgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-26 00:13:44.000000 mcqgen-0.1.4/mcqgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-26 00:13:44.000000 mcqgen-0.1.4/mcqgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:13:44.000000 mcqgen-0.1.4/mcqgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:13:44.000000 mcqgen-0.1.4/mcqgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:13:44.000000 mcqgen-0.1.4/mcqgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 00:13:44.112968 mcqgen-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-26 00:13:41.000000 mcqgen-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:29:31.640954 mcqgen-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 00:29:29.000000 mcqgen-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-26 00:29:31.640954 mcqgen-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-26 00:29:29.000000 mcqgen-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:29:31.636954 mcqgen-1.0.0/mcqgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:29:29.000000 mcqgen-1.0.0/mcqgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-26 00:29:29.000000 mcqgen-1.0.0/mcqgen/mcqgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:29:31.640954 mcqgen-1.0.0/mcqgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-26 00:29:31.000000 mcqgen-1.0.0/mcqgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-26 00:29:31.000000 mcqgen-1.0.0/mcqgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:29:31.000000 mcqgen-1.0.0/mcqgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:29:31.000000 mcqgen-1.0.0/mcqgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:29:31.000000 mcqgen-1.0.0/mcqgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 00:29:31.640954 mcqgen-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-26 00:29:29.000000 mcqgen-1.0.0/setup.py
```

### Comparing `mcqgen-0.1.4/LICENSE` & `mcqgen-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqgen-0.1.4/PKG-INFO` & `mcqgen-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: mcqgen
-Version: 0.1.4
+Version: 1.0.0
 Summary: Generate Multiple Choice Questions, Choices and Correct Answer in JSON Format
+Home-page: https://github.com/55abhilash/mcqgen
 Author: Abhilash Mhaisne
+Author-email: abhilashmhaisne@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mcqgen
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

### Comparing `mcqgen-0.1.4/README.md` & `mcqgen-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mcqgen-0.1.4/mcqgen.egg-info/PKG-INFO` & `mcqgen-1.0.0/mcqgen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: mcqgen
-Version: 0.1.4
+Version: 1.0.0
 Summary: Generate Multiple Choice Questions, Choices and Correct Answer in JSON Format
+Home-page: https://github.com/55abhilash/mcqgen
 Author: Abhilash Mhaisne
+Author-email: abhilashmhaisne@gmail.com
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mcqgen
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

