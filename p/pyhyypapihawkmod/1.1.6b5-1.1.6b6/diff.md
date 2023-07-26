# Comparing `tmp/pyhyypapihawkmod-1.1.6b5.tar.gz` & `tmp/pyhyypapihawkmod-1.1.6b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.6b5.tar", last modified: Wed Jul 26 15:36:21 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.6b6.tar", last modified: Wed Jul 26 15:43:36 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.6b5.tar` & `pyhyypapihawkmod-1.1.6b6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 15:36:21.290314 pyhyypapihawkmod-1.1.6b5/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b5/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b5/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-26 15:36:21.289811 pyhyypapihawkmod-1.1.6b5/PKG-INFO
--rw-rw-rw-   0        0        0     2024 2023-07-26 14:45:08.000000 pyhyypapihawkmod-1.1.6b5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 15:36:21.272706 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     9787 2023-07-26 15:14:04.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    29518 2023-07-26 15:35:57.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4027 2023-07-26 15:22:07.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 15:36:21.286316 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-26 15:36:21.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-26 15:36:21.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 15:36:21.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-26 15:36:21.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 15:36:21.000000 pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 15:36:21.290814 pyhyypapihawkmod-1.1.6b5/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-26 15:36:02.000000 pyhyypapihawkmod-1.1.6b5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:43:36.003079 pyhyypapihawkmod-1.1.6b6/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b6/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b6/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-26 15:43:36.002581 pyhyypapihawkmod-1.1.6b6/PKG-INFO
+-rw-rw-rw-   0        0        0     2024 2023-07-26 14:45:08.000000 pyhyypapihawkmod-1.1.6b6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 15:43:35.987863 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     9787 2023-07-26 15:14:04.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    29544 2023-07-26 15:43:06.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4027 2023-07-26 15:22:07.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:43:36.000082 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-26 15:43:35.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-26 15:43:35.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 15:43:35.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-26 15:43:35.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 15:43:35.000000 pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 15:43:36.003079 pyhyypapihawkmod-1.1.6b6/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-26 15:43:13.000000 pyhyypapihawkmod-1.1.6b6/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.6b5/LICENSE.md` & `pyhyypapihawkmod-1.1.6b6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b5/PKG-INFO` & `pyhyypapihawkmod-1.1.6b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b5
+Version: 1.1.6b6
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b5/README.md` & `pyhyypapihawkmod-1.1.6b6/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/alarm_info.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,17 +46,17 @@
         token: str | None = None,
     ) -> None:
         """Initialize the client object."""
         self._email = email
         self._password = password
         self._session = requests.session()
         self._session.headers.update(REQUEST_HEADER)
+        self._userid = userid
         STD_PARAMS["pkg"] = pkg
         STD_PARAMS["token"] = token
-        STD_PARAMS["userId"] = userid
         self._timeout = timeout
 
     def login(self) -> Any:
         """Login to ADT Secure Home API."""
 
         _params = STD_PARAMS.copy()
         _params["email"] = self._email
@@ -89,15 +89,15 @@
                 + str(req.text)
             ) from err
 
         if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
             raise HyypApiError(f"Login error: {_json_result['error']}")
 
         STD_PARAMS["token"] = _json_result["token"]
-        STD_PARAMS["userId"] = _json_result["user"]["id"]
+        self._userid = _json_result["user"]["id"]
 
         return _json_result
 
     def check_app_version(self) -> Any:
         """Check App version via API."""
 
         _params = STD_PARAMS.copy()
@@ -293,14 +293,15 @@
 
 
     def get_zone_state_info(self, site_id: int, json_key: str | None = None) -> Any:
         """Get state info from API. Returns armed, bypassed partition ids."""
 
         _params: dict[str, Any] = STD_PARAMS.copy()
         _params["siteId"] = site_id
+        _params["userId"] = self._userid
         print(_params)
         try:
             req = self._session.get(
                 "https://" + BASE_URL + API_ENDPOINT_GET_ZONE_STATE_INFO,
                 allow_redirects=False,
                 params=_params,
                 timeout=self._timeout,
```

### Comparing `pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b5
+Version: 1.1.6b6
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b5/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.6b6/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b5/setup.py` & `pyhyypapihawkmod-1.1.6b6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.6b5",
+    version="1.1.6b6",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

