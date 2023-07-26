# Comparing `tmp/pyhyypapihawkmod-1.1.6b2.tar.gz` & `tmp/pyhyypapihawkmod-1.1.6b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.6b2.tar", last modified: Tue Jul 25 18:14:17 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.6b3.tar", last modified: Wed Jul 26 14:46:22 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.6b2.tar` & `pyhyypapihawkmod-1.1.6b3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 18:14:17.351897 pyhyypapihawkmod-1.1.6b2/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b2/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b2/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-25 18:14:17.351897 pyhyypapihawkmod-1.1.6b2/PKG-INFO
--rw-rw-rw-   0        0        0     1940 2023-07-25 16:40:14.000000 pyhyypapihawkmod-1.1.6b2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 18:14:17.338711 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     8558 2023-07-25 18:11:13.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27868 2023-07-25 16:40:24.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:14:17.349872 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-25 18:14:17.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-25 18:14:17.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 18:14:17.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-25 18:14:17.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-25 18:14:17.000000 pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 18:14:17.352906 pyhyypapihawkmod-1.1.6b2/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-25 18:11:23.000000 pyhyypapihawkmod-1.1.6b2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:46:22.900594 pyhyypapihawkmod-1.1.6b3/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-26 14:46:22.899594 pyhyypapihawkmod-1.1.6b3/PKG-INFO
+-rw-rw-rw-   0        0        0     2024 2023-07-26 14:45:08.000000 pyhyypapihawkmod-1.1.6b3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 14:46:22.883602 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     9703 2023-07-26 14:43:59.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    29484 2023-07-26 14:07:07.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:46:22.897597 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-26 14:46:22.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-26 14:46:22.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 14:46:22.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-26 14:46:22.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 14:46:22.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 14:46:22.900594 pyhyypapihawkmod-1.1.6b3/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-26 06:19:37.000000 pyhyypapihawkmod-1.1.6b3/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.6b2/LICENSE.md` & `pyhyypapihawkmod-1.1.6b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/PKG-INFO` & `pyhyypapihawkmod-1.1.6b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b2
+Version: 1.1.6b3
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b2/README.md` & `pyhyypapihawkmod-1.1.6b3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
 Changelog 
 
+1.1.6-b3
+- Zones now show openviolated and tempered information from IDS server
+
 1.1.6-b1
 - Test version
 - Will now show zones as bypassed when a stay arm bypassing zones is activated.
 
 1.1.5
 - Added functions to supply notifications for debugging when specifically called.
```

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/alarm_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         self._notifications: dict = {}
         self._last_notification_check_timestamp = 0
 
     def _fetch_data(self) -> None:
         """Fetch data via client api."""
         self._sync_info = self._client.get_sync_info()
         self._state_info = self._client.get_state_info()
+
         
     def _fetch_notifications(self, site_id: int) -> dict[Any,Any]:
         """Fetch and cache site notifications."""
         self._notifications = self._client.site_notifications(site_id=site_id)
 
 
     def _last_notice(self) -> dict[Any, Any]:
@@ -112,14 +113,15 @@
             trigger["id"]: trigger for trigger in self._sync_info["triggers"]
         }
         
         for site in site_ids:
             
             self._fetch_notifications(site_id=site)
             triggered_zones = self._triggered_zones()
+            zone_states = self._client.get_zone_state_info(site_id=site)
 
             # Add last site notification.
             _last_notice = self._last_notice()
             site_ids[site]["lastNoticeTime"] = _last_notice["lastNoticeTime"]
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
 
             # Add triggers (PGM / Automations in APP)
@@ -153,14 +155,32 @@
 
                 # Add zone bypass info to zone.
                 for zone in site_ids[site]["partitions"][partition]["zones"]:
                     site_ids[site]["partitions"][partition]["zones"][zone][
                         "bypassed"
                     ] = bool(zone in self._state_info["bypassedZoneIds"])
 
+
+
+                # New zone information from IDS servers
+                
+                # add zone bypass info to zone
+                for zone in site_ids[site]["partitions"][partition]["zones"]:
+                    for zone_state in zone_states["zones"]:
+                        if site_ids[site]["partitions"][partition]["zones"][zone][
+                            "number"] != zone_state["number"]:
+                            continue
+                        site_ids[site]["partitions"][partition]["zones"][zone][
+                            "bypassed"] = bool(zone_state["bypassed"])
+                        site_ids[site]["partitions"][partition]["zones"][zone][
+                            "openviolated"] = bool(zone_state["openViolated"])
+                        site_ids[site]["partitions"][partition]["zones"][zone][
+                            "tampered"] = bool(zone_state["tampered"])
+
+
                 # Add zone trigger info to zone (Zone triggered alarm).
                 for zone in site_ids[site]["partitions"][partition]["zones"]:
                     site_ids[site]["partitions"][partition]["zones"][zone][
                         "triggered"
                     ] = bool(zone in triggered_zones)
 
 
@@ -190,19 +210,20 @@
                     site_ids[site]["partitions"][partition]["stayArmedProfileName"] = (
                         site_ids[site]["partitions"][partition]["stayProfiles"][
                             stay_profile]["name"]
                     )
                     
                     # Show zone as bypassed if stay partition has it bypassed                 
                     for zone in site_ids[site]["partitions"][partition]["zones"]:
+                        bypassed_due_to_stay = zone in site_ids[site]["partitions"][partition]["stayProfiles"][stay_profile]['zoneIds']
+                        site_ids[site]["partitions"][partition]["zones"][zone]["stay_bypassed"] = bypassed_due_to_stay
                         site_ids[site]["partitions"][partition]["zones"][zone][
                         "bypassed"
-                        ] = bool(site_ids[site]["partitions"][partition]["zones"][zone]["bypassed"] or 
-                                 zone in site_ids[site]["partitions"][partition]["stayProfiles"][stay_profile]['zoneIds']
-                                 )
+                        ] = bool(site_ids[site]["partitions"][partition]["zones"][zone]["bypassed"] or bypassed_due_to_stay)
+                        
 
         return site_ids
 
     def status(self) -> dict[Any, Any]:
         """Return the status of Hyyp connected alarms."""
 
         self._fetch_data()
```

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,34 +26,37 @@
 API_ENDPOINT_ARM_SITE = "/device/armSite"
 API_ENDPOINT_TRIGGER_ALARM = "/device/triggerAlarm"
 API_ENDPOINT_SET_ZONE_BYPASS = "/device/bypass"
 API_ENDPOINT_GET_CAMERA_BY_PARTITION = "/device/getCameraByPartition"
 API_ENDPOINT_UPDATE_SUB_USER = "/user/updateSubUser"
 API_ENDPOINT_SET_NOTIFICATION_SUBSCRIPTIONS = "/user/setNotificationSubscriptionsNew"
 API_ENDPOINT_TRIGGER_AUTOMATION = "/device/trigger"
