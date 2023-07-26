# Comparing `tmp/scrapy-puppeteer-client-0.1.0.tar.gz` & `tmp/scrapy-puppeteer-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-puppeteer-client-0.1.0.tar", last modified: Wed Jul 26 10:30:28 2023, max compression
+gzip compressed data, was "scrapy-puppeteer-client-0.1.1.tar", last modified: Wed Jul 26 12:01:36 2023, max compression
```

## Comparing `scrapy-puppeteer-client-0.1.0.tar` & `scrapy-puppeteer-client-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:30:28.087444 scrapy-puppeteer-client-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-26 10:30:16.000000 scrapy-puppeteer-client-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-26 10:30:28.087444 scrapy-puppeteer-client-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-26 10:30:16.000000 scrapy-puppeteer-client-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:30:28.087444 scrapy-puppeteer-client-0.1.0/scrapy_puppeteer_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-07-26 10:30:28.000000 scrapy-puppeteer-client-0.1.0/scrapy_puppeteer_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-26 10:30:28.000000 scrapy-puppeteer-client-0.1.0/scrapy_puppeteer_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:30:28.000000 scrapy-puppeteer-client-0.1.0/scrapy_puppeteer_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 10:30:28.000000 scrapy-puppeteer-client-0.1.0/scrapy_puppeteer_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:30:28.087444 scrapy-puppeteer-client-0.1.0/scrapypuppeteer/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 10:30:16.000000 scrapy-puppeteer-client-0.1.0/scrapypuppeteer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-26 10:30:16.000000 scrapy-puppeteer-client-0.1.0/scrapypuppeteer/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12779 2023-07-26 10:30:16.000000 scrapy-puppeteer-client-0.1.0/scrapypuppeteer/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-26 10:30:16.000000 scrapy-puppeteer-client-0.1.0/scrapypuppeteer/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-26 10:30:16.000000 scrapy-puppeteer-client-0.1.0/scrapypuppeteer/response.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 10:30:28.087444 scrapy-puppeteer-client-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 10:30:16.000000 scrapy-puppeteer-client-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:01:36.158429 scrapy-puppeteer-client-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-26 12:01:22.000000 scrapy-puppeteer-client-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-07-26 12:01:36.158429 scrapy-puppeteer-client-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-07-26 12:01:22.000000 scrapy-puppeteer-client-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:01:36.154429 scrapy-puppeteer-client-0.1.1/scrapy_puppeteer_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6206 2023-07-26 12:01:36.000000 scrapy-puppeteer-client-0.1.1/scrapy_puppeteer_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-26 12:01:36.000000 scrapy-puppeteer-client-0.1.1/scrapy_puppeteer_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:01:36.000000 scrapy-puppeteer-client-0.1.1/scrapy_puppeteer_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 12:01:36.000000 scrapy-puppeteer-client-0.1.1/scrapy_puppeteer_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:01:36.158429 scrapy-puppeteer-client-0.1.1/scrapypuppeteer/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 12:01:22.000000 scrapy-puppeteer-client-0.1.1/scrapypuppeteer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9365 2023-07-26 12:01:22.000000 scrapy-puppeteer-client-0.1.1/scrapypuppeteer/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-07-26 12:01:22.000000 scrapy-puppeteer-client-0.1.1/scrapypuppeteer/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-26 12:01:22.000000 scrapy-puppeteer-client-0.1.1/scrapypuppeteer/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-26 12:01:22.000000 scrapy-puppeteer-client-0.1.1/scrapypuppeteer/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:01:36.158429 scrapy-puppeteer-client-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-26 12:01:22.000000 scrapy-puppeteer-client-0.1.1/setup.py
```

### Comparing `scrapy-puppeteer-client-0.1.0/LICENSE` & `scrapy-puppeteer-client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.1.0/PKG-INFO` & `scrapy-puppeteer-client-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: scrapy-puppeteer-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to use Puppeteer-managed browser in Scrapy spiders
 Home-page: https://github.com/ispras/scrapy-puppeteer
 Author: MODIS @ ISP RAS
 Maintainer: Maksim Varlamov
 Maintainer-email: varlamov@ispras.ru
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Scrapy
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires: scrapy
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `scrapy-puppeteer-client-0.1.0/README.md` & `scrapy-puppeteer-client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.1.0/scrapy_puppeteer_client.egg-info/PKG-INFO` & `scrapy-puppeteer-client-0.1.1/scrapy_puppeteer_client.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: scrapy-puppeteer-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to use Puppeteer-managed browser in Scrapy spiders
 Home-page: https://github.com/ispras/scrapy-puppeteer
 Author: MODIS @ ISP RAS
 Maintainer: Maksim Varlamov
 Maintainer-email: varlamov@ispras.ru
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Scrapy
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires: scrapy
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `scrapy-puppeteer-client-0.1.0/scrapypuppeteer/actions.py` & `scrapy-puppeteer-client-0.1.1/scrapypuppeteer/actions.py`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.1.0/scrapypuppeteer/middleware.py` & `scrapy-puppeteer-client-0.1.1/scrapypuppeteer/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import logging
 from collections import defaultdict
 from typing import List, Union
-from urllib.parse import urljoin, urlencode
+from urllib.parse import urlencode, urljoin
 
 from scrapy import Request, signals
 from scrapy.crawler import Crawler
 from scrapy.exceptions import IgnoreRequest, NotConfigured
 from scrapy.http import Headers, TextResponse
 
-from scrapypuppeteer import PuppeteerRequest, PuppeteerHtmlResponse, PuppeteerResponse
-from scrapypuppeteer.actions import Screenshot, RecaptchaSolver, Click
+from scrapypuppeteer import PuppeteerHtmlResponse, PuppeteerRequest, PuppeteerResponse
+from scrapypuppeteer.actions import Click, GoBack, GoForward, GoTo, RecaptchaSolver, Screenshot, Scroll
 from scrapypuppeteer.response import PuppeteerJsonResponse, PuppeteerScreenshotResponse
 
 
 class PuppeteerServiceDownloaderMiddleware:
     """
     This downloader middleware converts PuppeteerRequest instances to
     Puppeteer service API requests and then converts its responses to
@@ -132,32 +132,32 @@
         if b'application/json' not in response.headers.get(b'Content-Type', b''):
             return response
 
         response_data = json.loads(response.text)
         context_id = response_data.pop('contextId', None)
         page_id = response_data.pop('pageId', None)
 
-        response_cls = self._get_response_class(puppeteer_request.action, response_data)
+        response_cls = self._get_response_class(puppeteer_request.action)
         response = response_cls(
             url=puppeteer_request.url,
             puppeteer_request=puppeteer_request,
             context_id=context_id,
             page_id=page_id,
             **response_data
         )
 
         self.used_contexts[id(spider)].add(context_id)
 
         return response
 
     @staticmethod
-    def _get_response_class(request_action, response_data):
-        if 'html' in response_data and 'recaptcha_data' not in response_data:
+    def _get_response_class(request_action):
+        if isinstance(request_action, (GoTo, GoForward, GoBack, Click, Scroll)):
             return PuppeteerHtmlResponse
-        if 'screenshot' in response_data and isinstance(request_action, Screenshot):
+        if isinstance(request_action, Screenshot):
             return PuppeteerScreenshotResponse
         return PuppeteerJsonResponse
 
     def close_used_contexts(self, spider):
         contexts = list(self.used_contexts[id(spider)])
         if contexts:
             request = Request(urljoin(self.service_base_url, '/close_context'),
```

### Comparing `scrapy-puppeteer-client-0.1.0/scrapypuppeteer/request.py` & `scrapy-puppeteer-client-0.1.1/scrapypuppeteer/request.py`

 * *Files identical despite different names*

### Comparing `scrapy-puppeteer-client-0.1.0/scrapypuppeteer/response.py` & `scrapy-puppeteer-client-0.1.1/scrapypuppeteer/response.py`

 * *Files identical despite different names*

