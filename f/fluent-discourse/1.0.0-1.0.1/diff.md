# Comparing `tmp/fluent-discourse-1.0.0.tar.gz` & `tmp/fluent-discourse-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluent-discourse-1.0.0.tar", last modified: Fri May 28 15:25:59 2021, max compression
+gzip compressed data, was "fluent-discourse-1.0.1.tar", last modified: Wed Jul 26 14:42:23 2023, max compression
```

## Comparing `fluent-discourse-1.0.0.tar` & `fluent-discourse-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 grayden    (501) staff       (20)        0 2021-05-28 15:25:59.083990 fluent-discourse-1.0.0/
--rw-r--r--   0 grayden    (501) staff       (20)     1056 2021-05-26 12:38:22.000000 fluent-discourse-1.0.0/LICENSE
--rw-r--r--   0 grayden    (501) staff       (20)     8206 2021-05-28 15:25:59.084143 fluent-discourse-1.0.0/PKG-INFO
--rw-r--r--   0 grayden    (501) staff       (20)     7627 2021-05-28 14:53:12.000000 fluent-discourse-1.0.0/README.md
--rw-r--r--   0 grayden    (501) staff       (20)      203 2021-05-26 16:32:49.000000 fluent-discourse-1.0.0/pyproject.toml
--rw-r--r--   0 grayden    (501) staff       (20)      695 2021-05-28 15:25:59.084730 fluent-discourse-1.0.0/setup.cfg
-drwxr-xr-x   0 grayden    (501) staff       (20)        0 2021-05-28 15:25:59.081562 fluent-discourse-1.0.0/src/
-drwxr-xr-x   0 grayden    (501) staff       (20)        0 2021-05-28 15:25:59.083144 fluent-discourse-1.0.0/src/fluent_discourse/
--rw-r--r--   0 grayden    (501) staff       (20)       55 2021-05-28 14:53:12.000000 fluent-discourse-1.0.0/src/fluent_discourse/__init__.py
--rw-r--r--   0 grayden    (501) staff       (20)     4682 2021-05-28 14:53:12.000000 fluent-discourse-1.0.0/src/fluent_discourse/discourse.py
--rw-r--r--   0 grayden    (501) staff       (20)      195 2021-05-28 14:53:12.000000 fluent-discourse-1.0.0/src/fluent_discourse/errors.py
-drwxr-xr-x   0 grayden    (501) staff       (20)        0 2021-05-28 15:25:59.083861 fluent-discourse-1.0.0/src/fluent_discourse.egg-info/
--rw-r--r--   0 grayden    (501) staff       (20)     8206 2021-05-28 15:25:59.000000 fluent-discourse-1.0.0/src/fluent_discourse.egg-info/PKG-INFO
--rw-r--r--   0 grayden    (501) staff       (20)      359 2021-05-28 15:25:59.000000 fluent-discourse-1.0.0/src/fluent_discourse.egg-info/SOURCES.txt
--rw-r--r--   0 grayden    (501) staff       (20)        1 2021-05-28 15:25:59.000000 fluent-discourse-1.0.0/src/fluent_discourse.egg-info/dependency_links.txt
--rw-r--r--   0 grayden    (501) staff       (20)        9 2021-05-28 15:25:59.000000 fluent-discourse-1.0.0/src/fluent_discourse.egg-info/requires.txt
--rw-r--r--   0 grayden    (501) staff       (20)       17 2021-05-28 15:25:59.000000 fluent-discourse-1.0.0/src/fluent_discourse.egg-info/top_level.txt
+drwxr-xr-x   0 gshand     (501) staff       (20)        0 2023-07-26 14:42:23.246446 fluent-discourse-1.0.1/
+-rw-r--r--   0 gshand     (501) staff       (20)     1056 2023-07-26 14:03:32.000000 fluent-discourse-1.0.1/LICENSE
+-rw-r--r--   0 gshand     (501) staff       (20)     8170 2023-07-26 14:42:23.246494 fluent-discourse-1.0.1/PKG-INFO
+-rw-r--r--   0 gshand     (501) staff       (20)     7627 2023-07-26 14:03:32.000000 fluent-discourse-1.0.1/README.md
+-rw-r--r--   0 gshand     (501) staff       (20)      203 2023-07-26 14:03:32.000000 fluent-discourse-1.0.1/pyproject.toml
+-rw-r--r--   0 gshand     (501) staff       (20)      695 2023-07-26 14:42:23.246736 fluent-discourse-1.0.1/setup.cfg
+drwxr-xr-x   0 gshand     (501) staff       (20)        0 2023-07-26 14:42:23.243951 fluent-discourse-1.0.1/src/
+drwxr-xr-x   0 gshand     (501) staff       (20)        0 2023-07-26 14:42:23.245625 fluent-discourse-1.0.1/src/fluent_discourse/
+-rw-r--r--   0 gshand     (501) staff       (20)       55 2023-07-26 14:03:32.000000 fluent-discourse-1.0.1/src/fluent_discourse/__init__.py
+-rw-r--r--   0 gshand     (501) staff       (20)     4557 2023-07-26 14:31:23.000000 fluent-discourse-1.0.1/src/fluent_discourse/discourse.py
+-rw-r--r--   0 gshand     (501) staff       (20)      195 2023-07-26 14:03:32.000000 fluent-discourse-1.0.1/src/fluent_discourse/errors.py
+drwxr-xr-x   0 gshand     (501) staff       (20)        0 2023-07-26 14:42:23.246343 fluent-discourse-1.0.1/src/fluent_discourse.egg-info/
+-rw-r--r--   0 gshand     (501) staff       (20)     8170 2023-07-26 14:42:23.000000 fluent-discourse-1.0.1/src/fluent_discourse.egg-info/PKG-INFO
+-rw-r--r--   0 gshand     (501) staff       (20)      359 2023-07-26 14:42:23.000000 fluent-discourse-1.0.1/src/fluent_discourse.egg-info/SOURCES.txt
+-rw-r--r--   0 gshand     (501) staff       (20)        1 2023-07-26 14:42:23.000000 fluent-discourse-1.0.1/src/fluent_discourse.egg-info/dependency_links.txt
+-rw-r--r--   0 gshand     (501) staff       (20)        9 2023-07-26 14:42:23.000000 fluent-discourse-1.0.1/src/fluent_discourse.egg-info/requires.txt
+-rw-r--r--   0 gshand     (501) staff       (20)       17 2023-07-26 14:42:23.000000 fluent-discourse-1.0.1/src/fluent_discourse.egg-info/top_level.txt
```

### Comparing `fluent-discourse-1.0.0/LICENSE` & `fluent-discourse-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fluent-discourse-1.0.0/PKG-INFO` & `fluent-discourse-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: fluent-discourse
-Version: 1.0.0
+Version: 1.0.1
 Summary: A fluent interface to the Discourse API
 Home-page: https://github.com/graydenshand/fluent_discourse
 Author: Grayden Shand
 Author-email: graydenshand@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/graydenshand/fluent_discourse/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -171,8 +169,7 @@
 black .
 ```
 
 ## Acknowledgements
 I stole the idea for a fluent API interface (and some code as a starting point) from SendGrid's Python API. [Here's a resouce that explains their approach](https://sendgrid.com/blog/using-python-to-implement-a-fluent-interface-to-any-rest-api/).
 
 There's a [Universal Client](https://universal-client.readthedocs.io/en/latest/) library that implements this framework as a flexible interface to ANY api. In contrast, this package is tailored specifically to Discourse's API including better error handling. 
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: fluent-discourse Version: 1.0.0 Summary: A fluent
+Metadata-Version: 2.1 Name: fluent-discourse Version: 1.0.1 Summary: A fluent
 interface to the Discourse API Home-page: https://github.com/graydenshand/
 fluent_discourse Author: Grayden Shand Author-email: graydenshand@gmail.com
-License: UNKNOWN Project-URL: Bug Tracker, https://github.com/graydenshand/
-fluent_discourse/issues Platform: UNKNOWN Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE # Fluent Discourse
+Project-URL: Bug Tracker, https://github.com/graydenshand/fluent_discourse/
+issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # Fluent Discourse
 [Build_and_test] [Code_Coverage]
 This package implements a [fluent interface](https://en.wikipedia.org/wiki/
 Fluent_interface) to the Discourse API. What does that mean? Instead of mapping
 every endpoint and method to a unique function, we present a framework for
 making any request. This means, with very little code, **this package is fully
 compatible with the Discourse API, including undocumented endpoints, endpoints
 from plugins, and endpoints that have yet to be created.** ## Installation The
```

