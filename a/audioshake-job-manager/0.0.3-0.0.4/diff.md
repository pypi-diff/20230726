# Comparing `tmp/audioshake_job_manager-0.0.3.tar.gz` & `tmp/audioshake_job_manager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioshake_job_manager-0.0.3.tar", last modified: Wed Jul 26 17:41:57 2023, max compression
+gzip compressed data, was "audioshake_job_manager-0.0.4.tar", last modified: Wed Jul 26 17:55:22 2023, max compression
```

## Comparing `audioshake_job_manager-0.0.3.tar` & `audioshake_job_manager-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:41:57.360780 audioshake_job_manager-0.0.3/
--rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 17:41:57.360395 audioshake_job_manager-0.0.3/PKG-INFO
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:41:57.358032 audioshake_job_manager-0.0.3/audioshake_job_manager/
--rw-r--r--   0 theslyguy   (501) staff       (20)     3651 2023-07-26 08:00:02.000000 audioshake_job_manager-0.0.3/audioshake_job_manager/__init__.py
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:41:57.359986 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/
--rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 17:41:57.000000 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/PKG-INFO
--rw-r--r--   0 theslyguy   (501) staff       (20)      278 2023-07-26 17:41:57.000000 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/SOURCES.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-26 17:41:57.000000 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/dependency_links.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-26 17:41:57.000000 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/requires.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)       23 2023-07-26 17:41:57.000000 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/top_level.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)      395 2023-07-26 17:41:44.000000 audioshake_job_manager-0.0.3/pyproject.toml
--rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-26 17:41:57.360880 audioshake_job_manager-0.0.3/setup.cfg
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:55:22.605971 audioshake_job_manager-0.0.4/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 17:55:22.605543 audioshake_job_manager-0.0.4/PKG-INFO
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:55:22.602424 audioshake_job_manager-0.0.4/audioshake_job_manager/
+-rw-r--r--   0 theslyguy   (501) staff       (20)     3680 2023-07-26 17:54:58.000000 audioshake_job_manager-0.0.4/audioshake_job_manager/__init__.py
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:55:22.604960 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 17:55:22.000000 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/PKG-INFO
+-rw-r--r--   0 theslyguy   (501) staff       (20)      278 2023-07-26 17:55:22.000000 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-26 17:55:22.000000 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-26 17:55:22.000000 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/requires.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)       23 2023-07-26 17:55:22.000000 audioshake_job_manager-0.0.4/audioshake_job_manager.egg-info/top_level.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)      395 2023-07-26 17:55:11.000000 audioshake_job_manager-0.0.4/pyproject.toml
+-rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-26 17:55:22.606117 audioshake_job_manager-0.0.4/setup.cfg
```

### Comparing `audioshake_job_manager-0.0.3/audioshake_job_manager/__init__.py` & `audioshake_job_manager-0.0.4/audioshake_job_manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 
 logger = logging.getLogger(__name__)
 
 
 class JobManager:
     __metaclass__ = abc.ABCMeta
 
-    def __init__(self, queue_url: str, max_number_of_message: int = 10, batch: int = 1):
+    def __init__(
+        self, queue_url: str, max_number_of_message: int = 10, batch_size: int = 1
+    ):
         self.max_number_of_message = max_number_of_message
         self.queue_url = queue_url
         # NOTE to be used for batching messages read from the queue.
-        self.batch = batch
+        self.batch_size = batch_size
 
         self.sqs_client = boto3.client(
             "sqs", region_name=AWS_REGION, endpoint_url=AWS_ENDPOINT_URL
         )
         self.step_function_client = boto3.client(
             "stepfunctions", region_name=AWS_REGION, endpoint_url=AWS_ENDPOINT_URL
         )
```

