# Comparing `tmp/AppiumExtended-0.0.1.tar.gz` & `tmp/AppiumExtended-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppiumExtended-0.0.1.tar", last modified: Wed Jul 26 17:36:16 2023, max compression
+gzip compressed data, was "AppiumExtended-0.0.2.tar", last modified: Wed Jul 26 17:49:58 2023, max compression
```

## Comparing `AppiumExtended-0.0.1.tar` & `AppiumExtended-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.384794 AppiumExtended-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.328527 AppiumExtended-0.0.1/AppiumExtended/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:45.000000 AppiumExtended-0.0.1/AppiumExtended/__init__.py
--rw-rw-rw-   0        0        0     2694 2023-07-26 16:13:14.000000 AppiumExtended-0.0.1/AppiumExtended/appium_base.py
--rw-rw-rw-   0        0        0    28523 2023-07-26 16:28:56.000000 AppiumExtended-0.0.1/AppiumExtended/appium_extended.py
--rw-rw-rw-   0        0        0    15339 2023-07-26 16:28:56.000000 AppiumExtended-0.0.1/AppiumExtended/appium_get.py
--rw-rw-rw-   0        0        0     2505 2023-07-26 16:28:56.000000 AppiumExtended-0.0.1/AppiumExtended/appium_is.py
--rw-rw-rw-   0        0        0     2259 2023-07-26 16:28:56.000000 AppiumExtended-0.0.1/AppiumExtended/appium_swipe.py
--rw-rw-rw-   0        0        0     1888 2023-07-26 16:28:56.000000 AppiumExtended-0.0.1/AppiumExtended/appium_tap.py
--rw-rw-rw-   0        0        0     7107 2023-07-26 16:28:56.000000 AppiumExtended-0.0.1/AppiumExtended/appium_wait.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.337657 AppiumExtended-0.0.1/AppiumExtended.egg-info/
--rw-rw-rw-   0        0        0      472 2023-07-26 17:36:16.000000 AppiumExtended-0.0.1/AppiumExtended.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1310 2023-07-26 17:36:16.000000 AppiumExtended-0.0.1/AppiumExtended.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:36:16.000000 AppiumExtended-0.0.1/AppiumExtended.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      232 2023-07-26 17:36:16.000000 AppiumExtended-0.0.1/AppiumExtended.egg-info/requires.txt
--rw-rw-rw-   0        0        0      131 2023-07-26 17:36:16.000000 AppiumExtended-0.0.1/AppiumExtended.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.340661 AppiumExtended-0.0.1/AppiumGraph/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:49.000000 AppiumExtended-0.0.1/AppiumGraph/__init__.py
--rw-rw-rw-   0        0        0      486 2023-07-26 16:29:27.000000 AppiumExtended-0.0.1/AppiumGraph/appium_graph.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.347658 AppiumExtended-0.0.1/AppiumHelpers/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:54.000000 AppiumExtended-0.0.1/AppiumHelpers/__init__.py
--rw-rw-rw-   0        0        0    18033 2023-07-26 16:33:16.000000 AppiumExtended-0.0.1/AppiumHelpers/appium_helpers.py
--rw-rw-rw-   0        0        0    32167 2023-07-26 16:36:11.000000 AppiumExtended-0.0.1/AppiumHelpers/appium_image.py
--rw-rw-rw-   0        0        0    19842 2023-07-26 17:18:17.000000 AppiumExtended-0.0.1/AppiumHelpers/helpers_decorators.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.351660 AppiumExtended-0.0.1/AppiumNavigator/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:58.000000 AppiumExtended-0.0.1/AppiumNavigator/__init__.py
--rw-rw-rw-   0        0        0     7435 2023-07-26 16:41:36.000000 AppiumExtended-0.0.1/AppiumNavigator/appium_navigator.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.354657 AppiumExtended-0.0.1/AppiumServer/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:03.000000 AppiumExtended-0.0.1/AppiumServer/__init__.py
--rw-rw-rw-   0        0        0     2145 2023-07-26 16:53:52.000000 AppiumExtended-0.0.1/AppiumServer/appium_server.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.370800 AppiumExtended-0.0.1/AppiumWebElementExtended/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:07.000000 AppiumExtended-0.0.1/AppiumWebElementExtended/__init__.py
--rw-rw-rw-   0        0        0        6 2023-05-31 18:50:55.000000 AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_actions.py
--rw-rw-rw-   0        0        0     9210 2023-07-26 16:51:39.000000 AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_adb_actions.py
--rw-rw-rw-   0        0        0    11345 2023-07-26 16:53:53.000000 AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_click.py
--rw-rw-rw-   0        0        0    14511 2023-07-26 16:56:52.000000 AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_dom.py
--rw-rw-rw-   0        0        0    17174 2023-07-26 16:56:57.000000 AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_extended.py
--rw-rw-rw-   0        0        0    23257 2023-07-26 16:58:06.000000 AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_get.py
--rw-rw-rw-   0        0        0    11658 2023-07-26 16:59:35.000000 AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_scroll.py
--rw-rw-rw-   0        0        0    12723 2023-07-26 16:59:35.000000 AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_tap.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.373797 AppiumExtended-0.0.1/AppiumWebElementsExtended/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:11.000000 AppiumExtended-0.0.1/AppiumWebElementsExtended/__init__.py
--rw-rw-rw-   0        0        0      493 2023-07-26 16:59:35.000000 AppiumExtended-0.0.1/AppiumWebElementsExtended/web_elements_extended.py
--rw-rw-rw-   0        0        0      472 2023-07-26 17:36:16.384794 AppiumExtended-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.376796 AppiumExtended-0.0.1/adb/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:15:39.000000 AppiumExtended-0.0.1/adb/__init__.py
--rw-rw-rw-   0        0        0    27262 2023-07-26 16:49:36.000000 AppiumExtended-0.0.1/adb/adb.py
--rw-rw-rw-   0        0        0       42 2023-07-26 17:36:16.384794 AppiumExtended-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      997 2023-07-26 17:33:25.000000 AppiumExtended-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:36:16.381801 AppiumExtended-0.0.1/utils/
--rw-rw-rw-   0        0        0        0 2023-07-26 17:16:21.000000 AppiumExtended-0.0.1/utils/__init__.py
--rw-rw-rw-   0        0        0    16209 2023-07-26 16:53:52.000000 AppiumExtended-0.0.1/utils/operations.py
--rw-rw-rw-   0        0        0     6955 2023-07-26 17:07:41.000000 AppiumExtended-0.0.1/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.978569 AppiumExtended-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.927042 AppiumExtended-0.0.2/AppiumExtended/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:15:45.000000 AppiumExtended-0.0.2/AppiumExtended/__init__.py
+-rw-rw-rw-   0        0        0     2694 2023-07-26 16:13:14.000000 AppiumExtended-0.0.2/AppiumExtended/appium_base.py
+-rw-rw-rw-   0        0        0    28523 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_extended.py
+-rw-rw-rw-   0        0        0    15339 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_get.py
+-rw-rw-rw-   0        0        0     2505 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_is.py
+-rw-rw-rw-   0        0        0     2259 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_swipe.py
+-rw-rw-rw-   0        0        0     1888 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_tap.py
+-rw-rw-rw-   0        0        0     7107 2023-07-26 16:28:56.000000 AppiumExtended-0.0.2/AppiumExtended/appium_wait.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.935042 AppiumExtended-0.0.2/AppiumExtended.egg-info/
+-rw-rw-rw-   0        0        0      472 2023-07-26 17:49:58.000000 AppiumExtended-0.0.2/AppiumExtended.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1310 2023-07-26 17:49:58.000000 AppiumExtended-0.0.2/AppiumExtended.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:49:58.000000 AppiumExtended-0.0.2/AppiumExtended.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      232 2023-07-26 17:49:58.000000 AppiumExtended-0.0.2/AppiumExtended.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      131 2023-07-26 17:49:58.000000 AppiumExtended-0.0.2/AppiumExtended.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.939486 AppiumExtended-0.0.2/AppiumGraph/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:15:49.000000 AppiumExtended-0.0.2/AppiumGraph/__init__.py
+-rw-rw-rw-   0        0        0      486 2023-07-26 16:29:27.000000 AppiumExtended-0.0.2/AppiumGraph/appium_graph.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.944879 AppiumExtended-0.0.2/AppiumHelpers/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:15:54.000000 AppiumExtended-0.0.2/AppiumHelpers/__init__.py
+-rw-rw-rw-   0        0        0    18033 2023-07-26 16:33:16.000000 AppiumExtended-0.0.2/AppiumHelpers/appium_helpers.py
+-rw-rw-rw-   0        0        0    32167 2023-07-26 16:36:11.000000 AppiumExtended-0.0.2/AppiumHelpers/appium_image.py
+-rw-rw-rw-   0        0        0    19788 2023-07-26 17:49:07.000000 AppiumExtended-0.0.2/AppiumHelpers/helpers_decorators.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.949016 AppiumExtended-0.0.2/AppiumNavigator/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:15:58.000000 AppiumExtended-0.0.2/AppiumNavigator/__init__.py
+-rw-rw-rw-   0        0        0     7435 2023-07-26 16:41:36.000000 AppiumExtended-0.0.2/AppiumNavigator/appium_navigator.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.952009 AppiumExtended-0.0.2/AppiumServer/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:16:03.000000 AppiumExtended-0.0.2/AppiumServer/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-07-26 16:53:52.000000 AppiumExtended-0.0.2/AppiumServer/appium_server.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.966894 AppiumExtended-0.0.2/AppiumWebElementExtended/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:16:07.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/__init__.py
+-rw-rw-rw-   0        0        0        6 2023-05-31 18:50:55.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_actions.py
+-rw-rw-rw-   0        0        0     9210 2023-07-26 16:51:39.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_adb_actions.py
+-rw-rw-rw-   0        0        0    11345 2023-07-26 16:53:53.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_click.py
+-rw-rw-rw-   0        0        0    14511 2023-07-26 16:56:52.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_dom.py
+-rw-rw-rw-   0        0        0    17174 2023-07-26 16:56:57.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_extended.py
+-rw-rw-rw-   0        0        0    23257 2023-07-26 16:58:06.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_get.py
+-rw-rw-rw-   0        0        0    11658 2023-07-26 16:59:35.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_scroll.py
+-rw-rw-rw-   0        0        0    12723 2023-07-26 16:59:35.000000 AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_tap.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.969468 AppiumExtended-0.0.2/AppiumWebElementsExtended/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:16:11.000000 AppiumExtended-0.0.2/AppiumWebElementsExtended/__init__.py
+-rw-rw-rw-   0        0        0      493 2023-07-26 16:59:35.000000 AppiumExtended-0.0.2/AppiumWebElementsExtended/web_elements_extended.py
+-rw-rw-rw-   0        0        0      472 2023-07-26 17:49:58.978569 AppiumExtended-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.972473 AppiumExtended-0.0.2/adb/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:15:39.000000 AppiumExtended-0.0.2/adb/__init__.py
+-rw-rw-rw-   0        0        0    27262 2023-07-26 16:49:36.000000 AppiumExtended-0.0.2/adb/adb.py
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:49:58.978569 AppiumExtended-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      997 2023-07-26 17:49:48.000000 AppiumExtended-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:49:58.976564 AppiumExtended-0.0.2/utils/
+-rw-rw-rw-   0        0        0        0 2023-07-26 17:16:21.000000 AppiumExtended-0.0.2/utils/__init__.py
+-rw-rw-rw-   0        0        0    16209 2023-07-26 16:53:52.000000 AppiumExtended-0.0.2/utils/operations.py
+-rw-rw-rw-   0        0        0     6955 2023-07-26 17:07:41.000000 AppiumExtended-0.0.2/utils/utils.py
```

### Comparing `AppiumExtended-0.0.1/AppiumExtended/appium_base.py` & `AppiumExtended-0.0.2/AppiumExtended/appium_base.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumExtended/appium_extended.py` & `AppiumExtended-0.0.2/AppiumExtended/appium_extended.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumExtended/appium_get.py` & `AppiumExtended-0.0.2/AppiumExtended/appium_get.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumExtended/appium_is.py` & `AppiumExtended-0.0.2/AppiumExtended/appium_is.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumExtended/appium_swipe.py` & `AppiumExtended-0.0.2/AppiumExtended/appium_swipe.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumExtended/appium_tap.py` & `AppiumExtended-0.0.2/AppiumExtended/appium_tap.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumExtended/appium_wait.py` & `AppiumExtended-0.0.2/AppiumExtended/appium_wait.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumExtended.egg-info/SOURCES.txt` & `AppiumExtended-0.0.2/AppiumExtended.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumHelpers/appium_helpers.py` & `AppiumExtended-0.0.2/AppiumHelpers/appium_helpers.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumHelpers/appium_image.py` & `AppiumExtended-0.0.2/AppiumHelpers/appium_image.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumHelpers/helpers_decorators.py` & `AppiumExtended-0.0.2/AppiumHelpers/helpers_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 from functools import wraps
 from datetime import datetime
 
 import allure
 import numpy as np
 from PIL import Image
 
