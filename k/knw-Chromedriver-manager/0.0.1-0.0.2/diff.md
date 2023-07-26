# Comparing `tmp/knw_Chromedriver_manager-0.0.1.tar.gz` & `tmp/knw_Chromedriver_manager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knw_Chromedriver_manager-0.0.1.tar", last modified: Wed Jul 26 16:04:17 2023, max compression
+gzip compressed data, was "knw_Chromedriver_manager-0.0.2.tar", last modified: Wed Jul 26 16:18:42 2023, max compression
```

## Comparing `knw_Chromedriver_manager-0.0.1.tar` & `knw_Chromedriver_manager-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:04:17.010628 knw_Chromedriver_manager-0.0.1/
--rw-rw-rw-   0        0        0      473 2023-07-26 16:04:17.010628 knw_Chromedriver_manager-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-07-26 15:37:35.000000 knw_Chromedriver_manager-0.0.1/README
-drwxrwxrwx   0        0        0        0 2023-07-26 16:04:16.999471 knw_Chromedriver_manager-0.0.1/knw_Chromedriver_manager/
--rw-rw-rw-   0        0        0        0 2023-07-26 15:28:35.000000 knw_Chromedriver_manager-0.0.1/knw_Chromedriver_manager/__init__.py
--rw-rw-rw-   0        0        0     5827 2023-07-26 15:20:53.000000 knw_Chromedriver_manager-0.0.1/knw_Chromedriver_manager/knw_Chromedriver_manager.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:04:17.009477 knw_Chromedriver_manager-0.0.1/knw_Chromedriver_manager.egg-info/
--rw-rw-rw-   0        0        0      473 2023-07-26 16:04:16.000000 knw_Chromedriver_manager-0.0.1/knw_Chromedriver_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-07-26 16:04:16.000000 knw_Chromedriver_manager-0.0.1/knw_Chromedriver_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:04:16.000000 knw_Chromedriver_manager-0.0.1/knw_Chromedriver_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-26 16:04:16.000000 knw_Chromedriver_manager-0.0.1/knw_Chromedriver_manager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 16:04:17.011630 knw_Chromedriver_manager-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      727 2023-07-26 16:01:13.000000 knw_Chromedriver_manager-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:18:42.412470 knw_Chromedriver_manager-0.0.2/
+-rw-rw-rw-   0        0        0      488 2023-07-26 16:18:42.411470 knw_Chromedriver_manager-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-07-26 16:17:05.000000 knw_Chromedriver_manager-0.0.2/README
+drwxrwxrwx   0        0        0        0 2023-07-26 16:18:42.401467 knw_Chromedriver_manager-0.0.2/knw_Chromedriver_manager/
+-rw-rw-rw-   0        0        0     5827 2023-07-26 15:20:53.000000 knw_Chromedriver_manager-0.0.2/knw_Chromedriver_manager/Chromedriver_manager.py
+-rw-rw-rw-   0        0        0        0 2023-07-26 15:28:35.000000 knw_Chromedriver_manager-0.0.2/knw_Chromedriver_manager/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:18:42.411470 knw_Chromedriver_manager-0.0.2/knw_Chromedriver_manager.egg-info/
+-rw-rw-rw-   0        0        0      488 2023-07-26 16:18:42.000000 knw_Chromedriver_manager-0.0.2/knw_Chromedriver_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-07-26 16:18:42.000000 knw_Chromedriver_manager-0.0.2/knw_Chromedriver_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 16:18:42.000000 knw_Chromedriver_manager-0.0.2/knw_Chromedriver_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-26 16:18:42.000000 knw_Chromedriver_manager-0.0.2/knw_Chromedriver_manager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 16:18:42.412470 knw_Chromedriver_manager-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      727 2023-07-26 16:18:08.000000 knw_Chromedriver_manager-0.0.2/setup.py
```

### Comparing `knw_Chromedriver_manager-0.0.1/knw_Chromedriver_manager/knw_Chromedriver_manager.py` & `knw_Chromedriver_manager-0.0.2/knw_Chromedriver_manager/Chromedriver_manager.py`

 * *Files identical despite different names*

### Comparing `knw_Chromedriver_manager-0.0.1/setup.py` & `knw_Chromedriver_manager-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="knw_Chromedriver_manager", # Replace with your own PyPI username(id)
-    version="0.0.1",
+    version="0.0.2",
     author="OH nam kyun",
     author_email="daumsong@gmail.com",
     description="Chromedriver_manager for knw",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/daumsong/knw_webdriver_manager",
     packages=setuptools.find_packages(),
```

