# Comparing `tmp/testflows.github.runners-1.2.230726.1183012.tar.gz` & `tmp/testflows.github.runners-1.2.230726.1204416.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.2.230726.1183012.tar", last modified: Wed Jul 26 18:30:12 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.2.230726.1204416.tar", last modified: Wed Jul 26 20:44:17 2023, max compression
```

## Comparing `testflows.github.runners-1.2.230726.1183012.tar` & `testflows.github.runners-1.2.230726.1204416.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1183012/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    32718 2023-07-26 18:23:14.000000 testflows.github.runners-1.2.230726.1183012/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.299094 testflows.github.runners-1.2.230726.1183012/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.299094 testflows.github.runners-1.2.230726.1183012/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1121 2023-07-25 02:04:51.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    19676 2023-07-26 15:33:47.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)     8131 2023-07-26 16:23:24.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    10837 2023-07-26 18:29:40.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-25 02:12:04.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-24 22:14:55.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-24 01:28:32.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      714 2023-07-24 01:27:59.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     4770 2023-07-26 15:40:21.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1183012/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 18:30:12.303094 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    33310 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 18:30:12.000000 testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-24 01:44:49.000000 testflows.github.runners-1.2.230726.1204416/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    33617 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    33025 2023-07-26 20:43:15.000000 testflows.github.runners-1.2.230726.1204416/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2018 2023-07-26 20:44:16.000000 testflows.github.runners-1.2.230726.1204416/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-07-26 20:44:16.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      999 2023-07-25 00:04:07.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2030 2023-07-26 20:24:26.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    19878 2023-07-26 20:43:36.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)     8087 2023-07-26 20:32:03.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1894 2023-07-26 15:00:13.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8571 2023-07-25 01:13:14.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10823 2023-07-26 20:14:36.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1008 2023-07-24 12:06:14.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-24 22:39:23.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      397 2023-07-26 20:21:59.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      218 2023-07-26 20:22:26.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-26 20:22:42.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-26 20:23:06.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2206 2023-07-24 23:48:54.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4829 2023-07-26 20:28:21.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-26 15:50:50.000000 testflows.github.runners-1.2.230726.1204416/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-26 20:44:17.142964 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    33617 2023-07-26 20:44:17.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1000 2023-07-26 20:44:17.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-26 20:44:17.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-24 17:57:22.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2023-07-26 20:44:17.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-26 20:44:17.000000 testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.2.230726.1183012/LICENSE` & `testflows.github.runners-1.2.230726.1204416/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1183012/PKG-INFO` & `testflows.github.runners-1.2.230726.1204416/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1183012
+Version: 1.2.230726.1204416
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -190,23 +190,23 @@
 -----------------------
 Specifying Runner Image
 -----------------------
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
 
-You can also use the **image-{name}** runner label to specify server image for a specific job. Where **{name}** must be a valid
-Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*.
+You can also use the **image-{type}-{name}** runner label to specify server image for a specific job. Where the **{name}** must be a valid
+Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*, and the **{type}** is either *system*, *snapshot*, *backup*, or *app*.
 
 For example,
 
 .. code-block:: yaml
 
    job-name:
-      runs-on: [self-hosted, type-cx11, in-ash, image-ubuntu-20.04]
+      runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
 
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
@@ -452,24 +452,24 @@
       set -x
 
       apt-get update
 
       apt-get -y install python3-pip
       apt-get -y install openssh-client
 
-      echo "Create and configure runner user"
+      echo "Create and configure ubuntu user"
 
-      adduser runner --disabled-password --gecos ""
+      adduser ubuntu --disabled-password --gecos ""
       echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
       addgroup wheel
-      usermod -aG wheel runner
-      usermod -aG sudo runner
+      usermod -aG wheel ubuntu
+      usermod -aG sudo ubuntu
 
       echo "Generate SSH Key"
-      sudo -u runner ssh-keygen -t rsa -q -f "/home/runner/.ssh/id_rsa" -N ""
+      sudo -u ubuntu ssh-keygen -t rsa -q -f "/home/ubuntu/.ssh/id_rsa" -N ""
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
@@ -682,15 +682,15 @@
 :Server Location:
 
    The server location can bespecified by using the **--default-location** option or the **in-<name>** runner label.
    By default, location is not set as some server types are not available in some locations.
 
 :Image:
 
-   The server is configured to have the image specified by the **--default-image** option or the **image-<name>** runner label.
+   The server is configured to have the image specified by the **--default-image** option or the **image-{type}-{name}** runner label.
 
 :SSH Access:
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
@@ -703,21 +703,21 @@
 
 :Setup:
 
    .. code-block:: bash
 
         set -x
 
-        echo "Create and configure runner user"
+        echo "Create and configure ubuntu user"
 
-        adduser runner --disabled-password --gecos ""
+        adduser ubuntu --disabled-password --gecos ""
         echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
         addgroup wheel
