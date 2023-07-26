# Comparing `tmp/alibabacloud_gpdb20160503_py2-2.0.0.tar.gz` & `tmp/alibabacloud_gpdb20160503_py2-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_gpdb20160503_py2-2.0.0.tar", last modified: Mon Jul 10 03:44:51 2023, max compression
+gzip compressed data, was "dist/alibabacloud_gpdb20160503_py2-2.0.1.tar", last modified: Wed Jul 26 06:50:39 2023, max compression
```

## Comparing `alibabacloud_gpdb20160503_py2-2.0.0.tar` & `alibabacloud_gpdb20160503_py2-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      924 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2499 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1036 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1119 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503/__init__.py
--rw-r--r--   0 root         (0) root         (0)   224085 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503/client.py
--rw-r--r--   0 root         (0) root         (0)   743628 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2499 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      448 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2929 2023-07-10 03:44:51.000000 alibabacloud_gpdb20160503_py2-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/
+-rw-r--r--   0 root         (0) root         (0)      980 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   224228 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/client.py
+-rw-r--r--   0 root         (0) root         (0)   743982 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      448 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-26 06:50:39.000000 alibabacloud_gpdb20160503_py2-2.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2929 2023-07-26 06:50:38.000000 alibabacloud_gpdb20160503_py2-2.0.1/setup.py
```

### Comparing `alibabacloud_gpdb20160503_py2-2.0.0/ChangeLog.md` & `alibabacloud_gpdb20160503_py2-2.0.1/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2023-07-10 Version: 2.0.0
+- Add Cloud Disk Encryption.
+
 2023-01-09 Version: 1.1.22
 - Support Pause and Resume Instance.
 
 
 2022-12-13 Version: 1.1.21
 - Support describe cluster support features.
```

### Comparing `alibabacloud_gpdb20160503_py2-2.0.0/LICENSE` & `alibabacloud_gpdb20160503_py2-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503_py2-2.0.0/PKG-INFO` & `alibabacloud_gpdb20160503_py2-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_gpdb20160503_py2
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503_py2-2.0.0/README-CN.md` & `alibabacloud_gpdb20160503_py2-2.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503_py2-2.0.0/README.md` & `alibabacloud_gpdb20160503_py2-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503/client.py` & `alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -652,14 +652,16 @@
     def delete_collection_data_with_options(self, request, runtime):
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

### Comparing `alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503/models.py` & `alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1789,18 +1789,19 @@
         if m.get('body') is not None:
             temp_model = DeleteCollectionResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class DeleteCollectionDataRequest(TeaModel):
-    def __init__(self, collection=None, collection_data=None, dbinstance_id=None, namespace=None,
-                 namespace_password=None, owner_id=None, region_id=None):
+    def __init__(self, collection=None, collection_data=None, collection_data_filter=None, dbinstance_id=None,
+                 namespace=None, namespace_password=None, owner_id=None, region_id=None):
         self.collection = collection  # type: str
         self.collection_data = collection_data  # type: str
+        self.collection_data_filter = collection_data_filter  # type: str
         self.dbinstance_id = dbinstance_id  # type: str
         self.namespace = namespace  # type: str
         self.namespace_password = namespace_password  # type: str
         self.owner_id = owner_id  # type: long
         self.region_id = region_id  # type: str
 
     def validate(self):
@@ -1812,14 +1813,16 @@
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
@@ -1830,14 +1833,16 @@
 
     def from_map(self, m=None):
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

### Comparing `alibabacloud_gpdb20160503_py2-2.0.0/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO` & `alibabacloud_gpdb20160503_py2-2.0.1/alibabacloud_gpdb20160503_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-gpdb20160503-py2
-Version: 2.0.0
+Version: 2.0.1
 Summary: Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_gpdb20160503_py2-2.0.0/setup.py` & `alibabacloud_gpdb20160503_py2-2.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_gpdb20160503_py2.
 
-Created on 10/07/2023
+Created on 26/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_gpdb20160503"
 NAME = "alibabacloud_gpdb20160503_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AnalyticDB for PostgreSQL (20160503) SDK Library for Python2"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python2-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util_py2>=0.0.8, <1.0.0",
+    "alibabacloud_tea_util_py2>=0.0.9, <1.0.0",
     "alibabacloud_tea_openapi_py2>=0.1.6, <1.0.0",
     "alibabacloud_openapi_util_py2>=0.1.1, <1.0.0",
     "alibabacloud_endpoint_util_py2>=0.0.2, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
```

