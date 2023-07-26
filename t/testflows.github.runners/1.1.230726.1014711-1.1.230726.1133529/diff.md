# Comparing `tmp/testflows.github.runners-1.1.230726.1014711.tar.gz` & `tmp/testflows.github.runners-1.1.230726.1133529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.1.230726.1014711.tar", last modified: Wed Jul 26 01:47:12 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.1.230726.1133529.tar", last modified: Wed Jul 26 13:35:29 2023, max compression
```

## Comparing `testflows.github.runners-1.1.230726.1014711.tar` & `testflows.github.runners-1.1.230726.1133529.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.018881 testflows.github.runners-1.1.230726.1014711/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230726.1014711/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    31896 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    31304 2023-07-26 01:46:29.000000 testflows.github.runners-1.1.230726.1014711/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 01:47:12.018881 testflows.github.runners-1.1.230726.1014711/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    19284 2023-07-26 01:36:04.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     9294 2023-07-26 00:14:03.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)     8184 2023-07-25 02:00:02.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4427 2023-07-25 23:18:15.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    31896 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.295917 testflows.github.runners-1.1.230726.1133529/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230726.1133529/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    32758 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    32166 2023-07-26 13:34:52.000000 testflows.github.runners-1.1.230726.1133529/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 13:35:29.295917 testflows.github.runners-1.1.230726.1133529/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    19651 2023-07-26 11:57:13.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8240 2023-07-26 12:06:11.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10060 2023-07-26 12:08:03.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4772 2023-07-26 12:06:30.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230726.1133529/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 13:35:29.291917 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    32758 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 13:35:29.000000 testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.1.230726.1014711/LICENSE` & `testflows.github.runners-1.1.230726.1133529/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/PKG-INFO` & `testflows.github.runners-1.1.230726.1133529/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230726.1014711
+Version: 1.1.230726.1133529
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -52,14 +52,15 @@
 Features
 --------
 
 * cost efficient on-demand runners using Hetzner Cloud
 * supports both x64 and ARM64 runners
 * supports specifying custom runner types using job labels
 * simple configuration
+* self-contained and can deploy and manage itself on a cloud instance
 
 ------------
 Installation
 ------------
 
 .. code-block:: bash
 
@@ -122,49 +123,90 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
------------------
-Using x64 Runners
------------------
+----------------------
+Specifying Runner Type
+----------------------
+
+x64 Runners
+============
 
 The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 
-You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
-The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
-server type name such as *cx11*, *cpx21* etc.
+:✋ Note:
+   You can use **--default-type** option to set a different default server type.
+
+You can specify different x64 server instance type by using the **type-{name}** runner label.
+The **{name}** must be a valid `Hetzner Cloud server type <https://www.hetzner.com/cloud>`_
+name such as *cx11*, *cpx21* etc.
 
 For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
 as follows:
 
 .. code-block:: yaml
 
    job-name:
-      runs-on: [self-hosted, server-cpx21]
+      runs-on: [self-hosted, type-cpx21]
 
--------------------
-Using ARM64 Runners
--------------------
+ARM64 Runners
+==============
 
-The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
-Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **server-{hetzner-server-type}** runner label.
-The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
-server type name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
+The default, the server type is **cx11**, which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **type-{name}** runner label.
+The **{name}** must be a valid `ARM64 Hetzner Cloud server type <https://www.hetzner.com/cloud>`_
+name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
 4 vCPU, 8GB RAM shared-cpu ARM64 instances respectively.
 
 For example, to use Ampere Altra, 4 vCPU, 8GB RAM shared-cpu ARM64 instance, you must define the **runs-on**
 as follows:
 
 .. code-block:: yaml
 
    job-name:
