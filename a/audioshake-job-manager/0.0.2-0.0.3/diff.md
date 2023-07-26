# Comparing `tmp/audioshake_job_manager-0.0.2.tar.gz` & `tmp/audioshake_job_manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioshake_job_manager-0.0.2.tar", last modified: Wed Jul 26 07:45:11 2023, max compression
+gzip compressed data, was "audioshake_job_manager-0.0.3.tar", last modified: Wed Jul 26 17:41:57 2023, max compression
```

## Comparing `audioshake_job_manager-0.0.2.tar` & `audioshake_job_manager-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 07:45:11.996811 audioshake_job_manager-0.0.2/
--rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 07:45:11.996415 audioshake_job_manager-0.0.2/PKG-INFO
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 07:45:11.993764 audioshake_job_manager-0.0.2/audioshake_job_manager/
--rw-r--r--   0 theslyguy   (501) staff       (20)     3604 2023-07-26 07:41:12.000000 audioshake_job_manager-0.0.2/audioshake_job_manager/__init__.py
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 07:45:11.995962 audioshake_job_manager-0.0.2/audioshake_job_manager.egg-info/
--rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 07:45:11.000000 audioshake_job_manager-0.0.2/audioshake_job_manager.egg-info/PKG-INFO
--rw-r--r--   0 theslyguy   (501) staff       (20)      278 2023-07-26 07:45:11.000000 audioshake_job_manager-0.0.2/audioshake_job_manager.egg-info/SOURCES.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-26 07:45:11.000000 audioshake_job_manager-0.0.2/audioshake_job_manager.egg-info/dependency_links.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-26 07:45:11.000000 audioshake_job_manager-0.0.2/audioshake_job_manager.egg-info/requires.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)       23 2023-07-26 07:45:11.000000 audioshake_job_manager-0.0.2/audioshake_job_manager.egg-info/top_level.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)      395 2023-07-26 07:45:00.000000 audioshake_job_manager-0.0.2/pyproject.toml
--rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-26 07:45:11.996921 audioshake_job_manager-0.0.2/setup.cfg
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:41:57.360780 audioshake_job_manager-0.0.3/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 17:41:57.360395 audioshake_job_manager-0.0.3/PKG-INFO
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:41:57.358032 audioshake_job_manager-0.0.3/audioshake_job_manager/
+-rw-r--r--   0 theslyguy   (501) staff       (20)     3651 2023-07-26 08:00:02.000000 audioshake_job_manager-0.0.3/audioshake_job_manager/__init__.py
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 17:41:57.359986 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      179 2023-07-26 17:41:57.000000 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/PKG-INFO
+-rw-r--r--   0 theslyguy   (501) staff       (20)      278 2023-07-26 17:41:57.000000 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-26 17:41:57.000000 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-26 17:41:57.000000 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/requires.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)       23 2023-07-26 17:41:57.000000 audioshake_job_manager-0.0.3/audioshake_job_manager.egg-info/top_level.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)      395 2023-07-26 17:41:44.000000 audioshake_job_manager-0.0.3/pyproject.toml
+-rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-26 17:41:57.360880 audioshake_job_manager-0.0.3/setup.cfg
```

### Comparing `audioshake_job_manager-0.0.2/audioshake_job_manager/__init__.py` & `audioshake_job_manager-0.0.3/audioshake_job_manager/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 
         self._process_results(futures, cache)
 
     def _process_results(self, futures: list[Future], cache: dict = {}):
         for future in futures:
             try:
                 result = future.result(timeout=JOB_TIMEOUT)
+                # TODO: process batch results.
                 response = result[0] if isinstance(result, list) else result
                 logger.info("response: %s", response)
             except TimeoutError as exc:
                 error_message = "Future timed out"
                 response = {"success": False, "error": error_message}
                 logger.exception(error_message)
             except Exception as exc:
```

