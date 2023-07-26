# Comparing `tmp/lsrestclient-0.2.1.tar.gz` & `tmp/lsrestclient-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsrestclient-0.2.1.tar", max compression
+gzip compressed data, was "lsrestclient-0.2.2.tar", max compression
```

## Comparing `lsrestclient-0.2.1.tar` & `lsrestclient-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-0.2.1/README.md
--rw-r--r--   0        0        0     3142 2023-07-25 14:53:36.290062 lsrestclient-0.2.1/lsrestclient/__init__.py
--rw-r--r--   0        0        0      707 2023-07-25 14:53:46.217996 lsrestclient-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6623 1970-01-01 00:00:00.000000 lsrestclient-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     6181 2023-07-25 09:41:02.649481 lsrestclient-0.2.2/README.md
+-rw-r--r--   0        0        0     3313 2023-07-26 07:12:24.295402 lsrestclient-0.2.2/lsrestclient/__init__.py
+-rw-r--r--   0        0        0      707 2023-07-26 07:12:48.835126 lsrestclient-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6623 1970-01-01 00:00:00.000000 lsrestclient-0.2.2/PKG-INFO
```

### Comparing `lsrestclient-0.2.1/README.md` & `lsrestclient-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `lsrestclient-0.2.1/lsrestclient/__init__.py` & `lsrestclient-0.2.2/lsrestclient/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Optional, Dict, Any
 
 import lsjsonclasses
 import requests
 from requests import Session, Response
 from requests.structures import CaseInsensitiveDict
 
+find_parameters_regex = re.compile('{(.*?)}')
 
-find_parameters_regex = re.compile("\{(.*?)\}")
 
 @dataclass
 class LsRestClientResponse:
     status_code: int
     content: str
     headers: CaseInsensitiveDict
 
@@ -35,25 +35,25 @@
 class LsRestClient(Session):
     _clients = {}
 
     @classmethod
     def client(cls, name):
         try:
             return cls._clients[name]
-        except KeyError as e:
+        except KeyError:
             raise Exception(f"LsRestClient with name '{name}' not initialized.")
 
     def __init__(self, base_url: str = None, name: str = "default") -> None:
         self.base_url = base_url
         self.base_headers = {'content-type': 'application/json'}
         self.name = name
         super().__init__()
         self._clients[name] = self
 
-    def full_url(self, url: str, params: dict | None = None) -> str:
+    def full_url(self, url: str, params: Optional[dict] = None) -> str:
         if params is None:
             params = {}
 
         full_url = f"{self.base_url}{url}"
         found = find_parameters_regex.findall(full_url)
         url_params = {p: params[p] for p in found}
         for p in found:
@@ -81,31 +81,32 @@
             kwargs['data'] = lsjsonclasses.LSoftJSONEncoder.dumps(body).encode("utf8")
 
         return LsRestClientResponse.from_requests_response(
             requests.request(
                 method.upper(),
                 self.full_url(url, params),
                 *args,
+                params=params,
                 **kwargs
             )
         )
 
-    def get(self, *args, **kwargs):
+    def get(self, *args, **kwargs) -> LsRestClientResponse:
         return self.request('GET', *args, **kwargs)
 
-    def post(self, *args, **kwargs):
+    def post(self, *args, **kwargs) -> LsRestClientResponse:
         return self.request('POST', *args, **kwargs)
 
-    def put(self, *args, **kwargs):
+    def put(self, *args, **kwargs) -> LsRestClientResponse:
         return self.request('PUT', *args, **kwargs)
 
-    def patch(self, *args, **kwargs):
+    def patch(self, *args, **kwargs) -> LsRestClientResponse:
         return self.request('PATCH', *args, **kwargs)
 
-    def delete(self, *args, **kwargs):
+    def delete(self, *args, **kwargs) -> LsRestClientResponse:
         return self.request('DELETE', *args, **kwargs)
 
-    def options(self, *args, **kwargs):
+    def options(self, *args, **kwargs) -> LsRestClientResponse:
         return self.request('OPTIONS', *args, **kwargs)
 
     def head(self, *args, **kwargs):
         return self.request('HEAD', *args, **kwargs)
```

### Comparing `lsrestclient-0.2.1/pyproject.toml` & `lsrestclient-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lsrestclient"
-version = "0.2.1"
+version = "0.2.2"
 description = "REST Api Client"
 authors = ["mba <bartel@electronic-shop.lu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
```

### Comparing `lsrestclient-0.2.1/PKG-INFO` & `lsrestclient-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsrestclient
-Version: 0.2.1
+Version: 0.2.2
 Summary: REST Api Client
 Author: mba
 Author-email: bartel@electronic-shop.lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

