# Comparing `tmp/flytekitplugins-pod-1.8.1.tar.gz` & `tmp/flytekitplugins-pod-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-pod-1.8.1.tar", last modified: Tue Jul 18 18:01:38 2023, max compression
+gzip compressed data, was "flytekitplugins-pod-1.9.0a0.tar", last modified: Thu Jul 20 18:58:20 2023, max compression
```

## Comparing `flytekitplugins-pod-1.8.1.tar` & `flytekitplugins-pod-1.9.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:38.927021 flytekitplugins-pod-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-18 18:01:38.927021 flytekitplugins-pod-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-18 18:01:17.000000 flytekitplugins-pod-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:38.923021 flytekitplugins-pod-1.8.1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:38.923021 flytekitplugins-pod-1.8.1/flytekitplugins/pod/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-18 18:01:17.000000 flytekitplugins-pod-1.8.1/flytekitplugins/pod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-18 18:01:17.000000 flytekitplugins-pod-1.8.1/flytekitplugins/pod/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:38.923021 flytekitplugins-pod-1.8.1/flytekitplugins_pod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-18 18:01:38.000000 flytekitplugins-pod-1.8.1/flytekitplugins_pod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-18 18:01:38.000000 flytekitplugins-pod-1.8.1/flytekitplugins_pod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:38.000000 flytekitplugins-pod-1.8.1/flytekitplugins_pod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:38.000000 flytekitplugins-pod-1.8.1/flytekitplugins_pod.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 18:01:38.000000 flytekitplugins-pod-1.8.1/flytekitplugins_pod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:38.000000 flytekitplugins-pod-1.8.1/flytekitplugins_pod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:01:38.927021 flytekitplugins-pod-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-18 18:01:33.000000 flytekitplugins-pod-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:20.172687 flytekitplugins-pod-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 18:58:20.172687 flytekitplugins-pod-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-20 18:57:54.000000 flytekitplugins-pod-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:20.168687 flytekitplugins-pod-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:20.172687 flytekitplugins-pod-1.9.0a0/flytekitplugins/pod/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-20 18:57:54.000000 flytekitplugins-pod-1.9.0a0/flytekitplugins/pod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-20 18:57:54.000000 flytekitplugins-pod-1.9.0a0/flytekitplugins/pod/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:20.172687 flytekitplugins-pod-1.9.0a0/flytekitplugins_pod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 18:58:20.000000 flytekitplugins-pod-1.9.0a0/flytekitplugins_pod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 18:58:20.000000 flytekitplugins-pod-1.9.0a0/flytekitplugins_pod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:20.000000 flytekitplugins-pod-1.9.0a0/flytekitplugins_pod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:20.000000 flytekitplugins-pod-1.9.0a0/flytekitplugins_pod.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 18:58:20.000000 flytekitplugins-pod-1.9.0a0/flytekitplugins_pod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:20.000000 flytekitplugins-pod-1.9.0a0/flytekitplugins_pod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:20.172687 flytekitplugins-pod-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-20 18:58:12.000000 flytekitplugins-pod-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-pod-1.8.1/PKG-INFO` & `flytekitplugins-pod-1.9.0a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pod
-Version: 1.8.1
+Version: 1.9.0a0
 Summary: Flytekit plugin to support K8s Pod tasks
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pod-1.8.1/README.md` & `flytekitplugins-pod-1.9.0a0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pod-1.8.1/flytekitplugins/pod/task.py` & `flytekitplugins-pod-1.9.0a0/flytekitplugins/pod/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-pod-1.8.1/flytekitplugins_pod.egg-info/PKG-INFO` & `flytekitplugins-pod-1.9.0a0/flytekitplugins_pod.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-pod
-Version: 1.8.1
+Version: 1.9.0a0
 Summary: Flytekit plugin to support K8s Pod tasks
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-pod-1.8.1/setup.py` & `flytekitplugins-pod-1.9.0a0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "kubernetes>=12.0.1",
 ]
 
-__version__ = "1.8.1"
+__version__ = "1.9.0a0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="Flytekit plugin to support K8s Pod tasks",
```

