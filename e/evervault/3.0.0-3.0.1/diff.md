# Comparing `tmp/evervault-3.0.0.tar.gz` & `tmp/evervault-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evervault-3.0.0.tar", max compression
+gzip compressed data, was "evervault-3.0.1.tar", max compression
```

## Comparing `evervault-3.0.0.tar` & `evervault-3.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1109 2023-05-25 15:56:34.253287 evervault-3.0.0/LICENSE
--rw-r--r--   0        0        0     9598 2023-07-21 12:11:23.147023 evervault-3.0.0/README.md
--rw-r--r--   0        0        0     5424 2023-07-25 11:03:54.075017 evervault-3.0.0/evervault/__init__.py
--rw-r--r--   0        0        0     4126 2023-05-25 15:56:34.253794 evervault-3.0.0/evervault/cages_v2.py
--rw-r--r--   0        0        0     4795 2023-07-21 12:11:23.147444 evervault-3.0.0/evervault/client.py
--rw-r--r--   0        0        0       55 2023-05-25 15:56:34.254073 evervault-3.0.0/evervault/crypto/__init__.py
--rw-r--r--   0        0        0     8468 2023-07-21 12:11:23.148512 evervault-3.0.0/evervault/crypto/client.py
--rw-r--r--   0        0        0       58 2023-05-25 15:56:34.254370 evervault-3.0.0/evervault/crypto/curves/__init__.py
--rw-r--r--   0        0        0     3428 2023-05-25 15:56:34.254522 evervault-3.0.0/evervault/crypto/curves/base.py
--rw-r--r--   0        0        0      779 2023-05-25 15:56:34.254660 evervault-3.0.0/evervault/crypto/curves/p256.py
--rw-r--r--   0        0        0       71 2023-05-25 15:56:34.254779 evervault-3.0.0/evervault/crypto/version.py
--rw-r--r--   0        0        0      112 2023-05-25 15:56:34.254938 evervault-3.0.0/evervault/datatypes/__init__.py
--rw-r--r--   0        0        0      376 2023-05-25 15:56:34.255055 evervault-3.0.0/evervault/datatypes/map.py
--rw-r--r--   0        0        0       43 2023-05-25 15:56:34.255199 evervault-3.0.0/evervault/errors/__init__.py
--rw-r--r--   0        0        0     1816 2023-05-25 15:56:34.255323 evervault-3.0.0/evervault/errors/error_handler.py
--rw-r--r--   0        0        0     1194 2023-05-25 15:56:34.255426 evervault-3.0.0/evervault/errors/evervault_errors.py
--rw-r--r--   0        0        0       37 2023-05-25 15:56:34.255561 evervault-3.0.0/evervault/http/__init__.py
--rw-r--r--   0        0        0     2260 2023-05-25 15:56:34.255678 evervault-3.0.0/evervault/http/outboundrelayconfig.py
--rw-r--r--   0        0        0     3926 2023-07-21 12:11:23.148904 evervault-3.0.0/evervault/http/request.py
--rw-r--r--   0        0        0     1201 2023-05-25 15:56:34.255939 evervault-3.0.0/evervault/http/requesthandler.py
--rw-r--r--   0        0        0     8546 2023-05-25 15:56:34.256091 evervault-3.0.0/evervault/http/requestintercept.py
--rw-r--r--   0        0        0       73 2023-05-25 15:56:34.256292 evervault-3.0.0/evervault/models/__init__.py
--rw-r--r--   0        0        0      315 2023-05-25 15:56:34.256396 evervault-3.0.0/evervault/models/cage.py
--rw-r--r--   0        0        0      392 2023-05-25 15:56:34.256485 evervault-3.0.0/evervault/models/cage_list.py
--rw-r--r--   0        0        0        0 2023-05-25 15:56:34.256570 evervault-3.0.0/evervault/services/__init__.py
--rw-r--r--   0        0        0      136 2023-05-25 15:56:34.256663 evervault-3.0.0/evervault/services/timeservice.py
--rw-r--r--   0        0        0     1143 2023-05-25 15:56:34.256806 evervault-3.0.0/evervault/threading/repeatedtimer.py
--rw-r--r--   0        0        0     1076 2023-07-25 10:50:58.265829 evervault-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    10527 1970-01-01 00:00:00.000000 evervault-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-07-26 15:00:28.516889 evervault-3.0.1/LICENSE
+-rw-r--r--   0        0        0     9598 2023-07-26 15:00:28.516889 evervault-3.0.1/README.md
+-rw-r--r--   0        0        0     5424 2023-07-26 15:00:55.666833 evervault-3.0.1/evervault/__init__.py
+-rw-r--r--   0        0        0     4126 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/cages_v2.py
+-rw-r--r--   0        0        0     4795 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/client.py
+-rw-r--r--   0        0        0       55 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/crypto/__init__.py
+-rw-r--r--   0        0        0     8468 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/crypto/client.py
+-rw-r--r--   0        0        0       58 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/crypto/curves/__init__.py
+-rw-r--r--   0        0        0     3428 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/crypto/curves/base.py
+-rw-r--r--   0        0        0      779 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/crypto/curves/p256.py
+-rw-r--r--   0        0        0       71 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/crypto/version.py
+-rw-r--r--   0        0        0      112 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/datatypes/__init__.py
+-rw-r--r--   0        0        0      376 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/datatypes/map.py
+-rw-r--r--   0        0        0       43 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/errors/__init__.py
+-rw-r--r--   0        0        0     1816 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/errors/error_handler.py
+-rw-r--r--   0        0        0     1194 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/errors/evervault_errors.py
+-rw-r--r--   0        0        0       37 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/http/__init__.py
+-rw-r--r--   0        0        0     2260 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/http/outboundrelayconfig.py
+-rw-r--r--   0        0        0     4001 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/http/request.py
+-rw-r--r--   0        0        0     1201 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/http/requesthandler.py
+-rw-r--r--   0        0        0     8546 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/http/requestintercept.py
+-rw-r--r--   0        0        0       73 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/models/__init__.py
+-rw-r--r--   0        0        0      315 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/models/cage.py
+-rw-r--r--   0        0        0      392 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/models/cage_list.py
+-rw-r--r--   0        0        0        0 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/services/__init__.py
+-rw-r--r--   0        0        0      136 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/services/timeservice.py
+-rw-r--r--   0        0        0     1143 2023-07-26 15:00:28.516889 evervault-3.0.1/evervault/threading/repeatedtimer.py
+-rw-r--r--   0        0        0     1076 2023-07-26 15:00:55.674833 evervault-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10527 1970-01-01 00:00:00.000000 evervault-3.0.1/PKG-INFO
```

### Comparing `evervault-3.0.0/LICENSE` & `evervault-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/README.md` & `evervault-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/__init__.py` & `evervault-3.0.1/evervault/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from .client import Client
 from .errors.evervault_errors import AuthenticationError, UnsupportedCurveError
 from .cages_v2 import CageRequestsSession
 import os
 import sys
 from warnings import warn
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 
 ev_client = None
 _app_uuid = None
 _api_key = None
 request_timeout = 30
 _retry = False
 _curve = None
