# Comparing `tmp/pyhyypapihawkmod-1.1.6b20.tar.gz` & `tmp/pyhyypapihawkmod-1.1.6b21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.6b20.tar", last modified: Wed Jul 26 19:21:49 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.6b21.tar", last modified: Wed Jul 26 21:09:48 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.6b20.tar` & `pyhyypapihawkmod-1.1.6b21.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 19:21:49.462267 pyhyypapihawkmod-1.1.6b20/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/MANIFEST.in
--rw-rw-rw-   0        0        0      520 2023-07-26 19:21:49.461760 pyhyypapihawkmod-1.1.6b20/PKG-INFO
--rw-rw-rw-   0        0        0     1940 2023-07-26 19:12:58.000000 pyhyypapihawkmod-1.1.6b20/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 19:21:49.449089 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     8641 2023-07-26 19:21:25.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27868 2023-07-26 19:12:58.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-07-26 19:12:58.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 19:21:49.460237 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      520 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 19:21:49.000000 pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 19:21:49.462267 pyhyypapihawkmod-1.1.6b20/setup.cfg
--rw-rw-rw-   0        0        0      924 2023-07-26 19:21:30.000000 pyhyypapihawkmod-1.1.6b20/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 21:09:48.212824 pyhyypapihawkmod-1.1.6b21/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/MANIFEST.in
+-rw-rw-rw-   0        0        0      520 2023-07-26 21:09:48.211811 pyhyypapihawkmod-1.1.6b21/PKG-INFO
+-rw-rw-rw-   0        0        0     2047 2023-07-26 20:04:50.000000 pyhyypapihawkmod-1.1.6b21/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 21:09:48.198083 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0    10144 2023-07-26 21:09:11.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27868 2023-07-26 20:03:06.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-07-26 20:03:06.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 21:09:48.210255 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-07-26 21:09:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-07-26 21:09:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 21:09:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-26 21:09:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 21:09:48.000000 pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 21:09:48.212824 pyhyypapihawkmod-1.1.6b21/setup.cfg
+-rw-rw-rw-   0        0        0      924 2023-07-26 21:09:22.000000 pyhyypapihawkmod-1.1.6b21/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.6b20/LICENSE.md` & `pyhyypapihawkmod-1.1.6b21/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/PKG-INFO` & `pyhyypapihawkmod-1.1.6b21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b20
+Version: 1.1.6b21
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b20/README.md` & `pyhyypapihawkmod-1.1.6b21/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 ```
 print(json.dumps(client.get_sync_info(),indent=2))
 
 ```
 
 Changelog 
 
+1.1.6b21
+- Test for polling scheduler (Delay polling)
+
+1.1.6b20
+- Hotfix for 0 length notifications
+
 1.1.6-b1
 - Test version
 - Will now show zones as bypassed when a stay arm bypassing zones is activated.
 
 1.1.5
 - Added functions to supply notifications for debugging when specifically called.
```

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.6b20
+Version: 1.1.6b21
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.6b20/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.6b21/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.6b20/setup.py` & `pyhyypapihawkmod-1.1.6b21/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.6b20",
+    version="1.1.6b21",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

