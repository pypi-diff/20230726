# Comparing `tmp/zlgsendcan-1.1.2.tar.gz` & `tmp/zlgsendcan-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.1.2.tar", last modified: Wed Jul 26 09:09:22 2023, max compression
+gzip compressed data, was "zlgsendcan-1.1.3.tar", last modified: Wed Jul 26 09:36:47 2023, max compression
```

## Comparing `zlgsendcan-1.1.2.tar` & `zlgsendcan-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:09:22.117669 zlgsendcan-1.1.2/
--rw-rw-rw-   0        0        0      220 2023-07-26 09:09:22.116670 zlgsendcan-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 09:09:22.117669 zlgsendcan-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      463 2023-07-26 09:09:16.000000 zlgsendcan-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:09:22.109890 zlgsendcan-1.1.2/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.2/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.2/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.2/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.1.2/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.2/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    24969 2023-07-26 06:37:07.000000 zlgsendcan-1.1.2/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.1.2/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:09:22.115689 zlgsendcan-1.1.2/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-26 09:09:22.000000 zlgsendcan-1.1.2/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-26 09:09:22.000000 zlgsendcan-1.1.2/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:09:22.000000 zlgsendcan-1.1.2/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 09:09:22.000000 zlgsendcan-1.1.2/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 09:09:22.000000 zlgsendcan-1.1.2/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 09:36:47.706282 zlgsendcan-1.1.3/
+-rw-rw-rw-   0        0        0      220 2023-07-26 09:36:47.706282 zlgsendcan-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 09:36:47.707282 zlgsendcan-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      463 2023-07-26 09:36:43.000000 zlgsendcan-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:36:47.698282 zlgsendcan-1.1.3/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.3/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.3/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.3/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.1.3/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.3/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    25077 2023-07-26 09:27:40.000000 zlgsendcan-1.1.3/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.1.3/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:36:47.705282 zlgsendcan-1.1.3/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-26 09:36:47.000000 zlgsendcan-1.1.3/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-26 09:36:47.000000 zlgsendcan-1.1.3/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:36:47.000000 zlgsendcan-1.1.3/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 09:36:47.000000 zlgsendcan-1.1.3/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 09:36:47.000000 zlgsendcan-1.1.3/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.1.2/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.1.3/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.2/zlgsendcan/parseDBC.py` & `zlgsendcan-1.1.3/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.2/zlgsendcan/yaml_util.py` & `zlgsendcan-1.1.3/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.2/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.1.3/zlgsendcan/zlgcan1.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 #  ------------------------------------------------------------------
 #
 import os
 import sys
 from ctypes import *
 import platform
 from zlgsendcan import frozen_dir
+import pkg_resources
 
 SETUP_DIR = frozen_dir.app_path() + r'\zlgcan_1.dll'
 sys.path.append(SETUP_DIR)
 
 ZCAN_DEVICE_TYPE = c_uint
 
 INVALID_DEVICE_HANDLE = 0
@@ -324,15 +325,16 @@
     def __init__(self):
         if platform.system() == "Windows":
             try:
                 base_path = sys._MEIPASS
             except Exception:
                 base_path = os.path.abspath('..')
             dll_path = os.path.join(base_path, 'zlgcan_1.dll')
-            dll_path = os.path.join('D:\\auto-qt\\newauto\zlgcan_1.dll')
+            # dll_path = os.path.join('D:\\auto-qt\\newauto\zlgcan_1.dll')
+            dll_path = pkg_resources.resource_filename('zlgsendcan', 'zlgcan_1.dll')
             self.__dll = windll.LoadLibrary(dll_path)
 
         else:
             print("No support now!")
         if self.__dll == None:
             print("DLL couldn't be loaded!")
```

### Comparing `zlgsendcan-1.1.2/zlgsendcan/zlgserver.py` & `zlgsendcan-1.1.3/zlgsendcan/zlgserver.py`

 * *Files identical despite different names*

