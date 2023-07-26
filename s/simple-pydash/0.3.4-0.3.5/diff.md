# Comparing `tmp/simple_pydash-0.3.4.tar.gz` & `tmp/simple_pydash-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_pydash-0.3.4.tar", last modified: Wed Jul 26 11:41:09 2023, max compression
+gzip compressed data, was "simple_pydash-0.3.5.tar", last modified: Wed Jul 26 11:44:41 2023, max compression
```

## Comparing `simple_pydash-0.3.4.tar` & `simple_pydash-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:41:09.975938 simple_pydash-0.3.4/
--rw-------   0 ft20308  (439624) psyc      (1340)    10423 2023-07-26 11:41:09.975938 simple_pydash-0.3.4/PKG-INFO
--rw-------   0 ft20308  (439624) psyc      (1340)    10108 2023-07-26 11:38:19.000000 simple_pydash-0.3.4/README.md
--rw-------   0 ft20308  (439624) psyc      (1340)       38 2023-07-26 11:41:09.975938 simple_pydash-0.3.4/setup.cfg
--rw-------   0 ft20308  (439624) psyc      (1340)      898 2023-07-26 11:40:57.000000 simple_pydash-0.3.4/setup.py
-drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:41:09.975938 simple_pydash-0.3.4/simple_pydash/
--rw-------   0 ft20308  (439624) psyc      (1340)      680 2023-07-25 14:04:10.000000 simple_pydash-0.3.4/simple_pydash/model.py
--rw-------   0 ft20308  (439624) psyc      (1340)     7042 2023-07-26 09:04:42.000000 simple_pydash-0.3.4/simple_pydash/server.py
-drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:41:09.975938 simple_pydash-0.3.4/simple_pydash.egg-info/
--rw-------   0 ft20308  (439624) psyc      (1340)    10423 2023-07-26 11:41:09.000000 simple_pydash-0.3.4/simple_pydash.egg-info/PKG-INFO
--rw-------   0 ft20308  (439624) psyc      (1340)      249 2023-07-26 11:41:09.000000 simple_pydash-0.3.4/simple_pydash.egg-info/SOURCES.txt
--rw-------   0 ft20308  (439624) psyc      (1340)        1 2023-07-26 11:41:09.000000 simple_pydash-0.3.4/simple_pydash.egg-info/dependency_links.txt
--rw-------   0 ft20308  (439624) psyc      (1340)       61 2023-07-26 11:41:09.000000 simple_pydash-0.3.4/simple_pydash.egg-info/requires.txt
--rw-------   0 ft20308  (439624) psyc      (1340)       14 2023-07-26 11:41:09.000000 simple_pydash-0.3.4/simple_pydash.egg-info/top_level.txt
+drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:44:41.673614 simple_pydash-0.3.5/
+-rw-------   0 ft20308  (439624) psyc      (1340)    10441 2023-07-26 11:44:41.673614 simple_pydash-0.3.5/PKG-INFO
+-rw-------   0 ft20308  (439624) psyc      (1340)    10126 2023-07-26 11:42:38.000000 simple_pydash-0.3.5/README.md
+-rw-------   0 ft20308  (439624) psyc      (1340)       38 2023-07-26 11:44:41.673614 simple_pydash-0.3.5/setup.cfg
+-rw-------   0 ft20308  (439624) psyc      (1340)      916 2023-07-26 11:44:21.000000 simple_pydash-0.3.5/setup.py
+drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:44:41.673614 simple_pydash-0.3.5/simple_pydash/
+-rw-------   0 ft20308  (439624) psyc      (1340)      680 2023-07-25 14:04:10.000000 simple_pydash-0.3.5/simple_pydash/model.py
+-rw-------   0 ft20308  (439624) psyc      (1340)     7042 2023-07-26 09:04:42.000000 simple_pydash-0.3.5/simple_pydash/server.py
+drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:44:41.673614 simple_pydash-0.3.5/simple_pydash.egg-info/
+-rw-------   0 ft20308  (439624) psyc      (1340)    10441 2023-07-26 11:44:41.000000 simple_pydash-0.3.5/simple_pydash.egg-info/PKG-INFO
+-rw-------   0 ft20308  (439624) psyc      (1340)      249 2023-07-26 11:44:41.000000 simple_pydash-0.3.5/simple_pydash.egg-info/SOURCES.txt
+-rw-------   0 ft20308  (439624) psyc      (1340)        1 2023-07-26 11:44:41.000000 simple_pydash-0.3.5/simple_pydash.egg-info/dependency_links.txt
+-rw-------   0 ft20308  (439624) psyc      (1340)       68 2023-07-26 11:44:41.000000 simple_pydash-0.3.5/simple_pydash.egg-info/requires.txt
+-rw-------   0 ft20308  (439624) psyc      (1340)       14 2023-07-26 11:44:41.000000 simple_pydash-0.3.5/simple_pydash.egg-info/top_level.txt
```

### Comparing `simple_pydash-0.3.4/PKG-INFO` & `simple_pydash-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_pydash
-Version: 0.3.4
+Version: 0.3.5
 Summary: Lightweight, modular Python library for creating real-time interactive dashboards in the web browser.
 Home-page: https://github.com/ValerioB88/simple-pydash
 Author: Valerio Biscione
 Author-email: valerio.biscione@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 Under the hood, SimplePyDash leverages the [FastAPI](https://fastapi.tiangolo.com/) web framework and uses [WebSocket](https://en.wikipedia.org/wiki/WebSocket) for bidirectional communication.
 
 ### Requirements
 Running 
 ```pip install simple-pydash```
 
 will install all the requirements. Otherwise you can do
-`pip install fastapi uvicorn[standard] numpy Pillow plotly sty`.
+`pip install fastapi uvicorn[standard] numpy Pillow plotly sty jinja2 matplotlib`.
 
 For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`: `
 pip install gym
 `
 
 
 ### Installation
```

### Comparing `simple_pydash-0.3.4/README.md` & `simple_pydash-0.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Under the hood, SimplePyDash leverages the [FastAPI](https://fastapi.tiangolo.com/) web framework and uses [WebSocket](https://en.wikipedia.org/wiki/WebSocket) for bidirectional communication.
 
 ### Requirements
 Running 
 ```pip install simple-pydash```
 
 will install all the requirements. Otherwise you can do
-`pip install fastapi uvicorn[standard] numpy Pillow plotly sty`.
+`pip install fastapi uvicorn[standard] numpy Pillow plotly sty jinja2 matplotlib`.
 
 For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`: `
 pip install gym
 `
 
 
 ### Installation
```

### Comparing `simple_pydash-0.3.4/setup.py` & `simple_pydash-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="simple_pydash",
-    version="0.3.4",
+    version="0.3.5",
     author="Valerio Biscione",
     author_email="valerio.biscione@gmail.com",
     description="Lightweight, modular Python library for creating real-time interactive dashboards in the web browser.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ValerioB88/simple-pydash",
     packages=["simple_pydash"],
@@ -18,14 +18,15 @@
         "fastapi",
         "uvicorn[standard]",
         "numpy",
         "Pillow",
         "plotly",
         "sty",
         "matplotlib",
+        "jinja2",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `simple_pydash-0.3.4/simple_pydash/model.py` & `simple_pydash-0.3.5/simple_pydash/model.py`

 * *Files identical despite different names*

### Comparing `simple_pydash-0.3.4/simple_pydash/server.py` & `simple_pydash-0.3.5/simple_pydash/server.py`

 * *Files identical despite different names*

### Comparing `simple_pydash-0.3.4/simple_pydash.egg-info/PKG-INFO` & `simple_pydash-0.3.5/simple_pydash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-pydash
-Version: 0.3.4
+Version: 0.3.5
 Summary: Lightweight, modular Python library for creating real-time interactive dashboards in the web browser.
 Home-page: https://github.com/ValerioB88/simple-pydash
 Author: Valerio Biscione
 Author-email: valerio.biscione@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,15 +21,15 @@
 Under the hood, SimplePyDash leverages the [FastAPI](https://fastapi.tiangolo.com/) web framework and uses [WebSocket](https://en.wikipedia.org/wiki/WebSocket) for bidirectional communication.
 
 ### Requirements
 Running 
 ```pip install simple-pydash```
 
 will install all the requirements. Otherwise you can do
-`pip install fastapi uvicorn[standard] numpy Pillow plotly sty`.
+`pip install fastapi uvicorn[standard] numpy Pillow plotly sty jinja2 matplotlib`.
 
 For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`: `
 pip install gym
 `
 
 
 ### Installation
```