-      runs-on: [self-hosted, server-cax21]
+      runs-on: [self-hosted, type-cax21]
+
+---------------------------
+Specifying Runner Location
+---------------------------
+
+By default, the default location of the server where the runner will be running is not specified. You can use the **--default-location**
+option to force specific default server location.
+
+You can also use the **in-{name}** runner label to specify server location for a specific job. Where **{name}** must be a valid
+`Hetzner Cloud location <https://docs.hetzner.com/cloud/general/locations/>`_ name such as *ash* for US, Ashburn, VA or
+*fsn1* for Germany, Falkenstein.
+
+For example,
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, type-cx11, in-ash]
+
+
+-----------------------
+Specifying Runner Image
+-----------------------
+
+By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
+option to force specific default server image.
+
+You can also use the **image-{name}** runner label to specify server image for a specific job. Where **{name}** must be a valid
+Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*.
+
+For example,
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, type-cx11, in-ash, image-ubuntu-20.04]
 
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
@@ -234,15 +276,14 @@
       User=1000
       Group=1000
       Type=simple
       Restart=always
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
-      Environment=HETZNER_IMAGE=ubuntu-22.04
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
 Modifying Program Options
 =========================
 
@@ -357,17 +398,17 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
----------------------
-Running Cloud Service
----------------------
+--------------------------
+Running as a Cloud Service
+--------------------------
 
 Instead of running **github-runners** program locally as a standalone application or as a service.
 You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
 
 See **-h, --help** for all the available commands.
 
 :✋ Note:
@@ -375,36 +416,14 @@
    is **github-runners**. If you want to use a custom server name, then
    you must use the **cloud --name** option for any **cloud** commands.
 
 .. code-block:: bash
 
    github-runners cloud -h
 
-::
-
-   usage: GitHub Actions runners scale up service cloud [-h] [-n server] command ...
-
-   Deploying and running application as a service on a cloud instance.
-
-   options:
-     -h, --help            show this help message and exit
-     -n server, --name server
-                           deployment server name, default: github-runners
-
-   commands:
-     command
-       deploy              deploy cloud service
-       logs                get cloud service logs
-       status              get cloud service status
-       start               start cloud service
-       stop                stop cloud service
-       install             install cloud service
-       uninstall           uninstall cloud service
-       upgrade             upgrade cloud service
-
 Deployment
 ==========
 
 You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
 using the **cloud deploy** command.
 
 :✋ Note:
@@ -624,36 +643,40 @@
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
 :Server Type:
 
    The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 
-   You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
-   The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+   You can specify different x64 server instance type by using the **type-{name}** runner label.
+   The **{name}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
    server type name such as *cx11*, *cpx21* etc.
 
    For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
    as follows:
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, server-cpx21]
+         runs-on: [self-hosted, type-cpx21]
+
+:Server Location:
+
+   The server location can bespecified by using the **--default-location** option or the **in-<name>** runner label.
+   By default, location is not set as some server types are not available in some locations.
+
+:Image:
+
+   The server is configured to have the image specified by the **--default-image** option or the **image-<name>** runner label.
 
 :SSH Access:
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
-:OS Image:
-
-   The server is configured to have the OS image specified by the **--hetzner-image** option or the **HETZNER_IMAGE**
-   environment variable.
-
 :Image Configuration:
    Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
 The Setup Script
 ================
 
 The **setup** script creates and configures **runner** user that has **sudo** privileges.
@@ -795,16 +818,22 @@
 
 * **--hetzner-token HETZNER_TOKEN**
   Hetzner Cloud token, default: *$HETZNER_TOKEN* environment variable
 
 * **--ssh-key path**
   public SSH key file, default: *~/.ssh/id_rsa.pub*
 
-* **--image HETZNER_IMAGE**
-  Hetzner Cloud server image name, default: *ubuntu-22.04*
+* **--default-type**
+  default runner server type name, default: *cx11*
+
+* **--default-location**
+  default runner server location name, default: not specified
+
+* **--default-image**
+  default runner server image name, default: *ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
```

### Comparing `testflows.github.runners-1.1.230726.1014711/README.rst` & `testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: testflows.github.runners
+Version: 1.1.230726.1133529
+Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
+Home-page: https://github.com/testflows/github-runners
+Author: Vitaliy Zakaznikov
+Author-email: vzakaznikov@testflows.com
+License: Apache-2.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 20%
    :target: https://testflows.com
    :alt: test bug
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
@@ -35,14 +52,15 @@
 Features
 --------
 
 * cost efficient on-demand runners using Hetzner Cloud
 * supports both x64 and ARM64 runners
 * supports specifying custom runner types using job labels
 * simple configuration
+* self-contained and can deploy and manage itself on a cloud instance
 
 ------------
 Installation
 ------------
 
 .. code-block:: bash
 
