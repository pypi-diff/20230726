# Comparing `tmp/craft2d-0.1.5.tar.gz` & `tmp/craft2d-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft2d-0.1.5.tar", max compression
+gzip compressed data, was "craft2d-0.1.6.tar", max compression
```

## Comparing `craft2d-0.1.5.tar` & `craft2d-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      488 2023-07-12 15:58:14.885516 craft2d-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-07-09 12:33:35.821513 craft2d-0.1.5/craft2d/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:38:39.479663 craft2d-0.1.5/craft2d/config/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 18:38:45.164798 craft2d-0.1.5/craft2d/env/__init__.py
--rw-r--r--   0        0        0    16585 2023-07-24 17:56:17.165502 craft2d-0.1.5/craft2d/env/environment.py
--rw-r--r--   0        0        0        0 2023-07-10 20:04:09.256648 craft2d-0.1.5/craft2d/render/__init__.py
--rw-r--r--   0        0        0    10299 2023-07-13 13:10:10.586272 craft2d-0.1.5/craft2d/render/render.py
--rw-r--r--   0        0        0     2193 2023-07-09 20:09:51.278818 craft2d-0.1.5/craft2d/resources/agent/agent-down.png
--rw-r--r--   0        0        0     2111 2023-07-09 20:09:25.442353 craft2d-0.1.5/craft2d/resources/agent/agent-left.png
--rw-r--r--   0        0        0     2153 2023-07-09 20:09:37.887138 craft2d-0.1.5/craft2d/resources/agent/agent-right.png
--rw-r--r--   0        0        0     2103 2023-07-09 20:09:11.258794 craft2d-0.1.5/craft2d/resources/agent/agent-up.png
--rw-r--r--   0        0        0     1797 2023-07-09 20:14:01.501432 craft2d-0.1.5/craft2d/resources/farm/plant-large.png
--rw-r--r--   0        0        0     1219 2023-07-09 20:13:45.609907 craft2d-0.1.5/craft2d/resources/farm/plant-medium.png
--rw-r--r--   0        0        0     1000 2023-07-09 20:13:26.261484 craft2d-0.1.5/craft2d/resources/farm/plant-small.png
--rw-r--r--   0        0        0     1074 2023-07-09 20:15:44.310385 craft2d-0.1.5/craft2d/resources/objects/bridge.png
--rw-r--r--   0        0        0     3400 2023-07-09 20:30:59.755816 craft2d-0.1.5/craft2d/resources/objects/crafting-table.png
--rw-r--r--   0        0        0     5133 2023-07-10 19:33:45.377024 craft2d-0.1.5/craft2d/resources/objects/gem.png
--rw-r--r--   0        0        0     1007 2023-07-09 20:29:41.393116 craft2d-0.1.5/craft2d/resources/objects/grass.png
--rw-r--r--   0        0        0     3826 2023-07-13 13:05:51.408981 craft2d-0.1.5/craft2d/resources/objects/princess.png
--rw-r--r--   0        0        0     3178 2023-07-10 16:32:23.402820 craft2d-0.1.5/craft2d/resources/objects/rope.png
--rw-r--r--   0        0        0     3823 2023-07-10 16:31:28.142800 craft2d-0.1.5/craft2d/resources/objects/sticks.png
--rw-r--r--   0        0        0     1364 2023-07-09 20:14:47.718624 craft2d-0.1.5/craft2d/resources/objects/stone.png
--rw-r--r--   0        0        0     1840 2023-07-09 20:14:15.424009 craft2d-0.1.5/craft2d/resources/objects/tree.png
--rw-r--r--   0        0        0     1423 2023-07-09 20:28:11.817175 craft2d-0.1.5/craft2d/resources/objects/weapon-advanced.png
--rw-r--r--   0        0        0     1437 2023-07-09 20:18:43.082515 craft2d-0.1.5/craft2d/resources/objects/weapon-basic.png
--rw-r--r--   0        0        0     1866 2023-07-09 20:15:14.696923 craft2d-0.1.5/craft2d/resources/objects/wood.png
--rw-r--r--   0        0        0     1164 2023-07-09 20:11:48.365759 craft2d-0.1.5/craft2d/resources/terrain/grass.png
--rw-r--r--   0        0        0     2474 2023-07-09 20:12:25.101611 craft2d-0.1.5/craft2d/resources/terrain/island.png
--rw-r--r--   0        0        0     1019 2023-07-10 17:23:00.155464 craft2d-0.1.5/craft2d/resources/terrain/water.png
--rw-r--r--   0        0        0      538 2023-07-24 17:56:46.958253 craft2d-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 craft2d-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      488 2023-07-12 15:58:14.885516 craft2d-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 12:33:35.821513 craft2d-0.1.6/craft2d/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:38:39.479663 craft2d-0.1.6/craft2d/config/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 18:38:45.164798 craft2d-0.1.6/craft2d/env/__init__.py
+-rw-r--r--   0        0        0    16628 2023-07-26 10:35:11.132625 craft2d-0.1.6/craft2d/env/environment.py
+-rw-r--r--   0        0        0        0 2023-07-10 20:04:09.256648 craft2d-0.1.6/craft2d/render/__init__.py
+-rw-r--r--   0        0        0    10299 2023-07-13 13:10:10.586272 craft2d-0.1.6/craft2d/render/render.py
+-rw-r--r--   0        0        0     2193 2023-07-09 20:09:51.278818 craft2d-0.1.6/craft2d/resources/agent/agent-down.png
+-rw-r--r--   0        0        0     2111 2023-07-09 20:09:25.442353 craft2d-0.1.6/craft2d/resources/agent/agent-left.png
+-rw-r--r--   0        0        0     2153 2023-07-09 20:09:37.887138 craft2d-0.1.6/craft2d/resources/agent/agent-right.png
+-rw-r--r--   0        0        0     2103 2023-07-09 20:09:11.258794 craft2d-0.1.6/craft2d/resources/agent/agent-up.png
+-rw-r--r--   0        0        0     1797 2023-07-09 20:14:01.501432 craft2d-0.1.6/craft2d/resources/farm/plant-large.png
+-rw-r--r--   0        0        0     1219 2023-07-09 20:13:45.609907 craft2d-0.1.6/craft2d/resources/farm/plant-medium.png
+-rw-r--r--   0        0        0     1000 2023-07-09 20:13:26.261484 craft2d-0.1.6/craft2d/resources/farm/plant-small.png
+-rw-r--r--   0        0        0     1074 2023-07-09 20:15:44.310385 craft2d-0.1.6/craft2d/resources/objects/bridge.png
+-rw-r--r--   0        0        0     3400 2023-07-09 20:30:59.755816 craft2d-0.1.6/craft2d/resources/objects/crafting-table.png
+-rw-r--r--   0        0        0     5133 2023-07-10 19:33:45.377024 craft2d-0.1.6/craft2d/resources/objects/gem.png
+-rw-r--r--   0        0        0     1007 2023-07-09 20:29:41.393116 craft2d-0.1.6/craft2d/resources/objects/grass.png
+-rw-r--r--   0        0        0     3826 2023-07-13 13:05:51.408981 craft2d-0.1.6/craft2d/resources/objects/princess.png
+-rw-r--r--   0        0        0     3178 2023-07-10 16:32:23.402820 craft2d-0.1.6/craft2d/resources/objects/rope.png
+-rw-r--r--   0        0        0     3823 2023-07-10 16:31:28.142800 craft2d-0.1.6/craft2d/resources/objects/sticks.png
+-rw-r--r--   0        0        0     1364 2023-07-09 20:14:47.718624 craft2d-0.1.6/craft2d/resources/objects/stone.png
+-rw-r--r--   0        0        0     1840 2023-07-09 20:14:15.424009 craft2d-0.1.6/craft2d/resources/objects/tree.png
+-rw-r--r--   0        0        0     1423 2023-07-09 20:28:11.817175 craft2d-0.1.6/craft2d/resources/objects/weapon-advanced.png
+-rw-r--r--   0        0        0     1437 2023-07-09 20:18:43.082515 craft2d-0.1.6/craft2d/resources/objects/weapon-basic.png
+-rw-r--r--   0        0        0     1866 2023-07-09 20:15:14.696923 craft2d-0.1.6/craft2d/resources/objects/wood.png
+-rw-r--r--   0        0        0     1164 2023-07-09 20:11:48.365759 craft2d-0.1.6/craft2d/resources/terrain/grass.png
+-rw-r--r--   0        0        0     2474 2023-07-09 20:12:25.101611 craft2d-0.1.6/craft2d/resources/terrain/island.png
+-rw-r--r--   0        0        0     1019 2023-07-10 17:23:00.155464 craft2d-0.1.6/craft2d/resources/terrain/water.png
+-rw-r--r--   0        0        0      538 2023-07-26 10:39:00.407153 craft2d-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 craft2d-0.1.6/PKG-INFO
```

### Comparing `craft2d-0.1.5/craft2d/env/environment.py` & `craft2d-0.1.6/craft2d/env/environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 LEFT = 1
 UP = 2
 DOWN = 3
 INTERACT = 4
 
 MAX_RESOURCE_COUNT = 10
 RESOURCE_COUNTS = {
-    "tree": 10,
-    "stone": 10,
-    "grass": 10,
-    "gem": 0,
+    "tree": 12,
+    "stone": 12,
+    "grass": 12,
+    "gem": 1,
 }
 ENVIRONMENT_OBJECTS = (
     "tree",
     "stone",
     "grass",
     "crafting-table",
     "water",
@@ -52,16 +52,18 @@
 }
 PROPS = (
     "WD",
     "STN",
     "GRS",
     "STKS",
     "RP",
-    "W-BSC",
     "BRG",
+    "W-BSC",
+    "GEM",
+    "W-ADV",
 )
 
 
 class Craft2dEnv(gym.Env):
     def __init__(
         self,
         n_rows: int,
@@ -109,24 +111,28 @@
                 inv_objects=INVENTORY_OBJECTS,
                 fps=24,
             )
 
     def reset(
         self,
         seed: int = None,
-        options: dict[str, str] = None,
+        options: dict[str, str] = {
+            "task_object": "WD",
+            "task_object_count": "M1",
+        },
     ):
         super().reset(seed=seed)
         np.random.seed(seed)
         # Reset number of steps taken in environment
         self.n_steps = 0
 
         # Reset task state
