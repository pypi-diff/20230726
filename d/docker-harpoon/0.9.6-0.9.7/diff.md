# Comparing `tmp/docker-harpoon-0.9.6.tar.gz` & `tmp/docker-harpoon-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/docker-harpoon-0.9.6.tar", last modified: Fri Aug 10 01:40:06 2018, max compression
+gzip compressed data, was "dist/docker-harpoon-0.9.7.tar", last modified: Sat Aug 11 02:48:52 2018, max compression
```

## Comparing `docker-harpoon-0.9.6.tar` & `docker-harpoon-0.9.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-10 01:40:06.000000 docker-harpoon-0.9.6/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      273 2018-08-10 01:40:06.000000 docker-harpoon-0.9.6/PKG-INFO
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-10 01:40:06.000000 docker-harpoon-0.9.6/harpoon/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3281 2017-09-12 02:00:05.000000 docker-harpoon-0.9.6/harpoon/formatter.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-10 01:40:06.000000 docker-harpoon-0.9.6/harpoon/option_spec/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3314 2017-11-18 00:58:43.000000 docker-harpoon-0.9.6/harpoon/option_spec/command_objs.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/option_spec/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     5013 2017-07-19 05:29:11.000000 docker-harpoon-0.9.6/harpoon/option_spec/image_specs.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3559 2017-10-17 01:33:07.000000 docker-harpoon-0.9.6/harpoon/option_spec/authentication_objs.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    16753 2017-11-20 06:16:24.000000 docker-harpoon-0.9.6/harpoon/option_spec/harpoon_specs.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3391 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/option_spec/task_objs.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    27504 2017-11-18 01:26:14.000000 docker-harpoon-0.9.6/harpoon/option_spec/image_objs.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     8979 2017-07-31 04:57:28.000000 docker-harpoon-0.9.6/harpoon/option_spec/command_specs.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-10 01:40:06.000000 docker-harpoon-0.9.6/harpoon/dockerpty/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3200 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/dockerpty/tty.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    11170 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/dockerpty/io.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1039 2016-05-22 00:20:11.000000 docker-harpoon-0.9.6/harpoon/dockerpty/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     7161 2016-05-22 00:22:03.000000 docker-harpoon-0.9.6/harpoon/dockerpty/pty.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    12709 2017-07-19 05:29:11.000000 docker-harpoon-0.9.6/harpoon/collector.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    12461 2018-08-10 01:32:04.000000 docker-harpoon-0.9.6/harpoon/actions.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)       16 2018-08-10 01:34:30.000000 docker-harpoon-0.9.6/harpoon/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1497 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/task_finder.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1839 2017-09-12 02:00:29.000000 docker-harpoon-0.9.6/harpoon/errors.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-10 01:40:06.000000 docker-harpoon-0.9.6/harpoon/ship/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     4851 2018-08-10 01:25:56.000000 docker-harpoon-0.9.6/harpoon/ship/syncer.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    26735 2017-07-19 05:29:11.000000 docker-harpoon-0.9.6/harpoon/ship/runner.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-10 01:40:06.000000 docker-harpoon-0.9.6/harpoon/ship/builders/
--rw-r--r--   0 stephenmoore   (501) staff       (20)     8597 2017-07-19 05:29:11.000000 docker-harpoon-0.9.6/harpoon/ship/builders/persistence.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1986 2017-11-18 00:57:34.000000 docker-harpoon-0.9.6/harpoon/ship/builders/normal.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2649 2017-07-19 05:29:11.000000 docker-harpoon-0.9.6/harpoon/ship/builders/squashed.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/ship/builders/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1705 2017-07-19 05:29:11.000000 docker-harpoon-0.9.6/harpoon/ship/builders/base.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/ship/__init__.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     6874 2017-11-18 00:58:27.000000 docker-harpoon-0.9.6/harpoon/ship/builder.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)    15397 2018-07-31 05:43:10.000000 docker-harpoon-0.9.6/harpoon/ship/context.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1619 2017-07-19 05:29:11.000000 docker-harpoon-0.9.6/harpoon/ship/network.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1244 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/ship/progress_stream.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2544 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/layers.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2034 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/helpers.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     6411 2017-07-19 05:29:11.000000 docker-harpoon-0.9.6/harpoon/executor.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)     3453 2016-05-17 08:18:51.000000 docker-harpoon-0.9.6/harpoon/amazon.py
-drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-10 01:40:06.000000 docker-harpoon-0.9.6/docker_harpoon.egg-info/
--rw-r--r--   0 stephenmoore   (501) staff       (20)      273 2018-08-10 01:40:01.000000 docker-harpoon-0.9.6/docker_harpoon.egg-info/PKG-INFO
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1179 2018-08-10 01:40:06.000000 docker-harpoon-0.9.6/docker_harpoon.egg-info/SOURCES.txt
--rw-r--r--   0 stephenmoore   (501) staff       (20)       51 2018-08-10 01:40:01.000000 docker-harpoon-0.9.6/docker_harpoon.egg-info/entry_points.txt
--rw-r--r--   0 stephenmoore   (501) staff       (20)      282 2018-08-10 01:40:01.000000 docker-harpoon-0.9.6/docker_harpoon.egg-info/requires.txt
--rw-r--r--   0 stephenmoore   (501) staff       (20)        8 2018-08-10 01:40:01.000000 docker-harpoon-0.9.6/docker_harpoon.egg-info/top_level.txt
--rw-r--r--   0 stephenmoore   (501) staff       (20)        1 2018-08-10 01:40:01.000000 docker-harpoon-0.9.6/docker_harpoon.egg-info/dependency_links.txt
--rw-r--r--   0 stephenmoore   (501) staff       (20)     1264 2018-07-24 06:48:44.000000 docker-harpoon-0.9.6/setup.py
--rw-r--r--   0 stephenmoore   (501) staff       (20)       59 2018-08-10 01:40:06.000000 docker-harpoon-0.9.6/setup.cfg
--rw-r--r--   0 stephenmoore   (501) staff       (20)     2486 2016-10-03 04:46:38.000000 docker-harpoon-0.9.6/README.rst
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      315 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/PKG-INFO
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2486 2016-10-03 04:46:38.000000 docker-harpoon-0.9.7/README.rst
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/docker_harpoon.egg-info/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      315 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/docker_harpoon.egg-info/PKG-INFO
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1179 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/docker_harpoon.egg-info/SOURCES.txt
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        1 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/docker_harpoon.egg-info/dependency_links.txt
+-rw-r--r--   0 stephenmoore   (501) staff       (20)       51 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/docker_harpoon.egg-info/entry_points.txt
+-rw-r--r--   0 stephenmoore   (501) staff       (20)      251 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/docker_harpoon.egg-info/requires.txt
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        8 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/docker_harpoon.egg-info/top_level.txt
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/harpoon/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)       16 2018-08-11 02:24:27.000000 docker-harpoon-0.9.7/harpoon/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    12461 2018-08-10 01:32:04.000000 docker-harpoon-0.9.7/harpoon/actions.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3453 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/amazon.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    12709 2017-07-19 05:29:11.000000 docker-harpoon-0.9.7/harpoon/collector.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/harpoon/dockerpty/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1039 2016-05-22 00:20:11.000000 docker-harpoon-0.9.7/harpoon/dockerpty/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    11170 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/dockerpty/io.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     7161 2016-05-22 00:22:03.000000 docker-harpoon-0.9.7/harpoon/dockerpty/pty.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3200 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/dockerpty/tty.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1839 2017-09-12 02:00:29.000000 docker-harpoon-0.9.7/harpoon/errors.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     6411 2017-07-19 05:29:11.000000 docker-harpoon-0.9.7/harpoon/executor.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3281 2017-09-12 02:00:05.000000 docker-harpoon-0.9.7/harpoon/formatter.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2034 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/helpers.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2544 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/layers.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/harpoon/option_spec/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/option_spec/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2926 2018-08-11 02:24:26.000000 docker-harpoon-0.9.7/harpoon/option_spec/authentication_objs.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3314 2017-11-18 00:58:43.000000 docker-harpoon-0.9.7/harpoon/option_spec/command_objs.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     8979 2017-07-31 04:57:28.000000 docker-harpoon-0.9.7/harpoon/option_spec/command_specs.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    16813 2018-08-10 06:11:42.000000 docker-harpoon-0.9.7/harpoon/option_spec/harpoon_specs.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    27651 2018-08-10 06:13:50.000000 docker-harpoon-0.9.7/harpoon/option_spec/image_objs.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     5013 2017-07-19 05:29:11.000000 docker-harpoon-0.9.7/harpoon/option_spec/image_specs.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     3391 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/option_spec/task_objs.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/harpoon/ship/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/ship/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     7003 2018-08-11 01:59:59.000000 docker-harpoon-0.9.7/harpoon/ship/builder.py
+drwxr-xr-x   0 stephenmoore   (501) staff       (20)        0 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/harpoon/ship/builders/
+-rw-r--r--   0 stephenmoore   (501) staff       (20)        0 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/ship/builders/__init__.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1705 2017-07-19 05:29:11.000000 docker-harpoon-0.9.7/harpoon/ship/builders/base.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1958 2018-08-10 05:58:20.000000 docker-harpoon-0.9.7/harpoon/ship/builders/normal.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     8597 2017-07-19 05:29:11.000000 docker-harpoon-0.9.7/harpoon/ship/builders/persistence.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     2649 2017-07-19 05:29:11.000000 docker-harpoon-0.9.7/harpoon/ship/builders/squashed.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    15400 2018-08-10 06:25:22.000000 docker-harpoon-0.9.7/harpoon/ship/context.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1619 2017-07-19 05:29:11.000000 docker-harpoon-0.9.7/harpoon/ship/network.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1244 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/ship/progress_stream.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)    26756 2018-08-10 06:12:23.000000 docker-harpoon-0.9.7/harpoon/ship/runner.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     4851 2018-08-10 01:25:56.000000 docker-harpoon-0.9.7/harpoon/ship/syncer.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1497 2016-05-17 08:18:51.000000 docker-harpoon-0.9.7/harpoon/task_finder.py
+-rw-r--r--   0 stephenmoore   (501) staff       (20)       38 2018-08-11 02:48:52.000000 docker-harpoon-0.9.7/setup.cfg
+-rw-r--r--   0 stephenmoore   (501) staff       (20)     1178 2018-08-11 02:24:26.000000 docker-harpoon-0.9.7/setup.py
```

### Comparing `docker-harpoon-0.9.6/harpoon/formatter.py` & `docker-harpoon-0.9.7/harpoon/formatter.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/option_spec/command_objs.py` & `docker-harpoon-0.9.7/harpoon/option_spec/command_objs.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/option_spec/image_specs.py` & `docker-harpoon-0.9.7/harpoon/option_spec/image_specs.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/option_spec/authentication_objs.py` & `docker-harpoon-0.9.7/harpoon/option_spec/authentication_objs.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from harpoon.amazon import assume_role, decrypt_kms, get_s3_slip
 
 from input_algorithms.spec_base import NotSpecified
 from input_algorithms.dictobj import dictobj
 
