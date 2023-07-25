# Comparing `tmp/Signal8-5.0.3.tar.gz` & `tmp/Signal8-5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-5.0.3.tar", last modified: Tue Jul 25 22:18:39 2023, max compression
+gzip compressed data, was "Signal8-5.0.4.tar", last modified: Tue Jul 25 22:22:03 2023, max compression
```

## Comparing `Signal8-5.0.3.tar` & `Signal8-5.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 22:18:39.311872 Signal8-5.0.3/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-5.0.3/LICENSE
--rw-rw-rw-   0        0        0     5300 2023-07-25 22:18:39.305872 Signal8-5.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4800 2023-07-22 22:09:51.000000 Signal8-5.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 22:18:39.186872 Signal8-5.0.3/Signal8/
--rw-rw-rw-   0        0        0    10059 2023-07-25 21:45:17.000000 Signal8-5.0.3/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-5.0.3/Signal8/__init__.py
--rw-rw-rw-   0        0        0     3284 2023-07-25 22:16:09.000000 Signal8-5.0.3/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:18:39.299872 Signal8-5.0.3/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-5.0.3/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5299 2023-07-22 23:36:30.000000 Signal8-5.0.3/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2184 2023-07-25 21:45:38.000000 Signal8-5.0.3/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-5.0.3/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11976 2023-07-22 23:36:18.000000 Signal8-5.0.3/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-5.0.3/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:18:39.254870 Signal8-5.0.3/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5300 2023-07-25 22:18:38.000000 Signal8-5.0.3/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-25 22:18:38.000000 Signal8-5.0.3/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 22:18:38.000000 Signal8-5.0.3/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 22:18:38.000000 Signal8-5.0.3/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 22:18:39.312871 Signal8-5.0.3/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-07-25 22:17:12.000000 Signal8-5.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:22:03.533220 Signal8-5.0.4/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-5.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5300 2023-07-25 22:22:03.528215 Signal8-5.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4800 2023-07-22 22:09:51.000000 Signal8-5.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 22:22:03.409214 Signal8-5.0.4/Signal8/
+-rw-rw-rw-   0        0        0    10063 2023-07-25 22:21:34.000000 Signal8-5.0.4/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-5.0.4/Signal8/__init__.py
+-rw-rw-rw-   0        0        0     3284 2023-07-25 22:16:09.000000 Signal8-5.0.4/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:22:03.522213 Signal8-5.0.4/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-5.0.4/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5299 2023-07-22 23:36:30.000000 Signal8-5.0.4/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2184 2023-07-25 21:45:38.000000 Signal8-5.0.4/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-5.0.4/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11976 2023-07-22 23:36:18.000000 Signal8-5.0.4/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-5.0.4/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:22:03.439216 Signal8-5.0.4/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5300 2023-07-25 22:22:02.000000 Signal8-5.0.4/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-25 22:22:03.000000 Signal8-5.0.4/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 22:22:02.000000 Signal8-5.0.4/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 22:22:02.000000 Signal8-5.0.4/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 22:22:03.534216 Signal8-5.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-07-25 22:21:42.000000 Signal8-5.0.4/setup.py
```

### Comparing `Signal8-5.0.3/LICENSE` & `Signal8-5.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.3/PKG-INFO` & `Signal8-5.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 5.0.3
+Version: 5.0.4
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-5.0.3/README.md` & `Signal8-5.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.3/Signal8/Signal8.py` & `Signal8-5.0.4/Signal8/Signal8.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import matplotlib.path as mpath
 
 from functools import partial
-from utils.scenario import BaseScenario
-from utils.simple_env import SimpleEnv, make_env
-from utils.core import Agent, Goal, Obstacle, World
-from utils.problems import get_problem_list, get_problem_instance
+from .utils.scenario import BaseScenario
+from .utils.simple_env import SimpleEnv, make_env
+from .utils.core import Agent, Goal, Obstacle, World
+from .utils.problems import get_problem_list, get_problem_instance
 
 from gymnasium.utils import EzPickle
 
 
 class raw_env(SimpleEnv, EzPickle):
     def __init__(
         self,
```

### Comparing `Signal8-5.0.3/Signal8/main.py` & `Signal8-5.0.4/Signal8/main.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.3/Signal8/utils/core.py` & `Signal8-5.0.4/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.3/Signal8/utils/problems.py` & `Signal8-5.0.4/Signal8/utils/problems.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.3/Signal8/utils/simple_env.py` & `Signal8-5.0.4/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.3/Signal8/utils/test_dynamic_obs.py` & `Signal8-5.0.4/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.3/Signal8.egg-info/PKG-INFO` & `Signal8-5.0.4/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 5.0.3
+Version: 5.0.4
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-5.0.3/setup.py` & `Signal8-5.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="5.0.3",
+    version="5.0.4",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