-        usermod -aG wheel runner
-        usermod -aG sudo runner
+        usermod -aG wheel ubuntu
+        usermod -aG sudo ubuntu
 
 The Start-up Script
 ===================
 
 The **startup** script installs GitHub Actions runner. After installation it configures the runner to start in an *--ephemeral* mode.
 The *--ephemeral* mode causes the runner to exit as soon as it completes a job. After the runner exits the server is powered off.
 
@@ -725,15 +725,15 @@
 
 :x64:
 
    .. code-block:: bash
 
      set -x
      echo "Install runner"
-     cd /home/runner
+     cd /home/ubuntu
      curl -o actions-runner-linux-x64-2.306.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.306.0/actions-runner-linux-x64-2.306.0.tar.gz
      echo "b0a090336f0d0a439dac7505475a1fb822f61bbb36420c7b3b3fe6b1bdc4dbaa  actions-runner-linux-x64-2.306.0.tar.gz" | shasum -a 256 -c
      tar xzf ./actions-runner-linux-x64-2.306.0.tar.gz
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
 
@@ -745,15 +745,15 @@
 
 :ARM64:
 
    .. code-block:: bash
 
      set -x
      echo "Install runner"
-     cd /home/runner
+     cd /home/ubuntu
 
      curl -o actions-runner-linux-arm64-2.306.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.306.0/actions-runner-linux-arm64-2.306.0.tar.gz# Optional: Validate the hash
      echo "842a9046af8439aa9bcabfe096aacd998fc3af82b9afe2434ddd77b96f872a83  actions-runner-linux-arm64-2.306.0.tar.gz" | shasum -a 256 -c# Extract the installer
      tar xzf ./actions-runner-linux-arm64-2.306.0.tar.gz
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
@@ -838,22 +838,24 @@
 
 * **--hetzner-token HETZNER_TOKEN**
   Hetzner Cloud token, default: *$HETZNER_TOKEN* environment variable
 
 * **--ssh-key path**
   public SSH key file, default: *~/.ssh/id_rsa.pub*
 
-* **--default-type**
+* **--default-type name**
   default runner server type name, default: *cx11*
 
-* **--default-location**
+* **--default-location name**
   default runner server location name, default: not specified
 
-* **--default-image**
-  default runner server image name, default: *ubuntu-22.04*
+* **--default-image type:name**
+  default runner server image type and name,
+  where type is either: 'system','snapshot','backup','app',
+  default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
@@ -905,16 +907,18 @@
 
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
-        * **-i name, --image name**
-          deployment server image, default: *ubuntu-22.04*
+        * **-i type:name, --image type:name**
+          deployment server image type and name,
+          where the type is either: 'system','snapshot','backup','app',
+          default: *system:ubuntu-22.04*
 
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
           follow logs journal, default: *False*
```

### Comparing `testflows.github.runners-1.2.230726.1183012/README.rst` & `testflows.github.runners-1.2.230726.1204416/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -173,23 +173,23 @@
 -----------------------
 Specifying Runner Image
 -----------------------
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
 
-You can also use the **image-{name}** runner label to specify server image for a specific job. Where **{name}** must be a valid
-Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*.
+You can also use the **image-{type}-{name}** runner label to specify server image for a specific job. Where the **{name}** must be a valid
+Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*, and the **{type}** is either *system*, *snapshot*, *backup*, or *app*.
 
 For example,
 
 .. code-block:: yaml
 
    job-name:
-      runs-on: [self-hosted, type-cx11, in-ash, image-ubuntu-20.04]
+      runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
 
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
@@ -435,24 +435,24 @@
       set -x
 
       apt-get update
 
       apt-get -y install python3-pip
       apt-get -y install openssh-client
 
-      echo "Create and configure runner user"
+      echo "Create and configure ubuntu user"
 
-      adduser runner --disabled-password --gecos ""
+      adduser ubuntu --disabled-password --gecos ""
       echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
       addgroup wheel
-      usermod -aG wheel runner
-      usermod -aG sudo runner
+      usermod -aG wheel ubuntu
+      usermod -aG sudo ubuntu
 
       echo "Generate SSH Key"
-      sudo -u runner ssh-keygen -t rsa -q -f "/home/runner/.ssh/id_rsa" -N ""
+      sudo -u ubuntu ssh-keygen -t rsa -q -f "/home/ubuntu/.ssh/id_rsa" -N ""
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
@@ -665,15 +665,15 @@
 :Server Location:
 
    The server location can bespecified by using the **--default-location** option or the **in-<name>** runner label.
    By default, location is not set as some server types are not available in some locations.
 
 :Image:
 
-   The server is configured to have the image specified by the **--default-image** option or the **image-<name>** runner label.
+   The server is configured to have the image specified by the **--default-image** option or the **image-{type}-{name}** runner label.
 
 :SSH Access:
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
@@ -686,21 +686,21 @@
 
 :Setup:
 
    .. code-block:: bash
 
         set -x
 