-from google.auth.transport.urllib3 import _make_default_http, Request as GoogleAuthRequest
 from six.moves.urllib.parse import urlparse
-import google.auth
 import subprocess
 import urllib3
 import logging
 import time
 import six
 import os
 
@@ -27,27 +25,14 @@
                 authenticator = self.registries[registry]['writing']
             else:
                 authenticator = self.registries[registry]['reading']
 
             if authenticator is not NotSpecified:
                 username, password = authenticator.creds
 
-        elif "gcr.io" in registry:
-            # login doesn't seem to work when using docker-py :(
-            global_docker = True
-            credentials, project = google.auth.default(scopes=['https://www.googleapis.com/auth/cloud-platform'])
-
-            log.info("Making credentials to log into gcr.io")
-            http = _make_default_http()
-            request = GoogleAuthRequest(http)
-            credentials.refresh(request)
-
-            username = "oauth2accesstoken"
-            password = credentials.token
-
         if username is not None:
             if global_docker:
                 # First work out if docker login supports --email
                 # If it does we must supply it otherwise it will prompt the user for it
                 # If it doesn't support --email then we can't supply it....
                 process = subprocess.Popen(["docker", "login", "--help"], stdout=subprocess.PIPE)
                 out, _ = process.communicate()
```

### Comparing `docker-harpoon-0.9.6/harpoon/option_spec/harpoon_specs.py` & `docker-harpoon-0.9.7/harpoon/option_spec/harpoon_specs.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,16 @@
                 , extra_hosts = listof(string_spec())
                 , network_mode = defaulted(string_spec(), None)
                 , publish_all_ports = defaulted(boolean(), False)
                 )
 
             , cpu = create_spec(image_objs.Cpu
                 , cap_add = defaulted(listof(string_spec()), None)
-                , cpuset = defaulted(listof(string_spec()), None)
+                , cpuset_cpus = defaulted(string_spec(), None)
+                , cpuset_mems = defaulted(string_spec(), None)
                 , cap_drop = defaulted(listof(string_spec()), None)
                 , mem_limit = defaulted(integer_spec(), 0)
                 , cpu_shares = defaulted(integer_spec(), None)
                 , memswap_limit = defaulted(integer_spec(), 0)
                 )
 
             , devices = defaulted(listof(dictionary_spec()), None)
