# Comparing `tmp/samplerate2-0.0.1.tar.gz` & `tmp/samplerate2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samplerate2-0.0.1.tar", last modified: Wed Jul 26 15:22:54 2023, max compression
+gzip compressed data, was "samplerate2-0.0.2.tar", last modified: Wed Jul 26 15:31:28 2023, max compression
```

## Comparing `samplerate2-0.0.1.tar` & `samplerate2-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:22:54.441470 samplerate2-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-26 15:22:10.000000 samplerate2-0.0.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 15:22:10.000000 samplerate2-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 15:22:10.000000 samplerate2-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-26 15:22:54.441470 samplerate2-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-26 15:22:10.000000 samplerate2-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:22:54.441470 samplerate2-0.0.1/external/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-26 15:22:10.000000 samplerate2-0.0.1/external/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 15:22:10.000000 samplerate2-0.0.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:22:54.441470 samplerate2-0.0.1/samplerate2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-26 15:22:54.000000 samplerate2-0.0.1/samplerate2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 15:22:54.000000 samplerate2-0.0.1/samplerate2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:22:54.000000 samplerate2-0.0.1/samplerate2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:22:30.000000 samplerate2-0.0.1/samplerate2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 15:22:54.000000 samplerate2-0.0.1/samplerate2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 15:22:54.000000 samplerate2-0.0.1/samplerate2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:22:54.441470 samplerate2-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-26 15:22:10.000000 samplerate2-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:22:54.441470 samplerate2-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-26 15:22:10.000000 samplerate2-0.0.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 15:22:10.000000 samplerate2-0.0.1/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-26 15:22:10.000000 samplerate2-0.0.1/tests/test_resampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:31:28.218526 samplerate2-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-26 15:30:53.000000 samplerate2-0.0.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 15:30:53.000000 samplerate2-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-26 15:30:53.000000 samplerate2-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-26 15:31:28.218526 samplerate2-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-26 15:30:53.000000 samplerate2-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:31:28.218526 samplerate2-0.0.2/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-26 15:30:53.000000 samplerate2-0.0.2/external/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 15:30:53.000000 samplerate2-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:31:28.218526 samplerate2-0.0.2/samplerate2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-26 15:31:28.000000 samplerate2-0.0.2/samplerate2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-26 15:31:28.000000 samplerate2-0.0.2/samplerate2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:31:28.000000 samplerate2-0.0.2/samplerate2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:31:08.000000 samplerate2-0.0.2/samplerate2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 15:31:28.000000 samplerate2-0.0.2/samplerate2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 15:31:28.000000 samplerate2-0.0.2/samplerate2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:31:28.218526 samplerate2-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-26 15:30:53.000000 samplerate2-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:31:28.218526 samplerate2-0.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 2023-07-26 15:30:53.000000 samplerate2-0.0.2/src/samplerate2.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:31:28.218526 samplerate2-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-26 15:30:53.000000 samplerate2-0.0.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 15:30:53.000000 samplerate2-0.0.2/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-26 15:30:53.000000 samplerate2-0.0.2/tests/test_resampling.py
```

### Comparing `samplerate2-0.0.1/CMakeLists.txt` & `samplerate2-0.0.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `samplerate2-0.0.1/LICENSE` & `samplerate2-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `samplerate2-0.0.1/setup.py` & `samplerate2-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="samplerate2",
-    version="0.0.1",
+    version="0.0.2",
     author="Robin Scheibler",
     author_email="fakufaku@gmail.com",
     url="https://github.com/fakufaku/python-samplerate2",
     description="Monolithic python wrapper for libsamplerate",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[CMakeExtension("samplerate2")],
```

### Comparing `samplerate2-0.0.1/tests/test_api.py` & `samplerate2-0.0.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `samplerate2-0.0.1/tests/test_resampling.py` & `samplerate2-0.0.2/tests/test_resampling.py`

 * *Files identical despite different names*