@@ -105,49 +123,90 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
------------------
-Using x64 Runners
------------------
+----------------------
+Specifying Runner Type
+----------------------
+
+x64 Runners
+============
 
 The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 
-You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
-The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
-server type name such as *cx11*, *cpx21* etc.
+:✋ Note:
+   You can use **--default-type** option to set a different default server type.
+
+You can specify different x64 server instance type by using the **type-{name}** runner label.
+The **{name}** must be a valid `Hetzner Cloud server type <https://www.hetzner.com/cloud>`_
+name such as *cx11*, *cpx21* etc.
 
 For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
 as follows:
 
 .. code-block:: yaml
 
    job-name:
-      runs-on: [self-hosted, server-cpx21]
+      runs-on: [self-hosted, type-cpx21]
 
--------------------
-Using ARM64 Runners
--------------------
+ARM64 Runners
+==============
 
-The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
-Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **server-{hetzner-server-type}** runner label.
-The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
-server type name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
+The default, the server type is **cx11**, which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **type-{name}** runner label.
+The **{name}** must be a valid `ARM64 Hetzner Cloud server type <https://www.hetzner.com/cloud>`_
+name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
 4 vCPU, 8GB RAM shared-cpu ARM64 instances respectively.
 
 For example, to use Ampere Altra, 4 vCPU, 8GB RAM shared-cpu ARM64 instance, you must define the **runs-on**
 as follows:
 
 .. code-block:: yaml
 
    job-name:
-      runs-on: [self-hosted, server-cax21]
+      runs-on: [self-hosted, type-cax21]
+
+---------------------------
+Specifying Runner Location
+---------------------------
+
+By default, the default location of the server where the runner will be running is not specified. You can use the **--default-location**
+option to force specific default server location.
+
+You can also use the **in-{name}** runner label to specify server location for a specific job. Where **{name}** must be a valid
+`Hetzner Cloud location <https://docs.hetzner.com/cloud/general/locations/>`_ name such as *ash* for US, Ashburn, VA or
+*fsn1* for Germany, Falkenstein.
+
+For example,
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, type-cx11, in-ash]
+
+
+-----------------------
+Specifying Runner Image
+-----------------------
+
+By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
+option to force specific default server image.
+
+You can also use the **image-{name}** runner label to specify server image for a specific job. Where **{name}** must be a valid
+Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*.
+
+For example,
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, type-cx11, in-ash, image-ubuntu-20.04]
 
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
@@ -217,15 +276,14 @@
       User=1000
       Group=1000
       Type=simple
       Restart=always
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
-      Environment=HETZNER_IMAGE=ubuntu-22.04
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
 Modifying Program Options
 =========================
 
@@ -340,17 +398,17 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
----------------------
-Running Cloud Service
----------------------
+--------------------------
+Running as a Cloud Service
+--------------------------
 
 Instead of running **github-runners** program locally as a standalone application or as a service.
 You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
 
 See **-h, --help** for all the available commands.
 
 :✋ Note:
@@ -358,36 +416,14 @@
    is **github-runners**. If you want to use a custom server name, then
    you must use the **cloud --name** option for any **cloud** commands.
 
 .. code-block:: bash
 
    github-runners cloud -h
 
-::
-
-   usage: GitHub Actions runners scale up service cloud [-h] [-n server] command ...
-
-   Deploying and running application as a service on a cloud instance.
-
-   options:
-     -h, --help            show this help message and exit
-     -n server, --name server
-                           deployment server name, default: github-runners
-
-   commands:
-     command
-       deploy              deploy cloud service
-       logs                get cloud service logs
-       status              get cloud service status
-       start               start cloud service
-       stop                stop cloud service
-       install             install cloud service
-       uninstall           uninstall cloud service
-       upgrade             upgrade cloud service
-
 Deployment
 ==========
 
 You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
 using the **cloud deploy** command.
 
 :✋ Note:
@@ -607,36 +643,40 @@
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
 :Server Type:
 
    The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 
