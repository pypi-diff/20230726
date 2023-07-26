# Comparing `tmp/httplus-0.1.1.tar.gz` & `tmp/httplus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httplus-0.1.1.tar", max compression
+gzip compressed data, was "httplus-0.1.2.tar", max compression
```

## Comparing `httplus-0.1.1.tar` & `httplus-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-05-28 07:57:55.312570 httplus-0.1.1/LICENSE
--rw-r--r--   0        0        0     1374 2023-05-31 11:47:23.520807 httplus-0.1.1/README.md
--rw-r--r--   0        0        0       47 2023-05-30 11:55:36.148288 httplus-0.1.1/httplus/__init__.py
--rw-r--r--   0        0        0     4273 2023-07-25 11:00:03.840090 httplus-0.1.1/httplus/client.py
--rw-r--r--   0        0        0     2215 2023-07-19 11:08:10.521237 httplus-0.1.1/httplus/request.py
--rw-r--r--   0        0        0     1174 2023-07-25 11:33:29.457438 httplus-0.1.1/httplus/response.py
--rw-r--r--   0        0        0      398 2023-07-25 11:25:32.674275 httplus-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 httplus-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-28 07:57:55.312570 httplus-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1374 2023-05-31 11:47:23.520807 httplus-0.1.2/README.md
+-rw-r--r--   0        0        0       47 2023-05-30 11:55:36.148288 httplus-0.1.2/httplus/__init__.py
+-rw-r--r--   0        0        0     4234 2023-07-26 11:20:01.672856 httplus-0.1.2/httplus/client.py
+-rw-r--r--   0        0        0     2215 2023-07-19 11:08:10.521237 httplus-0.1.2/httplus/request.py
+-rw-r--r--   0        0        0     1200 2023-07-26 11:20:01.684856 httplus-0.1.2/httplus/response.py
+-rw-r--r--   0        0        0      398 2023-07-26 11:22:42.281905 httplus-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 httplus-0.1.2/PKG-INFO
```

### Comparing `httplus-0.1.1/LICENSE` & `httplus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `httplus-0.1.1/README.md` & `httplus-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `httplus-0.1.1/httplus/client.py` & `httplus-0.1.2/httplus/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-import ssl
 import asyncio
-import socket
-from typing import Optional
-from .request import Request
-from .response import Response
+from httplus.request import Request
+from httplus.response import Response
 
 
 class Client:
     def __init__(self, verify: str = ''):
         self.verify = verify
         self.writer: asyncio.StreamWriter | None = None
         self.reader: asyncio.StreamReader | None = None
```

### Comparing `httplus-0.1.1/httplus/request.py` & `httplus-0.1.2/httplus/request.py`

 * *Files identical despite different names*

### Comparing `httplus-0.1.1/httplus/response.py` & `httplus-0.1.2/httplus/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,18 @@
         self.message = message[:-4]
         self.version = version
 
     def set_header_pair(self, line: bytes):
         self.raw += line
         key, value = line.decode().split(':', maxsplit=1)
         self.headers[key] = value[:-2].strip()
-        if key == 'Content-Type':
+        key = key.lower()
+        if key == 'content-type':
             self.content_type = value
-        elif key == 'Content-Length':
+        elif key == 'content-length':
             self.content_length = int(value)
 
     def set_body(self, line: bytes):
         self.body = line
 
     def json(self) -> dict | list:
         try:
```

### Comparing `httplus-0.1.1/PKG-INFO` & `httplus-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httplus
-Version: 0.1.1
+Version: 0.1.2
 Summary: An HTTP asynchronous client.
 License: MIT
 Author: Manasses Lima
 Author-email: manasseslima@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

