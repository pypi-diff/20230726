# Comparing `tmp/readme-metrics-3.0.2.tar.gz` & `tmp/readme-metrics-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme-metrics-3.0.2.tar", last modified: Wed Jun 21 18:01:44 2023, max compression
+gzip compressed data, was "readme-metrics-3.0.3.tar", last modified: Wed Jul 26 11:59:23 2023, max compression
```

## Comparing `readme-metrics-3.0.2.tar` & `readme-metrics-3.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 erunion    (501) staff       (20)        0 2023-06-21 18:01:44.424920 readme-metrics-3.0.2/
--rw-r--r--   0 erunion    (501) staff       (20)      725 2022-08-10 16:07:18.000000 readme-metrics-3.0.2/LICENSE
--rw-r--r--   0 erunion    (501) staff       (20)     2414 2023-06-21 18:01:44.424797 readme-metrics-3.0.2/PKG-INFO
--rw-r--r--   0 erunion    (501) staff       (20)     2091 2022-12-16 18:11:05.000000 readme-metrics-3.0.2/README.md
-drwxr-xr-x   0 erunion    (501) staff       (20)        0 2023-06-21 18:01:44.424001 readme-metrics-3.0.2/readme_metrics/
--rw-r--r--   0 erunion    (501) staff       (20)     3856 2022-09-06 16:40:49.000000 readme-metrics-3.0.2/readme_metrics/Metrics.py
--rw-r--r--   0 erunion    (501) staff       (20)     5998 2022-09-06 16:40:49.000000 readme-metrics-3.0.2/readme_metrics/MetricsApiConfig.py
--rw-r--r--   0 erunion    (501) staff       (20)     4225 2022-08-31 22:56:37.000000 readme-metrics-3.0.2/readme_metrics/MetricsMiddleware.py
--rw-r--r--   0 erunion    (501) staff       (20)    14450 2023-06-21 17:52:53.000000 readme-metrics-3.0.2/readme_metrics/PayloadBuilder.py
--rw-r--r--   0 erunion    (501) staff       (20)     1246 2022-08-10 16:07:18.000000 readme-metrics-3.0.2/readme_metrics/ResponseInfoWrapper.py
--rw-r--r--   0 erunion    (501) staff       (20)     1178 2023-06-21 17:52:53.000000 readme-metrics-3.0.2/readme_metrics/VerifyWebhook.py
--rw-r--r--   0 erunion    (501) staff       (20)      147 2023-06-21 18:00:06.000000 readme-metrics-3.0.2/readme_metrics/__init__.py
--rw-r--r--   0 erunion    (501) staff       (20)     1868 2022-09-06 16:40:49.000000 readme-metrics-3.0.2/readme_metrics/django.py
--rw-r--r--   0 erunion    (501) staff       (20)     2021 2022-08-15 15:46:25.000000 readme-metrics-3.0.2/readme_metrics/flask_readme.py
--rw-r--r--   0 erunion    (501) staff       (20)     3681 2023-06-21 17:52:53.000000 readme-metrics-3.0.2/readme_metrics/publisher.py
--rw-r--r--   0 erunion    (501) staff       (20)      357 2022-09-03 06:58:47.000000 readme-metrics-3.0.2/readme_metrics/util.py
-drwxr-xr-x   0 erunion    (501) staff       (20)        0 2023-06-21 18:01:44.424645 readme-metrics-3.0.2/readme_metrics.egg-info/
--rw-r--r--   0 erunion    (501) staff       (20)     2414 2023-06-21 18:01:44.000000 readme-metrics-3.0.2/readme_metrics.egg-info/PKG-INFO
--rw-r--r--   0 erunion    (501) staff       (20)      549 2023-06-21 18:01:44.000000 readme-metrics-3.0.2/readme_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 erunion    (501) staff       (20)        1 2023-06-21 18:01:44.000000 readme-metrics-3.0.2/readme_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 erunion    (501) staff       (20)       50 2023-06-21 18:01:44.000000 readme-metrics-3.0.2/readme_metrics.egg-info/requires.txt
--rw-r--r--   0 erunion    (501) staff       (20)       15 2023-06-21 18:01:44.000000 readme-metrics-3.0.2/readme_metrics.egg-info/top_level.txt
--rw-r--r--   0 erunion    (501) staff       (20)       38 2023-06-21 18:01:44.424952 readme-metrics-3.0.2/setup.cfg
--rw-r--r--   0 erunion    (501) staff       (20)      650 2022-08-15 16:25:29.000000 readme-metrics-3.0.2/setup.py
+drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-07-26 11:59:23.093529 readme-metrics-3.0.3/
+-rw-r--r--   0 domh       (501) staff       (20)      725 2022-08-22 12:38:51.000000 readme-metrics-3.0.3/LICENSE
+-rw-r--r--   0 domh       (501) staff       (20)     2414 2023-07-26 11:59:23.093406 readme-metrics-3.0.3/PKG-INFO
+-rw-r--r--   0 domh       (501) staff       (20)     2091 2023-02-22 13:36:42.000000 readme-metrics-3.0.3/README.md
+drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-07-26 11:59:23.092496 readme-metrics-3.0.3/readme_metrics/
+-rw-r--r--   0 domh       (501) staff       (20)     3856 2022-09-06 16:49:05.000000 readme-metrics-3.0.3/readme_metrics/Metrics.py
+-rw-r--r--   0 domh       (501) staff       (20)     5998 2022-09-06 16:49:05.000000 readme-metrics-3.0.3/readme_metrics/MetricsApiConfig.py
+-rw-r--r--   0 domh       (501) staff       (20)     4225 2022-08-22 12:38:51.000000 readme-metrics-3.0.3/readme_metrics/MetricsMiddleware.py
+-rw-r--r--   0 domh       (501) staff       (20)    14450 2023-07-26 09:14:27.000000 readme-metrics-3.0.3/readme_metrics/PayloadBuilder.py
+-rw-r--r--   0 domh       (501) staff       (20)     1246 2022-04-13 15:12:08.000000 readme-metrics-3.0.3/readme_metrics/ResponseInfoWrapper.py
+-rw-r--r--   0 domh       (501) staff       (20)     1178 2023-07-26 09:14:27.000000 readme-metrics-3.0.3/readme_metrics/VerifyWebhook.py
+-rw-r--r--   0 domh       (501) staff       (20)      147 2023-07-26 11:58:25.000000 readme-metrics-3.0.3/readme_metrics/__init__.py
+-rw-r--r--   0 domh       (501) staff       (20)     1876 2023-07-26 11:56:45.000000 readme-metrics-3.0.3/readme_metrics/django.py
+-rw-r--r--   0 domh       (501) staff       (20)     2021 2022-08-24 14:21:21.000000 readme-metrics-3.0.3/readme_metrics/flask_readme.py
+-rw-r--r--   0 domh       (501) staff       (20)     3681 2023-07-26 09:14:27.000000 readme-metrics-3.0.3/readme_metrics/publisher.py
+-rw-r--r--   0 domh       (501) staff       (20)      357 2022-09-06 09:57:52.000000 readme-metrics-3.0.3/readme_metrics/util.py
+drwxr-xr-x   0 domh       (501) staff       (20)        0 2023-07-26 11:59:23.093205 readme-metrics-3.0.3/readme_metrics.egg-info/
+-rw-r--r--   0 domh       (501) staff       (20)     2414 2023-07-26 11:59:23.000000 readme-metrics-3.0.3/readme_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 domh       (501) staff       (20)      549 2023-07-26 11:59:23.000000 readme-metrics-3.0.3/readme_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 domh       (501) staff       (20)        1 2023-07-26 11:59:23.000000 readme-metrics-3.0.3/readme_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 domh       (501) staff       (20)       50 2023-07-26 11:59:23.000000 readme-metrics-3.0.3/readme_metrics.egg-info/requires.txt
+-rw-r--r--   0 domh       (501) staff       (20)       15 2023-07-26 11:59:23.000000 readme-metrics-3.0.3/readme_metrics.egg-info/top_level.txt
+-rw-r--r--   0 domh       (501) staff       (20)       38 2023-07-26 11:59:23.093571 readme-metrics-3.0.3/setup.cfg
+-rw-r--r--   0 domh       (501) staff       (20)      650 2022-08-22 12:38:51.000000 readme-metrics-3.0.3/setup.py
```

### Comparing `readme-metrics-3.0.2/LICENSE` & `readme-metrics-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/PKG-INFO` & `readme-metrics-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-metrics
-Version: 3.0.2
+Version: 3.0.3
 Summary: ReadMe API Metrics SDK
 Home-page: https://github.com/readmeio/metrics-sdks/tree/main/packages/python
 Author: ReadMe
 Author-email: support@readme.io
 Description-Content-Type: text/markdown
 Provides-Extra: Flask
 Provides-Extra: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: readme-metrics Version: 3.0.2 Summary: ReadMe API
