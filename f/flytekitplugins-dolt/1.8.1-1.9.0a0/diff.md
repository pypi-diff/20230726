# Comparing `tmp/flytekitplugins-dolt-1.8.1.tar.gz` & `tmp/flytekitplugins-dolt-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-dolt-1.8.1.tar", last modified: Tue Jul 18 18:01:36 2023, max compression
+gzip compressed data, was "flytekitplugins-dolt-1.9.0a0.tar", last modified: Thu Jul 20 18:58:17 2023, max compression
```

## Comparing `flytekitplugins-dolt-1.8.1.tar` & `flytekitplugins-dolt-1.9.0a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:36.755021 flytekitplugins-dolt-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-18 18:01:36.755021 flytekitplugins-dolt-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-18 18:01:17.000000 flytekitplugins-dolt-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:36.755021 flytekitplugins-dolt-1.8.1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:36.755021 flytekitplugins-dolt-1.8.1/flytekitplugins/dolt/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-18 18:01:17.000000 flytekitplugins-dolt-1.8.1/flytekitplugins/dolt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-18 18:01:17.000000 flytekitplugins-dolt-1.8.1/flytekitplugins/dolt/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:36.755021 flytekitplugins-dolt-1.8.1/flytekitplugins_dolt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-18 18:01:36.000000 flytekitplugins-dolt-1.8.1/flytekitplugins_dolt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-18 18:01:36.000000 flytekitplugins-dolt-1.8.1/flytekitplugins_dolt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:36.000000 flytekitplugins-dolt-1.8.1/flytekitplugins_dolt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:36.000000 flytekitplugins-dolt-1.8.1/flytekitplugins_dolt.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 18:01:36.000000 flytekitplugins-dolt-1.8.1/flytekitplugins_dolt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:36.000000 flytekitplugins-dolt-1.8.1/flytekitplugins_dolt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:36.755021 flytekitplugins-dolt-1.8.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 18:01:17.000000 flytekitplugins-dolt-1.8.1/scripts/flytekit_install_dolt.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:01:36.755021 flytekitplugins-dolt-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-18 18:01:33.000000 flytekitplugins-dolt-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:17.272654 flytekitplugins-dolt-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-20 18:58:17.272654 flytekitplugins-dolt-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-20 18:57:54.000000 flytekitplugins-dolt-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:17.272654 flytekitplugins-dolt-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:17.272654 flytekitplugins-dolt-1.9.0a0/flytekitplugins/dolt/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 18:57:54.000000 flytekitplugins-dolt-1.9.0a0/flytekitplugins/dolt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-20 18:57:54.000000 flytekitplugins-dolt-1.9.0a0/flytekitplugins/dolt/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:17.272654 flytekitplugins-dolt-1.9.0a0/flytekitplugins_dolt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-20 18:58:17.000000 flytekitplugins-dolt-1.9.0a0/flytekitplugins_dolt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 18:58:17.000000 flytekitplugins-dolt-1.9.0a0/flytekitplugins_dolt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:17.000000 flytekitplugins-dolt-1.9.0a0/flytekitplugins_dolt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:17.000000 flytekitplugins-dolt-1.9.0a0/flytekitplugins_dolt.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 18:58:17.000000 flytekitplugins-dolt-1.9.0a0/flytekitplugins_dolt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:17.000000 flytekitplugins-dolt-1.9.0a0/flytekitplugins_dolt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:17.272654 flytekitplugins-dolt-1.9.0a0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 18:57:54.000000 flytekitplugins-dolt-1.9.0a0/scripts/flytekit_install_dolt.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:17.272654 flytekitplugins-dolt-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-20 18:58:12.000000 flytekitplugins-dolt-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-dolt-1.8.1/PKG-INFO` & `flytekitplugins-dolt-1.9.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-dolt
-Version: 1.8.1
+Version: 1.9.0a0
 Summary: Dolt plugin for flytekit
 Author: dolthub
 Author-email: max@dolthub.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-dolt-1.8.1/README.md` & `flytekitplugins-dolt-1.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-dolt-1.8.1/flytekitplugins/dolt/schema.py` & `flytekitplugins-dolt-1.9.0a0/flytekitplugins/dolt/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-dolt-1.8.1/flytekitplugins_dolt.egg-info/PKG-INFO` & `flytekitplugins-dolt-1.9.0a0/flytekitplugins_dolt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-dolt
-Version: 1.8.1
+Version: 1.9.0a0
 Summary: Dolt plugin for flytekit
 Author: dolthub
 Author-email: max@dolthub.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-dolt-1.8.1/setup.py` & `flytekitplugins-dolt-1.9.0a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PLUGIN_NAME = "dolt"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "dolt_integrations>=0.1.5"]
 dev_requires = ["pytest-mock>=3.6.1"]
 
-__version__ = "1.8.1"
+__version__ = "1.9.0a0"
 
 
 class PostDevelopCommand(develop):
     """Post-installation for development mode."""
 
     def run(self):
         develop.run(self)
```

