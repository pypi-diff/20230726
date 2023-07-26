# Comparing `tmp/ABPandas-0.2.tar.gz` & `tmp/ABPandas-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ABPandas-0.2.tar", last modified: Wed Jul 26 18:22:50 2023, max compression
+gzip compressed data, was "ABPandas-0.3.tar", last modified: Wed Jul 26 18:35:27 2023, max compression
```

## Comparing `ABPandas-0.2.tar` & `ABPandas-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 18:22:50.829364 ABPandas-0.2/
-drwxrwxrwx   0        0        0        0 2023-07-26 18:22:50.800442 ABPandas-0.2/ABPandas/
--rw-rw-rw-   0        0        0       82 2023-07-26 15:55:36.000000 ABPandas-0.2/ABPandas/__init__.py
--rw-rw-rw-   0        0        0      739 2023-07-26 16:13:24.000000 ABPandas-0.2/ABPandas/agent.py
--rw-rw-rw-   0        0        0     6697 2023-07-26 15:52:50.000000 ABPandas-0.2/ABPandas/model.py
--rw-rw-rw-   0        0        0     1178 2023-07-26 15:50:02.000000 ABPandas-0.2/ABPandas/space.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:22:50.826372 ABPandas-0.2/ABPandas.egg-info/
--rw-rw-rw-   0        0        0      931 2023-07-26 18:22:49.000000 ABPandas-0.2/ABPandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2023-07-26 18:22:50.000000 ABPandas-0.2/ABPandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 18:22:50.000000 ABPandas-0.2/ABPandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-26 18:22:50.000000 ABPandas-0.2/ABPandas.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 18:22:50.000000 ABPandas-0.2/ABPandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      931 2023-07-26 18:22:50.828367 ABPandas-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-26 18:22:50.829364 ABPandas-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1464 2023-07-26 18:21:35.000000 ABPandas-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:35:27.711153 ABPandas-0.3/
+drwxrwxrwx   0        0        0        0 2023-07-26 18:35:27.690209 ABPandas-0.3/ABPandas/
+-rw-rw-rw-   0        0        0       85 2023-07-26 18:33:02.000000 ABPandas-0.3/ABPandas/__init__.py
+-rw-rw-rw-   0        0        0      739 2023-07-26 16:13:24.000000 ABPandas-0.3/ABPandas/agent.py
+-rw-rw-rw-   0        0        0     6698 2023-07-26 18:33:17.000000 ABPandas-0.3/ABPandas/model.py
+-rw-rw-rw-   0        0        0     1178 2023-07-26 15:50:02.000000 ABPandas-0.3/ABPandas/space.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:35:27.707164 ABPandas-0.3/ABPandas.egg-info/
+-rw-rw-rw-   0        0        0      931 2023-07-26 18:35:26.000000 ABPandas-0.3/ABPandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2023-07-26 18:35:27.000000 ABPandas-0.3/ABPandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:35:26.000000 ABPandas-0.3/ABPandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-26 18:35:27.000000 ABPandas-0.3/ABPandas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 18:35:27.000000 ABPandas-0.3/ABPandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      931 2023-07-26 18:35:27.709158 ABPandas-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-26 18:35:27.711153 ABPandas-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1464 2023-07-26 18:32:23.000000 ABPandas-0.3/setup.py
```

### Comparing `ABPandas-0.2/ABPandas/agent.py` & `ABPandas-0.3/ABPandas/agent.py`

 * *Files identical despite different names*

### Comparing `ABPandas-0.2/ABPandas/model.py` & `ABPandas-0.3/ABPandas/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from agent import Agent
+from .agent import Agent
 import geopandas as gpd
 import pandas as pd
 import fiona
 import copy
 
 class Model:
     def __init__ (self, space, agents= []):
```

### Comparing `ABPandas-0.2/ABPandas/space.py` & `ABPandas-0.3/ABPandas/space.py`

 * *Files identical despite different names*

### Comparing `ABPandas-0.2/ABPandas.egg-info/PKG-INFO` & `ABPandas-0.3/ABPandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABPandas
-Version: 0.2
+Version: 0.3
 Summary: Agent Based Pandas tool (ABPandas)
 Author: Yahya Gamal
 Author-email: <abpandas.yg@outlook.com>
 License: UNKNOWN
 Keywords: python,Agent Based Model,Spatial,Pandas
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ABPandas-0.2/PKG-INFO` & `ABPandas-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ABPandas
-Version: 0.2
+Version: 0.3
 Summary: Agent Based Pandas tool (ABPandas)
 Author: Yahya Gamal
 Author-email: <abpandas.yg@outlook.com>
 License: UNKNOWN
 Keywords: python,Agent Based Model,Spatial,Pandas
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ABPandas-0.2/setup.py` & `ABPandas-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2' 
+VERSION = '0.3' 
 DESCRIPTION = 'Agent Based Pandas tool (ABPandas)'
 LONG_DESCRIPTION = 'An Agent Based Modelling (ABM) package that can generate grid spatial shape files or work with predefined shape files.\nThe package focuses on simplicity by assigning Agents to spatial Polygons instead of assigning x and y locations for each agents.\nThis makes it useful in situations where granual movement of agents in space is not necessary (e.g. residentail location models)'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ABPandas",
```

