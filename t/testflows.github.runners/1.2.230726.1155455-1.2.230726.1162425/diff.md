# Comparing `tmp/testflows.github.runners-1.2.230726.1155455.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1162425.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1155455.tar", last modified: Wed Jul 26 15:54:56 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1162425.tar", last modified: Wed Jul 26 16:24:25 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1155455.tar` & `testflows.github.runners-1.2.230726.1162425.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:54:56.025427 testflows.github.runners-1.2.230726.1155455/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1155455/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 15:54:56.025427 testflows.github.runners-1.2.230726.1155455/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    32769 2023-07-26 13:54:40.000000 testflows.github.runners-1.2.230726.1155455/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 15:54:56.025427 testflows.github.runners-1.2.230726.1155455/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 15:54:55.000000 testflows.github.runners-1.2.230726.1155455/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:54:56.021427 testflows.github.runners-1.2.230726.1155455/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:54:56.021427 testflows.github.runners-1.2.230726.1155455/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:54:56.025427 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 15:54:55.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:54:56.025427 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    19676 2023-07-26 15:33:47.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8136 2023-07-26 15:53:04.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    10944 2023-07-26 15:44:57.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:54:56.025427 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:54:56.025427 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4770 2023-07-26 15:40:21.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1155455/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:54:56.021427 testflows.github.runners-1.2.230726.1155455/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 15:54:55.000000 testflows.github.runners-1.2.230726.1155455/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 15:54:56.000000 testflows.github.runners-1.2.230726.1155455/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 15:54:55.000000 testflows.github.runners-1.2.230726.1155455/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1155455/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 15:54:55.000000 testflows.github.runners-1.2.230726.1155455/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 15:54:55.000000 testflows.github.runners-1.2.230726.1155455/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1162425/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    32769 2023-07-26 13:54:40.000000 testflows.github.runners-1.2.230726.1162425/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.397697 testflows.github.runners-1.2.230726.1162425/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.397697 testflows.github.runners-1.2.230726.1162425/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    19676 2023-07-26 15:33:47.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8131 2023-07-26 16:23:24.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10944 2023-07-26 15:44:57.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4770 2023-07-26 15:40:21.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1155455/LICENSE` & `testflows.github.runners-1.2.230726.1162425/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/PKG-INFO` & `testflows.github.runners-1.2.230726.1162425/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1155455
+Version: 1.2.230726.1162425
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1155455/README.rst` & `testflows.github.runners-1.2.230726.1162425/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/setup.py` & `testflows.github.runners-1.2.230726.1162425/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1155455",
+    version="1.2.230726.1162425",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230726.1155455"
+__version__ = "1.2.230726.1162425"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/cloud.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         check(args)
 
         server_name = args.server_name
 
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=args.hetzner_token)
 
-        with Action(f"Checking if server {server_name} already exists"):
+        with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Installing service"):
         command = f"\"su - runner -c '"
         command += f"GITHUB_TOKEN={args.github_token} "
         command += f"GITHUB_REPOSITORY={args.github_repository} "
         command += f"HETZNER_TOKEN={args.hetzner_token} "
@@ -120,15 +120,15 @@
     """Upgrade github-runners application on a cloud instance."""
     server_name = args.server_name
     upgrade_version = args.upgrade_version
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=args.hetzner_token)
 
-    with Action(f"Checking if server {server_name} already exists"):
+    with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
 
     stop(args, server=server)
 
     if upgrade_version:
         with Action(f"Upgrading github-runners to version {upgrade_version}"):
             ssh(
@@ -148,15 +148,15 @@
 def uninstall(args):
     """Uninstall github-runners service from a cloud instance."""
     server_name = args.server_name
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=args.hetzner_token)
 
-    with Action(f"Checking if server {server_name} already exists"):
+    with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Uninstalling service"):
         command = f"\"su - runner -c 'github-runners service uninstall'\""
         ssh(server, command)
 
 
@@ -165,15 +165,15 @@
     on Hetzner server instance by stopping the service
     and deleting the server."""
     server_name = args.server_name
 
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=args.hetzner_token)
 
-    with Action(f"Checking if server {server_name} already exists"):
+    with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Uninstalling service"):
         command = f"\"su - runner -c 'github-runners service uninstall'\""
         ssh(server, command)
 
     with Action(f"Deleting server {server_name}"):
@@ -181,16 +181,19 @@
 
 
 def logs(args, server: BoundServer = None):
     """Get cloud server service logs."""
     if server is None:
         server_name = args.server_name
 
-        client = Client(token=args.hetzner_token)
-        server = client.servers.get_by_name(server_name)
+        with Action("Logging in to Hetzner Cloud"):
+            client = Client(token=args.hetzner_token)
+
+        with Action(f"Getting server {server_name}"):
+            server: BoundServer = client.servers.get_by_name(server_name)
 
     if server is None:
         raise ValueError("server not found")
 
     command = (
         f"\"su - runner -c 'github-runners service logs"
         + (" -f" if args.follow else "")
@@ -203,15 +206,15 @@
     """Get cloud server service status."""
     if server is None:
         server_name = args.server_name
 
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=args.hetzner_token)
 
-        with Action(f"Checking if server {server_name} already exists"):
+        with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Getting status"):
         command = f"\"su - runner -c 'github-runners service status'\""
         ssh(server, command)
 
 
@@ -219,15 +222,15 @@
     """Start cloud server service."""
     if server is None:
         server_name = args.server_name
 
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=args.hetzner_token)
 
-        with Action(f"Checking if server {server_name} already exists"):
+        with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Starting service"):
         command = f"\"su - runner -c 'github-runners service start'\""
         ssh(server, command)
 
 
@@ -235,13 +238,13 @@
     """Stop cloud server service."""
     if server is None:
         server_name = args.server_name
 
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=args.hetzner_token)
 
-        with Action(f"Checking if server {server_name} already exists"):
+        with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Stopping service"):
         command = f"\"su - runner -c 'github-runners service stop'\""
         ssh(server, command)
```

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1155455
+Version: 1.2.230726.1162425
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1155455/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

