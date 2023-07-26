# Comparing `tmp/PyFlyt-0.8.4.tar.gz` & `tmp/PyFlyt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.8.4.tar", last modified: Tue Jul 25 14:43:24 2023, max compression
+gzip compressed data, was "PyFlyt-0.9.0.tar", last modified: Wed Jul 26 11:07:41 2023, max compression
```

## Comparing `PyFlyt-0.8.4.tar` & `PyFlyt-0.9.0.tar`

### file list

```diff
@@ -1,75 +1,57 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.860314 PyFlyt-0.8.4/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-06-30 13:35:00.000000 PyFlyt-0.8.4/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     4317 2023-07-25 14:43:24.860314 PyFlyt-0.8.4/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.848314 PyFlyt-0.8.4/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)      592 2023-07-25 14:26:37.000000 PyFlyt-0.8.4/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.848314 PyFlyt-0.8.4/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-07 16:22:47.000000 PyFlyt-0.8.4/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-27 15:02:04.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-16 17:24:04.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/base_wind_field.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12160 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-16 17:21:09.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7939 2023-07-25 14:21:42.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7474 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15874 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6826 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-02 11:06:46.000000 PyFlyt-0.8.4/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-05-16 17:31:41.000000 PyFlyt-0.8.4/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-11 16:33:17.000000 PyFlyt-0.8.4/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-16 17:13:33.000000 PyFlyt-0.8.4/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-05-16 17:12:54.000000 PyFlyt-0.8.4/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-16 17:14:09.000000 PyFlyt-0.8.4/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2570 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/core/wind/
--rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/core/wind/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-02 11:06:46.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9224 2023-07-25 14:21:42.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6261 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.852314 PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8958 2023-07-25 14:23:04.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-21 13:48:00.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3977 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6910 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11598 2023-07-25 14:23:00.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-05-25 12:51:02.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-07 18:11:27.000000 PyFlyt-0.8.4/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-28 12:51:18.000000 PyFlyt-0.8.4/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-06-30 13:35:00.000000 PyFlyt-0.8.4/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-28 12:51:18.000000 PyFlyt-0.8.4/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.844314 PyFlyt-0.8.4/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-22 14:06:54.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-21 13:48:00.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-02 11:06:46.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-15 11:28:20.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.856314 PyFlyt-0.8.4/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-07 01:25:05.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-07 01:25:05.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.860314 PyFlyt-0.8.4/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-07 18:11:27.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-07 18:11:27.000000 PyFlyt-0.8.4/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.848314 PyFlyt-0.8.4/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4317 2023-07-25 14:43:24.000000 PyFlyt-0.8.4/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1959 2023-07-25 14:43:24.000000 PyFlyt-0.8.4/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-07-25 14:43:24.000000 PyFlyt-0.8.4/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       43 2023-07-25 14:43:24.000000 PyFlyt-0.8.4/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-07-25 14:43:24.000000 PyFlyt-0.8.4/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1236 2023-07-25 14:43:12.000000 PyFlyt-0.8.4/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     2421 2023-07-25 13:06:07.000000 PyFlyt-0.8.4/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-07-25 14:43:24.860314 PyFlyt-0.8.4/setup.cfg
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-07-25 14:43:24.860314 PyFlyt-0.8.4/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9638 2023-07-25 14:35:24.000000 PyFlyt-0.8.4/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5304 2023-07-25 14:35:42.000000 PyFlyt-0.8.4/tests/test_gym_envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.241202 PyFlyt-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 11:07:41.241202 PyFlyt-0.9.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.233202 PyFlyt-0.9.0/PyFlyt/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.233202 PyFlyt-0.9.0/PyFlyt/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/core/abstractions/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/base_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/base_drone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/base_wind_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12160 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/boosters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/boring_bodies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/gimbals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/motors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/abstractions/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19052 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/aviary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/core/drones/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/drones/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/drones/fixedwing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18406 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/drones/quadx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/drones/rocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/load_objs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/core/wind/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/core/wind/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/gym_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/gym_envs/fixedwing_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.237202 PyFlyt-0.9.0/PyFlyt/gym_envs/rocket_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-07-26 11:07:25.000000 PyFlyt-0.9.0/PyFlyt/gym_envs/waypoint_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.241202 PyFlyt-0.9.0/PyFlyt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/PyFlyt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/PyFlyt/utils/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.233202 PyFlyt-0.9.0/PyFlyt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 11:07:41.000000 PyFlyt-0.9.0/PyFlyt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-26 11:07:41.000000 PyFlyt-0.9.0/PyFlyt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:07:41.000000 PyFlyt-0.9.0/PyFlyt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 11:07:41.000000 PyFlyt-0.9.0/PyFlyt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 11:07:41.000000 PyFlyt-0.9.0/PyFlyt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:07:41.241202 PyFlyt-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:07:41.241202 PyFlyt-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-07-26 11:07:26.000000 PyFlyt-0.9.0/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.8.4/LICENSE.txt` & `PyFlyt-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PKG-INFO` & `PyFlyt-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.8.4
+Version: 0.9.0
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,14 +28,15 @@
 Project-URL: Bug Report, https://github.com/jjshoots/PyFlyt/issues
 Keywords: Reinforcement Learning,UAVs,drones,Quadcopter,AI,RL,Gymnasium
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 ![GitHub CI](https://github.com/jjshoots/PyFlyt/actions/workflows/linux-test.yml/badge.svg)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![hits](https://hits.dwyl.com/jjshoots/PyFlyt.svg)](https://hits.dwyl.com/jjshoots/PyFlyt)
 [![total downloads](https://static.pepy.tech/personalized-badge/pyflyt?period=total&units=international_system&left_color=grey&right_color=green&left_text=total%20downloads)](https://pepy.tech/project/pyflyt)
 [![weekly downloads](https://static.pepy.tech/personalized-badge/pyflyt?period=week&units=international_system&left_color=grey&right_color=green&left_text=weekly%20downloads)](https://pepy.tech/project/pyflyt)
```

### Comparing `PyFlyt-0.8.4/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.9.0/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.9.0/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.9.0/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.9.0/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.9.0/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.9.0/PyFlyt/core/abstractions/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import math
 import warnings
 
 import numpy as np
 from pybullet_utils import bullet_client
 
+from PyFlyt.utils import check_numpy
+
 
 class Camera:
     """A camera component.
 
     The `Camera` component simulates a camera attached to a link on the drone.
     The camera itself can be gimballed to achieve a horizon lock effect.
     In addition, the field-of-view (FOV), tilt angle, resolution, and offset distance from the main link can be adjusted.
@@ -52,14 +54,15 @@
             camera_FOV_degrees (float): the field-of-view of the camera in degrees.
             camera_angle_degrees (float): when gimballed, this is the angle of downtilt from horizon; when not gimballed, this is theh angle of uptile from horizon.
             camera_resolution (tuple[int, int]): the resolution of the camera in terms of [width, height].
             camera_position_offset (np.ndarray = np.array([0.0, 0.0, 0.0])): an (3,) array representing an offset of where the camera is from the center of the link in `camera_id`.
             is_tracking_camera (bool = False): if the camera is a tracking camera, the focus point of the camera is adjusted to focus on the center body of the aircraft instead of at infinity.
             cinematic (bool = False): it's not a bug, it's a feature.
         """
+        check_numpy()
         if is_tracking_camera and use_gimbal:
             warnings.warn(
                 "Use_gimbal and is_tracking_camera are both enabled. This will lead to funky behaviour."
             )
 
         # grab the pybullet client instance and relevant IDs
         self.p = p
```

### Comparing `PyFlyt-0.8.4/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.9.0/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.9.0/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.9.0/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.9.0/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/aviary.py` & `PyFlyt-0.9.0/PyFlyt/core/aviary.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.9.0/PyFlyt/core/drones/fixedwing.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.9.0/PyFlyt/core/drones/quadx.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.9.0/PyFlyt/core/drones/rocket.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/core/load_objs.py` & `PyFlyt-0.9.0/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.9.0/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.9.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import gymnasium
 import numpy as np
 import pybullet as p
 from gymnasium import spaces
 
 from PyFlyt.core.aviary import Aviary
+from PyFlyt.utils import check_numpy
 
 
 class FixedwingBaseEnv(gymnasium.Env):
     """Base PyFlyt Environment for the Fixedwing model using the Gymnasim API."""
 
     metadata = {"render_modes": ["human", "rgb_array"], "render_fps": 30}
 
@@ -262,14 +263,15 @@
         # increment step count
         self.step_count += 1
 
         return self.state, self.reward, self.termination, self.truncation, self.info
 
     def render(self):
         """render."""
+        check_numpy()
         assert (
             self.render_mode is not None
         ), "Please set `render_mode='human'` or `render_mode='rgb_array'` to use this function."
 
         _, _, rgbaImg, _, _ = self.env.getCameraImage(
             width=self.render_resolution[1],
             height=self.render_resolution[0],
```

### Comparing `PyFlyt-0.8.4/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.9.0/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import gymnasium
 import numpy as np
 import pybullet as p
 from gymnasium import spaces
 
 from PyFlyt.core.aviary import Aviary
+from PyFlyt.utils import check_numpy
 
 
 class QuadXBaseEnv(gymnasium.Env):
     """Base PyFlyt Environment for the QuadX model using the Gymnasim API."""
 
     metadata = {"render_modes": ["human", "rgb_array"], "render_fps": 30}
 
@@ -256,14 +257,15 @@
         # increment step count
         self.step_count += 1
 
         return self.state, self.reward, self.termination, self.truncation, self.info
 
     def render(self):
         """render."""
+        check_numpy()
         assert (
             self.render_mode is not None
         ), "Please set `render_mode='human'` or `render_mode='rgb_array'` to use this function."
 
         _, _, rgbaImg, _, _ = self.env.getCameraImage(
             width=self.render_resolution[1],
             height=self.render_resolution[0],
```

### Comparing `PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.9.0/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.9.0/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import gymnasium
 import numpy as np
 import pybullet as p
 from gymnasium import spaces
 
 from PyFlyt.core.aviary import Aviary
+from PyFlyt.utils import check_numpy
 
 
 class RocketBaseEnv(gymnasium.Env):
     """Base PyFlyt Environment for the Rocket model using the Gymnasim API."""
 
     metadata = {"render_modes": ["human", "rgb_array"], "render_fps": 30}
 
@@ -318,14 +319,15 @@
         # increment step count
         self.step_count += 1
 
         return self.state, self.reward, self.termination, self.truncation, self.info
 
     def render(self):
         """render."""
+        check_numpy()
         assert (
             self.render_mode is not None
         ), "Please set `render_mode='human'` or `render_mode='rgb_array'` to use this function."
 
         _, _, rgbaImg, _, _ = self.env.getCameraImage(
             width=self.render_resolution[1],
             height=self.render_resolution[0],
```

### Comparing `PyFlyt-0.8.4/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.9.0/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.9.0/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.9.0/PyFlyt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.8.4
+Version: 0.9.0
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -28,14 +28,15 @@
 Project-URL: Bug Report, https://github.com/jjshoots/PyFlyt/issues
 Keywords: Reinforcement Learning,UAVs,drones,Quadcopter,AI,RL,Gymnasium
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE.txt
 
 ![GitHub CI](https://github.com/jjshoots/PyFlyt/actions/workflows/linux-test.yml/badge.svg)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://pre-commit.com/)
 [![hits](https://hits.dwyl.com/jjshoots/PyFlyt.svg)](https://hits.dwyl.com/jjshoots/PyFlyt)
 [![total downloads](https://static.pepy.tech/personalized-badge/pyflyt?period=total&units=international_system&left_color=grey&right_color=green&left_text=total%20downloads)](https://pepy.tech/project/pyflyt)
 [![weekly downloads](https://static.pepy.tech/personalized-badge/pyflyt?period=week&units=international_system&left_color=grey&right_color=green&left_text=weekly%20downloads)](https://pepy.tech/project/pyflyt)
```

### Comparing `PyFlyt-0.8.4/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.9.0/PyFlyt.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -33,23 +33,11 @@
 PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
 PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
 PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
 PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
 PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
 PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
 PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
-PyFlyt/models/landing_pad.urdf
-PyFlyt/models/race_gate.urdf
-PyFlyt/models/target.urdf
-PyFlyt/models/vehicles/cf2x/cf2.dae
-PyFlyt/models/vehicles/cf2x/cf2x.urdf
-PyFlyt/models/vehicles/cf2x/cf2x.yaml
-PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
-PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
-PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-PyFlyt/models/vehicles/quadplane/quadplane.urdf
-PyFlyt/models/vehicles/quadplane/quadplane.yaml
-PyFlyt/models/vehicles/rocket/rocket.urdf
-PyFlyt/models/vehicles/rocket/rocket.yaml
+PyFlyt/utils/__init__.py
+PyFlyt/utils/checks.py
 tests/test_core.py
 tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.8.4/pyproject.toml` & `PyFlyt-0.9.0/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.8.4"
+version = "0.9.0"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,14 +16,17 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = ["numpy", "matplotlib", "gymnasium", "pybullet", "pyyaml"]
 keywords = ["Reinforcement Learning", "UAVs", "drones", "Quadcopter", "AI", "RL", "Gymnasium"]
 license = { file="./LICENSE.txt" }
 
+[project.optional-dependencies]
+dev = ["pytest", "pre-commit"]
+
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["PyFlyt", "PyFlyt.*"]
 
 [project.urls]
```

### Comparing `PyFlyt-0.8.4/readme.md` & `PyFlyt-0.9.0/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/tests/test_core.py` & `PyFlyt-0.9.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.8.4/tests/test_gym_envs.py` & `PyFlyt-0.9.0/tests/test_gym_envs.py`

 * *Files identical despite different names*

