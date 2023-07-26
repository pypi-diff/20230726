# Comparing `tmp/zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172.tar.gz` & `tmp/zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172.tar", last modified: Wed Jul 26 20:59:32 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274.tar", last modified: Wed Jul 26 21:01:14 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172.tar` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1196 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      902 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14360 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3675 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     8818 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7367 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    16587 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    15533 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     7202 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1196 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      774 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-07-26 20:59:32.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      902 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14360 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8818 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7367 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    16587 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    15632 2023-07-26 20:59:46.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     7202 2023-07-26 20:58:23.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      774 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-07-26 21:01:14.000000 zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/PKG-INFO` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix-agent-baseurl-debug
-Version: 2.0.2023.7.26.1690405172
+Version: 2.0.2023.7.26.1690405274
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/README.md` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/setup.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/actions.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/BlockDevice.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/FileSystem.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/ManagedFS.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/ManagedFS.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/Usage.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/agent_report.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/disk_mon.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/hf_interface.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/models/overview.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/protocol.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,18 +82,21 @@
         logger.debug(f"Create request with base_url {api_base}, "
                      f"api_is_private_endpoint = {self.api_is_private_endpoint}")
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         cls.subclasses[cls.__name__] = cls
 
-    def send(self, logger):
+    def send(self, logger = None):
         print(vars(self))
         url = self.build_url()
-        logger.debug(f"send post request with url {url}")
+        if logger:
+            logger.debug(f"send post request with url {url}")
+        else:
+            print(f"send post request with url {url}")
         res = requests.post(
             url,
             data=json.dumps(self.message, separators=(',', ':')),
             headers={"Cache-Control": "no-cache", "Pragma": "no-cache", "x-api-key": self.api_key},
             timeout=(ESTABLISH_CONN_TIMEOUT, RECEIVE_RESPONSE_TIMEOUT)
         )
         return self.Response(res)
```

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/src/step_instructions.py` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/src/step_instructions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix-agent-baseurl-debug
-Version: 2.0.2023.7.26.1690405172
+Version: 2.0.2023.7.26.1690405274
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405172/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-agent-baseurl-debug-2.0.2023.7.26.1690405274/zesty.zbs_api_securonix_agent_baseurl_debug.egg-info/SOURCES.txt`

 * *Files identical despite different names*

