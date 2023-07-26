# Comparing `tmp/testflows.github.runners-1.2.230726.1162425.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1182348.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1162425.tar", last modified: Wed Jul 26 16:24:25 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1182348.tar", last modified: Wed Jul 26 18:23:48 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1162425.tar` & `testflows.github.runners-1.2.230726.1182348.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1162425/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    32769 2023-07-26 13:54:40.000000 testflows.github.runners-1.2.230726.1162425/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.397697 testflows.github.runners-1.2.230726.1162425/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.397697 testflows.github.runners-1.2.230726.1162425/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    19676 2023-07-26 15:33:47.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8131 2023-07-26 16:23:24.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    10944 2023-07-26 15:44:57.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4770 2023-07-26 15:40:21.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1162425/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 16:24:25.401697 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33361 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 16:24:25.000000 testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.358374 testflows.github.runners-1.2.230726.1182348/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1182348/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 18:23:48.358374 testflows.github.runners-1.2.230726.1182348/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    32718 2023-07-26 18:23:14.000000 testflows.github.runners-1.2.230726.1182348/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 18:23:48.358374 testflows.github.runners-1.2.230726.1182348/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.354374 testflows.github.runners-1.2.230726.1182348/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.354374 testflows.github.runners-1.2.230726.1182348/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.354374 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.354374 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    19676 2023-07-26 15:33:47.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8131 2023-07-26 16:23:24.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11025 2023-07-26 18:20:22.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.358374 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.358374 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4770 2023-07-26 15:40:21.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1182348/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:23:48.354374 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 18:23:48.000000 testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1162425/LICENSE` & `testflows.github.runners-1.2.230726.1182348/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/PKG-INFO` & `testflows.github.runners-1.2.230726.1182348/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1162425
+Version: 1.2.230726.1182348
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -294,17 +294,14 @@
 .. code-block:: bash
 
    github-runners service stop
    sudo vim /etc/systemd/system/github-runners.service
    sudo systemctl daemon-reload
    github-runners service start
 
-.. code-block:: bash
-
-   github-runners service uninstall
 
 Checking Status
 ================
 
 After installation, you can check the status of the service using the **service status** command.
 
 .. code-block:: bash
@@ -449,28 +446,28 @@
 
 The **cloud deploy** command uses the following setup script.
 
 :setup script:
    .. code-block:: bash
 
       set -x
-      
+
       apt-get update
-      
+
       apt-get -y install python3-pip
       apt-get -y install openssh-client
-      
+
       echo "Create and configure runner user"
-      
+
       adduser runner --disabled-password --gecos ""
       echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
       addgroup wheel
       usermod -aG wheel runner
       usermod -aG sudo runner
-      
+
       echo "Generate SSH Key"
       sudo -u runner ssh-keygen -t rsa -q -f "/home/runner/.ssh/id_rsa" -N ""
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
@@ -627,29 +624,29 @@
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
-   github-runner-{job.run_id}
+   github-runner-{job.run_id}-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
 to be the same as the server name so that servers can be deleted for any idle runner that for some reason
 does not pick up a job for which it was created within the **max-idle-runner-time** period.
 
 :Note:
-   Given that the server name is fixed and specific for each *job.run_id*, if multiple `github-runners` are running in parallel then
+   Given that the server name is fixed and specific for each *job.run_id, job.id* tuple, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the job with the exact **run_id** that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact **run_id, job.id** tuple that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 Maximum Number of Runners
 =========================
 
 By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
```

### Comparing `testflows.github.runners-1.2.230726.1162425/README.rst` & `testflows.github.runners-1.2.230726.1182348/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -277,17 +277,14 @@
 .. code-block:: bash
 
    github-runners service stop
    sudo vim /etc/systemd/system/github-runners.service
    sudo systemctl daemon-reload
    github-runners service start
 
-.. code-block:: bash
-
-   github-runners service uninstall
 
 Checking Status
 ================
 
 After installation, you can check the status of the service using the **service status** command.
 
 .. code-block:: bash
@@ -432,28 +429,28 @@
 
 The **cloud deploy** command uses the following setup script.
 
 :setup script:
    .. code-block:: bash
 
       set -x
