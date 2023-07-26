# Comparing `tmp/testflows.github.runners-1.2.230726.1212831.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1214351.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1212831.tar", last modified: Wed Jul 26 21:28:31 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1214351.tar", last modified: Wed Jul 26 21:43:51 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1212831.tar` & `testflows.github.runners-1.2.230726.1214351.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1212831/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    33100 2023-07-26 21:20:58.000000 testflows.github.runners-1.2.230726.1212831/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2780 2023-07-26 21:25:45.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    20330 2023-07-26 21:20:21.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8355 2023-07-26 21:08:50.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    10943 2023-07-26 21:25:45.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-26 20:21:59.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4829 2023-07-26 20:28:21.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1212831/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:28:31.245178 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 21:28:31.000000 testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.718075 testflows.github.runners-1.2.230726.1214351/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1214351/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 21:43:51.718075 testflows.github.runners-1.2.230726.1214351/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    33100 2023-07-26 21:20:58.000000 testflows.github.runners-1.2.230726.1214351/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 21:43:51.718075 testflows.github.runners-1.2.230726.1214351/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.714075 testflows.github.runners-1.2.230726.1214351/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.714075 testflows.github.runners-1.2.230726.1214351/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.714075 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2780 2023-07-26 21:42:21.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.714075 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    20372 2023-07-26 21:40:30.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8431 2023-07-26 21:41:13.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10943 2023-07-26 21:25:45.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.718075 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.718075 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-26 20:21:59.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4824 2023-07-26 21:41:44.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.714075 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1212831/LICENSE` & `testflows.github.runners-1.2.230726.1214351/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/PKG-INFO` & `testflows.github.runners-1.2.230726.1214351/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1212831
+Version: 1.2.230726.1214351
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1212831/README.rst` & `testflows.github.runners-1.2.230726.1214351/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/setup.py` & `testflows.github.runners-1.2.230726.1214351/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1212831",
+    version="1.2.230726.1214351",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230726.1212831"
+__version__ = "1.2.230726.1214351"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/bin/github-runners`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 
 from github import Github
 from github.Repository import Repository
 
-from argparse import ArgumentParser, RawTextHelpFormatter, FileType
+from argparse import ArgumentParser, RawTextHelpFormatter
 
 from testflows.github.runners import __version__, __license__
 from testflows.github.runners.actions import Action
 from testflows.github.runners.scale_up import scale_up
 from testflows.github.runners.scale_down import scale_down
 from testflows.github.runners.scripts import Scripts, scripts
 
@@ -97,15 +97,15 @@
         help="Hetzner Cloud token, default: $HETZNER_TOKEN environment variable",
         default="",
     )
 
     parser.add_argument(
         "--ssh-key",
         metavar="path",
-        type=FileType("r", encoding="utf-8"),
+        type=str,
         help="path to public SSH key, default: ~/.ssh/id_rsa.pub",
         default=os.path.expanduser("~/.ssh/id_rsa.pub"),
     )
 
     parser.add_argument(
         "-m",
         "--max-runners",
@@ -516,15 +516,16 @@
         with Action(f"Getting repository {args.github_repository}"):
             repo: Repository = github.get_repo(args.github_repository)
 
         with Action("Checking if default image exists"):
             args.default_image = check_image(client=client, image=args.default_image)
 
         with Action(f"Checking if SSH key exists"):
-            public_key = args.ssh_key.read()
+            with open(args.ssh_key, "r", encoding="utf-8") as ssh_key_file:
+                public_key = ssh_key_file.read()
             key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
             ssh_key = SSHKey(name=key_name, public_key=public_key)
 
             if not client.ssh_keys.get_by_name(name=ssh_key.name):
                 with Action(f"Creating SSH key {ssh_key.name}"):
                     client.ssh_keys.create(
                         name=ssh_key.name, public_key=ssh_key.public_key
```

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
     with Action("Checking if default image exists"):
         args.default_image = check_image(client=client, image=args.default_image)
 
     with Action("Checking if server image exists"):
         args.image = check_image(client=client, image=args.image)
 
     with Action(f"Checking if SSH key exists"):
-        public_key = args.ssh_key.read()
+        with open(args.ssh_key, "r", encoding="utf-8") as ssh_key_file:
+            public_key = ssh_key_file.read()
         key_name = hashlib.md5(public_key.encode("utf-8")).hexdigest()
         ssh_key = SSHKey(name=key_name, public_key=public_key)
 
         if not client.ssh_keys.get_by_name(name=ssh_key.name):
             with Action(f"Creating SSH key {ssh_key.name}"):
                 client.ssh_keys.create(name=ssh_key.name, public_key=ssh_key.public_key)
```

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             "Restart=always\n"
             f"Environment=GITHUB_TOKEN={args.github_token}\n"
             f"Environment=GITHUB_REPOSITORY={args.github_repository}\n"
             f"Environment=HETZNER_TOKEN={args.hetzner_token}\n"
             f"ExecStart={binary}"
             f" --workers {args.workers}"
         )
-        contents += f" --ssh-key {args.ssh_key.name}"
+        contents += f" --ssh-key {args.ssh_key}"
         contents += command_options(args)
         contents += "\n" "[Install]\n" "WantedBy=multi-user.target\n"
 
         os.system(f"sudo bash -c \"cat > {SERVICE}\" <<'EOF'\n{contents}\nEOF")
         os.system(f"sudo chmod 700 {SERVICE}")
 
     with Action("Reloading systemd"):
```

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1212831
+Version: 1.2.230726.1214351
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1212831/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