```

### Comparing `docker-harpoon-0.9.6/harpoon/option_spec/task_objs.py` & `docker-harpoon-0.9.7/harpoon/option_spec/task_objs.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/option_spec/image_objs.py` & `docker-harpoon-0.9.7/harpoon/option_spec/image_objs.py`

 * *Files 1% similar despite different names*

```diff
@@ -687,15 +687,16 @@
           "wait_condition": "Dictionary of image name to wait_conditions. These override wait conditions on the dependency itself"
         , ("attached", False): "Whether harpoon attaches to this container or not"
         }
 
 class Cpu(dictobj):
     """Cpu options"""
     fields = {
-          "cpuset": "cgroups Cpuset to use"
-        , "cap_add": "List of kernel capabilties to add to the container"
+          "cap_add": "List of kernel capabilties to add to the container"
         , "cap_drop": "List of kernel capabilties to drop from the container"
         , "mem_limit": "Memory limit in bytes"
         , "cpu_shares": "The CPU Shares for container (ie. the relative weight vs othercontainers)"
+        , "cpuset_cpus": "CPUs in which to allow execution (0-3, 0,1)."
+        , "cpuset_mems": "Memory nodes (MEMs) in which to allow execution (0-3, 0,1). Only effective on NUMA systems."
         , "memswap_limit": "Total memory usage (memory + swap); set -1 to disable swap"
         }