-        echo "Create and configure runner user"
+        echo "Create and configure ubuntu user"
 
-        adduser runner --disabled-password --gecos ""
+        adduser ubuntu --disabled-password --gecos ""
         echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
         addgroup wheel
-        usermod -aG wheel runner
-        usermod -aG sudo runner
+        usermod -aG wheel ubuntu
+        usermod -aG sudo ubuntu
 
 The Start-up Script
 ===================
 
 The **startup** script installs GitHub Actions runner. After installation it configures the runner to start in an *--ephemeral* mode.
 The *--ephemeral* mode causes the runner to exit as soon as it completes a job. After the runner exits the server is powered off.
 
@@ -708,15 +708,15 @@
 
 :x64:
 
    .. code-block:: bash
 
      set -x
      echo "Install runner"
-     cd /home/runner
+     cd /home/ubuntu
      curl -o actions-runner-linux-x64-2.306.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.306.0/actions-runner-linux-x64-2.306.0.tar.gz
      echo "b0a090336f0d0a439dac7505475a1fb822f61bbb36420c7b3b3fe6b1bdc4dbaa  actions-runner-linux-x64-2.306.0.tar.gz" | shasum -a 256 -c
      tar xzf ./actions-runner-linux-x64-2.306.0.tar.gz
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
 
@@ -728,15 +728,15 @@
 
 :ARM64:
 
    .. code-block:: bash
 
      set -x
      echo "Install runner"
-     cd /home/runner
+     cd /home/ubuntu
 
      curl -o actions-runner-linux-arm64-2.306.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.306.0/actions-runner-linux-arm64-2.306.0.tar.gz# Optional: Validate the hash
      echo "842a9046af8439aa9bcabfe096aacd998fc3af82b9afe2434ddd77b96f872a83  actions-runner-linux-arm64-2.306.0.tar.gz" | shasum -a 256 -c# Extract the installer
      tar xzf ./actions-runner-linux-arm64-2.306.0.tar.gz
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
@@ -821,22 +821,24 @@
 
 * **--hetzner-token HETZNER_TOKEN**
   Hetzner Cloud token, default: *$HETZNER_TOKEN* environment variable
 
 * **--ssh-key path**
   public SSH key file, default: *~/.ssh/id_rsa.pub*
 
-* **--default-type**
+* **--default-type name**
   default runner server type name, default: *cx11*
 
-* **--default-location**
+* **--default-location name**
   default runner server location name, default: not specified
 
-* **--default-image**
-  default runner server image name, default: *ubuntu-22.04*
+* **--default-image type:name**
+  default runner server image type and name,
+  where type is either: 'system','snapshot','backup','app',
+  default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
@@ -888,16 +890,18 @@
 
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
-        * **-i name, --image name**
-          deployment server image, default: *ubuntu-22.04*
+        * **-i type:name, --image type:name**
+          deployment server image type and name,
+          where the type is either: 'system','snapshot','backup','app',
+          default: *system:ubuntu-22.04*
 
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
           follow logs journal, default: *False*
```

### Comparing `testflows.github.runners-1.2.230726.1183012/setup.py` & `testflows.github.runners-1.2.230726.1204416/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.2.230726.1183012",
+    version="1.2.230726.1204416",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/__init__.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/__init__.py`

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
-__version__ = "1.2.230726.1183012"
+__version__ = "1.2.230726.1204416"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/actions.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/args.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,26 +8,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import sys
+import os
 
+from collections import namedtuple
 
-def check(args):
-    """Check mandatory arguments."""
+Scripts = namedtuple("Scripts", "setup, startup_x64 startup_arm64")
 
-    def _check(name, value):
-        if value:
-            return
-        value = "is not defined"
-        print(
-            f"argument error: --{name.lower().replace('_','-')} {value}",
-            file=sys.stderr,
-        )
-        sys.exit(1)
+current_dir = os.path.dirname(__file__)
 
-    _check("GITHUB_TOKEN", args.github_token)
-    _check("GITHUB_REPOSITORY", args.github_repository)
-    _check("HETZNER_TOKEN", args.hetzner_token)
+scripts = Scripts(
+    setup=os.path.join(current_dir, "setup.sh"),
+    startup_x64=os.path.join(current_dir, "startup_x64.sh"),
+    startup_arm64=os.path.join(current_dir, "startup_arm64.sh"),
+)
```

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/bin/github-runners`

 * *Files 6% similar despite different names*

```diff
@@ -20,31 +20,32 @@
 import logging
 import threading
 
 from concurrent.futures import ThreadPoolExecutor, Future
 
 from hcloud import Client
 from hcloud.ssh_keys.domain import SSHKey
