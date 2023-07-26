# Comparing `tmp/pyhyypapihawkmod-1.1.6b8.tar.gz` & `tmp/pyhyypapihawkmod-1.1.6b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.6b8.tar", last modified: Wed Jul 26 16:14:40 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.6b9.tar", last modified: Wed Jul 26 16:27:25 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.6b8.tar` & `pyhyypapihawkmod-1.1.6b9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:40.896236 pyhyypapihawkmod-1.1.6b8/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b8/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b8/MANIFEST.in
--rw-rw-rw-   0        0        0      519 2023-07-26 16:14:40.895081 pyhyypapihawkmod-1.1.6b8/PKG-INFO
--rw-rw-rw-   0        0        0     2024 2023-07-26 14:45:08.000000 pyhyypapihawkmod-1.1.6b8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:40.878451 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     9922 2023-07-26 16:13:45.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    29460 2023-07-26 16:06:03.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-07-26 15:45:45.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:14:40.892094 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      519 2023-07-26 16:14:40.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-26 16:14:40.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:14:40.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-26 16:14:40.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 16:14:40.000000 pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 16:14:40.896731 pyhyypapihawkmod-1.1.6b8/setup.cfg
--rw-rw-rw-   0        0        0      923 2023-07-26 16:14:10.000000 pyhyypapihawkmod-1.1.6b8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:27:25.104334 pyhyypapihawkmod-1.1.6b9/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b9/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b9/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-07-26 16:27:25.088365 pyhyypapihawkmod-1.1.6b9/PKG-INFO
+-rw-rw-rw-   0        0        0     2024 2023-07-26 14:45:08.000000 pyhyypapihawkmod-1.1.6b9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 16:27:25.056045 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     9953 2023-07-26 16:27:06.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    29460 2023-07-26 16:06:03.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-07-26 15:45:45.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:27:25.083369 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-26 16:27:24.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-26 16:27:25.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 16:27:24.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-26 16:27:24.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 16:27:24.000000 pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 16:27:25.105339 pyhyypapihawkmod-1.1.6b9/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-07-26 16:25:14.000000 pyhyypapihawkmod-1.1.6b9/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.6b8/LICENSE.md` & `pyhyypapihawkmod-1.1.6b9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b8/PKG-INFO` & `pyhyypapihawkmod-1.1.6b9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b8
+Version: 1.1.6b9
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b8/README.md` & `pyhyypapihawkmod-1.1.6b9/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/alarm_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,16 @@
             trigger["id"]: trigger for trigger in self._sync_info["triggers"]
         }
         
         for site in site_ids:
             
             self._fetch_notifications(site_id=site)
             triggered_zones = self._triggered_zones()
-            zone_states = self._client.get_zone_state_info(site_id=site)
+            #zone_states = self._client.get_zone_state_info(site_id=site)
+            zone_states = {}
             # Add last site notification.
             _last_notice = self._last_notice()
             site_ids[site]["lastNoticeTime"] = _last_notice["lastNoticeTime"]
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
 
             # Add triggers (PGM / Automations in APP)
             site_ids[site]["triggers"] = {}
```

### Comparing `pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b8
+Version: 1.1.6b9
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b8/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.6b9/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b8/setup.py` & `pyhyypapihawkmod-1.1.6b9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.6b8",
+    version="1.1.6b9",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

