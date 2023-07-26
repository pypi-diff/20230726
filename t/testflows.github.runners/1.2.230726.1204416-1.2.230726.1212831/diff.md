# Comparing `tmp/testflows.github.runners-1.2.230726.1204416.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1212831.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1204416.tar", last modified: Wed Jul 26 20:44:17 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1212831.tar", last modified: Wed Jul 26 21:28:31 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1204416.tar` & `testflows.github.runners-1.2.230726.1212831.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1204416/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33617 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    33025 2023-07-26 20:43:15.000000 testflows.github.runners-1.2.230726.1204416/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 20:44:16.000000 testflows.github.runners-1.2.230726.1204416/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 20:44:16.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2030 2023-07-26 20:24:26.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    19878 2023-07-26 20:43:36.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8087 2023-07-26 20:32:03.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    10823 2023-07-26 20:14:36.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-26 20:21:59.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4829 2023-07-26 20:28:21.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33617 2023-07-26 20:44:17.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 20:44:17.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 20:44:17.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 20:44:17.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 20:44:17.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1212831/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    33100 2023-07-26 21:20:58.000000 testflows.github.runners-1.2.230726.1212831/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2780 2023-07-26 21:25:45.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    20330 2023-07-26 21:20:21.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8355 2023-07-26 21:08:50.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10943 2023-07-26 21:25:45.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-26 20:21:59.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4829 2023-07-26 20:28:21.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1204416/LICENSE` & `testflows.github.runners-1.2.230726.1212831/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/PKG-INFO` & `testflows.github.runners-1.2.230726.1212831/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1204416
+Version: 1.2.230726.1212831
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -844,16 +844,16 @@
 
 * **--default-type name**
   default runner server type name, default: *cx11*
 
 * **--default-location name**
   default runner server location name, default: not specified
 
-* **--default-image type:name**
-  default runner server image type and name,
+* **--default-image type:name_or_description**
+  default runner server image type and name or description,
   where type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
@@ -907,16 +907,16 @@
 
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
-        * **-i type:name, --image type:name**
-          deployment server image type and name,
+        * **-i type:name_or_description, --image type:name_or_description**
+          deployment server image type and name or description,
           where the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
```

### Comparing `testflows.github.runners-1.2.230726.1204416/README.rst` & `testflows.github.runners-1.2.230726.1212831/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -827,16 +827,16 @@
 
 * **--default-type name**
   default runner server type name, default: *cx11*
 
 * **--default-location name**
   default runner server location name, default: not specified
 
-* **--default-image type:name**
-  default runner server image type and name,
+* **--default-image type:name_or_description**
+  default runner server image type and name or description,
   where type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
@@ -890,16 +890,16 @@
 
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
-        * **-i type:name, --image type:name**
-          deployment server image type and name,
+        * **-i type:name_or_description, --image type:name_or_description**
+          deployment server image type and name or description,
           where the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
```

### Comparing `testflows.github.runners-1.2.230726.1204416/setup.py` & `testflows.github.runners-1.2.230726.1212831/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1204416",
+    version="1.2.230726.1212831",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230726.1204416"
+__version__ = "1.2.230726.1212831"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/bin/github-runners`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from testflows.github.runners.scripts import Scripts, scripts
 
 import testflows.github.runners.args as args
 import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
 
 check_args = args.check
+check_image = args.check_image
 
 logger = logging.getLogger("testflows.github.runners")
 
 description = """Auto-scaling GitHub Actions runners service using Hetzner Cloud.
 
     Service that starts and monitors queued up GitHub Actions workflows.
     When a new job is queued up, it creates new Hetzner Cloud server instance
@@ -111,18 +112,18 @@
         metavar="count",
         type=args.count_type,
         help="maximum number of active runners, default: unlimited",
     )
 
     parser.add_argument(
         "--default-image",
-        metavar="type:name",
+        metavar="type:name_or_description",
         type=args.image_type,
         help=(
-            "default runner server image type and name,"
+            "default runner server image type and name or description,"
             "where the type is either: 'system','snapshot','backup','app',\n"
             "default: system:ubuntu-22.04"
         ),
         default="system:ubuntu-22.04",
     )
 
     parser.add_argument(
@@ -282,18 +283,18 @@
         help="deployment server type, default: cpx11",
         default="cpx11",
     )
 
     deploy_cloud_parser.add_argument(
         "-i",
         "--image",
-        metavar="type:name",
+        metavar="type:name_or_description",
         type=args.image_type,
         help=(
-            "deployment server image type and name,\n"
+            "deployment server image type and name or description,\n"
             "where the type is either: 'system','snapshot','backup','app',\n"
             "default: system:ubuntu-22.04"
         ),
         default="system:ubuntu-22.04",
     )
 
     deploy_cloud_parser.set_defaults(func=cloud.deploy)
@@ -511,14 +512,17 @@
 
         with Action("Logging in to GitHub"):
             github = Github(login_or_token=args.github_token)
 
         with Action(f"Getting repository {args.github_repository}"):
             repo: Repository = github.get_repo(args.github_repository)
 
+        with Action("Checking if default image exists"):
+            args.default_image = check_image(client=client, image=args.default_image)
+
         with Action(f"Checking if SSH key exists"):
             public_key = args.ssh_key.read()
             key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
             ssh_key = SSHKey(name=key_name, public_key=public_key)
 
             if not client.ssh_keys.get_by_name(name=ssh_key.name):
                 with Action(f"Creating SSH key {ssh_key.name}"):
@@ -583,14 +587,21 @@
     except KeyboardInterrupt as exc:
         msg = "❗ KeyboardInterrupt"
         if args.debug:
             logger.exception(f"{msg}\n{exc}")
         else:
             logger.error(msg)
         sys.exit(1)
+    except Exception as exc:
+        msg = f"❗ Error: {type(exc).__name__} {exc}"
+        if args.debug:
+            logger.exception(f"{msg}\n{exc}")
+        else:
+            logger.error(msg)
+        sys.exit(1)
 
 
 if __name__ == "__main__":
     args = argparser().parse_args()
 
     logging_level = logging.INFO
```

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/cloud.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.server_types.domain import ServerType
 from hcloud.servers.client import BoundServer
 from hcloud.images.domain import Image
 from hcloud.locations.domain import Location
 
 from .actions import Action
