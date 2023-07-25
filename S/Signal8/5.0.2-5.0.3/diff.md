# Comparing `tmp/Signal8-5.0.2.tar.gz` & `tmp/Signal8-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Signal8-5.0.2.tar", last modified: Sun Jul 23 21:41:40 2023, max compression
+gzip compressed data, was "Signal8-5.0.3.tar", last modified: Tue Jul 25 22:18:39 2023, max compression
```

## Comparing `Signal8-5.0.2.tar` & `Signal8-5.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-23 21:41:40.097639 Signal8-5.0.2/
--rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-5.0.2/LICENSE
--rw-rw-rw-   0        0        0     5300 2023-07-23 21:41:40.094642 Signal8-5.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4800 2023-07-22 22:09:51.000000 Signal8-5.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-23 21:41:40.035640 Signal8-5.0.2/Signal8/
--rw-rw-rw-   0        0        0    11576 2023-07-23 21:39:18.000000 Signal8-5.0.2/Signal8/Signal8.py
--rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-5.0.2/Signal8/__init__.py
--rw-rw-rw-   0        0        0     3301 2023-07-23 21:38:25.000000 Signal8-5.0.2/Signal8/main.py
-drwxrwxrwx   0        0        0        0 2023-07-23 21:41:40.090639 Signal8-5.0.2/Signal8/utils/
--rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-5.0.2/Signal8/utils/__init__.py
--rw-rw-rw-   0        0        0     5299 2023-07-22 23:36:30.000000 Signal8-5.0.2/Signal8/utils/core.py
--rw-rw-rw-   0        0        0     2326 2023-07-23 00:27:30.000000 Signal8-5.0.2/Signal8/utils/problems.py
--rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-5.0.2/Signal8/utils/scenario.py
--rw-rw-rw-   0        0        0    11976 2023-07-22 23:36:18.000000 Signal8-5.0.2/Signal8/utils/simple_env.py
--rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-5.0.2/Signal8/utils/test_dynamic_obs.py
-drwxrwxrwx   0        0        0        0 2023-07-23 21:41:40.073638 Signal8-5.0.2/Signal8.egg-info/
--rw-rw-rw-   0        0        0     5300 2023-07-23 21:41:39.000000 Signal8-5.0.2/Signal8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      510 2023-07-23 21:41:39.000000 Signal8-5.0.2/Signal8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-23 21:41:39.000000 Signal8-5.0.2/Signal8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-23 21:41:39.000000 Signal8-5.0.2/Signal8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-23 21:41:40.097639 Signal8-5.0.2/setup.cfg
--rw-rw-rw-   0        0        0      647 2023-07-23 21:40:56.000000 Signal8-5.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:18:39.311872 Signal8-5.0.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-10 03:39:38.000000 Signal8-5.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5300 2023-07-25 22:18:39.305872 Signal8-5.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4800 2023-07-22 22:09:51.000000 Signal8-5.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 22:18:39.186872 Signal8-5.0.3/Signal8/
+-rw-rw-rw-   0        0        0    10059 2023-07-25 21:45:17.000000 Signal8-5.0.3/Signal8/Signal8.py
+-rw-rw-rw-   0        0        0       24 2023-06-19 21:16:46.000000 Signal8-5.0.3/Signal8/__init__.py
+-rw-rw-rw-   0        0        0     3284 2023-07-25 22:16:09.000000 Signal8-5.0.3/Signal8/main.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:18:39.299872 Signal8-5.0.3/Signal8/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-19 05:01:34.000000 Signal8-5.0.3/Signal8/utils/__init__.py
+-rw-rw-rw-   0        0        0     5299 2023-07-22 23:36:30.000000 Signal8-5.0.3/Signal8/utils/core.py
+-rw-rw-rw-   0        0        0     2184 2023-07-25 21:45:38.000000 Signal8-5.0.3/Signal8/utils/problems.py
+-rw-rw-rw-   0        0        0      292 2023-02-28 21:08:59.000000 Signal8-5.0.3/Signal8/utils/scenario.py
+-rw-rw-rw-   0        0        0    11976 2023-07-22 23:36:18.000000 Signal8-5.0.3/Signal8/utils/simple_env.py
+-rw-rw-rw-   0        0        0     1659 2023-06-08 18:48:20.000000 Signal8-5.0.3/Signal8/utils/test_dynamic_obs.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:18:39.254870 Signal8-5.0.3/Signal8.egg-info/
+-rw-rw-rw-   0        0        0     5300 2023-07-25 22:18:38.000000 Signal8-5.0.3/Signal8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      510 2023-07-25 22:18:38.000000 Signal8-5.0.3/Signal8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 22:18:38.000000 Signal8-5.0.3/Signal8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-25 22:18:38.000000 Signal8-5.0.3/Signal8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 22:18:39.312871 Signal8-5.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      647 2023-07-25 22:17:12.000000 Signal8-5.0.3/setup.py
```

### Comparing `Signal8-5.0.2/LICENSE` & `Signal8-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.2/PKG-INFO` & `Signal8-5.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 5.0.2
+Version: 5.0.3
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-5.0.2/README.md` & `Signal8-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.2/Signal8/Signal8.py` & `Signal8-5.0.3/Signal8/Signal8.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import matplotlib.path as mpath
 
 from functools import partial
