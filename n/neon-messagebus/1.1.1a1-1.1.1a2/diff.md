# Comparing `tmp/neon_messagebus-1.1.1a1.tar.gz` & `tmp/neon_messagebus-1.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_messagebus-1.1.1a1.tar", last modified: Tue Jul 25 22:53:20 2023, max compression
+gzip compressed data, was "neon_messagebus-1.1.1a2.tar", last modified: Tue Jul 25 23:32:35 2023, max compression
```

## Comparing `neon_messagebus-1.1.1a1.tar` & `neon_messagebus-1.1.1a2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:53:20.820140 neon_messagebus-1.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-25 22:53:20.820140 neon_messagebus-1.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:53:20.816140 neon_messagebus-1.1.1a1/neon_messagebus/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/neon_messagebus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/neon_messagebus/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:53:20.816140 neon_messagebus-1.1.1a1/neon_messagebus/service/
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/neon_messagebus/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/neon_messagebus/service/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:53:20.820140 neon_messagebus-1.1.1a1/neon_messagebus/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/neon_messagebus/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/neon_messagebus/util/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/neon_messagebus/util/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/neon_messagebus/util/mq_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/neon_messagebus/util/signal_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:53:20.816140 neon_messagebus-1.1.1a1/neon_messagebus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-25 22:53:20.000000 neon_messagebus-1.1.1a1/neon_messagebus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-25 22:53:20.000000 neon_messagebus-1.1.1a1/neon_messagebus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:53:20.000000 neon_messagebus-1.1.1a1/neon_messagebus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 22:53:20.000000 neon_messagebus-1.1.1a1/neon_messagebus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 22:53:20.000000 neon_messagebus-1.1.1a1/neon_messagebus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 22:53:20.000000 neon_messagebus-1.1.1a1/neon_messagebus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 22:53:20.820140 neon_messagebus-1.1.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-25 22:53:16.000000 neon_messagebus-1.1.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:32:35.985178 neon_messagebus-1.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-25 23:32:35.985178 neon_messagebus-1.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:32:35.985178 neon_messagebus-1.1.1a2/neon_messagebus/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/neon_messagebus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/neon_messagebus/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:32:35.985178 neon_messagebus-1.1.1a2/neon_messagebus/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/neon_messagebus/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/neon_messagebus/service/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:32:35.985178 neon_messagebus-1.1.1a2/neon_messagebus/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/neon_messagebus/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/neon_messagebus/util/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/neon_messagebus/util/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/neon_messagebus/util/mq_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/neon_messagebus/util/signal_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:32:35.985178 neon_messagebus-1.1.1a2/neon_messagebus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-25 23:32:35.000000 neon_messagebus-1.1.1a2/neon_messagebus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-25 23:32:35.000000 neon_messagebus-1.1.1a2/neon_messagebus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:32:35.000000 neon_messagebus-1.1.1a2/neon_messagebus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-25 23:32:35.000000 neon_messagebus-1.1.1a2/neon_messagebus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 23:32:35.000000 neon_messagebus-1.1.1a2/neon_messagebus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 23:32:35.000000 neon_messagebus-1.1.1a2/neon_messagebus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:32:35.985178 neon_messagebus-1.1.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-25 23:32:32.000000 neon_messagebus-1.1.1a2/setup.py
```

### Comparing `neon_messagebus-1.1.1a1/LICENSE.md` & `neon_messagebus-1.1.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/PKG-INFO` & `neon_messagebus-1.1.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon_messagebus
-Version: 1.1.1a1
+Version: 1.1.1a2
 Summary: Neon Messagebus Module
 Home-page: https://github.com/NeonGeckoCom/neon_messagebus
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon_messagebus-1.1.1a1/README.md` & `neon_messagebus-1.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus/__init__.py` & `neon_messagebus-1.1.1a2/neon_messagebus/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus/cli.py` & `neon_messagebus-1.1.1a2/neon_messagebus/cli.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus/service/__init__.py` & `neon_messagebus-1.1.1a2/neon_messagebus/service/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus/service/__main__.py` & `neon_messagebus-1.1.1a2/neon_messagebus/service/__main__.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus/util/__init__.py` & `neon_messagebus-1.1.1a2/neon_messagebus/util/__init__.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus/util/config.py` & `neon_messagebus-1.1.1a2/neon_messagebus/util/config.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus/util/message_utils.py` & `neon_messagebus-1.1.1a2/neon_messagebus/util/message_utils.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus/util/mq_connector.py` & `neon_messagebus-1.1.1a2/neon_messagebus/util/mq_connector.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,13 +38,11 @@
     config = Configuration()
     mq_config = config.get("MQ", {})
     bus_config = bus_config or dict(config).get("websocket")
 
     if "neon_chat_api" not in mq_config.get("users", {}):
         LOG.info("Skipping MQ Connector init")
         return None
-    bus_config = bus_config
     chat_connector = ChatAPIProxy(service_name="neon_chat_api",
-                                  config={"MQ": mq_config,
-                                          "MESSAGEBUS": bus_config})
+                                  config=config)
     chat_connector.run(run_sync=False)
     return chat_connector
```

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus/util/signal_utils.py` & `neon_messagebus-1.1.1a2/neon_messagebus/util/signal_utils.py`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus.egg-info/PKG-INFO` & `neon_messagebus-1.1.1a2/neon_messagebus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-messagebus
-Version: 1.1.1a1
+Version: 1.1.1a2
 Summary: Neon Messagebus Module
 Home-page: https://github.com/NeonGeckoCom/neon_messagebus
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon_messagebus-1.1.1a1/neon_messagebus.egg-info/SOURCES.txt` & `neon_messagebus-1.1.1a2/neon_messagebus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon_messagebus-1.1.1a1/setup.py` & `neon_messagebus-1.1.1a2/setup.py`

 * *Files identical despite different names*

