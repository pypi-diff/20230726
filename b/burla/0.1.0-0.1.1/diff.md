# Comparing `tmp/burla-0.1.0.tar.gz` & `tmp/burla-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.1.0.tar", max compression
+gzip compressed data, was "burla-0.1.1.tar", max compression
```

## Comparing `burla-0.1.0.tar` & `burla-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      503 2023-07-26 19:38:38.352012 burla-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      175 2023-07-26 19:38:38.352012 burla-0.1.0/src/burla/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-26 19:38:38.352012 burla-0.1.0/src/burla/_logstream.py
--rw-r--r--   0        0        0      907 2023-07-26 19:38:38.352012 burla-0.1.0/src/burla/config.py
--rw-r--r--   0        0        0     5593 2023-07-26 19:38:38.352012 burla-0.1.0/src/burla/remote_parallel_map.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 burla-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      535 2023-07-26 20:17:28.637575 burla-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-26 20:17:28.637575 burla-0.1.1/src/burla/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-26 20:17:28.637575 burla-0.1.1/src/burla/_logstream.py
+-rw-r--r--   0        0        0      907 2023-07-26 20:17:28.637575 burla-0.1.1/src/burla/config.py
+-rw-r--r--   0        0        0     5433 2023-07-26 20:17:28.637575 burla-0.1.1/src/burla/remote_parallel_map.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 burla-0.1.1/PKG-INFO
```

### Comparing `burla-0.1.0/src/burla/_logstream.py` & `burla-0.1.1/src/burla/_logstream.py`

 * *Files identical despite different names*

### Comparing `burla-0.1.0/src/burla/config.py` & `burla-0.1.1/src/burla/config.py`

 * *Files identical despite different names*

### Comparing `burla-0.1.0/src/burla/remote_parallel_map.py` & `burla-0.1.1/src/burla/remote_parallel_map.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,17 +87,14 @@
 
 def _remote_parallel_map(
     function_: Callable,
     inputs: list,
     image: Optional[str] = None,
     api_key: Optional[str] = None,
 ):
-    if not function_.__annotations__.get("return") is str:
-        raise AttributeError("Please add the return type annotation 'str' to your input function.")
-
     # https://www.rfc-editor.org/rfc/rfc7235 <- specifies "correct" api key location
     headers = {"Authorization": f"Bearer {api_key or load_api_key_from_local_config()}"}
 
     response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/", json={}, headers=headers)
     response.raise_for_status()
     job_id = response.json()["job_id"]
```

### Comparing `burla-0.1.0/PKG-INFO` & `burla-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.1.0
-Summary: Make your python script 100x faster
+Version: 0.1.1
+Summary: Scale your program across 1000s of computers with one line of code.
 Author: Jake Zuliani
 Author-email: jake@burla.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

