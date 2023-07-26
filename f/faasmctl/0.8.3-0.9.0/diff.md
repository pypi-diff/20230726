# Comparing `tmp/faasmctl-0.8.3.tar.gz` & `tmp/faasmctl-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faasmctl-0.8.3.tar", last modified: Tue Jul 25 07:57:31 2023, max compression
+gzip compressed data, was "faasmctl-0.9.0.tar", last modified: Wed Jul 26 14:25:44 2023, max compression
```

## Comparing `faasmctl-0.8.3.tar` & `faasmctl-0.9.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:57:31.992661 faasmctl-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-25 07:55:27.000000 faasmctl-0.8.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-25 07:57:31.992661 faasmctl-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-25 07:55:27.000000 faasmctl-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:57:31.988661 faasmctl-0.8.3/faasmctl/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:57:31.988661 faasmctl-0.8.3/faasmctl/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/tasks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/tasks/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/tasks/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/tasks/flush.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/tasks/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/tasks/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/tasks/restart.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/tasks/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/tasks/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:57:31.988661 faasmctl-0.8.3/faasmctl/util/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/faasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/flush.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:57:31.992661 faasmctl-0.8.3/faasmctl/util/gen_proto/
--rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-25 07:57:17.000000 faasmctl-0.8.3/faasmctl/util/gen_proto/faabric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-25 07:57:17.000000 faasmctl-0.8.3/faasmctl/util/gen_proto/planner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/invoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/planner.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 07:55:27.000000 faasmctl-0.8.3/faasmctl/util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:57:31.988661 faasmctl-0.8.3/faasmctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-25 07:57:31.000000 faasmctl-0.8.3/faasmctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-25 07:57:31.000000 faasmctl-0.8.3/faasmctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:57:31.000000 faasmctl-0.8.3/faasmctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 07:57:31.000000 faasmctl-0.8.3/faasmctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 07:57:31.000000 faasmctl-0.8.3/faasmctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 07:57:31.000000 faasmctl-0.8.3/faasmctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-25 07:55:27.000000 faasmctl-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 07:57:31.992661 faasmctl-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:25:44.471477 faasmctl-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-26 14:23:41.000000 faasmctl-0.9.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-26 14:25:44.471477 faasmctl-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-26 14:23:41.000000 faasmctl-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:25:44.467477 faasmctl-0.9.0/faasmctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:25:44.471477 faasmctl-0.9.0/faasmctl/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/tasks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/tasks/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/tasks/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/tasks/flush.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/tasks/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/tasks/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/tasks/restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/tasks/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/tasks/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:25:44.471477 faasmctl-0.9.0/faasmctl/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10973 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/faasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/flush.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:25:44.471477 faasmctl-0.9.0/faasmctl/util/gen_proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-07-26 14:25:34.000000 faasmctl-0.9.0/faasmctl/util/gen_proto/faabric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-26 14:25:34.000000 faasmctl-0.9.0/faasmctl/util/gen_proto/planner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/invoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/planner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 14:23:41.000000 faasmctl-0.9.0/faasmctl/util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:25:44.471477 faasmctl-0.9.0/faasmctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-26 14:25:44.000000 faasmctl-0.9.0/faasmctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-26 14:25:44.000000 faasmctl-0.9.0/faasmctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:25:44.000000 faasmctl-0.9.0/faasmctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 14:25:44.000000 faasmctl-0.9.0/faasmctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 14:25:44.000000 faasmctl-0.9.0/faasmctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 14:25:44.000000 faasmctl-0.9.0/faasmctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-26 14:23:41.000000 faasmctl-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-26 14:25:44.471477 faasmctl-0.9.0/setup.cfg
```

### Comparing `faasmctl-0.8.3/LICENSE.md` & `faasmctl-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/PKG-INFO` & `faasmctl-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.8.3
+Version: 0.9.0
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.8.3
+pip install faasmctl==0.9.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.8.3/README.md` & `faasmctl-0.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.8.3
+pip install faasmctl==0.9.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.8.3/faasmctl/tasks/cli.py` & `faasmctl-0.9.0/faasmctl/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/tasks/delete.py` & `faasmctl-0.9.0/faasmctl/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/tasks/deploy.py` & `faasmctl-0.9.0/faasmctl/tasks/deploy.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
     deploy_compose_cluster,
     populate_host_sysroot,
     run_compose_cmd,
 )
 from faasmctl.util.deploy import fetch_faasm_code
 from faasmctl.util.k8s import DEFAULT_KUBECONFIG_PATH, deploy_k8s_cluster
 from invoke import task
