# Comparing `tmp/zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527.tar.gz` & `tmp/zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527.tar", last modified: Wed Jul 26 11:55:27 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559.tar", last modified: Wed Jul 26 20:15:59 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527.tar` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1196 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      902 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14360 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3675 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     8818 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7367 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    16587 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    15505 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     7202 2023-07-26 11:54:20.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1196 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      774 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-26 11:55:27.000000 zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      902 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14360 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8818 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7367 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    16587 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    15549 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     7202 2023-07-26 20:15:29.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      774 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-26 20:15:59.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/PKG-INFO` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix-agent-baseurl-debug
-Version: 1.0.2023.7.26.1690372527
+Version: 2.0.2023.7.26.1690402559
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/README.md` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/setup.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setuptools.setup(
     name='zesty.zbs-api-securonix-agent-baseurl-debug',  # TODO: Remove '-securonix' when we merge this branch to master.
     install_requires=['requests',
                       'zesty.zesty-id'],
 
-    version='1.0',
+    version='2.0',
     include_package_data=True,
     author="Zesty.co",
     author_email="rnd@cloudvisor.co",
     description="Zesty Disk API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/javatechy/dokr",
```

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/actions.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/BlockDevice.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/FileSystem.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/ManagedFS.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/ManagedFS.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/Usage.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/agent_report.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/disk_mon.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/hf_interface.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/models/overview.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/protocol.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 class Request:
     stage = None
     version = None
     api_key = None
     prefix = None
     api_base = None
     api_is_private_endpoint = False
+    logger = None
     subclasses = {}
 
     def __init__(self, logger:logging.Logger, stage, version, api_key, api_base: str = DEFAULT_BASE_URL):
         self.stage = stage
         self.version = version
         self.api_key = api_key
         self.prefix = ""
@@ -83,14 +84,15 @@
                      f"api_is_private_endpoint = {self.api_is_private_endpoint}")
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         cls.subclasses[cls.__name__] = cls
 
     def send(self):
+        print(vars(self))
         url = self.build_url()
         self.logger.debug(f"send post request with url {url}")
         res = requests.post(
             url,
             data=json.dumps(self.message, separators=(',', ':')),
             headers={"Cache-Control": "no-cache", "Pragma": "no-cache", "x-api-key": self.api_key},
             timeout=(ESTABLISH_CONN_TIMEOUT, RECEIVE_RESPONSE_TIMEOUT)
```

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/src/step_instructions.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/src/step_instructions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix-agent-baseurl-debug
-Version: 1.0.2023.7.26.1690372527
+Version: 2.0.2023.7.26.1690402559
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-1.0.2023.7.26.1690372527/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690402559/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

