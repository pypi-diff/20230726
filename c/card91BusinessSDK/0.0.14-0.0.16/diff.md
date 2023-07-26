# Comparing `tmp/card91BusinessSDK-0.0.14.tar.gz` & `tmp/card91BusinessSDK-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "card91BusinessSDK-0.0.14.tar", last modified: Wed Jul 26 06:24:59 2023, max compression
+gzip compressed data, was "card91BusinessSDK-0.0.16.tar", last modified: Wed Jul 26 10:23:16 2023, max compression
```

## Comparing `card91BusinessSDK-0.0.14.tar` & `card91BusinessSDK-0.0.16.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 06:24:59.146736 card91BusinessSDK-0.0.14/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      413 2023-07-26 06:24:59.146736 card91BusinessSDK-0.0.14/PKG-INFO
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 06:24:59.146736 card91BusinessSDK-0.0.14/card91BusinessSDK.egg-info/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      413 2023-07-26 06:24:59.000000 card91BusinessSDK-0.0.14/card91BusinessSDK.egg-info/PKG-INFO
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      285 2023-07-26 06:24:59.000000 card91BusinessSDK-0.0.14/card91BusinessSDK.egg-info/SOURCES.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-26 06:24:59.000000 card91BusinessSDK-0.0.14/card91BusinessSDK.egg-info/dependency_links.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        9 2023-07-26 06:24:59.000000 card91BusinessSDK-0.0.14/card91BusinessSDK.egg-info/requires.txt
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       20 2023-07-26 06:24:59.000000 card91BusinessSDK-0.0.14/card91BusinessSDK.egg-info/top_level.txt
-drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 06:24:59.146736 card91BusinessSDK-0.0.14/card91_business_sdk/
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       83 2023-07-26 05:47:15.000000 card91BusinessSDK-0.0.14/card91_business_sdk/__init__.py
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)     8063 2023-07-25 12:14:18.000000 card91BusinessSDK-0.0.14/card91_business_sdk/card91BusinessSDK.py
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-26 06:24:59.146736 card91BusinessSDK-0.0.14/setup.cfg
--rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      574 2023-07-26 06:24:32.000000 card91BusinessSDK-0.0.14/setup.py
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 10:23:16.472745 card91BusinessSDK-0.0.16/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      559 2023-07-26 10:23:16.472745 card91BusinessSDK-0.0.16/PKG-INFO
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      105 2023-07-26 10:22:13.000000 card91BusinessSDK-0.0.16/README.md
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 10:23:16.472745 card91BusinessSDK-0.0.16/card91BusinessSDK.egg-info/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      559 2023-07-26 10:23:16.000000 card91BusinessSDK-0.0.16/card91BusinessSDK.egg-info/PKG-INFO
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      295 2023-07-26 10:23:16.000000 card91BusinessSDK-0.0.16/card91BusinessSDK.egg-info/SOURCES.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        1 2023-07-26 10:23:16.000000 card91BusinessSDK-0.0.16/card91BusinessSDK.egg-info/dependency_links.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)        9 2023-07-26 10:23:16.000000 card91BusinessSDK-0.0.16/card91BusinessSDK.egg-info/requires.txt
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       20 2023-07-26 10:23:16.000000 card91BusinessSDK-0.0.16/card91BusinessSDK.egg-info/top_level.txt
+drwxrwxr-x   0 gautampandey  (1001) gautampandey  (1001)        0 2023-07-26 10:23:16.472745 card91BusinessSDK-0.0.16/card91_business_sdk/
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       83 2023-07-26 05:47:15.000000 card91BusinessSDK-0.0.16/card91_business_sdk/__init__.py
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)     8063 2023-07-25 12:14:18.000000 card91BusinessSDK-0.0.16/card91_business_sdk/card91BusinessSDK.py
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)       38 2023-07-26 10:23:16.472745 card91BusinessSDK-0.0.16/setup.cfg
+-rw-rw-r--   0 gautampandey  (1001) gautampandey  (1001)      749 2023-07-26 10:22:58.000000 card91BusinessSDK-0.0.16/setup.py
```

### Comparing `card91BusinessSDK-0.0.14/card91_business_sdk/card91BusinessSDK.py` & `card91BusinessSDK-0.0.16/card91_business_sdk/card91BusinessSDK.py`

 * *Files identical despite different names*