-from AppiumHelpers.appium_image import AppiumImage
-
 import config
 
 logger = logging.getLogger(config.APPIUM_LOG_NAME)
 
 
 def retry(func):
     max_retries = 3
```

### Comparing `AppiumExtended-0.0.1/AppiumNavigator/appium_navigator.py` & `AppiumExtended-0.0.2/AppiumNavigator/appium_navigator.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumServer/appium_server.py` & `AppiumExtended-0.0.2/AppiumServer/appium_server.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_adb_actions.py` & `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_adb_actions.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_click.py` & `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_click.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_dom.py` & `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_dom.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_extended.py` & `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_extended.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_get.py` & `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_get.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_scroll.py` & `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_scroll.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/AppiumWebElementExtended/web_element_tap.py` & `AppiumExtended-0.0.2/AppiumWebElementExtended/web_element_tap.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/adb/adb.py` & `AppiumExtended-0.0.2/adb/adb.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/setup.py` & `AppiumExtended-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='AppiumExtended',
-    version='0.0.1',
+    version='0.0.2',
     description='An extension library for adding ease of use Appium-Python-Client',
     author='open source community',
     packages=find_packages(),
     install_requires=[
         'Appium-Python-Client==2.11.1',
         'allure-pytest==2.13.2',
         'zlib-compress==0.0.1',
```

### Comparing `AppiumExtended-0.0.1/utils/operations.py` & `AppiumExtended-0.0.2/utils/operations.py`

 * *Files identical despite different names*

### Comparing `AppiumExtended-0.0.1/utils/utils.py` & `AppiumExtended-0.0.2/utils/utils.py`

 * *Files identical despite different names*