-   You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
-   The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+   You can specify different x64 server instance type by using the **type-{name}** runner label.
+   The **{name}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
    server type name such as *cx11*, *cpx21* etc.
 
    For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
    as follows:
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, server-cpx21]
+         runs-on: [self-hosted, type-cpx21]
+
+:Server Location:
+
+   The server location can bespecified by using the **--default-location** option or the **in-<name>** runner label.
+   By default, location is not set as some server types are not available in some locations.
+
+:Image:
+
+   The server is configured to have the image specified by the **--default-image** option or the **image-<name>** runner label.
 
 :SSH Access:
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
-:OS Image:
-
-   The server is configured to have the OS image specified by the **--hetzner-image** option or the **HETZNER_IMAGE**
-   environment variable.
-
 :Image Configuration:
    Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
 The Setup Script
 ================
 
 The **setup** script creates and configures **runner** user that has **sudo** privileges.
@@ -778,16 +818,22 @@
 
 * **--hetzner-token HETZNER_TOKEN**
   Hetzner Cloud token, default: *$HETZNER_TOKEN* environment variable
 
 * **--ssh-key path**
   public SSH key file, default: *~/.ssh/id_rsa.pub*
 
-* **--image HETZNER_IMAGE**
-  Hetzner Cloud server image name, default: *ubuntu-22.04*
+* **--default-type**
+  default runner server type name, default: *cx11*
+
+* **--default-location**
+  default runner server location name, default: not specified
+
+* **--default-image**
+  default runner server image name, default: *ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
```

### Comparing `testflows.github.runners-1.1.230726.1014711/setup.py` & `testflows.github.runners-1.1.230726.1133529/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.1.230726.1014711",
+    version="1.1.230726.1133529",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/__init__.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.1.230726.1014711"
+__version__ = "1.1.230726.1133529"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/actions.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/args.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -126,25 +126,40 @@
         "--max-runners",
         metavar="count",
         type=count,
         help="maximum number of active runners, default: unlimited",
     )
 
     parser.add_argument(
-        "--hetzner-image",
-        metavar="HETZNER_IMAGE",
-        type=env_var("HETZNER_IMAGE"),
+        "--default-image",
+        metavar="name",
         help=(
-            "Hetzner Cloud server image name, default: ubuntu-22.04, "
-            "or if specified, $HETZNER_IMAGE environment variable value"
+            "default runner server image name, default: ubuntu-22.04"
         ),
         default="ubuntu-22.04",
     )
 
     parser.add_argument(
+        "--default-type",
+        metavar="name",
+        help=(
+            "default runner server type name, default: cx11"
+        ),
+        default="cx11",
+    )
+
+    parser.add_argument(
+        "--default-location",
+        metavar="name",
+        help=(
+            "default runner server location name, by default not specified"
+        ),
+    )
+
+    parser.add_argument(
         "-w",
         "--workers",
         metavar="count",
         type=count,
         help="number of concurrent workers, default: 10",
         default=10,
     )
@@ -527,15 +542,17 @@
                 scale_up_service: Future = worker_pool.submit(
                     scale_up,
                     terminate=terminate,
                     repo=repo,
                     client=client,
                     scripts=scripts,
                     ssh_key=ssh_key,
-                    image=Image(name=args.hetzner_image),
+                    default_type=args.default_type,
+                    default_image=args.default_image,
+                    default_location=args.default_location,
                     worker_pool=worker_pool,
                     github_token=args.github_token,
                     github_repository=args.github_repository,
                     interval=args.scale_up_interval,
                     max_servers=args.max_runners,
                 )
