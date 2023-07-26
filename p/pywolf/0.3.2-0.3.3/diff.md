# Comparing `tmp/pywolf-0.3.2.tar.gz` & `tmp/pywolf-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywolf-0.3.2.tar", max compression
+gzip compressed data, was "pywolf-0.3.3.tar", max compression
```

## Comparing `pywolf-0.3.2.tar` & `pywolf-0.3.3.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1066 2023-03-01 12:22:11.903833 pywolf-0.3.2/LICENSE
--rw-r--r--   0        0        0        1 2023-03-17 16:04:20.392530 pywolf-0.3.2/bin/__init__.py
--rw-r--r--   0        0        0      583 2023-04-03 07:45:27.331763 pywolf-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-21 03:39:26.790188 pywolf-0.3.2/pywolf/__init__.py
--rw-r--r--   0        0        0        1 2023-03-21 03:38:40.871188 pywolf-0.3.2/pywolf/application/__init__.py
--rw-r--r--   0        0        0      427 2023-03-28 07:55:03.811677 pywolf-0.3.2/pywolf/application/application.py
--rw-r--r--   0        0        0     1026 2023-04-03 07:25:02.947129 pywolf-0.3.2/pywolf/application/bootstrap.py
--rw-r--r--   0        0        0     1420 2023-03-25 06:20:55.232882 pywolf-0.3.2/pywolf/application/config.py
--rw-r--r--   0        0        0      870 2023-03-25 06:20:55.225783 pywolf-0.3.2/pywolf/application/context.py
--rw-r--r--   0        0        0        0 2023-03-19 13:01:39.384217 pywolf-0.3.2/pywolf/application/path.py
--rw-r--r--   0        0        0        1 2023-03-20 10:06:57.469480 pywolf-0.3.2/pywolf/cli/__init__.py
--rw-r--r--   0        0        0      456 2023-03-25 06:21:28.984391 pywolf-0.3.2/pywolf/cli/command.py
--rw-r--r--   0        0        0        1 2023-03-01 12:35:39.620639 pywolf-0.3.2/pywolf/db/__init__.py
--rw-r--r--   0        0        0      319 2023-03-31 13:14:34.382017 pywolf-0.3.2/pywolf/db/config.py
--rw-r--r--   0        0        0      977 2023-04-03 07:18:49.153629 pywolf-0.3.2/pywolf/db/db.py
--rw-r--r--   0        0        0      179 2023-03-31 13:17:43.750803 pywolf-0.3.2/pywolf/db/db_config_demo.yaml
--rw-r--r--   0        0        0     1444 2023-03-25 06:22:45.891789 pywolf-0.3.2/pywolf/db/executor.py
--rw-r--r--   0        0        0     1844 2023-03-25 06:22:45.887626 pywolf-0.3.2/pywolf/db/result.py
--rw-r--r--   0        0        0     1553 2023-03-27 15:18:30.957090 pywolf-0.3.2/pywolf/db/sqlutils.py
--rw-r--r--   0        0        0      111 2023-03-28 13:26:29.711044 pywolf-0.3.2/pywolf/exception/base.py
--rw-r--r--   0        0        0      120 2023-03-28 13:26:28.204059 pywolf-0.3.2/pywolf/exception/business.py
--rw-r--r--   0        0        0      117 2023-03-28 13:26:24.233477 pywolf-0.3.2/pywolf/exception/system.py
--rw-r--r--   0        0        0        1 2023-03-01 12:35:37.104052 pywolf-0.3.2/pywolf/lang/__init__.py
--rw-r--r--   0        0        0     1151 2023-03-27 15:11:26.149783 pywolf-0.3.2/pywolf/lang/fileutils.py
--rw-r--r--   0        0        0      188 2023-03-27 15:11:26.145228 pywolf-0.3.2/pywolf/lang/pathutils.py
--rw-r--r--   0        0        0      311 2023-03-27 15:07:41.254727 pywolf-0.3.2/pywolf/lang/strutils.py
--rw-r--r--   0        0        0      445 2023-03-27 15:10:53.361036 pywolf-0.3.2/pywolf/lang/typeutils.py
--rw-r--r--   0        0        0        0 2023-03-31 09:44:30.341150 pywolf-0.3.2/pywolf/middleware/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 13:08:54.715411 pywolf-0.3.2/pywolf/middleware/cache/__init__.py
--rw-r--r--   0        0        0      955 2023-04-03 07:29:16.134118 pywolf-0.3.2/pywolf/middleware/cache/cache.py
--rw-r--r--   0        0        0      170 2023-03-31 13:47:40.277878 pywolf-0.3.2/pywolf/middleware/cache/cache_config_demo.yaml
--rw-r--r--   0        0        0      319 2023-04-03 07:25:34.025888 pywolf-0.3.2/pywolf/middleware/cache/config.py
--rw-r--r--   0        0        0        1 2023-03-20 07:52:57.219575 pywolf-0.3.2/pywolf/net/__init__.py
--rw-r--r--   0        0        0     1120 2023-03-31 15:59:57.602544 pywolf-0.3.2/pywolf/net/connection.py
--rw-r--r--   0        0        0      324 2023-03-25 06:24:07.956608 pywolf-0.3.2/pywolf/net/httpclient.py
--rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 pywolf-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-03-01 12:22:11.903833 pywolf-0.3.3/LICENSE
+-rw-r--r--   0        0        0        1 2023-03-17 16:04:20.392530 pywolf-0.3.3/bin/__init__.py
+-rw-r--r--   0        0        0      583 2023-07-26 12:08:56.564447 pywolf-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-21 03:39:26.790188 pywolf-0.3.3/pywolf/__init__.py
+-rw-r--r--   0        0        0        1 2023-03-21 03:38:40.871188 pywolf-0.3.3/pywolf/application/__init__.py
+-rw-r--r--   0        0        0      427 2023-03-28 07:55:03.811677 pywolf-0.3.3/pywolf/application/application.py
+-rw-r--r--   0        0        0     1026 2023-04-03 07:25:02.947129 pywolf-0.3.3/pywolf/application/bootstrap.py
+-rw-r--r--   0        0        0     1420 2023-03-25 06:20:55.232882 pywolf-0.3.3/pywolf/application/config.py
+-rw-r--r--   0        0        0      870 2023-03-25 06:20:55.225783 pywolf-0.3.3/pywolf/application/context.py
+-rw-r--r--   0        0        0        0 2023-03-19 13:01:39.384217 pywolf-0.3.3/pywolf/application/path.py
+-rw-r--r--   0        0        0        1 2023-03-20 10:06:57.469480 pywolf-0.3.3/pywolf/cli/__init__.py
+-rw-r--r--   0        0        0      456 2023-03-25 06:21:28.984391 pywolf-0.3.3/pywolf/cli/command.py
+-rw-r--r--   0        0        0        1 2023-03-01 12:35:39.620639 pywolf-0.3.3/pywolf/db/__init__.py
+-rw-r--r--   0        0        0      319 2023-03-31 13:14:34.382017 pywolf-0.3.3/pywolf/db/config.py
+-rw-r--r--   0        0        0      977 2023-04-03 07:18:49.153629 pywolf-0.3.3/pywolf/db/db.py
+-rw-r--r--   0        0        0      179 2023-03-31 13:17:43.750803 pywolf-0.3.3/pywolf/db/db_config_demo.yaml
+-rw-r--r--   0        0        0     1444 2023-03-25 06:22:45.891789 pywolf-0.3.3/pywolf/db/executor.py
+-rw-r--r--   0        0        0     1844 2023-03-25 06:22:45.887626 pywolf-0.3.3/pywolf/db/result.py
+-rw-r--r--   0        0        0     1553 2023-03-27 15:18:30.957090 pywolf-0.3.3/pywolf/db/sqlutils.py
+-rw-r--r--   0        0        0      111 2023-03-28 13:26:29.711044 pywolf-0.3.3/pywolf/exception/base.py
+-rw-r--r--   0        0        0      120 2023-03-28 13:26:28.204059 pywolf-0.3.3/pywolf/exception/business.py
+-rw-r--r--   0        0        0      117 2023-03-28 13:26:24.233477 pywolf-0.3.3/pywolf/exception/system.py
+-rw-r--r--   0        0        0        0 2023-03-31 09:44:30.341150 pywolf-0.3.3/pywolf/middleware/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 13:08:54.715411 pywolf-0.3.3/pywolf/middleware/cache/__init__.py
+-rw-r--r--   0        0        0      955 2023-04-03 07:29:16.134118 pywolf-0.3.3/pywolf/middleware/cache/cache.py
+-rw-r--r--   0        0        0      170 2023-03-31 13:47:40.277878 pywolf-0.3.3/pywolf/middleware/cache/cache_config_demo.yaml
+-rw-r--r--   0        0        0      319 2023-04-03 07:25:34.025888 pywolf-0.3.3/pywolf/middleware/cache/config.py
+-rw-r--r--   0        0        0        1 2023-03-20 07:52:57.219575 pywolf-0.3.3/pywolf/net/__init__.py
+-rw-r--r--   0        0        0     1120 2023-03-31 15:59:57.602544 pywolf-0.3.3/pywolf/net/connection.py
+-rw-r--r--   0        0        0      324 2023-03-25 06:24:07.956608 pywolf-0.3.3/pywolf/net/httpclient.py
+-rw-r--r--   0        0        0        1 2023-03-01 12:35:37.104052 pywolf-0.3.3/pywolf/utils/__init__.py
+-rw-r--r--   0        0        0     1151 2023-03-27 15:11:26.149783 pywolf-0.3.3/pywolf/utils/fileutils.py
+-rw-r--r--   0        0        0      188 2023-03-27 15:11:26.145228 pywolf-0.3.3/pywolf/utils/pathutils.py
+-rw-r--r--   0        0        0      311 2023-03-27 15:07:41.254727 pywolf-0.3.3/pywolf/utils/strutils.py
+-rw-r--r--   0        0        0      445 2023-03-27 15:10:53.361036 pywolf-0.3.3/pywolf/utils/typeutils.py
+-rw-r--r--   0        0        0       36 2023-07-26 11:57:20.541006 pywolf-0.3.3/pywolf/utils/urlutils.py
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 pywolf-0.3.3/PKG-INFO
```

### Comparing `pywolf-0.3.2/LICENSE` & `pywolf-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/pyproject.toml` & `pywolf-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywolf"
-version = "0.3.2"
+version = "0.3.3"
 description = "python utils"
 authors = ["winglechen <winglechen@gmail.com>"]
 license = "MIT License"
 packages = [
     {include = "pywolf"},
     {include = "bin/**/*.py"},
 ]
