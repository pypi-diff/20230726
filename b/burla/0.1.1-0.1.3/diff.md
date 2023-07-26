# Comparing `tmp/burla-0.1.1.tar.gz` & `tmp/burla-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.1.1.tar", max compression
+gzip compressed data, was "burla-0.1.3.tar", max compression
```

## Comparing `burla-0.1.1.tar` & `burla-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      535 2023-07-26 20:17:28.637575 burla-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      175 2023-07-26 20:17:28.637575 burla-0.1.1/src/burla/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-26 20:17:28.637575 burla-0.1.1/src/burla/_logstream.py
--rw-r--r--   0        0        0      907 2023-07-26 20:17:28.637575 burla-0.1.1/src/burla/config.py
--rw-r--r--   0        0        0     5433 2023-07-26 20:17:28.637575 burla-0.1.1/src/burla/remote_parallel_map.py
--rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 burla-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      535 2023-07-26 21:20:40.795038 burla-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-26 21:20:40.795038 burla-0.1.3/src/burla/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-26 21:20:40.795038 burla-0.1.3/src/burla/_logstream.py
+-rw-r--r--   0        0        0      907 2023-07-26 21:20:40.795038 burla-0.1.3/src/burla/config.py
+-rw-r--r--   0        0        0     5560 2023-07-26 21:20:40.795038 burla-0.1.3/src/burla/remote_parallel_map.py
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 burla-0.1.3/PKG-INFO
```

### Comparing `burla-0.1.1/pyproject.toml` & `burla-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "burla"
-version = "0.1.1"
+version = "0.1.3"
 description = "Scale your program across 1000s of computers with one line of code."
 authors = ["Jake Zuliani <jake@burla.dev>"]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dill = "^0.3.6"
```

### Comparing `burla-0.1.1/src/burla/_logstream.py` & `burla-0.1.3/src/burla/_logstream.py`

 * *Files identical despite different names*

### Comparing `burla-0.1.1/src/burla/config.py` & `burla-0.1.3/src/burla/config.py`

 * *Files identical despite different names*

### Comparing `burla-0.1.1/src/burla/remote_parallel_map.py` & `burla-0.1.3/src/burla/remote_parallel_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from tblib import pickling_support
 
 from burla._logstream import print_logs_from_queue
 from burla.config import load_api_key_from_local_config
 
 pickling_support.install()
 
-BURLA_SERVICE_URL = "https://burla-webservice-zqhes3whbq-uc.a.run.app"  # prod
-JOB_ENV_REPO = "us-docker.pkg.dev/burla-prod/burla-job-environments"
+# BURLA_SERVICE_URL = "https://burla-webservice-zqhes3whbq-uc.a.run.app"  # prod
+# JOB_ENV_REPO = "us-docker.pkg.dev/burla-prod/burla-job-environments"
 
-# BURLA_SERVICE_URL = "https://burla-webservice-y66ufvpuua-uc.a.run.app"  # test
-# JOB_ENV_REPO = "us-docker.pkg.dev/burla-test/burla-job-environments"
+BURLA_SERVICE_URL = "https://burla-webservice-y66ufvpuua-uc.a.run.app"  # test
+JOB_ENV_REPO = "us-docker.pkg.dev/burla-test/burla-job-environments"
 
 # BURLA_SERVICE_URL = "http://127.0.0.1:5000"
 
 MAX_CONCURRENCY = 100  # If your snooping on my code and want to increase this, don't, it wont work.
 JOB_STATUS_POLL_RATE_SEC = 6  # how often to check for job completion
 TIMEOUT_MIN = 60 * 12  # max time a Burla job can run for
 
@@ -77,19 +77,22 @@
             )
         )
     outputs = []
     input_batches = [
         inputs[i : i + MAX_CONCURRENCY] for i in range(0, len(inputs), MAX_CONCURRENCY)
     ]
     for input_batch in input_batches:
-        outputs.extend(_remote_parallel_map(function_, input_batch, image, api_key))
-    return outputs
+        outputs.extend(remote_parallel_map_single_batch(function_, input_batch, image, api_key))
 
+    all_outputs_are_none = all(item is None for item in outputs)
+    if not all_outputs_are_none:
+        return outputs
 
-def _remote_parallel_map(
+
+def remote_parallel_map_single_batch(
     function_: Callable,
     inputs: list,
     image: Optional[str] = None,
     api_key: Optional[str] = None,
 ):
     # https://www.rfc-editor.org/rfc/rfc7235 <- specifies "correct" api key location
     headers = {"Authorization": f"Bearer {api_key or load_api_key_from_local_config()}"}
```

### Comparing `burla-0.1.1/PKG-INFO` & `burla-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.1.1
+Version: 0.1.3
 Summary: Scale your program across 1000s of computers with one line of code.
 Author: Jake Zuliani
 Author-email: jake@burla.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

