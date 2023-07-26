# Comparing `tmp/simple_pydash-0.3.0.tar.gz` & `tmp/simple_pydash-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_pydash-0.3.0.tar", last modified: Wed Jul 26 11:18:45 2023, max compression
+gzip compressed data, was "simple_pydash-0.3.1.tar", last modified: Wed Jul 26 11:29:02 2023, max compression
```

## Comparing `simple_pydash-0.3.0.tar` & `simple_pydash-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:18:45.176048 simple_pydash-0.3.0/
--rw-------   0 ft20308  (439624) psyc      (1340)    10263 2023-07-26 11:18:45.176048 simple_pydash-0.3.0/PKG-INFO
--rw-------   0 ft20308  (439624) psyc      (1340)     9942 2023-07-26 11:09:05.000000 simple_pydash-0.3.0/README.md
--rw-------   0 ft20308  (439624) psyc      (1340)       38 2023-07-26 11:18:45.176048 simple_pydash-0.3.0/setup.cfg
--rw-------   0 ft20308  (439624) psyc      (1340)      818 2023-07-26 11:17:39.000000 simple_pydash-0.3.0/setup.py
-drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:18:45.176048 simple_pydash-0.3.0/simple_pydash/
--rw-------   0 ft20308  (439624) psyc      (1340)      680 2023-07-25 14:04:10.000000 simple_pydash-0.3.0/simple_pydash/model.py
--rw-------   0 ft20308  (439624) psyc      (1340)     7042 2023-07-26 09:04:42.000000 simple_pydash-0.3.0/simple_pydash/server.py
-drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:18:45.176048 simple_pydash-0.3.0/simple_pydash.egg-info/
--rw-------   0 ft20308  (439624) psyc      (1340)    10263 2023-07-26 11:18:44.000000 simple_pydash-0.3.0/simple_pydash.egg-info/PKG-INFO
--rw-------   0 ft20308  (439624) psyc      (1340)      249 2023-07-26 11:18:45.000000 simple_pydash-0.3.0/simple_pydash.egg-info/SOURCES.txt
--rw-------   0 ft20308  (439624) psyc      (1340)        1 2023-07-26 11:18:44.000000 simple_pydash-0.3.0/simple_pydash.egg-info/dependency_links.txt
--rw-------   0 ft20308  (439624) psyc      (1340)       47 2023-07-26 11:18:44.000000 simple_pydash-0.3.0/simple_pydash.egg-info/requires.txt
--rw-------   0 ft20308  (439624) psyc      (1340)       14 2023-07-26 11:18:44.000000 simple_pydash-0.3.0/simple_pydash.egg-info/top_level.txt
+drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:29:02.000506 simple_pydash-0.3.1/
+-rw-------   0 ft20308  (439624) psyc      (1340)    10126 2023-07-26 11:29:02.000506 simple_pydash-0.3.1/PKG-INFO
+-rw-------   0 ft20308  (439624) psyc      (1340)     9805 2023-07-26 11:24:49.000000 simple_pydash-0.3.1/README.md
+-rw-------   0 ft20308  (439624) psyc      (1340)       38 2023-07-26 11:29:02.000506 simple_pydash-0.3.1/setup.cfg
+-rw-------   0 ft20308  (439624) psyc      (1340)      876 2023-07-26 11:22:19.000000 simple_pydash-0.3.1/setup.py
+drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:29:02.000506 simple_pydash-0.3.1/simple_pydash/
+-rw-------   0 ft20308  (439624) psyc      (1340)      680 2023-07-25 14:04:10.000000 simple_pydash-0.3.1/simple_pydash/model.py
+-rw-------   0 ft20308  (439624) psyc      (1340)     7042 2023-07-26 09:04:42.000000 simple_pydash-0.3.1/simple_pydash/server.py
+drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:29:02.000506 simple_pydash-0.3.1/simple_pydash.egg-info/
+-rw-------   0 ft20308  (439624) psyc      (1340)    10126 2023-07-26 11:29:01.000000 simple_pydash-0.3.1/simple_pydash.egg-info/PKG-INFO
+-rw-------   0 ft20308  (439624) psyc      (1340)      249 2023-07-26 11:29:01.000000 simple_pydash-0.3.1/simple_pydash.egg-info/SOURCES.txt
+-rw-------   0 ft20308  (439624) psyc      (1340)        1 2023-07-26 11:29:01.000000 simple_pydash-0.3.1/simple_pydash.egg-info/dependency_links.txt
+-rw-------   0 ft20308  (439624) psyc      (1340)       50 2023-07-26 11:29:01.000000 simple_pydash-0.3.1/simple_pydash.egg-info/requires.txt
+-rw-------   0 ft20308  (439624) psyc      (1340)       14 2023-07-26 11:29:01.000000 simple_pydash-0.3.1/simple_pydash.egg-info/top_level.txt
```

### Comparing `simple_pydash-0.3.0/PKG-INFO` & `simple_pydash-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_pydash
-Version: 0.3.0
+Version: 0.3.1
 Summary: Lightweight, modular Python library for creating real-time interactive dashboards in the web browser.
 Home-page: https://github.com/ValerioB88/simple-pydash
 Author: Valerio Biscione
 Author-email: valerio.biscione@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,24 +16,24 @@
 
 **SimplePyDash** is a versatile, browser-based dashboard designed for real-time data plotting. With a focus on simplicity, it allows Python developers to easily visualize data streams without complex setup or dependencies.
 
 Although originally developed to facilitate real-time plotting of OpenAI Gym environments for observing agent behavior, the versatility of SimplePyDash extends its utility beyond this use case, making it an excellent tool for many other data visualization scenarios.
 
 Under the hood, SimplePyDash leverages the [FastAPI](https://fastapi.tiangolo.com/) web framework and uses [WebSocket](https://en.wikipedia.org/wiki/WebSocket) for bidirectional communication.
 
-### Requirements:
-Use the following command to install necessary dependencies:
-```
-pip install fastapi "uvicorn[standard]"
-```
-For working with OpenAI Gym environments, install the `gym` library using the command:
+### Installation
+Run 
+`pip install simple-pydash`
+
+
+For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`:
 ```
 pip install gym
 ```
-Note: This library is only needed for running the `examples/openai_gym.py` example and is otherwise not mandatory.
+
 
 ### Installation
 To install SimplePyDash, you can _either_:
 
 - Install directly from the repository:
 ```
 pip install git+https://github.com/ValerioB88/browser-dashboard.git
```

### Comparing `simple_pydash-0.3.0/README.md` & `simple_pydash-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 **SimplePyDash** is a versatile, browser-based dashboard designed for real-time data plotting. With a focus on simplicity, it allows Python developers to easily visualize data streams without complex setup or dependencies.
 
 Although originally developed to facilitate real-time plotting of OpenAI Gym environments for observing agent behavior, the versatility of SimplePyDash extends its utility beyond this use case, making it an excellent tool for many other data visualization scenarios.
 
 Under the hood, SimplePyDash leverages the [FastAPI](https://fastapi.tiangolo.com/) web framework and uses [WebSocket](https://en.wikipedia.org/wiki/WebSocket) for bidirectional communication.
 
-### Requirements:
-Use the following command to install necessary dependencies:
-```
-pip install fastapi "uvicorn[standard]"
-```
-For working with OpenAI Gym environments, install the `gym` library using the command:
+### Installation
+Run 
+`pip install simple-pydash`
+
+
+For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`:
 ```
 pip install gym
 ```
-Note: This library is only needed for running the `examples/openai_gym.py` example and is otherwise not mandatory.
+
 
 ### Installation
 To install SimplePyDash, you can _either_:
 
 - Install directly from the repository:
 ```
 pip install git+https://github.com/ValerioB88/browser-dashboard.git
```

### Comparing `simple_pydash-0.3.0/simple_pydash/model.py` & `simple_pydash-0.3.1/simple_pydash/model.py`

 * *Files identical despite different names*

### Comparing `simple_pydash-0.3.0/simple_pydash/server.py` & `simple_pydash-0.3.1/simple_pydash/server.py`

 * *Files identical despite different names*

### Comparing `simple_pydash-0.3.0/simple_pydash.egg-info/PKG-INFO` & `simple_pydash-0.3.1/simple_pydash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-pydash
-Version: 0.3.0
+Version: 0.3.1
 Summary: Lightweight, modular Python library for creating real-time interactive dashboards in the web browser.
 Home-page: https://github.com/ValerioB88/simple-pydash
 Author: Valerio Biscione
 Author-email: valerio.biscione@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,24 +16,24 @@
 
 **SimplePyDash** is a versatile, browser-based dashboard designed for real-time data plotting. With a focus on simplicity, it allows Python developers to easily visualize data streams without complex setup or dependencies.
 
 Although originally developed to facilitate real-time plotting of OpenAI Gym environments for observing agent behavior, the versatility of SimplePyDash extends its utility beyond this use case, making it an excellent tool for many other data visualization scenarios.
 
 Under the hood, SimplePyDash leverages the [FastAPI](https://fastapi.tiangolo.com/) web framework and uses [WebSocket](https://en.wikipedia.org/wiki/WebSocket) for bidirectional communication.
 
-### Requirements:
-Use the following command to install necessary dependencies:
-```
-pip install fastapi "uvicorn[standard]"
-```
-For working with OpenAI Gym environments, install the `gym` library using the command:
+### Installation
+Run 
+`pip install simple-pydash`
+
+
+For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`:
 ```
 pip install gym
 ```
-Note: This library is only needed for running the `examples/openai_gym.py` example and is otherwise not mandatory.
+
 
 ### Installation
 To install SimplePyDash, you can _either_:
 
 - Install directly from the repository:
 ```
 pip install git+https://github.com/ValerioB88/browser-dashboard.git
```

