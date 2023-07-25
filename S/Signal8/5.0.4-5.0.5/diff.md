# Comparing `tmp/Signal8-5.0.4.tar.gz` & `tmp/Signal8-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-5.0.4.tar", last modified: Tue Jul 25 22:22:03 2023, max compression
+gzip compressed data, was "Signal8-5.0.5.tar", last modified: Tue Jul 25 22:38:04 2023, max compression
```

## Comparing `Signal8-5.0.4.tar` & `Signal8-5.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 22:22:03.533220 Signal8-5.0.4/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-5.0.4/LICENSE
--rw-rw-rw-   0        0        0     5300 2023-07-25 22:22:03.528215 Signal8-5.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4800 2023-07-22 22:09:51.000000 Signal8-5.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 22:22:03.409214 Signal8-5.0.4/Signal8/
--rw-rw-rw-   0        0        0    10063 2023-07-25 22:21:34.000000 Signal8-5.0.4/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-5.0.4/Signal8/__init__.py
--rw-rw-rw-   0        0        0     3284 2023-07-25 22:16:09.000000 Signal8-5.0.4/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:22:03.522213 Signal8-5.0.4/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-5.0.4/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5299 2023-07-22 23:36:30.000000 Signal8-5.0.4/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2184 2023-07-25 21:45:38.000000 Signal8-5.0.4/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-5.0.4/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11976 2023-07-22 23:36:18.000000 Signal8-5.0.4/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-5.0.4/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:22:03.439216 Signal8-5.0.4/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5300 2023-07-25 22:22:02.000000 Signal8-5.0.4/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-25 22:22:03.000000 Signal8-5.0.4/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 22:22:02.000000 Signal8-5.0.4/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-25 22:22:02.000000 Signal8-5.0.4/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 22:22:03.534216 Signal8-5.0.4/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-07-25 22:21:42.000000 Signal8-5.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:38:04.857646 Signal8-5.0.5/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-5.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5300 2023-07-25 22:38:04.855641 Signal8-5.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4800 2023-07-22 22:09:51.000000 Signal8-5.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 22:38:04.762601 Signal8-5.0.5/Signal8/
+-rw-rw-rw-   0        0        0    10063 2023-07-25 22:37:39.000000 Signal8-5.0.5/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-5.0.5/Signal8/__init__.py
+-rw-rw-rw-   0        0        0     3288 2023-07-25 22:34:44.000000 Signal8-5.0.5/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:38:04.847641 Signal8-5.0.5/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-5.0.5/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5299 2023-07-22 23:36:30.000000 Signal8-5.0.5/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     1208 2023-07-25 22:36:49.000000 Signal8-5.0.5/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-5.0.5/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11976 2023-07-22 23:36:18.000000 Signal8-5.0.5/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-5.0.5/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:38:04.811641 Signal8-5.0.5/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5300 2023-07-25 22:38:04.000000 Signal8-5.0.5/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-25 22:38:04.000000 Signal8-5.0.5/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 22:38:04.000000 Signal8-5.0.5/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 22:38:04.000000 Signal8-5.0.5/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 22:38:04.858640 Signal8-5.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-07-25 22:36:55.000000 Signal8-5.0.5/setup.py
```

### Comparing `Signal8-5.0.4/LICENSE` & `Signal8-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.4/PKG-INFO` & `Signal8-5.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 5.0.4
+Version: 5.0.5
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-5.0.4/README.md` & `Signal8-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.4/Signal8/Signal8.py` & `Signal8-5.0.5/Signal8/Signal8.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.4/Signal8/main.py` & `Signal8-5.0.5/Signal8/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     boundary = lines.convex_hull
     polygons = boundary.difference(lines)
     regions = [polygons] if polygons.geom_type == 'Polygon' else list(polygons.geoms)
     return regions
 
 
 env = signal8.env()
-problem_instance = 'corners'
+problem_instance = 'stellaris'
 
 agent_radius = env.unwrapped.world.agents[0].radius
 obstacle_radius = env.unwrapped.world.large_obstacles[0].radius
 
 start_time = time.time()
 for i in range(100):
     env.reset(options={'problem_instance': problem_instance})
@@ -93,9 +93,9 @@
     plt.fill(*goal_with_size.exterior.xy, alpha=0.5, color='green')
 
 end_time = time.time()
 print(f'Elapsed time: {end_time - start_time}')
 
 plt.xlim(-1, 1)
 plt.ylim(-1, 1)
-plt.savefig('scatter.png')
+plt.savefig('stellaris.png')
 a=3
```

### Comparing `Signal8-5.0.4/Signal8/utils/core.py` & `Signal8-5.0.5/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.4/Signal8/utils/simple_env.py` & `Signal8-5.0.5/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.4/Signal8/utils/test_dynamic_obs.py` & `Signal8-5.0.5/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.4/Signal8.egg-info/PKG-INFO` & `Signal8-5.0.5/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 5.0.4
+Version: 5.0.5
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-5.0.4/setup.py` & `Signal8-5.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="5.0.4",
+    version="5.0.5",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

