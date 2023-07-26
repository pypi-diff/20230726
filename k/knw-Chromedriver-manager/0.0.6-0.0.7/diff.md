# Comparing `tmp/knw_Chromedriver_manager-0.0.6.tar.gz` & `tmp/knw_Chromedriver_manager-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knw_Chromedriver_manager-0.0.6.tar", last modified: Wed Jul 26 17:03:38 2023, max compression
+gzip compressed data, was "knw_Chromedriver_manager-0.0.7.tar", last modified: Wed Jul 26 17:10:00 2023, max compression
```

## Comparing `knw_Chromedriver_manager-0.0.6.tar` & `knw_Chromedriver_manager-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:03:38.471352 knw_Chromedriver_manager-0.0.6/
--rw-rw-rw-   0        0        0      914 2023-07-26 17:03:38.470353 knw_Chromedriver_manager-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-07-26 16:26:44.000000 knw_Chromedriver_manager-0.0.6/README
-drwxrwxrwx   0        0        0        0 2023-07-26 17:03:38.462350 knw_Chromedriver_manager-0.0.6/knw_Chromedriver_manager/
--rw-rw-rw-   0        0        0     5040 2023-07-26 16:33:29.000000 knw_Chromedriver_manager-0.0.6/knw_Chromedriver_manager/Chromedriver_manager.py
--rw-rw-rw-   0        0        0        0 2023-07-26 15:28:35.000000 knw_Chromedriver_manager-0.0.6/knw_Chromedriver_manager/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:03:38.470353 knw_Chromedriver_manager-0.0.6/knw_Chromedriver_manager.egg-info/
--rw-rw-rw-   0        0        0      914 2023-07-26 17:03:38.000000 knw_Chromedriver_manager-0.0.6/knw_Chromedriver_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-07-26 17:03:38.000000 knw_Chromedriver_manager-0.0.6/knw_Chromedriver_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:03:38.000000 knw_Chromedriver_manager-0.0.6/knw_Chromedriver_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-26 17:03:38.000000 knw_Chromedriver_manager-0.0.6/knw_Chromedriver_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 17:03:38.471352 knw_Chromedriver_manager-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-07-26 17:03:22.000000 knw_Chromedriver_manager-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:10:00.784429 knw_Chromedriver_manager-0.0.7/
+-rw-rw-rw-   0        0        0     1186 2023-07-26 17:10:00.784429 knw_Chromedriver_manager-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      741 2023-07-26 17:09:28.000000 knw_Chromedriver_manager-0.0.7/README
+drwxrwxrwx   0        0        0        0 2023-07-26 17:10:00.775428 knw_Chromedriver_manager-0.0.7/knw_Chromedriver_manager/
+-rw-rw-rw-   0        0        0     5040 2023-07-26 16:33:29.000000 knw_Chromedriver_manager-0.0.7/knw_Chromedriver_manager/Chromedriver_manager.py
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:28:35.000000 knw_Chromedriver_manager-0.0.7/knw_Chromedriver_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:10:00.783429 knw_Chromedriver_manager-0.0.7/knw_Chromedriver_manager.egg-info/
+-rw-rw-rw-   0        0        0     1186 2023-07-26 17:10:00.000000 knw_Chromedriver_manager-0.0.7/knw_Chromedriver_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-07-26 17:10:00.000000 knw_Chromedriver_manager-0.0.7/knw_Chromedriver_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:10:00.000000 knw_Chromedriver_manager-0.0.7/knw_Chromedriver_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-26 17:10:00.000000 knw_Chromedriver_manager-0.0.7/knw_Chromedriver_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:10:00.784429 knw_Chromedriver_manager-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-07-26 17:05:26.000000 knw_Chromedriver_manager-0.0.7/setup.py
```

### Comparing `knw_Chromedriver_manager-0.0.6/PKG-INFO` & `knw_Chromedriver_manager-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: knw_Chromedriver_manager
-Version: 0.0.6
+Version: 0.0.7
 Summary: Chromedriver_manager for knw
 Home-page: https://github.com/daumsong/knw_webdriver_manager
 Author: OH nam kyun
 Author-email: daumsong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Chromedriver_manager for knw / By archon.oh
 
+
+#####################################
 [install]
-pip install knw_Chromedriver_manager
 
+pip install knw-Chromedriver-manager
+#####################################
 
+#############################################################################################
 [sample code]
+
 from knw_Chromedriver_manager import Chromedriver_manager
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 options = Options()
 driver = webdriver.Chrome(service=Service(Chromedriver_manager.install()), options=options)
 driver.get("https://www.daum.net/")
+#############################################################################################
```

### Comparing `knw_Chromedriver_manager-0.0.6/knw_Chromedriver_manager/Chromedriver_manager.py` & `knw_Chromedriver_manager-0.0.7/knw_Chromedriver_manager/Chromedriver_manager.py`

 * *Files identical despite different names*

### Comparing `knw_Chromedriver_manager-0.0.6/knw_Chromedriver_manager.egg-info/PKG-INFO` & `knw_Chromedriver_manager-0.0.7/knw_Chromedriver_manager.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 Metadata-Version: 2.1
 Name: knw-Chromedriver-manager
-Version: 0.0.6
+Version: 0.0.7
 Summary: Chromedriver_manager for knw
 Home-page: https://github.com/daumsong/knw_webdriver_manager
 Author: OH nam kyun
 Author-email: daumsong@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Chromedriver_manager for knw / By archon.oh
 
+
+#####################################
 [install]
-pip install knw_Chromedriver_manager
 
+pip install knw-Chromedriver-manager
+#####################################
 
+#############################################################################################
 [sample code]
+
 from knw_Chromedriver_manager import Chromedriver_manager
 
 from selenium import webdriver
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.chrome.service import Service
 
 options = Options()
 driver = webdriver.Chrome(service=Service(Chromedriver_manager.install()), options=options)
 driver.get("https://www.daum.net/")
+#############################################################################################
```

### Comparing `knw_Chromedriver_manager-0.0.6/setup.py` & `knw_Chromedriver_manager-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="knw_Chromedriver_manager",
-    version="0.0.6",
+    version="0.0.7",
     author="OH nam kyun",
     author_email="daumsong@gmail.com",
     description="Chromedriver_manager for knw",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/daumsong/knw_webdriver_manager",
     packages=setuptools.find_packages(),
```