+API_ENDPOINT_GET_ZONE_STATE_INFO = "/device/getZoneStateInfo"
 
 
 class HyypClient:
     """Initialize api client object."""
 
     def __init__(
         self,
         email: str | None = None,
         password: str | None = None,
         pkg: str = HyypPkg.ADT_SECURE_HOME.value,
+        userid: int | None = None,
         timeout: int = DEFAULT_TIMEOUT,
         token: str | None = None,
     ) -> None:
         """Initialize the client object."""
         self._email = email
         self._password = password
         self._session = requests.session()
         self._session.headers.update(REQUEST_HEADER)
         STD_PARAMS["pkg"] = pkg
         STD_PARAMS["token"] = token
+        STD_PARAMS["userId"] = userid
         self._timeout = timeout
 
     def login(self) -> Any:
         """Login to ADT Secure Home API."""
 
         _params = STD_PARAMS.copy()
         _params["email"] = self._email
@@ -86,14 +89,15 @@
                 + str(req.text)
             ) from err
 
         if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
             raise HyypApiError(f"Login error: {_json_result['error']}")
 
         STD_PARAMS["token"] = _json_result["token"]
+        STD_PARAMS["userId"] = _json_result["user"]["id"]
 
         return _json_result
 
     def check_app_version(self) -> Any:
         """Check App version via API."""
 
         _params = STD_PARAMS.copy()
@@ -282,14 +286,62 @@
             )
 
         if json_key is None:
             return _json_result
 
         return _json_result[json_key]
 
+
+
+    def get_zone_state_info(self, site_id: int, json_key: str | None = None) -> Any:
+        """Get state info from API. Returns armed, bypassed partition ids."""
+
+        _params: dict[str, Any] = STD_PARAMS.copy()
+        _params["siteId"] = site_id
+
+        try:
+            req = self._session.get(
+                "https://" + BASE_URL + API_ENDPOINT_GET_ZONE_STATE_INFO,
+                allow_redirects=False,
+                params=_params,
+                timeout=self._timeout,
+            )
+
+            req.raise_for_status()
+
+        except requests.ConnectionError as err:
+            raise InvalidURL("A Invalid URL or Proxy error occured") from err
+
+        except requests.HTTPError as err:
+            raise HTTPError from err
+
+        try:
+            _json_result: dict[Any, Any] = req.json()
+
+        except ValueError as err:
+            raise HyypApiError(
+                "Impossible to decode response: "
+                + str(err)
+                + "\nResponse was: "
+                + str(req.text)
+            ) from err
+
+        if _json_result["status"] != "SUCCESS" and _json_result["error"] is not None:
+            raise HyypApiError(
+                f"Error getting zone state info from api: {_json_result['error']}"
+            )
+
+        if json_key is None:
+            return _json_result
+
+        return _json_result[json_key]
+
+
+
+
     def get_sync_info(self, json_key: str | None = None) -> Any:
         """Get user, site, partition and users info from API."""
 
         _params = STD_PARAMS
 
         try:
             req = self._session.get(
```

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b2
+Version: 1.1.6b3
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/setup.py` & `pyhyypapihawkmod-1.1.6b3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.6b2",
+    version="1.1.6b3",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

