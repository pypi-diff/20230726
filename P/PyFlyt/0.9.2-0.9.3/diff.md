# Comparing `tmp/PyFlyt-0.9.2.tar.gz` & `tmp/PyFlyt-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.9.2.tar", last modified: Wed Jul 26 12:11:20 2023, max compression
+gzip compressed data, was "PyFlyt-0.9.3.tar", last modified: Wed Jul 26 12:19:27 2023, max compression
```

## Comparing `PyFlyt-0.9.2.tar` & `PyFlyt-0.9.3.tar`

### file list

```diff
@@ -1,57 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.729003 PyFlyt-0.9.2/PyFlyt/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.729003 PyFlyt-0.9.2/PyFlyt/core/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.733003 PyFlyt-0.9.2/PyFlyt/core/abstractions/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/base_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/base_drone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/base_wind_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/boosters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/boring_bodies.py
--rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/gimbals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/motors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/abstractions/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/aviary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.733003 PyFlyt-0.9.2/PyFlyt/core/drones/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/drones/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/drones/fixedwing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/drones/quadx.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/drones/rocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/load_objs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.733003 PyFlyt-0.9.2/PyFlyt/core/wind/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/core/wind/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.733003 PyFlyt-0.9.2/PyFlyt/gym_envs/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.733003 PyFlyt-0.9.2/PyFlyt/gym_envs/fixedwing_envs/
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/PyFlyt/gym_envs/rocket_envs/
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/gym_envs/waypoint_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/PyFlyt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/PyFlyt/utils/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.729003 PyFlyt-0.9.2/PyFlyt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 12:11:20.000000 PyFlyt-0.9.2/PyFlyt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-26 12:11:20.000000 PyFlyt-0.9.2/PyFlyt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:11:20.000000 PyFlyt-0.9.2/PyFlyt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 12:11:20.000000 PyFlyt-0.9.2/PyFlyt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 12:11:20.000000 PyFlyt-0.9.2/PyFlyt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:11:20.737003 PyFlyt-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-26 12:11:07.000000 PyFlyt-0.9.2/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.626584 PyFlyt-0.9.3/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-06-30 13:35:00.000000 PyFlyt-0.9.3/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4337 2023-07-26 12:19:27.626584 PyFlyt-0.9.3/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.614584 PyFlyt-0.9.3/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-07-26 10:35:55.000000 PyFlyt-0.9.3/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.614584 PyFlyt-0.9.3/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-07 16:22:47.000000 PyFlyt-0.9.3/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.618584 PyFlyt-0.9.3/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-15 11:28:20.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-27 15:02:04.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-16 17:24:04.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-15 11:28:20.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/base_wind_field.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12160 2023-07-25 13:06:07.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-16 17:21:09.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7999 2023-07-26 10:41:20.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7474 2023-07-25 13:06:07.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15874 2023-07-25 13:06:07.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6826 2023-07-25 13:06:07.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-02 11:06:46.000000 PyFlyt-0.9.3/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-05-16 17:31:41.000000 PyFlyt-0.9.3/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.618584 PyFlyt-0.9.3/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-11 16:33:17.000000 PyFlyt-0.9.3/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-16 17:13:33.000000 PyFlyt-0.9.3/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-05-16 17:12:54.000000 PyFlyt-0.9.3/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-16 17:14:09.000000 PyFlyt-0.9.3/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2570 2023-07-25 13:06:07.000000 PyFlyt-0.9.3/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.618584 PyFlyt-0.9.3/PyFlyt/core/wind/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-15 11:28:20.000000 PyFlyt-0.9.3/PyFlyt/core/wind/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.618584 PyFlyt-0.9.3/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-02 11:06:46.000000 PyFlyt-0.9.3/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.618584 PyFlyt-0.9.3/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9283 2023-07-26 10:41:16.000000 PyFlyt-0.9.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-07-25 13:06:07.000000 PyFlyt-0.9.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.622584 PyFlyt-0.9.3/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9017 2023-07-26 10:40:36.000000 PyFlyt-0.9.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-21 13:48:00.000000 PyFlyt-0.9.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3977 2023-07-25 13:06:07.000000 PyFlyt-0.9.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-07-25 13:06:07.000000 PyFlyt-0.9.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.622584 PyFlyt-0.9.3/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11657 2023-07-26 10:39:33.000000 PyFlyt-0.9.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-05-25 12:51:02.000000 PyFlyt-0.9.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-07 18:11:27.000000 PyFlyt-0.9.3/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.622584 PyFlyt-0.9.3/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-28 12:51:18.000000 PyFlyt-0.9.3/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-06-30 13:35:00.000000 PyFlyt-0.9.3/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-28 12:51:18.000000 PyFlyt-0.9.3/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.610584 PyFlyt-0.9.3/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.622584 PyFlyt-0.9.3/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-22 14:06:54.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-15 11:28:20.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-15 11:28:20.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.622584 PyFlyt-0.9.3/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-21 13:48:00.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-02 11:06:46.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.622584 PyFlyt-0.9.3/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-15 11:28:20.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-15 11:28:20.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.626584 PyFlyt-0.9.3/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-07 01:25:05.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-07 01:25:05.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.626584 PyFlyt-0.9.3/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-07 18:11:27.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-07 18:11:27.000000 PyFlyt-0.9.3/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.626584 PyFlyt-0.9.3/PyFlyt/utils/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       56 2023-07-26 10:40:27.000000 PyFlyt-0.9.3/PyFlyt/utils/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      690 2023-07-26 10:57:45.000000 PyFlyt-0.9.3/PyFlyt/utils/checks.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.614584 PyFlyt-0.9.3/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4337 2023-07-26 12:19:27.000000 PyFlyt-0.9.3/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2007 2023-07-26 12:19:27.000000 PyFlyt-0.9.3/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-26 12:19:27.000000 PyFlyt-0.9.3/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       68 2023-07-26 12:19:27.000000 PyFlyt-0.9.3/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-07-26 12:19:27.000000 PyFlyt-0.9.3/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1369 2023-07-26 12:18:58.000000 PyFlyt-0.9.3/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2421 2023-07-25 13:06:07.000000 PyFlyt-0.9.3/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-26 12:19:27.626584 PyFlyt-0.9.3/setup.cfg
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-26 12:19:27.626584 PyFlyt-0.9.3/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9638 2023-07-25 14:35:24.000000 PyFlyt-0.9.3/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5304 2023-07-25 14:35:42.000000 PyFlyt-0.9.3/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.9.2/LICENSE.txt` & `PyFlyt-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PKG-INFO` & `PyFlyt-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.9.2
+Version: 0.9.3
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.9.2/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.9.3/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.9.3/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.9.3/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.9.3/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.9.3/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.9.3/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.9.3/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.9.3/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.9.3/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.9.3/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/aviary.py` & `PyFlyt-0.9.3/PyFlyt/core/aviary.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.9.3/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.9.3/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.9.3/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/core/load_objs.py` & `PyFlyt-0.9.3/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.9.3/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.9.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.9.3/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.9.3/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.9.3/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.9.3/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.9.3/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.9.3/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.9.3/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.9.3/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt/utils/checks.py` & `PyFlyt-0.9.3/PyFlyt/utils/checks.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.9.3/PyFlyt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.9.2
+Version: 0.9.3
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `PyFlyt-0.9.2/pyproject.toml` & `PyFlyt-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.9.2"
+version = "0.9.3"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -27,15 +27,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["PyFlyt", "PyFlyt.*"]
 
 [tool.setuptools.package-data]
 pyflyt = [
-    "PyFlyt/models/*",
+    "PyFlyt/models/**",
 ]
 
 [project.urls]
 Repository = "https://github.com/jjshoots/PyFlyt"
 Documentation = "https://jjshoots.github.io/PyFlyt/documentation.html"
 "Bug Report" = "https://github.com/jjshoots/PyFlyt/issues"
```

### Comparing `PyFlyt-0.9.2/readme.md` & `PyFlyt-0.9.3/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/tests/test_core.py` & `PyFlyt-0.9.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.9.2/tests/test_gym_envs.py` & `PyFlyt-0.9.3/tests/test_gym_envs.py`

 * *Files identical despite different names*