+Metadata-Version: 2.1 Name: readme-metrics Version: 3.0.3 Summary: ReadMe API
 Metrics SDK Home-page: https://github.com/readmeio/metrics-sdks/tree/main/
 packages/python Author: ReadMe Author-email: support@readme.io Description-
 Content-Type: text/markdown Provides-Extra: Flask Provides-Extra: Django
 License-File: LICENSE # ReadMe Metrics
 [https://user-images.githubusercontent.com/33762/182927634-2aebeb46-c215-4ac3-
                             9e98-61f931e33583.png]
             Track usage of your API and troubleshoot issues faster.
```

### Comparing `readme-metrics-3.0.2/README.md` & `readme-metrics-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/readme_metrics/Metrics.py` & `readme-metrics-3.0.3/readme_metrics/Metrics.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/readme_metrics/MetricsApiConfig.py` & `readme-metrics-3.0.3/readme_metrics/MetricsApiConfig.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/readme_metrics/MetricsMiddleware.py` & `readme-metrics-3.0.3/readme_metrics/MetricsMiddleware.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/readme_metrics/PayloadBuilder.py` & `readme-metrics-3.0.3/readme_metrics/PayloadBuilder.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/readme_metrics/ResponseInfoWrapper.py` & `readme-metrics-3.0.3/readme_metrics/ResponseInfoWrapper.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/readme_metrics/VerifyWebhook.py` & `readme-metrics-3.0.3/readme_metrics/VerifyWebhook.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/readme_metrics/django.py` & `readme-metrics-3.0.3/readme_metrics/django.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,16 +15,16 @@
         assert isinstance(self.config, MetricsApiConfig)
         self.metrics_core = Metrics(self.config)
 
     def __call__(self, request):
         try:
             request.rm_start_dt = datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%SZ")
             request.rm_start_ts = int(time.time() * 1000)
