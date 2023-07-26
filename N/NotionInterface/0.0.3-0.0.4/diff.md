# Comparing `tmp/NotionInterface-0.0.3.tar.gz` & `tmp/NotionInterface-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NotionInterface-0.0.3.tar", last modified: Thu Jul 13 19:14:02 2023, max compression
+gzip compressed data, was "NotionInterface-0.0.4.tar", last modified: Wed Jul 26 16:56:39 2023, max compression
```

## Comparing `NotionInterface-0.0.3.tar` & `NotionInterface-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-13 19:14:02.521296 NotionInterface-0.0.3/
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-13 19:14:02.520114 NotionInterface-0.0.3/NotionInterface/
--rw-r--r--   0 lukapedra   (501) staff       (20)      183 2023-07-13 19:13:24.000000 NotionInterface-0.0.3/NotionInterface/__init__.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      213 2023-06-20 12:23:58.000000 NotionInterface-0.0.3/NotionInterface/constants.py
--rw-r--r--   0 lukapedra   (501) staff       (20)     5286 2023-07-06 18:36:15.000000 NotionInterface-0.0.3/NotionInterface/notion_database.py
--rw-r--r--   0 lukapedra   (501) staff       (20)     4871 2023-07-06 18:36:53.000000 NotionInterface-0.0.3/NotionInterface/notion_database_types.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      209 2023-06-20 12:23:58.000000 NotionInterface-0.0.3/NotionInterface/notion_header.py
--rw-r--r--   0 lukapedra   (501) staff       (20)      673 2023-07-13 19:07:31.000000 NotionInterface-0.0.3/NotionInterface/notion_page.py
-drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-13 19:14:02.520995 NotionInterface-0.0.3/NotionInterface.egg-info/
--rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-07-13 19:14:02.000000 NotionInterface-0.0.3/NotionInterface.egg-info/PKG-INFO
--rw-r--r--   0 lukapedra   (501) staff       (20)      409 2023-07-13 19:14:02.000000 NotionInterface-0.0.3/NotionInterface.egg-info/SOURCES.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)        1 2023-07-13 19:14:02.000000 NotionInterface-0.0.3/NotionInterface.egg-info/dependency_links.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)      105 2023-07-13 19:14:02.000000 NotionInterface-0.0.3/NotionInterface.egg-info/requires.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)       16 2023-07-13 19:14:02.000000 NotionInterface-0.0.3/NotionInterface.egg-info/top_level.txt
--rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-07-13 19:14:02.521176 NotionInterface-0.0.3/PKG-INFO
--rw-r--r--   0 lukapedra   (501) staff       (20)       93 2023-06-20 12:23:58.000000 NotionInterface-0.0.3/README.md
--rw-r--r--   0 lukapedra   (501) staff       (20)       38 2023-07-13 19:14:02.521340 NotionInterface-0.0.3/setup.cfg
--rw-r--r--   0 lukapedra   (501) staff       (20)      858 2023-07-13 19:13:40.000000 NotionInterface-0.0.3/setup.py
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-26 16:56:39.037881 NotionInterface-0.0.4/
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-26 16:56:39.036173 NotionInterface-0.0.4/NotionInterface/
+-rw-r--r--   0 lukapedra   (501) staff       (20)      183 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/__init__.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      213 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/constants.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)     6724 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/notion_database.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)     4871 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/notion_database_types.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      209 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/notion_header.py
+-rw-r--r--   0 lukapedra   (501) staff       (20)      673 2023-07-26 16:55:50.000000 NotionInterface-0.0.4/NotionInterface/notion_page.py
+drwxr-xr-x   0 lukapedra   (501) staff       (20)        0 2023-07-26 16:56:39.037417 NotionInterface-0.0.4/NotionInterface.egg-info/
+-rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-07-26 16:56:38.000000 NotionInterface-0.0.4/NotionInterface.egg-info/PKG-INFO
+-rw-r--r--   0 lukapedra   (501) staff       (20)      409 2023-07-26 16:56:39.000000 NotionInterface-0.0.4/NotionInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)        1 2023-07-26 16:56:38.000000 NotionInterface-0.0.4/NotionInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)      105 2023-07-26 16:56:38.000000 NotionInterface-0.0.4/NotionInterface.egg-info/requires.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)       16 2023-07-26 16:56:38.000000 NotionInterface-0.0.4/NotionInterface.egg-info/top_level.txt
+-rw-r--r--   0 lukapedra   (501) staff       (20)      573 2023-07-26 16:56:39.037701 NotionInterface-0.0.4/PKG-INFO
+-rw-r--r--   0 lukapedra   (501) staff       (20)       93 2023-06-20 12:23:58.000000 NotionInterface-0.0.4/README.md
+-rw-r--r--   0 lukapedra   (501) staff       (20)       38 2023-07-26 16:56:39.037985 NotionInterface-0.0.4/setup.cfg
+-rw-r--r--   0 lukapedra   (501) staff       (20)      858 2023-07-26 16:56:26.000000 NotionInterface-0.0.4/setup.py
```

### Comparing `NotionInterface-0.0.3/NotionInterface/notion_database.py` & `NotionInterface-0.0.4/NotionInterface/notion_database.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import requests
 import json
 from . import constants
 from .notion_header import getHeader
 from .notion_database_types import getValue, generateNotionProperty
 import pandas as pd
