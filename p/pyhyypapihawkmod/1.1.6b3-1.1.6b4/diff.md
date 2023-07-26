# Comparing `tmp/pyhyypapihawkmod-1.1.6b3.tar.gz` & `tmp/pyhyypapihawkmod-1.1.6b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.6b3.tar", last modified: Wed Jul 26 14:46:22 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.6b4.tar", last modified: Wed Jul 26 15:22:54 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.6b3.tar` & `pyhyypapihawkmod-1.1.6b4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 14:46:22.900594 pyhyypapihawkmod-1.1.6b3/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-26 14:46:22.899594 pyhyypapihawkmod-1.1.6b3/PKG-INFO
--rw-rw-rw-   0        0        0     2024 2023-07-26 14:45:08.000000 pyhyypapihawkmod-1.1.6b3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 14:46:22.883602 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     9703 2023-07-26 14:43:59.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    29484 2023-07-26 14:07:07.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 14:46:22.897597 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-26 14:46:22.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-26 14:46:22.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 14:46:22.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-26 14:46:22.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 14:46:22.000000 pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 14:46:22.900594 pyhyypapihawkmod-1.1.6b3/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-26 06:19:37.000000 pyhyypapihawkmod-1.1.6b3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:22:54.037267 pyhyypapihawkmod-1.1.6b4/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b4/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b4/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-26 15:22:54.036270 pyhyypapihawkmod-1.1.6b4/PKG-INFO
+-rw-rw-rw-   0        0        0     2024 2023-07-26 14:45:08.000000 pyhyypapihawkmod-1.1.6b4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 15:22:54.020768 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     9787 2023-07-26 15:14:04.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    29484 2023-07-26 15:22:30.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4027 2023-07-26 15:22:07.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:22:54.033770 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-26 15:22:53.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-26 15:22:53.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 15:22:53.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-26 15:22:53.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 15:22:53.000000 pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 15:22:54.037771 pyhyypapihawkmod-1.1.6b4/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-26 15:22:35.000000 pyhyypapihawkmod-1.1.6b4/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.6b3/LICENSE.md` & `pyhyypapihawkmod-1.1.6b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b3/PKG-INFO` & `pyhyypapihawkmod-1.1.6b4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b3
+Version: 1.1.6b4
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b3/README.md` & `pyhyypapihawkmod-1.1.6b4/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/alarm_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,14 @@
         }
         
         for site in site_ids:
             
             self._fetch_notifications(site_id=site)
             triggered_zones = self._triggered_zones()
             zone_states = self._client.get_zone_state_info(site_id=site)
-
             # Add last site notification.
             _last_notice = self._last_notice()
             site_ids[site]["lastNoticeTime"] = _last_notice["lastNoticeTime"]
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
 
             # Add triggers (PGM / Automations in APP)
             site_ids[site]["triggers"] = {}
@@ -161,14 +160,16 @@
 
 
 
                 # New zone information from IDS servers
                 
                 # add zone bypass info to zone
                 for zone in site_ids[site]["partitions"][partition]["zones"]:
+                    if "zones" not in zone_states:
+                        continue
                     for zone_state in zone_states["zones"]:
                         if site_ids[site]["partitions"][partition]["zones"][zone][
                             "number"] != zone_state["number"]:
                             continue
                         site_ids[site]["partitions"][partition]["zones"][zone][
                             "bypassed"] = bool(zone_state["bypassed"])
                         site_ids[site]["partitions"][partition]["zones"][zone][
```

### Comparing `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     "appVersionCode": "401",
     "_appVersionCode": "401",
     "deviceOS": "12.0",
     "deviceName": "Python API",
     "pkg": "za.co.adt.securehome.android",
     "_appVersionName": "3.5.19",
     "token": None,
+    "userId" : None,
 }  # Standard request parameters.
 
 # Rpc to name mapping. Used in push notifications.
 RpcCodes = {
     "202": "IMEI unknown to SMART platform. Registration failed.",
     "203": "Command failed",
     "204": "VALUE is invalid",
```

### Comparing `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b3
+Version: 1.1.6b4
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b3/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.6b4/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b3/setup.py` & `pyhyypapihawkmod-1.1.6b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.6b3",
+    version="1.1.6b4",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