-from hcloud.images.domain import Image
 
 from github import Github
 from github.Repository import Repository
 
 from argparse import ArgumentParser, RawTextHelpFormatter, FileType
 
 from testflows.github.runners import __version__, __license__
 from testflows.github.runners.actions import Action
 from testflows.github.runners.scale_up import scale_up
 from testflows.github.runners.scale_down import scale_down
 from testflows.github.runners.scripts import Scripts, scripts
-from testflows.github.runners.args import check
 
+import testflows.github.runners.args as args
 import testflows.github.runners.cloud as cloud
 import testflows.github.runners.service as service
 
+check_args = args.check
+
 logger = logging.getLogger("testflows.github.runners")
 
 description = """Auto-scaling GitHub Actions runners service using Hetzner Cloud.
 
     Service that starts and monitors queued up GitHub Actions workflows.
     When a new job is queued up, it creates new Hetzner Cloud server instance
     that provides an ephemeral GitHub Actions runner. Server is automatically
@@ -53,31 +54,14 @@
 
     By default, uses `$GITHUB_TOKEN`, `$GITHUB_REPOSITORY`, and `$HETZNER_TOKEN`
     environment variables or you can specify these values `--github-token`,
     `--github-repository`, and `--hetzner-token` options.
 """
 
 
-def count(v):
-    """Count argument type."""
-    v = int(v)
-    assert v >= 1
-    return v
-
-
-def env_var(name):
-    """Environment variable type."""
-
-    def option(v):
-        v = v if v else os.getenv(name)
-        return v
-
-    return option
-
-
 def argparser():
     """Command line argument parser."""
 
     parser = ArgumentParser(
         "GitHub Actions runners scale up service",
         description=description,
         formatter_class=RawTextHelpFormatter,
@@ -90,29 +74,29 @@
         action="version",
         help="show program's license and exit",
         version=f"{__license__}",
     )
 
     parser.add_argument(
         "--github-token",
-        type=env_var("GITHUB_TOKEN"),
+        type=args.env_var_type("GITHUB_TOKEN"),
         help="GitHub token, default: $GITHUB_TOKEN environment variable",
         default="",
     )
 
     parser.add_argument(
         "--github-repository",
-        type=env_var("GITHUB_REPOSITORY"),
+        type=args.env_var_type("GITHUB_REPOSITORY"),
         help="GitHub repository, default: $GITHUB_REPOSITORY environment variable",
         default="",
     )
 
     parser.add_argument(
         "--hetzner-token",
-        type=env_var("HETZNER_TOKEN"),
+        type=args.env_var_type("HETZNER_TOKEN"),
         help="Hetzner Cloud token, default: $HETZNER_TOKEN environment variable",
         default="",
     )
 
     parser.add_argument(
         "--ssh-key",
         metavar="path",
@@ -121,49 +105,50 @@
         default=os.path.expanduser("~/.ssh/id_rsa.pub"),
     )
 
     parser.add_argument(
         "-m",
         "--max-runners",
         metavar="count",
-        type=count,
+        type=args.count_type,
         help="maximum number of active runners, default: unlimited",
     )
 
     parser.add_argument(
         "--default-image",
-        metavar="name",
+        metavar="type:name",
+        type=args.image_type,
         help=(
-            "default runner server image name, default: ubuntu-22.04"
+            "default runner server image type and name,"
+            "where the type is either: 'system','snapshot','backup','app',\n"
+            "default: system:ubuntu-22.04"
         ),
-        default="ubuntu-22.04",
+        default="system:ubuntu-22.04",
     )
 
     parser.add_argument(
         "--default-type",
         metavar="name",
-        help=(
-            "default runner server type name, default: cx11"
-        ),
+        type=args.server_type,
+        help=("default runner server type name, default: cx11"),
         default="cx11",
     )
 
     parser.add_argument(
         "--default-location",
         metavar="name",
-        help=(
-            "default runner server location name, by default not specified"
-        ),
+        type=args.location_type,
+        help=("default runner server location name, by default not specified"),
     )
 
     parser.add_argument(
         "-w",
         "--workers",
         metavar="count",
-        type=count,
+        type=args.count_type,
         help="number of concurrent workers, default: 10",
         default=10,
     )
 
     parser.add_argument(
         "--logger-config",
         metavar="path",
@@ -191,47 +176,47 @@
         type=str,
         help="path to custom ARM64 server startup script",
     )
 
     parser.add_argument(
         "--max-powered-off-time",
         metavar="sec",
-        type=count,
+        type=args.count_type,
         help="maximum time after which a powered off server is deleted, default: 20 sec",
         default=20,
     )
 
     parser.add_argument(
         "--max-idle-runner-time",
         metavar="sec",
-        type=count,
+        type=args.count_type,
         help="maximum time after which an idle runner is removed and its server deleted, default: 120 sec",
         default=120,
     )
 
     parser.add_argument(
         "--max-runner-registration-time",
         metavar="sec",
-        type=count,
+        type=args.count_type,
         help="maximum time after which the server will be deleted if it fails to register a runner, default: 60 sec",
         default=60,
     )
 
     parser.add_argument(
         "--scale-up-interval",
         metavar="sec",
-        type=count,
+        type=args.count_type,
         help="scale up service interval, default: 10 sec",
         default=10,
     )
 
     parser.add_argument(
         "--scale-down-interval",
         metavar="sec",
-        type=count,
+        type=args.count_type,
         help="scale down service interval, default: 10 sec",
         default=10,
     )
 
     parser.add_argument(
         "--debug",
         action="store_true",
@@ -280,35 +265,39 @@
         help="force deployment if already exist",
     )
 
     deploy_cloud_parser.add_argument(
         "-l",
         "--location",
         metavar="name",
-        type=str,
+        type=args.location_type,
         help="deployment server location, default: ash",
         default="ash",
     )
 
     deploy_cloud_parser.add_argument(
         "-t",
         "--type",
         metavar="name",
-        type=str,
+        type=args.server_type,
         help="deployment server type, default: cpx11",
         default="cpx11",
     )
 
     deploy_cloud_parser.add_argument(
         "-i",
         "--image",
-        metavar="name",
-        type=str,
-        help="deployment server image, default: ubuntu-22.04",
-        default="ubuntu-22.04",
+        metavar="type:name",
+        type=args.image_type,
+        help=(
+            "deployment server image type and name,\n"
+            "where the type is either: 'system','snapshot','backup','app',\n"
+            "default: system:ubuntu-22.04"
+        ),
+        default="system:ubuntu-22.04",
     )
 
     deploy_cloud_parser.set_defaults(func=cloud.deploy)
 
     logs_cloud_parser = cloud_commands.add_parser(
         "logs",
         help="get cloud service logs",
@@ -638,13 +627,13 @@
                 raise
         except BaseException as exc:
             if args.debug:
                 raise
             logger.fatal(f"❗ Error: {exc}")
 
     else:
-        check(args)
+        check_args(args)
 
         with ThreadPoolExecutor(
             max_workers=args.workers + 2, thread_name_prefix="worker"
         ) as worker_pool:
             main(args=args, scripts=scripts, worker_pool=worker_pool)
```

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/cloud.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,17 +58,17 @@
         if not client.ssh_keys.get_by_name(name=ssh_key.name):
             with Action(f"Creating SSH key {ssh_key.name}"):
                 client.ssh_keys.create(name=ssh_key.name, public_key=ssh_key.public_key)
 
     with Action(f"Creating new server"):
         response = client.servers.create(
             name=server_name,
-            server_type=ServerType(name=args.type),
-            image=Image(name=args.image),
-            location=Location(name=args.location),
+            server_type=args.type,
+            image=args.image,
+            location=args.location,
             ssh_keys=[ssh_key],
         )
         server: BoundServer = response.server
 
     with Action(f"Waiting for server to be ready") as action:
         wait_ready(server=server, timeout=timeout, action=action)
 
@@ -80,15 +80,15 @@
             server,
             f"bash -s  < {os.path.join(current_dir, 'scripts', 'deploy', 'setup.sh')}",
         )
 
     with Action("Installing github-runners"):
         ssh(
             server,
-            f"'sudo -u runner pip3 install testflows.github.runners=={__version__}'",
+            f"'sudo -u ubuntu pip3 install testflows.github.runners=={__version__}'",
         )
 
     install(args, server=server)
 
 
 def install(args, server: BoundServer = None):
     """Install service on a cloud instance."""
@@ -100,15 +100,15 @@
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=args.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Installing service"):
-        command = f"\"su - runner -c '"
+        command = f"\"su - ubuntu -c '"
         command += f"GITHUB_TOKEN={args.github_token} "
         command += f"GITHUB_REPOSITORY={args.github_repository} "
         command += f"HETZNER_TOKEN={args.hetzner_token} "
 
         command += "github-runners"
         command += command_options(args)
         command += " service install -f'\""
@@ -129,21 +129,21 @@
 
     stop(args, server=server)
 
     if upgrade_version:
         with Action(f"Upgrading github-runners to version {upgrade_version}"):
             ssh(
                 server,
-                f"'sudo -u runner pip3 install testflows.github.runners=={upgrade_version}'",
+                f"'sudo -u ubuntu pip3 install testflows.github.runners=={upgrade_version}'",
             )
     else:
         with Action(f"Upgrading github-runners the latest version"):
             ssh(
                 server,
-                f"'sudo -u runner pip3 install --upgrade testflows.github.runners'",
+                f"'sudo -u ubuntu pip3 install --upgrade testflows.github.runners'",
             )
 
     start(args, server=server)
 
 
 def uninstall(args):
     """Uninstall github-runners service from a cloud instance."""
@@ -152,15 +152,15 @@
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=args.hetzner_token)
 
     with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Uninstalling service"):
-        command = f"\"su - runner -c 'github-runners service uninstall'\""
+        command = f"\"su - ubuntu -c 'github-runners service uninstall'\""
         ssh(server, command)
 
 
 def delete(args):
     """Delete github-runners service running
     on Hetzner server instance by stopping the service
     and deleting the server."""
@@ -169,15 +169,15 @@
     with Action("Logging in to Hetzner Cloud"):
         client = Client(token=args.hetzner_token)
 
     with Action(f"Getting server {server_name}"):
         server: BoundServer = client.servers.get_by_name(server_name)
 
     with Action("Uninstalling service"):
-        command = f"\"su - runner -c 'github-runners service uninstall'\""
+        command = f"\"su - ubuntu -c 'github-runners service uninstall'\""
         ssh(server, command)
 
     with Action(f"Deleting server {server_name}"):
         server.delete()
 
 
 def logs(args, server: BoundServer = None):
@@ -191,15 +191,15 @@
         with Action(f"Getting server {server_name}"):
             server: BoundServer = client.servers.get_by_name(server_name)
 
     if server is None:
         raise ValueError("server not found")
 
     command = (
-        f"\"su - runner -c 'github-runners service logs"
+        f"\"su - ubuntu -c 'github-runners service logs"
         + (" -f" if args.follow else "")
         + "'\""
     )
     ssh(server, command, use_logger=False)
 
 
 def status(args, server: BoundServer = None):
@@ -210,15 +210,15 @@
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=args.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Getting status"):
-        command = f"\"su - runner -c 'github-runners service status'\""
+        command = f"\"su - ubuntu -c 'github-runners service status'\""
         ssh(server, command)
 
 
 def start(args, server: BoundServer = None):
     """Start cloud server service."""
     if server is None:
         server_name = args.server_name
@@ -226,15 +226,15 @@
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=args.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Starting service"):
-        command = f"\"su - runner -c 'github-runners service start'\""
+        command = f"\"su - ubuntu -c 'github-runners service start'\""
         ssh(server, command)
 
 
 def stop(args, server: BoundServer = None):
     """Stop cloud server service."""
     if server is None:
         server_name = args.server_name
@@ -242,9 +242,9 @@
         with Action("Logging in to Hetzner Cloud"):
             client = Client(token=args.hetzner_token)
 
         with Action(f"Getting server {server_name}"):
             server = client.servers.get_by_name(server_name)
 
     with Action("Stopping service"):
-        command = f"\"su - runner -c 'github-runners service stop'\""
+        command = f"\"su - ubuntu -c 'github-runners service stop'\""
         ssh(server, command)
```

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/request.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scale_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,62 +119,62 @@
         startup_script=startup_script,
         github_token=github_token,
         github_repository=github_repository,
         runner_labels=",".join(job.raw_data["labels"]),
     )
 
 
