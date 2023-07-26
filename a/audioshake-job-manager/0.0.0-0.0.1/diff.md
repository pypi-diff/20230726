# Comparing `tmp/audioshake_job_manager-0.0.0.tar.gz` & `tmp/audioshake_job_manager-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioshake_job_manager-0.0.0.tar", last modified: Wed Jul 26 06:43:44 2023, max compression
+gzip compressed data, was "audioshake_job_manager-0.0.1.tar", last modified: Wed Jul 26 07:14:15 2023, max compression
```

## Comparing `audioshake_job_manager-0.0.0.tar` & `audioshake_job_manager-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 06:43:44.598674 audioshake_job_manager-0.0.0/
--rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 06:43:44.598177 audioshake_job_manager-0.0.0/PKG-INFO
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 06:43:44.595596 audioshake_job_manager-0.0.0/audioshake_job_manager/
--rw-r--r--   0 theslyguy   (501) staff       (20)     3412 2023-07-26 06:38:41.000000 audioshake_job_manager-0.0.0/audioshake_job_manager/__init__.py
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 06:43:44.597572 audioshake_job_manager-0.0.0/audioshake_job_manager.egg-info/
--rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 06:43:44.000000 audioshake_job_manager-0.0.0/audioshake_job_manager.egg-info/PKG-INFO
--rw-r--r--   0 theslyguy   (501) staff       (20)      278 2023-07-26 06:43:44.000000 audioshake_job_manager-0.0.0/audioshake_job_manager.egg-info/SOURCES.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-26 06:43:44.000000 audioshake_job_manager-0.0.0/audioshake_job_manager.egg-info/dependency_links.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-26 06:43:44.000000 audioshake_job_manager-0.0.0/audioshake_job_manager.egg-info/requires.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)       23 2023-07-26 06:43:44.000000 audioshake_job_manager-0.0.0/audioshake_job_manager.egg-info/top_level.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)      395 2023-07-26 06:43:32.000000 audioshake_job_manager-0.0.0/pyproject.toml
--rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-26 06:43:44.598829 audioshake_job_manager-0.0.0/setup.cfg
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 07:14:15.255952 audioshake_job_manager-0.0.1/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 07:14:15.255547 audioshake_job_manager-0.0.1/PKG-INFO
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 07:14:15.252754 audioshake_job_manager-0.0.1/audioshake_job_manager/
+-rw-r--r--   0 theslyguy   (501) staff       (20)     3570 2023-07-26 07:13:26.000000 audioshake_job_manager-0.0.1/audioshake_job_manager/__init__.py
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 07:14:15.255085 audioshake_job_manager-0.0.1/audioshake_job_manager.egg-info/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 07:14:15.000000 audioshake_job_manager-0.0.1/audioshake_job_manager.egg-info/PKG-INFO
+-rw-r--r--   0 theslyguy   (501) staff       (20)      278 2023-07-26 07:14:15.000000 audioshake_job_manager-0.0.1/audioshake_job_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-26 07:14:15.000000 audioshake_job_manager-0.0.1/audioshake_job_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-26 07:14:15.000000 audioshake_job_manager-0.0.1/audioshake_job_manager.egg-info/requires.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)       23 2023-07-26 07:14:15.000000 audioshake_job_manager-0.0.1/audioshake_job_manager.egg-info/top_level.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)      395 2023-07-26 07:08:02.000000 audioshake_job_manager-0.0.1/pyproject.toml
+-rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-26 07:14:15.256121 audioshake_job_manager-0.0.1/setup.cfg
```

### Comparing `audioshake_job_manager-0.0.0/audioshake_job_manager/__init__.py` & `audioshake_job_manager-0.0.1/audioshake_job_manager/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,19 +13,18 @@
 
 logger = logging.getLogger(__name__)
 
 
 class JobManager:
     __metaclass__ = abc.ABCMeta
 
-    def __init__(
-        self, queue_url: str, max_number_of_message: int = 10, batch: bool = False
-    ):
+    def __init__(self, queue_url: str, max_number_of_message: int = 10, batch: int = 1):
         self.max_number_of_message = max_number_of_message
         self.queue_url = queue_url
+        # NOTE to be used for batching messages read from the queue.
         self.batch = batch
 
         self.sqs_client = boto3.client(
             "sqs", region_name=AWS_REGION, endpoint_url=AWS_ENDPOINT_URL
         )
         self.step_function_client = boto3.client(
             "stepfunctions", region_name=AWS_REGION, endpoint_url=AWS_ENDPOINT_URL
@@ -71,18 +70,21 @@
             future = self.process(json.dumps(payload))
             futures.append(future)
             cache[future._id] = {
                 "job_id": job["ReceiptHandle"],
                 "task_token": task_token,
             }
 
+        self._process_results(futures, cache)
+
+    def _process_results(self, futures: list[Future], cache: dict = {}):
         for future in futures:
             try:
-                result = future.result(timeout=JOB_TIMEOUT)
-                response = {"success": True, **result}
+                results = future.result(timeout=JOB_TIMEOUT)
+                response = {**results[0]}
                 logger.info("response: %s", response)
             except TimeoutError as exc:
                 error_message = "Future timed out"
                 response = {"success": False, "error": error_message}
                 logger.exception(error_message)
             except Exception as exc:
                 error_message = f"Unknown error occured. {exc}"
```