### Comparing `fluent-discourse-1.0.0/README.md` & `fluent-discourse-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fluent-discourse-1.0.0/setup.cfg` & `fluent-discourse-1.0.1/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fluent-discourse
-version = 1.0.0
+version = 1.0.1
 author = Grayden Shand
 author_email = graydenshand@gmail.com
 description = A fluent interface to the Discourse API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/graydenshand/fluent_discourse
 project_urls =
```

### Comparing `fluent-discourse-1.0.0/src/fluent_discourse/discourse.py` & `fluent-discourse-1.0.1/src/fluent_discourse/discourse.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,14 @@
             except JSONDecodeError as e:
                 # Request succeeded but response body was not valid JSON
                 return r.text
         else:
             return self._handle_error(r, method, url, data, params)
 
     def _handle_error(self, response, method, url, data, params):
-        self._cache = []
         if response.status_code == 404:
             raise PageNotFoundError(
                 f"The requested page was not found, or you do not have permission to access it: {response.url}"
             )
         elif response.status_code == 403:
             raise UnauthorizedError("Invalid credentials")
         elif response.status_code == 429:
@@ -90,33 +89,29 @@
         # sleep for wait_seconds
         time.sleep(wait_seconds)
         return
 
     def get(self, data=None):
         # Make a get request
         url = self._make_url()
