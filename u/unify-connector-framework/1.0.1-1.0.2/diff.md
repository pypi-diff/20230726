# Comparing `tmp/unify-connector-framework-1.0.1.tar.gz` & `tmp/unify-connector-framework-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unify-connector-framework-1.0.1.tar", last modified: Tue Jun 27 18:17:08 2023, max compression
+gzip compressed data, was "dist/unify-connector-framework-1.0.2.tar", last modified: Wed Jul 26 17:40:13 2023, max compression
```

## Comparing `unify-connector-framework-1.0.1.tar` & `unify-connector-framework-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2477 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1690 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      553 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unify_connector_framework.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 18:17:08.000000 unify-connector-framework-1.0.1/unifyconnectorframework/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      855 2023-06-27 18:17:02.000000 unify-connector-framework-1.0.1/unifyconnectorframework/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      787 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/config_not_found_error.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15890 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/connector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10771 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/connector_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1691 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/logging.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17963 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/organization_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1373 2023-06-27 18:17:01.000000 unify-connector-framework-1.0.1/unifyconnectorframework/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 17:40:13.000000 unify-connector-framework-1.0.2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-07-26 17:40:04.000000 unify-connector-framework-1.0.2/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-07-26 17:40:13.000000 unify-connector-framework-1.0.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2477 2023-07-26 17:40:04.000000 unify-connector-framework-1.0.2/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-07-26 17:40:13.000000 unify-connector-framework-1.0.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1690 2023-07-26 17:40:04.000000 unify-connector-framework-1.0.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 17:40:13.000000 unify-connector-framework-1.0.2/unify_connector_framework.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-07-26 17:40:13.000000 unify-connector-framework-1.0.2/unify_connector_framework.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      553 2023-07-26 17:40:13.000000 unify-connector-framework-1.0.2/unify_connector_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-07-26 17:40:13.000000 unify-connector-framework-1.0.2/unify_connector_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2023-07-26 17:40:13.000000 unify-connector-framework-1.0.2/unify_connector_framework.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-07-26 17:40:13.000000 unify-connector-framework-1.0.2/unify_connector_framework.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-07-26 17:40:13.000000 unify-connector-framework-1.0.2/unifyconnectorframework/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      855 2023-07-26 17:40:04.000000 unify-connector-framework-1.0.2/unifyconnectorframework/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      787 2023-07-26 17:40:04.000000 unify-connector-framework-1.0.2/unifyconnectorframework/config_not_found_error.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15890 2023-07-26 17:40:04.000000 unify-connector-framework-1.0.2/unifyconnectorframework/connector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10771 2023-07-26 17:40:04.000000 unify-connector-framework-1.0.2/unifyconnectorframework/connector_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1691 2023-07-26 17:40:04.000000 unify-connector-framework-1.0.2/unifyconnectorframework/logging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17963 2023-07-26 17:40:04.000000 unify-connector-framework-1.0.2/unifyconnectorframework/organization_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1829 2023-07-26 17:40:04.000000 unify-connector-framework-1.0.2/unifyconnectorframework/utils.py
```

### Comparing `unify-connector-framework-1.0.1/LICENSE` & `unify-connector-framework-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.1/PKG-INFO` & `unify-connector-framework-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-connector-framework
-Version: 1.0.1
+Version: 1.0.2
 Summary: Develop connectors for Element Unify with the Connector Framework
 Home-page: https://github.com/ElementAnalytics/unify-python-agents-common
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-connector-framework-1.0.1/README.md` & `unify-connector-framework-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.1/setup.py` & `unify-connector-framework-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.1/unify_connector_framework.egg-info/PKG-INFO` & `unify-connector-framework-1.0.2/unify_connector_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-connector-framework
-Version: 1.0.1
+Version: 1.0.2
 Summary: Develop connectors for Element Unify with the Connector Framework
 Home-page: https://github.com/ElementAnalytics/unify-python-agents-common
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-connector-framework-1.0.1/unify_connector_framework.egg-info/SOURCES.txt` & `unify-connector-framework-1.0.2/unify_connector_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.1/unifyconnectorframework/__init__.py` & `unify-connector-framework-1.0.2/unifyconnectorframework/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 Defines package information
 """
 from .organization_client import DatasetOperation, OrganizationClient
 from .connector_handler import ConnectorHandler
 from .connector import Connector
 from .config_not_found_error import ConfigNotFoundError
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
```

### Comparing `unify-connector-framework-1.0.1/unifyconnectorframework/config_not_found_error.py` & `unify-connector-framework-1.0.2/unifyconnectorframework/config_not_found_error.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.1/unifyconnectorframework/connector.py` & `unify-connector-framework-1.0.2/unifyconnectorframework/connector.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.1/unifyconnectorframework/connector_handler.py` & `unify-connector-framework-1.0.2/unifyconnectorframework/connector_handler.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.1/unifyconnectorframework/logging.py` & `unify-connector-framework-1.0.2/unifyconnectorframework/logging.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.1/unifyconnectorframework/organization_client.py` & `unify-connector-framework-1.0.2/unifyconnectorframework/organization_client.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-1.0.1/unifyconnectorframework/utils.py` & `unify-connector-framework-1.0.2/unifyconnectorframework/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,7 +42,22 @@
 
 def get_name(prefix):
     """
     Construct name with current timestamp
     """
     time_stamp = datetime.utcnow().strftime("%H-%M-%S")
     return f"{prefix}-{time_stamp}"
+
+def get_or_raise_error(config, param_name):
+    """
+    Function used for several connectors for validating if
+    `config` dict contains a `param_name` key defined
+    :param config:
+    :param param_name:
+    :return:
+    """
+    if param_name not in config:
+        raise ValueError(
+            f"Connector needs the `{param_name}` param to be defined. " +
+            "Please use Unify Connector Portal.",
+            )
+    return config[param_name]
```

