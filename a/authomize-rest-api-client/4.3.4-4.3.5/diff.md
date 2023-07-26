# Comparing `tmp/authomize-rest-api-client-4.3.4.tar.gz` & `tmp/authomize-rest-api-client-4.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "authomize-rest-api-client-4.3.4.tar", last modified: Tue Jul 25 08:36:04 2023, max compression
+gzip compressed data, was "authomize-rest-api-client-4.3.5.tar", last modified: Wed Jul 26 10:34:57 2023, max compression
```

## Comparing `authomize-rest-api-client-4.3.4.tar` & `authomize-rest-api-client-4.3.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/
--rw-r--r--   0 root         (0) root         (0)     1072 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3020 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/
--rw-r--r--   0 root         (0) root         (0)      627 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/
--rw-r--r--   0 root         (0) root         (0)       81 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/base_client.py
--rw-r--r--   0 root         (0) root         (0)    10358 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/client.py
--rw-r--r--   0 root         (0) root         (0)    13027 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/connectors_client.py
--rw-r--r--   0 root         (0) root         (0)     1102 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/platform_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/configuration/authomize_api_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84645 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49495 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/external_rest_api/schemas.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/connectors_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   200535 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/external_rest_api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/external_rest_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115884 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/external_rest_api/openapi.json
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-25 08:35:38.000000 authomize-rest-api-client-4.3.4/authomize/rest_api_client/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      251 2023-07-25 08:36:04.000000 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1356 2023-07-25 08:36:04.000000 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 08:36:04.000000 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-07-25 08:36:04.000000 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-07-25 08:36:04.000000 authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      336 2023-07-25 08:36:04.094931 authomize-rest-api-client-4.3.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1117 2023-07-25 08:35:49.000000 authomize-rest-api-client-4.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3020 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.738721 authomize-rest-api-client-4.3.5/authomize/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.738721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/
+-rw-r--r--   0 root         (0) root         (0)      627 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2566 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/base_client.py
+-rw-r--r--   0 root         (0) root         (0)    10358 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    13027 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/connectors_client.py
+-rw-r--r--   0 root         (0) root         (0)     1102 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/platform_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/configuration/authomize_api_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84645 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49494 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/external_rest_api/schemas.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/connectors_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/connectors_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   200535 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/external_rest_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/external_rest_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115884 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-26 10:34:38.000000 authomize-rest-api-client-4.3.5/authomize/rest_api_client/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-26 10:34:57.000000 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1356 2023-07-26 10:34:57.000000 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 10:34:57.000000 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-07-26 10:34:57.000000 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-07-26 10:34:57.000000 authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      336 2023-07-26 10:34:57.742721 authomize-rest-api-client-4.3.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-07-26 10:34:42.000000 authomize-rest-api-client-4.3.5/setup.py
```

### Comparing `authomize-rest-api-client-4.3.4/LICENSE.txt` & `authomize-rest-api-client-4.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/README.md` & `authomize-rest-api-client-4.3.5/README.md`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/authomize/rest_api_client/__init__.py` & `authomize-rest-api-client-4.3.5/authomize/rest_api_client/__init__.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/base_client.py` & `authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/base_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/client.py` & `authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/connectors_client.py` & `authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/connectors_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/authomize/rest_api_client/client/platform_client.py` & `authomize-rest-api-client-4.3.5/authomize/rest_api_client/client/platform_client.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/connectors_rest_api/schemas.py` & `authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/connectors_rest_api/schemas.py`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/authomize/rest_api_client/generated/external_rest_api/schemas.py` & `authomize-rest-api-client-4.3.5/authomize/rest_api_client/generated/external_rest_api/schemas.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1620,8 +1620,8 @@
     appId: Optional[SearchGroupsAppIdFilter] = Field(
         default=None, description='Find groups by their app ID', title='Appid'
     )
     authomizeId: Optional[SearchGroupsIdFilter] = Field(
         default=None,
         description='Find groups by their Authomize ID',
         title='Authomizeid',
-    )
+    )
```

### Comparing `authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json` & `authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/connectors_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/authomize/rest_api_client/openapi/external_rest_api/openapi.json` & `authomize-rest-api-client-4.3.5/authomize/rest_api_client/openapi/external_rest_api/openapi.json`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/authomize_rest_api_client.egg-info/SOURCES.txt` & `authomize-rest-api-client-4.3.5/authomize_rest_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authomize-rest-api-client-4.3.4/setup.py` & `authomize-rest-api-client-4.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 if __name__ == '__main__':
     setup(
-        version='4.3.4',
+        version='4.3.5',
         name='authomize-rest-api-client',
         author='Authomize inc.',
         license='MIT',
         author_email='info@authomize.com',
         description='Authomize REST API Python Client',
         packages=find_namespace_packages(include=['authomize.*']),
         package_data={
```