```

### Comparing `pywolf-0.3.2/pywolf/application/bootstrap.py` & `pywolf-0.3.3/pywolf/application/bootstrap.py`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/pywolf/application/config.py` & `pywolf-0.3.3/pywolf/application/config.py`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/pywolf/application/context.py` & `pywolf-0.3.3/pywolf/application/context.py`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/pywolf/db/db.py` & `pywolf-0.3.3/pywolf/db/db.py`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/pywolf/db/executor.py` & `pywolf-0.3.3/pywolf/db/executor.py`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/pywolf/db/result.py` & `pywolf-0.3.3/pywolf/db/result.py`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/pywolf/db/sqlutils.py` & `pywolf-0.3.3/pywolf/db/sqlutils.py`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/pywolf/lang/fileutils.py` & `pywolf-0.3.3/pywolf/utils/fileutils.py`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/pywolf/middleware/cache/cache.py` & `pywolf-0.3.3/pywolf/middleware/cache/cache.py`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/pywolf/net/connection.py` & `pywolf-0.3.3/pywolf/net/connection.py`

 * *Files identical despite different names*

### Comparing `pywolf-0.3.2/PKG-INFO` & `pywolf-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywolf
-Version: 0.3.2
+Version: 0.3.3
 Summary: python utils
 License: MIT
 Author: winglechen
 Author-email: winglechen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

