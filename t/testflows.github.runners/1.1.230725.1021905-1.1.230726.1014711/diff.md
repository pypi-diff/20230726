# Comparing `tmp/testflows.github.runners-1.1.230725.1021905.tar.gz` & `tmp/testflows.github.runners-1.1.230726.1014711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.1.230725.1021905.tar", last modified: Tue Jul 25 02:19:05 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.1.230726.1014711.tar", last modified: Wed Jul 26 01:47:12 2023, max compression
```

## Comparing `testflows.github.runners-1.1.230725.1021905.tar` & `testflows.github.runners-1.1.230726.1014711.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:19:05.633342 testflows.github.runners-1.1.230725.1021905/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230725.1021905/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    22139 2023-07-25 02:19:05.633342 testflows.github.runners-1.1.230725.1021905/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    21547 2023-07-25 01:47:16.000000 testflows.github.runners-1.1.230725.1021905/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 02:19:05.633342 testflows.github.runners-1.1.230725.1021905/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-25 02:19:05.000000 testflows.github.runners-1.1.230725.1021905/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:19:05.629342 testflows.github.runners-1.1.230725.1021905/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:19:05.629342 testflows.github.runners-1.1.230725.1021905/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:19:05.629342 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-25 02:19:05.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:19:05.629342 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    14693 2023-07-25 02:07:25.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     4473 2023-07-25 02:17:59.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/deploy.py
--rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)     8184 2023-07-25 02:00:02.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:19:05.629342 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:19:05.629342 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4426 2023-07-25 02:03:48.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230725.1021905/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 02:19:05.629342 testflows.github.runners-1.1.230725.1021905/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    22139 2023-07-25 02:19:05.000000 testflows.github.runners-1.1.230725.1021905/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1001 2023-07-25 02:19:05.000000 testflows.github.runners-1.1.230725.1021905/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 02:19:05.000000 testflows.github.runners-1.1.230725.1021905/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230725.1021905/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-25 02:19:05.000000 testflows.github.runners-1.1.230725.1021905/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-25 02:19:05.000000 testflows.github.runners-1.1.230725.1021905/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.018881 testflows.github.runners-1.1.230726.1014711/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.1.230726.1014711/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    31896 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    31304 2023-07-26 01:46:29.000000 testflows.github.runners-1.1.230726.1014711/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 01:47:12.018881 testflows.github.runners-1.1.230726.1014711/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    19284 2023-07-26 01:36:04.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     9294 2023-07-26 00:14:03.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1266 2023-07-24 15:25:53.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8184 2023-07-25 02:00:02.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4427 2023-07-25 23:18:15.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1392 2023-07-24 23:28:45.000000 testflows.github.runners-1.1.230726.1014711/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 01:47:12.014881 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    31896 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 01:47:11.000000 testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.1.230725.1021905/LICENSE` & `testflows.github.runners-1.1.230726.1014711/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/PKG-INFO` & `testflows.github.runners-1.1.230726.1014711/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: testflows.github.runners
-Version: 1.1.230725.1021905
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
@@ -122,14 +105,78 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
+-----------------
+Using x64 Runners
+-----------------
+
+The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+
+You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
+The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+server type name such as *cx11*, *cpx21* etc.
+
+For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
+as follows:
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, server-cpx21]
+
+-------------------
+Using ARM64 Runners
+-------------------
+
+The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **server-{hetzner-server-type}** runner label.
+The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+server type name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
+4 vCPU, 8GB RAM shared-cpu ARM64 instances respectively.
+
+For example, to use Ampere Altra, 4 vCPU, 8GB RAM shared-cpu ARM64 instance, you must define the **runs-on**
+as follows:
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, server-cax21]
+
+-------
+SSH Key
+-------
+
+All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
+using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
+
+The SSH key will be automatically added to your project using the MD5 hash of the public key as the SSH key name.
+
+:❗Warning:
+   Given that each new SSH key is automatically added to your Hetzner project, you must manually delete them when no longer needed.
+
+Most GitHub users already have an SSH key associated with the account. If you want to know how to add an SSH key, see `Adding a new SSH key to your GitHub account    <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account>`_ article.
+
+Generating New SSH Key
+=======================
+
+If you need to generate a new SSH key, see `Generating a new SSH key and adding it to the ssh-agent <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>`_ article.
+
+Cloud Deployment
+================
+
+If you are deploying the **github-runners** program as a cloud service using the **github-runners <options> cloud deploy** command, then
+after provisoning a new cloud server instance that will host the **github-runners** service, a new SSH key will be
+auto-generated to access the runners. The auto-generated key will be placed in */home/runner/.ssh/id_rsa*, where **runner**
+is the user under which the **github-runners** service runs on the cloud instance. The auto-generated SSH key will be automatically
+added to your project using the MD5 hash of the public key as the SSH key name.
+
 -----------------------
 Running as a Service
 -----------------------
 
 You can run **github-runners** as a service.
 
 :✋ Note:
@@ -293,23 +340,62 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
------------------------
-Deploying Application
------------------------
+---------------------
+Running Cloud Service
+---------------------
 
-You can deploy **github-runners** as a service to a new Hetzner Cloud server instance
-using the **deploy** command.
+Instead of running **github-runners** program locally as a standalone application or as a service.
+You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
+
+See **-h, --help** for all the available commands.
 
 :✋ Note:
