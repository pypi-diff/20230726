# Comparing `tmp/pyinels-0.6.8.tar.gz` & `tmp/pyinels-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinels-0.6.8.tar", last modified: Wed Dec  1 23:22:30 2021, max compression
+gzip compressed data, was "pyinels-0.6.9.tar", last modified: Tue Dec  7 09:37:40 2021, max compression
```

## Comparing `pyinels-0.6.8.tar` & `pyinels-0.6.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-01 23:22:30.218916 pyinels-0.6.8/
--rw-r--r--   0 vsts      (1001) docker     (116)     1093 2021-12-01 23:22:10.000000 pyinels-0.6.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (116)       60 2021-12-01 23:22:10.000000 pyinels-0.6.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (116)     2119 2021-12-01 23:22:30.218916 pyinels-0.6.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)     1657 2021-12-01 23:22:10.000000 pyinels-0.6.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-01 23:22:30.214916 pyinels-0.6.8/pyinels/
--rw-r--r--   0 vsts      (1001) docker     (116)       95 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-01 23:22:30.214916 pyinels-0.6.8/pyinels/api/
--rw-r--r--   0 vsts      (1001) docker     (116)     7762 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4479 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/api/resources.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1634 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/const.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-01 23:22:30.218916 pyinels-0.6.8/pyinels/device/
--rw-r--r--   0 vsts      (1001) docker     (116)      406 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/device/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2195 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/device/pyBase.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1272 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/device/pyDoor.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1803 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/device/pyLight.py
--rw-r--r--   0 vsts      (1001) docker     (116)     6435 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/device/pyShutter.py
--rw-r--r--   0 vsts      (1001) docker     (116)      271 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/device/pySwitch.py
--rw-r--r--   0 vsts      (1001) docker     (116)      568 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/exception.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1668 2021-12-01 23:22:10.000000 pyinels-0.6.8/pyinels/pyTimer.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-01 23:22:30.214916 pyinels-0.6.8/pyinels.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (116)     2119 2021-12-01 23:22:30.000000 pyinels-0.6.8/pyinels.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (116)      751 2021-12-01 23:22:30.000000 pyinels-0.6.8/pyinels.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2021-12-01 23:22:30.000000 pyinels-0.6.8/pyinels.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        1 2021-12-01 23:22:30.000000 pyinels-0.6.8/pyinels.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (116)       14 2021-12-01 23:22:30.000000 pyinels-0.6.8/pyinels.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (116)        0 2021-12-01 23:22:10.000000 pyinels-0.6.8/requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (116)      118 2021-12-01 23:22:30.218916 pyinels-0.6.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (116)      878 2021-12-01 23:22:10.000000 pyinels-0.6.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-01 23:22:30.218916 pyinels-0.6.8/tests/
--rw-r--r--   0 vsts      (1001) docker     (116)       36 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (116)     5027 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/api_test.py
--rw-r--r--   0 vsts      (1001) docker     (116)     6663 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/const_test.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2870 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/door_test.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1200 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/examples.py
--rw-r--r--   0 vsts      (1001) docker     (116)     6166 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/light_test.py
--rw-r--r--   0 vsts      (1001) docker     (116)     3351 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/production_test.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2200 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/real_worl_test.py
--rw-r--r--   0 vsts      (1001) docker     (116)     4299 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/resource_test.py
--rw-r--r--   0 vsts      (1001) docker     (116)     6126 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/shutter_test.py
--rw-r--r--   0 vsts      (1001) docker     (116)     2975 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/switch_test.py
--rw-r--r--   0 vsts      (1001) docker     (116)     1377 2021-12-01 23:22:10.000000 pyinels-0.6.8/tests/timer_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-07 09:37:40.768143 pyinels-0.6.9/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1093 2021-12-07 09:37:22.000000 pyinels-0.6.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (116)       60 2021-12-07 09:37:22.000000 pyinels-0.6.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (116)     2119 2021-12-07 09:37:40.768143 pyinels-0.6.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)     1657 2021-12-07 09:37:22.000000 pyinels-0.6.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-07 09:37:40.764142 pyinels-0.6.9/pyinels/
+-rw-r--r--   0 vsts      (1001) docker     (116)       95 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-07 09:37:40.768143 pyinels-0.6.9/pyinels/api/
+-rw-r--r--   0 vsts      (1001) docker     (116)     7762 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4479 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/api/resources.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1634 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/const.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-07 09:37:40.768143 pyinels-0.6.9/pyinels/device/
+-rw-r--r--   0 vsts      (1001) docker     (116)      406 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/device/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2195 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/device/pyBase.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1272 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/device/pyDoor.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1803 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/device/pyLight.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3789 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/device/pyShutter.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      271 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/device/pySwitch.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      568 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/exception.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1668 2021-12-07 09:37:22.000000 pyinels-0.6.9/pyinels/pyTimer.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-07 09:37:40.768143 pyinels-0.6.9/pyinels.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (116)     2119 2021-12-07 09:37:40.000000 pyinels-0.6.9/pyinels.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)      751 2021-12-07 09:37:40.000000 pyinels-0.6.9/pyinels.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2021-12-07 09:37:40.000000 pyinels-0.6.9/pyinels.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2021-12-07 09:37:40.000000 pyinels-0.6.9/pyinels.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (116)       14 2021-12-07 09:37:40.000000 pyinels-0.6.9/pyinels.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        0 2021-12-07 09:37:22.000000 pyinels-0.6.9/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      118 2021-12-07 09:37:40.768143 pyinels-0.6.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (116)      878 2021-12-07 09:37:22.000000 pyinels-0.6.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2021-12-07 09:37:40.768143 pyinels-0.6.9/tests/
+-rw-r--r--   0 vsts      (1001) docker     (116)       36 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5027 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/api_test.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6663 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/const_test.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2870 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/door_test.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1200 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/examples.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6166 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/light_test.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3351 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/production_test.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2200 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/real_worl_test.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4299 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/resource_test.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3666 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/shutter_test.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2975 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/switch_test.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1377 2021-12-07 09:37:22.000000 pyinels-0.6.9/tests/timer_test.py
```

### Comparing `pyinels-0.6.8/LICENSE` & `pyinels-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/PKG-INFO` & `pyinels-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinels
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python library for iNels BUS
 Home-page: https://github.com/JH-Soft-Technology/pyinels
 Author: JH Soft Technology
 Author-email: horalek.jiri@gmail.com
 License: MIT
 Keywords: iNels,Elko EP,Home assistant integration
 Platform: UNKNOWN