+import datetime
+import dateutil.parser
 
 class NotionDatabase:
     db_id:str
     key:str
     columns=None
 
     def __init__(self, database_id:str, notion_key:str):
@@ -32,15 +34,15 @@
         result['database_title'] = res_dict["title"][0]['text']['content']
         for key in res_dict['properties'].keys():
             properties[key] = res_dict['properties'][key]['type']
         result['properties'] = properties
         
         return result
     
-    def getAllRecords(self, next_cursor=None):
+    def getAllRecords(self,next_cursor=None):
         url = f"https://api.notion.com/v1/databases/{self.db_id}/query"
 
         if (next_cursor==None):
             payload = {"page_size": 100}
         else:
             payload = {"start_cursor": next_cursor}
         
@@ -53,27 +55,66 @@
         for res in res_dict['results']:
             linha = {}
             properties = {}
             linha['id'] = res['id']
             linha['created_time'] = res['created_time']
             linha['last_edited_time'] = res['last_edited_time']
 
+
             for key in res['properties'].keys():
                 properties[key] = getValue(res['properties'][key])
             linha['properties'] = properties
 
             result.append(linha)
 
         # RECURSÃO PARA PRÓXIMO CURSOR
         if res_dict['next_cursor'] != None:
             result_rec = self.getAllRecords(next_cursor=res_dict['next_cursor'])
             result.extend(result_rec)
 
         return result
+    def getAllRecordsSince(self, Updated_Since:datetime.datetime,next_cursor=None):
+        url = f"https://api.notion.com/v1/databases/{self.db_id}/query"
+
+        if (next_cursor==None):
+            payload = {"page_size": 100}
+        else:
+            payload = {"start_cursor": next_cursor}
+        
+        res_dict = requests.post(url, json=payload, headers=getHeader(self.key)).json()
 
+        if (res_dict['object'] != 'list'):
+            raise Exception(constants.ERROR_NOT_LIST)
+
+        result = []
+        for res in res_dict['results']:
+            date = dateutil.parser.isoparse(res['last_edited_time'])
+            date = date.replace(tzinfo=None)
+            if (date < Updated_Since):
+                continue
+            linha = {}
+            properties = {}
+            linha['id'] = res['id']
+            linha['created_time'] = res['created_time']
+            linha['last_edited_time'] = res['last_edited_time']
+
+
+            for key in res['properties'].keys():
+                properties[key] = getValue(res['properties'][key])
+            linha['properties'] = properties
+
+            result.append(linha)
+
+        # RECURSÃO PARA PRÓXIMO CURSOR
+        if res_dict['next_cursor'] != None:
+            result_rec = self.getAllRecordsSince(next_cursor=res_dict['next_cursor'],Updated_Since=Updated_Since)
+            result.extend(result_rec)
+
+        return result
+    
 
     def getRecord(self, pageId:str):
         pageId = self.formatURLString(pageId)
         url = f"https://api.notion.com/v1/pages/{pageId}"
 
         res_dict = requests.get(url, headers=getHeader(self.key)).json()
         if (res_dict['object'] != 'page'):
```

### Comparing `NotionInterface-0.0.3/NotionInterface/notion_database_types.py` & `NotionInterface-0.0.4/NotionInterface/notion_database_types.py`

 * *Files identical despite different names*

### Comparing `NotionInterface-0.0.3/NotionInterface/notion_page.py` & `NotionInterface-0.0.4/NotionInterface/notion_page.py`

 * *Files identical despite different names*

### Comparing `NotionInterface-0.0.3/NotionInterface.egg-info/PKG-INFO` & `NotionInterface-0.0.4/NotionInterface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NotionInterface
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple Notion db interface for Python
 Home-page: UNKNOWN
 Author: LukaPedra (Lucca Rocha)
 Author-email: <lucca.v.rocha@gmail.com>
 License: UNKNOWN
 Keywords: python,Notion,Database,page,Block,pandas
 Platform: UNKNOWN
```

### Comparing `NotionInterface-0.0.3/PKG-INFO` & `NotionInterface-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NotionInterface
-Version: 0.0.3
+Version: 0.0.4
 Summary: A simple Notion db interface for Python
 Home-page: UNKNOWN
 Author: LukaPedra (Lucca Rocha)
 Author-email: <lucca.v.rocha@gmail.com>
 License: UNKNOWN
 Keywords: python,Notion,Database,page,Block,pandas
 Platform: UNKNOWN
```

### Comparing `NotionInterface-0.0.3/setup.py` & `NotionInterface-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A simple Notion db interface for Python'
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 # Setting up
 setup(
```

