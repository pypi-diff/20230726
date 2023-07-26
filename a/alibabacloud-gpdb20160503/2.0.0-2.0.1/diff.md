# Comparing `tmp/alibabacloud_gpdb20160503-2.0.0.tar.gz` & `tmp/alibabacloud_gpdb20160503-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gpdb20160503-2.0.0.tar", last modified: Mon Jul 10 03:44:50 2023, max compression
+gzip compressed data, was "dist/alibabacloud_gpdb20160503-2.0.1.tar", last modified: Wed Jul 26 06:51:06 2023, max compression
```

## Comparing `alibabacloud_gpdb20160503-2.0.0.tar` & `alibabacloud_gpdb20160503-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/
--rw-r--r--   0 root         (0) root         (0)     1014 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2355 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503/__init__.py
--rw-r--r--   0 root         (0) root         (0)   505840 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503/client.py
--rw-r--r--   0 root         (0) root         (0)   737881 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2355 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2023-07-10 03:44:50.000000 alibabacloud_gpdb20160503-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   506126 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/client.py
+-rw-r--r--   0 root         (0) root         (0)   738237 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 06:51:06.000000 alibabacloud_gpdb20160503-2.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2637 2023-07-26 06:51:05.000000 alibabacloud_gpdb20160503-2.0.1/setup.py
```

### Comparing `alibabacloud_gpdb20160503-2.0.0/ChangeLog.md` & `alibabacloud_gpdb20160503-2.0.1/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-10 Version: 2.0.0
+- Add Cloud Disk Encryption.
+
 2023-01-09 Version: 1.1.21
 - Support Pause and Resume Instance.
 
 
 2022-12-13 Version: 1.1.20
 - Support describe cluster support features.
```

### Comparing `alibabacloud_gpdb20160503-2.0.0/LICENSE` & `alibabacloud_gpdb20160503-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-2.0.0/PKG-INFO` & `alibabacloud_gpdb20160503-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gpdb20160503
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503-2.0.0/README-CN.md` & `alibabacloud_gpdb20160503-2.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-2.0.0/README.md` & `alibabacloud_gpdb20160503-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503/client.py` & `alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1375,14 +1375,16 @@
     ) -> gpdb_20160503_models.DeleteCollectionDataResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.collection):
             query['Collection'] = request.collection
         if not UtilClient.is_unset(request.collection_data):
             query['CollectionData'] = request.collection_data
+        if not UtilClient.is_unset(request.collection_data_filter):
+            query['CollectionDataFilter'] = request.collection_data_filter
         if not UtilClient.is_unset(request.dbinstance_id):
             query['DBInstanceId'] = request.dbinstance_id
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         if not UtilClient.is_unset(request.namespace_password):
             query['NamespacePassword'] = request.namespace_password
         if not UtilClient.is_unset(request.owner_id):
@@ -1415,14 +1417,16 @@
     ) -> gpdb_20160503_models.DeleteCollectionDataResponse:
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.collection):
             query['Collection'] = request.collection
         if not UtilClient.is_unset(request.collection_data):
             query['CollectionData'] = request.collection_data
+        if not UtilClient.is_unset(request.collection_data_filter):
+            query['CollectionDataFilter'] = request.collection_data_filter
         if not UtilClient.is_unset(request.dbinstance_id):
             query['DBInstanceId'] = request.dbinstance_id
         if not UtilClient.is_unset(request.namespace):
             query['Namespace'] = request.namespace
         if not UtilClient.is_unset(request.namespace_password):
             query['NamespacePassword'] = request.namespace_password
         if not UtilClient.is_unset(request.owner_id):
```

### Comparing `alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503/models.py` & `alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -2010,22 +2010,24 @@
 
 
 class DeleteCollectionDataRequest(TeaModel):
     def __init__(
         self,
         collection: str = None,
         collection_data: str = None,
+        collection_data_filter: str = None,
         dbinstance_id: str = None,
         namespace: str = None,
         namespace_password: str = None,
         owner_id: int = None,
         region_id: str = None,
     ):
         self.collection = collection
         self.collection_data = collection_data
+        self.collection_data_filter = collection_data_filter
         self.dbinstance_id = dbinstance_id
         self.namespace = namespace
         self.namespace_password = namespace_password
         self.owner_id = owner_id
         self.region_id = region_id
 
     def validate(self):
@@ -2037,14 +2039,16 @@
             return _map
 
         result = dict()
         if self.collection is not None:
             result['Collection'] = self.collection
         if self.collection_data is not None:
             result['CollectionData'] = self.collection_data
+        if self.collection_data_filter is not None:
+            result['CollectionDataFilter'] = self.collection_data_filter
         if self.dbinstance_id is not None:
             result['DBInstanceId'] = self.dbinstance_id
         if self.namespace is not None:
             result['Namespace'] = self.namespace
         if self.namespace_password is not None:
             result['NamespacePassword'] = self.namespace_password
         if self.owner_id is not None:
@@ -2055,14 +2059,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Collection') is not None:
             self.collection = m.get('Collection')
         if m.get('CollectionData') is not None:
             self.collection_data = m.get('CollectionData')
+        if m.get('CollectionDataFilter') is not None:
+            self.collection_data_filter = m.get('CollectionDataFilter')
         if m.get('DBInstanceId') is not None:
             self.dbinstance_id = m.get('DBInstanceId')
         if m.get('Namespace') is not None:
             self.namespace = m.get('Namespace')
         if m.get('NamespacePassword') is not None:
             self.namespace_password = m.get('NamespacePassword')
         if m.get('OwnerId') is not None:
```

### Comparing `alibabacloud_gpdb20160503-2.0.0/alibabacloud_gpdb20160503.egg-info/PKG-INFO` & `alibabacloud_gpdb20160503-2.0.1/alibabacloud_gpdb20160503.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gpdb20160503
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503-2.0.0/setup.py` & `alibabacloud_gpdb20160503-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,28 +20,28 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gpdb20160503.
 
-Created on 10/07/2023
+Created on 26/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gpdb20160503"
 NAME = "alibabacloud_gpdb20160503" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.9, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
```

