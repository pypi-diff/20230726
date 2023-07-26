# Comparing `tmp/PyZeta-0.0.1.tar.gz` & `tmp/PyZeta-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyZeta-0.0.1.tar", last modified: Mon May  8 21:39:05 2023, max compression
+gzip compressed data, was "PyZeta-0.0.2.tar", last modified: Wed Jul 26 10:56:56 2023, max compression
```

## Comparing `PyZeta-0.0.1.tar` & `PyZeta-0.0.2.tar`

### file list

```diff
@@ -1,83 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.533177 PyZeta-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 21:38:52.000000 PyZeta-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 21:38:52.000000 PyZeta-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    48299 2023-05-08 21:39:05.533177 PyZeta-0.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/PyZeta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48299 2023-05-08 21:39:05.000000 PyZeta-0.0.1/PyZeta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-08 21:39:05.000000 PyZeta-0.0.1/PyZeta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:39:05.000000 PyZeta-0.0.1/PyZeta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-08 21:39:05.000000 PyZeta-0.0.1/PyZeta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-08 21:39:05.000000 PyZeta-0.0.1/PyZeta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-08 21:39:05.000000 PyZeta-0.0.1/PyZeta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-08 21:38:52.000000 PyZeta-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.517177 PyZeta-0.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-08 21:38:52.000000 PyZeta-0.0.1/docs/_static/docstr_coverage_badge.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/pyzeta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/pyzeta/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/pyzeta/core/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/core/distributions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/pyzeta/core/dynamics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/core/dynamics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/pyzeta/core/dynamics/function_systems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/core/dynamics/function_systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/pyzeta/core/dynamics/symbolic_dynamics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/core/dynamics/symbolic_dynamics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/pyzeta/core/factories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/core/factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/pyzeta/core/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/core/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.525177 PyZeta-0.0.1/pyzeta/core/pyzeta_types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/core/pyzeta_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/core/symmetries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/core/symmetries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/core/zetas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/core/zetas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/experiments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/experiments/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/experiments/configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/framework/analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/framework/analyzers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/framework/feature_toggle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/framework/feature_toggle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/framework/feature_toggle/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/framework/feature_toggle/toggle_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/framework/initialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/framework/initialization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/framework/ioc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/framework/ioc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/framework/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/framework/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/framework/pyzeta_logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/framework/pyzeta_logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/framework/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/framework/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/geometry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/tests/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/tests/feature_toggle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/tests/feature_toggle/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2236 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/tests/feature_toggle/test_toggle_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.529177 PyZeta-0.0.1/pyzeta/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/tests/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.533177 PyZeta-0.0.1/pyzeta/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.533177 PyZeta-0.0.1/pyzeta/view/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.533177 PyZeta-0.0.1/pyzeta/view/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/view/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/view/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:39:05.533177 PyZeta-0.0.1/pyzeta/view/gui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:52.000000 PyZeta-0.0.1/pyzeta/view/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 21:39:05.533177 PyZeta-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.353160 PyZeta-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 10:56:45.000000 PyZeta-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-26 10:56:45.000000 PyZeta-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    48326 2023-07-26 10:56:56.353160 PyZeta-0.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/PyZeta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48326 2023-07-26 10:56:56.000000 PyZeta-0.0.2/PyZeta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-07-26 10:56:56.000000 PyZeta-0.0.2/PyZeta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 10:56:56.000000 PyZeta-0.0.2/PyZeta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-26 10:56:56.000000 PyZeta-0.0.2/PyZeta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-26 10:56:56.000000 PyZeta-0.0.2/PyZeta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 10:56:56.000000 PyZeta-0.0.2/PyZeta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-26 10:56:45.000000 PyZeta-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.333159 PyZeta-0.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-26 10:56:45.000000 PyZeta-0.0.2/docs/_static/docstr_coverage_badge.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/core/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/distributions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/core/dynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/function_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/helpers/schottky_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/implementations/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/implementations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/implementations/funnel_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/implementations/funnel_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/implementations/hyperbolic_cylinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/integral_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/map_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/moebius_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/schottky_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/function_systems/schottky_surface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/core/dynamics/symbolic_dynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/symbolic_dynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/symbolic_dynamics/abstract_dynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/core/dynamics/symbolic_dynamics/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/symbolic_dynamics/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7584 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/symbolic_dynamics/helpers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/symbolic_dynamics/reduced_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/dynamics/symbolic_dynamics/symbolic_dynamics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/core/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.341159 PyZeta-0.0.2/pyzeta/core/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/core/pyzeta_types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/pyzeta_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/pyzeta_types/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/pyzeta_types/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/pyzeta_types/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/core/symmetries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/symmetries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/symmetries/symmetry_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/symmetries/trivial_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/core/zetas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/zetas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/zetas/abstract_zeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/core/zetas/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/zetas/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/zetas/helpers/bell_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/core/zetas/selberg_zeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/experiments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/experiments/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/experiments/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/framework/aop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/aop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/aop/advice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/framework/aop/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/aop/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/aop/analyzers/profiling_advice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/aop/analyzers/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/aop/aspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/aop/aspect_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/aop/point_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/aop/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/framework/feature_toggle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/feature_toggle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/feature_toggle/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/feature_toggle/toggle_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/feature_toggle/toggle_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/framework/initialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/initialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/initialization/init_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/initialization/initialization_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/framework/ioc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/ioc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/ioc/configuration_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/ioc/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/ioc/container_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.345159 PyZeta-0.0.2/pyzeta/framework/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/framework/pyzeta_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/pyzeta_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/pyzeta_logging/log_levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/pyzeta_logging/log_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/pyzeta_logging/loggable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/pyzeta_logging/logger_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/framework/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/core_settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/invalid_setting_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/framework/settings/json_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/json_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/json_settings/json_core_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/json_settings/json_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/json_settings/json_settings_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/framework/settings/ram_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/ram_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/ram_settings/ram_settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/settings_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/framework/settings/settings_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/geometry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/tests/dynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/dynamics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/tests/dynamics/function_systems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/dynamics/function_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/dynamics/function_systems/test_cylinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/tests/dynamics/symbolic_dynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/dynamics/symbolic_dynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/dynamics/symbolic_dynamics/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/dynamics/symbolic_dynamics/test_reduced_symbolics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/dynamics/symbolic_dynamics/test_symbolics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/tests/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/tests/framework/feature_toggle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/framework/feature_toggle/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4423 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/framework/feature_toggle/test_toggle_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/tests/framework/ioc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/framework/ioc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/framework/ioc/test_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/resources/symbolics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/tests/zetas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/zetas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/tests/zetas/test_selberg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.349159 PyZeta-0.0.2/pyzeta/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.353160 PyZeta-0.0.2/pyzeta/view/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/view/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/view/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:56.353160 PyZeta-0.0.2/pyzeta/view/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 10:56:45.000000 PyZeta-0.0.2/pyzeta/view/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 10:56:56.353160 PyZeta-0.0.2/setup.cfg
```

### Comparing `PyZeta-0.0.1/LICENSE` & `PyZeta-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyZeta-0.0.1/PKG-INFO` & `PyZeta-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyZeta
-Version: 0.0.1
+Version: 0.0.2
 Summary: Numerical project all about (dynamical) zeta functions and resonances.
 Author-email: Philipp Schuette <pschuet2@mail.uni-paderborn.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,14 +693,15 @@
 
 ==================
 The PyZeta Project
 ==================
 
 .. |badge0| image:: https://github.com/Spectral-Analysis-UPB/PyZeta/blob/main/docs/_static/docstr_coverage_badge.svg
    :target: https://pypi.org/project/docstr-coverage/
