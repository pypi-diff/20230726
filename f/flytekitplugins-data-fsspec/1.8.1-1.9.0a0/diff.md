# Comparing `tmp/flytekitplugins-data-fsspec-1.8.1.tar.gz` & `tmp/flytekitplugins-data-fsspec-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-data-fsspec-1.8.1.tar", last modified: Tue Jul 18 18:01:35 2023, max compression
+gzip compressed data, was "flytekitplugins-data-fsspec-1.9.0a0.tar", last modified: Thu Jul 20 18:58:15 2023, max compression
```

## Comparing `flytekitplugins-data-fsspec-1.8.1.tar` & `flytekitplugins-data-fsspec-1.9.0a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:35.647021 flytekitplugins-data-fsspec-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-18 18:01:35.647021 flytekitplugins-data-fsspec-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-18 18:01:17.000000 flytekitplugins-data-fsspec-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:35.647021 flytekitplugins-data-fsspec-1.8.1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:35.647021 flytekitplugins-data-fsspec-1.8.1/flytekitplugins/fsspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:17.000000 flytekitplugins-data-fsspec-1.8.1/flytekitplugins/fsspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:35.647021 flytekitplugins-data-fsspec-1.8.1/flytekitplugins_data_fsspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-18 18:01:35.000000 flytekitplugins-data-fsspec-1.8.1/flytekitplugins_data_fsspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-18 18:01:35.000000 flytekitplugins-data-fsspec-1.8.1/flytekitplugins_data_fsspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:35.000000 flytekitplugins-data-fsspec-1.8.1/flytekitplugins_data_fsspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:35.000000 flytekitplugins-data-fsspec-1.8.1/flytekitplugins_data_fsspec.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 18:01:35.000000 flytekitplugins-data-fsspec-1.8.1/flytekitplugins_data_fsspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:35.000000 flytekitplugins-data-fsspec-1.8.1/flytekitplugins_data_fsspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:01:35.651021 flytekitplugins-data-fsspec-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-07-18 18:01:33.000000 flytekitplugins-data-fsspec-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:15.820635 flytekitplugins-data-fsspec-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-20 18:58:15.820635 flytekitplugins-data-fsspec-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-20 18:57:54.000000 flytekitplugins-data-fsspec-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:15.816635 flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:15.816635 flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins/fsspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins/fsspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:15.820635 flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins_data_fsspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-20 18:58:15.000000 flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins_data_fsspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-20 18:58:15.000000 flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins_data_fsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:15.000000 flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins_data_fsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:15.000000 flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins_data_fsspec.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 18:58:15.000000 flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins_data_fsspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:15.000000 flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins_data_fsspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:15.820635 flytekitplugins-data-fsspec-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-07-20 18:58:12.000000 flytekitplugins-data-fsspec-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-data-fsspec-1.8.1/PKG-INFO` & `flytekitplugins-data-fsspec-1.9.0a0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-data-fsspec
-Version: 1.8.1
+Version: 1.9.0a0
 Summary: This is a deprecated plugin as of flytekit 1.5
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-data-fsspec-1.8.1/flytekitplugins_data_fsspec.egg-info/PKG-INFO` & `flytekitplugins-data-fsspec-1.9.0a0/flytekitplugins_data_fsspec.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-data-fsspec
-Version: 1.8.1
+Version: 1.9.0a0
 Summary: This is a deprecated plugin as of flytekit 1.5
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-data-fsspec-1.8.1/setup.py` & `flytekitplugins-data-fsspec-1.9.0a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "fsspec"
 
 microlib_name = f"flytekitplugins-data-{PLUGIN_NAME}"
 
 plugin_requires = []
 
-__version__ = "1.8.1"
+__version__ = "1.9.0a0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is a deprecated plugin as of flytekit 1.5",
```