```

### Comparing `docker-harpoon-0.9.6/harpoon/option_spec/command_specs.py` & `docker-harpoon-0.9.7/harpoon/option_spec/command_specs.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/dockerpty/tty.py` & `docker-harpoon-0.9.7/harpoon/dockerpty/tty.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/dockerpty/io.py` & `docker-harpoon-0.9.7/harpoon/dockerpty/io.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/dockerpty/__init__.py` & `docker-harpoon-0.9.7/harpoon/dockerpty/__init__.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/dockerpty/pty.py` & `docker-harpoon-0.9.7/harpoon/dockerpty/pty.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/collector.py` & `docker-harpoon-0.9.7/harpoon/collector.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/actions.py` & `docker-harpoon-0.9.7/harpoon/actions.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/task_finder.py` & `docker-harpoon-0.9.7/harpoon/task_finder.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/errors.py` & `docker-harpoon-0.9.7/harpoon/errors.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/ship/syncer.py` & `docker-harpoon-0.9.7/harpoon/ship/syncer.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/ship/runner.py` & `docker-harpoon-0.9.7/harpoon/ship/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,14 +280,17 @@
             , extra_hosts = conf.network.extra_hosts
             , network_mode = conf.network.network_mode
             , publish_all_ports = conf.network.publish_all_ports
 
             , cap_add = conf.cpu.cap_add
             , cap_drop = conf.cpu.cap_drop
             , mem_limit = conf.cpu.mem_limit
+            , cpu_shares = conf.cpu.cpu_shares
+            , cpuset_cpus = conf.cpu.cpuset_cpus
+            , cpuset_mems = conf.cpu.cpuset_mems
             , memswap_limit = conf.cpu.memswap_limit
 
             , ulimits = conf.ulimits
             , read_only = conf.read_only_rootfs
             , log_config = conf.log_config
             , security_opt = conf.security_opt
 
@@ -302,22 +305,18 @@
             , environment=env
 
             , tty = False if no_tty_option else tty
             , user = conf.user
             , ports = ports
             , stdin_open = tty
 
-            , dns = conf.network.dns
             , hostname = conf.network.hostname
             , domainname = conf.network.domainname
             , network_disabled = conf.network.disabled
 
-            , cpuset = conf.cpu.cpuset
-            , cpu_shares = conf.cpu.cpu_shares
-
             , host_config = host_config
 
             , **conf.other_options.create
             )
 
         if isinstance(container_id, dict):
             if "errorDetail" in container_id:
