# Comparing `tmp/authomize-rest-api-client-4.3.5.tar.gz` & `tmp/authomize-rest-api-client-4.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.3.5.tar", last modified: Wed Jul 26 10:34:57 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.3.6.tar", last modified: Wed Jul 26 11:00:00 2023, max compression
```

## Comparing `authomize-rest-api-client-4.3.5.tar` & `authomize-rest-api-client-4.3.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3020 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.738721 authomize-rest-api-client-4.3.5/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.738721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84645 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49494 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   200535 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115884 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-26 10:34:57.000000 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-07-26 10:34:57.000000 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 10:34:57.000000 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-26 10:34:57.000000 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-26 10:34:57.000000 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1117 2023-07-26 10:34:42.000000 authomize-rest-api-client-4.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2201 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84645 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49496 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   200535 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115488 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-26 10:59:40.000000 authomize-rest-api-client-4.3.6/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-26 11:00:00.000000 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-26 11:00:00.000000 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 11:00:00.000000 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-26 11:00:00.000000 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-26 11:00:00.000000 authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-26 11:00:00.153061 authomize-rest-api-client-4.3.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-07-26 10:59:44.000000 authomize-rest-api-client-4.3.6/setup.py
```

### Comparing `authomize-rest-api-client-4.3.5/LICENSE.txt` & `authomize-rest-api-client-4.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.5/README.md` & `authomize-rest-api-client-4.3.6/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -45,40 +45,27 @@
 ```
 pip install authomize-rest-api-client
 ```
 
 ## Making changes to this repository
 
 For code automatically generated from openapi.json using [datamodel-code-generator](https://github.com/koxudaxi/datamodel-code-generator)
-
+```
+pip install -e .[codegen]
+```
 Fetching openapi.json and updating schema.
 
 for connectors-rest-api:
 ```
 curl --socks5-hostname 127.0.0.1:1337 http://connectors-rest-api.application.svc:8080/openapi-extended.json | jq --indent 2 . > authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
 ```
 ```
-pip install -e .[codegen]
 datamodel-codegen --use-default-kwarg --encoding=utf-8 --input authomize/rest_api_client/openapi/connectors_rest_api/openapi.json --output authomize/rest_api_client/generated/connectors_rest_api/schemas.py
 ```
 
 for external-rest-api:
-1.
 ```
 curl https://apidev.authomize.com/openapi-platform.json | jq --indent 2 . > authomize/rest_api_client/openapi/external_rest_api/openapi.json
 ```
-2.
 ```
-datamodel-codegen --use-default-kwarg --encoding=utf-8 --input authomize/rest_api_client/openapi/external_rest_api/openapi.json --output authomize/rest_api_client/generated/external_rest_api
+datamodel-codegen --use-default-kwarg --encoding=utf-8 --input authomize/rest_api_client/openapi/external_rest_api/openapi.json --output authomize/rest_api_client/generated/external_rest_api/schemas.py
 ```
-The main schema then is created in an `__init__.py` file, and some missing schemas are created inside another file.  
-Then:
-3. Replace the content of `authomize/rest_api_client/generated/external_rest_api/schemas.py` from the newly created `__init__.py`  
-```
- mv authomize/rest_api_client/generated/external_rest_api/__init__.py authomize/rest_api_client/generated/external_rest_api/schemas.py
- touch authomize/rest_api_client/generated/external_rest_api/__init__.py
-```   
-4. Add the missing schemas from the other file to the end of `schemas.py`
-5. Fix the imports / errors in `schemas.py`
-  for example `from .field_class__authomize.external_rest_api.app.routes_schema import inventory`  
-  should be removed , and all references to inventory updated in the code
-6. Remove all the newly created files (leave only `schemas.py`)
```

### Comparing `authomize-rest-api-client-4.3.5/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.3.6/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.3.6/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.3.6/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  openapi.json
-#   timestamp: 2023-07-24T16:36:38+00:00
+#   timestamp: 2023-07-26T10:45:11+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import List, Optional, Union
 
@@ -420,15 +420,15 @@
     A_8_2_3 = 'A.8.2.3'
     A_7_3_1 = 'A.7.3.1'
     A_8_1_4 = 'A.8.1.4'
 
 
 class MeResponse(BaseModel):
     version: Optional[str] = Field(
-        default='4.3.2', description='**version**', title='Version'
+        default='4.3.0', description='**version**', title='Version'
     )
     id: str = Field(..., description='**id**', title='Id')
     tenant: str = Field(..., description='**tenant**', title='Tenant')
 
 
 class NonPaginatedResponseSchemaCommentSchema(BaseModel):
     class Config:
@@ -1175,14 +1175,36 @@
         title='Sort',
     )
     filter: Optional[SearchAccountsFilterBody] = Field(
         default=None, description='Search Accounts Filter', title='Filter'
     )
 
 
