# Comparing `tmp/PyFlyt-0.9.0.tar.gz` & `tmp/PyFlyt-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.9.0.tar", last modified: Wed Jul 26 11:07:41 2023, max compression
+gzip compressed data, was "PyFlyt-0.9.2.tar", last modified: Wed Jul 26 12:11:20 2023, max compression
```

## Comparing `PyFlyt-0.9.0.tar` & `PyFlyt-0.9.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.241202 PyFlyt-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 11:07:41.241202 PyFlyt-0.9.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.233202 PyFlyt-0.9.0/PyFlyt/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.233202 PyFlyt-0.9.0/PyFlyt/core/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/core/abstractions/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/base_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/base_drone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/base_wind_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/boosters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/boring_bodies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/gimbals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/motors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/aviary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/core/drones/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/drones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/drones/fixedwing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/drones/quadx.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/drones/rocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/load_objs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/core/wind/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/wind/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/gym_envs/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/gym_envs/fixedwing_envs/
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/gym_envs/rocket_envs/
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/waypoint_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.241202 PyFlyt-0.9.0/PyFlyt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/PyFlyt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/PyFlyt/utils/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.233202 PyFlyt-0.9.0/PyFlyt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 11:07:41.000000 PyFlyt-0.9.0/PyFlyt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-26 11:07:41.000000 PyFlyt-0.9.0/PyFlyt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:07:41.000000 PyFlyt-0.9.0/PyFlyt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 11:07:41.000000 PyFlyt-0.9.0/PyFlyt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 11:07:41.000000 PyFlyt-0.9.0/PyFlyt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:07:41.241202 PyFlyt-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.241202 PyFlyt-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/tests/test_gym_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.729003 PyFlyt-0.9.2/PyFlyt/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.729003 PyFlyt-0.9.2/PyFlyt/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.733003 PyFlyt-0.9.2/PyFlyt/core/abstractions/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/base_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/base_drone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/base_wind_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/boosters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/boring_bodies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/gimbals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/motors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/aviary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.733003 PyFlyt-0.9.2/PyFlyt/core/drones/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/drones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/drones/fixedwing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/drones/quadx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/drones/rocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/load_objs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.733003 PyFlyt-0.9.2/PyFlyt/core/wind/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/wind/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.733003 PyFlyt-0.9.2/PyFlyt/gym_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.733003 PyFlyt-0.9.2/PyFlyt/gym_envs/fixedwing_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/PyFlyt/gym_envs/rocket_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/waypoint_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/PyFlyt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/utils/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.729003 PyFlyt-0.9.2/PyFlyt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 12:11:20.000000 PyFlyt-0.9.2/PyFlyt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-26 12:11:20.000000 PyFlyt-0.9.2/PyFlyt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:11:20.000000 PyFlyt-0.9.2/PyFlyt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 12:11:20.000000 PyFlyt-0.9.2/PyFlyt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 12:11:20.000000 PyFlyt-0.9.2/PyFlyt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.9.0/LICENSE.txt` & `PyFlyt-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PKG-INFO` & `PyFlyt-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.9.0
+Version: 0.9.2
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.9.0/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.9.2/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.9.2/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.9.2/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.9.2/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.9.2/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.9.2/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.9.2/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.9.2/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.9.2/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.9.2/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/aviary.py` & `PyFlyt-0.9.2/PyFlyt/core/aviary.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.9.2/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.9.2/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.9.2/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/core/load_objs.py` & `PyFlyt-0.9.2/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.9.2/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.9.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.9.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.9.2/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.9.2/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.9.2/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt/utils/checks.py` & `PyFlyt-0.9.2/PyFlyt/utils/checks.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.9.2/PyFlyt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.9.0
+Version: 0.9.2
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.9.0/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.9.2/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/pyproject.toml` & `PyFlyt-0.9.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.9.0"
+version = "0.9.2"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -25,14 +25,19 @@
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["PyFlyt", "PyFlyt.*"]
 
+[tool.setuptools.package-data]
+pyflyt = [
+    "PyFlyt/models/*",
+]
+
 [project.urls]
 Repository = "https://github.com/jjshoots/PyFlyt"
 Documentation = "https://jjshoots.github.io/PyFlyt/documentation.html"
 "Bug Report" = "https://github.com/jjshoots/PyFlyt/issues"
 
 #######################################################################################
 # linters
```

### Comparing `PyFlyt-0.9.0/readme.md` & `PyFlyt-0.9.2/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/tests/test_core.py` & `PyFlyt-0.9.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.0/tests/test_gym_envs.py` & `PyFlyt-0.9.2/tests/test_gym_envs.py`

 * *Files identical despite different names*

