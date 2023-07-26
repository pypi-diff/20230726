# Comparing `tmp/adafri-0.0.64.tar.gz` & `tmp/adafri-0.0.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.64.tar", last modified: Wed Jul 26 07:29:24 2023, max compression
+gzip compressed data, was "adafri-0.0.65.tar", last modified: Wed Jul 26 07:42:44 2023, max compression
```

## Comparing `adafri-0.0.64.tar` & `adafri-0.0.65.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.238583 adafri-0.0.64/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-26 07:29:24.238098 adafri-0.0.64/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.193627 adafri-0.0.64/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-26 07:29:16.000000 adafri-0.0.64/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.201136 adafri-0.0.64/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.64/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.64/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.64/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.64/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    17783 2023-07-26 06:40:14.000000 adafri-0.0.64/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.202484 adafri-0.0.64/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.64/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.203662 adafri-0.0.64/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.64/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.210339 adafri-0.0.64/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.64/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.64/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.64/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.211271 adafri-0.0.64/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.64/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.213223 adafri-0.0.64/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.64/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.64/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.214374 adafri-0.0.64/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.64/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.214908 adafri-0.0.64/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.64/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.223152 adafri-0.0.64/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.64/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6848 2023-07-26 05:25:24.000000 adafri-0.0.64/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.64/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16141 2023-07-26 05:25:12.000000 adafri-0.0.64/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.64/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9462 2023-07-26 05:24:58.000000 adafri-0.0.64/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.64/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.226334 adafri-0.0.64/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.64/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.64/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.64/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.228899 adafri-0.0.64/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.64/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.64/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.229405 adafri-0.0.64/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)     7392 2023-07-26 04:34:01.000000 adafri-0.0.64/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.230144 adafri-0.0.64/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.64/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.237018 adafri-0.0.64/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.64/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11611 2023-07-26 06:16:52.000000 adafri-0.0.64/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7314 2023-07-26 07:29:12.000000 adafri-0.0.64/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:29:24.195864 adafri-0.0.64/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-26 07:29:24.000000 adafri-0.0.64/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1250 2023-07-26 07:29:24.000000 adafri-0.0.64/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-26 07:29:24.000000 adafri-0.0.64/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-26 07:29:24.000000 adafri-0.0.64/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-26 07:29:24.239240 adafri-0.0.64/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.64/setup.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.879123 adafri-0.0.65/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-26 07:42:44.878650 adafri-0.0.65/PKG-INFO
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.829939 adafri-0.0.65/adafri/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-07-26 07:42:39.000000 adafri-0.0.65/adafri/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.838055 adafri-0.0.65/adafri/utils/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.65/adafri/utils/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.65/adafri/utils/country.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.65/adafri/utils/phone_number.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1268 2023-07-11 19:28:16.000000 adafri-0.0.65/adafri/utils/response.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    17783 2023-07-26 06:40:14.000000 adafri-0.0.65/adafri/utils/utils.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.839376 adafri-0.0.65/adafri/v1/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.65/adafri/v1/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.840172 adafri-0.0.65/adafri/v1/account/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.65/adafri/v1/account/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.842691 adafri-0.0.65/adafri/v1/account/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.65/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.65/adafri/v1/account/models/account.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3816 2023-07-12 22:09:50.000000 adafri-0.0.65/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.843610 adafri-0.0.65/adafri/v1/auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.65/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.845048 adafri-0.0.65/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.65/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.65/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.846090 adafri-0.0.65/adafri/v1/auth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.65/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.846785 adafri-0.0.65/adafri/v1/auth/oauth/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      814 2023-07-18 00:36:46.000000 adafri-0.0.65/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.858785 adafri-0.0.65/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.65/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     6848 2023-07-26 05:25:24.000000 adafri-0.0.65/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4857 2023-07-13 16:12:18.000000 adafri-0.0.65/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    16141 2023-07-26 05:25:12.000000 adafri-0.0.65/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3635 2023-07-19 20:20:48.000000 adafri-0.0.65/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     9462 2023-07-26 05:24:58.000000 adafri-0.0.65/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     3710 2023-07-21 03:04:50.000000 adafri-0.0.65/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.862036 adafri-0.0.65/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.65/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.65/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.65/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.864542 adafri-0.0.65/adafri/v1/base/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.65/adafri/v1/base/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.65/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.865804 adafri-0.0.65/adafri/v1/mailing/
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7392 2023-07-26 04:34:01.000000 adafri-0.0.65/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.873628 adafri-0.0.65/adafri/v1/user/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.65/adafri/v1/user/__init__.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.877647 adafri-0.0.65/adafri/v1/user/models/
+-rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.65/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)    11624 2023-07-26 07:42:34.000000 adafri-0.0.65/adafri/v1/user/models/user.py
+-rw-r--r--   0 ibrahima   (502) staff       (20)     7346 2023-07-26 07:42:30.000000 adafri-0.0.65/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-07-26 07:42:44.833373 adafri-0.0.65/adafri.egg-info/
+-rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-07-26 07:42:44.000000 adafri-0.0.65/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 ibrahima   (502) staff       (20)     1250 2023-07-26 07:42:44.000000 adafri-0.0.65/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-07-26 07:42:44.000000 adafri-0.0.65/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-07-26 07:42:44.000000 adafri-0.0.65/adafri.egg-info/top_level.txt
+-rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-07-26 07:42:44.879561 adafri-0.0.65/setup.cfg
+-rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.65/setup.py
```

### Comparing `adafri-0.0.64/adafri/utils/country.py` & `adafri-0.0.65/adafri/utils/country.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/utils/phone_number.py` & `adafri-0.0.65/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/utils/response.py` & `adafri-0.0.65/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/utils/utils.py` & `adafri-0.0.65/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/account/models/account.py` & `adafri-0.0.65/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/account/models/account_fields.py` & `adafri-0.0.65/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.65/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.65/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.65/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.65/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.65/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.65/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.65/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.65/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.65/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.65/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/base/firebase_collection.py` & `adafri-0.0.65/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/mailing/__init__.py` & `adafri-0.0.65/adafri/v1/mailing/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/adafri/v1/user/models/user.py` & `adafri-0.0.65/adafri/v1/user/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,16 @@
     password: str
     provider: str
     status: str
     _emailValidationSendDate: str
     businessType: str
     phoneVerified: bool
     emailVerified: bool