-   The options that are passed to the **github-runners <options> deploy** command
+   By default, the server name where the **github-runners** service will be running
+   is **github-runners**. If you want to use a custom server name, then
+   you must use the **cloud --name** option for any **cloud** commands.
+
+.. code-block:: bash
+
+   github-runners cloud -h
+
+::
+
+   usage: GitHub Actions runners scale up service cloud [-h] [-n server] command ...
+
+   Deploying and running application as a service on a cloud instance.
+
+   options:
+     -h, --help            show this help message and exit
+     -n server, --name server
+                           deployment server name, default: github-runners
+
+   commands:
+     command
+       deploy              deploy cloud service
+       logs                get cloud service logs
+       status              get cloud service status
+       start               start cloud service
+       stop                stop cloud service
+       install             install cloud service
+       uninstall           uninstall cloud service
+       upgrade             upgrade cloud service
+
+Deployment
+==========
+
+You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
+using the **cloud deploy** command.
+
+:✋ Note:
+   The options that are passed to the **github-runners <options> cloud deploy** command
    will be the same options with which the service will be executed.
 
 .. code-block:: bash
 
    export GITHUB_TOKEN=ghp_...
    export GITHUB_REPOSITORY=testflows/github-runners
    export HETZNER_TOKEN=GJzdc...
@@ -327,46 +413,191 @@
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
+The cloud instance that runs the **github-runners** service can either be x64 or ARM64 instance. By default, **cpx11**
+AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used.
+
+Using ARM64 Instance
+++++++++++++++++++++
+
+If you want to deploy the **github-runners** service to an ARM64 instance, then you must specify the instance
+type using the **--type** option.
+
+:✋ Note:
+   Currently Hetzner Cloud has ARM64 instances only available in Germany, Falkenstein (**fsn1**) location.
+
+For example, to use Ampere Altra, 4 vCPU, 8GB RAM shared-cpu ARM64 instance, you must specify **cax21**
+as the value of the **--type** as follows:
+
+.. code-block:: bash
+
+   github-runners deploy --location fsn1 --type cax21 --image ubuntu-22.04
+
+Using x64 Instance
+++++++++++++++++++
+
+By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
+a different x64 instance then specify desired type using the **--type** option.
+
+Cloud Service Logs
+===================
+
+You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
+Specify **-f, --follow** if you want to follow the logs journal.
+
+For example,
+
+:dump the full log:
+
+   .. code-block:: bash
+
+      github-runners cloud logs
+
+:follow the logs journal:
+
+   .. code-block:: bash
+
+      github-runners cloud logs -f
+
+
+Cloud Service Status
+=====================
+
+You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
+
+For example,
+
+.. code-block:: bash
+
+   github-runners cloud status
+
+Stopping Cloud Service
+======================
+
+You can manually stop the **github-runners** service running on a cloud instance using the **github-runners cloud stop** command.
+
+.. code-block:: bash
+
+   github-runners cloud stop
+
+Starting Cloud Service
+======================
+
+You can manually start the **github-runners** service running on a cloud instance after it was being manually stopped
+using the **github-runners cloud start** command.
+
+.. code-block:: bash
+
+   github-runners cloud start
+
+Installing Cloud Service
+========================
+
+You can manually force installation of the **github-runners** service running on a cloud instance using
+the **github-runners cloud install** command.
+
+:✋ Note:
+   Just like with the `github-runners <options> service install` command,
+   the options that are passed to the `github-runners <options> cloud install` command
+   will be the same options with which the service will be executed.
+
+You can specify **-f, --force** option to force service re-installation if it is already installed.
+
+.. code-block:: bash
+
+   github-runners <options> cloud install -f
+
+
+Uninstalling Cloud Service
+==========================
+
+You can manually force uninstallation of the **github-runners** service running on a cloud instance using
+the **github-runners cloud uninstall** command.
+
+.. code-block:: bash
+
+   github-runners cloud uninstall
+
+Upgrading Cloud Service
+========================
+
+You can manually upgrade the **github-runners** service package running on a cloud instance using
+the **github-runners cloud upgrade** command.
+
+If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
+the specified version otherwise the version is upgraded to the latest available.
+
+:✋ Note:
+   The service is not re-installed during the package upgrade process.
+   Instead, it is stopped before the upgrade and then started back up
+   after the package upgrade is complete.
+
+.. code-block:: bash
+
+   github-runners cloud upgrade --version <version>
+
+Deleting Cloud Service
+======================
+
+You can delete the **github-runners** cloud service and the cloud instance that is running on using
+the **github-runners cloud delete** command.
+
+The **cloud delete** command, deletes the cloud service by first stopping the service and then deleting the server instance.
+
+:❗Warning:
+   The default server name where the cloud service is deployed is **github-runners**.
+   Please make sure to specify the **cloud --name** option if you have deployed the service to a server with a different name.
+
+For example,
+
+:default name:
+   .. code-block:: bash
+
+      github-runners cloud delete
+
+:custom name:
+   .. code-block:: bash
+
+      github-runners cloud --name <custom_name> delete
 
 ------------------
 Scaling Up Runners
 ------------------
 