```

### Comparing `pyinels-0.6.8/README.md` & `pyinels-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/pyinels/api/__init__.py` & `pyinels-0.6.9/pyinels/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/pyinels/api/resources.py` & `pyinels-0.6.9/pyinels/api/resources.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/pyinels/const.py` & `pyinels-0.6.9/pyinels/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,8 +75,8 @@
 SUPPORT_STOP_TILT = 64
 
 STATE_OPEN = "open"
 STATE_OPENING = "opening"
 STATE_CLOSED = "closed"
 STATE_CLOSING = "closing"
 
-VERSION = "0.6.8"
+VERSION = "0.6.9"
```

### Comparing `pyinels-0.6.8/pyinels/device/pyBase.py` & `pyinels-0.6.9/pyinels/device/pyBase.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/pyinels/device/pyDoor.py` & `pyinels-0.6.9/pyinels/device/pyDoor.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/pyinels/device/pyLight.py` & `pyinels-0.6.9/pyinels/device/pyLight.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/pyinels/exception.py` & `pyinels-0.6.9/pyinels/exception.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/pyinels/pyTimer.py` & `pyinels-0.6.9/pyinels/pyTimer.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/pyinels.egg-info/PKG-INFO` & `pyinels-0.6.9/pyinels.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinels
-Version: 0.6.8
+Version: 0.6.9
 Summary: Python library for iNels BUS
 Home-page: https://github.com/JH-Soft-Technology/pyinels
 Author: JH Soft Technology
 Author-email: horalek.jiri@gmail.com
 License: MIT
 Keywords: iNels,Elko EP,Home assistant integration
 Platform: UNKNOWN
```

### Comparing `pyinels-0.6.8/pyinels.egg-info/SOURCES.txt` & `pyinels-0.6.9/pyinels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/setup.py` & `pyinels-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/tests/api_test.py` & `pyinels-0.6.9/tests/api_test.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/tests/const_test.py` & `pyinels-0.6.9/tests/const_test.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/tests/door_test.py` & `pyinels-0.6.9/tests/door_test.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/tests/examples.py` & `pyinels-0.6.9/tests/examples.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/tests/light_test.py` & `pyinels-0.6.9/tests/light_test.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/tests/production_test.py` & `pyinels-0.6.9/tests/production_test.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/tests/real_worl_test.py` & `pyinels-0.6.9/tests/real_worl_test.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/tests/resource_test.py` & `pyinels-0.6.9/tests/resource_test.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/tests/switch_test.py` & `pyinels-0.6.9/tests/switch_test.py`

 * *Files identical despite different names*

### Comparing `pyinels-0.6.8/tests/timer_test.py` & `pyinels-0.6.9/tests/timer_test.py`

 * *Files identical despite different names*