-       
+    postalCode: str
+
     def __init__(self, user=None, **kwargs):
         if type(user) is str:
             user = {"uid": user} 
         (cls_object, keys, data_args) = init_class_kwargs(self, user, STANDARD_FIELDS, UserFieldProps, USERS_COLLECTION, ['id','uid'], **kwargs)
         super().__init__(**data_args);
         for key in keys:
             setattr(self, key, cls_object[key]);
```

### Comparing `adafri-0.0.64/adafri/v1/user/models/user_fields.py` & `adafri-0.0.65/adafri/v1/user/models/user_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     entrepriseName = 'entrepriseName';
     entrepriseUrl = 'entrepriseUrl';
     isConnectWithMailAndPassword = 'isConnectWithMailAndPassword';
     address = 'addresse';
     photoURL = 'photoURL';
     profileCompleted = 'profileCompleted';
     telephone = 'telephone';
-    postalCode = 'postal';
+    postalCode = 'postalCode';
     token = 'token';
     deviceInfo = 'deviceInfo';
     phoneInfo = 'phoneInfo';
     country = 'country';
     showPushToken = 'showPushToken'
     authorizedPush = 'authorizedPush';
     hasApprouvedPolicy = 'hasApprouvedPolicy';
@@ -260,21 +260,21 @@
     "mutable": True,
     "editable": True,
     "interactive": False,
     "default_value": "",
     "pickable": True,
     },
      UserFields.postal:{
-    "type": str,
-    "required": False,
-    "mutable": True,
-    "editable": True,
-    "interactive": False,
-    "default_value": "",
-    "pickable": True,
+        "type": str,
+        "required": False,
+        "mutable": True,
+        "editable": True,
+        "interactive": False,
+        "default_value": "",
+        "pickable": True,
     },
     UserFields.phoneVerified:{
         "type": bool,
         "required": False,
         "mutable": True,
         "editable": True,
         "interactive": False,
```

### Comparing `adafri-0.0.64/adafri.egg-info/SOURCES.txt` & `adafri-0.0.65/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.64/setup.py` & `adafri-0.0.65/setup.py`

 * *Files identical despite different names*