```

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/cloud.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/cloud.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from hcloud.locations.domain import Location
 
 from .actions import Action
 from .args import check
 from . import __version__
 
 from .server import wait_ready, wait_ssh, ssh
+from .service import command_options
 
 current_dir = os.path.dirname(__file__)
 
 
 def deploy(args, timeout=60):
     """Deploy github-runners as a service to a
     new Hetzner server instance."""
@@ -105,39 +106,15 @@
     with Action("Installing service"):
         command = f"\"su - runner -c '"
         command += f"GITHUB_TOKEN={args.github_token} "
         command += f"GITHUB_REPOSITORY={args.github_repository} "
         command += f"HETZNER_TOKEN={args.hetzner_token} "
 
         command += "github-runners"
-        command += f" --workers {args.workers}"
-        command += f" --hetzner-image {args.hetzner_image}"
-        command += f" --max-runners {args.max_runners}" if args.max_runners else ""
-        command += (
-            f" --logger-config {args.logger_config}" if args.logger_config else ""
-        )
-        command += f" --setup-script {args.setup_script}" if args.setup_script else ""
-        command += (
-            f" --startup-x64-script {args.startup_x64_script}"
-            if args.startup_x64_script
-            else ""
-        )
-        command += (
-            f" --startup-arm64-script {args.startup_arm64_script}"
-            if args.startup_arm64_script
-            else ""
-        )
-        command += (
-            f" --max-powered-off-time {args.max_powered_off_time}"
-            f" --max-idle-runner-time {args.max_idle_runner_time}"
-            f" --max-runner-registration-time {args.max_runner_registration_time}"
-            f" --scale-up-interval {args.scale_up_interval}"
-            f" --scale-down-interval {args.scale_down_interval}"
-        )
-        command += f" --debug" if args.debug else ""
+        command += command_options(args)
         command += " service install -f'\""
 
         ssh(server, command)
 
 
 def upgrade(args):
     """Upgrade github-runners application on a cloud instance."""
```

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/request.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scale_up.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .request import request
 
 from .server import wait_ssh, ssh, wait_ready
 
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
 from hcloud.server_types.domain import ServerType
+from hcloud.locations.domain import Location
 from hcloud.servers.client import BoundServer
 from hcloud.images.domain import Image
 
 from github.Repository import Repository
 from github.WorkflowJob import WorkflowJob
 
 from concurrent.futures import ThreadPoolExecutor, Future
@@ -82,30 +83,32 @@
 
 
 def create_server(
     client: Client,
     job: WorkflowJob,
     name: str,
     server_type: ServerType,
+    server_location: Location,
+    server_image: Image,
     setup_script: str,
     startup_script: str,
     github_token: str,
     github_repository: str,
     ssh_key: SSHKey,
-    image: Image,
     count=1,
     timeout=60,
 ):
     """Create specified number of server instances."""
 
     with Action("Create server"):
         response = client.servers.create(
             name=name,
             server_type=server_type,
-            image=image,
+            location=server_location,
+            image=server_image,
             ssh_keys=[ssh_key],
         )
         server: BoundServer = response.server
 
     with Action(f"Waiting for server {server.name} to be ready") as action:
         wait_ready(server=server, timeout=timeout, action=action)
 
@@ -115,31 +118,66 @@
         startup_script=startup_script,
         github_token=github_token,
         github_repository=github_repository,
         runner_labels=",".join(job.raw_data["labels"]),
     )
 
 
-def get_server_type(job: WorkflowJob, default="cx11", label_prefix="server-"):
+def get_server_type(job: WorkflowJob, default: str, label_prefix="type-"):
     """Get server type for the specified job."""
     server_type = None
-    server_type_name = default
 
     if server_type is None:
         for label in job.raw_data["labels"]:
             if label.startswith(label_prefix):
                 server_type_name = label.split(label_prefix, 1)[-1].lower()
                 server_type = ServerType(name=server_type_name)
 
     if server_type is None:
-        server_type = ServerType(name=server_type_name)
+        server_type = ServerType(name=default)
 
     return server_type
 
 
+def get_server_location(job: WorkflowJob, default: str = "", label_prefix="in-"):
+    """Get preferred server location for the specified job.
+
+    By default, location is set to `None` to avoid server type mismatching
+    the location as some server types are not available at some locations.
+    """
+    server_location: Location = None
+
+    if server_location is None:
+        for label in job.raw_data["labels"]:
+            if label.startswith(label_prefix):
+                server_location_name = label.split(label_prefix, 1)[-1].lower()
+                server_location = Location(name=server_location_name)
+
+    if server_location is None and default:
+        server_location = Location(name=default)
+
+    return server_location
+
+
+def get_server_image(job: WorkflowJob, default: str, label_prefix="image-"):
+    """Get preferred server image for the specified job."""
+    server_image: Image = None
+
+    if server_image is None:
+        for label in job.raw_data["labels"]:
+            if label.startswith(label_prefix):
+                server_image_name = label.split(label_prefix, 1)[-1].lower()
+                server_image = Image(name=server_image_name)
+
+    if server_image is None:
+        server_image = Image(name=default)
+
+    return server_image
+
+
 def get_startup_script(server_type: ServerType, scripts: Scripts):
     """Get startup script based on the requested server type.
     ARM64 servers type names start with "CA" prefix.
 
     For example, CAX11, CAX21, CAX31, and CAX41
     """
     if server_type.name.lower().startswith("ca"):
