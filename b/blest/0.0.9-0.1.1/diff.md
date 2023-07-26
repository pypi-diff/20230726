# Comparing `tmp/blest-0.0.9.tar.gz` & `tmp/blest-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blest-0.0.9.tar", last modified: Fri Jun 23 04:10:52 2023, max compression
+gzip compressed data, was "blest-0.1.1.tar", last modified: Wed Jul 26 18:34:00 2023, max compression
```

## Comparing `blest-0.0.9.tar` & `blest-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-23 04:10:52.524010 blest-0.0.9/
--rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 blest-0.0.9/LICENSE
--rw-r--r--   0 admin      (501) wheel        (0)     4125 2023-06-23 04:10:52.523430 blest-0.0.9/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)     3369 2023-06-23 01:13:48.000000 blest-0.0.9/README.md
--rw-r--r--   0 admin      (501) wheel        (0)        0 2023-06-23 04:09:47.000000 blest-0.0.9/__init__.py
-drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-06-23 04:10:52.522704 blest-0.0.9/blest.egg-info/
--rw-r--r--   0 admin      (501) wheel        (0)     4125 2023-06-23 04:10:52.000000 blest-0.0.9/blest.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) wheel        (0)      191 2023-06-23 04:10:52.000000 blest-0.0.9/blest.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-23 04:10:52.000000 blest-0.0.9/blest.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) wheel        (0)        8 2023-06-23 04:10:52.000000 blest-0.0.9/blest.egg-info/requires.txt
--rw-r--r--   0 admin      (501) wheel        (0)        1 2023-06-23 04:10:52.000000 blest-0.0.9/blest.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) wheel        (0)     8984 2023-06-23 04:09:55.000000 blest-0.0.9/blest.py
--rw-r--r--   0 admin      (501) wheel        (0)       38 2023-06-23 04:10:52.524147 blest-0.0.9/setup.cfg
--rw-r--r--   0 admin      (501) wheel        (0)     1014 2023-06-23 04:08:35.000000 blest-0.0.9/setup.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-07-26 18:34:00.608087 blest-0.1.1/
+-rw-r--r--   0 admin      (501) wheel        (0)     1061 2023-06-11 20:34:38.000000 blest-0.1.1/LICENSE
+-rw-r--r--   0 admin      (501) wheel        (0)     4631 2023-07-26 18:34:00.607722 blest-0.1.1/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)     3888 2023-07-26 18:32:30.000000 blest-0.1.1/README.md
+-rw-r--r--   0 admin      (501) wheel        (0)        0 2023-06-23 04:09:47.000000 blest-0.1.1/__init__.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-07-26 18:34:00.606889 blest-0.1.1/blest.egg-info/
+-rw-r--r--   0 admin      (501) wheel        (0)     4631 2023-07-26 18:34:00.000000 blest-0.1.1/blest.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) wheel        (0)      212 2023-07-26 18:34:00.000000 blest-0.1.1/blest.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-07-26 18:34:00.000000 blest-0.1.1/blest.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        8 2023-07-26 18:34:00.000000 blest-0.1.1/blest.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) wheel        (0)        1 2023-07-26 18:34:00.000000 blest-0.1.1/blest.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) wheel        (0)    21918 2023-07-26 18:28:44.000000 blest-0.1.1/blest.py
+-rw-r--r--   0 admin      (501) wheel        (0)       38 2023-07-26 18:34:00.608218 blest-0.1.1/setup.cfg
+-rw-r--r--   0 admin      (501) wheel        (0)     1001 2023-07-26 18:28:53.000000 blest-0.1.1/setup.py
+drwxr-xr-x   0 admin      (501) wheel        (0)        0 2023-07-26 18:34:00.607276 blest-0.1.1/tests/
+-rw-r--r--   0 admin      (501) wheel        (0)     8790 2023-07-26 18:27:14.000000 blest-0.1.1/tests/test_router.py
```

### Comparing `blest-0.0.9/LICENSE` & `blest-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blest-0.0.9/PKG-INFO` & `blest-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,14 @@
-Metadata-Version: 2.1
-Name: blest
-Version: 0.0.9
-Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST.
-Home-page: https://github.com/jhuntdev/blest-py
-Author: JHunt
-Author-email: blest@jhunt.dev
-Platform: any
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # BLEST Python
 
 The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST. It includes examples for Django, FastAPI, and Flask.
 
 To learn more about BLEST, please refer to the white paper: https://jhunt.dev/BLEST%20White%20Paper.pdf
 
-For a front-end implementation in React, please visit https://github.com/jhunt/blest-react
+For a front-end implementation in React, please visit https://github.com/jhuntdev/blest-react
 
 ## Features
 
 - Built on JSON - Reduce parsing time and overhead
 - Request Batching - Save bandwidth and reduce load times
 - Compact Payloads - Save more bandwidth
 - Selective Returns - Save even more bandwidth
@@ -38,15 +21,40 @@
 
 ```bash
 python3 -m pip install blest
 ```
 
 ## Usage
 