-        self.task_object = None
-        self.task_object_count = None
+        self.task_object = options["task_object"]
+        self.task_object_count = options["task_object_count"]
+        self.task_set = False
 
         # Object order specified in ENVIRONMENT_OBJECTS
         self.grid = np.zeros((self.n_rows, self.n_cols, self.n_env_objects))
         # Object order specified in INVENTORY_OBJECTS
         self.inventory = np.zeros((self.n_inv_objects,))
 
         # Initialize agent position and direction
@@ -138,16 +144,16 @@
 
             # Add resources to environment
             self._initialize_environment()
             self.cached_grid = self.grid.copy()
         else:
             self.grid = self.cached_grid.copy()
 
-        # # Setup island
-        # self._initialize_island()
+        # Setup island
+        self._initialize_island()
 
         self.interaction_props = ()
         return self._create_observation()
 
     def step(self, action: int):
         self.interaction_props = ()
 
@@ -161,15 +167,24 @@
         reward = 0
 
         # Reward = 1 when agent interacts with princess while holding task object
         props = obs[-1]
         if props == ("P",) and self.task_object is not None:
             task_obj_idx = PROPS.index(self.task_object)
 
-            count = 1 if self.task_object_count == "M1" else 2
+            if self.task_object_count == "M1":
+                count = 1
+            elif self.task_object_count == "M2":
+                count = 2
+            elif self.task_object_count == "M3":
+                count = 3
+            elif self.task_object_count == "M4":
+                count = 4
+            elif self.task_object_count == "M5":
+                count = 5
 
             if self.inventory[task_obj_idx] == count:
                 reward = 1
 
         done = reward == 1
         return obs, reward, done
 