-            if request.headers["Content-Length"] or request.body:
-                request.rm_content_length = request.headers["Content-Length"] or "0"
+            if request.headers.get("Content-Length") or request.body:
+                request.rm_content_length = request.headers.get("Content-Length") or "0"
                 request.rm_body = request.body or ""
         except Exception as e:
             # Errors in the Metrics SDK should never cause the application to
             # throw an error. Log it but don't re-raise.
             self.config.LOGGER.exception(e)
 
         response = self.get_response(request)
```

### Comparing `readme-metrics-3.0.2/readme_metrics/flask_readme.py` & `readme-metrics-3.0.3/readme_metrics/flask_readme.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/readme_metrics/publisher.py` & `readme-metrics-3.0.3/readme_metrics/publisher.py`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/readme_metrics.egg-info/PKG-INFO` & `readme-metrics-3.0.3/readme_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-metrics
-Version: 3.0.2
+Version: 3.0.3
 Summary: ReadMe API Metrics SDK
 Home-page: https://github.com/readmeio/metrics-sdks/tree/main/packages/python
 Author: ReadMe
 Author-email: support@readme.io
 Description-Content-Type: text/markdown
 Provides-Extra: Flask
 Provides-Extra: Django
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: readme-metrics Version: 3.0.2 Summary: ReadMe API
+Metadata-Version: 2.1 Name: readme-metrics Version: 3.0.3 Summary: ReadMe API
 Metrics SDK Home-page: https://github.com/readmeio/metrics-sdks/tree/main/
 packages/python Author: ReadMe Author-email: support@readme.io Description-
 Content-Type: text/markdown Provides-Extra: Flask Provides-Extra: Django
 License-File: LICENSE # ReadMe Metrics
 [https://user-images.githubusercontent.com/33762/182927634-2aebeb46-c215-4ac3-
                             9e98-61f931e33583.png]
             Track usage of your API and troubleshoot issues faster.
```

### Comparing `readme-metrics-3.0.2/readme_metrics.egg-info/SOURCES.txt` & `readme-metrics-3.0.3/readme_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `readme-metrics-3.0.2/setup.py` & `readme-metrics-3.0.3/setup.py`

 * *Files identical despite different names*

