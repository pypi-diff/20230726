# Comparing `tmp/eagleeyev3-0.0.7.tar.gz` & `tmp/eagleeyev3-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eagleeyev3-0.0.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "eagleeyev3-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `eagleeyev3-0.0.7.tar` & `eagleeyev3-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      162 2023-07-24 21:05:15.503728 eagleeyev3-0.0.7/.gitignore
--rw-r--r--   0        0        0     1049 2023-07-18 18:55:59.571391 eagleeyev3-0.0.7/LICENSE
--rw-r--r--   0        0        0     1126 2023-07-25 16:21:45.463775 eagleeyev3-0.0.7/README.md
--rw-r--r--   0        0        0      380 2023-07-20 15:33:42.589081 eagleeyev3-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    27503 2023-07-25 16:25:06.684769 eagleeyev3-0.0.7/src/EagleEyev3/__init__.py
--rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 eagleeyev3-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      162 2023-07-24 21:05:15.503728 eagleeyev3-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1049 2023-07-18 18:55:59.571391 eagleeyev3-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1126 2023-07-25 16:21:45.463775 eagleeyev3-0.0.8/README.md
+-rw-r--r--   0        0        0      380 2023-07-20 15:33:42.589081 eagleeyev3-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    27419 2023-07-26 13:31:32.656024 eagleeyev3-0.0.8/src/EagleEyev3/__init__.py
+-rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 eagleeyev3-0.0.8/PKG-INFO
```

### Comparing `eagleeyev3-0.0.7/LICENSE` & `eagleeyev3-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `eagleeyev3-0.0.7/README.md` & `eagleeyev3-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `eagleeyev3-0.0.7/src/EagleEyev3/__init__.py` & `eagleeyev3-0.0.8/src/EagleEyev3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """ Python client for Eagle Eye Networks APIv3 """
-version = "0.0.7"
+version = "0.0.8"
 __version__ = version
 
 
 import json
 import logging
 import requests
 
@@ -272,15 +272,15 @@
             # Send a GET request to obtain the current user information
             response = requests.get(url, headers=headers, timeout=self._get_timeout_values('curent_user'))
             response_json = response.json()
 
             logging.info(f"{response.status_code} in get_current_user")
 
         except requests.exceptions.Timeout:
-            logging.warn(f"timeout expired for {self.id} get_current_user()")
+            logging.warn(f"timeout expired for get_current_user()")
             return {
                 "success": False,
                 "response_http_status": 0,
                 "data": None
             }
 
         except requests.exceptions.RequestException as e:
@@ -320,15 +320,15 @@
         try:
             response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_users'))
             response_json = response.json()
 
             logging.info(f"{response.status_code} in get_list_of_users")
 
         except requests.exceptions.Timeout:
-            logging.warn(f"timeout expired for {self.id} get_list_of_users()")
+            logging.warn(f"timeout expired for get_list_of_users()")
             return {
                 "success": False,
                 "response_http_status": 0,
                 "data": None
             }
 
         except requests.exceptions.RequestException as e:
@@ -367,15 +367,15 @@
         try:
             response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_cameras'))
             response_json = response.json()
 
             logging.info(f"{response.status_code} in get_list_of_cameras")
 
         except requests.exceptions.Timeout:
-            logging.warn(f"timeout expired for {self.id} get_list_of_cameras()")
+            logging.warn(f"timeout expired get_list_of_cameras()")
             return {
                 "success": False,
                 "response_http_status": 0,
                 "data": None
             }
 
         except requests.exceptions.RequestException as e:
@@ -424,15 +424,15 @@
         try:
             response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_bridges'))
             response_json = response.json()
 
             logging.info(f"{response.status_code} in get_list_of_bridges")
 
         except requests.exceptions.Timeout:
-            logging.warn(f"timeout expired for {self.id} get_list_of_bridges()")
+            logging.warn(f"timeout expired for get_list_of_bridges()")
             return {
                 "success": False,
                 "response_http_status": 0,
                 "data": None
             }
 
         except requests.exceptions.RequestException as e:
@@ -471,15 +471,15 @@
         try:
             response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_switches'))
             response_json = response.json()
 
             logging.info(f"{response.status_code} in get_list_of_switches")
 
         except requests.exceptions.Timeout:
-            logging.warn(f"timeout expired for {self.id} get_list_of_switches()")
+            logging.warn(f"timeout expired for get_list_of_switches()")
             return {
                 "success": False,
                 "response_http_status": 0,
                 "data": None
             }
 
         except requests.exceptions.RequestException as e:
@@ -518,15 +518,15 @@
         try:
             response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_available_devices'))
             response_json = response.json()
 
             logging.info(f"{response.status_code} in get_list_of_available_devices")
 
         except requests.exceptions.Timeout:
-            logging.warn(f"timeout expired for {self.id} get_list_of_available_devices()")
+            logging.warn(f"timeout expired for get_list_of_available_devices()")
             return {
                 "success": False,
                 "response_http_status": 0,
                 "data": None
             }
 
         except requests.exceptions.RequestException as e:
@@ -564,15 +564,15 @@
         try:
             response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_multi_cameras'))
             response_json = response.json()
 
             logging.info(f"{response.status_code} in get_list_of_multi_cameras")
 
         except requests.exceptions.Timeout:
-            logging.warn(f"timeout expired for {self.id} get_list_of_multi_cameras()")
+            logging.warn(f"timeout expired for get_list_of_multi_cameras()")
             return {
                 "success": False,
                 "response_http_status": 0,
                 "data": None
             }
 
         except requests.exceptions.RequestException as e:
@@ -610,15 +610,15 @@
         try:
             response = requests.get(url, headers=headers, timeout=self._get_timeout_values('list_of_feeds'))
             response_json = response.json()
 
             logging.info(f"{response.status_code} in get_list_of_feeds")
 
         except requests.exceptions.Timeout:
-            logging.warn(f"timeout expired for {self.id} get_list_of_feeds()")
+            logging.warn(f"timeout expired for get_list_of_feeds()")
             return {
                 "success": False,
                 "response_http_status": 0,
                 "data": None
             }
 
         except requests.exceptions.RequestException as e:
```

### Comparing `eagleeyev3-0.0.7/PKG-INFO` & `eagleeyev3-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EagleEyev3
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python client for Eagle Eye Networks APIv3 
 Author-email: mcotton <mcotton@mcottondesign.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Home, https://mcottondesign.com
 
 # EagleEyev3 #
```