@@ -236,34 +251,37 @@
                 continue
 
             if object_name in RESOURCE_COUNTS:
                 count = RESOURCE_COUNTS[object_name]
             else:
                 count = 1
 
-            print(object_name)
+            # print(object_name)
 
-            center_row = np.random.randint(3, self.n_rows - 4)
-            center_col = np.random.randint(3, self.n_cols - 4)
+            center_row = np.random.randint(5, self.n_rows - 4)
+            center_col = np.random.randint(5, self.n_cols - 4)
 
             if object_name == "tree":
-                center_row = 3
-                center_col = 8
+                center_row = 4
+                center_col = 10
             elif object_name == "stone":
-                center_row = 8
+                center_row = 10
                 center_col = 3
             elif object_name == "grass":
-                center_row = 8
-                center_col = 8
+                center_row = 10
+                center_col = 10
             elif object_name == "princess":
                 center_row = 0 + 2
-                center_col = 4 + 2
+                center_col = 3 + 2
             elif object_name == "crafting-table":
-                center_row = 2 + 2
-                center_col = 2 + 2
+                center_row = 0 + 2
+                center_col = 6 + 2
+            elif object_name == "gem":
+                center_row = 3 + 2
+                center_col = 3 + 2
 
             counter = 0
 
             for d_r, d_c in product(range(-2, 2), range(-2, 2)):
                 if counter == count:
                     break
 
