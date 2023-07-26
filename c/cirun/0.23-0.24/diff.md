# Comparing `tmp/cirun-0.23.tar.gz` & `tmp/cirun-0.24.tar.gz`

## Comparing `cirun-0.23.tar` & `cirun-0.24.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cirun-0.23/requirements.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cirun-0.23/cirun/__about__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cirun-0.23/cirun/__init__.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 cirun-0.23/cirun/client.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 cirun-0.23/cirun/cloud.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cirun-0.23/cirun/main.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 cirun-0.23/cirun/repo.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cirun-0.23/cirun/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cirun-0.23/cirun/tests/__init__.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 cirun-0.23/cirun/tests/test_client.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cirun-0.23/tests/__init__.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 cirun-0.23/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cirun-0.23/LICENSE.txt
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 cirun-0.23/README.md
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 cirun-0.23/pyproject.toml
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 cirun-0.23/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 cirun-0.24/requirements.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cirun-0.24/cirun/__about__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 cirun-0.24/cirun/__init__.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 cirun-0.24/cirun/client.py
+-rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 cirun-0.24/cirun/cloud.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cirun-0.24/cirun/main.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 cirun-0.24/cirun/repo.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cirun-0.24/cirun/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cirun-0.24/cirun/tests/__init__.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 cirun-0.24/cirun/tests/test_client.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cirun-0.24/tests/__init__.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 cirun-0.24/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cirun-0.24/LICENSE.txt
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 cirun-0.24/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 cirun-0.24/pyproject.toml
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 cirun-0.24/PKG-INFO
```

### Comparing `cirun-0.23/cirun/client.py` & `cirun-0.24/cirun/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 import requests
 from rich.console import Console
 
-API_ENDPOINT = "https://cirun.io/api/v1"
+API_ENDPOINT = "https://api.cirun.io/api/v1"
 
 
 class CirunAPIException(Exception):
     pass
 
 
 def _print_error(response):
@@ -26,14 +26,15 @@
     return rjson
 
 
 class Cirun:
     def __init__(self, token=None):
         self.token = token
         self._get_credentials()
+        self.api_endpoint = os.environ.get('CIRUN_API_ENDPOINT', API_ENDPOINT)
 
     def _get_credentials(self):
         if not self.token:
             try:
                 token = os.environ['CIRUN_API_KEY']
                 self.token = token
             except KeyError:
@@ -42,18 +43,18 @@
     def _headers(self):
         return {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.token}"
         }
 
     def _get(self, path, *args, **kwargs):
-        return requests.get(f"{API_ENDPOINT}/{path}", headers=self._headers(), *args, **kwargs)
+        return requests.get(f"{self.api_endpoint}/{path}", headers=self._headers(), *args, **kwargs)
 
     def _post(self, path, *args, **kwargs):
-        return requests.post(f"{API_ENDPOINT}/{path}", headers=self._headers(), *args, **kwargs)
+        return requests.post(f"{self.api_endpoint}/{path}", headers=self._headers(), *args, **kwargs)
 
     def get_repos(self, print_error=False):
         """Get all the repositories connected to cirun."""
         response = self._get("repo")
         if response.status_code not in [200, 201]:
             if print_error:
                 return _print_error(response)
```

### Comparing `cirun-0.23/cirun/cloud.py` & `cirun-0.24/cirun/cloud.py`

 * *Files identical despite different names*

### Comparing `cirun-0.23/cirun/main.py` & `cirun-0.24/cirun/main.py`

 * *Files identical despite different names*

### Comparing `cirun-0.23/cirun/repo.py` & `cirun-0.24/cirun/repo.py`

 * *Files identical despite different names*

### Comparing `cirun-0.23/.gitignore` & `cirun-0.24/.gitignore`

 * *Files identical despite different names*

### Comparing `cirun-0.23/LICENSE.txt` & `cirun-0.24/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cirun-0.23/README.md` & `cirun-0.24/README.md`

 * *Files identical despite different names*

### Comparing `cirun-0.23/pyproject.toml` & `cirun-0.24/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 keywords = []
 authors = [
   { name = "Amit Kumar", email = "amit@cirun.io" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
@@ -47,15 +46,15 @@
 ]
 
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=cirun --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
-python = ["37", "38", "39", "310", "311"]
+python = ["38", "39", "310", "311"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "cirun/__about__.py",
 ]
```

### Comparing `cirun-0.23/PKG-INFO` & `cirun-0.24/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: cirun
-Version: 0.23
+Version: 0.24
 Summary: Cirun Python Client
 Project-URL: Documentation, https://github.com/aktechlabs/cirun-py#readme
 Project-URL: Issues, https://github.com/aktechlabs/cirun-py/issues
 Project-URL: Source, https://github.com/aktechlabs/cirun-py
 Author-email: Amit Kumar <amit@cirun.io>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
```

