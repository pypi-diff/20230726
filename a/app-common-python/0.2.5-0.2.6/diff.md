# Comparing `tmp/app-common-python-0.2.5.tar.gz` & `tmp/app-common-python-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app-common-python-0.2.5.tar", last modified: Wed Feb 15 16:16:17 2023, max compression
+gzip compressed data, was "app-common-python-0.2.6.tar", last modified: Wed Jul 26 12:24:12 2023, max compression
```

## Comparing `app-common-python-0.2.5.tar` & `app-common-python-0.2.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:16:17.209625 app-common-python-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:16:17.205625 app-common-python-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:16:17.205625 app-common-python-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-02-15 16:16:03.000000 app-common-python-0.2.5/.github/workflows/package.yml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-15 16:16:03.000000 app-common-python-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-02-15 16:16:17.209625 app-common-python-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-02-15 16:16:03.000000 app-common-python-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:16:17.205625 app-common-python-0.2.5/app_common_python/
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-02-15 16:16:03.000000 app-common-python-0.2.5/app_common_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16727 2023-02-15 16:16:03.000000 app-common-python-0.2.5/app_common_python/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:16:17.209625 app-common-python-0.2.5/app_common_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-02-15 16:16:17.000000 app-common-python-0.2.5/app_common_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-15 16:16:17.000000 app-common-python-0.2.5/app_common_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 16:16:17.000000 app-common-python-0.2.5/app_common_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 16:16:16.000000 app-common-python-0.2.5/app_common_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-15 16:16:17.000000 app-common-python-0.2.5/app_common_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-15 16:16:03.000000 app-common-python-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    18572 2023-02-15 16:16:03.000000 app-common-python-0.2.5/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-15 16:16:17.209625 app-common-python-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 16:16:03.000000 app-common-python-0.2.5/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      323 2023-02-15 16:16:03.000000 app-common-python-0.2.5/sync_config.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-02-15 16:16:03.000000 app-common-python-0.2.5/test.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 16:16:17.209625 app-common-python-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-02-15 16:16:03.000000 app-common-python-0.2.5/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:12.830904 app-common-python-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:12.826904 app-common-python-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:12.830904 app-common-python-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-26 12:23:55.000000 app-common-python-0.2.6/.github/workflows/package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 12:23:55.000000 app-common-python-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 12:24:12.830904 app-common-python-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-26 12:23:55.000000 app-common-python-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:12.830904 app-common-python-0.2.6/app_common_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-26 12:23:55.000000 app-common-python-0.2.6/app_common_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16885 2023-07-26 12:23:55.000000 app-common-python-0.2.6/app_common_python/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:12.830904 app-common-python-0.2.6/app_common_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-26 12:24:12.000000 app-common-python-0.2.6/app_common_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-26 12:24:12.000000 app-common-python-0.2.6/app_common_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:24:12.000000 app-common-python-0.2.6/app_common_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:24:12.000000 app-common-python-0.2.6/app_common_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 12:24:12.000000 app-common-python-0.2.6/app_common_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-26 12:23:55.000000 app-common-python-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-07-26 12:23:55.000000 app-common-python-0.2.6/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-26 12:24:12.834904 app-common-python-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:23:55.000000 app-common-python-0.2.6/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      323 2023-07-26 12:23:55.000000 app-common-python-0.2.6/sync_config.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-26 12:23:55.000000 app-common-python-0.2.6/test.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:24:12.830904 app-common-python-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-26 12:23:55.000000 app-common-python-0.2.6/tests/test_config.py
```

### Comparing `app-common-python-0.2.5/.github/workflows/package.yml` & `app-common-python-0.2.6/.github/workflows/package.yml`

 * *Files identical despite different names*

### Comparing `app-common-python-0.2.5/PKG-INFO` & `app-common-python-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-common-python
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://github.com/RedHatInsights/app-common-python
 Author-email: psavage@redhat.com
 Description-Content-Type: text/markdown
 
 app-common-python
 =================
```

### Comparing `app-common-python-0.2.5/README.md` & `app-common-python-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `app-common-python-0.2.5/app_common_python/__init__.py` & `app-common-python-0.2.6/app_common_python/__init__.py`

 * *Files identical despite different names*

### Comparing `app-common-python-0.2.5/app_common_python/types.py` & `app-common-python-0.2.6/app_common_python/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -382,14 +382,17 @@
 
         #: Dependent service connection info
         self.app = None
 
         #: Dependent service connection info
         self.tlsPort = None
 
+        #: The top level api path that the app should serve from /api/<apiPath>
+        self.apiPath = None
+
     @classmethod
     def dictToObject(cls, dict):
         if dict is None:
             return None
         obj = cls()
 
         obj.name = dict.get('name', None)