@@ -153,15 +191,17 @@
     repo: Repository,
     client: Client,
     scripts: Scripts,
     worker_pool: ThreadPoolExecutor,
     github_token: str,
     github_repository: str,
     ssh_key: SSHKey,
-    image: Image,
+    default_type: str,
+    default_location: str,
+    default_image: str,
     interval: int,
     max_servers: int,
 ):
     """Scale up service."""
     while True:
         if terminate.is_set():
             with Action("Terminating scale up service"):
@@ -182,15 +222,21 @@
 
         with Action("Looking for queued jobs", level=logging.DEBUG) as action:
             for run in workflow_runs:
                 for job in run.jobs():
                     if job.status == "queued":
                         with Action(f"Found queued job {job}"):
                             server_name = f"{runner_server_prefix}{job.run_id}"
-                            server_type = get_server_type(job=job)
+                            server_type = get_server_type(job=job, default=default_type)
+                            server_location = get_server_location(
+                                job=job, default=default_location
+                            )
+                            server_image = get_server_image(
+                                job=job, default=default_image
+                            )
                             startup_script = get_startup_script(
                                 server_type=server_type, scripts=scripts
                             )
 
                             if max_servers is not None:
                                 with Action(
                                     f"Checking if maximum number of servers has been reached",
@@ -213,14 +259,16 @@
                             futures.append(
                                 worker_pool.submit(
                                     create_server,
                                     client=client,
                                     job=job,
                                     name=server_name,
                                     server_type=server_type,
+                                    server_location=server_location,
+                                    server_image=server_image,
                                     setup_script=scripts.setup,
                                     startup_script=startup_script,
                                     github_token=github_token,
                                     github_repository=github_repository,
                                     ssh_key=ssh_key,
                                     image=image,
                                 )
```

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/server.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/service.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,54 @@
 NAME = "github-runners"
 SERVICE = f"/etc/systemd/system/{NAME}.service"
 
 from .actions import Action
 from .args import check
 
 
+def command_options(args):
+    """Build service install command options not including:
+
+    --github-token
+    --github-repository
+    --hetzner-token
+    --ssh-key
+    """
+    command = None
+    command += f" --workers {args.workers}"
+    command += f" --default-type {args.default_type}"
+    command += (
+        f" --default-location {args.default_location}" if args.default_location else ""
+    )
+    command += f" --default-image {args.default_image}"
+    command += f" --max-runners {args.max_runners}" if args.max_runners else ""
+    command += f" --logger-config {args.logger_config}" if args.logger_config else ""
+    command += f" --setup-script {args.setup_script}" if args.setup_script else ""
+    command += (
+        f" --startup-x64-script {args.startup_x64_script}"
+        if args.startup_x64_script
+        else ""
+    )
+    command += (
+        f" --startup-arm64-script {args.startup_arm64_script}"
+        if args.startup_arm64_script
+        else ""
+    )
+    command += (
+        f" --max-powered-off-time {args.max_powered_off_time}"
+        f" --max-idle-runner-time {args.max_idle_runner_time}"
+        f" --max-runner-registration-time {args.max_runner_registration_time}"
+        f" --scale-up-interval {args.scale_up_interval}"
+        f" --scale-down-interval {args.scale_down_interval}"
+    )
+    command += f" --debug" if args.debug else ""
+
+    return command
+
+
 def install(args):
     """Install service."""
     check(args)
 
     force = args.force
 
     current_dir = os.path.dirname(__file__)
@@ -51,38 +91,15 @@
             f"Environment=GITHUB_TOKEN={args.github_token}\n"
             f"Environment=GITHUB_REPOSITORY={args.github_repository}\n"
             f"Environment=HETZNER_TOKEN={args.hetzner_token}\n"
             f"ExecStart={binary}"
             f" --workers {args.workers}"
         )
         contents += f" --ssh-key {args.ssh_key.name}"
-        contents += f" --max-runners {args.max_runners}" if args.max_runners else ""
-        contents += (
-            f" --logger-config {args.logger_config}" if args.logger_config else ""
-        )
-        contents += f" --hetzner-image {args.hetzner_image}"
-        contents += f" --setup-script {args.setup_script}" if args.setup_script else ""
-        contents += (
-            f" --startup-x64-script {args.startup_x64_script}"
-            if args.startup_x64_script
-            else ""
-        )
-        contents += (
-            f" --startup-arm64-script {args.startup_arm64_script}"
-            if args.startup_arm64_script
-            else ""
-        )
-        contents += (
-            f" --max-powered-off-time {args.max_powered_off_time}"
-            f" --max-idle-runner-time {args.max_idle_runner_time}"
-            f" --max-runner-registration-time {args.max_runner_registration_time}"
-            f" --scale-up-interval {args.scale_up_interval}"
-            f" --scale-down-interval {args.scale_down_interval}"
-        )
-        contents += f" --debug" if args.debug else ""
+        contents += command_options(args)
         contents += "\n" "[Install]\n" "WantedBy=multi-user.target\n"
 
         os.system(f"sudo bash -c \"cat > {SERVICE}\" <<'EOF'\n{contents}\nEOF")
         os.system(f"sudo chmod 700 {SERVICE}")
 
     with Action("Reloading systemd"):
         os.system("sudo systemctl daemon-reload")
```

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/shell.py` & `testflows.github.runners-1.1.230726.1133529/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.1.230726.1133529/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: testflows.github.runners
-Version: 1.1.230726.1014711
-Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
-Home-page: https://github.com/testflows/github-runners
-Author: Vitaliy Zakaznikov
-Author-email: vzakaznikov@testflows.com
-License: Apache-2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 20%
    :target: https://testflows.com
    :alt: test bug
 
 ======================================================
 Autoscaling GitHub Actions Runners Using Hetzner Cloud
@@ -52,14 +35,15 @@
 Features
 --------
 
 * cost efficient on-demand runners using Hetzner Cloud
 * supports both x64 and ARM64 runners
 * supports specifying custom runner types using job labels
 * simple configuration
+* self-contained and can deploy and manage itself on a cloud instance
 
 ------------
 Installation
 ------------
 
 .. code-block:: bash
 
@@ -122,49 +106,90 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
------------------
-Using x64 Runners
------------------
+----------------------
+Specifying Runner Type
+----------------------
+
+x64 Runners
+============
 
 The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 
-You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
-The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
-server type name such as *cx11*, *cpx21* etc.
+:✋ Note:
+   You can use **--default-type** option to set a different default server type.
+
+You can specify different x64 server instance type by using the **type-{name}** runner label.
+The **{name}** must be a valid `Hetzner Cloud server type <https://www.hetzner.com/cloud>`_
+name such as *cx11*, *cpx21* etc.
 
 For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
 as follows:
 
 .. code-block:: yaml
 
    job-name:
-      runs-on: [self-hosted, server-cpx21]
+      runs-on: [self-hosted, type-cpx21]
 
--------------------
-Using ARM64 Runners
--------------------
+ARM64 Runners
+==============
 
-The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
-Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **server-{hetzner-server-type}** runner label.
-The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
-server type name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
+The default, the server type is **cx11**, which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **type-{name}** runner label.
+The **{name}** must be a valid `ARM64 Hetzner Cloud server type <https://www.hetzner.com/cloud>`_
+name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
 4 vCPU, 8GB RAM shared-cpu ARM64 instances respectively.
 
 For example, to use Ampere Altra, 4 vCPU, 8GB RAM shared-cpu ARM64 instance, you must define the **runs-on**
 as follows:
 
 .. code-block:: yaml
 
    job-name:
-      runs-on: [self-hosted, server-cax21]
+      runs-on: [self-hosted, type-cax21]
+
+---------------------------
+Specifying Runner Location
+---------------------------
+
+By default, the default location of the server where the runner will be running is not specified. You can use the **--default-location**
+option to force specific default server location.
+
+You can also use the **in-{name}** runner label to specify server location for a specific job. Where **{name}** must be a valid
+`Hetzner Cloud location <https://docs.hetzner.com/cloud/general/locations/>`_ name such as *ash* for US, Ashburn, VA or
+*fsn1* for Germany, Falkenstein.
+
+For example,
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, type-cx11, in-ash]
+
+
+-----------------------
+Specifying Runner Image
+-----------------------
+
+By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
+option to force specific default server image.
+
+You can also use the **image-{name}** runner label to specify server image for a specific job. Where **{name}** must be a valid
+Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*.
+
+For example,
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, type-cx11, in-ash, image-ubuntu-20.04]
 
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
@@ -234,15 +259,14 @@
       User=1000
       Group=1000
       Type=simple
       Restart=always
       Environment=GITHUB_TOKEN=ghp_...
       Environment=GITHUB_REPOSITORY=testflows/github-runners
       Environment=HETZNER_TOKEN=GJ..