@@ -384,33 +402,17 @@
             return
 
         # Get object type
         object_type = np.argmax(self.grid[itr_row, itr_col])
         object_name = ENVIRONMENT_OBJECTS[object_type]
 
         if object_name == "princess":
-            if self.task_object is None:
-                self.task_object = np.random.choice(
-                    (
-                        "WD",
-                        # "STN",
-                        # "GRS",
-                        # "STKS",
-                        # "RP",
-                        # "W-BSC",
-                        # "BRG",
-                    )
-                )
-                if self.task_object in ("WD", "STN"):
-                    count_options = ("M1",)
-                else:
-                    count_options = ("M1",)
-
-                self.task_object_count = np.random.choice(count_options)
+            if not self.task_set:
                 self.interaction_props = (self.task_object, self.task_object_count)
+                self.task_set = True
             else:
                 self.interaction_props = ("P",)
         elif self.task_object is None:
             # Cannot interact before task specified
             return
 
         # Collect resources from environment
```

### Comparing `craft2d-0.1.5/craft2d/render/render.py` & `craft2d-0.1.6/craft2d/render/render.py`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/agent/agent-down.png` & `craft2d-0.1.6/craft2d/resources/agent/agent-down.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/agent/agent-left.png` & `craft2d-0.1.6/craft2d/resources/agent/agent-left.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/agent/agent-right.png` & `craft2d-0.1.6/craft2d/resources/agent/agent-right.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/agent/agent-up.png` & `craft2d-0.1.6/craft2d/resources/agent/agent-up.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/farm/plant-large.png` & `craft2d-0.1.6/craft2d/resources/farm/plant-large.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/farm/plant-medium.png` & `craft2d-0.1.6/craft2d/resources/farm/plant-medium.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/farm/plant-small.png` & `craft2d-0.1.6/craft2d/resources/farm/plant-small.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/bridge.png` & `craft2d-0.1.6/craft2d/resources/objects/bridge.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/crafting-table.png` & `craft2d-0.1.6/craft2d/resources/objects/crafting-table.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/gem.png` & `craft2d-0.1.6/craft2d/resources/objects/gem.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/grass.png` & `craft2d-0.1.6/craft2d/resources/objects/grass.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/princess.png` & `craft2d-0.1.6/craft2d/resources/objects/princess.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/rope.png` & `craft2d-0.1.6/craft2d/resources/objects/rope.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/sticks.png` & `craft2d-0.1.6/craft2d/resources/objects/sticks.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/stone.png` & `craft2d-0.1.6/craft2d/resources/objects/stone.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/tree.png` & `craft2d-0.1.6/craft2d/resources/objects/tree.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/weapon-advanced.png` & `craft2d-0.1.6/craft2d/resources/objects/weapon-advanced.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/weapon-basic.png` & `craft2d-0.1.6/craft2d/resources/objects/weapon-basic.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/objects/wood.png` & `craft2d-0.1.6/craft2d/resources/objects/wood.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/terrain/grass.png` & `craft2d-0.1.6/craft2d/resources/terrain/grass.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/terrain/island.png` & `craft2d-0.1.6/craft2d/resources/terrain/island.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/craft2d/resources/terrain/water.png` & `craft2d-0.1.6/craft2d/resources/terrain/water.png`

 * *Files identical despite different names*

### Comparing `craft2d-0.1.5/pyproject.toml` & `craft2d-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "craft2d"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["Tristan Bester <tristanbester@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 numpy = "^1.25.1"
```

### Comparing `craft2d-0.1.5/PKG-INFO` & `craft2d-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft2d
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Author: Tristan Bester
 Author-email: tristanbester@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

