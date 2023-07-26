# Comparing `tmp/burla-0.0.9.tar.gz` & `tmp/burla-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "burla-0.0.9.tar", max compression
+gzip compressed data, was "burla-0.1.0.tar", max compression
```

## Comparing `burla-0.0.9.tar` & `burla-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      503 2023-07-18 23:01:39.157499 burla-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      175 2023-07-13 18:25:13.491110 burla-0.0.9/src/burla/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-12 19:34:52.816658 burla-0.0.9/src/burla/_logstream.py
--rw-r--r--   0        0        0      907 2023-07-13 18:24:57.649392 burla-0.0.9/src/burla/config.py
--rw-r--r--   0        0        0     4407 2023-07-18 23:02:00.574713 burla-0.0.9/src/burla/remote_parallel_map.py
--rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 burla-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      503 2023-07-26 19:38:38.352012 burla-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-26 19:38:38.352012 burla-0.1.0/src/burla/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-26 19:38:38.352012 burla-0.1.0/src/burla/_logstream.py
+-rw-r--r--   0        0        0      907 2023-07-26 19:38:38.352012 burla-0.1.0/src/burla/config.py
+-rw-r--r--   0        0        0     5593 2023-07-26 19:38:38.352012 burla-0.1.0/src/burla/remote_parallel_map.py
+-rw-r--r--   0        0        0      616 1970-01-01 00:00:00.000000 burla-0.1.0/PKG-INFO
```

### Comparing `burla-0.0.9/src/burla/_logstream.py` & `burla-0.1.0/src/burla/_logstream.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.9/src/burla/config.py` & `burla-0.1.0/src/burla/config.py`

 * *Files identical despite different names*

### Comparing `burla-0.0.9/src/burla/remote_parallel_map.py` & `burla-0.1.0/src/burla/remote_parallel_map.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 import sys
 import requests
-import threading
 import warnings
 import pickle
+import math
 from six import reraise
+from threading import Thread, Event
 from typing import Callable, Optional
 from time import sleep, time
 from queue import PriorityQueue
 
 import dill
 from tblib import pickling_support
 
 from burla._logstream import print_logs_from_queue
 from burla.config import load_api_key_from_local_config
 
 pickling_support.install()
 
-BURLA_SERVICE_URL = "https://burla-webservice-prod-0-0-9-gxc7eo4ala-uc.a.run.app"
-# BURLA_SERVICE_URL = "https://burla-webservice-gxc7eo4ala-uc.a.run.app"
-# BURLA_SERVICE_URL = "https://127.0.0.1:5000"
+BURLA_SERVICE_URL = "https://burla-webservice-zqhes3whbq-uc.a.run.app"  # prod
+JOB_ENV_REPO = "us-docker.pkg.dev/burla-prod/burla-job-environments"
 
-JOB_ENV_REPO = "us-east4-docker.pkg.dev/burla-389321/burla-job-environments"
+# BURLA_SERVICE_URL = "https://burla-webservice-y66ufvpuua-uc.a.run.app"  # test
+# JOB_ENV_REPO = "us-docker.pkg.dev/burla-test/burla-job-environments"
 
+# BURLA_SERVICE_URL = "http://127.0.0.1:5000"
+
+MAX_CONCURRENCY = 100  # If your snooping on my code and want to increase this, don't, it wont work.
 JOB_STATUS_POLL_RATE_SEC = 6  # how often to check for job completion
 TIMEOUT_MIN = 60 * 12  # max time a Burla job can run for
 
 
 class JobTimeoutError(Exception):
     def __init__(self, job_id, timeout):
         super().__init__(f"Burla job with id: '{job_id}' timed out after {timeout} seconds.")
@@ -46,58 +50,79 @@
             )
             sleep(2)
             return _get_job_info(job_id, epoch, headers, attempt=attempt + 1)
         else:
             raise e
 
 