+from os import environ
 from os.path import abspath
 
 
 @task
 def compose(ctx, workers=2, mount_source=None, clean=False, ini_file=None):
     """
     Deploy a Faasm cluster on docker compose
@@ -87,13 +88,15 @@
     Returns:
     - (str): path to the generated ini_file
     """
     # First, check-out the Faasm source if necessary (we need it for the k8s
     # deployment files, eventually we could publish them as helm charts)
     faasm_checkout, faasm_ver = fetch_faasm_code()
 
-    if not context:
-        context = DEFAULT_KUBECONFIG_PATH
-    else:
+    if context:
         context = abspath(context)
+    elif "KUBECONFIG" in environ:
+        context = abspath(environ["KUBECONFIG"])
+    else:
+        context = DEFAULT_KUBECONFIG_PATH
 
     return deploy_k8s_cluster(context, faasm_checkout, workers, ini_file)
```

### Comparing `faasmctl-0.8.3/faasmctl/tasks/flush.py` & `faasmctl-0.9.0/faasmctl/tasks/flush.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/tasks/invoke.py` & `faasmctl-0.9.0/faasmctl/tasks/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/tasks/logs.py` & `faasmctl-0.9.0/faasmctl/tasks/logs.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/tasks/restart.py` & `faasmctl-0.9.0/faasmctl/tasks/restart.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/tasks/status.py` & `faasmctl-0.9.0/faasmctl/tasks/status.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/util/compose.py` & `faasmctl-0.9.0/faasmctl/util/compose.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/util/config.py` & `faasmctl-0.9.0/faasmctl/util/config.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/util/deploy.py` & `faasmctl-0.9.0/faasmctl/util/deploy.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/util/docker.py` & `faasmctl-0.9.0/faasmctl/util/docker.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/util/faasm.py` & `faasmctl-0.9.0/faasmctl/util/faasm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from os import environ
 
