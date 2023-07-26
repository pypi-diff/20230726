# Comparing `tmp/testflows.github.runners-1.2.230726.1214351.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1214947.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1214351.tar", last modified: Wed Jul 26 21:43:51 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1214947.tar", last modified: Wed Jul 26 21:49:47 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1214351.tar` & `testflows.github.runners-1.2.230726.1214947.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.718075 testflows.github.runners-1.2.230726.1214351/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1214351/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 21:43:51.718075 testflows.github.runners-1.2.230726.1214351/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    33100 2023-07-26 21:20:58.000000 testflows.github.runners-1.2.230726.1214351/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 21:43:51.718075 testflows.github.runners-1.2.230726.1214351/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.714075 testflows.github.runners-1.2.230726.1214351/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.714075 testflows.github.runners-1.2.230726.1214351/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.714075 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2780 2023-07-26 21:42:21.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.714075 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    20372 2023-07-26 21:40:30.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8431 2023-07-26 21:41:13.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    10943 2023-07-26 21:25:45.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.718075 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.718075 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-26 20:21:59.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4824 2023-07-26 21:41:44.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1214351/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:43:51.714075 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 21:43:51.000000 testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:49:47.931116 testflows.github.runners-1.2.230726.1214947/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1214947/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 21:49:47.931116 testflows.github.runners-1.2.230726.1214947/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    33100 2023-07-26 21:20:58.000000 testflows.github.runners-1.2.230726.1214947/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 21:49:47.931116 testflows.github.runners-1.2.230726.1214947/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 21:49:47.000000 testflows.github.runners-1.2.230726.1214947/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:49:47.931116 testflows.github.runners-1.2.230726.1214947/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:49:47.931116 testflows.github.runners-1.2.230726.1214947/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:49:47.931116 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 21:49:47.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2780 2023-07-26 21:42:21.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:49:47.931116 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    20372 2023-07-26 21:40:30.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8431 2023-07-26 21:41:13.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10943 2023-07-26 21:25:45.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:49:47.931116 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:49:47.931116 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-26 20:21:59.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4856 2023-07-26 21:48:39.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1214947/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 21:49:47.931116 testflows.github.runners-1.2.230726.1214947/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33692 2023-07-26 21:49:47.000000 testflows.github.runners-1.2.230726.1214947/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 21:49:47.000000 testflows.github.runners-1.2.230726.1214947/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 21:49:47.000000 testflows.github.runners-1.2.230726.1214947/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1214947/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 21:49:47.000000 testflows.github.runners-1.2.230726.1214947/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 21:49:47.000000 testflows.github.runners-1.2.230726.1214947/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1214351/LICENSE` & `testflows.github.runners-1.2.230726.1214947/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/PKG-INFO` & `testflows.github.runners-1.2.230726.1214947/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1214351
+Version: 1.2.230726.1214947
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1214351/README.rst` & `testflows.github.runners-1.2.230726.1214947/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/setup.py` & `testflows.github.runners-1.2.230726.1214947/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1214351",
+    version="1.2.230726.1214947",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230726.1214351"
+__version__ = "1.2.230726.1214947"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     """
     command = ""
     command += f" --workers {args.workers}"
     command += f" --default-type {args.default_type.name}"
     command += (
         f" --default-location {args.default_location.name}"
         if args.default_location
-        else None
+        else ""
     )
-    command += f" --default-image {args.default_image.type}:{args.default_image.name}"
+    command += f" --default-image {args.default_image.type}:{args.default_image.name or args.default_image.description}"
     command += f" --max-runners {args.max_runners}" if args.max_runners else ""
     command += f" --logger-config {args.logger_config}" if args.logger_config else ""
     command += f" --setup-script {args.setup_script}" if args.setup_script else ""
     command += (
         f" --startup-x64-script {args.startup_x64_script}"
         if args.startup_x64_script
         else ""
```

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1214947/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1214947/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1214351
+Version: 1.2.230726.1214947
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1214351/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1214947/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

