# Comparing `tmp/adafri-0.0.59.tar.gz` & `tmp/adafri-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.59.tar", last modified: Wed Jul 26 05:03:56 2023, max compression
+gzip compressed data, was "adafri-0.0.60.tar", last modified: Wed Jul 26 05:25:35 2023, max compression
```

## Comparing `adafri-0.0.59.tar` & `adafri-0.0.60.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.351039 adafri-0.0.59/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-26 05:03:56.350719 adafri-0.0.59/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.311945 adafri-0.0.59/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-26 05:03:51.000000 adafri-0.0.59/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.319978 adafri-0.0.59/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.59/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.59/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.59/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.59/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    17636 2023-07-25 19:33:39.000000 adafri-0.0.59/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.321223 adafri-0.0.59/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.59/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.322286 adafri-0.0.59/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.59/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.324797 adafri-0.0.59/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.59/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.59/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.59/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.325632 adafri-0.0.59/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.59/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.326812 adafri-0.0.59/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.59/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.59/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.328109 adafri-0.0.59/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.59/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.328550 adafri-0.0.59/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.59/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.334774 adafri-0.0.59/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.59/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6861 2023-07-26 05:03:44.000000 adafri-0.0.59/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.59/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16153 2023-07-26 05:03:20.000000 adafri-0.0.59/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.59/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9474 2023-07-26 05:03:08.000000 adafri-0.0.59/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.59/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.339228 adafri-0.0.59/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.59/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.59/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.59/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.345623 adafri-0.0.59/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.59/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.59/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.346403 adafri-0.0.59/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)     7392 2023-07-26 04:34:01.000000 adafri-0.0.59/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.347431 adafri-0.0.59/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.59/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.349851 adafri-0.0.59/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.59/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11571 2023-07-26 04:58:31.000000 adafri-0.0.59/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6139 2023-07-26 04:58:18.000000 adafri-0.0.59/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:03:56.314601 adafri-0.0.59/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-26 05:03:56.000000 adafri-0.0.59/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1250 2023-07-26 05:03:56.000000 adafri-0.0.59/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-26 05:03:56.000000 adafri-0.0.59/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-26 05:03:56.000000 adafri-0.0.59/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-26 05:03:56.351171 adafri-0.0.59/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.59/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.604285 adafri-0.0.60/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-26 05:25:35.603845 adafri-0.0.60/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.504637 adafri-0.0.60/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-26 05:25:29.000000 adafri-0.0.60/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.518368 adafri-0.0.60/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.60/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.60/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.60/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.60/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    17636 2023-07-25 19:33:39.000000 adafri-0.0.60/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.523006 adafri-0.0.60/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.60/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.523767 adafri-0.0.60/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.60/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.534663 adafri-0.0.60/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.60/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.60/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.60/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.535327 adafri-0.0.60/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.60/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.542415 adafri-0.0.60/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.60/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.60/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.547126 adafri-0.0.60/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.60/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.547572 adafri-0.0.60/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.60/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.582448 adafri-0.0.60/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.60/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6848 2023-07-26 05:25:24.000000 adafri-0.0.60/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.60/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16141 2023-07-26 05:25:12.000000 adafri-0.0.60/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.60/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9462 2023-07-26 05:24:58.000000 adafri-0.0.60/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.60/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.590659 adafri-0.0.60/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.60/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.60/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.60/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.594640 adafri-0.0.60/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.60/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.60/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.595775 adafri-0.0.60/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7392 2023-07-26 04:34:01.000000 adafri-0.0.60/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.597208 adafri-0.0.60/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.60/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.601996 adafri-0.0.60/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.60/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11560 2023-07-26 05:24:39.000000 adafri-0.0.60/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6139 2023-07-26 04:58:18.000000 adafri-0.0.60/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 05:25:35.509122 adafri-0.0.60/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-26 05:25:35.000000 adafri-0.0.60/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1250 2023-07-26 05:25:35.000000 adafri-0.0.60/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-26 05:25:35.000000 adafri-0.0.60/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-26 05:25:35.000000 adafri-0.0.60/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-26 05:25:35.604485 adafri-0.0.60/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.60/setup.py
```

### Comparing `adafri-0.0.59/adafri/utils/country.py` & `adafri-0.0.60/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/utils/phone_number.py` & `adafri-0.0.60/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/utils/response.py` & `adafri-0.0.60/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/utils/utils.py` & `adafri-0.0.60/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/account/models/account.py` & `adafri-0.0.60/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/account/models/account_fields.py` & `adafri-0.0.60/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.60/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.60/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.60/adafri/v1/auth/oauth/models/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     client_id_issued_at: int
     createdAt: any
     allowed_redirect_uris: list[str]
     default_redirect_uri: str
     
     def __init__(self, client=None, default_redirect_uri=None, **kwargs):
         if type(client) is str:
-            client = {[ClientFields.client_id]: client} 
+            client = {"client_id": client} 
         (cls_object, keys, data_args) = init_class_kwargs(self, client, STANDARD_FIELDS, ClientFieldProps, CLIENT_COLLECTION, ['id'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key])
         if bool(self.allowed_redirect_uris) is False:
             self.allowed_redirect_uris = self.redirect_uris
         #self.default_redirect_uri = default_redirect_uri
```

### Comparing `adafri-0.0.59/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.60/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.60/adafri/v1/auth/oauth/models/grant.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     expires: str
     code_challenge: str
     code_challenge_method: str
     auth_time: int
     
     def __init__(self, grant=None, **kwargs):
         if type(grant) is str:
-            grant = {[GrantFields.code]: grant} 
+            grant = {"code": grant} 
         (cls_object, keys, data_args) = init_class_kwargs(self, grant, STANDARD_FIELDS, GrantFieldsProps, GRANT_COLLECTION, ['id'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key]) 
         # kwargs['fields'] = STANDARD_FIELDS
         # kwargs['fields_props'] = GrantFieldsProps
         # collection_name = getattr(kwargs, 'collection_name', None)
```

### Comparing `adafri-0.0.59/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.60/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.60/adafri/v1/auth/oauth/models/token.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     expired_at: str
     expires_in: int
     revoked: bool
     type: str
 
     def __init__(self, token=None, **kwargs):
         if type(token) is str:
-            token = {[TokenFields.access_token]: token} 
+            token = {"access_token": token} 
         (cls_object, keys, data_args) = init_class_kwargs(self, token, STANDARD_FIELDS, TokenFieldsProps, TOKEN_COLLECTION, ['id'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key]) 
 
 
     @staticmethod
```

### Comparing `adafri-0.0.59/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.60/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.60/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.60/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/base/firebase_collection.py` & `adafri-0.0.60/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/mailing/__init__.py` & `adafri-0.0.60/adafri/v1/mailing/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri/v1/user/models/user.py` & `adafri-0.0.60/adafri/v1/user/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     provider: str
     status: str
     _emailValidationSendDate: str
     businessType: str
     
     def __init__(self, user=None, **kwargs):
         if type(user) is str:
-            user = {[UserFields.uid]: user} 
+            user = {"uid": user} 
         (cls_object, keys, data_args) = init_class_kwargs(self, user, STANDARD_FIELDS, UserFieldProps, USERS_COLLECTION, ['id','uid'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key]);
```

### Comparing `adafri-0.0.59/adafri/v1/user/models/user_fields.py` & `adafri-0.0.60/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/adafri.egg-info/SOURCES.txt` & `adafri-0.0.60/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.59/setup.py` & `adafri-0.0.60/setup.py`

 * *Files identical despite different names*