-      
+
       apt-get update
-      
+
       apt-get -y install python3-pip
       apt-get -y install openssh-client
-      
+
       echo "Create and configure runner user"
-      
+
       adduser runner --disabled-password --gecos ""
       echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
       addgroup wheel
       usermod -aG wheel runner
       usermod -aG sudo runner
-      
+
       echo "Generate SSH Key"
       sudo -u runner ssh-keygen -t rsa -q -f "/home/runner/.ssh/id_rsa" -N ""
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
@@ -610,29 +607,29 @@
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
-   github-runner-{job.run_id}
+   github-runner-{job.run_id}-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
 to be the same as the server name so that servers can be deleted for any idle runner that for some reason
 does not pick up a job for which it was created within the **max-idle-runner-time** period.
 
 :Note:
-   Given that the server name is fixed and specific for each *job.run_id*, if multiple `github-runners` are running in parallel then
+   Given that the server name is fixed and specific for each *job.run_id, job.id* tuple, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the job with the exact **run_id** that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact **run_id, job.id** tuple that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 Maximum Number of Runners
 =========================
 
 By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
```

### Comparing `testflows.github.runners-1.2.230726.1162425/setup.py` & `testflows.github.runners-1.2.230726.1182348/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1162425",
+    version="1.2.230726.1182348",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/__init__.py`

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
-__version__ = "1.2.230726.1162425"
+__version__ = "1.2.230726.1182348"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scale_up.py`

 * *Files 0% similar despite different names*

```diff
@@ -227,15 +227,17 @@
             futures: list[Future] = []
 
             with Action("Looking for queued jobs", level=logging.DEBUG) as action:
                 for run in workflow_runs:
                     for job in run.jobs():
                         if job.status == "queued":
                             with Action(f"Found queued job {job}"):
-                                server_name = f"{runner_server_prefix}{job.run_id}"
+                                server_name = (
+                                    f"{runner_server_prefix}{job.run_id}-{job.id}"
+                                )
                                 server_type = get_server_type(
                                     job=job, default=default_type
                                 )
                                 server_location = get_server_location(
                                     job=job, default=default_location
                                 )
                                 server_image = get_server_image(
```

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1182348/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1162425
+Version: 1.2.230726.1182348
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -294,17 +294,14 @@
 .. code-block:: bash
 
    github-runners service stop
    sudo vim /etc/systemd/system/github-runners.service
    sudo systemctl daemon-reload
    github-runners service start
 
-.. code-block:: bash
-
-   github-runners service uninstall
 
 Checking Status
 ================
 
 After installation, you can check the status of the service using the **service status** command.
 
 .. code-block:: bash
@@ -449,28 +446,28 @@
 
 The **cloud deploy** command uses the following setup script.
 
 :setup script:
    .. code-block:: bash
 
       set -x
-      
+
       apt-get update
-      
+
       apt-get -y install python3-pip
       apt-get -y install openssh-client
-      
+
       echo "Create and configure runner user"
-      
+
       adduser runner --disabled-password --gecos ""
       echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
       addgroup wheel
       usermod -aG wheel runner
       usermod -aG sudo runner
-      
+
       echo "Generate SSH Key"
       sudo -u runner ssh-keygen -t rsa -q -f "/home/runner/.ssh/id_rsa" -N ""
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
@@ -627,29 +624,29 @@
 ------------------
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
-   github-runner-{job.run_id}
+   github-runner-{job.run_id}-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
 to be the same as the server name so that servers can be deleted for any idle runner that for some reason
 does not pick up a job for which it was created within the **max-idle-runner-time** period.
 
 :Note:
-   Given that the server name is fixed and specific for each *job.run_id*, if multiple `github-runners` are running in parallel then
+   Given that the server name is fixed and specific for each *job.run_id, job.id* tuple, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the job with the exact **run_id** that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact **run_id, job.id** tuple that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 Maximum Number of Runners
 =========================
 
 By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
```

### Comparing `testflows.github.runners-1.2.230726.1162425/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1182348/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