-The program scale up runners by looking for any jobs that have **queued** status.
+The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
    github-runner-{job.run_id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
-to be the same as the server name so that servers can deleted for any idle runner that for some reason
+to be the same as the server name so that servers can be deleted for any idle runner that for some reason
 does not pick up a job for which it was created within the **max-idle-runner-time** period.
 
 :Note:
    Given that the server name is fixed and specific for each *job.run_id*, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the the job with the exact **run_id** that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact **run_id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
-   equal the number of jobs and therefore under normal conditions all jobs will executed as expected.
+   equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 Maximum Number of Runners
 =========================
 
-By default, the maximum number of runners and therefore the maximum number if server instances is not set and therefore is unlimited.
+By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
 
 
@@ -374,40 +605,45 @@
 ==========
 
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
 :Server Type:
 
-   The default server type is **cx11**. However, a job **server-{hetzner-server-type}** label can be used to specify
-   custom server type. Where the **{hetzner-server-type}** must be a valid Hetzner Cloud server type name such as *cx11*, *cpx21* etc.
+   The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+
+   You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
+   The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+   server type name such as *cx11*, *cpx21* etc.
 
-   For example,
+   For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
+   as follows:
 
    .. code-block:: yaml
 
-       runs-on: [self-hosted, server-cpx21]
+      job-name:
+         runs-on: [self-hosted, server-cpx21]
 
 :SSH Access:
 
-   The server is configured to be accessed using *ssh* utility and the SSH public key path is specified either using the **--ssh-key**
+   The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :OS Image:
 
    The server is configured to have the OS image specified by the **--hetzner-image** option or the **HETZNER_IMAGE**
    environment variable.
 
 :Image Configuration:
-   Each new server instance is configured using `setup <#the-setup-script>`_ and `startup <#the-start-up-script>`_ scripts.
+   Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
 The Setup Script
 ================
 
-The **setup** script created and configures **runner** user that has **sudo** privileges.
+The **setup** script creates and configures **runner** user that has **sudo** privileges.
 
 :Setup:
 
    .. code-block:: bash
 
         set -x
 
@@ -585,31 +821,64 @@
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
 
-    * **deploy**
-      deploy application
+    * **cloud**
+      cloud service commands
 
-      * **-n, --name**
+      * **-n server, --name server**
         deployment server name, default: *github-runners*
 
-      * **-f, --force**
-        force deployment if already exist
+      * **deploy**
+        deploy cloud service
+
+        * **-f, --force**
+          force deployment if already exist
+
+        * **-l name, --location name**
+          deployment server location, default: *ash*
+
+        * **-t name, --type name**
+          deployment server type, default: *cpx11*
+
+        * **-i name, --image name**
+          deployment server image, default: *ubuntu-22.04*
+
+      * **logs**
+        get cloud service logs
+
+        * **-f, --follow**
+          follow logs journal, default: *False*
+
+      * **status**
+        get cloud service status
+
+      * **start**
+        start cloud service
+
+      * **stop**
+        stop cloud service
+
+      * **install**
+        install cloud service
+
+        * **-f, --force**
+          force installation if service already exists
 
-      * **-l name, --location name**
-        deployment server location, default: *ash*
+      * **uninstall**
+        uninstall cloud service
 
-      * **-t name, --type name**
-        deployment server type, default: *cpx11*
+      * **upgrade**
+        upgrade cloud service
 
-      * **-i name, --image name**
-        deployment server image, default: *ubuntu-22.04*
+        * **--version version**
+          package version, default: *the latest*
 
     * **service**
       service commands
 
       * **install**
         install service
```

### Comparing `testflows.github.runners-1.1.230725.1021905/README.rst` & `testflows.github.runners-1.1.230726.1014711/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: testflows.github.runners
+Version: 1.1.230726.1014711
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
@@ -105,14 +122,78 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
+-----------------
+Using x64 Runners
+-----------------
+
+The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+
+You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
+The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+server type name such as *cx11*, *cpx21* etc.
+
+For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
+as follows:
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, server-cpx21]
+
+-------------------
+Using ARM64 Runners
+-------------------
+
+The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **server-{hetzner-server-type}** runner label.
+The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+server type name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
+4 vCPU, 8GB RAM shared-cpu ARM64 instances respectively.
+
+For example, to use Ampere Altra, 4 vCPU, 8GB RAM shared-cpu ARM64 instance, you must define the **runs-on**
+as follows:
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, server-cax21]
+
+-------
+SSH Key
+-------
+
+All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
+using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
+
+The SSH key will be automatically added to your project using the MD5 hash of the public key as the SSH key name.
+
+:❗Warning:
+   Given that each new SSH key is automatically added to your Hetzner project, you must manually delete them when no longer needed.
+
+Most GitHub users already have an SSH key associated with the account. If you want to know how to add an SSH key, see `Adding a new SSH key to your GitHub account    <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account>`_ article.
+
+Generating New SSH Key
+=======================
+
+If you need to generate a new SSH key, see `Generating a new SSH key and adding it to the ssh-agent <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>`_ article.
+
+Cloud Deployment
+================
+
+If you are deploying the **github-runners** program as a cloud service using the **github-runners <options> cloud deploy** command, then
+after provisoning a new cloud server instance that will host the **github-runners** service, a new SSH key will be
+auto-generated to access the runners. The auto-generated key will be placed in */home/runner/.ssh/id_rsa*, where **runner**
+is the user under which the **github-runners** service runs on the cloud instance. The auto-generated SSH key will be automatically
+added to your project using the MD5 hash of the public key as the SSH key name.
+
 -----------------------
 Running as a Service
 -----------------------
 
 You can run **github-runners** as a service.
 
 :✋ Note:
@@ -276,23 +357,62 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
------------------------
-Deploying Application
------------------------
+---------------------
+Running Cloud Service
+---------------------
 
-You can deploy **github-runners** as a service to a new Hetzner Cloud server instance
-using the **deploy** command.
+Instead of running **github-runners** program locally as a standalone application or as a service.
+You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
+
+See **-h, --help** for all the available commands.
 
 :✋ Note:
-   The options that are passed to the **github-runners <options> deploy** command
+   By default, the server name where the **github-runners** service will be running
+   is **github-runners**. If you want to use a custom server name, then
+   you must use the **cloud --name** option for any **cloud** commands.
+
+.. code-block:: bash
+
+   github-runners cloud -h
+
+::
+
+   usage: GitHub Actions runners scale up service cloud [-h] [-n server] command ...
+
+   Deploying and running application as a service on a cloud instance.
+
+   options:
+     -h, --help            show this help message and exit
+     -n server, --name server
+                           deployment server name, default: github-runners
+
+   commands:
+     command
+       deploy              deploy cloud service
+       logs                get cloud service logs
+       status              get cloud service status
+       start               start cloud service
+       stop                stop cloud service
+       install             install cloud service
+       uninstall           uninstall cloud service
+       upgrade             upgrade cloud service
+
+Deployment
+==========
+
+You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
+using the **cloud deploy** command.
+
+:✋ Note:
+   The options that are passed to the **github-runners <options> cloud deploy** command
    will be the same options with which the service will be executed.
 
 .. code-block:: bash
 
    export GITHUB_TOKEN=ghp_...
    export GITHUB_REPOSITORY=testflows/github-runners
    export HETZNER_TOKEN=GJzdc...