-from .utils.scenario import BaseScenario
-from .utils.simple_env import SimpleEnv, make_env
-from .utils.core import Agent, Goal, Obstacle, World
-from .utils.problems import get_problem_list, get_problem_instance
+from utils.scenario import BaseScenario
+from utils.simple_env import SimpleEnv, make_env
+from utils.core import Agent, Goal, Obstacle, World
+from utils.problems import get_problem_list, get_problem_instance
 
 from gymnasium.utils import EzPickle
 
 
 class raw_env(SimpleEnv, EzPickle):
     def __init__(
         self, 
@@ -79,59 +79,43 @@
     # Generate valid points according to some condition
     def _generate_position(self, np_random, condition):
         while True:
             point = np_random.uniform(-1, +1, 2)
             if condition(point):
                 break
         return point
-
-    # Check if point is outside of triangular obstacle regions
-    def _outside_triangle(self, point, paths, epsilon):
-        enlarged_paths = []
-        for path in paths:
-            centroid = np.mean(path.vertices, axis=0)
-            # Make the triangle larger by moving each vertex away from the centroid by the `epsilon` distance
-            enlarged_vertices = centroid + (1 + epsilon) * (path.vertices - centroid) / np.linalg.norm(centroid - path.vertices)
-            enlarged_paths.append(mpath.Path(enlarged_vertices))
-        return not any(path.contains_points(point[None, :]) for path in enlarged_paths)
     
     # Check if point is outside of circular obstacle regions
     def _outside_circles(self, point, centers_radii, epsilon):
         return not any(np.linalg.norm(point - center) <= radius + epsilon for center, radius in centers_radii)
     
     # Check if point is outside of rectangular obstacle regions
     def _outside_rectangle(self, point, x_constraints, y_constraints, epsilon):
         within_constraints = any(
             (low_x - epsilon <= point[0] <= high_x + epsilon) and (low_y - epsilon <= point[1] <= high_y + epsilon)
             for (low_x, high_x), (low_y, high_y) in zip(x_constraints, y_constraints)
         )
         return not within_constraints
 
     # Reset agents and goals to their initial positions
-    def _reset_agents_and_goals(self, world, np_random, paths):
+    def _reset_agents_and_goals(self, world, np_random):
         epsilon = world.agents[0].radius
         
-        if world.problem_instance not in ['einstein_tile', 'corners', 'right_arrows', 'circle', 'solar_system']:
+        if world.problem_instance in ['bisect', 'cross', 'quarters']:
             # Used for problem instances composed of rectangles
             x_constraints = [constr[0] for constr in world.instance_constr]
             y_constraints = [constr[1] for constr in world.instance_constr]
 
         for i, agent in enumerate(world.agents):
             agent.goal = world.goals[i]
 
             agent.state.p_vel = np.zeros(world.dim_p)
             agent.goal.state.p_vel = np.zeros(world.dim_p)
 
-            if world.problem_instance in ['einstein_tile', 'corners', 'right_arrows']:
-                condition = partial(
-                    self._outside_triangle, 
-                    paths=paths, 
-                    epsilon=epsilon
-                    )
-            elif world.problem_instance in ['circle', 'solar_system']:
+            if world.problem_instance in ['circle', 'corners', 'scatter', 'stellaris']:
                 condition = partial(
                     self._outside_circles,
                     centers_radii=world.instance_constr,
                     epsilon=epsilon,
                     )
             else:
                 condition = partial(
@@ -163,45 +147,38 @@
                     occupied.clear()
                 
                 if shape_idx not in occupied:
                     large_obstacle.state.p_pos = pos
                     occupied.add(shape_idx)
                     break
     
-    def _reset_small_obstacles(self, world, np_random, paths):
+    def _reset_small_obstacles(self, world, np_random):
         epsilon = world.small_obstacles[0].radius
 
         agent_positions = [agent.state.p_pos for agent in world.agents]
         goal_positions = [goal.state.p_pos for goal in world.goals]
         large_obstacle_positions = [obstacle.state.p_pos for obstacle in world.large_obstacles]
 
         def safe_position(point):
             outside_entity_positions = not any(np.linalg.norm(point - pos) <= epsilon for pos in agent_positions + goal_positions + large_obstacle_positions)
 
-            if world.problem_instance in ['einstein_tile', 'corners', 'right_arrows']:
-                outside_obstacle_constraints = self._outside_triangle(point, paths, epsilon)
-            elif world.problem_instance in ['circle', 'solar_system']:
+            if world.problem_instance in ['circle', 'corners', 'scatter', 'stellaris']:
                 outside_obstacle_constraints = self._outside_circles(point, world.instance_constr, epsilon) 
             else:
                 x_constraints = [constr[0] for constr in world.instance_constr]
                 y_constraints = [constr[1] for constr in world.instance_constr]
                 outside_obstacle_constraints = self._outside_rectangle(point, x_constraints, y_constraints, epsilon)
 
             return outside_entity_positions and outside_obstacle_constraints
 
         for small_obstacle in world.small_obstacles:
             small_obstacle.state.p_vel = np.zeros(world.dim_p)
             small_obstacle.state.p_pos = self._generate_position(np_random, safe_position)
 
-    def reset_world(self, world, np_random, problem_instance):
-        def make_triangle_points(vertices, epsilon):
-            centroid = np.mean(vertices, axis=0)
-            shrunk_vertices = vertices + epsilon * (centroid - vertices)
-            return shrunk_vertices
-        
+    def reset_world(self, world, np_random, problem_instance):        
         def make_circle_points(center, radius_and_epsilon, num_points=100):
             t = np.linspace(0, 2*np.pi, num_points)
             x = center[0] + radius_and_epsilon * np.cos(t)
             y = center[1] + radius_and_epsilon * np.sin(t)
             points = np.column_stack([x, y])
             return points
         
@@ -214,24 +191,22 @@
                 (max_x - epsilon, max_y - epsilon),
                 (min_x + epsilon, max_y - epsilon),
             ]
 
         epsilon = world.large_obstacles[0].radius
         self._set_problem_instance(world, problem_instance)
         
-        if world.problem_instance in ['einstein_tile', 'corners', 'right_arrows']:
-            paths = [mpath.Path(make_triangle_points(vertices, epsilon)) for vertices in world.instance_constr]
-        elif world.problem_instance in ['circle', 'solar_system']:
+        if world.problem_instance in ['circle', 'corners', 'scatter', 'stellaris']:
             paths = [mpath.Path(make_circle_points(center, radius - epsilon)) for center, radius in world.instance_constr]
         else:
             paths = [mpath.Path(make_rectangle_points(bounds, epsilon)) for bounds in world.instance_constr]
 
+        self._reset_agents_and_goals(world, np_random)
         self._reset_large_obstacles(world, np_random, paths)
-        self._reset_agents_and_goals(world, np_random, paths)
-        self._reset_small_obstacles(world, np_random, paths)
+        self._reset_small_obstacles(world, np_random)
     
     # Ground agents can only observe the positions of other agents, goals, and small obstacles
     def observation(self, agent, world):
         agent_pos = agent.state.p_pos
         
         num_agents = len(world.agents)
         num_small_obstacles = len(world.small_obstacles)
```

### Comparing `Signal8-5.0.2/Signal8/main.py` & `Signal8-5.0.3/Signal8/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import time
 import signal8
 import numpy as np
 import matplotlib.pyplot as plt
 
 from itertools import product
 from shapely import Point, LineString, MultiLineString, Polygon
 
@@ -64,21 +65,20 @@
     boundary = lines.convex_hull
     polygons = boundary.difference(lines)
     regions = [polygons] if polygons.geom_type == 'Polygon' else list(polygons.geoms)
     return regions
 
 
 env = signal8.env()
-given_list =  [0.38, -1, 0.9, 0.38, -1, 0.275, 0.93, -1, -0.05, 0.93, -1, -0.8, -1, -0.474, -0.15, -1, -0.143, 0.8]
-problem_instance = 'right_arrows'
-test_coeffs(given_list)
+problem_instance = 'corners'
 
 agent_radius = env.unwrapped.world.agents[0].radius
 obstacle_radius = env.unwrapped.world.large_obstacles[0].radius
 
+start_time = time.time()
 for i in range(100):
     env.reset(options={'problem_instance': problem_instance})
     start_state = env.state()
     start = start_state[0:2]
     goal = start_state[2:4]
     obstacles = start_state[4:].reshape(-1, 2)
     
@@ -88,11 +88,14 @@
 
     for obstacle in obstacles_with_size:
         plt.fill(*obstacle.exterior.xy, alpha=0.5, color='red')
     
     plt.fill(*agent_with_size.exterior.xy, alpha=0.5, color='green')
     plt.fill(*goal_with_size.exterior.xy, alpha=0.5, color='green')
 
+end_time = time.time()
+print(f'Elapsed time: {end_time - start_time}')
+
 plt.xlim(-1, 1)
 plt.ylim(-1, 1)
-plt.show()
+plt.savefig('scatter.png')
 a=3
```

### Comparing `Signal8-5.0.2/Signal8/utils/core.py` & `Signal8-5.0.3/Signal8/utils/core.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.2/Signal8/utils/problems.py` & `Signal8-5.0.3/Signal8/utils/problems.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
     'bisect': [
         ((-1, -0), (-1, 1))
         ],
     'circle':  [
         ((0, 0), (0.5)),
         ],
     'corners': [
-        ((1, 1), (1, 0.65), (0.65, 1)),
-        ((1, -1), (1, -0.65), (0.65, -1)),
-        ((-1, -1), (-1, -0.65), (-0.65, -1)),
-        ((-1, 1), (-1, 0.65), (-0.65, 1)),
+        ((1, 1), (0.40)),
+        ((1, -1), (0.40)),
+        ((-1, -1), (0.40)),
+        ((-1, 1), (0.40)),
         ],
     'cross': [
         ((-0.1875, 0.1875), (0, 0.7)),
         ((-0.1875, 0.1875), (-0.7, 0)),
         ((-0.7, 0), (-0.1875, 0.1875)),
         ((0, 0.7), (-0.1875, 0.1875)),
         ],
@@ -38,27 +38,27 @@
         ],
     'quarters': [
         ((-1, -0.450), (-0.20, 0.20)),
         ((-0.20, 0.20), (0.450, 1)),
         ((0.450, 1), (-0.20, 0.20)),
         ((-0.20, 0.20), (-1, -0.450)),
         ],
