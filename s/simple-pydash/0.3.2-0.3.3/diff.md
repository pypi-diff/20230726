# Comparing `tmp/simple_pydash-0.3.2.tar.gz` & `tmp/simple_pydash-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_pydash-0.3.2.tar", last modified: Wed Jul 26 11:35:34 2023, max compression
+gzip compressed data, was "simple_pydash-0.3.3.tar", last modified: Wed Jul 26 11:38:37 2023, max compression
```

## Comparing `simple_pydash-0.3.2.tar` & `simple_pydash-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:35:34.178963 simple_pydash-0.3.2/
--rw-------   0 ft20308  (439624) psyc      (1340)    10355 2023-07-26 11:35:34.178963 simple_pydash-0.3.2/PKG-INFO
--rw-------   0 ft20308  (439624) psyc      (1340)    10039 2023-07-26 11:34:24.000000 simple_pydash-0.3.2/README.md
--rw-------   0 ft20308  (439624) psyc      (1340)       38 2023-07-26 11:35:34.178963 simple_pydash-0.3.2/setup.cfg
--rw-------   0 ft20308  (439624) psyc      (1340)      876 2023-07-26 11:35:03.000000 simple_pydash-0.3.2/setup.py
-drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:35:34.174963 simple_pydash-0.3.2/simple_pydash/
--rw-------   0 ft20308  (439624) psyc      (1340)      680 2023-07-25 14:04:10.000000 simple_pydash-0.3.2/simple_pydash/model.py
--rw-------   0 ft20308  (439624) psyc      (1340)     7042 2023-07-26 09:04:42.000000 simple_pydash-0.3.2/simple_pydash/server.py
-drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:35:34.178963 simple_pydash-0.3.2/simple_pydash.egg-info/
--rw-------   0 ft20308  (439624) psyc      (1340)    10355 2023-07-26 11:35:33.000000 simple_pydash-0.3.2/simple_pydash.egg-info/PKG-INFO
--rw-------   0 ft20308  (439624) psyc      (1340)      249 2023-07-26 11:35:34.000000 simple_pydash-0.3.2/simple_pydash.egg-info/SOURCES.txt
--rw-------   0 ft20308  (439624) psyc      (1340)        1 2023-07-26 11:35:33.000000 simple_pydash-0.3.2/simple_pydash.egg-info/dependency_links.txt
--rw-------   0 ft20308  (439624) psyc      (1340)       50 2023-07-26 11:35:33.000000 simple_pydash-0.3.2/simple_pydash.egg-info/requires.txt
--rw-------   0 ft20308  (439624) psyc      (1340)       14 2023-07-26 11:35:34.000000 simple_pydash-0.3.2/simple_pydash.egg-info/top_level.txt
+drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:38:37.795858 simple_pydash-0.3.3/
+-rw-------   0 ft20308  (439624) psyc      (1340)    10423 2023-07-26 11:38:37.795858 simple_pydash-0.3.3/PKG-INFO
+-rw-------   0 ft20308  (439624) psyc      (1340)    10108 2023-07-26 11:38:19.000000 simple_pydash-0.3.3/README.md
+-rw-------   0 ft20308  (439624) psyc      (1340)       38 2023-07-26 11:38:37.795858 simple_pydash-0.3.3/setup.cfg
+-rw-------   0 ft20308  (439624) psyc      (1340)      876 2023-07-26 11:38:29.000000 simple_pydash-0.3.3/setup.py
+drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:38:37.795858 simple_pydash-0.3.3/simple_pydash/
+-rw-------   0 ft20308  (439624) psyc      (1340)      680 2023-07-25 14:04:10.000000 simple_pydash-0.3.3/simple_pydash/model.py
+-rw-------   0 ft20308  (439624) psyc      (1340)     7042 2023-07-26 09:04:42.000000 simple_pydash-0.3.3/simple_pydash/server.py
+drwx------   0 ft20308  (439624) psyc      (1340)        0 2023-07-26 11:38:37.795858 simple_pydash-0.3.3/simple_pydash.egg-info/
+-rw-------   0 ft20308  (439624) psyc      (1340)    10423 2023-07-26 11:38:37.000000 simple_pydash-0.3.3/simple_pydash.egg-info/PKG-INFO
+-rw-------   0 ft20308  (439624) psyc      (1340)      249 2023-07-26 11:38:37.000000 simple_pydash-0.3.3/simple_pydash.egg-info/SOURCES.txt
+-rw-------   0 ft20308  (439624) psyc      (1340)        1 2023-07-26 11:38:37.000000 simple_pydash-0.3.3/simple_pydash.egg-info/dependency_links.txt
+-rw-------   0 ft20308  (439624) psyc      (1340)       50 2023-07-26 11:38:37.000000 simple_pydash-0.3.3/simple_pydash.egg-info/requires.txt
+-rw-------   0 ft20308  (439624) psyc      (1340)       14 2023-07-26 11:38:37.000000 simple_pydash-0.3.3/simple_pydash.egg-info/top_level.txt
```

### Comparing `simple_pydash-0.3.2/PKG-INFO` & `simple_pydash-0.3.3/simple_pydash.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simple_pydash
-Version: 0.3.2
+Name: simple-pydash
+Version: 0.3.3
 Summary: Lightweight, modular Python library for creating real-time interactive dashboards in the web browser.
 Home-page: https://github.com/ValerioB88/simple-pydash
 Author: Valerio Biscione
 Author-email: valerio.biscione@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,23 +17,23 @@
 **SimplePyDash** is a versatile, browser-based dashboard designed for real-time data plotting. With a focus on simplicity, it allows Python developers to easily visualize data streams without complex setup or dependencies.
 
 Although originally developed to facilitate real-time plotting of OpenAI Gym environments for observing agent behavior, the versatility of SimplePyDash extends its utility beyond this use case, making it an excellent tool for many other data visualization scenarios.
 
 Under the hood, SimplePyDash leverages the [FastAPI](https://fastapi.tiangolo.com/) web framework and uses [WebSocket](https://en.wikipedia.org/wiki/WebSocket) for bidirectional communication.
 
 ### Requirements
-Running
-`pip install simple-pydash`
+Running 
+```pip install simple-pydash```
+
 will install all the requirements. Otherwise you can do
 `pip install fastapi uvicorn[standard] numpy Pillow plotly sty`.
 
-For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`:
-```
+For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`: `
 pip install gym
-```
+`
 
 
 ### Installation
 To install SimplePyDash, you can _either_:
 
 - Install directly from the repository:
 ```
@@ -42,16 +42,17 @@
 **OR**
 - Clone/fork the repository, and install in editable mode (recommended if you plan to modify the code):
 ```
 pip install -e {path_to_cloned_folder}
 ```
 
 **OR**
-`pip install simple-pydash`
-(this won't include the examples, which you can download from GitHub)
+from PyPl:
+```pip install simple-pydash```
+(this won't include the examples, which you can download from GitHub).
 
 ### Examples 
 The best way to get started is to explore the examples provided. `examples/openai_gym.py` demonstrates plotting a gym environment (requires the `gym` library), while `examples/generic.py` is a more general use case.
 
 To run an example, navigate to the repository folder and execute the Python module:
 ```
 cd {path_to_repo_folder}
@@ -70,15 +71,15 @@
 Then, open your browser and visit `localhost:8000` to view the dashboard.
 
 ## Quick Start 
 SimplePyDash organizes your dashboard into columns (2 by default). The `CustomAPI` object takes a `model_obj` and a series of `DashboardComponents`. The user-defined `model_obj` is a simple iterator performing the computations (e.g., running a neural network and returning an action). `DashboardComponents` are widgets that can be displayed in the browser.
 
 SimplePyDash includes several default widgets, including `HeatMap`, `LinePlot`, `StaticImage`, `TextInfo`, and `RenderGymEnv`. The `plot` widgets, such as `HeatMap` and `LinePlot`, are based on the [Plotly](https://plotly.com/python/) graphics library, allowing for easy addition of Plotly graphs to your widget list.
 
-Here's a basic example of a `CustomAPI` object:
+Here's a basic instance of a `CustomAPI` object (see `examples/generic.py` for the full example):
 ```python
 server = CustomAPI(
     model_obj=DummyModel,
     dash_comps=[
         GeneralTextInfo(location_col_idx=0, use_scroll=False),
         MatplotlibPlot(location_col_idx=0, width=500),
         AppendScatterPlot(
```

### Comparing `simple_pydash-0.3.2/README.md` & `simple_pydash-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 **SimplePyDash** is a versatile, browser-based dashboard designed for real-time data plotting. With a focus on simplicity, it allows Python developers to easily visualize data streams without complex setup or dependencies.
 
 Although originally developed to facilitate real-time plotting of OpenAI Gym environments for observing agent behavior, the versatility of SimplePyDash extends its utility beyond this use case, making it an excellent tool for many other data visualization scenarios.
 
 Under the hood, SimplePyDash leverages the [FastAPI](https://fastapi.tiangolo.com/) web framework and uses [WebSocket](https://en.wikipedia.org/wiki/WebSocket) for bidirectional communication.
 
 ### Requirements
-Running
-`pip install simple-pydash`
+Running 
+```pip install simple-pydash```
+
 will install all the requirements. Otherwise you can do
 `pip install fastapi uvicorn[standard] numpy Pillow plotly sty`.
 
-For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`:
-```
+For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`: `
 pip install gym
-```
+`
 
 
 ### Installation
 To install SimplePyDash, you can _either_:
 
 - Install directly from the repository:
 ```
@@ -30,16 +30,17 @@
 **OR**
 - Clone/fork the repository, and install in editable mode (recommended if you plan to modify the code):
 ```
 pip install -e {path_to_cloned_folder}
 ```
 
 **OR**
-`pip install simple-pydash`
-(this won't include the examples, which you can download from GitHub)
+from PyPl:
+```pip install simple-pydash```
+(this won't include the examples, which you can download from GitHub).
 
 ### Examples 
 The best way to get started is to explore the examples provided. `examples/openai_gym.py` demonstrates plotting a gym environment (requires the `gym` library), while `examples/generic.py` is a more general use case.
 
 To run an example, navigate to the repository folder and execute the Python module:
 ```
 cd {path_to_repo_folder}
@@ -58,15 +59,15 @@
 Then, open your browser and visit `localhost:8000` to view the dashboard.
 
 ## Quick Start 
 SimplePyDash organizes your dashboard into columns (2 by default). The `CustomAPI` object takes a `model_obj` and a series of `DashboardComponents`. The user-defined `model_obj` is a simple iterator performing the computations (e.g., running a neural network and returning an action). `DashboardComponents` are widgets that can be displayed in the browser.
 
 SimplePyDash includes several default widgets, including `HeatMap`, `LinePlot`, `StaticImage`, `TextInfo`, and `RenderGymEnv`. The `plot` widgets, such as `HeatMap` and `LinePlot`, are based on the [Plotly](https://plotly.com/python/) graphics library, allowing for easy addition of Plotly graphs to your widget list.
 
-Here's a basic example of a `CustomAPI` object:
+Here's a basic instance of a `CustomAPI` object (see `examples/generic.py` for the full example):
 ```python
 server = CustomAPI(
     model_obj=DummyModel,
     dash_comps=[
         GeneralTextInfo(location_col_idx=0, use_scroll=False),
         MatplotlibPlot(location_col_idx=0, width=500),
         AppendScatterPlot(
```

### Comparing `simple_pydash-0.3.2/setup.py` & `simple_pydash-0.3.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="simple_pydash",
-    version="0.3.2",
+    version="0.3.3",
     author="Valerio Biscione",
     author_email="valerio.biscione@gmail.com",
     description="Lightweight, modular Python library for creating real-time interactive dashboards in the web browser.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ValerioB88/simple-pydash",
     packages=["simple_pydash"],
```

### Comparing `simple_pydash-0.3.2/simple_pydash/model.py` & `simple_pydash-0.3.3/simple_pydash/model.py`

 * *Files identical despite different names*

### Comparing `simple_pydash-0.3.2/simple_pydash/server.py` & `simple_pydash-0.3.3/simple_pydash/server.py`

 * *Files identical despite different names*

### Comparing `simple_pydash-0.3.2/simple_pydash.egg-info/PKG-INFO` & `simple_pydash-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: simple-pydash
-Version: 0.3.2
+Name: simple_pydash
+Version: 0.3.3
 Summary: Lightweight, modular Python library for creating real-time interactive dashboards in the web browser.
 Home-page: https://github.com/ValerioB88/simple-pydash
 Author: Valerio Biscione
 Author-email: valerio.biscione@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,23 +17,23 @@
 **SimplePyDash** is a versatile, browser-based dashboard designed for real-time data plotting. With a focus on simplicity, it allows Python developers to easily visualize data streams without complex setup or dependencies.
 
 Although originally developed to facilitate real-time plotting of OpenAI Gym environments for observing agent behavior, the versatility of SimplePyDash extends its utility beyond this use case, making it an excellent tool for many other data visualization scenarios.
 
 Under the hood, SimplePyDash leverages the [FastAPI](https://fastapi.tiangolo.com/) web framework and uses [WebSocket](https://en.wikipedia.org/wiki/WebSocket) for bidirectional communication.
 
 ### Requirements
-Running
-`pip install simple-pydash`
+Running 
+```pip install simple-pydash```
+
 will install all the requirements. Otherwise you can do
 `pip install fastapi uvicorn[standard] numpy Pillow plotly sty`.
 
-For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`:
-```
+For running the OpenAI Gym example, you additionally need to have  the `gym` library. This is not a requirement for using `simple-pydash`: `
 pip install gym
-```
+`
 
 
 ### Installation
 To install SimplePyDash, you can _either_:
 
 - Install directly from the repository:
 ```
@@ -42,16 +42,17 @@
 **OR**
 - Clone/fork the repository, and install in editable mode (recommended if you plan to modify the code):
 ```
 pip install -e {path_to_cloned_folder}
 ```
 
 **OR**
-`pip install simple-pydash`
-(this won't include the examples, which you can download from GitHub)
+from PyPl:
+```pip install simple-pydash```
+(this won't include the examples, which you can download from GitHub).
 
 ### Examples 
 The best way to get started is to explore the examples provided. `examples/openai_gym.py` demonstrates plotting a gym environment (requires the `gym` library), while `examples/generic.py` is a more general use case.
 
 To run an example, navigate to the repository folder and execute the Python module:
 ```
 cd {path_to_repo_folder}
@@ -70,15 +71,15 @@
 Then, open your browser and visit `localhost:8000` to view the dashboard.
 
 ## Quick Start 
 SimplePyDash organizes your dashboard into columns (2 by default). The `CustomAPI` object takes a `model_obj` and a series of `DashboardComponents`. The user-defined `model_obj` is a simple iterator performing the computations (e.g., running a neural network and returning an action). `DashboardComponents` are widgets that can be displayed in the browser.
 
 SimplePyDash includes several default widgets, including `HeatMap`, `LinePlot`, `StaticImage`, `TextInfo`, and `RenderGymEnv`. The `plot` widgets, such as `HeatMap` and `LinePlot`, are based on the [Plotly](https://plotly.com/python/) graphics library, allowing for easy addition of Plotly graphs to your widget list.
 
-Here's a basic example of a `CustomAPI` object:
+Here's a basic instance of a `CustomAPI` object (see `examples/generic.py` for the full example):
 ```python
 server = CustomAPI(
     model_obj=DummyModel,
     dash_comps=[
         GeneralTextInfo(location_col_idx=0, use_scroll=False),
         MatplotlibPlot(location_col_idx=0, width=500),
         AppendScatterPlot(
```

