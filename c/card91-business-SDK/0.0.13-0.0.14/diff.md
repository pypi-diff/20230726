# Comparing `tmp/Card91-Business-SDK-0.0.13.tar.gz` & `tmp/card91_business_SDK-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Card91-Business-SDK-0.0.13.tar", last modified: Wed Jul 26 06:07:48 2023, max compression
+gzip compressed data, was "card91_business_SDK-0.0.14.tar", last modified: Wed Jul 26 06:15:19 2023, max compression
```

## Comparing `Card91-Business-SDK-0.0.13.tar` & `card91_business_SDK-0.0.14.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 06:07:48.264162 Card91-Business-SDK-0.0.13/
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 06:07:48.264162 Card91-Business-SDK-0.0.13/Card91_Business_SDK.egg-info/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      415 2023-07-26 06:07:48.000000 Card91-Business-SDK-0.0.13/Card91_Business_SDK.egg-info/PKG-INFO
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      295 2023-07-26 06:07:48.000000 Card91-Business-SDK-0.0.13/Card91_Business_SDK.egg-info/SOURCES.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-26 06:07:48.000000 Card91-Business-SDK-0.0.13/Card91_Business_SDK.egg-info/dependency_links.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        9 2023-07-26 06:07:48.000000 Card91-Business-SDK-0.0.13/Card91_Business_SDK.egg-info/requires.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       20 2023-07-26 06:07:48.000000 Card91-Business-SDK-0.0.13/Card91_Business_SDK.egg-info/top_level.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      415 2023-07-26 06:07:48.264162 Card91-Business-SDK-0.0.13/PKG-INFO
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 06:07:48.264162 Card91-Business-SDK-0.0.13/card91_business_sdk/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       83 2023-07-26 05:47:15.000000 Card91-Business-SDK-0.0.13/card91_business_sdk/__init__.py
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)     8063 2023-07-25 12:14:18.000000 Card91-Business-SDK-0.0.13/card91_business_sdk/card91BusinessSDK.py
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-26 06:07:48.264162 Card91-Business-SDK-0.0.13/setup.cfg
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      576 2023-07-26 05:47:29.000000 Card91-Business-SDK-0.0.13/setup.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 06:15:19.667582 card91_business_SDK-0.0.14/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      415 2023-07-26 06:15:19.663582 card91_business_SDK-0.0.14/PKG-INFO
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 06:15:19.663582 card91_business_SDK-0.0.14/card91_business_SDK.egg-info/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      415 2023-07-26 06:15:19.000000 card91_business_SDK-0.0.14/card91_business_SDK.egg-info/PKG-INFO
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      295 2023-07-26 06:15:19.000000 card91_business_SDK-0.0.14/card91_business_SDK.egg-info/SOURCES.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-26 06:15:19.000000 card91_business_SDK-0.0.14/card91_business_SDK.egg-info/dependency_links.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        9 2023-07-26 06:15:19.000000 card91_business_SDK-0.0.14/card91_business_SDK.egg-info/requires.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       20 2023-07-26 06:15:19.000000 card91_business_SDK-0.0.14/card91_business_SDK.egg-info/top_level.txt
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 06:15:19.663582 card91_business_SDK-0.0.14/card91_business_sdk/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       83 2023-07-26 05:47:15.000000 card91_business_SDK-0.0.14/card91_business_sdk/__init__.py
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)     8063 2023-07-25 12:14:18.000000 card91_business_SDK-0.0.14/card91_business_sdk/card91BusinessSDK.py
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-26 06:15:19.667582 card91_business_SDK-0.0.14/setup.cfg
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      576 2023-07-26 06:15:14.000000 card91_business_SDK-0.0.14/setup.py
```

### Comparing `Card91-Business-SDK-0.0.13/card91_business_sdk/card91BusinessSDK.py` & `card91_business_SDK-0.0.14/card91_business_sdk/card91BusinessSDK.py`

 * *Files identical despite different names*

### Comparing `Card91-Business-SDK-0.0.13/setup.py` & `card91_business_SDK-0.0.14/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="Card91-Business-SDK",
-    version="0.0.13",
+    name="card91_business_SDK",
+    version="0.0.14",
     description="This package is used to access the bunch of Card91 fintech business services",
     url="https://github.com/nk2909/Python-SDK.git",
     author="Card91",
     author_email="tech.apps@card91.io",
     install_requires=["requests"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

