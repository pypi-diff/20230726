# Comparing `tmp/pyhyypapihawkmod-1.1.6b2.tar.gz` & `tmp/pyhyypapihawkmod-1.1.6b20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.6b2.tar", last modified: Tue Jul 25 18:14:17 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.6b20.tar", last modified: Wed Jul 26 19:21:49 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.6b2.tar` & `pyhyypapihawkmod-1.1.6b20.tar`

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
+drwxrwxrwx   0        0        0        0 2023-07-26 19:21:49.462267 pyhyypapihawkmod-1.1.6b20/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/MANIFEST.in
+-rw-rw-rw-   0        0        0      520 2023-07-26 19:21:49.461760 pyhyypapihawkmod-1.1.6b20/PKG-INFO
+-rw-rw-rw-   0        0        0     1940 2023-07-26 19:12:58.000000 pyhyypapihawkmod-1.1.6b20/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 19:21:49.449089 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     8641 2023-07-26 19:21:25.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27868 2023-07-26 19:12:58.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-07-26 19:12:58.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:21:49.460237 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 19:21:49.462267 pyhyypapihawkmod-1.1.6b20/setup.cfg
+-rw-rw-rw-   0        0        0      924 2023-07-26 19:21:30.000000 pyhyypapihawkmod-1.1.6b20/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.6b2/LICENSE.md` & `pyhyypapihawkmod-1.1.6b20/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/PKG-INFO` & `pyhyypapihawkmod-1.1.6b20/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b2
+Version: 1.1.6b20
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b2/README.md` & `pyhyypapihawkmod-1.1.6b20/README.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/alarm_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,17 @@
         self._notifications = self._client.site_notifications(site_id=site_id)
 
 
     def _last_notice(self) -> dict[Any, Any]:
         """Get last notification."""
         _response: dict[Any, Any] = {"lastNoticeTime": None, "lastNoticeName": None}
 
+        if len(self._notifications) == 0:
+            return _response
+        
         _last_notification = self._notifications[0]
         
         if _last_notification:
 
             _last_event = _last_notification["eventNumber"]
             _last_event_datetime = str(
                 datetime.fromtimestamp(_last_notification["timestamp"] / 1000)
```

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b2
+Version: 1.1.6b20
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b2/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b2/setup.py` & `pyhyypapihawkmod-1.1.6b20/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.6b2",
+    version="1.1.6b20",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

