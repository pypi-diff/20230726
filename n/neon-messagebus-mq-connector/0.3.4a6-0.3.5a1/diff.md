# Comparing `tmp/neon-messagebus-mq-connector-0.3.4a6.tar.gz` & `tmp/neon-messagebus-mq-connector-0.3.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-messagebus-mq-connector-0.3.4a6.tar", last modified: Tue Jul 18 18:35:06 2023, max compression
+gzip compressed data, was "neon-messagebus-mq-connector-0.3.5a1.tar", last modified: Tue Jul 25 23:25:43 2023, max compression
```

## Comparing `neon-messagebus-mq-connector-0.3.4a6.tar` & `neon-messagebus-mq-connector-0.3.5a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:35:06.910917 neon-messagebus-mq-connector-0.3.4a6/
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-18 18:35:01.000000 neon-messagebus-mq-connector-0.3.4a6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-18 18:35:06.910917 neon-messagebus-mq-connector-0.3.4a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-18 18:35:01.000000 neon-messagebus-mq-connector-0.3.4a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:35:06.910917 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-18 18:35:01.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-18 18:35:01.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-18 18:35:01.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14584 2023-07-18 18:35:01.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-18 18:35:01.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-18 18:35:01.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:35:06.910917 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-18 18:35:06.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-18 18:35:06.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:35:06.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-18 18:35:06.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 18:35:06.000000 neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 18:35:06.910917 neon-messagebus-mq-connector-0.3.4a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-18 18:35:01.000000 neon-messagebus-mq-connector-0.3.4a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:25:43.724092 neon-messagebus-mq-connector-0.3.5a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-25 23:25:43.724092 neon-messagebus-mq-connector-0.3.5a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:25:43.724092 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:25:43.724092 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-25 23:25:43.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-25 23:25:43.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:25:43.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-25 23:25:43.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-25 23:25:43.000000 neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:25:43.724092 neon-messagebus-mq-connector-0.3.5a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-25 23:25:40.000000 neon-messagebus-mq-connector-0.3.5a1/setup.py
```

### Comparing `neon-messagebus-mq-connector-0.3.4a6/LICENSE.md` & `neon-messagebus-mq-connector-0.3.5a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a6/PKG-INFO` & `neon-messagebus-mq-connector-0.3.5a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-messagebus-mq-connector
-Version: 0.3.4a6
+Version: 0.3.5a1
 Summary: MQ-Messagebus Connector Module
 Home-page: https://github.com/neongeckocom/neon-messagebus-mq-connector
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/__init__.py` & `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/__main__.py` & `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/__main__.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/config.py` & `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/config.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/controller.py` & `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import time
 from typing import List, Type, Tuple
 
 import pika
 from ovos_bus_client.client import MessageBusClient
 from ovos_bus_client.message import Message
 
-from neon_utils.logger import LOG
+from ovos_utils.log import LOG, log_deprecation
 from neon_utils.socket_utils import b64_to_dict
 from ovos_config.config import Configuration
 from neon_mq_connector.connector import MQConnector
 from pika.channel import Channel
 from pydantic import ValidationError
 
 from .enums import NeonResponseTypes
@@ -44,19 +44,23 @@
 
 
 class ChatAPIProxy(MQConnector):
     """
     Proxy module for establishing connection between PyKlatchat and neon chat api"""
 
     def __init__(self, config: dict, service_name: str):
-        super().__init__(config, service_name)
-
+        config = config or Configuration()
+        mq_config = config.get("MQ", config)
+        super().__init__(mq_config, service_name)
+        self.bus_config = config.get("websocket")
+        if config.get("MESSAGEBUS"):
+            log_deprecation("MESSAGEBUS config is deprecated. use `websocket`",
+                            "1.0.0")
+            self.bus_config = config.get("websocket")
         self._vhost = '/neon_chat_api'
-        self.bus_config = config.get('MESSAGEBUS') or \
-                          dict(Configuration()).get("websocket")
         self._bus = None
         self.connect_bus()
         self.register_consumer(name=f'neon_api_request_{self.service_id}',
                                vhost=self.vhost,
                                queue=f'neon_chat_api_request_{self.service_id}',
                                callback=self.handle_user_message,
                                on_error=self.default_error_handler,
```

### Comparing `neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/enums.py` & `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/enums.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector/messages.py` & `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector/messages.py`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector.egg-info/PKG-INFO` & `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-messagebus-mq-connector
-Version: 0.3.4a6
+Version: 0.3.5a1
 Summary: MQ-Messagebus Connector Module
 Home-page: https://github.com/neongeckocom/neon-messagebus-mq-connector
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `neon-messagebus-mq-connector-0.3.4a6/neon_messagebus_mq_connector.egg-info/SOURCES.txt` & `neon-messagebus-mq-connector-0.3.5a1/neon_messagebus_mq_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-messagebus-mq-connector-0.3.4a6/setup.py` & `neon-messagebus-mq-connector-0.3.5a1/setup.py`

 * *Files identical despite different names*