-def get_server_type(job: WorkflowJob, default: str, label_prefix="type-"):
+def get_server_type(job: WorkflowJob, default: ServerType, label_prefix="type-"):
     """Get server type for the specified job."""
     server_type = None
 
     if server_type is None:
         for label in job.raw_data["labels"]:
             if label.startswith(label_prefix):
                 server_type_name = label.split(label_prefix, 1)[-1].lower()
                 server_type = ServerType(name=server_type_name)
 
     if server_type is None:
-        server_type = ServerType(name=default)
+        server_type = default
 
     return server_type
 
 
-def get_server_location(job: WorkflowJob, default: str = "", label_prefix="in-"):
+def get_server_location(job: WorkflowJob, default: Location = None, label_prefix="in-"):
     """Get preferred server location for the specified job.
 
     By default, location is set to `None` to avoid server type mismatching
     the location as some server types are not available at some locations.
     """
     server_location: Location = None
 
     if server_location is None:
         for label in job.raw_data["labels"]:
             if label.startswith(label_prefix):
                 server_location_name = label.split(label_prefix, 1)[-1].lower()
                 server_location = Location(name=server_location_name)
 
     if server_location is None and default:
-        server_location = Location(name=default)
+        server_location = default
 
     return server_location
 
 
-def get_server_image(job: WorkflowJob, default: str, label_prefix="image-"):
+def get_server_image(job: WorkflowJob, default: Image, label_prefix="image-"):
     """Get preferred server image for the specified job."""
     server_image: Image = None
 
     if server_image is None:
         for label in job.raw_data["labels"]:
             if label.startswith(label_prefix):
                 server_image_name = label.split(label_prefix, 1)[-1].lower()
                 server_image = Image(name=server_image_name)
 
     if server_image is None:
-        server_image = Image(name=default)
+        server_image = default
 
     return server_image
 
 
 def get_startup_script(server_type: ServerType, scripts: Scripts):
     """Get startup script based on the requested server type.
     ARM64 servers type names start with "CA" prefix.
@@ -192,17 +192,17 @@
     repo: Repository,
     client: Client,
     scripts: Scripts,
     worker_pool: ThreadPoolExecutor,
     github_token: str,
     github_repository: str,
     ssh_key: SSHKey,
-    default_type: str,
-    default_location: str,
-    default_image: str,
+    default_type: ServerType,
+    default_location: Location,
+    default_image: Image,
     interval: int,
     max_servers: int,
 ):
     """Scale up service."""
 
     with ThreadPoolExecutor(
         max_workers=worker_pool._max_workers, thread_name_prefix=f"setup-worker"
```

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 set -x
 echo "Install runner"
-cd /home/runner
+cd /home/ubuntu
 
 curl -o actions-runner-linux-arm64-2.306.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.306.0/actions-runner-linux-arm64-2.306.0.tar.gz# Optional: Validate the hash
 echo "842a9046af8439aa9bcabfe096aacd998fc3af82b9afe2434ddd77b96f872a83  actions-runner-linux-arm64-2.306.0.tar.gz" | shasum -a 256 -c# Extract the installer
 tar xzf ./actions-runner-linux-arm64-2.306.0.tar.gz
 
 echo "Configure runner"
 ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
```

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/scripts/startup_x64.sh`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 set -x
 echo "Install runner"
-cd /home/runner
+cd /home/ubuntu
+
 curl -o actions-runner-linux-x64-2.306.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.306.0/actions-runner-linux-x64-2.306.0.tar.gz
 echo "b0a090336f0d0a439dac7505475a1fb822f61bbb36420c7b3b3fe6b1bdc4dbaa  actions-runner-linux-x64-2.306.0.tar.gz" | shasum -a 256 -c
 tar xzf ./actions-runner-linux-x64-2.306.0.tar.gz
 
 echo "Configure runner"
 ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
```

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/server.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/service.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,19 +28,21 @@
     --github-token
     --github-repository
     --hetzner-token
     --ssh-key
     """
     command = ""
     command += f" --workers {args.workers}"