-Use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Use the `create_http_server` function to create a standalone HTTP server for your request handler. Use the `create_http_client` function to create a BLEST HTTP client.
+This default export of this library is an API very similar to Flask or FastAPI. For convenience it also provides a `create_request_handler` function to create a request handler suitable for use in an existing application, a `create_http_server` function to create a standalone HTTP server, and a `create_http_client` function to create a BLEST HTTP client.
+
+
+```python
+from blest import Blest
+
+app = new Blest({ 'timeout': 1000 })
+
+@app.before_request
+async def auth_middleware(params, context):
+  if params.get('name'):
+    context['user'] = {
+      'name': params['name']
+    }
+  else:
+    raise Exception('Unauthorized')
+
+@app.route('greet')
+async def greet_controller(params, context):
+  return {
+    'greeting': f"Hi, {context['user']['name']}!"
+  }
+
+if __name__ == '__main__':
+  app.listen(8080)
+```
 
 ### create_request_handler
 
 The following example uses Flask, but you can find examples with other frameworks [here](examples).
 
 ```python
 from flask import Flask, make_response, request
@@ -133,8 +141,8 @@
     # Do something with the result
   except Exception as error:
     # Do something in case of error
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `blest-0.0.9/README.md` & `blest-0.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,31 @@
+Metadata-Version: 2.1
+Name: blest
+Version: 0.1.1
+Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST.
+Home-page: https://blest.jhunt.dev
+Author: JHunt
+Author-email: blest@jhunt.dev
+Platform: any
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # BLEST Python
 
 The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST. It includes examples for Django, FastAPI, and Flask.
 
 To learn more about BLEST, please refer to the white paper: https://jhunt.dev/BLEST%20White%20Paper.pdf
 
-For a front-end implementation in React, please visit https://github.com/jhunt/blest-react
+For a front-end implementation in React, please visit https://github.com/jhuntdev/blest-react
 
 ## Features
 
 - Built on JSON - Reduce parsing time and overhead
 - Request Batching - Save bandwidth and reduce load times
 - Compact Payloads - Save more bandwidth
 - Selective Returns - Save even more bandwidth
@@ -21,15 +38,40 @@
 
 ```bash
 python3 -m pip install blest
 ```
 
 ## Usage
 
-Use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Use the `create_http_server` function to create a standalone HTTP server for your request handler. Use the `create_http_client` function to create a BLEST HTTP client.
+This default export of this library is an API very similar to Flask or FastAPI. For convenience it also provides a `create_request_handler` function to create a request handler suitable for use in an existing application, a `create_http_server` function to create a standalone HTTP server, and a `create_http_client` function to create a BLEST HTTP client.
+
+
+```python
+from blest import Blest
+
+app = new Blest({ 'timeout': 1000 })
+
+@app.before_request
+async def auth_middleware(params, context):
+  if params.get('name'):
+    context['user'] = {
+      'name': params['name']
+    }
+  else:
+    raise Exception('Unauthorized')
+
+@app.route('greet')
+async def greet_controller(params, context):
+  return {
+    'greeting': f"Hi, {context['user']['name']}!"
+  }
+
+if __name__ == '__main__':
+  app.listen(8080)
+```
 
 ### create_request_handler
 
 The following example uses Flask, but you can find examples with other frameworks [here](examples).
 
 ```python
 from flask import Flask, make_response, request
@@ -116,8 +158,8 @@
     # Do something with the result
   except Exception as error:
     # Do something in case of error
 ```
 
 ## License
 
-This project is licensed under the [MIT License](LICENSE).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `blest-0.0.9/blest.egg-info/PKG-INFO` & `blest-0.1.1/blest.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: blest
-Version: 0.0.9
+Version: 0.1.1
 Summary: The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST.
-Home-page: https://github.com/jhuntdev/blest-py
+Home-page: https://blest.jhunt.dev
 Author: JHunt
 Author-email: blest@jhunt.dev
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # BLEST Python
 
 The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST. It includes examples for Django, FastAPI, and Flask.
 
 To learn more about BLEST, please refer to the white paper: https://jhunt.dev/BLEST%20White%20Paper.pdf
 
-For a front-end implementation in React, please visit https://github.com/jhunt/blest-react
+For a front-end implementation in React, please visit https://github.com/jhuntdev/blest-react
 
 ## Features
 
 - Built on JSON - Reduce parsing time and overhead
 - Request Batching - Save bandwidth and reduce load times
 - Compact Payloads - Save more bandwidth
 - Selective Returns - Save even more bandwidth
@@ -38,15 +38,40 @@
 
 ```bash
 python3 -m pip install blest
 ```
 
 ## Usage
 
-Use the `create_request_handler` function to create a request handler suitable for use in an existing Python application. Use the `create_http_server` function to create a standalone HTTP server for your request handler. Use the `create_http_client` function to create a BLEST HTTP client.
+This default export of this library is an API very similar to Flask or FastAPI. For convenience it also provides a `create_request_handler` function to create a request handler suitable for use in an existing application, a `create_http_server` function to create a standalone HTTP server, and a `create_http_client` function to create a BLEST HTTP client.
+
+
+```python
+from blest import Blest
+
+app = new Blest({ 'timeout': 1000 })
+
+@app.before_request
+async def auth_middleware(params, context):
+  if params.get('name'):
+    context['user'] = {
+      'name': params['name']
+    }
+  else:
+    raise Exception('Unauthorized')
+
+@app.route('greet')
+async def greet_controller(params, context):
+  return {
+    'greeting': f"Hi, {context['user']['name']}!"
+  }
+
+if __name__ == '__main__':
+  app.listen(8080)
+```
 
 ### create_request_handler
 
 The following example uses Flask, but you can find examples with other frameworks [here](examples).
 
 ```python
 from flask import Flask, make_response, request
```

### Comparing `blest-0.0.9/setup.py` & `blest-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup
 
 with open("README.md", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="blest",
-    version="0.0.9",
+    version="0.1.1",
     author="JHunt",
     author_email="blest@jhunt.dev",
     description="The Python reference implementation of BLEST (Batch-able, Lightweight, Encrypted State Transfer), an improved communication protocol for web APIs which leverages JSON, supports request batching and selective returns, and provides a modern alternative to REST.",
     long_description=readme,
     long_description_content_type="text/markdown",
-    url="https://github.com/jhuntdev/blest-py",
+    url="https://blest.jhunt.dev",
     packages=["."],
     classifiers=[
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "aiohttp"
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     platforms="any",
 )
```

