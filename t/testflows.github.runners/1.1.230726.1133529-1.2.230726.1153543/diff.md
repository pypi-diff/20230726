# Comparing `tmp/testflows.github.runners-1.1.230726.1133529.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1153543.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.1.230726.1133529.tar", last modified: Wed Jul 26 13:35:29 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1153543.tar", last modified: Wed Jul 26 15:35:43 2023, max compression
```

## Comparing `testflows.github.runners-1.1.230726.1133529.tar` & `testflows.github.runners-1.2.230726.1153543.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.295917 testflows.github.runners-1.1.230726.1133529/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230726.1133529/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    32758 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    32166 2023-07-26 13:34:52.000000 testflows.github.runners-1.1.230726.1133529/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 13:35:29.295917 testflows.github.runners-1.1.230726.1133529/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    19651 2023-07-26 11:57:13.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8240 2023-07-26 12:06:11.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    10060 2023-07-26 12:08:03.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4772 2023-07-26 12:06:30.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    32758 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.474126 testflows.github.runners-1.2.230726.1153543/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1153543/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 15:35:43.474126 testflows.github.runners-1.2.230726.1153543/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    32769 2023-07-26 13:54:40.000000 testflows.github.runners-1.2.230726.1153543/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 15:35:43.474126 testflows.github.runners-1.2.230726.1153543/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.470126 testflows.github.runners-1.2.230726.1153543/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.470126 testflows.github.runners-1.2.230726.1153543/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.470126 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.470126 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    19676 2023-07-26 15:33:47.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8240 2023-07-26 12:06:11.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10943 2023-07-26 15:32:38.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.474126 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.474126 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4772 2023-07-26 12:06:30.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.2.230726.1153543/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 15:35:43.470126 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 15:35:43.000000 testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.1.230726.1133529/LICENSE` & `testflows.github.runners-1.2.230726.1153543/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/PKG-INFO` & `testflows.github.runners-1.2.230726.1153543/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230726.1133529
+Version: 1.2.230726.1153543
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -443,14 +443,37 @@
 :location:
    *ash*
 :type:
    *cpx11*
 :image:
    *ubuntu-22.04*
 
+The **cloud deploy** command uses the following setup script.
+
+:setup script:
+   .. code-block:: bash
+
+      set -x
+      
+      apt-get update
+      
+      apt-get -y install python3-pip
+      apt-get -y install openssh-client
+      
+      echo "Create and configure runner user"
+      
+      adduser runner --disabled-password --gecos ""
+      echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
+      addgroup wheel
+      usermod -aG wheel runner
+      usermod -aG sudo runner
+      
+      echo "Generate SSH Key"
+      sudo -u runner ssh-keygen -t rsa -q -f "/home/runner/.ssh/id_rsa" -N ""
+
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
 The cloud instance that runs the **github-runners** service can either be x64 or ARM64 instance. By default, **cpx11**
```

### Comparing `testflows.github.runners-1.1.230726.1133529/README.rst` & `testflows.github.runners-1.2.230726.1153543/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -426,14 +426,37 @@
 :location:
    *ash*
 :type:
    *cpx11*
 :image:
    *ubuntu-22.04*
 
+The **cloud deploy** command uses the following setup script.
+
+:setup script:
+   .. code-block:: bash
+
+      set -x
+      
+      apt-get update
+      
+      apt-get -y install python3-pip
+      apt-get -y install openssh-client
+      
+      echo "Create and configure runner user"
+      
+      adduser runner --disabled-password --gecos ""
+      echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
+      addgroup wheel
+      usermod -aG wheel runner
+      usermod -aG sudo runner
+      
+      echo "Generate SSH Key"
+      sudo -u runner ssh-keygen -t rsa -q -f "/home/runner/.ssh/id_rsa" -N ""
+
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
 The cloud instance that runs the **github-runners** service can either be x64 or ARM64 instance. By default, **cpx11**
```

### Comparing `testflows.github.runners-1.1.230726.1133529/setup.py` & `testflows.github.runners-1.2.230726.1153543/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.1.230726.1133529",
+    version="1.2.230726.1153543",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/__init__.py`

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
-__version__ = "1.1.230726.1133529"
+__version__ = "1.2.230726.1153543"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/bin/github-runners`

 * *Files 0% similar despite different names*

```diff
@@ -611,15 +611,15 @@
 
     if args.logger_config:
         logging.config.fileConfig(args.logger_config)
     else:
         logger.setLevel(logging_level)
         handler = logging.StreamHandler(sys.stdout)
         formatter = logging.Formatter(
-            "%(asctime)s %(levelname)8s %(threadName)10s %(funcName)15s %(message)s",
+            "%(asctime)s %(levelname)8s %(threadName)16s %(funcName)15s %(message)s",
             datefmt="%m/%d/%Y %I:%M:%S %p",
         )
         handler.setFormatter(formatter)
         logger.addHandler(handler)
 
     if args.setup_script:
         scripts.setup = args.setup_script
@@ -643,8 +643,8 @@
 
     else:
         check(args)
 
         with ThreadPoolExecutor(
             max_workers=args.workers + 2, thread_name_prefix="worker"
         ) as worker_pool:
-            main(args, scripts, worker_pool)
+            main(args=args, scripts=scripts, worker_pool=worker_pool)
```

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/request.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,27 +11,52 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import json as json
 
 from http.client import HTTPResponse