-FAASM_VERSION = "0.10.0"
+FAASM_VERSION = "0.10.2"
 
 
 def get_version():
     """
     Get the Faasm version to check-out the source from
 
     Faasmctl ships with a default Faasm version (`FAASM_VERSION` in this file)
```

### Comparing `faasmctl-0.8.3/faasmctl/util/flush.py` & `faasmctl-0.9.0/faasmctl/util/flush.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,14 @@
         )
         raise RuntimeError("POST request to flush failed!")
 
     print("Response ({}): {}".format(response.status_code, response.text))
 
 
 def flush_hosts(ini_file=None):
-    msg = prepare_planner_msg("FLUSH_HOSTS")
+    msg = prepare_planner_msg("FLUSH_AVAILABLE_HOSTS")
     do_flush(msg, ini_file)
 
 
 def flush_workers(ini_file=None):
     msg = prepare_planner_msg("FLUSH_EXECUTORS")
     do_flush(msg, ini_file)
```

### Comparing `faasmctl-0.8.3/faasmctl/util/gen_proto/faabric_pb2.py` & `faasmctl-0.9.0/faasmctl/util/gen_proto/faabric_pb2.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/util/gen_proto/planner_pb2.py` & `faasmctl-0.9.0/faasmctl/util/gen_proto/planner_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19src/planner/planner.proto\x12\x0f\x66\x61\x61\x62ric.planner\"\x1e\n\rEmptyResponse\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"\x1d\n\x0c\x45mptyRequest\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"e\n\x0eResponseStatus\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.faabric.planner.ResponseStatus.Status\"\x1b\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x1c\n\tTimestamp\x12\x0f\n\x07\x65pochMs\x18\x01 \x01(\x03\"\xff\x01\n\x0bHttpMessage\x12:\n\x04type\x18\x01 \x01(\x0e\x32!.faabric.planner.HttpMessage.TypeR\thttp_type\x12\x1c\n\x0bpayloadJson\x18\x02 \x01(\tR\x07payload\"\x95\x01\n\x04Type\x12\x0b\n\x07NO_TYPE\x10\x00\x12\t\n\x05RESET\x10\x01\x12\x0f\n\x0b\x46LUSH_HOSTS\x10\x02\x12\x13\n\x0f\x46LUSH_EXECUTORS\x10\x03\x12\x0e\n\nGET_CONFIG\x10\x04\x12\x12\n\x0eGET_EXEC_GRAPH\x10\x05\x12\x11\n\rEXECUTE_BATCH\x10\x06\x12\x18\n\x14\x45XECUTE_BATCH_STATUS\x10\x07\"N\n\rPlannerConfig\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x13\n\x0bhostTimeout\x18\x02 \x01(\x05\x12\x1c\n\x14numThreadsHttpServer\x18\x03 \x01(\x05\"d\n\x04Host\x12\n\n\x02ip\x18\x01 \x01(\t\x12\r\n\x05slots\x18\x02 \x01(\x05\x12\x11\n\tusedSlots\x18\x03 \x01(\x05\x12.\n\nregisterTs\x18\x04 \x01(\x0b\x32\x1a.faabric.planner.Timestamp\">\n\x0cPingResponse\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\"M\n\x13RegisterHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\x12\x11\n\toverwrite\x18\x02 \x01(\x08\"\x87\x01\n\x14RegisterHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\x12.\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\x12\x0e\n\x06hostId\x18\x03 \x01(\x05\"8\n\x11RemoveHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\"E\n\x12RemoveHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\">\n\x16\x41vailableHostsResponse\x12$\n\x05hosts\x18\x01 \x03(\x0b\x32\x15.faabric.planner.Hostb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19src/planner/planner.proto\x12\x0f\x66\x61\x61\x62ric.planner\"\x1e\n\rEmptyResponse\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"\x1d\n\x0c\x45mptyRequest\x12\r\n\x05\x65mpty\x18\x01 \x01(\x05\"e\n\x0eResponseStatus\x12\x36\n\x06status\x18\x01 \x01(\x0e\x32&.faabric.planner.ResponseStatus.Status\"\x1b\n\x06Status\x12\x06\n\x02OK\x10\x00\x12\t\n\x05\x45RROR\x10\x01\"\x1c\n\tTimestamp\x12\x0f\n\x07\x65pochMs\x18\x01 \x01(\x03\"\xa2\x02\n\x0bHttpMessage\x12:\n\x04type\x18\x01 \x01(\x0e\x32!.faabric.planner.HttpMessage.TypeR\thttp_type\x12\x1c\n\x0bpayloadJson\x18\x02 \x01(\tR\x07payload\"\xb8\x01\n\x04Type\x12\x0b\n\x07NO_TYPE\x10\x00\x12\t\n\x05RESET\x10\x01\x12\x19\n\x15\x46LUSH_AVAILABLE_HOSTS\x10\x02\x12\x13\n\x0f\x46LUSH_EXECUTORS\x10\x03\x12\x17\n\x13GET_AVAILABLE_HOSTS\x10\x04\x12\x0e\n\nGET_CONFIG\x10\x05\x12\x12\n\x0eGET_EXEC_GRAPH\x10\x06\x12\x11\n\rEXECUTE_BATCH\x10\x07\x12\x18\n\x14\x45XECUTE_BATCH_STATUS\x10\x08\"N\n\rPlannerConfig\x12\n\n\x02ip\x18\x01 \x01(\t\x12\x13\n\x0bhostTimeout\x18\x02 \x01(\x05\x12\x1c\n\x14numThreadsHttpServer\x18\x03 \x01(\x05\"d\n\x04Host\x12\n\n\x02ip\x18\x01 \x01(\t\x12\r\n\x05slots\x18\x02 \x01(\x05\x12\x11\n\tusedSlots\x18\x03 \x01(\x05\x12.\n\nregisterTs\x18\x04 \x01(\x0b\x32\x1a.faabric.planner.Timestamp\">\n\x0cPingResponse\x12.\n\x06\x63onfig\x18\x01 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\"M\n\x13RegisterHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\x12\x11\n\toverwrite\x18\x02 \x01(\x08\"\x87\x01\n\x14RegisterHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\x12.\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x1e.faabric.planner.PlannerConfig\x12\x0e\n\x06hostId\x18\x03 \x01(\x05\"8\n\x11RemoveHostRequest\x12#\n\x04host\x18\x01 \x01(\x0b\x32\x15.faabric.planner.Host\"E\n\x12RemoveHostResponse\x12/\n\x06status\x18\x01 \x01(\x0b\x32\x1f.faabric.planner.ResponseStatus\">\n\x16\x41vailableHostsResponse\x12$\n\x05hosts\x18\x01 \x03(\x0b\x32\x15.faabric.planner.Hostb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'src.planner.planner_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _EMPTYRESPONSE._serialized_start=46
@@ -27,27 +27,27 @@
   _RESPONSESTATUS._serialized_start=109
   _RESPONSESTATUS._serialized_end=210
   _RESPONSESTATUS_STATUS._serialized_start=183
   _RESPONSESTATUS_STATUS._serialized_end=210
   _TIMESTAMP._serialized_start=212
   _TIMESTAMP._serialized_end=240
   _HTTPMESSAGE._serialized_start=243
-  _HTTPMESSAGE._serialized_end=498
+  _HTTPMESSAGE._serialized_end=533
   _HTTPMESSAGE_TYPE._serialized_start=349
-  _HTTPMESSAGE_TYPE._serialized_end=498
-  _PLANNERCONFIG._serialized_start=500
-  _PLANNERCONFIG._serialized_end=578
-  _HOST._serialized_start=580
-  _HOST._serialized_end=680
-  _PINGRESPONSE._serialized_start=682
-  _PINGRESPONSE._serialized_end=744
-  _REGISTERHOSTREQUEST._serialized_start=746
-  _REGISTERHOSTREQUEST._serialized_end=823
-  _REGISTERHOSTRESPONSE._serialized_start=826
-  _REGISTERHOSTRESPONSE._serialized_end=961
-  _REMOVEHOSTREQUEST._serialized_start=963
-  _REMOVEHOSTREQUEST._serialized_end=1019
-  _REMOVEHOSTRESPONSE._serialized_start=1021
-  _REMOVEHOSTRESPONSE._serialized_end=1090
-  _AVAILABLEHOSTSRESPONSE._serialized_start=1092
-  _AVAILABLEHOSTSRESPONSE._serialized_end=1154
+  _HTTPMESSAGE_TYPE._serialized_end=533
+  _PLANNERCONFIG._serialized_start=535
+  _PLANNERCONFIG._serialized_end=613
+  _HOST._serialized_start=615
+  _HOST._serialized_end=715
+  _PINGRESPONSE._serialized_start=717
+  _PINGRESPONSE._serialized_end=779
+  _REGISTERHOSTREQUEST._serialized_start=781
+  _REGISTERHOSTREQUEST._serialized_end=858
+  _REGISTERHOSTRESPONSE._serialized_start=861
+  _REGISTERHOSTRESPONSE._serialized_end=996
+  _REMOVEHOSTREQUEST._serialized_start=998
+  _REMOVEHOSTREQUEST._serialized_end=1054
+  _REMOVEHOSTRESPONSE._serialized_start=1056
+  _REMOVEHOSTRESPONSE._serialized_end=1125
+  _AVAILABLEHOSTSRESPONSE._serialized_start=1127
+  _AVAILABLEHOSTSRESPONSE._serialized_end=1189
 # @@protoc_insertion_point(module_scope)
```

### Comparing `faasmctl-0.8.3/faasmctl/util/invoke.py` & `faasmctl-0.9.0/faasmctl/util/invoke.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/util/k8s.py` & `faasmctl-0.9.0/faasmctl/util/k8s.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/util/network.py` & `faasmctl-0.9.0/faasmctl/util/network.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl/util/planner.py` & `faasmctl-0.9.0/faasmctl/util/planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # ----------
 
 
 def prepare_planner_msg(msg_type, msg_body=None):
     http_message = HttpMessage()
     if msg_type == "RESET":
         http_message.type = HttpMessage.Type.RESET
-    elif msg_type == "FLUSH_HOSTS":
-        http_message.type = HttpMessage.Type.FLUSH_HOSTS
+    elif msg_type == "FLUSH_AVAILABLE_HOSTS":
+        http_message.type = HttpMessage.Type.FLUSH_AVAILABLE_HOSTS
     elif msg_type == "FLUSH_EXECUTORS":
         http_message.type = HttpMessage.Type.FLUSH_EXECUTORS
     elif msg_type == "GET_CONFIG":
         http_message.type = HttpMessage.Type.GET_CONFIG
     elif msg_type == "GET_EXEC_GRAPH":
         http_message.type = HttpMessage.Type.GET_EXEC_GRAPH
     elif msg_type == "EXECUTE_BATCH":
```

### Comparing `faasmctl-0.8.3/faasmctl/util/upload.py` & `faasmctl-0.9.0/faasmctl/util/upload.py`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/faasmctl.egg-info/PKG-INFO` & `faasmctl-0.9.0/faasmctl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faasmctl
-Version: 0.8.3
+Version: 0.9.0
 Summary: Command line tool to deploy, manage, and interact with Faasm
 Author-email: Faasm Team <foo@bar.com>
 Project-URL: Homepage, https://github.com/faasm/faasmctl
 Project-URL: Bug Tracker, https://github.com/faasm/faasmctl/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -17,15 +17,15 @@
 running [Faasm](https://github.com/faasm/faasm) cluster.
 
 ## Install
 
 To install `faasmctl` you need a working `pip` (virtual-)environment. Then:
 
 ```bash
-pip install faasmctl==0.8.3
+pip install faasmctl==0.9.0
 ```
 
 ## Usage
 
 `faasmctl` aggregates tasks related to deploying, managing, and interacting
 with running Faasm clusters. You can list all the available tasks with a
 short description using:
```

### Comparing `faasmctl-0.8.3/faasmctl.egg-info/SOURCES.txt` & `faasmctl-0.9.0/faasmctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faasmctl-0.8.3/pyproject.toml` & `faasmctl-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faasmctl"
-version = "0.8.3"
+version = "0.9.0"
 authors = [
   { name="Faasm Team", email="foo@bar.com" },
 ]
 description = "Command line tool to deploy, manage, and interact with Faasm"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