@@ -310,46 +430,191 @@
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
+The cloud instance that runs the **github-runners** service can either be x64 or ARM64 instance. By default, **cpx11**
+AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used.
+
+Using ARM64 Instance
+++++++++++++++++++++
+
+If you want to deploy the **github-runners** service to an ARM64 instance, then you must specify the instance
+type using the **--type** option.
+
+:✋ Note:
+   Currently Hetzner Cloud has ARM64 instances only available in Germany, Falkenstein (**fsn1**) location.
+
+For example, to use Ampere Altra, 4 vCPU, 8GB RAM shared-cpu ARM64 instance, you must specify **cax21**
+as the value of the **--type** as follows:
+
+.. code-block:: bash
+
+   github-runners deploy --location fsn1 --type cax21 --image ubuntu-22.04
+
+Using x64 Instance
+++++++++++++++++++
+
+By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
+a different x64 instance then specify desired type using the **--type** option.
+
+Cloud Service Logs
+===================
+
+You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
+Specify **-f, --follow** if you want to follow the logs journal.
+
+For example,
+
+:dump the full log:
+
+   .. code-block:: bash
+
+      github-runners cloud logs
+
+:follow the logs journal:
+
+   .. code-block:: bash
+
+      github-runners cloud logs -f
+
+
+Cloud Service Status
+=====================
+
+You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
+
+For example,
+
+.. code-block:: bash
+
+   github-runners cloud status
+
+Stopping Cloud Service
+======================
+
+You can manually stop the **github-runners** service running on a cloud instance using the **github-runners cloud stop** command.
+
+.. code-block:: bash
+
+   github-runners cloud stop
+
+Starting Cloud Service
+======================
+
+You can manually start the **github-runners** service running on a cloud instance after it was being manually stopped
+using the **github-runners cloud start** command.
+
+.. code-block:: bash
+
+   github-runners cloud start
+
+Installing Cloud Service
+========================
+
+You can manually force installation of the **github-runners** service running on a cloud instance using
+the **github-runners cloud install** command.
+
+:✋ Note:
+   Just like with the `github-runners <options> service install` command,
+   the options that are passed to the `github-runners <options> cloud install` command
+   will be the same options with which the service will be executed.
+
+You can specify **-f, --force** option to force service re-installation if it is already installed.
+
+.. code-block:: bash
+
+   github-runners <options> cloud install -f
+
+
+Uninstalling Cloud Service
+==========================
+
+You can manually force uninstallation of the **github-runners** service running on a cloud instance using
+the **github-runners cloud uninstall** command.
+
+.. code-block:: bash
+
+   github-runners cloud uninstall
+
+Upgrading Cloud Service
+========================
+
+You can manually upgrade the **github-runners** service package running on a cloud instance using
+the **github-runners cloud upgrade** command.
+
+If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
+the specified version otherwise the version is upgraded to the latest available.
+
+:✋ Note:
+   The service is not re-installed during the package upgrade process.
+   Instead, it is stopped before the upgrade and then started back up
+   after the package upgrade is complete.
+
+.. code-block:: bash
+
+   github-runners cloud upgrade --version <version>
+
+Deleting Cloud Service
+======================
+
+You can delete the **github-runners** cloud service and the cloud instance that is running on using
+the **github-runners cloud delete** command.
+
+The **cloud delete** command, deletes the cloud service by first stopping the service and then deleting the server instance.
+
+:❗Warning:
+   The default server name where the cloud service is deployed is **github-runners**.
+   Please make sure to specify the **cloud --name** option if you have deployed the service to a server with a different name.
+
+For example,
+
+:default name:
+   .. code-block:: bash
+
+      github-runners cloud delete
+
+:custom name:
+   .. code-block:: bash
+
+      github-runners cloud --name <custom_name> delete
 
 ------------------
 Scaling Up Runners
 ------------------
 
