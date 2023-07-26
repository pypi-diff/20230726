# Comparing `tmp/trochilidae-2.1.10.0.tar.gz` & `tmp/trochilidae-2.1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trochilidae-2.1.10.0.tar", last modified: Sun Mar  5 21:45:40 2023, max compression
+gzip compressed data, was "dist/trochilidae-2.1.4.0.tar", last modified: Sat May 15 21:08:11 2021, max compression
```

## Comparing `trochilidae-2.1.10.0.tar` & `trochilidae-2.1.4.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:45:40.419758 trochilidae-2.1.10.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-05 21:45:40.419758 trochilidae-2.1.10.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-05 21:45:40.419758 trochilidae-2.1.10.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:45:40.415758 trochilidae-2.1.10.0/trochilidae/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/interoperable_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/interoperable_get_arg_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/interoperable_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/interoperable_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/interoperable_with_metaclass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:45:40.415758 trochilidae-2.1.10.0/trochilidae/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/tests/test_interoperable_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/tests/test_interoperable_get_arg_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/tests/test_interoperable_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/tests/test_interoperable_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-05 21:45:32.000000 trochilidae-2.1.10.0/trochilidae/tests/test_interoperable_with_metaclass_import.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 21:45:40.415758 trochilidae-2.1.10.0/trochilidae.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-05 21:45:40.000000 trochilidae-2.1.10.0/trochilidae.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-05 21:45:40.000000 trochilidae-2.1.10.0/trochilidae.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 21:45:40.000000 trochilidae-2.1.10.0/trochilidae.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 21:45:40.000000 trochilidae-2.1.10.0/trochilidae.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-05 21:45:40.000000 trochilidae-2.1.10.0/trochilidae.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-05 21:45:40.000000 trochilidae-2.1.10.0/trochilidae.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 21:08:11.074439 trochilidae-2.1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2021-05-15 21:08:11.074439 trochilidae-2.1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2021-05-15 21:08:11.074439 trochilidae-2.1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 21:08:11.074439 trochilidae-2.1.4.0/trochilidae/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      230 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/interoperable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      260 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/interoperable_get_arg_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/interoperable_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/interoperable_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (121)      609 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/interoperable_with_metaclass.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 21:08:11.074439 trochilidae-2.1.4.0/trochilidae/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/tests/test_interoperable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/tests/test_interoperable_get_arg_spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)      208 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/tests/test_interoperable_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/tests/test_interoperable_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2021-05-15 21:07:54.000000 trochilidae-2.1.4.0/trochilidae/tests/test_interoperable_with_metaclass_import.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-15 21:08:11.074439 trochilidae-2.1.4.0/trochilidae.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      557 2021-05-15 21:08:10.000000 trochilidae-2.1.4.0/trochilidae.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2021-05-15 21:08:10.000000 trochilidae-2.1.4.0/trochilidae.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-15 21:08:10.000000 trochilidae-2.1.4.0/trochilidae.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-15 21:08:10.000000 trochilidae-2.1.4.0/trochilidae.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-05-15 21:08:10.000000 trochilidae-2.1.4.0/trochilidae.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-05-15 21:08:10.000000 trochilidae-2.1.4.0/trochilidae.egg-info/top_level.txt
```

### Comparing `trochilidae-2.1.10.0/PKG-INFO` & `trochilidae-2.1.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: trochilidae
-Version: 2.1.10.0
+Version: 2.1.4.0
 Summary: version interoperability library
 Home-page: https://github.com/MATTHEWFRAZER/trochilidae
 Author: Matthew Frazer
 Author-email: mfrazeriguess@gmail.com
 License: UNKNOWN
+Description: UNKNOWN
 Keywords: version interoperability
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `trochilidae-2.1.10.0/README.md` & `trochilidae-2.1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `trochilidae-2.1.10.0/setup.py` & `trochilidae-2.1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `trochilidae-2.1.10.0/trochilidae/interoperable_with_metaclass.py` & `trochilidae-2.1.4.0/trochilidae/interoperable_with_metaclass.py`

 * *Files identical despite different names*

### Comparing `trochilidae-2.1.10.0/trochilidae.egg-info/PKG-INFO` & `trochilidae-2.1.4.0/trochilidae.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: trochilidae
-Version: 2.1.10.0
+Version: 2.1.4.0
 Summary: version interoperability library
 Home-page: https://github.com/MATTHEWFRAZER/trochilidae
 Author: Matthew Frazer
 Author-email: mfrazeriguess@gmail.com
 License: UNKNOWN
+Description: UNKNOWN
 Keywords: version interoperability
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `trochilidae-2.1.10.0/trochilidae.egg-info/SOURCES.txt` & `trochilidae-2.1.4.0/trochilidae.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.cfg
 setup.py
 trochilidae/__init__.py
 trochilidae/interoperable_filter.py
 trochilidae/interoperable_get_arg_spec.py
 trochilidae/interoperable_map.py
```