```

### Comparing `evervault-3.0.0/evervault/cages_v2.py` & `evervault-3.0.1/evervault/cages_v2.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/client.py` & `evervault-3.0.1/evervault/client.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/crypto/client.py` & `evervault-3.0.1/evervault/crypto/client.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/crypto/curves/base.py` & `evervault-3.0.1/evervault/crypto/curves/base.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/crypto/curves/p256.py` & `evervault-3.0.1/evervault/crypto/curves/p256.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/errors/error_handler.py` & `evervault-3.0.1/evervault/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/errors/evervault_errors.py` & `evervault-3.0.1/evervault/errors/evervault_errors.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/http/outboundrelayconfig.py` & `evervault-3.0.1/evervault/http/outboundrelayconfig.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/http/request.py` & `evervault-3.0.1/evervault/http/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,13 +99,14 @@
             allow_redirects=False,
             **req_params,
         )
 
     def __parse_body(self, resp, should_parse=True):
         if resp.content and resp.content.strip():
             try:
-                decoded_body = resp.content.decode(
-                    resp.encoding or resp.apparent_encoding
-                )
+                encoding = resp.encoding or resp.apparent_encoding
+                if encoding is None:
+                    return resp.content
+                decoded_body = resp.content.decode(encoding)
                 return json.loads(decoded_body) if should_parse else decoded_body
             except ValueError:
                 error_handler.raise_errors_on_failure(resp)
```

### Comparing `evervault-3.0.0/evervault/http/requesthandler.py` & `evervault-3.0.1/evervault/http/requesthandler.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/http/requestintercept.py` & `evervault-3.0.1/evervault/http/requestintercept.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/evervault/threading/repeatedtimer.py` & `evervault-3.0.1/evervault/threading/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `evervault-3.0.0/pyproject.toml` & `evervault-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "evervault"
-version = "3.0.0"
+version = "3.0.1"
 description = "Evervault SDK"
 authors = ["Evervault <engineering@evervault.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://evervault.com"
 repository = "https://github.com/evervault/evervault-python"
```

### Comparing `evervault-3.0.0/PKG-INFO` & `evervault-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evervault
-Version: 3.0.0
+Version: 3.0.1
 Summary: Evervault SDK
 Home-page: https://evervault.com
 License: MIT
 Author: Evervault
 Author-email: engineering@evervault.com
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

