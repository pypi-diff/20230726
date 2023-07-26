# Comparing `tmp/flytekitplugins-kfpytorch-1.8.1.tar.gz` & `tmp/flytekitplugins-kfpytorch-1.9.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-kfpytorch-1.8.1.tar", last modified: Tue Jul 18 18:01:39 2023, max compression
+gzip compressed data, was "flytekitplugins-kfpytorch-1.9.0a0.tar", last modified: Thu Jul 20 18:58:21 2023, max compression
```

## Comparing `flytekitplugins-kfpytorch-1.8.1.tar` & `flytekitplugins-kfpytorch-1.9.0a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:39.659021 flytekitplugins-kfpytorch-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-18 18:01:39.659021 flytekitplugins-kfpytorch-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-18 18:01:17.000000 flytekitplugins-kfpytorch-1.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:39.655022 flytekitplugins-kfpytorch-1.8.1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:39.655022 flytekitplugins-kfpytorch-1.8.1/flytekitplugins/kfpytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-18 18:01:17.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins/kfpytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16802 2023-07-18 18:01:17.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins/kfpytorch/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:01:39.659021 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:01:39.000000 flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:01:39.659021 flytekitplugins-kfpytorch-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-18 18:01:33.000000 flytekitplugins-kfpytorch-1.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.128697 flytekitplugins-kfpytorch-1.9.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-20 18:58:21.128697 flytekitplugins-kfpytorch-1.9.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-20 18:57:54.000000 flytekitplugins-kfpytorch-1.9.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.124697 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.124697 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins/kfpytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 18:57:54.000000 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins/kfpytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9425 2023-07-20 18:57:54.000000 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins/kfpytorch/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:21.128697 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins_kfpytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-20 18:58:21.000000 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins_kfpytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-20 18:58:21.000000 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins_kfpytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:21.000000 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins_kfpytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:21.000000 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins_kfpytorch.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-20 18:58:21.000000 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins_kfpytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 18:58:21.000000 flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins_kfpytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 18:58:21.128697 flytekitplugins-kfpytorch-1.9.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-07-20 18:58:12.000000 flytekitplugins-kfpytorch-1.9.0a0/setup.py
```

### Comparing `flytekitplugins-kfpytorch-1.8.1/PKG-INFO` & `flytekitplugins-kfpytorch-1.9.0a0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.8.1
+Version: 1.9.0a0
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.8.1/flytekitplugins_kfpytorch.egg-info/PKG-INFO` & `flytekitplugins-kfpytorch-1.9.0a0/flytekitplugins_kfpytorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-kfpytorch
-Version: 1.8.1
+Version: 1.9.0a0
 Summary: K8s based Pytorch plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-kfpytorch-1.8.1/setup.py` & `flytekitplugins-kfpytorch-1.9.0a0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 PLUGIN_NAME = "kfpytorch"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
-plugin_requires = ["cloudpickle", "flyteidl>=1.5.1", "flytekit>=1.6.1"]
+plugin_requires = ["cloudpickle", "flytekit>=1.3.0,<2.0.0", "flyteidl>=1.3.19"]
 
-__version__ = "1.8.1"
+__version__ = "1.9.0a0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="K8s based Pytorch plugin for Flytekit",
```

