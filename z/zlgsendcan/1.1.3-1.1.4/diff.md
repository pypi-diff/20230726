# Comparing `tmp/zlgsendcan-1.1.3.tar.gz` & `tmp/zlgsendcan-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zlgsendcan-1.1.3.tar", last modified: Wed Jul 26 09:36:47 2023, max compression
+gzip compressed data, was "zlgsendcan-1.1.4.tar", last modified: Wed Jul 26 09:43:01 2023, max compression
```

## Comparing `zlgsendcan-1.1.3.tar` & `zlgsendcan-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:36:47.706282 zlgsendcan-1.1.3/
--rw-rw-rw-   0        0        0      220 2023-07-26 09:36:47.706282 zlgsendcan-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 09:36:47.707282 zlgsendcan-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      463 2023-07-26 09:36:43.000000 zlgsendcan-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:36:47.698282 zlgsendcan-1.1.3/zlgsendcan/
--rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.3/zlgsendcan/__init__.py
--rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.3/zlgsendcan/frozen_dir.py
--rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.3/zlgsendcan/get_conf_info.py
--rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.1.3/zlgsendcan/parseDBC.py
--rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.3/zlgsendcan/yaml_util.py
--rw-rw-rw-   0        0        0    25077 2023-07-26 09:27:40.000000 zlgsendcan-1.1.3/zlgsendcan/zlgcan1.py
--rw-rw-rw-   0        0        0    18573 2023-07-26 06:37:07.000000 zlgsendcan-1.1.3/zlgsendcan/zlgserver.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:36:47.705282 zlgsendcan-1.1.3/zlgsendcan.egg-info/
--rw-rw-rw-   0        0        0      220 2023-07-26 09:36:47.000000 zlgsendcan-1.1.3/zlgsendcan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-07-26 09:36:47.000000 zlgsendcan-1.1.3/zlgsendcan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:36:47.000000 zlgsendcan-1.1.3/zlgsendcan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-26 09:36:47.000000 zlgsendcan-1.1.3/zlgsendcan.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 09:36:47.000000 zlgsendcan-1.1.3/zlgsendcan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 09:43:01.279761 zlgsendcan-1.1.4/
+-rw-rw-rw-   0        0        0      220 2023-07-26 09:43:01.279761 zlgsendcan-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 09:43:01.280761 zlgsendcan-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      463 2023-07-26 09:42:56.000000 zlgsendcan-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:43:01.269755 zlgsendcan-1.1.4/zlgsendcan/
+-rw-rw-rw-   0        0        0        0 2023-07-26 06:34:10.000000 zlgsendcan-1.1.4/zlgsendcan/__init__.py
+-rw-rw-rw-   0        0        0      237 2023-02-14 03:41:12.000000 zlgsendcan-1.1.4/zlgsendcan/frozen_dir.py
+-rw-rw-rw-   0        0        0     3026 2023-07-26 09:03:48.000000 zlgsendcan-1.1.4/zlgsendcan/get_conf_info.py
+-rw-rw-rw-   0        0        0     5211 2023-07-19 02:48:32.000000 zlgsendcan-1.1.4/zlgsendcan/parseDBC.py
+-rw-rw-rw-   0        0        0     1122 2023-07-26 08:41:01.000000 zlgsendcan-1.1.4/zlgsendcan/yaml_util.py
+-rw-rw-rw-   0        0        0    25077 2023-07-26 09:27:40.000000 zlgsendcan-1.1.4/zlgsendcan/zlgcan1.py
+-rw-rw-rw-   0        0        0    18584 2023-07-26 09:42:40.000000 zlgsendcan-1.1.4/zlgsendcan/zlgserver.py
+drwxrwxrwx   0        0        0        0 2023-07-26 09:43:01.277760 zlgsendcan-1.1.4/zlgsendcan.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-07-26 09:43:01.000000 zlgsendcan-1.1.4/zlgsendcan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-26 09:43:01.000000 zlgsendcan-1.1.4/zlgsendcan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 09:43:01.000000 zlgsendcan-1.1.4/zlgsendcan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 09:43:01.000000 zlgsendcan-1.1.4/zlgsendcan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 09:43:01.000000 zlgsendcan-1.1.4/zlgsendcan.egg-info/top_level.txt
```

### Comparing `zlgsendcan-1.1.3/zlgsendcan/get_conf_info.py` & `zlgsendcan-1.1.4/zlgsendcan/get_conf_info.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.3/zlgsendcan/parseDBC.py` & `zlgsendcan-1.1.4/zlgsendcan/parseDBC.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.3/zlgsendcan/yaml_util.py` & `zlgsendcan-1.1.4/zlgsendcan/yaml_util.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.3/zlgsendcan/zlgcan1.py` & `zlgsendcan-1.1.4/zlgsendcan/zlgcan1.py`

 * *Files identical despite different names*

### Comparing `zlgsendcan-1.1.3/zlgsendcan/zlgserver.py` & `zlgsendcan-1.1.4/zlgsendcan/zlgserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 import importlib
 import time
 from PyQt5.QtWidgets import QMessageBox
 from zlgsendcan.parseDBC import GlobleValue, DbcInit
-from zlgcan1 import *
+from zlgsendcan.zlgcan1 import *
 import threading
 from zlgsendcan.get_conf_info import GetBaseInfo
 data_ = GetBaseInfo().get_base_config()
 condition = threading.Condition()
 
 
 class MessageDate:
```