-    'solar_system': [
+    'scatter': [
+        ((0.55, 0), (0.15)),
+        ((0.45, 0.70), (0.15)),
+        ((-0.60, 0.3), (0.15)),
+        ((-0.15, -0.65), (0.15)),
+        ],
+    'stellaris': [
         ((0.5, 0.5), (0.45)),
         ((-0.15, -0.675), (0.225)),
         ((-0.625, 0.175), (0.175)),
         ((-0.0375, 0), (0.1125)),
         ((-0.125, 0.475), (0.075)),
         ],
-    'right_arrows': [
-        ((0.4, 0.2), (0.4, -0.2), (0.7, 0)), 
-        ((0.3, 0.9), (0.3, 0.5), (0.6, 0.7)), 
-        ((-0.75, 0.5), (-0.75, 0.1), (-0.45, 0.3)), 
-        ((-0.3, -0.45), (-0.3, -0.85), (0, -0.65)),
-        ]
     }
 
 def get_problem_list():
     return list(problems.keys())
 
 def get_problem_instance(instance_name):
     instance_constr = problems[instance_name]
```

### Comparing `Signal8-5.0.2/Signal8/utils/simple_env.py` & `Signal8-5.0.3/Signal8/utils/simple_env.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.2/Signal8/utils/test_dynamic_obs.py` & `Signal8-5.0.3/Signal8/utils/test_dynamic_obs.py`

 * *Files identical despite different names*

### Comparing `Signal8-5.0.2/Signal8.egg-info/PKG-INFO` & `Signal8-5.0.3/Signal8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Signal8
-Version: 5.0.2
+Version: 5.0.3
 Summary: A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.
 Home-page: https://github.com/ethanmclark1/signal8
 Author: Ethan Clark
 Author-email: eclark715@gmail.com.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
```

### Comparing `Signal8-5.0.2/setup.py` & `Signal8-5.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="Signal8",
-    version="5.0.2",
+    version="5.0.3",
     packages=find_packages(),
     author="Ethan Clark",
     author_email="eclark715@gmail.com.com",
     description="A multi-agent environment inspired by the Lewis Signaling Game, featuring eight unique problem configurations with both static and dynamic obstacles.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/ethanmclark1/signal8",
```

