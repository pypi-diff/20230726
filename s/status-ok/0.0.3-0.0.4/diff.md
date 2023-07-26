# Comparing `tmp/status_ok-0.0.3.tar.gz` & `tmp/status_ok-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "status_ok-0.0.3.tar", last modified: Tue Jul 25 11:06:47 2023, max compression
+gzip compressed data, was "status_ok-0.0.4.tar", last modified: Wed Jul 26 15:02:22 2023, max compression
```

## Comparing `status_ok-0.0.3.tar` & `status_ok-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-25 11:06:47.173451 status_ok-0.0.3/
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      490 2023-07-25 11:06:47.173338 status_ok-0.0.3/PKG-INFO
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)       38 2023-07-25 11:06:47.173490 status_ok-0.0.3/setup.cfg
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      728 2023-07-25 11:06:16.000000 status_ok-0.0.3/setup.py
-drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-25 11:06:47.172457 status_ok-0.0.3/status_ok/
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-20 08:56:59.000000 status_ok-0.0.3/status_ok/__init__.py
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      837 2023-07-25 11:03:43.000000 status_ok-0.0.3/status_ok/handle_error.py
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      420 2023-07-25 11:05:50.000000 status_ok-0.0.3/status_ok/status.py
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)     2006 2023-07-25 11:00:07.000000 status_ok-0.0.3/status_ok/status_codex.py
-drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-25 11:06:47.173160 status_ok-0.0.3/status_ok.egg-info/
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      490 2023-07-25 11:06:47.000000 status_ok-0.0.3/status_ok.egg-info/PKG-INFO
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      266 2023-07-25 11:06:47.000000 status_ok-0.0.3/status_ok.egg-info/SOURCES.txt
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        1 2023-07-25 11:06:47.000000 status_ok-0.0.3/status_ok.egg-info/dependency_links.txt
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        9 2023-07-25 11:06:47.000000 status_ok-0.0.3/status_ok.egg-info/requires.txt
--rw-r--r--   0 YuvrajSynapses   (502) staff       (20)       10 2023-07-25 11:06:47.000000 status_ok-0.0.3/status_ok.egg-info/top_level.txt
+drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-26 15:02:22.140040 status_ok-0.0.4/
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      490 2023-07-26 15:02:22.139927 status_ok-0.0.4/PKG-INFO
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)       38 2023-07-26 15:02:22.140075 status_ok-0.0.4/setup.cfg
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      728 2023-07-26 15:02:15.000000 status_ok-0.0.4/setup.py
+drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-26 15:02:22.139047 status_ok-0.0.4/status_ok/
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-20 08:56:59.000000 status_ok-0.0.4/status_ok/__init__.py
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      837 2023-07-25 11:03:43.000000 status_ok-0.0.4/status_ok/handle_error.py
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      789 2023-07-26 14:28:00.000000 status_ok-0.0.4/status_ok/status.py
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)     2353 2023-07-26 14:59:34.000000 status_ok-0.0.4/status_ok/status_codex.py
+drwxr-xr-x   0 YuvrajSynapses   (502) staff       (20)        0 2023-07-26 15:02:22.139762 status_ok-0.0.4/status_ok.egg-info/
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      490 2023-07-26 15:02:22.000000 status_ok-0.0.4/status_ok.egg-info/PKG-INFO
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)      266 2023-07-26 15:02:22.000000 status_ok-0.0.4/status_ok.egg-info/SOURCES.txt
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        1 2023-07-26 15:02:22.000000 status_ok-0.0.4/status_ok.egg-info/dependency_links.txt
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)        9 2023-07-26 15:02:22.000000 status_ok-0.0.4/status_ok.egg-info/requires.txt
+-rw-r--r--   0 YuvrajSynapses   (502) staff       (20)       10 2023-07-26 15:02:22.000000 status_ok-0.0.4/status_ok.egg-info/top_level.txt
```

### Comparing `status_ok-0.0.3/setup.py` & `status_ok-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 LICENSE = 'MIT'
 REQUIRES = [
     'requests',
 ]
 
 setup(
     name="status_ok",
-    version="0.0.3",
+    version="0.0.4",
     description="This library is used to handle http responses.",
     long_description="This library is used to handle http responses in python.",
     long_description_content_type='text/markdown',
     author="yuvraj jaiswal",
     author_email="y.jaiswal@thesynapses.com",
     url="https://github.com/iLS-yuvrajj/statusOk/tree/main",
     license=LICENSE,
```

### Comparing `status_ok-0.0.3/status_ok/handle_error.py` & `status_ok-0.0.4/status_ok/handle_error.py`

 * *Files identical despite different names*

### Comparing `status_ok-0.0.3/status_ok/status_codex.py` & `status_ok-0.0.4/status_ok/status_codex.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,67 @@
 
-status_codes = {
-        100: "Continue",
-        101: "Switching Protocols",
-        102: "Processing",
-        103: "Early Hints",
-        200: "OK", 201: "Created",202: "Accepted",
-        203: "Non - Authoritative Information",
-        204: "No Content",
-        205: "Reset Content",
-        206: "Partial Content",
-        207: "Multi - Status",
-        208: "Already Reported",
-        226: "IM Used",
-        300: "Multiple Choices",
-        301: "Moved Permanently",
-        302: "Found",
-        303: "See Other",
-        304: "Not Modified",
-        305: "Use Proxy",
-        307: "Temporary Redirect",
-        308: "Permanent Redirect",
-        400: "Bad Request",
-        401: "Unauthorized",
-        402: "Payment Required",
-        403: "Forbidden",
-        404: "Not Found",
-        405: "Method Not Allowed",
-        406: "Not Acceptable",
-        407: "Proxy Authentication Required",
-        408: "Request Timeout",
-        409: "Conflict",
-        410: "Gone",
-        411: "Length Required",
-        412: "Precondition Failed",
-        413: "Payload Too Large",
-        414: "URI Too Long",
-        415: "Unsupported Media Type",
-        416: "Range Not Satisfiable",
-        417: "Expectation Failed",
-        418: "Im a teapot",
-        421: "Misdirected Request",
-        422: "Unprocessable Entity",
-        423: "Locked",
-        424: "Failed Dependency",
-        425: "Too Early",
-        426: "Upgrade Required",
-        428: "Precondition Required",
-        429: "Too Many Requests",
-        431: "Request Header Fields Too Large",
-        451: "Unavailable For Legal Reasons",
-        500: "Internal Server Error",
-        501: "Not Implemented",
-        502: "Bad Gateway",
-        503: "Service Unavailable",
-        504: "Gateway Timeout",
-        505: "HTTP Version Not Supported",
-        506: "Variant Also Negotiates",
-        507: "Insufficient Storage",
-        508: "Loop Detected",
-        510: "Not Extended",
-        511: "Network Authentication Required"
-    }
+class Custom_status:
+    def __init__(self):
+        self.status_codes = {
+            100: "Continue",
+            101: "Switching Protocols",
+            102: "Processing",
+            103: "Early Hints",
+            200: "OK", 201: "Created",202: "Accepted",
+            203: "Non - Authoritative Information",
+            204: "No Content",
+            205: "Reset Content",
+            206: "Partial Content",
+            207: "Multi - Status",
+            208: "Already Reported",
+            226: "IM Used",
+            300: "Multiple Choices",
+            301: "Moved Permanently",
+            302: "Found",
+            303: "See Other",
+            304: "Not Modified",
+            305: "Use Proxy",
+            307: "Temporary Redirect",
+            308: "Permanent Redirect",
+            400: "Bad Request",
+            401: "Unauthorized",
+            402: "Payment Required",
+            403: "Forbidden",
+            404: "Not Found",
+            405: "Method Not Allowed",
+            406: "Not Acceptable",
+            407: "Proxy Authentication Required",
+            408: "Request Timeout",
+            409: "Conflict",
+            410: "Gone",
+            411: "Length Required",
+            412: "Precondition Failed",
+            413: "Payload Too Large",
+            414: "URI Too Long",
+            415: "Unsupported Media Type",
+            416: "Range Not Satisfiable",
+            417: "Expectation Failed",
+            418: "Im a teapot",
+            421: "Misdirected Request",
+            422: "Unprocessable Entity",
+            423: "Locked",
+            424: "Failed Dependency",
+            425: "Too Early",
+            426: "Upgrade Required",
+            428: "Precondition Required",
+            429: "Too Many Requests",
+            431: "Request Header Fields Too Large",
+            451: "Unavailable For Legal Reasons",
+            500: "Internal Server Error",
+            501: "Not Implemented",
+            502: "Bad Gateway",
+            503: "Service Unavailable",
+            504: "Gateway Timeout",
+            505: "HTTP Version Not Supported",
+            506: "Variant Also Negotiates",
+            507: "Insufficient Storage",
+            508: "Loop Detected",
+            510: "Not Extended",
+            511: "Network Authentication Required"
+        }
+
+status_codes = Custom_status().status_codes
```