-from .args import check
+from .args import check, check_image
 from . import __version__
 
 from .server import wait_ready, wait_ssh, ssh
 from .service import command_options
 
 current_dir = os.path.dirname(__file__)
 
@@ -46,14 +46,20 @@
         with Action(
             f"Checking if server {server_name} already exists", ignore_fail=True
         ):
             server: BoundServer = client.servers.get_by_name(server_name)
             with Action(f"Deleting server {server_name}"):
                 server.delete()
 
+    with Action("Checking if default image exists"):
+        args.default_image = check_image(client=client, image=args.default_image)
+
+    with Action("Checking if server image exists"):
+        args.image = check_image(client=client, image=args.image)
+
     with Action(f"Checking if SSH key exists"):
         public_key = args.ssh_key.read()
         key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
         ssh_key = SSHKey(name=key_name, public_key=public_key)
 
         if not client.ssh_keys.get_by_name(name=ssh_key.name):
             with Action(f"Creating SSH key {ssh_key.name}"):
```

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scale_up.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import time
 import logging
 import threading
 
 from .actions import Action
 from .scripts import Scripts
 from .request import request
+from .args import image_type, check_image
 
 from .server import wait_ssh, ssh, wait_ready
 
 from hcloud import Client, APIException
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.server_types.domain import ServerType
 from hcloud.locations.domain import Location
@@ -155,23 +156,27 @@
 
     if server_location is None and default:
         server_location = default
 
     return server_location
 
 
-def get_server_image(job: WorkflowJob, default: Image, label_prefix="image-"):
+def get_server_image(
+    client: Client, job: WorkflowJob, default: Image, label_prefix="image-"
+):
     """Get preferred server image for the specified job."""
     server_image: Image = None
 
     if server_image is None:
         for label in job.raw_data["labels"]:
             if label.startswith(label_prefix):
-                server_image_name = label.split(label_prefix, 1)[-1].lower()
-                server_image = Image(name=server_image_name)
+                server_image = check_image(
+                    client,
+                    image_type(label.split(label_prefix, 1)[-1].lower(), separator="-"),
+                )
 
     if server_image is None:
         server_image = default
 
     return server_image
 
 
@@ -237,15 +242,15 @@
                                 server_type = get_server_type(
                                     job=job, default=default_type
                                 )
                                 server_location = get_server_location(
                                     job=job, default=default_location
                                 )
                                 server_image = get_server_image(
-                                    job=job, default=default_image
+                                    client=client, job=job, default=default_image
                                 )
                                 startup_script = get_startup_script(
                                     server_type=server_type, scripts=scripts
                                 )
 
                                 if max_servers is not None:
                                     with Action(
```

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1204416
+Version: 1.2.230726.1212831
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -844,16 +844,16 @@
 
 * **--default-type name**
   default runner server type name, default: *cx11*
 
 * **--default-location name**
   default runner server location name, default: not specified
 
-* **--default-image type:name**
-  default runner server image type and name,
+* **--default-image type:name_or_description**
+  default runner server image type and name or description,
   where type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
@@ -907,16 +907,16 @@
 
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
-        * **-i type:name, --image type:name**
-          deployment server image type and name,
+        * **-i type:name_or_description, --image type:name_or_description**
+          deployment server image type and name or description,
           where the type is either: 'system','snapshot','backup','app',
           default: *system:ubuntu-22.04*
 
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
```

### Comparing `testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

