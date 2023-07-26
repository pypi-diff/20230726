# Comparing `tmp/testflows.github.runners-1.2.230726.1153543.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1154059.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1153543.tar", last modified: Wed Jul 26 15:35:43 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1154059.tar", last modified: Wed Jul 26 15:40:59 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1153543.tar` & `testflows.github.runners-1.2.230726.1154059.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.474126 testflows.github.runners-1.2.230726.1153543/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1153543/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 15:35:43.474126 testflows.github.runners-1.2.230726.1153543/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    32769 2023-07-26 13:54:40.000000 testflows.github.runners-1.2.230726.1153543/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 15:35:43.474126 testflows.github.runners-1.2.230726.1153543/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.470126 testflows.github.runners-1.2.230726.1153543/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.470126 testflows.github.runners-1.2.230726.1153543/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.470126 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.470126 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    19676 2023-07-26 15:33:47.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8240 2023-07-26 12:06:11.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    10943 2023-07-26 15:32:38.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.474126 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.474126 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4772 2023-07-26 12:06:30.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.470126 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:40:59.239774 testflows.github.runners-1.2.230726.1154059/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1154059/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 15:40:59.239774 testflows.github.runners-1.2.230726.1154059/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    32769 2023-07-26 13:54:40.000000 testflows.github.runners-1.2.230726.1154059/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 15:40:59.239774 testflows.github.runners-1.2.230726.1154059/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 15:40:59.000000 testflows.github.runners-1.2.230726.1154059/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:40:59.239774 testflows.github.runners-1.2.230726.1154059/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:40:59.239774 testflows.github.runners-1.2.230726.1154059/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:40:59.239774 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 15:40:59.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:40:59.239774 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    19676 2023-07-26 15:33:47.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8240 2023-07-26 12:06:11.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10943 2023-07-26 15:32:38.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:40:59.239774 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:40:59.239774 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4770 2023-07-26 15:40:21.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.2.230726.1154059/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:40:59.239774 testflows.github.runners-1.2.230726.1154059/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 15:40:59.000000 testflows.github.runners-1.2.230726.1154059/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 15:40:59.000000 testflows.github.runners-1.2.230726.1154059/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 15:40:59.000000 testflows.github.runners-1.2.230726.1154059/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1154059/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 15:40:59.000000 testflows.github.runners-1.2.230726.1154059/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 15:40:59.000000 testflows.github.runners-1.2.230726.1154059/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1153543/LICENSE` & `testflows.github.runners-1.2.230726.1154059/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/PKG-INFO` & `testflows.github.runners-1.2.230726.1154059/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1153543
+Version: 1.2.230726.1154059
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1153543/README.rst` & `testflows.github.runners-1.2.230726.1154059/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/setup.py` & `testflows.github.runners-1.2.230726.1154059/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1153543",
+    version="1.2.230726.1154059",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/__init__.py`

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
-__version__ = "1.2.230726.1153543"
+__version__ = "1.2.230726.1154059"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/service.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     """Build service install command options not including:
 
     --github-token
     --github-repository
     --hetzner-token
     --ssh-key
     """
-    command = None
+    command = ""
     command += f" --workers {args.workers}"
     command += f" --default-type {args.default_type}"
     command += (
         f" --default-location {args.default_location}" if args.default_location else ""
     )
     command += f" --default-image {args.default_image}"
     command += f" --max-runners {args.max_runners}" if args.max_runners else ""
```

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1154059/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1154059/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1153543
+Version: 1.2.230726.1154059
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1154059/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