+class SearchAssetsFilterBody(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    originId: Optional[OriginIdFilter] = Field(
+        default=None,
+        description='Find assets by their ID in the source system',
+        title='Originid',
+    )
+    appId: Optional[AppIdFilter] = Field(
+        default=None, description='Find assets by their app ID', title='Appid'
+    )
+    uniqueId: Optional[UniqueIdFilter] = Field(
+        default=None, description='Find assets by their unique ID', title='Uniqueid'
+    )
+    authomizeId: Optional[AssetIdFilter] = Field(
+        default=None,
+        description='Find assets by their Authomize ID',
+        title='Authomizeid',
+    )
+
+
 class SearchAssetsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     sort: Optional[List[SortSchemaSearchAssetsSortFields]] = Field(
         default=None,
         description="Sort the results by asset's name in ascending or descending order",
@@ -1230,14 +1252,36 @@
     sort: Optional[List[SortSchemaFieldName]] = Field(
         default=None,
         description='Sort the results by campaign fields in ascending or descending order',
         title='Sort',
     )
 
 
+class SearchGroupsFilterBody(BaseModel):
+    class Config:
+        extra = Extra.forbid
+
+    uniqueId: Optional[SearchGroupsUniqueIdFilter] = Field(
+        default=None, description='Find groups by their unique ID', title='Uniqueid'
+    )
+    originId: Optional[SearchGroupsOriginIdFilter] = Field(
+        default=None,
+        description='Find groups by their ID in the source system',
+        title='Originid',
+    )
+    appId: Optional[SearchGroupsAppIdFilter] = Field(
+        default=None, description='Find groups by their app ID', title='Appid'
+    )
+    authomizeId: Optional[SearchGroupsIdFilter] = Field(
+        default=None,
+        description='Find groups by their Authomize ID',
+        title='Authomizeid',
+    )
+
+
 class SearchGroupsRequestSchema(BaseModel):
     class Config:
         extra = Extra.forbid
 
     sort: Optional[List[SortSchemaSearchGroupsSortFields]] = Field(
         default=None,
         description="Sort the results by group's name in ascending or descending order",
@@ -1578,50 +1622,7 @@
 
     pagination: Optional[PaginationResponseSchema] = Field(
         default=None, description='Pagination Metadata', title='Pagination'
     )
     data: List[IncidentSchema] = Field(
         ..., description='List of Actual Data', title='Data'
     )
-
-class SearchAssetsFilterBody(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    originId: Optional[OriginIdFilter] = Field(
-        default=None,
-        description='Find assets by their ID in the source system',
-        title='Originid',
-    )
-    appId: Optional[AppIdFilter] = Field(
-        default=None, description='Find assets by their app ID', title='Appid'
-    )
-    uniqueId: Optional[UniqueIdFilter] = Field(
-        default=None, description='Find assets by their unique ID', title='Uniqueid'
-    )
-    authomizeId: Optional[AssetIdFilter] = Field(
-        default=None,
-        description='Find assets by their Authomize ID',
-        title='Authomizeid',
-    )
-
-
-class SearchGroupsFilterBody(BaseModel):
-    class Config:
-        extra = Extra.forbid
-
-    uniqueId: Optional[SearchGroupsUniqueIdFilter] = Field(
-        default=None, description='Find groups by their unique ID', title='Uniqueid'
-    )
-    originId: Optional[SearchGroupsOriginIdFilter] = Field(
-        default=None,
-        description='Find groups by their ID in the source system',
-        title='Originid',
-    )
-    appId: Optional[SearchGroupsAppIdFilter] = Field(
-        default=None, description='Find groups by their app ID', title='Appid'
-    )
-    authomizeId: Optional[SearchGroupsIdFilter] = Field(
-        default=None,
-        description='Find groups by their Authomize ID',
-        title='Authomizeid',
-    )
```

### Comparing `authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.3.6/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9866661783854166%*

 * *Differences: {"'components'": "{'schemas': {'MeResponse': {'properties': {'version': {'default': '4.3.0'}}}, "*

 * *                 "'SearchAssetsRequestSchema': {'properties': {'filter': {'allOf': {0: {'$ref': "*

 * *                 "'#/components/schemas/SearchAssetsFilterBody'}}}}}, 'SearchGroupsRequestSchema': "*

 * *                 "{'properties': {'filter': {'allOf': {0: {'$ref': "*

 * *                 "'#/components/schemas/SearchGroupsFilterBody'}}}}}, 'SearchAssetsFilterBody': "*

 * *                 "OrderedDict([('title', 'Search […]*

```diff
@@ -1577,15 +1577,15 @@
                     },
                     "tenant": {
                         "description": "**tenant**",
                         "title": "Tenant",
                         "type": "string"
                     },
                     "version": {
-                        "default": "4.3.2",
+                        "default": "4.3.0",
                         "description": "**version**",
                         "title": "Version",
                         "type": "string"
                     }
                 },
                 "required": [
                     "id",
@@ -2286,29 +2286,73 @@
                 "description": "An enumeration.",
                 "enum": [
                     "account.name"
                 ],
                 "title": "SearchAccountsSortFields",
                 "type": "string"
             },
+            "SearchAssetsFilterBody": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "appId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/AppIdFilter"
+                            }
+                        ],
+                        "description": "Find assets by their app ID",
+                        "title": "Appid"
+                    },
+                    "authomizeId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/AssetIdFilter"
+                            }
+                        ],
+                        "description": "Find assets by their Authomize ID",
+                        "title": "Authomizeid"
+                    },
+                    "originId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/OriginIdFilter"
+                            }
+                        ],
+                        "description": "Find assets by their ID in the source system",
+                        "title": "Originid"
+                    },
+                    "uniqueId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/UniqueIdFilter"
+                            }
+                        ],
+                        "description": "Find assets by their unique ID",
+                        "title": "Uniqueid"
+                    }
+                },
+                "title": "SearchAssetsFilterBody",
+                "type": "object"
+            },
             "SearchAssetsRequestSchema": {
                 "additionalProperties": false,
                 "description": "Base schema for all incoming API requests.",
                 "properties": {
                     "expand": {
                         "description": "Expand fields (to show additional information)",
                         "items": {
                             "$ref": "#/components/schemas/AssetExpansion"
                         },
                         "type": "array"
                     },
                     "filter": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/_class__authomize.external_rest_api.app.routes_schema.inventory.SearchAssetsFilterBody__"
+                                "$ref": "#/components/schemas/SearchAssetsFilterBody"
                             }
                         ],
                         "description": "Search Assets Filter",
                         "title": "Filter"
                     },
                     "pagination": {
                         "allOf": [
@@ -2421,14 +2465,58 @@
                         "title": "$Eq",
                         "type": "string"
                     }
                 },
                 "title": "SearchGroupsAppIdFilter",
                 "type": "object"
             },
+            "SearchGroupsFilterBody": {
+                "additionalProperties": false,
+                "description": "Base schema for all incoming API requests.",
+                "properties": {
+                    "appId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchGroupsAppIdFilter"
+                            }
+                        ],
+                        "description": "Find groups by their app ID",
+                        "title": "Appid"
+                    },
+                    "authomizeId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchGroupsIdFilter"
+                            }
+                        ],
+                        "description": "Find groups by their Authomize ID",
+                        "title": "Authomizeid"
+                    },
+                    "originId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchGroupsOriginIdFilter"
+                            }
+                        ],
+                        "description": "Find groups by their ID in the source system",
+                        "title": "Originid"
+                    },
+                    "uniqueId": {
+                        "allOf": [
+                            {
+                                "$ref": "#/components/schemas/SearchGroupsUniqueIdFilter"
+                            }
+                        ],
+                        "description": "Find groups by their unique ID",
+                        "title": "Uniqueid"
+                    }
+                },
+                "title": "SearchGroupsFilterBody",
+                "type": "object"
+            },
             "SearchGroupsIdFilter": {
                 "additionalProperties": false,
                 "properties": {
                     "$in": {
                         "default": [],
                         "description": "In",
                         "items": {
@@ -2467,15 +2555,15 @@
                             "$ref": "#/components/schemas/GroupExpansion"
                         },
                         "type": "array"
                     },
                     "filter": {
                         "allOf": [
                             {
-                                "$ref": "#/components/schemas/_class__authomize.external_rest_api.app.routes_schema.inventory.SearchGroupsFilterBody__"
+                                "$ref": "#/components/schemas/SearchGroupsFilterBody"
                             }
                         ],
                         "description": "Search Groups Filter",
                         "title": "Filter"
                     },
                     "pagination": {
                         "allOf": [
@@ -3075,116 +3163,28 @@
                 "required": [
                     "loc",
                     "msg",
                     "type"
                 ],
                 "title": "ValidationError",
                 "type": "object"
-            },
-            "_class__authomize.external_rest_api.app.routes_schema.inventory.SearchAssetsFilterBody__": {
-                "additionalProperties": false,
-                "description": "Base schema for all incoming API requests.",
-                "properties": {
-                    "appId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/AppIdFilter"
-                            }
-                        ],
-                        "description": "Find assets by their app ID",
-                        "title": "Appid"
-                    },
-                    "authomizeId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/AssetIdFilter"
-                            }
-                        ],
-                        "description": "Find assets by their Authomize ID",
-                        "title": "Authomizeid"
-                    },
-                    "originId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/OriginIdFilter"
-                            }
-                        ],
-                        "description": "Find assets by their ID in the source system",
-                        "title": "Originid"
-                    },
-                    "uniqueId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/UniqueIdFilter"
-                            }
-                        ],
-                        "description": "Find assets by their unique ID",
-                        "title": "Uniqueid"
-                    }
-                },
-                "title": "<class 'authomize.external_rest_api.app.routes_schema.inventory.SearchAssetsFilterBody'>",
-                "type": "object"
-            },
-            "_class__authomize.external_rest_api.app.routes_schema.inventory.SearchGroupsFilterBody__": {
-                "additionalProperties": false,
-                "description": "Base schema for all incoming API requests.",
-                "properties": {
-                    "appId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/SearchGroupsAppIdFilter"
-                            }
-                        ],
-                        "description": "Find groups by their app ID",
-                        "title": "Appid"
-                    },
-                    "authomizeId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/SearchGroupsIdFilter"
-                            }
-                        ],
-                        "description": "Find groups by their Authomize ID",
-                        "title": "Authomizeid"
-                    },
-                    "originId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/SearchGroupsOriginIdFilter"
-                            }
-                        ],
-                        "description": "Find groups by their ID in the source system",
-                        "title": "Originid"
-                    },
-                    "uniqueId": {
-                        "allOf": [
-                            {
-                                "$ref": "#/components/schemas/SearchGroupsUniqueIdFilter"
-                            }
-                        ],
-                        "description": "Find groups by their unique ID",
-                        "title": "Uniqueid"
-                    }
-                },
-                "title": "<class 'authomize.external_rest_api.app.routes_schema.inventory.SearchGroupsFilterBody'>",
-                "type": "object"
             }
         },
         "securitySchemes": {
             "APIKeyHeader": {
                 "in": "header",
                 "name": "Authorization",
                 "type": "apiKey"
             }
         }
     },
     "info": {
         "description": "Authomize enables users to integrate your applications with Authomize via custom connectors.\n\nYou can use the APIs described in this document to create your connector.\n\nOnce data is uploaded and processed successfully, your custom connector will function in the same way as the connectors created by Authomize.\n\n## How does Authomize work?\nAuthomize works by gathering information about:\n\n\u00b7 individuals, teams and functions.\n\n\u00b7 apps, assets and accounts.\n\n\u00b7 all the relationships between them.\n\n![img.png](https://storagetry1.blob.core.windows.net/public/78d82650-71b0-4909-8444-022aab79add5.png)\n\n## Connector APIs\n\nAuthomize connector APIs enable pushing data into Authomize from external sources.\n\nThese APIs enable data extracted from outside applications (via application APIs) to be delivered to Authomize.\n\nA connector processes extracted application data to transform it into a format compatible with Authomize.\n\n![img_1.png](https://storagetry1.blob.core.windows.net/public/341bf6ef-2e5b-4284-b715-45105ffbf0f8.png)\n\n## Authentication\nTo Authenticate use the API Token, with the format: `Authorization: API_Token`.\n\nAn API Token is a token you provide when making API calls. \n\n\nThe API Token should be included in every request to the API in an `Authorization` header.\n```\ncurl -v -X POST \\n\n     -H \"Authorization: {API_Token}\" \\n\n     ...\n```\n\n## Limits\nRequests cannot exceed a size of 1MB.\n",
         "title": "Authomize API Reference",
-        "version": "4.3.2",
+        "version": "4.3.0",
         "x-logo": {
             "url": "https://static.authomize.com/public/icons/authomize-green.svg"
         }
     },
     "openapi": "3.0.2",
     "paths": {
         "/is_alive": {
```

### Comparing `authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.3.6/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.5/setup.py` & `authomize-rest-api-client-4.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.3.5',
+        version='4.3.6',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

