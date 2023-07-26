# Comparing `tmp/zero_python_sdk-0.2.0.tar.gz` & `tmp/zero_python_sdk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zero_python_sdk-0.2.0.tar", max compression
+gzip compressed data, was "zero_python_sdk-0.2.1.tar", max compression
```

## Comparing `zero_python_sdk-0.2.0.tar` & `zero_python_sdk-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0      741 2023-07-24 08:00:59.404919 zero_python_sdk-0.2.0/LICENSE
--rw-r--r--   0        0        0      402 2023-07-24 10:27:14.876660 zero_python_sdk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      128 2023-07-24 08:00:59.406299 zero_python_sdk-0.2.0/zero_python_sdk/__init__.py
--rw-r--r--   0        0        0     1916 2023-07-24 09:51:38.935016 zero_python_sdk-0.2.0/zero_python_sdk/zero.py
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 zero_python_sdk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      741 2023-07-26 14:18:50.739412 zero_python_sdk-0.2.1/LICENSE
+-rw-r--r--   0        0        0      530 2023-07-26 14:18:50.739412 zero_python_sdk-0.2.1/README.md
+-rw-r--r--   0        0        0      423 2023-07-26 14:18:50.743412 zero_python_sdk-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      128 2023-07-26 14:18:50.743412 zero_python_sdk-0.2.1/zero_python_sdk/__init__.py
+-rw-r--r--   0        0        0     1964 2023-07-26 14:18:50.743412 zero_python_sdk-0.2.1/zero_python_sdk/zero.py
+-rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 zero_python_sdk-0.2.1/PKG-INFO
```

### Comparing `zero_python_sdk-0.2.0/LICENSE` & `zero_python_sdk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zero_python_sdk-0.2.0/zero_python_sdk/zero.py` & `zero_python_sdk-0.2.1/zero_python_sdk/zero.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 """Zero SDK for Python"""
 import asyncio
 from typing import List, Dict, Optional
-
 from python_graphql_client import GraphqlClient
 
 
 class ZeroException(Exception):
     pass
 
 
 class ZeroApiClient:
     """The Zero API"""
 
-    query = """
-        query Secrets($token: String!, $pick: [String!], callerName: String) {
-            secrets(zeroToken: $token, pick: $pick, callerName: $callerName) {
-                name
-
-                fields {
+    def __init__(self, url: str, token: str, pick: List[str], caller_name: Optional[str]):
+        self.query = """
+            query Secrets($token: String!, $pick: [String!], $callerName: String) {
+                secrets(zeroToken: $token, pick: $pick, callerName: $callerName) {
                     name
-                    value
+                    fields {
+                        name
+                        value
+                    }
                 }
             }
-        }
-    """
+        """
 
-    def __init__(self, url: str, token: str, pick: List[str], caller_name: Optional[str]):
         self.client = GraphqlClient(endpoint=url)
         self.variables = {"token": token, "pick": pick, "callerName": caller_name}
 
     def fetch(self) -> Dict[str, Dict[str, str]]:
         """Grab the secrets from the Zero API"""
 
         response_body = asyncio.run(
```