+def start_job(function_: Callable, inputs: list, image: str, job_id: str, headers: dict):
+    function_pkl_hex = dill.dumps(function_).hex()
+    data = {"function_pkl_hex": function_pkl_hex, "inputs": inputs, "image": image}
+    response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}", json=data, headers=headers)
+    response.raise_for_status()
+
+
 def remote_parallel_map(
     function_: Callable,
     inputs: list,
-    cpus: int = 0,
+    image: Optional[str] = None,
+    api_key: Optional[str] = None,
+):
+    n_batches = math.ceil(len(inputs) / MAX_CONCURRENCY)
+    if len(inputs) > MAX_CONCURRENCY:
+        warnings.warn(
+            (
+                f"Because the current maximum concurrency is {MAX_CONCURRENCY} and you submitted "
+                f"{len(inputs)} inputs, these inputs will be processed in {n_batches} separate "
+                "batches. We are working hard to increase this concurrency limit."
+            )
+        )
+    outputs = []
+    input_batches = [
+        inputs[i : i + MAX_CONCURRENCY] for i in range(0, len(inputs), MAX_CONCURRENCY)
+    ]
+    for input_batch in input_batches:
+        outputs.extend(_remote_parallel_map(function_, input_batch, image, api_key))
+    return outputs
+
+
+def _remote_parallel_map(
+    function_: Callable,
+    inputs: list,
     image: Optional[str] = None,
     api_key: Optional[str] = None,
 ):
     if not function_.__annotations__.get("return") is str:
         raise AttributeError("Please add the return type annotation 'str' to your input function.")
 
-    if cpus > 100:
-        raise AttributeError("Currently unable to satisfy requests for > 100 computers")
-
     # https://www.rfc-editor.org/rfc/rfc7235 <- specifies "correct" api key location
     headers = {"Authorization": f"Bearer {api_key or load_api_key_from_local_config()}"}
 
     response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/", json={}, headers=headers)
     response.raise_for_status()
     job_id = response.json()["job_id"]
 
     user_python_version = f"{sys.version_info.major}.{sys.version_info.minor}"
     default_docker_image = f"{JOB_ENV_REPO}/python{user_python_version}/burla_job_env:latest"
+    image = image or default_docker_image  # sets image to default_docker_image if image is None
 
-    data = {
-        "function_pkl_hex": dill.dumps(function_.__code__).hex(),
-        "inputs": inputs,
-        "image": image or default_docker_image,
-        "num_computers": cpus,
-    }
+    # This is on a separate thread so we can print logs before all sub_jobs are running.
+    start_job_thread = Thread(target=start_job, args=(function_, inputs, image, job_id, headers))
     job_started_at_epoch = int(time())
-
-    # TODO: start this on separate thread so we can print logs before all subjobs are running.
-    response = requests.post(f"{BURLA_SERVICE_URL}/v1/jobs/{job_id}", json=data, headers=headers)
-    response.raise_for_status()
+    start_job_thread.start()
 
     last_epoch = job_started_at_epoch
     epoch = last_epoch
     job_is_running = True
     job_timed_out = False
 
     # Start printing logs generated by this job using a separate thread.
     print_queue = PriorityQueue()
-    stop_event = threading.Event()
-    log_thread = threading.Thread(target=print_logs_from_queue, args=(print_queue, stop_event))
+    stop_event = Event()
+    log_thread = Thread(target=print_logs_from_queue, args=(print_queue, stop_event))
     log_thread.start()
 
     # loop until job finishes, or times out
     while job_is_running and (not job_timed_out):
         # TODO: record and subtract time so this loop always takes exactly JOB_STATUS_POLL_RATE_SEC
         # sec to run? This might fix late logs?
         sleep(JOB_STATUS_POLL_RATE_SEC)
@@ -111,14 +136,15 @@
         last_epoch = epoch
         job_is_running = job["job_is_done"] == False
         job_failed = job.get("error") is not None
         job_timed_out = (time() - job_started_at_epoch) > (TIMEOUT_MIN * 60)
 
     stop_event.set()
     log_thread.join()
+    start_job_thread.join()
 
     if job_failed:
         error = pickle.loads(bytes.fromhex(job.get("error")))
         reraise(*error)
 
     if job_timed_out:
         raise JobTimeoutError(job_id=job_id, timeout=TIMEOUT_MIN)
```

### Comparing `burla-0.0.9/PKG-INFO` & `burla-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: burla
-Version: 0.0.9
+Version: 0.1.0
 Summary: Make your python script 100x faster
 Author: Jake Zuliani
 Author-email: jake@burla.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