@@ -397,14 +400,16 @@
         obj.hostname = dict.get('hostname', None)
 
         obj.port = dict.get('port', None)
 
         obj.app = dict.get('app', None)
 
         obj.tlsPort = dict.get('tlsPort', None)
+
+        obj.apiPath = dict.get('apiPath', None)
         return obj
 
 
 class PrivateDependencyEndpoint:
     """ Dependent service connection info
     """
```

### Comparing `app-common-python-0.2.5/app_common_python.egg-info/PKG-INFO` & `app-common-python-0.2.6/app_common_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: app-common-python
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://github.com/RedHatInsights/app-common-python
 Author-email: psavage@redhat.com
 Description-Content-Type: text/markdown
 
 app-common-python
 =================
```

### Comparing `app-common-python-0.2.5/schema.json` & `app-common-python-0.2.6/schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998854166666667%*

 * *Differences: {"'definitions'": "{'DependencyEndpoint': {'properties': {'apiPath': OrderedDict([('description', "*

 * *                  "'The top level api path that the app should serve from /api/<apiPath>')])}, "*

 * *                  "'required': {insert: [(4, 'apiPath')]}}}"}*

```diff
@@ -215,14 +215,17 @@
             "title": "DatabaseConfig",
             "type": "object"
         },
         "DependencyEndpoint": {
             "description": "Dependent service connection info",
             "id": "dependency",
             "properties": {
+                "apiPath": {
+                    "description": "The top level api path that the app should serve from /api/<apiPath>"
+                },
                 "app": {
                     "description": "The app name of the ClowdApp hosting the service.",
                     "type": "string"
                 },
                 "hostname": {
                     "description": "The hostname of the dependent service.",
                     "type": "string"
@@ -240,15 +243,16 @@
                     "type": "integer"
                 }
             },
             "required": [
                 "name",
                 "hostname",
                 "port",
-                "app"
+                "app",
+                "apiPath"
             ],
             "type": "object"
         },
         "DeploymentMetadata": {
             "description": "Deployment Metadata",
             "properties": {
                 "image": {
```

### Comparing `app-common-python-0.2.5/test.json` & `app-common-python-0.2.6/test.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'apiPath'": "'api-path'",*

 * * "'endpoints'": "{0: {'apiPath': 'app1-api-path'}, 1: {'apiPath': 'app2-api-path'}}"}*

```diff
@@ -1,28 +1,31 @@
 {
+    "apiPath": "api-path",
     "database": {
         "adminPassword": "adminpassword",
         "adminUsername": "adminusername",
         "hostname": "hostname",
         "name": "dBaseName",
         "password": "password",
         "pgPass": "testing",
         "port": 5432,
         "rdsCa": "ca",
         "sslMode": "verify-full",
         "username": "username"
     },
     "endpoints": [
         {
+            "apiPath": "app1-api-path",
             "app": "app1",
             "hostname": "endpoint1.svc",
             "name": "endpoint1",
             "port": 8000
         },
         {
+            "apiPath": "app2-api-path",
             "app": "app2",
             "hostname": "endpoint2.svc",
             "name": "endpoint2",
             "port": 8000
         }
     ],
     "featureFlags": {
```

### Comparing `app-common-python-0.2.5/tests/test_config.py` & `app-common-python-0.2.6/tests/test_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from app_common_python import LoadedConfig, KafkaTopics, DependencyEndpoints, ObjectBuckets, KafkaServers, isClowderEnabled, PrivateDependencyEndpoints
 
 def test_load_config():
     assert LoadedConfig.kafka.brokers[0].port == 27015, "Port failed to be found"
     assert KafkaTopics["originalName"].name == "someTopic"
     assert DependencyEndpoints["app1"]["endpoint1"].port == 8000
     assert DependencyEndpoints["app2"]["endpoint2"].name == "endpoint2"
+    assert DependencyEndpoints["app1"]["endpoint1"].apiPath == "app1-api-path"
+    assert DependencyEndpoints["app2"]["endpoint2"].apiPath == "app2-api-path"
     assert PrivateDependencyEndpoints["app1"]["endpoint1"].port == 10000
     assert PrivateDependencyEndpoints["app2"]["endpoint2"].name == "endpoint2"
     assert ObjectBuckets["reqname"].name == "name"
     assert KafkaServers[0] == "broker-host:27015"
     assert LoadedConfig.kafka.brokers[0].securityProtocol == "plaintext"
     with open(LoadedConfig.rds_ca()) as fp:
         ca_content = fp.read()
```