+   :alt: docstr-coverage=?
 
 .. |badge1| image:: https://img.shields.io/badge/Language-Python-blue.svg
    :target: https://pypi.org/project/PyZeta/
 
 .. |badge2| image:: http://img.shields.io/badge/benchmarked%20by-asv-blue.svg?style=flat
    :target: https://github.com/Spectral-Analysis-UPB/PyZeta
```

### Comparing `PyZeta-0.0.1/PyZeta.egg-info/PKG-INFO` & `PyZeta-0.0.2/PyZeta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyZeta
-Version: 0.0.1
+Version: 0.0.2
 Summary: Numerical project all about (dynamical) zeta functions and resonances.
 Author-email: Philipp Schuette <pschuet2@mail.uni-paderborn.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -693,14 +693,15 @@
 
 ==================
 The PyZeta Project
 ==================
 
 .. |badge0| image:: https://github.com/Spectral-Analysis-UPB/PyZeta/blob/main/docs/_static/docstr_coverage_badge.svg
    :target: https://pypi.org/project/docstr-coverage/
+   :alt: docstr-coverage=?
 
 .. |badge1| image:: https://img.shields.io/badge/Language-Python-blue.svg
    :target: https://pypi.org/project/PyZeta/
 
 .. |badge2| image:: http://img.shields.io/badge/benchmarked%20by-asv-blue.svg?style=flat
    :target: https://github.com/Spectral-Analysis-UPB/PyZeta