-        self._cache = []
         return self._request("GET", url, params=data)
 
     def post(self, data=None):
         # Make a post request
         url = self._make_url()
-        self._cache = []
         return self._request("POST", url, data=data)
 
     def put(self, data=None):
         # Make a put request
         url = self._make_url()
-        self._cache = []
         return self._request("PUT", url, data=data)
 
     def delete(self, data=None):
         # Make a delete request
         url = self._make_url()
-        self._cache = []
         return self._request("DELETE", url, data=data)
 
     def _make_url(self):
         # Build the request url from cache segments
         endpoint = "/".join(self._cache)
         # strip forward slash from e.g. '.json' or '.rss' segments if passed
         endpoint = endpoint.replace("/.", ".")
```

### Comparing `fluent-discourse-1.0.0/src/fluent_discourse.egg-info/PKG-INFO` & `fluent-discourse-1.0.1/src/fluent_discourse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: fluent-discourse
-Version: 1.0.0
+Version: 1.0.1
 Summary: A fluent interface to the Discourse API
 Home-page: https://github.com/graydenshand/fluent_discourse
 Author: Grayden Shand
 Author-email: graydenshand@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/graydenshand/fluent_discourse/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -171,8 +169,7 @@
 black .
 ```
 
 ## Acknowledgements
 I stole the idea for a fluent API interface (and some code as a starting point) from SendGrid's Python API. [Here's a resouce that explains their approach](https://sendgrid.com/blog/using-python-to-implement-a-fluent-interface-to-any-rest-api/).
 
 There's a [Universal Client](https://universal-client.readthedocs.io/en/latest/) library that implements this framework as a flexible interface to ANY api. In contrast, this package is tailored specifically to Discourse's API including better error handling. 
-
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: fluent-discourse Version: 1.0.0 Summary: A fluent
+Metadata-Version: 2.1 Name: fluent-discourse Version: 1.0.1 Summary: A fluent
 interface to the Discourse API Home-page: https://github.com/graydenshand/
 fluent_discourse Author: Grayden Shand Author-email: graydenshand@gmail.com
-License: UNKNOWN Project-URL: Bug Tracker, https://github.com/graydenshand/
-fluent_discourse/issues Platform: UNKNOWN Classifier: Programming Language ::
-Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
-Type: text/markdown License-File: LICENSE # Fluent Discourse
+Project-URL: Bug Tracker, https://github.com/graydenshand/fluent_discourse/
+issues Classifier: Programming Language :: Python :: 3 Classifier: License ::
+OSI Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # Fluent Discourse
 [Build_and_test] [Code_Coverage]
 This package implements a [fluent interface](https://en.wikipedia.org/wiki/
 Fluent_interface) to the Discourse API. What does that mean? Instead of mapping
 every endpoint and method to a unique function, we present a framework for
 making any request. This means, with very little code, **this package is fully
 compatible with the Discourse API, including undocumented endpoints, endpoints
 from plugins, and endpoints that have yet to be created.** ## Installation The
```

