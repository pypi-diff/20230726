# Comparing `tmp/harlogger-3.0.0.tar.gz` & `tmp/harlogger-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlogger-3.0.0.tar", last modified: Sun Jul 16 15:30:35 2023, max compression
+gzip compressed data, was "harlogger-3.0.1.tar", last modified: Wed Jul 26 15:06:48 2023, max compression
```

## Comparing `harlogger-3.0.0.tar` & `harlogger-3.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:30:35.663331 harlogger-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-16 15:30:18.000000 harlogger-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46994 2023-07-16 15:30:35.663331 harlogger-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-16 15:30:18.000000 harlogger-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:30:35.663331 harlogger-3.0.0/harlogger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/haralyzer_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/http_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/sniffers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:30:35.663331 harlogger-3.0.0/harlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46994 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-16 15:30:18.000000 harlogger-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-16 15:30:18.000000 harlogger-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:30:35.663331 harlogger-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:06:48.511663 harlogger-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-26 15:06:33.000000 harlogger-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46994 2023-07-26 15:06:48.507663 harlogger-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-26 15:06:33.000000 harlogger-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:06:48.507663 harlogger-3.0.1/harlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:06:33.000000 harlogger-3.0.1/harlogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-26 15:06:33.000000 harlogger-3.0.1/harlogger/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 15:06:33.000000 harlogger-3.0.1/harlogger/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-26 15:06:33.000000 harlogger-3.0.1/harlogger/haralyzer_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-26 15:06:33.000000 harlogger-3.0.1/harlogger/http_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-26 15:06:33.000000 harlogger-3.0.1/harlogger/sniffers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:06:48.507663 harlogger-3.0.1/harlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46994 2023-07-26 15:06:48.000000 harlogger-3.0.1/harlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-26 15:06:48.000000 harlogger-3.0.1/harlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:06:48.000000 harlogger-3.0.1/harlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 15:06:48.000000 harlogger-3.0.1/harlogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 15:06:48.000000 harlogger-3.0.1/harlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 15:06:48.000000 harlogger-3.0.1/harlogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-26 15:06:33.000000 harlogger-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 15:06:33.000000 harlogger-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:06:48.511663 harlogger-3.0.1/setup.cfg
```

### Comparing `harlogger-3.0.0/LICENSE` & `harlogger-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `harlogger-3.0.0/PKG-INFO` & `harlogger-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harlogger
-Version: 3.0.0
+Version: 3.0.1
 Summary: Simple utlity for sniffing decrypted HTTP/HTTPS traffic on an iOS device (either jailbroken or not)
 Author-email: doronz88 <doron88@gmail.com>, netanelc305 <netanelc305@protonmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, netanelc305 <netanelc305@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `harlogger-3.0.0/README.md` & `harlogger-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `harlogger-3.0.0/harlogger/__main__.py` & `harlogger-3.0.1/harlogger/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 from pymobiledevice3.cli.cli_common import Command
-from pymobiledevice3.lockdown import LockdownClient
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
 
 from harlogger.sniffers import Filters, SnifferPreference, SnifferProfile
 
 
 @click.group()
 def cli():
     pass
@@ -15,41 +15,44 @@
 @click.option('--color/--no-color', default=True)
 @click.option('process_names', '-pn', '--process-name', multiple=True, help='filter process name list')
 @click.option('images', '-i', '--image', multiple=True, help='filter image list')
 @click.option('--request/--no-request', is_flag=True, default=True, help='show requests')
 @click.option('--response/--no-response', is_flag=True, default=True, help='show responses')
 @click.option('-u', '--unique', is_flag=True, help='show only unique requests per image/pid/method/uri combination')
 @click.option('--black-list/--white-list', default=True, is_flag=True)
-def cli_profile(lockdown: LockdownClient, pids, process_names, color, request, response, images, unique, black_list):
+def cli_profile(service_provider: LockdownServiceProvider, pids, process_names, color, request, response, images,
+                unique, black_list):
     """
     Sniff using CFNetworkDiagnostics.mobileconfig profile.
 
     This requires the specific Apple profile to be installed for the sniff to work.
     """
     filters = Filters(pids, process_names, images, black_list)
-    SnifferProfile(lockdown, filters=filters, request=request, response=response, color=color, unique=unique).sniff()
+    SnifferProfile(service_provider, filters=filters, request=request, response=response, color=color,
+                   unique=unique).sniff()
 
 
 @cli.command('preference', cls=Command)
 @click.option('-o', '--out', type=click.File('w'), help='file to store the har entries into upon exit (ctrl+c)')
 @click.option('pids', '-p', '--pid', type=click.INT, multiple=True, help='filter pid list')
 @click.option('--color/--no-color', default=True)
 @click.option('process_names', '-pn', '--process-name', multiple=True, help='filter process name list')
 @click.option('images', '-i', '--image', multiple=True, help='filter image list')
 @click.option('--request/--no-request', is_flag=True, default=True, help='show requests')
 @click.option('--response/--no-response', is_flag=True, default=True, help='show responses')
 @click.option('-u', '--unique', is_flag=True, help='show only unique requests per image/pid/method/uri combination')
 @click.option('--black-list/--white-list', default=True, is_flag=True)
-def cli_preference(lockdown: LockdownClient, out, pids, process_names, images, request, response, color, unique, black_list):
+def cli_preference(service_provider: LockdownServiceProvider, out, pids, process_names, images, request, response,
+                   color, unique, black_list):
     """
     Sniff using the secret com.apple.CFNetwork.plist configuration.
 
     This sniff includes the request/response body as well but requires the device to be jailbroken for
     the sniff to work
     """
     filters = Filters(pids, process_names, images, black_list)
-    SnifferPreference(lockdown, filters=filters, request=request, response=response, out=out, color=color,
+    SnifferPreference(service_provider, filters=filters, request=request, response=response, out=out, color=color,
                       unique=unique).sniff()
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `harlogger-3.0.0/harlogger/http_transaction.py` & `harlogger-3.0.1/harlogger/http_transaction.py`

 * *Files identical despite different names*

### Comparing `harlogger-3.0.0/harlogger/sniffers.py` & `harlogger-3.0.1/harlogger/sniffers.py`

 * *Files identical despite different names*

### Comparing `harlogger-3.0.0/harlogger.egg-info/PKG-INFO` & `harlogger-3.0.1/harlogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harlogger
-Version: 3.0.0
+Version: 3.0.1
 Summary: Simple utlity for sniffing decrypted HTTP/HTTPS traffic on an iOS device (either jailbroken or not)
 Author-email: doronz88 <doron88@gmail.com>, netanelc305 <netanelc305@protonmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, netanelc305 <netanelc305@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `harlogger-3.0.0/pyproject.toml` & `harlogger-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "harlogger"
-version = "3.0.0"
+version = "3.0.1"
 description = "Simple utlity for sniffing decrypted HTTP/HTTPS traffic on an iOS device (either jailbroken or not)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "http", "https", "har", "sniffer", "jailbroken"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" },
```

