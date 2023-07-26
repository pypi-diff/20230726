# Comparing `tmp/pyhyypapihawkmod-1.1.6b21.tar.gz` & `tmp/pyhyypapihawkmod-1.1.6b22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.6b21.tar", last modified: Wed Jul 26 21:09:48 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.6b22.tar", last modified: Wed Jul 26 21:31:20 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.6b21.tar` & `pyhyypapihawkmod-1.1.6b22.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 21:09:48.212824 pyhyypapihawkmod-1.1.6b21/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/MANIFEST.in
--rw-rw-rw-   0        0        0      520 2023-07-26 21:09:48.211811 pyhyypapihawkmod-1.1.6b21/PKG-INFO
--rw-rw-rw-   0        0        0     2047 2023-07-26 20:04:50.000000 pyhyypapihawkmod-1.1.6b21/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 21:09:48.198083 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0    10144 2023-07-26 21:09:11.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27868 2023-07-26 20:03:06.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-07-26 20:03:06.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 21:09:48.210255 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      520 2023-07-26 21:09:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-26 21:09:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 21:09:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-26 21:09:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 21:09:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 21:09:48.212824 pyhyypapihawkmod-1.1.6b21/setup.cfg
--rw-rw-rw-   0        0        0      924 2023-07-26 21:09:22.000000 pyhyypapihawkmod-1.1.6b21/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 21:31:20.841059 pyhyypapihawkmod-1.1.6b22/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b22/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b22/MANIFEST.in
+-rw-rw-rw-   0        0        0      520 2023-07-26 21:31:20.840049 pyhyypapihawkmod-1.1.6b22/PKG-INFO
+-rw-rw-rw-   0        0        0     2047 2023-07-26 20:04:50.000000 pyhyypapihawkmod-1.1.6b22/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 21:31:20.829445 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     9152 2023-07-26 21:30:56.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27868 2023-07-26 20:03:06.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-07-26 20:03:06.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 21:31:20.839039 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-07-26 21:31:20.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-26 21:31:20.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 21:31:20.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-26 21:31:20.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 21:31:20.000000 pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 21:31:20.841059 pyhyypapihawkmod-1.1.6b22/setup.cfg
+-rw-rw-rw-   0        0        0      924 2023-07-26 21:31:03.000000 pyhyypapihawkmod-1.1.6b22/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.6b21/LICENSE.md` & `pyhyypapihawkmod-1.1.6b22/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b21/PKG-INFO` & `pyhyypapihawkmod-1.1.6b22/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b21
+Version: 1.1.6b22
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b21/README.md` & `pyhyypapihawkmod-1.1.6b22/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/alarm_info.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,48 +19,20 @@
         """init."""
         self._client = client
         self._sync_info: dict = {}
         self._state_info: dict = {}
         self._notifications: dict = {}
         self._scheduled_task_list = []
         self._last_notification_check_timestamp = 0
-        self.startup = True
-        self.timer = thread.Timer(0.01, function=self._fetch_data_executer)
-        self.timer.start() 
 
     def _fetch_data_sync_and_state(self) -> None:
         
-        self._fetch_data_scheduler(self._fetch_sync_info, '')
-        self._fetch_data_scheduler(self._fetch_state_info, '')
+        thread.Timer(0.01, lambda:  self._fetch_sync_info() ).start()
+        thread.Timer(0.01, lambda:  self._fetch_state_info() ).start()
       
-    def _fetch_data_scheduler(self, function, parameters):
-        
-        element = [function, parameters]
-        self._scheduled_task_list.append(element)
-
-    def _fetch_data_executer(self):
-        
-        tasklist = []
-        task_number = 0
-        POLLING_DELAY = 1.1
-        while 1:
-            while task_number < len(tasklist):
-                tasklist[task_number][0](tasklist[task_number][1])
-                time.sleep(POLLING_DELAY)
-                task_number += 1
-                tasklist = self._scheduled_task_list
-            if len(tasklist) == 0:
-                time.sleep(POLLING_DELAY)
-                tasklist = self._scheduled_task_list
-            else:
-                tasklist = []
-                self._scheduled_task_list = []
-                task_number = 0
-                self.startup = False
-            
      
     def _fetch_sync_info(self, place = None):
         self._sync_info = self._client.get_sync_info()
         print("sync")
         
     def _fetch_state_info(self, place = None):
         self._state_info = self._client.get_state_info()
@@ -128,17 +100,14 @@
      
      
     def _format_data(self) -> dict[Any, Any]:
         """Format data for Hass."""
 
         # The API returns data from site level.
         # Partitions are used as entity that actions are performed on.
-
-        if self.startup:
-            return {}
         
         site_ids = {site["id"]: site for site in self._sync_info["sites"]}
         zone_ids = {zone["id"]: zone for zone in self._sync_info["zones"]}
         stay_ids = {
             stay_profile["id"]: stay_profile
             for stay_profile in self._sync_info["stayProfiles"]
         }
@@ -148,15 +117,16 @@
         
         trigger_ids = {
             trigger["id"]: trigger for trigger in self._sync_info["triggers"]
         }
         
         for site in site_ids:
             
-            self._fetch_data_scheduler(function=self._fetch_notifications, parameters=site)
+            
+            thread.Timer(0.01, lambda:  self._fetch_notifications(site) ).start()
             #self._fetch_notifications(site_id=site)
             triggered_zones = self._triggered_zones()
 
             # Add last site notification.
             _last_notice = self._last_notice()
             site_ids[site]["lastNoticeTime"] = _last_notice["lastNoticeTime"]
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
@@ -251,15 +221,16 @@
 
 
 
     def debug_notifications(self) -> dict[Any, Any]:
         """Pull notifications for debug purposes."""
         # The API returns data from site level.
 
-        self._fetch_data()
+        #self._fetch_data()
+        self._fetch_data_sync_and_state()
         site_ids = {site["id"]: site for site in self._sync_info["sites"]}
         
         for site in site_ids:
             self._fetch_notifications(site_id=site)
             site_ids[site] = self._notifications
```

### Comparing `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b21
+Version: 1.1.6b22
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.6b22/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b21/setup.py` & `pyhyypapihawkmod-1.1.6b22/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.6b21",
+    version="1.1.6b22",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