-      Environment=HETZNER_IMAGE=ubuntu-22.04
       ExecStart=/home/user/.local/lib/python3.10/site-packages/testflows/github/runners/bin/github-runners --workers 10 --max-powered-off-time 20 --max-idle-runner-time 120 --max-runner-registration-time 60 --scale-up-interval 10 --scale-down-interval 10
       [Install]
       WantedBy=multi-user.target
 
 Modifying Program Options
 =========================
 
@@ -357,17 +381,17 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
----------------------
-Running Cloud Service
----------------------
+--------------------------
+Running as a Cloud Service
+--------------------------
 
 Instead of running **github-runners** program locally as a standalone application or as a service.
 You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
 
 See **-h, --help** for all the available commands.
 
 :✋ Note:
@@ -375,36 +399,14 @@
    is **github-runners**. If you want to use a custom server name, then
    you must use the **cloud --name** option for any **cloud** commands.
 
 .. code-block:: bash
 
    github-runners cloud -h
 
-::
-
-   usage: GitHub Actions runners scale up service cloud [-h] [-n server] command ...
-
-   Deploying and running application as a service on a cloud instance.
-
-   options:
-     -h, --help            show this help message and exit
-     -n server, --name server
-                           deployment server name, default: github-runners
-
-   commands:
-     command
-       deploy              deploy cloud service
-       logs                get cloud service logs
-       status              get cloud service status
-       start               start cloud service
-       stop                stop cloud service
-       install             install cloud service
-       uninstall           uninstall cloud service
-       upgrade             upgrade cloud service
-
 Deployment
 ==========
 
 You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
 using the **cloud deploy** command.
 
 :✋ Note:
@@ -624,36 +626,40 @@
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
 :Server Type:
 
    The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
 
-   You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
-   The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+   You can specify different x64 server instance type by using the **type-{name}** runner label.
+   The **{name}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
    server type name such as *cx11*, *cpx21* etc.
 
    For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
    as follows:
 
    .. code-block:: yaml
 
       job-name:
-         runs-on: [self-hosted, server-cpx21]
+         runs-on: [self-hosted, type-cpx21]
+
+:Server Location:
+
+   The server location can bespecified by using the **--default-location** option or the **in-<name>** runner label.
+   By default, location is not set as some server types are not available in some locations.
+
+:Image:
+
+   The server is configured to have the image specified by the **--default-image** option or the **image-<name>** runner label.
 
 :SSH Access:
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
-:OS Image:
-
-   The server is configured to have the OS image specified by the **--hetzner-image** option or the **HETZNER_IMAGE**
-   environment variable.
-
 :Image Configuration:
    Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
 The Setup Script
 ================
 
 The **setup** script creates and configures **runner** user that has **sudo** privileges.
@@ -795,16 +801,22 @@
 
 * **--hetzner-token HETZNER_TOKEN**
   Hetzner Cloud token, default: *$HETZNER_TOKEN* environment variable
 
 * **--ssh-key path**
   public SSH key file, default: *~/.ssh/id_rsa.pub*
 
-* **--image HETZNER_IMAGE**
-  Hetzner Cloud server image name, default: *ubuntu-22.04*
+* **--default-type**
+  default runner server type name, default: *cx11*
+
+* **--default-location**
+  default runner server location name, default: not specified
+
+* **--default-image**
+  default runner server image name, default: *ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
```

### Comparing `testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.1.230726.1133529/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

