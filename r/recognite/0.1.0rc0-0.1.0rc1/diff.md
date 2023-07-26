# Comparing `tmp/recognite-0.1.0rc0.tar.gz` & `tmp/recognite-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recognite-0.1.0rc0.tar", last modified: Wed Jul 26 11:23:27 2023, max compression
+gzip compressed data, was "recognite-0.1.0rc1.tar", last modified: Wed Jul 26 12:29:48 2023, max compression
```

## Comparing `recognite-0.1.0rc0.tar` & `recognite-0.1.0rc1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:23:27.329775 recognite-0.1.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-26 11:23:17.000000 recognite-0.1.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-26 11:23:27.329775 recognite-0.1.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-26 11:23:17.000000 recognite-0.1.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:23:27.329775 recognite-0.1.0rc0/recognite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-26 11:23:27.000000 recognite-0.1.0rc0/recognite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-26 11:23:27.000000 recognite-0.1.0rc0/recognite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:23:27.000000 recognite-0.1.0rc0/recognite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:23:27.000000 recognite-0.1.0rc0/recognite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 11:23:27.000000 recognite-0.1.0rc0/recognite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:23:27.000000 recognite-0.1.0rc0/recognite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:23:27.329775 recognite-0.1.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-26 11:23:17.000000 recognite-0.1.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:48.709915 recognite-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-26 12:29:36.000000 recognite-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-26 12:29:48.709915 recognite-0.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-26 12:29:36.000000 recognite-0.1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:29:48.709915 recognite-0.1.0rc1/recognite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:29:48.000000 recognite-0.1.0rc1/recognite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:29:48.709915 recognite-0.1.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-07-26 12:29:36.000000 recognite-0.1.0rc1/setup.py
```

### Comparing `recognite-0.1.0rc0/LICENSE` & `recognite-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `recognite-0.1.0rc0/PKG-INFO` & `recognite-0.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recognite
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: Recognite is a library to kickstart your next PyTorch-based recognition project.
 Home-page: https://github.com/florisdf/recognite
 Author: Floris De Feyter
 Author-email: floris.defeyter@kuleuven.be
 License: MIT license
 Keywords: recognite
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `recognite-0.1.0rc0/recognite.egg-info/PKG-INFO` & `recognite-0.1.0rc1/recognite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recognite
-Version: 0.1.0rc0
+Version: 0.1.0rc1
 Summary: Recognite is a library to kickstart your next PyTorch-based recognition project.
 Home-page: https://github.com/florisdf/recognite
 Author: Floris De Feyter
 Author-email: floris.defeyter@kuleuven.be
 License: MIT license
 Keywords: recognite
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `recognite-0.1.0rc0/setup.py` & `recognite-0.1.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords='recognite',
     name='recognite',
     packages=find_packages(include=['recognite', 'recognite.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/florisdf/recognite',
-    version='0.1.0-rc0',
+    version='0.1.0-rc1',
     zip_safe=False,
 )
```