-    command += f" --default-type {args.default_type}"
+    command += f" --default-type {args.default_type.name}"
     command += (
-        f" --default-location {args.default_location}" if args.default_location else ""
+        f" --default-location {args.default_location.name}"
+        if args.default_location
+        else None
     )
-    command += f" --default-image {args.default_image}"
+    command += f" --default-image {args.default_image.type}:{args.default_image.name}"
     command += f" --max-runners {args.max_runners}" if args.max_runners else ""
     command += f" --logger-config {args.logger_config}" if args.logger_config else ""
     command += f" --setup-script {args.setup_script}" if args.setup_script else ""
     command += (
         f" --startup-x64-script {args.startup_x64_script}"
         if args.startup_x64_script
         else ""
```

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows/github/runners/shell.py` & `testflows.github.runners-1.2.230726.1204416/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.2.230726.1183012
+Version: 1.2.230726.1204416
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -190,23 +190,23 @@
 -----------------------
 Specifying Runner Image
 -----------------------
 
 By default, the default image of the server for the runner is **ubuntu-22.04**. You can use the **--default-image**
 option to force specific default server image.
 
-You can also use the **image-{name}** runner label to specify server image for a specific job. Where **{name}** must be a valid
-Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*.
+You can also use the **image-{type}-{name}** runner label to specify server image for a specific job. Where the **{name}** must be a valid
+Hetzner Cloud image such as *ubuntu-22.04* or *ubuntu-20.04*, and the **{type}** is either *system*, *snapshot*, *backup*, or *app*.
 
 For example,
 
 .. code-block:: yaml
 
    job-name:
-      runs-on: [self-hosted, type-cx11, in-ash, image-ubuntu-20.04]
+      runs-on: [self-hosted, type-cx11, in-ash, image-system-ubuntu-20.04]
 
 -------
 SSH Key
 -------
 
 All server instances that are created are accessed via SSH using the **ssh** utility and therefore you must provide a valid SSH key
 using the **--ssh-key** option. If the **--ssh-key** option is no specified, then the *~/.ssh/id_rsa.pub* default key path will be used.
@@ -452,24 +452,24 @@
       set -x
 
       apt-get update
 
       apt-get -y install python3-pip
       apt-get -y install openssh-client
 
-      echo "Create and configure runner user"
+      echo "Create and configure ubuntu user"
 
-      adduser runner --disabled-password --gecos ""
+      adduser ubuntu --disabled-password --gecos ""
       echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
       addgroup wheel
-      usermod -aG wheel runner
-      usermod -aG sudo runner
+      usermod -aG wheel ubuntu
+      usermod -aG sudo ubuntu
 
       echo "Generate SSH Key"
-      sudo -u runner ssh-keygen -t rsa -q -f "/home/runner/.ssh/id_rsa" -N ""
+      sudo -u ubuntu ssh-keygen -t rsa -q -f "/home/ubuntu/.ssh/id_rsa" -N ""
 
 You can customize deployment server location, type, and image using the *--location*, *--type*, and *--image* options.
 
 .. code-block:: bash
 
    github-runners deploy --location nbg1 --type cx11 --image ubuntu-22.04
 
@@ -682,15 +682,15 @@
 :Server Location:
 
    The server location can bespecified by using the **--default-location** option or the **in-<name>** runner label.
    By default, location is not set as some server types are not available in some locations.
 
 :Image:
 
-   The server is configured to have the image specified by the **--default-image** option or the **image-<name>** runner label.
+   The server is configured to have the image specified by the **--default-image** option or the **image-{type}-{name}** runner label.
 
 :SSH Access:
 
    The server is configured to be accessed using *ssh* utility and the SSH public key path is specified using the **--ssh-key**
    option.
 
 :Image Configuration:
@@ -703,21 +703,21 @@
 
 :Setup:
 
    .. code-block:: bash
 
         set -x
 
-        echo "Create and configure runner user"
+        echo "Create and configure ubuntu user"
 
-        adduser runner --disabled-password --gecos ""
+        adduser ubuntu --disabled-password --gecos ""
         echo "%wheel   ALL=(ALL:ALL) NOPASSWD:ALL" >> /etc/sudoers
         addgroup wheel
-        usermod -aG wheel runner
-        usermod -aG sudo runner
+        usermod -aG wheel ubuntu
+        usermod -aG sudo ubuntu
 
 The Start-up Script
 ===================
 
 The **startup** script installs GitHub Actions runner. After installation it configures the runner to start in an *--ephemeral* mode.
 The *--ephemeral* mode causes the runner to exit as soon as it completes a job. After the runner exits the server is powered off.
 
@@ -725,15 +725,15 @@
 
 :x64:
 
    .. code-block:: bash
 
      set -x
      echo "Install runner"
-     cd /home/runner
+     cd /home/ubuntu
      curl -o actions-runner-linux-x64-2.306.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.306.0/actions-runner-linux-x64-2.306.0.tar.gz
      echo "b0a090336f0d0a439dac7505475a1fb822f61bbb36420c7b3b3fe6b1bdc4dbaa  actions-runner-linux-x64-2.306.0.tar.gz" | shasum -a 256 -c
      tar xzf ./actions-runner-linux-x64-2.306.0.tar.gz
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
 
@@ -745,15 +745,15 @@
 
 :ARM64:
 
    .. code-block:: bash
 
      set -x
      echo "Install runner"
-     cd /home/runner
+     cd /home/ubuntu
 
      curl -o actions-runner-linux-arm64-2.306.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.306.0/actions-runner-linux-arm64-2.306.0.tar.gz# Optional: Validate the hash
      echo "842a9046af8439aa9bcabfe096aacd998fc3af82b9afe2434ddd77b96f872a83  actions-runner-linux-arm64-2.306.0.tar.gz" | shasum -a 256 -c# Extract the installer
      tar xzf ./actions-runner-linux-arm64-2.306.0.tar.gz
 
      echo "Configure runner"
      ./config.sh --unattended --replace --url https://github.com/${GITHUB_REPOSITORY} --token ${GITHUB_RUNNER_TOKEN} --name "$(hostname)" --runnergroup "${GITHUB_RUNNER_GROUP}" --labels "${GITHUB_RUNNER_LABELS}" --work _work --ephemeral
@@ -838,22 +838,24 @@
 
 * **--hetzner-token HETZNER_TOKEN**
   Hetzner Cloud token, default: *$HETZNER_TOKEN* environment variable
 
 * **--ssh-key path**
   public SSH key file, default: *~/.ssh/id_rsa.pub*
 
-* **--default-type**
+* **--default-type name**
   default runner server type name, default: *cx11*
 
-* **--default-location**
+* **--default-location name**
   default runner server location name, default: not specified
 
-* **--default-image**
-  default runner server image name, default: *ubuntu-22.04*
+* **--default-image type:name**
+  default runner server image type and name,
+  where type is either: 'system','snapshot','backup','app',
+  default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *unlimited*
 
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
@@ -905,16 +907,18 @@
 
         * **-l name, --location name**
           deployment server location, default: *ash*
 
         * **-t name, --type name**
           deployment server type, default: *cpx11*
 
-        * **-i name, --image name**
-          deployment server image, default: *ubuntu-22.04*
+        * **-i type:name, --image type:name**
+          deployment server image type and name,
+          where the type is either: 'system','snapshot','backup','app',
+          default: *system:ubuntu-22.04*
 
       * **logs**
         get cloud service logs
 
         * **-f, --follow**
           follow logs journal, default: *False*
```

### Comparing `testflows.github.runners-1.2.230726.1183012/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.2.230726.1204416/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