-The program scale up runners by looking for any jobs that have **queued** status.
+The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
    github-runner-{job.run_id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
-to be the same as the server name so that servers can deleted for any idle runner that for some reason
+to be the same as the server name so that servers can be deleted for any idle runner that for some reason
 does not pick up a job for which it was created within the **max-idle-runner-time** period.
 
 :Note:
    Given that the server name is fixed and specific for each *job.run_id*, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the the job with the exact **run_id** that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact **run_id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
-   equal the number of jobs and therefore under normal conditions all jobs will executed as expected.
+   equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 Maximum Number of Runners
 =========================
 
-By default, the maximum number of runners and therefore the maximum number if server instances is not set and therefore is unlimited.
+By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
 
 
@@ -357,40 +622,45 @@
 ==========
 
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
 :Server Type:
 
-   The default server type is **cx11**. However, a job **server-{hetzner-server-type}** label can be used to specify
-   custom server type. Where the **{hetzner-server-type}** must be a valid Hetzner Cloud server type name such as *cx11*, *cpx21* etc.
+   The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+
+   You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
+   The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+   server type name such as *cx11*, *cpx21* etc.
 
-   For example,
+   For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
+   as follows:
 
    .. code-block:: yaml
 
-       runs-on: [self-hosted, server-cpx21]
+      job-name:
+         runs-on: [self-hosted, server-cpx21]
 
 :SSH Access:
 
-   The server is configured to be accessed using *ssh* utility and the SSH public key path is specified either using the **--ssh-key**
+   The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :OS Image:
 
    The server is configured to have the OS image specified by the **--hetzner-image** option or the **HETZNER_IMAGE**
    environment variable.
 
 :Image Configuration:
-   Each new server instance is configured using `setup <#the-setup-script>`_ and `startup <#the-start-up-script>`_ scripts.
+   Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
 The Setup Script
 ================
 
-The **setup** script created and configures **runner** user that has **sudo** privileges.
+The **setup** script creates and configures **runner** user that has **sudo** privileges.
 
 :Setup:
 
    .. code-block:: bash
 
         set -x
 
@@ -568,31 +838,64 @@
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
 
-    * **deploy**
-      deploy application
+    * **cloud**
+      cloud service commands
 
-      * **-n, --name**
+      * **-n server, --name server**
         deployment server name, default: *github-runners*
 
-      * **-f, --force**
-        force deployment if already exist
+      * **deploy**
+        deploy cloud service
+
+        * **-f, --force**
+          force deployment if already exist
+
+        * **-l name, --location name**
+          deployment server location, default: *ash*
+
+        * **-t name, --type name**
+          deployment server type, default: *cpx11*
+
+        * **-i name, --image name**
+          deployment server image, default: *ubuntu-22.04*
+
+      * **logs**
+        get cloud service logs
+
+        * **-f, --follow**
+          follow logs journal, default: *False*
+
+      * **status**
+        get cloud service status
+
+      * **start**
+        start cloud service
+
+      * **stop**
+        stop cloud service
+
+      * **install**
+        install cloud service
+
+        * **-f, --force**
+          force installation if service already exists
 
-      * **-l name, --location name**
-        deployment server location, default: *ash*
+      * **uninstall**
+        uninstall cloud service
 
-      * **-t name, --type name**
-        deployment server type, default: *cpx11*
+      * **upgrade**
+        upgrade cloud service
 
-      * **-i name, --image name**
-        deployment server image, default: *ubuntu-22.04*
+        * **--version version**
+          package version, default: *the latest*
 
     * **service**
       service commands
 
       * **install**
         install service
```

### Comparing `testflows.github.runners-1.1.230725.1021905/setup.py` & `testflows.github.runners-1.1.230726.1014711/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.1.230725.1021905",
+    version="1.1.230726.1014711",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/__init__.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/__init__.py`

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
-__version__ = "1.1.230725.1021905"
+__version__ = "1.1.230726.1014711"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/actions.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/args.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/bin/github-runners`

 * *Files 24% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 
 from testflows.github.runners import __version__, __license__
 from testflows.github.runners.actions import Action
 from testflows.github.runners.scale_up import scale_up
 from testflows.github.runners.scale_down import scale_down
 from testflows.github.runners.scripts import Scripts, scripts
 from testflows.github.runners.args import check
-from testflows.github.runners.deploy import deploy
 
+import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
 
 logger = logging.getLogger("testflows.github.runners")
 
 description = """Auto-scaling GitHub Actions runners service using Hetzner Cloud.
 
     Service that starts and monitors queued up GitHub Actions workflows.
@@ -224,76 +224,215 @@
         default=False,
     )
 
     commands = parser.add_subparsers(
         title="commands", metavar="command", description=None, help=None
     )
 
-    deploy_parser = commands.add_parser(
-        "deploy",
-        help="deploy application",
-        description="Deploy application as a service to a cloud instance.",
+    cloud_parser = commands.add_parser(
+        "cloud",
+        help="cloud service commands",
+        description="Deploying and running application as a service on a cloud instance.",
         formatter_class=RawTextHelpFormatter,
     )
-    deploy_parser.add_argument(
+
+    cloud_parser.add_argument(
         "-n",
         "--name",
-        metavar="name",
+        metavar="server",
+        dest="server_name",
         type=str,
         help="deployment server name, default: github-runners",
         default="github-runners",
     )
-    deploy_parser.add_argument(
+
+    cloud_commands = cloud_parser.add_subparsers(
+        title="commands", metavar="command", description=None, help=None
+    )
+
+    cloud_commands.required = True
+
+    deploy_cloud_parser = cloud_commands.add_parser(
+        "deploy",
+        help="deploy cloud service",
+        description="Deploy application as a service to a new server instance.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    deploy_cloud_parser.add_argument(
         "-f",
         "--force",
         action="store_true",
         help="force deployment if already exist",
     )
-    deploy_parser.add_argument(
+
+    deploy_cloud_parser.add_argument(
         "-l",
         "--location",
         metavar="name",
         type=str,
         help="deployment server location, default: ash",
         default="ash",
     )
-    deploy_parser.add_argument(
+
+    deploy_cloud_parser.add_argument(
         "-t",
         "--type",
         metavar="name",
         type=str,
         help="deployment server type, default: cpx11",
         default="cpx11",
     )
-    deploy_parser.add_argument(
+
+    deploy_cloud_parser.add_argument(
         "-i",
         "--image",
         metavar="name",
         type=str,
         help="deployment server image, default: ubuntu-22.04",
         default="ubuntu-22.04",
     )
-    deploy_parser.set_defaults(func=deploy)
+
+    deploy_cloud_parser.set_defaults(func=cloud.deploy)
+
+    logs_cloud_parser = cloud_commands.add_parser(
+        "logs",
+        help="get cloud service logs",
+        description="Get cloud service logs.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    logs_cloud_parser.add_argument(
+        "-f",
+        "--follow",
+        action="store_true",
+        help="follow the logs journal",
+    )
+
+    logs_cloud_parser.set_defaults(func=cloud.logs)
+
+    status_cloud_parser = cloud_commands.add_parser(
+        "status",
+        help="get cloud service status",
+        description="Get cloud service status.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    status_cloud_parser.set_defaults(func=cloud.status)
+
+    start_cloud_parser = cloud_commands.add_parser(
+        "start",
+        help="start cloud service ",
+        description="Start cloud service.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    start_cloud_parser.set_defaults(func=cloud.start)
+
+    stop_cloud_parser = cloud_commands.add_parser(
+        "stop",
+        help="stop cloud service",
+        description="Stop cloud service.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    stop_cloud_parser.set_defaults(func=cloud.stop)
+
+    install_cloud_parser = cloud_commands.add_parser(
+        "install",
+        help="install cloud service",
+        description=(
+            "Install cloud service.\n\n"
+            "The `github-runners <options> service install` command will be executed on the cloud server instance.\n\n"
+            "Note: Just like with the `github-runners <options> service install` command,\n"
+            "      the options that are passed to the `github-runners <options> cloud install` command\n"
+            "      will be the same options with which the service will be executed."
+        ),
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    install_cloud_parser.add_argument(
+        "-f",
+        "--force",
+        action="store_true",
+        help="force service install",
+        default=False,
+    )
+
+    install_cloud_parser.set_defaults(func=cloud.install)
+
+    uninstall_cloud_parser = cloud_commands.add_parser(
+        "uninstall",
+        help="uninstall cloud service",
+        description="Uninstall cloud service.",
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    uninstall_cloud_parser.set_defaults(func=cloud.uninstall)
+
+    upgrade_cloud_parser = cloud_commands.add_parser(
+        "upgrade",
+        help="upgrade cloud service",
+        description=(
+            "Upgrade cloud service application.\n\n"
+            "If specific '--version' is specified then the `testflows.github.runners`\n"
+            "package is upgraded to the specified version otherwise the version is\n"
+            "upgraded to the latest available.\n\n"
+            "Note: The service is not re-installed during the package upgrade process.\n"
+            "      Instead, it is stopped before the upgrade and then started back up\n"
+            "      after the package upgrade is complete."
+        ),
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    upgrade_cloud_parser.add_argument(
+        "--version",
+        type=str,
+        metavar="version",
+        dest="upgrade_version",
+        help="package version, default: the latest",
+    )
+
+    upgrade_cloud_parser.set_defaults(func=cloud.upgrade)
+
+    delete_cloud_parser = cloud_commands.add_parser(
+        "delete",
+        help="delete cloud service",
+        description=(
+            "Delete cloud service.\n\n"
+            "Deletes `github-runners` service running on the cloud server instance\n"
+            "by first stopping the service and then deleting the server."
+        ),
+        formatter_class=RawTextHelpFormatter,
+    )
+
+    delete_cloud_parser.set_defaults(func=cloud.delete)
 
     service_parser = commands.add_parser(
         "service",
         help="service commands",
         description="Service commands.",
         formatter_class=RawTextHelpFormatter,
     )
 
     service_commands = service_parser.add_subparsers(
         title="commands", metavar="command", description=None, help=None
     )
+
     service_commands.required = True
 
     install_service_parser = service_commands.add_parser(
         "install",
         help="install",
-        description="Install service.",
+        description=(
+            "Install service.\n\n"
+            "The `/etc/systemd/system/github-runners.service` file will be created and service will be started.\n\n"
+            "Note: The options that are passed to the `github-runners <options> service install` command\n"
+            "      will be the same options with which the service will be executed."
+        ),
         formatter_class=RawTextHelpFormatter,
     )
     install_service_parser.add_argument(
         "-f",
         "--force",
         action="store_true",
         help="force service install",
```

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/request.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/server.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/service.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         os.system(f"sudo rm -f {SERVICE}")
 
     with Action("Reloading systemd"):
         os.system("sudo systemctl daemon-reload")
 
 
 def logs(args):
-    """Get service logs"""
+    """Get service logs."""
     os.system(
         f'sudo bash -c "journalctl -u {NAME}.service'
         + (" -f" if args.follow else "")
         + ' | tee"'
     )
```

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows/github/runners/shell.py` & `testflows.github.runners-1.1.230726.1014711/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.1.230725.1021905
+Version: 1.1.230726.1014711
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -122,14 +122,78 @@
 
 or you can specify these values using the following options:
 
 * **--github-token**
 * **--github-repository**
 * **--hetzner-token**
 
+-----------------
+Using x64 Runners
+-----------------
+
+The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+
+You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
+The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+server type name such as *cx11*, *cpx21* etc.
+
+For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
+as follows:
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, server-cpx21]
+
+-------------------
+Using ARM64 Runners
+-------------------
+
+The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+Therefore, in order to use ARM64 runners you must specify ARM64 server instance type by using the **server-{hetzner-server-type}** runner label.
+The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+server type name such as *cax11*, *cax21* etc. which correspond to the Ampere Altra, 2 vCPU, 4GB RAM and
+4 vCPU, 8GB RAM shared-cpu ARM64 instances respectively.
+
+For example, to use Ampere Altra, 4 vCPU, 8GB RAM shared-cpu ARM64 instance, you must define the **runs-on**
+as follows:
+
+.. code-block:: yaml
+
+   job-name:
+      runs-on: [self-hosted, server-cax21]
+
+-------
+SSH Key
+-------
+
+All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
+using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
+
+The SSH key will be automatically added to your project using the MD5 hash of the public key as the SSH key name.
+
+:❗Warning:
+   Given that each new SSH key is automatically added to your Hetzner project, you must manually delete them when no longer needed.
+
+Most GitHub users already have an SSH key associated with the account. If you want to know how to add an SSH key, see `Adding a new SSH key to your GitHub account    <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account>`_ article.
+
+Generating New SSH Key
+=======================
+
+If you need to generate a new SSH key, see `Generating a new SSH key and adding it to the ssh-agent <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>`_ article.
+
+Cloud Deployment
+================
+
+If you are deploying the **github-runners** program as a cloud service using the **github-runners <options> cloud deploy** command, then
+after provisoning a new cloud server instance that will host the **github-runners** service, a new SSH key will be
+auto-generated to access the runners. The auto-generated key will be placed in */home/runner/.ssh/id_rsa*, where **runner**
+is the user under which the **github-runners** service runs on the cloud instance. The auto-generated SSH key will be automatically
+added to your project using the MD5 hash of the public key as the SSH key name.
+
 -----------------------
 Running as a Service
 -----------------------
 
 You can run **github-runners** as a service.
 
 :✋ Note:
@@ -293,23 +357,62 @@
       Jul 24 14:24:42 user-node env[62771]: LANGUAGE=en_CA:en
       Jul 24 14:24:42 user-node env[62771]: PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/snap/bin
       Jul 24 14:24:42 user-node env[62771]: INVOCATION_ID=dc7b778f95fa4ccf95e4a4592b50d9e1
       Jul 24 14:24:42 user-node env[62771]: JOURNAL_STREAM=8:328542
       Jul 24 14:24:42 user-node env[62771]: SYSTEMD_EXEC_PID=62771
       ...
 
------------------------
-Deploying Application
------------------------
+---------------------
+Running Cloud Service
+---------------------
+
+Instead of running **github-runners** program locally as a standalone application or as a service.
+You can easily deploy **github-runners** to run on a Hetzner Cloud instance.
+
+See **-h, --help** for all the available commands.
+
+:✋ Note:
+   By default, the server name where the **github-runners** service will be running
+   is **github-runners**. If you want to use a custom server name, then
+   you must use the **cloud --name** option for any **cloud** commands.
+
+.. code-block:: bash
 
-You can deploy **github-runners** as a service to a new Hetzner Cloud server instance
-using the **deploy** command.
+   github-runners cloud -h
+
+::
+
+   usage: GitHub Actions runners scale up service cloud [-h] [-n server] command ...
+
+   Deploying and running application as a service on a cloud instance.
+
+   options:
+     -h, --help            show this help message and exit
+     -n server, --name server
+                           deployment server name, default: github-runners
+
+   commands:
+     command
+       deploy              deploy cloud service
+       logs                get cloud service logs
+       status              get cloud service status
+       start               start cloud service
+       stop                stop cloud service
+       install             install cloud service
+       uninstall           uninstall cloud service
+       upgrade             upgrade cloud service
+
+Deployment
+==========
+
+You can deploy **github-runners** as a service to a new Hetzner Cloud server instance, that will be created for you automatically,
+using the **cloud deploy** command.
 
 :✋ Note:
-   The options that are passed to the **github-runners <options> deploy** command
+   The options that are passed to the **github-runners <options> cloud deploy** command
    will be the same options with which the service will be executed.
 
 .. code-block:: bash
 
    export GITHUB_TOKEN=ghp_...
    export GITHUB_REPOSITORY=testflows/github-runners
    export HETZNER_TOKEN=GJzdc...
@@ -327,46 +430,191 @@
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
+The cloud instance that runs the **github-runners** service can either be x64 or ARM64 instance. By default, **cpx11**
+AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used.
+
+Using ARM64 Instance
+++++++++++++++++++++
+
+If you want to deploy the **github-runners** service to an ARM64 instance, then you must specify the instance
+type using the **--type** option.
+
+:✋ Note:
+   Currently Hetzner Cloud has ARM64 instances only available in Germany, Falkenstein (**fsn1**) location.
+
+For example, to use Ampere Altra, 4 vCPU, 8GB RAM shared-cpu ARM64 instance, you must specify **cax21**
+as the value of the **--type** as follows:
+
+.. code-block:: bash
+
+   github-runners deploy --location fsn1 --type cax21 --image ubuntu-22.04
+
+Using x64 Instance
+++++++++++++++++++
+
+By default, the **cpx11** AMD, 2 vCPU, 2GB RAM, shared-cpu x64 instance type is used. If you want to use
+a different x64 instance then specify desired type using the **--type** option.
+
+Cloud Service Logs
+===================
+
+You can check logs for the **github-runners** service running on a cloud instance using the **github-runners cloud logs** command.
+Specify **-f, --follow** if you want to follow the logs journal.
+
+For example,
+
+:dump the full log:
+
+   .. code-block:: bash
+
+      github-runners cloud logs
+
+:follow the logs journal:
+
+   .. code-block:: bash
+
+      github-runners cloud logs -f
+
+
+Cloud Service Status
+=====================
+
+You can check the status of the **github-runners** service running on a cloud instance using the **github-runners cloud status** command.
+
+For example,
+
+.. code-block:: bash
+
+   github-runners cloud status
+
+Stopping Cloud Service
+======================
+
+You can manually stop the **github-runners** service running on a cloud instance using the **github-runners cloud stop** command.
+
+.. code-block:: bash
+
+   github-runners cloud stop
+
+Starting Cloud Service
+======================
+
+You can manually start the **github-runners** service running on a cloud instance after it was being manually stopped
+using the **github-runners cloud start** command.
+
+.. code-block:: bash
+
+   github-runners cloud start
+
+Installing Cloud Service
+========================
+
+You can manually force installation of the **github-runners** service running on a cloud instance using
+the **github-runners cloud install** command.
+
+:✋ Note:
+   Just like with the `github-runners <options> service install` command,
+   the options that are passed to the `github-runners <options> cloud install` command
+   will be the same options with which the service will be executed.
+
+You can specify **-f, --force** option to force service re-installation if it is already installed.
+
+.. code-block:: bash
+
+   github-runners <options> cloud install -f
+
+
+Uninstalling Cloud Service
+==========================
+
+You can manually force uninstallation of the **github-runners** service running on a cloud instance using
+the **github-runners cloud uninstall** command.
+
+.. code-block:: bash
+
+   github-runners cloud uninstall
+
+Upgrading Cloud Service
+========================
+
+You can manually upgrade the **github-runners** service package running on a cloud instance using
+the **github-runners cloud upgrade** command.
+
+If specific '--version' is specified then the *testflows.github.runners* package is upgraded to
+the specified version otherwise the version is upgraded to the latest available.
+
+:✋ Note:
+   The service is not re-installed during the package upgrade process.
+   Instead, it is stopped before the upgrade and then started back up
+   after the package upgrade is complete.
+
+.. code-block:: bash
+
+   github-runners cloud upgrade --version <version>
+
+Deleting Cloud Service
+======================
+
+You can delete the **github-runners** cloud service and the cloud instance that is running on using
+the **github-runners cloud delete** command.
+
+The **cloud delete** command, deletes the cloud service by first stopping the service and then deleting the server instance.
+
+:❗Warning:
+   The default server name where the cloud service is deployed is **github-runners**.
+   Please make sure to specify the **cloud --name** option if you have deployed the service to a server with a different name.
+
+For example,
+
+:default name:
+   .. code-block:: bash
+
+      github-runners cloud delete
+
+:custom name:
+   .. code-block:: bash
+
+      github-runners cloud --name <custom_name> delete
 
 ------------------
 Scaling Up Runners
 ------------------
 
-The program scale up runners by looking for any jobs that have **queued** status.
+The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
    github-runner-{job.run_id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
-to be the same as the server name so that servers can deleted for any idle runner that for some reason
+to be the same as the server name so that servers can be deleted for any idle runner that for some reason
 does not pick up a job for which it was created within the **max-idle-runner-time** period.
 
 :Note:
    Given that the server name is fixed and specific for each *job.run_id*, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the the job with the exact **run_id** that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact **run_id** that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
-   equal the number of jobs and therefore under normal conditions all jobs will executed as expected.
+   equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 Maximum Number of Runners
 =========================
 
-By default, the maximum number of runners and therefore the maximum number if server instances is not set and therefore is unlimited.
+By default, the maximum number of runners and therefore the maximum number of server instances is not set and therefore is unlimited.
 You can set the maximum number of runners using the **--max-runners** option.
 
 .. code-blocks::bash
 
    github-runners --max-runners 10
 
 
@@ -374,40 +622,45 @@
 ==========
 
 The new server is accessed using SSH. It boots up with the specified OS image and is configured using
 the **setup** and **startup** scripts.
 
 :Server Type:
 
-   The default server type is **cx11**. However, a job **server-{hetzner-server-type}** label can be used to specify
-   custom server type. Where the **{hetzner-server-type}** must be a valid Hetzner Cloud server type name such as *cx11*, *cpx21* etc.
+   The default server type is **cx11** which is an Intel, 1 vCPU, 2GB RAM shared-cpu x64 instance.
+
+   You can specify different x64 server instance type by using the **server-{hetzner-server-type}** runner label.
+   The **{hetzner-server-type}** must be a valid `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+   server type name such as *cx11*, *cpx21* etc.
 
-   For example,
+   For example, to use AMD, 3 vCPU, 4GB RAM shared-cpu x64 instance, you can define the **runs-on**
+   as follows:
 
    .. code-block:: yaml
 
-       runs-on: [self-hosted, server-cpx21]
+      job-name:
+         runs-on: [self-hosted, server-cpx21]
 
 :SSH Access:
 
-   The server is configured to be accessed using *ssh* utility and the SSH public key path is specified either using the **--ssh-key**
+   The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :OS Image:
 
    The server is configured to have the OS image specified by the **--hetzner-image** option or the **HETZNER_IMAGE**
    environment variable.
 
 :Image Configuration:
-   Each new server instance is configured using `setup <#the-setup-script>`_ and `startup <#the-start-up-script>`_ scripts.
+   Each new server instance is configured using the `setup <#the-setup-script>`_ and the `startup <#the-start-up-script>`_ scripts.
 
 The Setup Script
 ================
 
-The **setup** script created and configures **runner** user that has **sudo** privileges.
+The **setup** script creates and configures **runner** user that has **sudo** privileges.
 
 :Setup:
 
    .. code-block:: bash
 
         set -x
 
@@ -585,31 +838,64 @@
 * **--debug**
   enable debugging mode, default: *False*
 
 * **commands:**
 
   * *command*
 
-    * **deploy**
-      deploy application
+    * **cloud**
+      cloud service commands
 
-      * **-n, --name**
+      * **-n server, --name server**
         deployment server name, default: *github-runners*
 
-      * **-f, --force**
-        force deployment if already exist
+      * **deploy**
+        deploy cloud service
+
+        * **-f, --force**
+          force deployment if already exist
+
+        * **-l name, --location name**
+          deployment server location, default: *ash*
+
+        * **-t name, --type name**
+          deployment server type, default: *cpx11*
+
+        * **-i name, --image name**
+          deployment server image, default: *ubuntu-22.04*
+
+      * **logs**
+        get cloud service logs
+
+        * **-f, --follow**
+          follow logs journal, default: *False*
+
+      * **status**
+        get cloud service status
+
+      * **start**
+        start cloud service
+
+      * **stop**
+        stop cloud service
+
+      * **install**
+        install cloud service
+
+        * **-f, --force**
+          force installation if service already exists
 
-      * **-l name, --location name**
-        deployment server location, default: *ash*
+      * **uninstall**
+        uninstall cloud service
 
-      * **-t name, --type name**
-        deployment server type, default: *cpx11*
+      * **upgrade**
+        upgrade cloud service
 
-      * **-i name, --image name**
-        deployment server image, default: *ubuntu-22.04*
+        * **--version version**
+          package version, default: *the latest*
 
     * **service**
       service commands
 
       * **install**
         install service
```

### Comparing `testflows.github.runners-1.1.230725.1021905/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.1.230726.1014711/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 testflows.github.runners.egg-info/dependency_links.txt
 testflows.github.runners.egg-info/not-zip-safe
 testflows.github.runners.egg-info/requires.txt
 testflows.github.runners.egg-info/top_level.txt
 testflows/github/runners/__init__.py
 testflows/github/runners/actions.py
 testflows/github/runners/args.py
-testflows/github/runners/deploy.py
+testflows/github/runners/cloud.py
 testflows/github/runners/request.py
 testflows/github/runners/scale_down.py
 testflows/github/runners/scale_up.py
 testflows/github/runners/server.py
 testflows/github/runners/service.py
 testflows/github/runners/shell.py
 testflows/github/runners/bin/github-runners
```