-from urllib.request import urlopen, Request
+from urllib.request import urlopen, Request, HTTPError
 
 
-def request(url, headers=None, data=None, format=None, encoding="utf-8", timeout=60):
+def request(
+    url,
+    headers=None,
+    data=None,
+    format=None,
+    encoding="utf-8",
+    timeout=60,
+    process_error=True,
+):
     """Perform URL request."""
     if headers is None:
         headers = {}
 
-    request = Request(url, headers=headers, data=data)
+    r = Request(url, headers=headers, data=data)
 
-    with urlopen(request, timeout=timeout) as response:
-        response: HTTPResponse = response
-
-        data = response.read()
-        if encoding:
-            data = data.decode(encoding)
-        if format == "json":
-            data = json.loads(data)
-
-        return data, response
+    try:
+        with urlopen(r, timeout=timeout) as response:
+            response: HTTPResponse = response
+
+            data = response.read()
+            if encoding:
+                data = data.decode(encoding)
+            if format == "json":
+                data = json.loads(data)
+
+            return data, response
+    except HTTPError as exc:
+        if not process_error:
+            raise
+
+        if exc.getcode() in (307, 308):
+            # process 307 (Temporary Redirect") and 308 (Permanent Redirect)
+            error_data = json.loads(exc.read().decode(encoding))
+            return request(
+                url=error_data["url"],
+                headers=headers,
+                data=data,
+                format=format,
+                encoding=encoding,
+                timeout=timeout,
+                process_error=False,
+            )
```

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scale_up.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from .actions import Action
 from .scripts import Scripts
 from .request import request
 
 from .server import wait_ssh, ssh, wait_ready
 
-from hcloud import Client
+from hcloud import Client, APIException
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.server_types.domain import ServerType
 from hcloud.locations.domain import Location
 from hcloud.servers.client import BoundServer
 from hcloud.images.domain import Image
 
 from github.Repository import Repository
@@ -79,26 +79,26 @@
             f"GITHUB_RUNNER_GROUP=Default "
             f'GITHUB_RUNNER_LABELS="{runner_labels}" '
             f"bash -s' < {startup_script}",
         )
 
 
 def create_server(
+    setup_worker_pool: ThreadPoolExecutor,
     client: Client,
     job: WorkflowJob,
     name: str,
     server_type: ServerType,
     server_location: Location,
     server_image: Image,
     setup_script: str,
     startup_script: str,
     github_token: str,
     github_repository: str,
     ssh_key: SSHKey,
-    count=1,
     timeout=60,
 ):
     """Create specified number of server instances."""
 
     with Action("Create server"):
         response = client.servers.create(
             name=name,
@@ -108,15 +108,16 @@
             ssh_keys=[ssh_key],
         )
         server: BoundServer = response.server
 
     with Action(f"Waiting for server {server.name} to be ready") as action:
         wait_ready(server=server, timeout=timeout, action=action)
 
-    server_setup(
+    setup_worker_pool.submit(
+        server_setup,
         server=response.server,
         setup_script=setup_script,
         startup_script=startup_script,
         github_token=github_token,
         github_repository=github_repository,
         runner_labels=",".join(job.raw_data["labels"]),
     )
@@ -198,85 +199,100 @@
     default_type: str,
     default_location: str,
     default_image: str,
     interval: int,
     max_servers: int,
 ):
     """Scale up service."""
-    while True:
-        if terminate.is_set():
-            with Action("Terminating scale up service"):
-                break
-
-        with Action("Getting list of servers", level=logging.DEBUG):
-            servers: list[BoundServer] = client.servers.get_all()
-            servers = [
-                server
-                for server in servers
-                if server.name.startswith(runner_server_prefix)
-            ]
-
-        with Action("Getting workflow runs", level=logging.DEBUG):
-            workflow_runs = repo.get_workflow_runs(branch="main", status="queued")
-
-        futures: list[Future] = []
-
-        with Action("Looking for queued jobs", level=logging.DEBUG) as action:
-            for run in workflow_runs:
-                for job in run.jobs():
-                    if job.status == "queued":
-                        with Action(f"Found queued job {job}"):
-                            server_name = f"{runner_server_prefix}{job.run_id}"
-                            server_type = get_server_type(job=job, default=default_type)
-                            server_location = get_server_location(
-                                job=job, default=default_location
-                            )
-                            server_image = get_server_image(
-                                job=job, default=default_image
-                            )
-                            startup_script = get_startup_script(
-                                server_type=server_type, scripts=scripts
-                            )
 
-                            if max_servers is not None:
+    with ThreadPoolExecutor(
+        max_workers=worker_pool._max_workers, thread_name_prefix=f"setup-worker"
+    ) as setup_worker_pool:
+
+        while True:
+            if terminate.is_set():
+                with Action("Terminating scale up service"):
+                    break
+
+            with Action("Getting list of servers", level=logging.DEBUG):
+                servers: list[BoundServer] = client.servers.get_all()
+                servers = [
+                    server
+                    for server in servers
+                    if server.name.startswith(runner_server_prefix)
+                ]
+
+            with Action("Getting workflow runs", level=logging.DEBUG):
+                workflow_runs = repo.get_workflow_runs(branch="main", status="queued")
+
+            futures: list[Future] = []
+
+            with Action("Looking for queued jobs", level=logging.DEBUG) as action:
+                for run in workflow_runs:
+                    for job in run.jobs():
+                        if job.status == "queued":
+                            with Action(f"Found queued job {job}"):
+                                server_name = f"{runner_server_prefix}{job.run_id}"
+                                server_type = get_server_type(
+                                    job=job, default=default_type
+                                )
+                                server_location = get_server_location(
+                                    job=job, default=default_location
+                                )
+                                server_image = get_server_image(
+                                    job=job, default=default_image
+                                )
+                                startup_script = get_startup_script(
+                                    server_type=server_type, scripts=scripts
+                                )
+
+                                if max_servers is not None:
+                                    with Action(
+                                        f"Checking if maximum number of servers has been reached",
+                                        level=logging.DEBUG,
+                                    ):
+                                        if len(servers) >= max_servers:
+                                            with Action(
+                                                f"Maximum number of servers {max_servers} has been reached"
+                                            ):
+                                                continue
+
                                 with Action(
-                                    f"Checking if maximum number of servers has been reached",
+                                    f"Checking if server already exists for {job}",
                                     level=logging.DEBUG,
-                                ):
-                                    if len(servers) >= max_servers:
-                                        with Action(
-                                            f"Maximum number of servers {max_servers} has been reached"
-                                        ):
+                                ) as action:
+                                    if server_name in [
+                                        server.name for server in servers
+                                    ]:
+                                        with Action(f"Server already exists for {job}"):
                                             continue
 
-                            with Action(
-                                f"Checking if server already exists for {job}",
-                                level=logging.DEBUG,
-                            ) as action:
-                                if server_name in [server.name for server in servers]:
-                                    with Action(f"Server already exists for {job}"):
-                                        continue
-
-                            futures.append(
-                                worker_pool.submit(
-                                    create_server,
-                                    client=client,
-                                    job=job,
-                                    name=server_name,
-                                    server_type=server_type,
-                                    server_location=server_location,
-                                    server_image=server_image,
-                                    setup_script=scripts.setup,
-                                    startup_script=startup_script,
-                                    github_token=github_token,
-                                    github_repository=github_repository,
-                                    ssh_key=ssh_key,
-                                    image=image,
+                                futures.append(
+                                    worker_pool.submit(
+                                        create_server,
+                                        setup_worker_pool=setup_worker_pool,
+                                        client=client,
+                                        job=job,
+                                        name=server_name,
+                                        server_type=server_type,
+                                        server_location=server_location,
+                                        server_image=server_image,
+                                        setup_script=scripts.setup,
+                                        startup_script=startup_script,
+                                        github_token=github_token,
+                                        github_repository=github_repository,
+                                        ssh_key=ssh_key,
+                                    )
                                 )
-                            )
-
-        for future in futures:
-            with Action("Waiting to finish creating server", ignore_fail=True):
-                future.result()
 
-        with Action(f"Sleeping until next interval {interval}s", level=logging.DEBUG):
-            time.sleep(interval)
+            for future in futures:
+                with Action("Waiting to finish creating server", ignore_fail=True):
+                    try:
+                        future.result()
+                    except APIException as exc:
+                        with Action("Sleeping as we have: {exc}"):
+                            time.sleep(60)
+
+            with Action(
+                f"Sleeping until next interval {interval}s", level=logging.DEBUG
+            ):
+                time.sleep(interval)
```

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1153543/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230726.1133529
+Version: 1.2.230726.1153543
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -443,14 +443,37 @@
 :location:
    *ash*
 :type:
    *cpx11*
 :image:
    *ubuntu-22.04*
 
+The **cloud deploy** command uses the following setup script.
+
+:setup script:
+   .. code-block:: bash
+
+      set -x
+      
+      apt-get update
+      
+      apt-get -y install python3-pip
+      apt-get -y install openssh-client
+      
+      echo "Create and configure runner user"
+      
+      adduser runner --disabled-password --gecos ""
+      echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
+      addgroup wheel
+      usermod -aG wheel runner
+      usermod -aG sudo runner
+      
+      echo "Generate SSH Key"
+      sudo -u runner ssh-keygen -t rsa -q -f "/home/runner/.ssh/id_rsa" -N ""
+
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
 The cloud instance that runs the **github-runners** service can either be x64 or ARM64 instance. By default, **cpx11**
```

### Comparing `testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1153543/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