```

### Comparing `PyZeta-0.0.1/README.rst` & `PyZeta-0.0.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ==================
 The PyZeta Project
 ==================
 
 .. |badge0| image:: https://github.com/Spectral-Analysis-UPB/PyZeta/blob/main/docs/_static/docstr_coverage_badge.svg
    :target: https://pypi.org/project/docstr-coverage/
+   :alt: docstr-coverage=?
 
 .. |badge1| image:: https://img.shields.io/badge/Language-Python-blue.svg
    :target: https://pypi.org/project/PyZeta/
 
 .. |badge2| image:: http://img.shields.io/badge/benchmarked%20by-asv-blue.svg?style=flat
    :target: https://github.com/Spectral-Analysis-UPB/PyZeta
```

### Comparing `PyZeta-0.0.1/pyproject.toml` & `PyZeta-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyZeta"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name = "Philipp Schuette", email = "pschuet2@mail.uni-paderborn.de"}
 ]
 description = "Numerical project all about (dynamical) zeta functions and resonances."
 readme = "README.rst"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
@@ -22,14 +22,15 @@
     "numpy>=1.24",
     "cython",
     "matplotlib",
     "scipy>=1.9.1",
     "typing-extensions",
     "numba>=0.55.1",
     "bokeh",
+    "pyzeal>=1.0.0"
 ]
 
 [project.optional-dependencies]
 docs = [
 	"sphinx",
 	"sphinx-material",
 	"nbsphinx",
@@ -76,14 +77,15 @@
 junit_family = "legacy"
 filterwarnings = "ignore::DeprecationWarning"
 
 [tool.pytest.ini_options]
 addopts = "--import-mode=importlib --strict-markers -p no:logging"
 markers = [
     "slow: mark tests as slow",
+    "container: mark tests of dependency inversion containers",
 ]
 
 [tool.coverage.run]
 omit = ["pyzeta/tests/*/*.py"]
 
 [tool.mypy]
 python_version = "3.9"
```

### Comparing `PyZeta-0.0.1/pyzeta/framework/feature_toggle/feature_flag.py` & `PyZeta-0.0.2/pyzeta/framework/feature_toggle/feature_flag.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,28 +2,33 @@
 Very basic implementation of feature flags. Instances of these flags are useful
 to e.g. toggle certain (parts of) workflows in complex numerical experiments.
 
 Authors:\n
 - Philipp Schuette\n
 """
 from dataclasses import dataclass
-from logging import Logger
+
+from pyzeta.framework.pyzeta_logging.logger_facade import PyZetaLogger
 
 
 @dataclass
 class FeatureFlag:
     "Simple implementation of a feature flag."
     name: str
     value: bool
     description: str
-    logger: Logger
+    logger: PyZetaLogger
     timesAccessible: int = 1
 
     def __bool__(self) -> bool:
-        # TODO: replace this with framework logging!
+        """
+        Custom boolean evaluation that makes the flag delegate boolean behavior
+        to its `value` attribute after checking the current status of
+        `timesAccessible`.
+        """
         self.logger.warning(
             "feature flag %s with value %s accessed!",
             self.name,
             str(self.value),
         )
         if self.timesAccessible != 0:
             self.timesAccessible -= 1
```

### Comparing `PyZeta-0.0.1/pyzeta/framework/feature_toggle/toggle_collection.py` & `PyZeta-0.0.2/pyzeta/framework/feature_toggle/toggle_collection.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,18 +13,19 @@
     toggles = MyToggles("toggles.json")
 
 Authors:\n
 - Philipp Schuette\n
 """
 
 from json import load
-from logging import getLogger
 from typing import Dict, Type, TypedDict
 
 from pyzeta.framework.feature_toggle.feature_flag import FeatureFlag
+from pyzeta.framework.feature_toggle.toggle_exception import ToggleException
+from pyzeta.framework.pyzeta_logging.loggable import Loggable
 
 
 class LoadedToggleRequired(TypedDict):
     "This is need to be able to mix required and optional keys pre python3.11."
     name: str
     value: bool
     description: str
@@ -32,73 +33,70 @@
 
 class LoadedToggle(LoadedToggleRequired, total=False):
     "The type of a toggle configuration loaded from json."
     timesAccessible: int
 
 
 # pylint: disable=too-few-public-methods
-class ToggleCollection:
+class ToggleCollection(Loggable):
     "Subclass this class to implement your own collection of feature flags."
 
     def __init__(self, filename: str) -> None:
         """
         Initialize a new collection of feature toggles from a given `.json`
         config file.
 
         :param filename: name of the .json config file
         """
         annotations = self._retrieveAnnotations()
         self._config = self._loadFromJson(filename)
 
         if undeclaredToggles := set(self._config) - set(annotations):
-            # TODO: replace with custom Exception subclass
-            raise ValueError(
-                f"config file has undeclared toggles ({undeclaredToggles})!"
+            raise ToggleException(
+                f"excess toggles [{undeclaredToggles}] in config file!"
             )
 
         if unconfiguredToggles := set(annotations) - set(self._config):
-            raise ValueError(
-                f"toggles without config found ({unconfiguredToggles})!"
+            raise ToggleException(
+                f"unconfigured toggles [{unconfiguredToggles}] in script!"
             )
 
         for toggle, config in self._config.items():
             self._createAttr(toggle, config)
 
     def __str__(self) -> str:
+        "Custom string representation of a collection of feature flags."
         return f"{self._config}"
 
     def _retrieveAnnotations(self) -> Dict[str, Type[object]]:
         "Retrieve the annotations of the toggle collection."
         if not (annotations := getattr(self, "__annotations__", None)):
-            raise ValueError(
-                "valid collections of feature flags must contain at least one"
-                " annotated variable!"
+            raise ToggleException(
+                "valid collection must contain >=1 annotated variables!"
             )
 
         result: Dict[str, Type[object]] = {}
         for attr, attrType in annotations.items():
             if attrType != bool:
-                raise ValueError(
-                    f"feature flag {attr} must be bool, not {attrType}!"
-                )
+                raise ToggleException(f"{attr} must be bool, not {attrType}!")
             # further checks on the attributes present could be done here
             result[attr] = attrType
         return result
 
     def _loadFromJson(self, filename: str) -> Dict[str, LoadedToggle]:
         "Load a collection of toggles from a .json file."
         try:
             with open(filename, "r", encoding="utf-8") as configFile:
                 config = load(configFile)
         except Exception as ex:
-            raise ValueError(f"invalid toggle config file: {filename}") from ex
+            raise ToggleException(f"config file {filename} invalid!") from ex
 
         result: Dict[str, LoadedToggle] = {}
         for toggleName, toggleConfig in config.items():
             # further checks on the loaded configuration could be done here
             result[toggleName] = toggleConfig
         return result
 
     def _createAttr(self, toggle: str, config: LoadedToggle) -> None:
         "Create a toggle instance attribute from a config."
-        flag = FeatureFlag(**config, logger=getLogger(__name__))
+        flag = FeatureFlag(**config, logger=self.logger)
         setattr(self, toggle, flag)
```