```

### Comparing `docker-harpoon-0.9.6/harpoon/ship/builders/persistence.py` & `docker-harpoon-0.9.7/harpoon/ship/builders/persistence.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/ship/builders/normal.py` & `docker-harpoon-0.9.7/harpoon/ship/builders/normal.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,14 @@
         lines = conf.harpoon.docker_api.build(
               tag = image_name
             , fileobj = context.tmpfile
             , custom_context = True
 
             , rm = True
             , pull = False
-            , stream = True
             )
 
         for found in lines:
             for line in found.decode().split("\n"):
                 if line.strip():
                     try:
                         stream.feed(line.encode())
```

### Comparing `docker-harpoon-0.9.6/harpoon/ship/builders/squashed.py` & `docker-harpoon-0.9.7/harpoon/ship/builders/squashed.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/ship/builders/base.py` & `docker-harpoon-0.9.7/harpoon/ship/builders/base.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/ship/builder.py` & `docker-harpoon-0.9.7/harpoon/ship/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,18 @@
     def setup(self):
         self.last_line = ""
         self.current_action = ""
         self.current_container = None
 
     def interpret_line(self, line_detail):
         if "stream" in line_detail:
+            if line_detail["stream"].strip() == "":
+                self.add_line(line_detail["stream"])
+                return
+
             self.interpret_stream(line_detail["stream"])
             self.last_line = line_detail["stream"]
         elif "status" in line_detail:
             self.interpret_status(line_detail["status"])
             self.last_line = line_detail["status"]
         elif "aux" in line_detail:
             log.info("Created image\t%s", line_detail["aux"].get("ID", ""))
```

### Comparing `docker-harpoon-0.9.6/harpoon/ship/context.py` & `docker-harpoon-0.9.7/harpoon/ship/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                     try:
                         strm, stat = content["docker_api"].get_archive(content["conf"].container_id, content["path"])
                     except docker.errors.NotFound:
                         raise BadOption("Trying to get something from an image that don't exist!", path=content["path"], image=content["conf"].image_name)
                     else:
                         log.debug(stat)
 
-                        fo = BytesIO(strm.read())
+                        fo = BytesIO(b''.join(strm))
 
                         # In newer docker the archive is a gzipped archive
                         # But in older docker, it's a normal tar
                         for mode in ("r:gz", "r"):
                             try:
                                 tf = tarfile.open(fileobj=fo, mode=mode)
                                 break
```

### Comparing `docker-harpoon-0.9.6/harpoon/ship/network.py` & `docker-harpoon-0.9.7/harpoon/ship/network.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/ship/progress_stream.py` & `docker-harpoon-0.9.7/harpoon/ship/progress_stream.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/layers.py` & `docker-harpoon-0.9.7/harpoon/layers.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/helpers.py` & `docker-harpoon-0.9.7/harpoon/helpers.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/executor.py` & `docker-harpoon-0.9.7/harpoon/executor.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/harpoon/amazon.py` & `docker-harpoon-0.9.7/harpoon/amazon.py`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/docker_harpoon.egg-info/SOURCES.txt` & `docker-harpoon-0.9.7/docker_harpoon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `docker-harpoon-0.9.6/setup.py` & `docker-harpoon-0.9.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,39 +9,35 @@
 
     , install_requires =
       [ "delfick_app==0.9.5"
       , "option_merge==1.6"
       , "input_algorithms==0.6.0"
       , "option_merge_addons==0.2"
 
-      , "docker==2.5.1"
+      , "docker==3.5.0"
 
       , "six"
       , "glob2"
       , "humanize"
 
       , "boto3==1.4.4"
       , "pyYaml==3.13"
-      , "google-auth==1.0.2"
-
-      # google auth needs urllib3
-      , "urllib3==1.22"
       ]
 
     , extras_require =
       { "tests":
         [ "noseOfYeti>=1.7"
         , "nose"
         , "mock==1.0.1"
         , "nose-pattern-exclude"
         , "nose-focus==0.1.2"
         , "tox"
         ]
       , "git":
-        [ "gitmit==0.3"
+        [ "gitmit==0.4.1"
         ]
       }
 
     , entry_points =
       { 'console_scripts' :
         [ 'harpoon = harpoon.executor:main'
         ]
```

### Comparing `docker-harpoon-0.9.6/README.rst` & `docker-harpoon-0.9.7/README.rst`

 * *Files identical despite different names*

