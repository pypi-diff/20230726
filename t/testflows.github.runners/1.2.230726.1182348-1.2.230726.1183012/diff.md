# Comparing `tmp/testflows.github.runners-1.2.230726.1182348.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1183012.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1182348.tar", last modified: Wed Jul 26 18:23:48 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1183012.tar", last modified: Wed Jul 26 18:30:12 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1182348.tar` & `testflows.github.runners-1.2.230726.1183012.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.358374 testflows.github.runners-1.2.230726.1182348/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1182348/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 18:23:48.358374 testflows.github.runners-1.2.230726.1182348/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    32718 2023-07-26 18:23:14.000000 testflows.github.runners-1.2.230726.1182348/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 18:23:48.358374 testflows.github.runners-1.2.230726.1182348/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.354374 testflows.github.runners-1.2.230726.1182348/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.354374 testflows.github.runners-1.2.230726.1182348/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.354374 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.354374 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    19676 2023-07-26 15:33:47.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8131 2023-07-26 16:23:24.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    11025 2023-07-26 18:20:22.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.358374 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.358374 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4770 2023-07-26 15:40:21.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.354374 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1183012/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    32718 2023-07-26 18:23:14.000000 testflows.github.runners-1.2.230726.1183012/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.299094 testflows.github.runners-1.2.230726.1183012/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.299094 testflows.github.runners-1.2.230726.1183012/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    19676 2023-07-26 15:33:47.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8131 2023-07-26 16:23:24.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10837 2023-07-26 18:29:40.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4770 2023-07-26 15:40:21.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1182348/LICENSE` & `testflows.github.runners-1.2.230726.1183012/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/PKG-INFO` & `testflows.github.runners-1.2.230726.1183012/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1182348
+Version: 1.2.230726.1183012
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1182348/README.rst` & `testflows.github.runners-1.2.230726.1183012/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/setup.py` & `testflows.github.runners-1.2.230726.1183012/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1182348",
+    version="1.2.230726.1183012",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.2.230726.1182348"
+__version__ = "1.2.230726.1183012"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scale_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,17 +284,13 @@
                                         github_repository=github_repository,
                                         ssh_key=ssh_key,
                                     )
                                 )
 
             for future in futures:
                 with Action("Waiting to finish creating server", ignore_fail=True):
-                    try:
-                        future.result()
-                    except APIException as exc:
-                        with Action(f"Sleeping as we have: {exc}"):
-                            time.sleep(60)
+                    future.result()
 
             with Action(
                 f"Sleeping until next interval {interval}s", level=logging.DEBUG
             ):
                 time.sleep(interval)
```

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1182348
+Version: 1.2.230726.1183012
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

