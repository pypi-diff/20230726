# Comparing `tmp/pandana-0.6.1.tar.gz` & `tmp/pandana-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandana-0.6.1.tar", last modified: Wed Mar 17 22:16:48 2021, max compression
+gzip compressed data, was "pandana-0.7.tar", last modified: Wed Jul 26 15:17:04 2023, max compression
```

## Comparing `pandana-0.6.1.tar` & `pandana-0.7.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.594127 pandana-0.6.1/
--rw-r--r--   0 maurer     (501) staff       (20)     2717 2021-03-17 16:56:06.000000 pandana-0.6.1/CHANGELOG.md
--rw-r--r--   0 maurer     (501) staff       (20)     3986 2021-03-17 16:19:53.000000 pandana-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 maurer     (501) staff       (20)    34461 2020-07-19 21:22:24.000000 pandana-0.6.1/LICENSE.txt
--rw-r--r--   0 maurer     (501) staff       (20)      324 2020-08-05 20:45:39.000000 pandana-0.6.1/MANIFEST.in
--rw-r--r--   0 maurer     (501) staff       (20)      784 2021-03-17 22:16:48.594320 pandana-0.6.1/PKG-INFO
--rw-r--r--   0 maurer     (501) staff       (20)     2207 2021-03-17 16:21:35.000000 pandana-0.6.1/README.md
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.572465 pandana-0.6.1/examples/
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.573023 pandana-0.6.1/examples/.ipynb_checkpoints/
--rw-r--r--   0 maurer     (501) staff       (20)   213581 2020-07-28 15:50:06.000000 pandana-0.6.1/examples/.ipynb_checkpoints/Pandana-demo-checkpoint.ipynb
--rw-r--r--   0 maurer     (501) staff       (20)   213286 2021-03-17 16:19:53.000000 pandana-0.6.1/examples/Pandana-demo.ipynb
--rw-r--r--   0 maurer     (501) staff       (20)     1327 2020-07-20 18:27:01.000000 pandana-0.6.1/examples/node_id_checks.py
--rw-r--r--   0 maurer     (501) staff       (20)     2838 2020-11-19 21:50:54.000000 pandana-0.6.1/examples/shortest_path_example.py
--rw-r--r--   0 maurer     (501) staff       (20)     1330 2020-07-19 21:22:24.000000 pandana-0.6.1/examples/simple_example.py
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.577432 pandana-0.6.1/pandana/
--rw-r--r--   0 maurer     (501) staff       (20)       62 2021-03-17 16:21:05.000000 pandana-0.6.1/pandana/__init__.py
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.580128 pandana-0.6.1/pandana/loaders/
--rw-r--r--   0 maurer     (501) staff       (20)        0 2020-07-19 21:22:24.000000 pandana-0.6.1/pandana/loaders/__init__.py
--rw-r--r--   0 maurer     (501) staff       (20)     5672 2020-08-05 20:45:39.000000 pandana-0.6.1/pandana/loaders/osm.py
--rw-r--r--   0 maurer     (501) staff       (20)     2024 2020-07-19 21:22:24.000000 pandana-0.6.1/pandana/loaders/pandash5.py
--rw-r--r--   0 maurer     (501) staff       (20)    31271 2021-02-09 01:03:49.000000 pandana-0.6.1/pandana/network.py
--rw-r--r--   0 maurer     (501) staff       (20)      114 2021-03-17 16:19:53.000000 pandana-0.6.1/pandana/testing.py
--rw-r--r--   0 maurer     (501) staff       (20)      681 2020-07-19 21:22:24.000000 pandana-0.6.1/pandana/utils.py
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.579036 pandana-0.6.1/pandana.egg-info/
--rw-r--r--   0 maurer     (501) staff       (20)      784 2021-03-17 22:16:48.000000 pandana-0.6.1/pandana.egg-info/PKG-INFO
--rw-r--r--   0 maurer     (501) staff       (20)     1391 2021-03-17 22:16:48.000000 pandana-0.6.1/pandana.egg-info/SOURCES.txt
--rw-r--r--   0 maurer     (501) staff       (20)        1 2021-03-17 22:16:48.000000 pandana-0.6.1/pandana.egg-info/dependency_links.txt
--rw-r--r--   0 maurer     (501) staff       (20)      161 2021-03-17 22:16:48.000000 pandana-0.6.1/pandana.egg-info/requires.txt
--rw-r--r--   0 maurer     (501) staff       (20)        8 2021-03-17 22:16:48.000000 pandana-0.6.1/pandana.egg-info/top_level.txt
--rw-r--r--   0 maurer     (501) staff       (20)      132 2020-08-05 20:45:39.000000 pandana-0.6.1/requirements-dev.txt
--rw-r--r--   0 maurer     (501) staff       (20)       79 2020-08-05 20:45:39.000000 pandana-0.6.1/requirements-extras.txt
--rw-r--r--   0 maurer     (501) staff       (20)       94 2021-03-17 22:16:48.594784 pandana-0.6.1/setup.cfg
--rw-r--r--   0 maurer     (501) staff       (20)     5572 2021-03-17 16:44:15.000000 pandana-0.6.1/setup.py
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.586695 pandana-0.6.1/src/
--rw-r--r--   0 maurer     (501) staff       (20)    11954 2021-03-17 16:19:53.000000 pandana-0.6.1/src/accessibility.cpp
--rw-r--r--   0 maurer     (501) staff       (20)     4044 2021-02-09 01:03:49.000000 pandana-0.6.1/src/accessibility.h
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.563132 pandana-0.6.1/src/contraction_hierarchies/
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.588485 pandana-0.6.1/src/contraction_hierarchies/src/
--rw-r--r--   0 maurer     (501) staff       (20)     1722 2020-07-19 21:22:24.000000 pandana-0.6.1/src/contraction_hierarchies/src/BasicDefinitions.h
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.589531 pandana-0.6.1/src/contraction_hierarchies/src/Contractor/
--rw-r--r--   0 maurer     (501) staff       (20)    10871 2020-07-19 21:22:24.000000 pandana-0.6.1/src/contraction_hierarchies/src/Contractor/ContractionCleanup.h
--rw-r--r--   0 maurer     (501) staff       (20)    25877 2020-07-19 21:22:24.000000 pandana-0.6.1/src/contraction_hierarchies/src/Contractor/Contractor.h
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.592353 pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/
--rw-r--r--   0 maurer     (501) staff       (20)     7951 2020-07-19 21:22:24.000000 pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/BinaryHeap.h
--rw-r--r--   0 maurer     (501) staff       (20)     8018 2020-07-19 21:22:24.000000 pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/DynamicGraph.h
--rw-r--r--   0 maurer     (501) staff       (20)     2550 2020-07-19 21:22:24.000000 pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/Percent.h
--rw-r--r--   0 maurer     (501) staff       (20)    11501 2020-07-19 21:22:24.000000 pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/SimpleCHQuery.h
--rw-r--r--   0 maurer     (501) staff       (20)     4794 2020-07-19 21:22:24.000000 pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/StaticGraph.h
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.593099 pandana-0.6.1/src/contraction_hierarchies/src/POIIndex/
--rw-r--r--   0 maurer     (501) staff       (20)    14384 2021-03-17 16:19:53.000000 pandana-0.6.1/src/contraction_hierarchies/src/POIIndex/POIIndex.h
-drwxr-xr-x   0 maurer     (501) staff       (20)        0 2021-03-17 22:16:48.593670 pandana-0.6.1/src/contraction_hierarchies/src/Util/
--rw-r--r--   0 maurer     (501) staff       (20)     2584 2020-12-11 22:10:48.000000 pandana-0.6.1/src/contraction_hierarchies/src/Util/HyperThreading.h
--rw-r--r--   0 maurer     (501) staff       (20)    17252 2021-03-17 16:19:53.000000 pandana-0.6.1/src/contraction_hierarchies/src/libch.cpp
--rw-r--r--   0 maurer     (501) staff       (20)     6951 2020-07-19 21:22:24.000000 pandana-0.6.1/src/contraction_hierarchies/src/libch.h
--rw-r--r--   0 maurer     (501) staff       (20)   409887 2021-02-09 01:10:01.000000 pandana-0.6.1/src/cyaccess.cpp
--rw-r--r--   0 maurer     (501) staff       (20)     6586 2021-02-09 01:03:49.000000 pandana-0.6.1/src/cyaccess.pyx
--rw-r--r--   0 maurer     (501) staff       (20)     3082 2021-03-11 19:14:08.000000 pandana-0.6.1/src/graphalg.cpp
--rw-r--r--   0 maurer     (501) staff       (20)     1257 2020-07-19 21:22:24.000000 pandana-0.6.1/src/graphalg.h
--rw-r--r--   0 maurer     (501) staff       (20)      249 2020-07-19 21:22:24.000000 pandana-0.6.1/src/shared.h
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.831021 pandana-0.7/
+-rw-r--r--   0 maurer     (501) staff       (20)     3168 2023-07-25 22:36:59.000000 pandana-0.7/CHANGELOG.md
+-rw-r--r--   0 maurer     (501) staff       (20)     4079 2022-08-23 21:36:28.000000 pandana-0.7/CONTRIBUTING.md
+-rw-r--r--   0 maurer     (501) staff       (20)    34461 2022-08-23 21:36:28.000000 pandana-0.7/LICENSE.txt
+-rw-r--r--   0 maurer     (501) staff       (20)      324 2022-08-23 21:36:28.000000 pandana-0.7/MANIFEST.in
+-rw-r--r--   0 maurer     (501) staff       (20)      764 2023-07-26 15:17:04.831086 pandana-0.7/PKG-INFO
+-rw-r--r--   0 maurer     (501) staff       (20)     2216 2023-07-25 22:38:07.000000 pandana-0.7/README.md
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.823940 pandana-0.7/examples/
+-rw-r--r--   0 maurer     (501) staff       (20)   213286 2022-08-23 21:36:28.000000 pandana-0.7/examples/Pandana-demo.ipynb
+-rw-r--r--   0 maurer     (501) staff       (20)      887 2023-07-25 21:51:08.000000 pandana-0.7/examples/range_example.py
+-rw-r--r--   0 maurer     (501) staff       (20)     2838 2023-07-25 21:50:07.000000 pandana-0.7/examples/shortest_path_example.py
+-rw-r--r--   0 maurer     (501) staff       (20)     1322 2023-07-25 21:42:08.000000 pandana-0.7/examples/simple_example.py
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.824843 pandana-0.7/pandana/
+-rw-r--r--   0 maurer     (501) staff       (20)       60 2023-07-25 21:45:41.000000 pandana-0.7/pandana/__init__.py
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.825912 pandana-0.7/pandana/loaders/
+-rw-r--r--   0 maurer     (501) staff       (20)        0 2022-08-23 21:36:28.000000 pandana-0.7/pandana/loaders/__init__.py
+-rw-r--r--   0 maurer     (501) staff       (20)     5672 2022-08-23 21:36:28.000000 pandana-0.7/pandana/loaders/osm.py
+-rw-r--r--   0 maurer     (501) staff       (20)     2024 2022-08-23 21:36:28.000000 pandana-0.7/pandana/loaders/pandash5.py
+-rw-r--r--   0 maurer     (501) staff       (20)    34081 2023-07-25 21:49:16.000000 pandana-0.7/pandana/network.py
+-rw-r--r--   0 maurer     (501) staff       (20)      114 2022-08-23 21:36:28.000000 pandana-0.7/pandana/testing.py
+-rw-r--r--   0 maurer     (501) staff       (20)      899 2023-07-25 21:48:28.000000 pandana-0.7/pandana/utils.py
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.825598 pandana-0.7/pandana.egg-info/
+-rw-r--r--   0 maurer     (501) staff       (20)      764 2023-07-26 15:17:04.000000 pandana-0.7/pandana.egg-info/PKG-INFO
+-rw-r--r--   0 maurer     (501) staff       (20)     1453 2023-07-26 15:17:04.000000 pandana-0.7/pandana.egg-info/SOURCES.txt
+-rw-r--r--   0 maurer     (501) staff       (20)        1 2023-07-26 15:17:04.000000 pandana-0.7/pandana.egg-info/dependency_links.txt
+-rw-r--r--   0 maurer     (501) staff       (20)       69 2023-07-26 15:17:04.000000 pandana-0.7/pandana.egg-info/requires.txt
+-rw-r--r--   0 maurer     (501) staff       (20)        8 2023-07-26 15:17:04.000000 pandana-0.7/pandana.egg-info/top_level.txt
+-rw-r--r--   0 maurer     (501) staff       (20)      225 2023-07-25 21:42:08.000000 pandana-0.7/pyproject.toml
+-rw-r--r--   0 maurer     (501) staff       (20)      132 2022-08-23 21:36:28.000000 pandana-0.7/requirements-dev.txt
+-rw-r--r--   0 maurer     (501) staff       (20)       79 2022-08-23 21:36:28.000000 pandana-0.7/requirements-extras.txt
+-rw-r--r--   0 maurer     (501) staff       (20)       94 2023-07-26 15:17:04.831274 pandana-0.7/setup.cfg
+-rw-r--r--   0 maurer     (501) staff       (20)     4148 2023-07-25 22:39:15.000000 pandana-0.7/setup.py
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.828479 pandana-0.7/src/
+-rw-r--r--   0 maurer     (501) staff       (20)    13447 2023-07-25 21:42:08.000000 pandana-0.7/src/accessibility.cpp
+-rw-r--r--   0 maurer     (501) staff       (20)     4175 2023-07-25 21:42:08.000000 pandana-0.7/src/accessibility.h
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.820323 pandana-0.7/src/contraction_hierarchies/
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.828935 pandana-0.7/src/contraction_hierarchies/src/
+-rw-r--r--   0 maurer     (501) staff       (20)     1722 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/BasicDefinitions.h
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.829218 pandana-0.7/src/contraction_hierarchies/src/Contractor/
+-rw-r--r--   0 maurer     (501) staff       (20)    10871 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/Contractor/ContractionCleanup.h
+-rw-r--r--   0 maurer     (501) staff       (20)    25877 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/Contractor/Contractor.h
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.829914 pandana-0.7/src/contraction_hierarchies/src/DataStructures/
+-rw-r--r--   0 maurer     (501) staff       (20)     7951 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/DataStructures/BinaryHeap.h
+-rw-r--r--   0 maurer     (501) staff       (20)     8018 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/DataStructures/DynamicGraph.h
+-rw-r--r--   0 maurer     (501) staff       (20)     2550 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/DataStructures/Percent.h
+-rw-r--r--   0 maurer     (501) staff       (20)    11501 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/DataStructures/SimpleCHQuery.h
+-rw-r--r--   0 maurer     (501) staff       (20)     4794 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/DataStructures/StaticGraph.h
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.830038 pandana-0.7/src/contraction_hierarchies/src/POIIndex/
+-rw-r--r--   0 maurer     (501) staff       (20)    14384 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/POIIndex/POIIndex.h
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.830162 pandana-0.7/src/contraction_hierarchies/src/Util/
+-rw-r--r--   0 maurer     (501) staff       (20)     2584 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/Util/HyperThreading.h
+-rw-r--r--   0 maurer     (501) staff       (20)    17252 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/libch.cpp
+-rw-r--r--   0 maurer     (501) staff       (20)     6951 2022-08-23 21:36:28.000000 pandana-0.7/src/contraction_hierarchies/src/libch.h
+-rw-r--r--   0 maurer     (501) staff       (20)   651537 2023-07-25 19:22:22.000000 pandana-0.7/src/cyaccess.cpp
+-rw-r--r--   0 maurer     (501) staff       (20)     7106 2023-07-25 21:42:08.000000 pandana-0.7/src/cyaccess.pyx
+-rw-r--r--   0 maurer     (501) staff       (20)     3082 2022-08-23 21:36:28.000000 pandana-0.7/src/graphalg.cpp
+-rw-r--r--   0 maurer     (501) staff       (20)     1257 2022-08-23 21:36:28.000000 pandana-0.7/src/graphalg.h
+-rw-r--r--   0 maurer     (501) staff       (20)      249 2022-08-23 21:36:28.000000 pandana-0.7/src/shared.h
+drwxr-xr-x   0 maurer     (501) staff       (20)        0 2023-07-26 15:17:04.830890 pandana-0.7/tests/
+-rw-r--r--   0 maurer     (501) staff       (20)     3542 2023-07-25 21:42:08.000000 pandana-0.7/tests/test_cyaccess.py
+-rw-r--r--   0 maurer     (501) staff       (20)     2408 2023-07-25 21:42:08.000000 pandana-0.7/tests/test_osm.py
+-rw-r--r--   0 maurer     (501) staff       (20)    13589 2023-07-25 21:42:08.000000 pandana-0.7/tests/test_pandana.py
+-rw-r--r--   0 maurer     (501) staff       (20)     4517 2023-07-25 21:42:08.000000 pandana-0.7/tests/test_pandash5.py
+-rw-r--r--   0 maurer     (501) staff       (20)      862 2023-07-25 21:42:08.000000 pandana-0.7/tests/test_utils.py
```

### Comparing `pandana-0.6.1/CHANGELOG.md` & `pandana-0.7/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+v0.7
+====
+
+2023/07/26
+
+* Adds support for calculating accessibility isochrones: which nodes are within x network distance of a source node
+* Allows a maximum distance to be set for POIs
+* Adds a warning when a shortest path is requested between unconnected nodes
+* Supports PyTables 3.7+
+* Support Pandas 2.0
+* Switches to pyproject.toml packaging standards
+* Adds binaries on PyPI to support Python 3.10 and 3.11
+* Improves compilation in MacOS 12+
+
 v0.6.1
 ======
 
 2021/03/17
 
 * Adds support for non-x86 CPUs, including ARM-based Macs
 * Removes accommodations for pre-C++11 compilers
```

### Comparing `pandana-0.6.1/CONTRIBUTING.md` & `pandana-0.7/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 You can contact Sam Maurer, the lead maintainer, at `maurer@urbansim.com`.
 
 
 ## If you have a problem:
 
 - Take a look at the [open issues](https://github.com/UDST/pandana/issues) and [closed issues](https://github.com/UDST/pandana/issues?q=is%3Aissue+is%3Aclosed) to see if there's already a related discussion
 
-- Open a new issue describing the problem -- if possible, include any error messages, the operating system and version of python you're using, and versions of any libraries that may be relevant
+- Open a new issue describing the problem -- if possible, include any error messages, a full reproducible example of the code that generated the error, the operating system and version of python you're using, and versions of any libraries that may be relevant
 
 
 ## Feature proposals:
 
 - Take a look at the [open issues](https://github.com/UDST/pandana/issues) and [closed issues](https://github.com/UDST/pandana/issues?q=is%3Aissue+is%3Aclosed) to see if there's already a related discussion
 
 - Post your proposal as a new issue, so we can discuss it (some proposals may not be a good fit for the project)
@@ -21,15 +21,15 @@
 
 ## Contributing code:
 
 - Create a new branch of `UDST/pandana`, or fork the repository to your own account
 
 - Make your changes, following the existing styles for code and inline documentation
 
-- Add [tests](https://github.com/UDST/urbansim/tree/master/pandana/tests) if possible!
+- Add [tests](https://github.com/UDST/pandana/tree/master/pandana/tests) if possible!
 
 - Open a pull request to the `UDST/pandana` dev branch, including a writeup of your changes -- take a look at some of the closed PR's for examples
 
 - Current maintainers will review the code, suggest changes, and hopefully merge it!
 
 
 ## Updating the documentation: 
@@ -42,15 +42,16 @@
 - Make a new branch for release prep
 
 - Update the version number and changelog
   - `CHANGELOG.md`
   - `setup.py`
   - `pandana/__init__.py`
   - `docs/source/index.rst`
-
+  - `docs/source/conf.py`
+  
 - Make sure all the tests are passing, and check if updates are needed to `README.md` or to the documentation
 
 - Open a pull request to the master branch to finalize it
 
 - After merging, tag the release on GitHub and follow the distribution procedures below
```

### Comparing `pandana-0.6.1/LICENSE.txt` & `pandana-0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/README.md` & `pandana-0.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ### Installation
 
 As of March 2021, binary installers are provided for Mac, Linux, and Windows through both PyPI and Conda Forge. 
 
 - `pip install pandana`
 - `conda install pandana --channel conda-forge`
 
-Pandana works best in Python 3.6+, although binary installers for Python 3.5 remain available on Pip. The last version of Pandana with Python 2.7 binaries is v0.4.4 on Conda Forge.
+Pandana is easiest to install in Python 3.8 to 3.11. The last version of Pandana with Python 2.7 binaries is v0.4.4 on Conda Forge. The last version with Python 3.5 binaries is v0.6 on Pip.
 
 See the documentation for information about other [installation options](http://udst.github.io/pandana/installation.html).
 
 
 ### Demo
 
 [Pandana-demo.ipynb](examples/Pandana-demo.ipynb)
```

### Comparing `pandana-0.6.1/examples/.ipynb_checkpoints/Pandana-demo-checkpoint.ipynb` & `pandana-0.7/examples/Pandana-demo.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998611111111111%*

 * *Differences: {"'cells'": "{22: {'source': {delete: [5, 4]}}}"}*

```diff
@@ -582,17 +582,15 @@
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Then get the routing between the nodes.\n",
                 "- [network.shortest_path()](http://udst.github.io/pandana/network.html#pandana.network.Network.shortest_path)\n",
                 "- [network.shortest_path_length()](http://udst.github.io/pandana/network.html#pandana.network.Network.shortest_path_length)\n",
-                "- [network.shortest_path_lengths()](http://udst.github.io/pandana/network.html#pandana.network.Network.shortest_path_lengths)\n",
-                "\n",
-                "Note that these are only *approximately* the shortest path. Pandana uses a heuristic called [contraction hierarchies](https://en.wikipedia.org/wiki/Contraction_hierarchies) to prioritize trunk routes, similar to e.g. Google Maps. This dramatically improves routing performance."
+                "- [network.shortest_path_lengths()](http://udst.github.io/pandana/network.html#pandana.network.Network.shortest_path_lengths)\n"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "metadata": {},
             "outputs": [
```

### Comparing `pandana-0.6.1/examples/shortest_path_example.py` & `pandana-0.7/examples/shortest_path_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 if len(sys.argv) > 1:
     # allow test file to be passed as an argument
     storef = sys.argv[1]
 else:
     # if no argument provided look for it in the test data
     storef = os.path.normpath(os.path.join(
         os.path.dirname(os.path.abspath(__file__)),
-        '../pandana/tests/osm_sample.h5'))
+        '../tests/osm_sample.h5'))
 
 if not os.path.isfile(storef):
     raise IOError('Could not find test input file: {!r}'.format(storef))
 
 print('Building network from file: {!r}'.format(storef))
 
 store = pd.HDFStore(storef, "r")
@@ -46,37 +46,37 @@
 print()
 
 # Demonstrate shortest path code - the largest connected subgraph here has 477 nodes,
 # per the unit tests
 
 net.set(pd.Series(net.node_ids))
 s = net.aggregate(10000, type='count')
-connected_nodes = s[s==477]
+connected_nodes = s[s == 477]
 
 n = 10000
 nodes_a = np.random.choice(connected_nodes.index, n)
 nodes_b = np.random.choice(connected_nodes.index, n)
 
 print('Shortest path 1:')
 print(nodes_a[0])
 print(nodes_b[0])
 
-print(net.shortest_path(nodes_a[0],nodes_b[0]))
-print(net.shortest_path_length(nodes_a[0],nodes_b[0]))
+print(net.shortest_path(nodes_a[0], nodes_b[0]))
+print(net.shortest_path_length(nodes_a[0], nodes_b[0]))
 
 print('Shortest path 2:')
 print(nodes_a[1])
 print(nodes_b[1])
 
-print(net.shortest_path(nodes_a[1],nodes_b[1]))
-print(net.shortest_path_length(nodes_a[1],nodes_b[1]))
+print(net.shortest_path(nodes_a[1], nodes_b[1]))
+print(net.shortest_path_length(nodes_a[1], nodes_b[1]))
 
 print('Repeat with vectorized calculations:')
-print(net.shortest_paths(nodes_a[0:2],nodes_b[0:2]))
-print(net.shortest_path_lengths(nodes_a[0:2],nodes_b[0:2]))
+print(net.shortest_paths(nodes_a[0:2], nodes_b[0:2]))
+print(net.shortest_path_lengths(nodes_a[0:2], nodes_b[0:2]))
 
 # Performance comparison
 print('Performance comparison for 10k distance calculations:')
 
 t0 = time.time()
 for i in range(n):
     _ = net.shortest_path(nodes_a[i], nodes_b[i])
```

### Comparing `pandana-0.6.1/examples/simple_example.py` & `pandana-0.7/examples/simple_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 if len(sys.argv) > 1:
     # allow test file to be passed as an argument
     storef = sys.argv[1]
 else:
     # if no argument provided look for it in the test data
     storef = os.path.normpath(os.path.join(
         os.path.dirname(os.path.abspath(__file__)),
-        '../pandana/tests/osm_sample.h5'))
+        '../tests/osm_sample.h5'))
 
 if not os.path.isfile(storef):
     raise IOError('Could not find test input file: {!r}'.format(storef))
 
 print('Building network from file: {!r}'.format(storef))
 
 store = pd.HDFStore(storef, "r")
```

### Comparing `pandana-0.6.1/pandana/loaders/osm.py` & `pandana-0.7/pandana/loaders/osm.py`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/pandana/loaders/pandash5.py` & `pandana-0.7/pandana/loaders/pandash5.py`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/pandana/network.py` & `pandana-0.7/pandana/network.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,93 +14,94 @@
     This function was previously used to reserve memory space for multiple
     graphs. It is no longer needed in Pandana 0.4+, and will be removed in a
     future version.
 
     Parameters
     ----------
     num : int
-        Number of graph to be reserved in memory
+        Number of graphs to be reserved in memory
 
     """
     warnings.warn(
         "Function reserve_num_graphs() is no longer needed in Pandana 0.4+\
          and will be removed in a future version",
-        DeprecationWarning
+        DeprecationWarning,
     )
     return None
 
 
 class Network:
     """
     Create the transportation network in the city.  Typical data would be
     distance based from OpenStreetMap or travel time from GTFS transit data.
 
     Parameters
     ----------
-    node_x : Pandas Series, float
+    node_x : pandas.Series, float
         Defines the x attribute for nodes in the network (e.g. longitude)
-    node_y : Pandas Series, float
+    node_y : pandas.Series, float
         Defines the y attribute for nodes in the network (e.g. latitude)
         This param and the one above should have the *same* index which
         should be the node_ids that are referred to in the edges below.
-    edge_from : Pandas Series, int
-        Defines the node id that begins an edge - should refer to the index
+    edge_from : pandas.Series, int
+        Defines the node ID that begins an edge - should refer to the index
         of the two series objects above
-    edge_to : Pandas Series, int
-        Defines the node id that ends an edge - should refer to the index
+    edge_to : pandas.Series, int
+        Defines the node ID that ends an edge - should refer to the index
         of the two series objects above
-    edge_weights : Pandas DataFrame, all numerics
+    edge_weights : pandas.DataFrame, all numerics
         Specifies one or more *impedances* on the network which define the
         distances between nodes.  Multiple impedances can be used to
         capture travel times at different times of day, for instance
     twoway : boolean, optional
         Whether the edges in this network are two way edges or one way (
         where the one direction is directed from the from node to the to
-        node). If twoway = True, it is assumed that the from and to id in the
+        node). If twoway = True, it is assumed that the from and to ID in the
         edge table occurs once and that travel can occur in both directions
         on the single edge record. Pandana will internally flip and append
-        the from and to ids to the original edges to create a two direction
+        the from and to IDs to the original edges to create a two direction
         network. If twoway = False, it is assumed that travel can only occur
-        in the explicit direction indicated by the from and to id in the edge
+        in the explicit direction indicated by the from and to ID in the edge
         table.
 
     """
 
-    def __init__(self, node_x, node_y, edge_from, edge_to, edge_weights,
-                 twoway=True):
-        nodes_df = pd.DataFrame({'x': node_x, 'y': node_y})
-        edges_df = pd.DataFrame({'from': edge_from, 'to': edge_to}).\
-            join(edge_weights)
+    def __init__(self, node_x, node_y, edge_from, edge_to, edge_weights, twoway=True):
+        nodes_df = pd.DataFrame({"x": node_x, "y": node_y})
+        edges_df = pd.DataFrame({"from": edge_from, "to": edge_to}).join(edge_weights)
 
         self.nodes_df = nodes_df
         self.edges_df = edges_df
 
         self.impedance_names = list(edge_weights.columns)
         self.variable_names = set()
         self.poi_category_names = []
         self.poi_category_indexes = {}
 
-        # this maps ids to indexes which are used internally
+        # this maps IDs to indexes which are used internally
         # this is a constant source of headaches, but all node identifiers
         # in the c extension are actually indexes ordered from 0 to numnodes-1
-        # node ids are thus translated back and forth in the python layer, which
-        # allows non-integer node ids as well
-        self.node_idx = pd.Series(np.arange(len(nodes_df), dtype="int"),
-                                  index=nodes_df.index)
-
-        edges = pd.concat([self._node_indexes(edges_df["from"]),
-                           self._node_indexes(edges_df["to"])], axis=1)
-
-        self.net = cyaccess(self.node_idx.values,
-                            nodes_df.astype('double').values,
-                            edges.values,
-                            edges_df[edge_weights.columns].transpose()
-                                                          .astype('double')
-                                                          .values,
-                            twoway)
+        # node IDs are thus translated back and forth in the python layer,
+        # which allows non-integer node IDs as well
+        self.node_idx = pd.Series(
+            np.arange(len(nodes_df), dtype="int"), index=nodes_df.index
+        )
+
+        edges = pd.concat(
+            [self._node_indexes(edges_df["from"]), self._node_indexes(edges_df["to"])],
+            axis=1,
+        )
+
+        self.net = cyaccess(
+            self.node_idx.values,
+            nodes_df.astype("double").values,
+            edges.values,
+            edges_df[edge_weights.columns].transpose().astype("double").values,
+            twoway,
+        )
 
         self._twoway = twoway
 
         self.kdtree = KDTree(nodes_df.values)
 
     @classmethod
     def from_hdf5(cls, filename):
@@ -133,55 +134,61 @@
             be saved as part of the Network.
 
         """
         ph5.network_to_pandas_hdf5(self, filename, rm_nodes)
 
     def _node_indexes(self, node_ids):
         # for some reason, merge is must faster than .loc
-        df = pd.merge(pd.DataFrame({"node_ids": node_ids}),
-                      pd.DataFrame({"node_idx": self.node_idx}),
-                      left_on="node_ids",
-                      right_index=True,
-                      how="left")
+        df = pd.merge(
+            pd.DataFrame({"node_ids": node_ids}),
+            pd.DataFrame({"node_idx": self.node_idx}),
+            left_on="node_ids",
+            right_index=True,
+            how="left",
+        )
         return df.node_idx
 
     @property
     def aggregations(self):
         return self.net.get_available_aggregations()
 
     @property
     def decays(self):
         return self.net.get_available_decays()
 
     @property
     def node_ids(self):
         """
-        The node ids which will be used as the index of many return series
+        The node IDs which will be used as the index of many return series
         """
         return self.node_idx.index
 
     @property
     def bbox(self):
         """
         The bounding box for nodes in this network [xmin, ymin, xmax, ymax]
         """
-        return [self.nodes_df.x.min(), self.nodes_df.y.min(),
-                self.nodes_df.x.max(), self.nodes_df.y.max()]
+        return [
+            self.nodes_df.x.min(),
+            self.nodes_df.y.min(),
+            self.nodes_df.x.max(),
+            self.nodes_df.y.max(),
+        ]
 
     def shortest_path(self, node_a, node_b, imp_name=None):
         """
-        Return the shortest path between two node ids in the network. Must
+        Return the shortest path between two node IDs in the network. Must
         provide an impedance name if more than one is available.
 
         Parameters
         ----------
         node_a : int
-            Source node id
+            Source node ID
         node_b : int
-            Destination node id
+            Destination node ID
         imp_name : string, optional
             The impedance name to use for the shortest path
 
         Returns
         -------
         path : np.ndarray
             Nodes that are traversed in the shortest path
@@ -192,73 +199,76 @@
         node_a = node_idx.iloc[0]
         node_b = node_idx.iloc[1]
 
         imp_num = self._imp_name_to_num(imp_name)
 
         path = self.net.shortest_path(node_a, node_b, imp_num)
 
-        # map back to external node ids
+        # map back to external node IDs
         return self.node_ids.values[path]
 
     def shortest_paths(self, nodes_a, nodes_b, imp_name=None):
         """
         Vectorized calculation of shortest paths. Accepts a list of origins
         and list of destinations and returns a corresponding list of
         shortest path routes. Must provide an impedance name if more than
         one is available.
 
         Added in Pandana v0.6.
 
         Parameters
         ----------
         nodes_a : list-like of ints
-            Source node ids
+            Source node IDs
         nodes_b : list-like of ints
-            Corresponding destination node ids
+            Corresponding destination node IDs
         imp_name : string
             The impedance name to use for the shortest path
 
         Returns
         -------
         paths : list of np.ndarray
             Nodes traversed in each shortest path
 
         """
         if len(nodes_a) != len(nodes_b):
-            raise ValueError("Origin and destination counts don't match: {}, {}"
-                             .format(len(nodes_a), len(nodes_b)))
+            raise ValueError(
+                "Origin and destination counts don't match: {}, {}".format(
+                    len(nodes_a), len(nodes_b)
+                )
+            )
 
         # map to internal node indexes
         nodes_a_idx = self._node_indexes(pd.Series(nodes_a)).values
         nodes_b_idx = self._node_indexes(pd.Series(nodes_b)).values
 
         imp_num = self._imp_name_to_num(imp_name)
 
         paths = self.net.shortest_paths(nodes_a_idx, nodes_b_idx, imp_num)
 
         # map back to external node ids
         return [self.node_ids.values[p] for p in paths]
 
     def shortest_path_length(self, node_a, node_b, imp_name=None):
         """
-        Return the length of the shortest path between two node ids in the
+        Return the length of the shortest path between two node IDs in the
         network. Must provide an impedance name if more than one is
         available.
 
         If you have a large number of paths to calculate, don't use this
         function! Use the vectorized one instead.
 
         Added in Pandana v0.5.
 
         Parameters
         ----------
         node_a : int
-            Source node id
+            Source node ID
         node_b : int
-            Destination node id
+            Destination node ID
         imp_name : string
             The impedance name to use for the shortest path
 
         Returns
         -------
         length : float
 
@@ -268,64 +278,80 @@
         node_a = node_idx.iloc[0]
         node_b = node_idx.iloc[1]
 
         imp_num = self._imp_name_to_num(imp_name)
 
         len = self.net.shortest_path_distance(node_a, node_b, imp_num)
 
+        if len == 4294967.295:
+            warnings.warn(
+                "Unsigned integer: shortest path distance is trying to be calculated between\
+                external %s and %s unconntected nodes" % (node_a, node_b)
+            )
+
         return len
 
     def shortest_path_lengths(self, nodes_a, nodes_b, imp_name=None):
         """
         Vectorized calculation of shortest path lengths. Accepts a list of
         origins and list of destinations and returns a corresponding list
         of shortest path lengths. Must provide an impedance name if more
         than one is available.
 
         Added in Pandana v0.5.
 
         Parameters
         ----------
         nodes_a : list-like of ints
-            Source node ids
+            Source node IDs
         nodes_b : list-like of ints
-            Corresponding destination node ids
+            Corresponding destination node IDs
         imp_name : string
             The impedance name to use for the shortest path
 
         Returns
         -------
-        lenths : list of floats
+        lengths : list of floats
 
         """
         if len(nodes_a) != len(nodes_b):
-            raise ValueError("Origin and destination counts don't match: {}, {}"
-                             .format(len(nodes_a), len(nodes_b)))
+            raise ValueError(
+                "Origin and destination counts don't match: {}, {}".format(
+                    len(nodes_a), len(nodes_b)
+                )
+            )
 
         # map to internal node indexes
         nodes_a_idx = self._node_indexes(pd.Series(nodes_a)).values
         nodes_b_idx = self._node_indexes(pd.Series(nodes_b)).values
 
         imp_num = self._imp_name_to_num(imp_name)
 
         lens = self.net.shortest_path_distances(nodes_a_idx, nodes_b_idx, imp_num)
 
+        if 4294967.295 in lens:
+            unconnected_idx = [i for i, v in enumerate(lens) if v == 4294967.295]
+            unconnected_nodes = [(nodes_a[i], nodes_b[i]) for i in unconnected_idx]
+            warnings.warn(
+                "Unsigned integer: shortest path distance is trying to be calculated \
+                between the following external unconnected nodes: %s" % (unconnected_nodes))
+
         return lens
 
     def set(self, node_ids, variable=None, name="tmp"):
         """
         Characterize urban space with a variable that is related to nodes in
         the network.
 
         Parameters
         ----------
-        node_ids : Pandas Series, int
+        node_ids : pandas.Series, int
             A series of node_ids which are usually computed using
             get_node_ids on this object.
-        variable : Pandas Series, numeric, optional
+        variable : pandas.Series, numeric, optional
             A series which represents some variable defined in urban space.
             It could be the location of buildings, or the income of all
             households - just about anything can be aggregated using the
             network queries provided here and this provides the api to set
             the variable at its disaggregate locations.  Note that node_id
             and variable should have the same index (although the index is
             not actually used).  If variable is not set, then it is assumed
@@ -345,31 +371,31 @@
         Returns
         -------
         Nothing
 
         """
         if variable is None:
             variable = pd.Series(np.ones(len(node_ids)), index=node_ids.index)
-
-        df = pd.DataFrame({name: variable,
-                           "node_idx": self._node_indexes(node_ids)})
+        df = pd.DataFrame({name: variable, "node_idx": self._node_indexes(node_ids)})
 
         length = len(df)
         df = df.dropna(how="any")
         newl = len(df)
-        if length-newl > 0:
+        if length - newl > 0:
             print(
-                "Removed %d rows because they contain missing values" %
-                (length-newl))
+                "Removed %d rows because they contain missing values" % (length - newl)
+            )
 
         self.variable_names.add(name)
 
-        self.net.initialize_access_var(name.encode('utf-8'),
-                                       df.node_idx.values.astype('int'),
-                                       df[name].values.astype('double'))
+        self.net.initialize_access_var(
+            name.encode("utf-8"),
+            df.node_idx.values.astype("int"),
+            df[name].values.astype("double"),
+        )
 
     def precompute(self, distance):
         """
         Precomputes the range queries (the reachable nodes within this
         maximum distance.  So as long as you use a smaller distance, cached
         results will be used.)
 
@@ -382,27 +408,75 @@
 
         Returns
         -------
         Nothing
         """
         self.net.precompute_range(distance)
 
+    def nodes_in_range(self, nodes, radius, imp_name=None):
+        """
+        Computes the range queries (the reachable nodes within this maximum
+        distance) for each input node.
+
+        Parameters
+        ----------
+        nodes : list-like of ints
+            Source node IDs
+        radius : float
+            Maximum distance to use. This will usually be a distance unit in
+            meters however if you have customized the impedance (using the
+            imp_name option) this could be in other units such as utility or
+            time etc.
+        imp_name : string, optional
+            The impedance name to use for the aggregation on this network.
+            Must be one of the impedance names passed in the constructor of
+            this object.  If not specified, there must be only one impedance
+            passed in the constructor, which will be used.
+
+        Returns
+        -------
+        d : pandas.DataFrame
+            Like nearest_pois, this is a dataframe containing the input node
+            index, the index of the nearby nodes within the search radius,
+            and the distance (according to the requested impedance) from the
+            source to the nearby node.
+        """
+        imp_num = self._imp_name_to_num(imp_name)
+        imp_name = self.impedance_names[imp_num]
+        ext_ids = self.node_idx.index.values
+
+        raw_result = self.net.nodes_in_range(nodes, radius, imp_num, ext_ids)
+        clean_result = pd.concat(
+            [
+                pd.DataFrame(r, columns=["destination", imp_name]).assign(source=ix)
+                for r, ix in zip(raw_result, nodes)
+            ]
+        )[["source", "destination", imp_name]]
+        return (
+            clean_result.drop_duplicates(subset=["source", "destination"])
+            .reset_index(drop=True)
+            .query("{} <= {}".format(imp_name, radius))
+        )
+
     def _imp_name_to_num(self, imp_name):
         if imp_name is None:
-            assert len(self.impedance_names) == 1,\
-                "must pass impedance name if there are multiple impedances set"
+            assert (
+                len(self.impedance_names) == 1
+            ), "must pass impedance name if there are multiple impedances set"
             imp_name = self.impedance_names[0]
 
-        assert imp_name in self.impedance_names, "An impedance with that name" \
-                                                 "was not found"
+        assert imp_name in self.impedance_names, (
+            "An impedance with that name" "was not found"
+        )
 
         return self.impedance_names.index(imp_name)
 
-    def aggregate(self, distance, type="sum", decay="linear", imp_name=None,
-                  name="tmp"):
+    def aggregate(
+        self, distance, type="sum", decay="linear", imp_name=None, name="tmp"
+    ):
         """
         Aggregate information for every source node in the network - this is
         really the main purpose of this library.  This allows you to touch
         the data specified by calling set and perform some aggregation on it
         within the specified distance.  For instance, summing the population
         within 1000 meters.
 
@@ -442,94 +516,103 @@
             The variable to aggregate.  This variable will have been created
             and named by a call to ``set``.  If not specified, the default
             variable name will be used so that the most recent call to set
             without giving a name will be the variable used.
 
         Returns
         -------
-        agg : Pandas Series
+        agg : pandas.Series
             Returns a Pandas Series for every origin node in the network,
             with the index which is the same as the node_ids passed to the
             init method and the values are the aggregations for each source
             node in the network.
         """
 
         imp_num = self._imp_name_to_num(imp_name)
         type = type.lower()
 
         # Resolve aliases
-        if type in ['ave', 'avg', 'average']:
-            type = 'mean'
+        if type in ["ave", "avg", "average"]:
+            type = "mean"
 
-        if type in ['stddev']:
-            type = 'std'
+        if type in ["stddev"]:
+            type = "std"
 
-        if type in ['med']:
-            type = 'median'
+        if type in ["med"]:
+            type = "median"
+
+        assert name in self.variable_names, (
+            "A variable with that name " "has not yet been initialized"
+        )
 
-        assert name in self.variable_names, "A variable with that name " \
-                                            "has not yet been initialized"
-
-        res = self.net.get_all_aggregate_accessibility_variables(distance,
-                                                                 name.encode('utf-8'),
-                                                                 type.encode('utf-8'),
-                                                                 decay.encode('utf-8'),
-                                                                 imp_num)
+        res = self.net.get_all_aggregate_accessibility_variables(
+            distance,
+            name.encode("utf-8"),
+            type.encode("utf-8"),
+            decay.encode("utf-8"),
+            imp_num,
+        )
 
         return pd.Series(res, index=self.node_ids)
 
     def get_node_ids(self, x_col, y_col, mapping_distance=None):
         """
         Assign node_ids to data specified by x_col and y_col.
 
         Parameters
         ----------
-        x_col : Pandas series (float)
+        x_col : pandas.Series (float)
             A Pandas Series where values specify the x (e.g. longitude)
             location of dataset.
-        y_col : Pandas series (float)
+        y_col : pandas.Series (float)
             A Pandas Series where values specify the y (e.g. latitude)
             location of dataset.  x_col and y_col should use the same index.
         mapping_distance : float, optional
             The maximum distance that will be considered a match between the
             x, y data and the nearest node in the network.  This will usually
             be a distance unit in meters however if you have customized the
             impedance this could be in other units such as utility or time
             etc. If not specified, every x, y coordinate will be mapped to
             the nearest node.
 
         Returns
         -------
-        node_ids : Pandas series (int)
+        node_ids : pandas.Series (int)
             Returns a Pandas Series of node_ids for each x, y in the
             input data. The index is the same as the indexes of the
             x, y input data, and the values are the mapped node_ids.
             If mapping distance is not passed and if there are no nans in the
             x, y data, this will be the same length as the x, y data.
             If the mapping is imperfect, this function returns all the
             input x, y's that were successfully mapped to node_ids.
         """
-        xys = pd.DataFrame({'x': x_col, 'y': y_col})
+        xys = pd.DataFrame({"x": x_col, "y": y_col})
 
         distances, indexes = self.kdtree.query(xys.values)
         indexes = np.transpose(indexes)[0]
         distances = np.transpose(distances)[0]
 
         node_ids = self.nodes_df.iloc[indexes].index
 
-        df = pd.DataFrame({"node_id": node_ids, "distance": distances},
-                          index=xys.index)
+        df = pd.DataFrame({"node_id": node_ids, "distance": distances}, index=xys.index)
 
         if mapping_distance is not None:
             df = df[df.distance <= mapping_distance]
 
         return df.node_id
 
-    def plot(self, data, bbox=None, plot_type='scatter', fig_kwargs=None,
-             plot_kwargs=None, cbar_kwargs=None):
+    def plot(
+        self,
+        data,
+        bbox=None,
+        plot_type="scatter",
+        fig_kwargs=None,
+        plot_kwargs=None,
+        cbar_kwargs=None,
+    ):
         """
         Plot an array of data on a map using Matplotlib, automatically matching
         the data to the Pandana network node positions. Keyword arguments are
         passed to the plotting routine.
 
         Modified in Pandana v0.6 to eliminate usage of Matplotlib's deprecated
         Basemap toolkit. No longer accepts bmap_kwargs and no longer returns
@@ -566,207 +649,224 @@
 
         try:
             import matplotlib
             import matplotlib.pyplot as plt
         except (ModuleNotFoundError, RuntimeError):
             raise ModuleNotFoundError("Pandana's network.plot() requires Matplotlib")
 
-        fig_kwargs = fig_kwargs or {'figsize': (10, 8)}
-        plot_kwargs = plot_kwargs or {'cmap': 'hot_r', 's': 1}
+        fig_kwargs = fig_kwargs or {"figsize": (10, 8)}
+        plot_kwargs = plot_kwargs or {"cmap": "hot_r", "s": 1}
         cbar_kwargs = cbar_kwargs or {}
 
         if not bbox:
             bbox = (
                 self.nodes_df.y.min(),
                 self.nodes_df.x.min(),
                 self.nodes_df.y.max(),
-                self.nodes_df.x.max())
+                self.nodes_df.x.max(),
+            )
 
         fig, ax = plt.subplots(**fig_kwargs)
 
         x, y = (self.nodes_df.x.values, self.nodes_df.y.values)
 
-        if plot_type == 'scatter':
-            plot = plt.scatter(
-                x, y, c=data.values, **plot_kwargs)
-        elif plot_type == 'hexbin':
-            plot = plt.hexbin(
-                x, y, C=data.values, **plot_kwargs)
+        if plot_type == "scatter":
+            plot = plt.scatter(x, y, c=data.values, **plot_kwargs)
+        elif plot_type == "hexbin":
+            plot = plt.hexbin(x, y, C=data.values, **plot_kwargs)
 
         colorbar = plt.colorbar(plot, **cbar_kwargs)
 
         plt.show()
 
         return fig, ax
 
     def init_pois(self, num_categories, max_dist, max_pois):
         """
-        Initialize the point of interest infrastructure. This is no longer
-        needed in Pandana 0.4+ and will be removed in a future version.
+        Initialize the point of interest (POI) infrastructure.
+        This is no longer needed in Pandana 0.4+ and will be removed in a
+        future version.
 
         Parameters
         ----------
         num_categories : int
             Number of categories of POIs
         max_dist : float
             Maximum distance that will be tested to nearest POIs. This will
             usually be a distance unit in meters however if you have
             customized the impedance this could be in other
             units such as utility or time etc.
-        max_pois :
+        max_pois : int
             Maximum number of POIs to return in the nearest query
 
         """
         self.num_categories = num_categories
         self.max_dist = max_dist
         self.max_pois = max_pois
         warnings.warn(
             "Method init_pois() is no longer needed in Pandana 0.4+ and will be removed in a \
             future version; maxdist and maxitems should now be passed to set_pois()",
-            DeprecationWarning
+            DeprecationWarning,
         )
         return None
 
-    def set_pois(self, category=None, maxdist=None, maxitems=None, x_col=None, y_col=None):
+    def set_pois(self, category=None, maxdist=None, maxitems=None, x_col=None, y_col=None,
+                 mapping_distance=None):
         """
-        Set the location of all the pois of this category. The pois are
-        connected to the closest node in the Pandana network which assumes
-        no impedance between the location of the variable and the location
-        of the closest network node.
+        Set the location of all the points of interest (POIs) of this category.
+         The POIs are connected to the closest node in the Pandana network
+         which assumes no impedance between the location of the variable and
+         the location of the closest network node.
 
         Parameters
         ----------
         category : string
-            The name of the category for this set of pois
-        maxdist - the maximum distance that will later be used in
-            find_all_nearest_pois
-        maxitems - the maximum number of items that will later be requested
-            in find_all_nearest_pois
-        x_col : Pandas Series (float)
-            The x location (longitude) of pois in this category
-        y_col : Pandas Series (Float)
-            The y location (latitude) of pois in this category
+            The name of the category for this set of POIs
+        maxdist : float
+            The maximum distance that will later be used in
+            find_all_nearest_pois()
+        maxitems : int
+            The maximum number of items that will later be requested
+            in find_all_nearest_pois()
+        x_col : pandas.Series (float)
+            The x location (longitude) of POIs in this category
+        y_col : pandas.Series (float)
+            The y location (latitude) of POIs in this category
+        mapping_distance : float, optional
+            The maximum distance that will be considered a match between the
+            POIs and the nearest node in the network.  This will usually
+            be a distance unit in meters however if you have customized the
+            impedance this could be in other units such as utility or time
+            etc. If not specified, every POI will be mapped to
+            the nearest node.
 
         Returns
         -------
         Nothing
 
         """
         # condition to check if missing arguments for keyword arguments using set_pois() from v0.3
         if maxitems is None:
-            print('Reading parameters from init_pois()')
+            print("Reading parameters from init_pois()")
             maxitems = self.max_pois
 
         # condition to check for positional arguments in set_pois() from v0.3
         elif isinstance(maxitems, type(pd.Series())):
             y_col = maxitems
             maxitems = self.max_pois
 
         if maxdist is None:
-            print('Reading parameters from init_pois()')
+            print("Reading parameters from init_pois()")
             maxdist = self.max_dist
 
         elif isinstance(maxdist, type(pd.Series())):
             x_col = maxdist
             maxdist = self.max_dist
 
         if category not in self.poi_category_names:
             self.poi_category_names.append(category)
 
         self.max_pois = maxitems
 
-        node_ids = self.get_node_ids(x_col, y_col)
+        node_ids = self.get_node_ids(x_col, y_col, mapping_distance=mapping_distance)
 
         self.poi_category_indexes[category] = node_ids.index
 
         node_idx = self._node_indexes(node_ids)
 
-        self.net.initialize_category(maxdist, maxitems, category.encode('utf-8'), node_idx.values)
+        self.net.initialize_category(
+            maxdist, maxitems, category.encode("utf-8"), node_idx.values
+        )
 
-    def nearest_pois(self, distance, category, num_pois=1, max_distance=None,
-                     imp_name=None, include_poi_ids=False):
+    def nearest_pois(
+        self,
+        distance,
+        category,
+        num_pois=1,
+        max_distance=None,
+        imp_name=None,
+        include_poi_ids=False,
+    ):
         """
-        Find the distance to the nearest pois from each source node.  The
-        bigger values in this case mean less accessibility.
+        Find the distance to the nearest points of interest (POI)s from each
+        source node.  The bigger values in this case mean less accessibility.
 
         Parameters
         ----------
         distance : float
-            The maximum distance to look for pois. This will usually be a
+            The maximum distance to look for POIs. This will usually be a
             distance unit in meters however if you have customized the
             impedance this could be in other units such as utility or time
             etc.
         category : string
-            The name of the category of poi to look for
+            The name of the category of POI to look for
         num_pois : int
-            The number of pois to look for, this also sets the number of
+            The number of POIs to look for, this also sets the number of
             columns in the DataFrame that gets returned
         max_distance : float, optional
-            The value to set the distance to if there is NO poi within the
+            The value to set the distance to if there is no POI within the
             specified distance - if not specified, gets set to distance. This
             will usually be a distance unit in meters however if you have
             customized the impedance this could be in other units such as
             utility or time etc.
         imp_name : string, optional
             The impedance name to use for the aggregation on this network.
             Must be one of the impedance names passed in the constructor of
             this object.  If not specified, there must be only one impedance
             passed in the constructor, which will be used.
         include_poi_ids : bool, optional
             If this flag is set to true, the call will add columns to the
             return DataFrame - instead of just returning the distance for
             the nth POI, it will also return the id of that POI.  The names
-            of the columns with the poi ids will be poi1, poi2, etc - it
-            will take roughly twice as long to include these ids as to not
+            of the columns with the POI IDs will be poi1, poi2, etc - it
+            will take roughly twice as long to include these IDs as to not
             include them
 
         Returns
         -------
-        d : Pandas DataFrame
+        d : pandas.DataFrame
             Like aggregate, this series has an index of all the node ids for
             the network.  Unlike aggregate, this method returns a dataframe
             with the number of columns equal to the distances to the Nth
-            closest poi.  For instance, if you ask for the 10 closest poi to
-            each node, column d[1] wil be the distance to the 1st closest poi
+            closest POI.  For instance, if you ask for the 10 closest poi to
+            each node, column d[1] wil be the distance to the 1st closest POI
             of that category while column d[2] will be the distance to the 2nd
-            closest poi, and so on.
+            closest POI, and so on.
         """
         if max_distance is None:
             max_distance = distance
 
         if category not in self.poi_category_names:
             assert 0, "Need to call set_pois for this category"
 
         if num_pois > self.max_pois:
-            assert 0, "Asking for more pois than set in init_pois"
+            assert 0, "Asking for more POIs than set in init_pois"
 
         imp_num = self._imp_name_to_num(imp_name)
 
         dists, poi_ids = self.net.find_all_nearest_pois(
-            distance,
-            num_pois,
-            category.encode('utf-8'),
-            imp_num)
+            distance, num_pois, category.encode("utf-8"), imp_num
+        )
         dists[dists == -1] = max_distance
 
         df = pd.DataFrame(dists, index=self.node_ids)
-        df.columns = list(range(1, num_pois+1))
+        df.columns = list(range(1, num_pois + 1))
 
         if include_poi_ids:
             df2 = pd.DataFrame(poi_ids, index=self.node_ids)
-            df2.columns = ["poi%d" % i for i in range(1, num_pois+1)]
+            df2.columns = ["poi%d" % i for i in range(1, num_pois + 1)]
             for col in df2.columns:
                 # if this is still all working according to plan at this point
                 # the great magic trick is now to turn the integer position of
                 # the poi, which is painstakingly returned from the c++ code,
                 # and turn it into the actual index that was used when it was
-                # initialized as a pandas series - this really is pandas-like
+                # initialized as a pandas.Series - this really is pandas-like
                 # thinking.  it's complicated on the inside, but quite
                 # intuitive to the user I think
-                s = df2[col].astype('int')
+                s = df2[col].astype("int")
                 df2[col] = self.poi_category_indexes[category].values[s]
                 df2.loc[s == -1, col] = np.nan
 
             df = pd.concat([df, df2], axis=1)
 
         return df
 
@@ -795,14 +895,13 @@
         Returns
         -------
         node_ids : array
             List of "low connectivity" node IDs.
 
         """
         # set a counter variable on all nodes
-        self.set(self.node_ids.to_series(), name='counter')
+        self.set(self.node_ids.to_series(), name="counter")
 
         # count nodes within impedance range
-        agg = self.aggregate(
-            impedance, type='count', imp_name=imp_name, name='counter')
+        agg = self.aggregate(impedance, type="count", imp_name=imp_name, name="counter")
 
         return np.array(agg[agg < count].index)
```

### Comparing `pandana-0.6.1/pandana.egg-info/SOURCES.txt` & `pandana-0.7/pandana.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 CHANGELOG.md
 CONTRIBUTING.md
 LICENSE.txt
 MANIFEST.in
 README.md
+pyproject.toml
 requirements-dev.txt
 requirements-extras.txt
 setup.cfg
 setup.py
 examples/Pandana-demo.ipynb
-examples/node_id_checks.py
+examples/range_example.py
 examples/shortest_path_example.py
 examples/simple_example.py
-examples/.ipynb_checkpoints/Pandana-demo-checkpoint.ipynb
 pandana/__init__.py
 pandana/network.py
 pandana/testing.py
 pandana/utils.py
 pandana.egg-info/PKG-INFO
 pandana.egg-info/SOURCES.txt
 pandana.egg-info/dependency_links.txt
@@ -38,8 +38,13 @@
 src/contraction_hierarchies/src/Contractor/Contractor.h
 src/contraction_hierarchies/src/DataStructures/BinaryHeap.h
 src/contraction_hierarchies/src/DataStructures/DynamicGraph.h
 src/contraction_hierarchies/src/DataStructures/Percent.h
 src/contraction_hierarchies/src/DataStructures/SimpleCHQuery.h
 src/contraction_hierarchies/src/DataStructures/StaticGraph.h
 src/contraction_hierarchies/src/POIIndex/POIIndex.h
-src/contraction_hierarchies/src/Util/HyperThreading.h
+src/contraction_hierarchies/src/Util/HyperThreading.h
+tests/test_cyaccess.py
+tests/test_osm.py
+tests/test_pandana.py
+tests/test_pandash5.py
+tests/test_utils.py
```

### Comparing `pandana-0.6.1/src/accessibility.cpp` & `pandana-0.7/src/accessibility.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #include "accessibility.h"
 #include <algorithm>
 #include <cmath>
 #include <functional>
+#include <unordered_map>
 #include <utility>
 #include "graphalg.h"
 
 namespace MTC {
 namespace accessibility {
 
 using std::string;
@@ -77,14 +78,56 @@
         }
     }
     }
     dmsradius = radius;
 }
 
 
+vector<vector<pair<long, float>>>
+Accessibility::Range(vector<long> srcnodes, float radius, int graphno, 
+                     vector<long> ext_ids) {
+
+    // Set up a mapping between the external node ids and internal ones
+    std::unordered_map<long, int> int_ids(ext_ids.size());
+    for (int i = 0; i < ext_ids.size(); i++) {
+        int_ids.insert(pair<long, int>(ext_ids[i], i));
+    }
+    
+    // use cached results if available
+    vector<DistanceVec> dists(srcnodes.size());
+    if (dmsradius > 0 && radius <= dmsradius) {
+        for (int i = 0; i < srcnodes.size(); i++) {
+            dists[i] = dms[graphno][int_ids[srcnodes[i]]];
+        }
+    }
+    else {
+        #pragma omp parallel
+        #pragma omp for schedule(guided)
+        for (int i = 0; i < srcnodes.size(); i++) {
+            ga[graphno]->Range(int_ids[srcnodes[i]], radius,
+                omp_get_thread_num(), dists[i]);
+        }
+    }
+    
+    // todo: check that results are returned from cache correctly
+    // todo: check that performing an aggregation creates cache
+
+    // Convert back to external node ids
+    vector<vector<pair<long, float>>> output(dists.size());
+    for (int i = 0; i < dists.size(); i++) {
+        output[i].resize(dists[i].size());
+        for (int j = 0; j < dists[i].size(); j++) {
+            output[i][j] = std::make_pair(ext_ids[dists[i][j].first], 
+                                          dists[i][j].second);
+        }
+    }
+    return output;
+}
+
+
 vector<int>
 Accessibility::Route(int src, int tgt, int graphno) {
     vector<NodeID> ret = this->ga[graphno]->Route(src, tgt);
     return vector<int> (ret.begin(), ret.end());
 }
```

### Comparing `pandana-0.6.1/src/accessibility.h` & `pandana-0.7/src/accessibility.h`

 * *Files 3% similar despite different names*

```diff
@@ -41,23 +41,24 @@
     getAllAggregateAccessibilityVariables(
         float radius,
         string index,
         string aggtyp,
         string decay,
         int graphno = 0);
 
-    // get nodes with the range
-    DistanceVec Range(int srcnode, float radius, int graphno = 0);
+    // get nodes with a range for a specific list of source nodes
+    vector<vector<pair<long, float>>> Range(vector<long> srcnodes, float radius, 
+                                            int graphno, vector<long> ext_ids);
 
     // shortest path between two points
     vector<int> Route(int src, int tgt, int graphno = 0);
 
     // shortest path between list of origins and destinations
     vector<vector<int>> Routes(vector<long> sources, vector<long> targets,  
-                             int graphno = 0);
+                               int graphno = 0);
 
     // shortest path distance between two points
     double Distance(int src, int tgt, int graphno = 0);
     
     // shortest path distances between list of origins and destinations
     vector<double> Distances(vector<long> sources, vector<long> targets,  
                              int graphno = 0);
```

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/BasicDefinitions.h` & `pandana-0.7/src/contraction_hierarchies/src/BasicDefinitions.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/Contractor/ContractionCleanup.h` & `pandana-0.7/src/contraction_hierarchies/src/Contractor/ContractionCleanup.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/Contractor/Contractor.h` & `pandana-0.7/src/contraction_hierarchies/src/Contractor/Contractor.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/BinaryHeap.h` & `pandana-0.7/src/contraction_hierarchies/src/DataStructures/BinaryHeap.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/DynamicGraph.h` & `pandana-0.7/src/contraction_hierarchies/src/DataStructures/DynamicGraph.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/Percent.h` & `pandana-0.7/src/contraction_hierarchies/src/DataStructures/Percent.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/SimpleCHQuery.h` & `pandana-0.7/src/contraction_hierarchies/src/DataStructures/SimpleCHQuery.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/DataStructures/StaticGraph.h` & `pandana-0.7/src/contraction_hierarchies/src/DataStructures/StaticGraph.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/POIIndex/POIIndex.h` & `pandana-0.7/src/contraction_hierarchies/src/POIIndex/POIIndex.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/Util/HyperThreading.h` & `pandana-0.7/src/contraction_hierarchies/src/Util/HyperThreading.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/libch.cpp` & `pandana-0.7/src/contraction_hierarchies/src/libch.cpp`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/contraction_hierarchies/src/libch.h` & `pandana-0.7/src/contraction_hierarchies/src/libch.h`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/cyaccess.cpp` & `pandana-0.7/src/cyaccess.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,77 @@
-/* Generated by Cython 0.29.21 */
+/* Generated by Cython 3.0.0 */
 
+/* BEGIN: Cython Metadata
+{
+    "distutils": {
+        "depends": [
+            "/Users/maurer/opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/Users/maurer/opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/Users/maurer/opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/Users/maurer/opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/Users/maurer/opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "src/accessibility.h"
+        ],
+        "extra_compile_args": [
+            "-w",
+            "-std=c++11",
+            "-O3",
+            "-stdlib=libc++",
+            "-fopenmp"
+        ],
+        "extra_link_args": [
+            "-stdlib=libc++"
+        ],
+        "include_dirs": [
+            "src",
+            ".",
+            "/Users/maurer/opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/core/include"
+        ],
+        "language": "c++",
+        "name": "pandana.cyaccess",
+        "sources": [
+            "src/cyaccess.pyx",
+            "src/accessibility.cpp",
+            "src/graphalg.cpp",
+            "src/contraction_hierarchies/src/libch.cpp"
+        ]
+    },
+    "module_name": "pandana.cyaccess"
+}
+END: Cython Metadata */
+
+#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
+#endif /* PY_SSIZE_T_CLEAN */
+#if defined(CYTHON_LIMITED_API) && 0
+  #ifndef Py_LIMITED_API
+    #if CYTHON_LIMITED_API+0 > 0x03030000
+      #define Py_LIMITED_API CYTHON_LIMITED_API
+    #else
+      #define Py_LIMITED_API 0x03030000
+    #endif
+  #endif
+#endif
+
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.6+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.7+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_21"
-#define CYTHON_HEX_VERSION 0x001D15F0
-#define CYTHON_FUTURE_DIVISION 0
+#define CYTHON_ABI "3_0_0"
+#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
+#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
+#define CYTHON_HEX_VERSION 0x030000F0
+#define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -29,30 +82,34 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #if PY_VERSION_HEX >= 0x02070000
-    #define HAVE_LONG_LONG
-  #endif
+  #define HAVE_LONG_LONG
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#ifdef PYPY_VERSION
-  #define CYTHON_COMPILING_IN_PYPY 1
-  #define CYTHON_COMPILING_IN_PYSTON 0
+#if defined(GRAALVM_PYTHON)
+  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
+     The existence of this section does not imply that anything works or is even tested */
+  #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -69,35 +126,167 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-#elif defined(PYSTON_VERSION)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PYPY_VERSION)
+  #define CYTHON_COMPILING_IN_PYPY 1
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 0
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 0
+  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #undef CYTHON_AVOID_BORROWED_REFS
+  #define CYTHON_AVOID_BORROWED_REFS 1
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
+  #endif
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(CYTHON_LIMITED_API)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 1
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
+  #undef CYTHON_CLINE_IN_TRACEBACK
+  #define CYTHON_CLINE_IN_TRACEBACK 0
+  #undef CYTHON_USE_TYPE_SLOTS
+  #define CYTHON_USE_TYPE_SLOTS 0
+  #undef CYTHON_USE_TYPE_SPECS
+  #define CYTHON_USE_TYPE_SPECS 1
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #undef CYTHON_USE_ASYNC_SLOTS
+  #define CYTHON_USE_ASYNC_SLOTS 0
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #undef CYTHON_USE_UNICODE_INTERNALS
+  #define CYTHON_USE_UNICODE_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_WRITER
+    #define CYTHON_USE_UNICODE_WRITER 0
+  #endif
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #undef CYTHON_ASSUME_SAFE_MACROS
+  #define CYTHON_ASSUME_SAFE_MACROS 0
+  #undef CYTHON_UNPACK_METHODS
+  #define CYTHON_UNPACK_METHODS 0
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #undef CYTHON_METH_FASTCALL
+  #define CYTHON_METH_FASTCALL 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_MODULE_STATE
+  #define CYTHON_USE_MODULE_STATE 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #undef CYTHON_USE_ASYNC_SLOTS
-  #define CYTHON_USE_ASYNC_SLOTS 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
@@ -112,54 +301,55 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_LIMITED_API 0
+  #define CYTHON_COMPILING_IN_GRAAL 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYTYPE_LOOKUP
-    #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
+  #ifndef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #if PY_VERSION_HEX < 0x02070000
-    #undef CYTHON_USE_PYLONG_INTERNALS
-    #define CYTHON_USE_PYLONG_INTERNALS 0
-  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
@@ -169,35 +359,68 @@
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
+  #ifndef CYTHON_FAST_GIL
+    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
+  #endif
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
+  #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
   #endif
-  #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #if PY_VERSION_HEX < 0x03050000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
+  #if PY_VERSION_HEX < 0x030400a1
+    #undef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 0
+  #elif !defined(CYTHON_USE_TP_FINALIZE)
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #if PY_VERSION_HEX < 0x030600B1
+    #undef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS 0
+  #elif !defined(CYTHON_USE_DICT_VERSIONS)
+    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
+  #endif
+  #if PY_VERSION_HEX < 0x030700A3
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+    #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
+#if !defined(CYTHON_VECTORCALL)
+#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
+#endif
+#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -215,78 +438,128 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(maybe_unused)
+        #define CYTHON_UNUSED [[maybe_unused]]
+      #endif
+    #endif
+  #endif
+#endif
+#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
+#ifndef CYTHON_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
+#ifndef CYTHON_MAYBE_UNUSED_VAR
+  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
+#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-           typedef unsigned char     uint8_t;
-           typedef unsigned int      uint32_t;
+            typedef unsigned char     uint8_t;
+            typedef unsigned short    uint16_t;
+            typedef unsigned int      uint32_t;
         #else
-           typedef unsigned __int8   uint8_t;
-           typedef unsigned __int32  uint32_t;
+            typedef unsigned __int8   uint8_t;
+            typedef unsigned __int16  uint16_t;
+            typedef unsigned __int32  uint32_t;
+        #endif
+    #endif
+    #if _MSC_VER < 1300
+        #ifdef _WIN64
+            typedef unsigned long long  __pyx_uintptr_t;
+        #else
+            typedef unsigned int        __pyx_uintptr_t;
+        #endif
+    #else
+        #ifdef _WIN64
+            typedef unsigned __int64    __pyx_uintptr_t;
+        #else
+            typedef unsigned __int32    __pyx_uintptr_t;
         #endif
     #endif
 #else
-   #include <stdint.h>
+    #include <stdint.h>
+    typedef uintptr_t  __pyx_uintptr_t;
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus) && __cplusplus >= 201103L
-    #if __has_cpp_attribute(fallthrough)
-      #define CYTHON_FALLTHROUGH [[fallthrough]]
-    #elif __has_cpp_attribute(clang::fallthrough)
-      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-    #elif __has_cpp_attribute(gnu::fallthrough)
-      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+  #if defined(__cplusplus)
+    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
+     * but leads to warnings with -pedantic, since it is a C++17 feature */
+    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
+      #if __has_cpp_attribute(fallthrough)
+        #define CYTHON_FALLTHROUGH [[fallthrough]]
+      #endif
+    #endif
+    #ifndef CYTHON_FALLTHROUGH
+      #if __has_cpp_attribute(clang::fallthrough)
+        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+      #elif __has_cpp_attribute(gnu::fallthrough)
+        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
+      #endif
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__ ) && defined(__apple_build_version__)
+  #if defined(__clang__) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
+#ifdef __cplusplus
+  template <typename T>
+  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
+  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
+#else
+  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
+#endif
+#if CYTHON_COMPILING_IN_PYPY == 1
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
+#else
+  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
+#endif
+#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef __cplusplus
   #error "Cython files generated with the C++ option must be compiled with a C++ compiler."
 #endif
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
@@ -302,99 +575,233 @@
 class __Pyx_FakeReference {
   public:
     __Pyx_FakeReference() : ptr(NULL) { }
     __Pyx_FakeReference(const T& ref) : ptr(const_cast<T*>(&ref)) { }
     T *operator->() { return ptr; }
     T *operator&() { return ptr; }
     operator T&() { return *ptr; }
-    template<typename U> bool operator ==(U other) { return *ptr == other; }
-    template<typename U> bool operator !=(U other) { return *ptr != other; }
+    template<typename U> bool operator ==(const U& other) const { return *ptr == other; }
+    template<typename U> bool operator !=(const U& other) const { return *ptr != other; }
+    template<typename U> bool operator==(const __Pyx_FakeReference<U>& other) const { return *ptr == *other.ptr; }
+    template<typename U> bool operator!=(const __Pyx_FakeReference<U>& other) const { return *ptr != *other.ptr; }
   private:
     T *ptr;
 };
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject *co=NULL, *result=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
+        if (!(empty = PyTuple_New(0))) goto end;
+        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
+    end:
+        Py_XDECREF((PyObject*) co);
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return result;
+    }
+#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-  #define __Pyx_DefaultClassType PyType_Type
+#endif
+#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
+  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
+#else
+  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
+  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
+#else
+  #define __Pyx_Py_Is(x, y) ((x) == (y))
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
+  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
+#else
+  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
+  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
+#else
+  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
+#endif
+#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
+  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
+#else
+  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
+#endif
+#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
+#ifndef CO_COROUTINE
+  #define CO_COROUTINE 0x80
+#endif
+#ifndef CO_ASYNC_GENERATOR
+  #define CO_ASYNC_GENERATOR 0x200
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
+#ifndef Py_TPFLAGS_SEQUENCE
+  #define Py_TPFLAGS_SEQUENCE 0
+#endif
+#ifndef Py_TPFLAGS_MAPPING
+  #define Py_TPFLAGS_MAPPING 0
+#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_FAST_PYCCALL
-#define __Pyx_PyFastCFunction_Check(func)\
-    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
+#if CYTHON_METH_FASTCALL
+  #define __Pyx_METH_FASTCALL METH_FASTCALL
+  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
+  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
+#else
+  #define __Pyx_METH_FASTCALL METH_VARARGS
+  #define __Pyx_PyCFunction_FastCall PyCFunction
+  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
+#endif
+#if CYTHON_VECTORCALL
+  #define __pyx_vectorcallfunc vectorcallfunc
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
+  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
+#elif CYTHON_BACKPORT_VECTORCALL
+  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
+                                            size_t nargsf, PyObject *kwnames);
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
+#else
+  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
+  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
+#endif
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
+  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
 #else
-#define __Pyx_PyFastCFunction_Check(func) 0
+  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
+  #define __Pyx_PyCMethod  PyCMethod
+#endif
+#ifndef METH_METHOD
+  #define METH_METHOD 0x200
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
-  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
-  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
-  #define PyMem_RawFree(p)             PyMem_Free(p)
-#endif
-#if CYTHON_COMPILING_IN_PYSTON
-  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyThreadState_Current PyThreadState_Get()
+#elif !CYTHON_FAST_THREAD_STATE
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
+{
+    void *result;
+    result = PyModule_GetState(op);
+    if (!result)
+        Py_FatalError("Couldn't find the module state");
+    return result;
+}
+#endif
+#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
+#if CYTHON_COMPILING_IN_LIMITED_API
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
+#else
+  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
+#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -417,78 +824,166 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
+#if PY_MAJOR_VERSION < 3
+    #if CYTHON_COMPILING_IN_PYPY
+        #if PYPY_VERSION_NUM < 0x07030600
+            #if defined(__cplusplus) && __cplusplus >= 201402L
+                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
+            #elif defined(__GNUC__) || defined(__clang__)
+                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
+            #elif defined(_MSC_VER)
+                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
+            #endif
+            static CYTHON_INLINE int PyGILState_Check(void) {
+                return 0;
+            }
+        #else  // PYPY_VERSION_NUM < 0x07030600
+        #endif  // PYPY_VERSION_NUM < 0x07030600
+    #else
+        static CYTHON_INLINE int PyGILState_Check(void) {
+            PyThreadState * tstate = _PyThreadState_Current;
+            return tstate && (tstate == PyGILState_GetThisThreadState());
+        }
+    #endif
+#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
+    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
+    if (res == NULL) PyErr_Clear();
+    return res;
+}
+#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
+#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#else
+static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyDict_GetItem(dict, name);
 #else
-#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
+    PyDictEntry *ep;
+    PyDictObject *mp = (PyDictObject*) dict;
+    long hash = ((PyStringObject *) name)->ob_shash;
+    assert(hash != -1);
+    ep = (mp->ma_lookup)(mp, name, hash);
+    if (ep == NULL) {
+        return NULL;
+    }
+    return ep->me_value;
+#endif
+}
+#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#endif
+#if CYTHON_USE_TYPE_SLOTS
+  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
+  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
+#else
+  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
+  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
+  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
 #endif
-#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
+    PyTypeObject *type = Py_TYPE(obj);\
+    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
+    PyObject_GC_Del(obj);\
+    Py_DECREF(type);\
+}
+#else
+#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
   #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #define __Pyx_PyUnicode_READY(op)       (0)
+  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
+  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
+  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
+  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
+#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+  #define CYTHON_PEP393_ENABLED 1
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
-  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
+  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
-  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
-  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-#endif
-#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
-  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+#if CYTHON_COMPILING_IN_PYPY
+  #if !defined(PyUnicode_DecodeUnicodeEscape)
+    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
+  #endif
+  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
+    #undef PyUnicode_Contains
+    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+  #endif
+  #if !defined(PyByteArray_Check)
+    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+  #endif
+  #if !defined(PyObject_Format)
+    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
+  #endif
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -509,16 +1004,22 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
+#if CYTHON_COMPILING_IN_CPYTHON
+  #define __Pyx_PySequence_ListKeepNew(obj)\
+    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
+#else
+  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
+#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
+  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
@@ -529,46 +1030,46 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
+  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
+  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
+#else
+  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
+  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
-#endif
-#if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
-#else
-  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
+  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
@@ -580,16 +1081,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -604,50 +1107,59 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifndef __PYX_EXTERN_C
-  #ifdef __cplusplus
-    #define __PYX_EXTERN_C extern "C"
-  #else
-    #define __PYX_EXTERN_C extern
-  #endif
+#ifdef CYTHON_EXTERN_C
+    #undef __PYX_EXTERN_C
+    #define __PYX_EXTERN_C CYTHON_EXTERN_C
+#elif defined(__PYX_EXTERN_C)
+    #ifdef _MSC_VER
+    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
+    #else
+    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
+    #endif
+#else
+    #define __PYX_EXTERN_C extern "C++"
 #endif
 
 #define __PYX_HAVE__pandana__cyaccess
 #define __PYX_HAVE_API__pandana__cyaccess
 /* Early includes */
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
 #include <string.h>
 #include <string>
 #include <utility>
 
-    #if __cplusplus > 199711L
+    #if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
+    // move should be defined for these versions of MSVC, but __cplusplus isn't set usefully
     #include <type_traits>
 
     namespace cython_std {
     template <typename T> typename std::remove_reference<T>::type&& move(T& t) noexcept { return std::move(t); }
     template <typename T> typename std::remove_reference<T>::type&& move(T&& t) noexcept { return std::move(t); }
     }
 
     #endif
     
 #include <stdio.h>
-#include "numpy/arrayobject.h"
-#include "numpy/ufuncobject.h"
 
-    /* NumPy API declarations from "numpy/__init__.pxd" */
+    /* Using NumPy API declarations from "numpy/__init__.cython-30.pxd" */
     
+#include "numpy/arrayobject.h"
+#include "numpy/ndarrayobject.h"
+#include "numpy/ndarraytypes.h"
+#include "numpy/arrayscalars.h"
+#include "numpy/ufuncobject.h"
 #include "accessibility.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -709,54 +1221,111 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
+{
+    const wchar_t *u_end = u;
+    while (*u_end++) ;
+    return (size_t)(u_end - u - 1);
+}
+#else
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
+{
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
+#endif
+#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
+#if CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX >= 0x030C00A7
+  #ifndef _PyLong_SIGN_MASK
+    #define _PyLong_SIGN_MASK 3
+  #endif
+  #ifndef _PyLong_NON_SIZE_BITS
+    #define _PyLong_NON_SIZE_BITS 3
+  #endif
+  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
+  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
+  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
+  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
+  #define __Pyx_PyLong_SignedDigitCount(x)\
+        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
+  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
+    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
+    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
+  #else
+    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
+    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
+  #endif
+  typedef Py_ssize_t  __Pyx_compact_pylong;
+  typedef size_t  __Pyx_compact_upylong;
+  #else  // Py < 3.12
+  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
+  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
+  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
+  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
+  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
+  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
+  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
+  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
+  #define __Pyx_PyLong_CompactValue(x)\
+        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
+  typedef sdigit  __Pyx_compact_pylong;
+  typedef digit  __Pyx_compact_upylong;
+  #endif
+  #if PY_VERSION_HEX >= 0x030C00A5
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
+  #else
+  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
+  #endif
+#endif
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -770,15 +1339,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = c;
+            ascii_chars[c] = (char) c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -835,31 +1404,27 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
+#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-static PyObject *__pyx_d;
-static PyObject *__pyx_b;
-static PyObject *__pyx_cython_runtime = NULL;
-static PyObject *__pyx_empty_tuple;
-static PyObject *__pyx_empty_bytes;
-static PyObject *__pyx_empty_unicode;
+#endif
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm= __FILE__;
+static const char * __pyx_cfilenm = __FILE__;
 static const char *__pyx_filename;
 
 /* Header.proto */
 #if !defined(CYTHON_CCOMPLEX)
   #if defined(__cplusplus)
     #define CYTHON_CCOMPLEX 1
-  #elif defined(_Complex_I)
+  #elif (defined(_Complex_I) && !defined(_MSC_VER)) || ((defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) && !defined(__STDC_NO_COMPLEX__))
     #define CYTHON_CCOMPLEX 1
   #else
     #define CYTHON_CCOMPLEX 0
   #endif
 #endif
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
@@ -869,23 +1434,24 @@
   #endif
 #endif
 #if CYTHON_CCOMPLEX && !defined(__cplusplus) && defined(__sun__) && defined(__GNUC__)
   #undef _Complex_I
   #define _Complex_I 1.0fj
 #endif
 
+/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
   "src/cyaccess.pyx",
-  "stringsource",
-  "__init__.pxd",
+  "<stringsource>",
+  "__init__.cython-30.pxd",
   "type.pxd",
 };
+/* #### Code section: utility_code_proto_before_types ### */
 /* BufferFormatStructs.proto */
-#define IS_UNSIGNED(type) (((type) -1) > 0)
 struct __Pyx_StructField_;
 #define __PYX_BUF_FLAGS_PACKED_STRUCT (1 << 0)
 typedef struct {
   const char* name;
   struct __Pyx_StructField_* fields;
   size_t size;
   size_t arraysize[8];
@@ -912,354 +1478,444 @@
   int is_complex;
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
+/* #### Code section: numeric_typedefs ### */
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":718
- * 
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
+/* #### Code section: complex_type_declarations ### */
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< float > __pyx_t_float_complex;
   #else
     typedef float _Complex __pyx_t_float_complex;
   #endif
 #else
     typedef struct { float real, imag; } __pyx_t_float_complex;
 #endif
 static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float, float);
 
 /* Declarations.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     typedef ::std::complex< double > __pyx_t_double_complex;
   #else
     typedef double _Complex __pyx_t_double_complex;
   #endif
 #else
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
+/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 struct __pyx_obj_7pandana_8cyaccess_cyaccess;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "src/cyaccess.pyx":58
+/* "src/cyaccess.pyx":61
  * 
  * 
  * cdef class cyaccess:             # <<<<<<<<<<<<<<
  *     cdef Accessibility * access
  * 
  */
 struct __pyx_obj_7pandana_8cyaccess_cyaccess {
   PyObject_HEAD
   MTC::accessibility::Accessibility *access;
 };
 
+/* #### Code section: utility_code_proto ### */
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, int);
-    void (*DECREF)(void*, PyObject*, int);
-    void (*GOTREF)(void*, PyObject*, int);
-    void (*GIVEREF)(void*, PyObject*, int);
-    void* (*SetupContext)(const char*, int, const char*);
+    void (*INCREF)(void*, PyObject*, Py_ssize_t);
+    void (*DECREF)(void*, PyObject*, Py_ssize_t);
+    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
+    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
+    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+          }
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
+  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
 #endif
+  #define __Pyx_RefNannyFinishContextNogil() {\
+              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
+              __Pyx_RefNannyFinishContext();\
+              PyGILState_Release(__pyx_gilstate_save);\
+          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
-  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
+  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
+  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
+#define __Pyx_Py_XDECREF_SET(r, v) do {\
+        PyObject *tmp = (PyObject *) r;\
+        r = v; Py_XDECREF(tmp);\
+    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
+/* PyThreadStateGet.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
+#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
+#if PY_VERSION_HEX >= 0x030C00A6
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
+#else
+#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
+#endif
+#else
+#define __Pyx_PyThreadState_declare
+#define __Pyx_PyThreadState_assign
+#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
+#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
+#endif
+
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
 /* PyObjectGetAttrStr.proto */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
+
 /* GetBuiltinName.proto */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name);
 
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
+
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
 #define __PYX_GET_DICT_VERSION(dict)  (((PyDictObject*)(dict))->ma_version_tag)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)\
     (version_var) = __PYX_GET_DICT_VERSION(dict);\
     (cache_var) = (value);
@@ -1280,40 +1936,33 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* PyObjectCall.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
-#else
-#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
-#endif
-
 /* ExtTypeTest.proto */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type);
 
 /* SetItemInt.proto */
 #define __Pyx_SetItemInt(o, i, v, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
@@ -1341,29 +1990,72 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
+/* TupleAndListFromArray.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
+static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
+#endif
+
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* fastcall.proto */
+#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
+#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
+#define __Pyx_KwValues_VARARGS(args, nargs) NULL
+#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
+#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
+#if CYTHON_METH_FASTCALL
+    #define __Pyx_Arg_FASTCALL(args, i) args[i]
+    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
+    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
+    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
+    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
+#else
+    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
+    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
+    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
+    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
+    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
+#else
+#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
+#endif
+
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
 /* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
+    PyObject **argnames[],
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
     const char* function_name);
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
-    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+    ((likely(__Pyx_IS_TYPE(obj, type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
 /* IsLittleEndian.proto */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
 
 /* BufferFormatCheck.proto */
@@ -1380,157 +2072,285 @@
 static int  __Pyx__GetBufferAndValidate(Py_buffer* buf, PyObject* obj,
     __Pyx_TypeInfo* dtype, int flags, int nd, int cast, __Pyx_BufFmt_StackElem* stack);
 static void __Pyx_ZeroBuffer(Py_buffer* buf);
 static CYTHON_INLINE void __Pyx_SafeReleaseBuffer(Py_buffer* info);
 static Py_ssize_t __Pyx_minusones[] = { -1, -1, -1, -1, -1, -1, -1, -1 };
 static Py_ssize_t __Pyx_zeros[] = { 0, 0, 0, 0, 0, 0, 0, 0 };
 
-/* PyThreadStateGet.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
-#define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
+/* MoveIfSupported.proto */
+#if __cplusplus >= 201103L || (defined(_MSC_VER) && _MSC_VER >= 1600)
+  #include <utility>
+  #define __PYX_STD_MOVE_IF_SUPPORTED(x) std::move(x)
 #else
-#define __Pyx_PyThreadState_declare
-#define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
+  #define __PYX_STD_MOVE_IF_SUPPORTED(x) x
 #endif
 
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
-#endif
+/* KeywordStringCheck.proto */
+static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
-/* RaiseException.proto */
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
+/* IncludeStructmemberH.proto */
+#include <structmember.h>
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+/* FixUpExtensionType.proto */
+#if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
 #endif
 
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+/* PyFunctionFastCall.proto */
+#if CYTHON_FAST_PYCALL
+#if !CYTHON_VECTORCALL
+#define __Pyx_PyFunction_FastCall(func, args, nargs)\
+    __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
 #endif
-
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#define __Pyx_BUILD_ASSERT_EXPR(cond)\
+    (sizeof(char [1 - 2*!(cond)]) - 1)
+#ifndef Py_MEMBER_SIZE
+#define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
+#endif
+#if !CYTHON_VECTORCALL
+#if PY_VERSION_HEX >= 0x03080000
+  #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+  #define __Pxy_PyFrame_Initialize_Offsets()
+  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
 #else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+  static size_t __pyx_pyframe_localsplus_offset = 0;
+  #include "frameobject.h"
+  #define __Pxy_PyFrame_Initialize_Offsets()\
+    ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
+     (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
+  #define __Pyx_PyFrame_GetLocalsplus(frame)\
+    (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif
+#endif
 #endif
 
-/* GetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+/* PyObjectCallMethO.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* ListCompAppend.proto */
-#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
-static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
-    PyListObject* L = (PyListObject*) list;
-    Py_ssize_t len = Py_SIZE(list);
-    if (likely(L->allocated > len)) {
-        Py_INCREF(x);
-        PyList_SET_ITEM(list, len, x);
-        __Pyx_SET_SIZE(list, len + 1);
-        return 0;
-    }
-    return PyList_Append(list, x);
-}
-#else
-#define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
+/* PyObjectFastCall.proto */
+#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
+
+/* PyObjectCallNoArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
+
+/* PyObjectCallOneArg.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
+
+/* PyObjectGetMethod.proto */
+static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
+
+/* PyObjectCallMethod0.proto */
+static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
+
+/* ValidateBasesTuple.proto */
+#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
 #endif
 
+/* PyType_Ready.proto */
+CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
+
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
 /* PyObject_GenericGetAttr.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
-/* PyObjectGetAttrStrNoError.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
-
 /* SetupReduce.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
+#endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_0
+#define __PYX_HAVE_RT_ImportType_proto_3_0_0
+#if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_0(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_3_0_0 {
+   __Pyx_ImportType_CheckSize_Error_3_0_0 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_0 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_0 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
+/* ImportDottedModule.proto */
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple);
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple);
+#endif
+
+/* FetchSharedCythonModule.proto */
+static PyObject *__Pyx_FetchSharedCythonABIModule(void);
+
+/* FetchCommonType.proto */
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
+#else
+static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
+#endif
+
+/* PyMethodNew.proto */
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
+    CYTHON_UNUSED_VAR(typ);
+    if (!self)
+        return __Pyx_NewRef(func);
+    return PyMethod_New(func, self);
+}
+#else
+    #define __Pyx_PyMethod_New PyMethod_New
+#endif
+
+/* PyVectorcallFastCallDict.proto */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
+#endif
+
+/* CythonFunctionShared.proto */
+#define __Pyx_CyFunction_USED
+#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
+#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
+#define __Pyx_CYFUNCTION_CCLASS        0x04
+#define __Pyx_CYFUNCTION_COROUTINE     0x08
+#define __Pyx_CyFunction_GetClosure(f)\
+    (((__pyx_CyFunctionObject *) (f))->func_closure)
+#if PY_VERSION_HEX < 0x030900B1
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      (((__pyx_CyFunctionObject *) (f))->func_classobj)
+#else
+  #define __Pyx_CyFunction_GetClassObj(f)\
+      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
+#endif
+#define __Pyx_CyFunction_SetClassObj(f, classobj)\
+    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
+#define __Pyx_CyFunction_Defaults(type, f)\
+    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
+#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
+    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
+typedef struct {
+#if PY_VERSION_HEX < 0x030900B1
+    PyCFunctionObject func;
+#else
+    PyCMethodObject func;
+#endif
+#if CYTHON_BACKPORT_VECTORCALL
+    __pyx_vectorcallfunc func_vectorcall;
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    PyObject *func_weakreflist;
+#endif
+    PyObject *func_dict;
+    PyObject *func_name;
+    PyObject *func_qualname;
+    PyObject *func_doc;
+    PyObject *func_globals;
+    PyObject *func_code;
+    PyObject *func_closure;
+#if PY_VERSION_HEX < 0x030900B1
+    PyObject *func_classobj;
+#endif
+    void *defaults;
+    int defaults_pyobjects;
+    size_t defaults_size;  // used by FusedFunction for copying defaults
+    int flags;
+    PyObject *defaults_tuple;
+    PyObject *defaults_kwdict;
+    PyObject *(*defaults_getter)(PyObject *);
+    PyObject *func_annotations;
+    PyObject *func_is_coroutine;
+} __pyx_CyFunctionObject;
+#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
+#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
+#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
+                                                         size_t size,
+                                                         int pyobjects);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
+                                                            PyObject *tuple);
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
+                                                             PyObject *dict);
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
+                                                              PyObject *dict);
+static int __pyx_CyFunction_init(PyObject *module);
+#if CYTHON_METH_FASTCALL
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
+#if CYTHON_BACKPORT_VECTORCALL
+#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
+#else
+#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
+#endif
+#endif
+
+/* CythonFunction.proto */
+static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
+                                      int flags, PyObject* qualname,
+                                      PyObject *closure,
+                                      PyObject *module, PyObject *globals,
+                                      PyObject* code);
+
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
+#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
+#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* BufferStructDeclare.proto */
 typedef struct {
@@ -1551,19 +2371,18 @@
     static void __Pyx_ReleaseBuffer(Py_buffer *view);
 #else
     #define __Pyx_GetBuffer PyObject_GetBuffer
     #define __Pyx_ReleaseBuffer PyBuffer_Release
 #endif
 
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+/* GCCDiagnostics.proto */
+#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
 
 /* CppExceptionConversion.proto */
 #ifndef __Pyx_CppExn2PyErr
 #include <new>
 #include <typeinfo>
 #include <stdexcept>
 #include <ios>
@@ -1622,15 +2441,15 @@
     #define __Pyx_SET_CIMAG(z,y) ((z).imag(y))
 #else
     #define __Pyx_SET_CREAL(z,x) __Pyx_CREAL(z) = (x)
     #define __Pyx_SET_CIMAG(z,y) __Pyx_CIMAG(z) = (y)
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_float(a, b)   ((a)==(b))
     #define __Pyx_c_sum_float(a, b)  ((a)+(b))
     #define __Pyx_c_diff_float(a, b) ((a)-(b))
     #define __Pyx_c_prod_float(a, b) ((a)*(b))
     #define __Pyx_c_quot_float(a, b) ((a)/(b))
     #define __Pyx_c_neg_float(a)     (-(a))
   #ifdef __cplusplus
@@ -1660,15 +2479,15 @@
     #if 1
         static CYTHON_INLINE float __Pyx_c_abs_float(__pyx_t_float_complex);
         static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_pow_float(__pyx_t_float_complex, __pyx_t_float_complex);
     #endif
 #endif
 
 /* Arithmetic.proto */
-#if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_double(a, b)   ((a)==(b))
     #define __Pyx_c_sum_double(a, b)  ((a)+(b))
     #define __Pyx_c_diff_double(a, b) ((a)-(b))
     #define __Pyx_c_prod_double(a, b) ((a)*(b))
     #define __Pyx_c_quot_double(a, b) ((a)/(b))
     #define __Pyx_c_neg_double(a)     (-(a))
   #ifdef __cplusplus
@@ -1701,224 +2520,4114 @@
     #endif
 #endif
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntFromPy.proto */
-static CYTHON_INLINE Py_intptr_t __Pyx_PyInt_As_Py_intptr_t(PyObject *);
-
-/* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
+/* FormatTypeName.proto */
+#if CYTHON_COMPILING_IN_LIMITED_API
+typedef PyObject *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%U"
+static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
+#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
+#else
+typedef const char *__Pyx_TypeName;
+#define __Pyx_FMT_TYPENAME "%.200s"
+#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
+#define __Pyx_DECREF_TypeName(obj)
+#endif
+
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
+#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
+#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
+/* #### Code section: module_declarations ### */
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self); /* proto*/
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self); /* proto*/
 
-/* Module declarations from 'cython' */
-
-/* Module declarations from 'libcpp' */
+/* Module declarations from "cython" */
 
-/* Module declarations from 'libcpp.vector' */
+/* Module declarations from "libcpp" */
 
-/* Module declarations from 'libc.string' */
+/* Module declarations from "libcpp.vector" */
 
-/* Module declarations from 'libcpp.string' */
+/* Module declarations from "libc.string" */
 
-/* Module declarations from 'libcpp.utility' */
+/* Module declarations from "libcpp.string" */
 
-/* Module declarations from 'libcpp.pair' */
+/* Module declarations from "libcpp.utility" */
 
-/* Module declarations from 'cpython.buffer' */
+/* Module declarations from "libcpp.pair" */
 
-/* Module declarations from 'libc.stdio' */
+/* Module declarations from "libc.stdio" */
 
-/* Module declarations from '__builtin__' */
+/* Module declarations from "__builtin__" */
 
-/* Module declarations from 'cpython.type' */
-static PyTypeObject *__pyx_ptype_7cpython_4type_type = 0;
+/* Module declarations from "cpython.type" */
 
-/* Module declarations from 'cpython' */
+/* Module declarations from "cpython" */
 
-/* Module declarations from 'cpython.object' */
+/* Module declarations from "cpython.object" */
 
-/* Module declarations from 'cpython.ref' */
+/* Module declarations from "cpython.ref" */
 
-/* Module declarations from 'cpython.mem' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
+/* Module declarations from "numpy" */
 
-/* Module declarations from 'numpy' */
-static PyTypeObject *__pyx_ptype_5numpy_dtype = 0;
-static PyTypeObject *__pyx_ptype_5numpy_flatiter = 0;
-static PyTypeObject *__pyx_ptype_5numpy_broadcast = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ndarray = 0;
-static PyTypeObject *__pyx_ptype_5numpy_ufunc = 0;
-
-/* Module declarations from 'pandana.cyaccess' */
-static PyTypeObject *__pyx_ptype_7pandana_8cyaccess_cyaccess = 0;
+/* Module declarations from "pandana.cyaccess" */
 static PyArrayObject *__pyx_f_7pandana_8cyaccess_convert_vector_to_array_dbl(std::vector<double> ); /*proto*/
 static PyArrayObject *__pyx_f_7pandana_8cyaccess_convert_2D_vector_to_array_dbl(std::vector<std::vector<double> > ); /*proto*/
 static PyArrayObject *__pyx_f_7pandana_8cyaccess_convert_2D_vector_to_array_int(std::vector<std::vector<int> > ); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
-static PyObject *__pyx_convert_vector_to_py_double(const std::vector<double>  &); /*proto*/
-static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(const std::vector<std::vector<double> >  &); /*proto*/
-static PyObject *__pyx_convert_vector_to_py_int(const std::vector<int>  &); /*proto*/
-static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(const std::vector<std::vector<int> >  &); /*proto*/
 static std::vector<long>  __pyx_convert_vector_from_py_long(PyObject *); /*proto*/
+static PyObject *__pyx_convert_vector_to_py_double(std::vector<double>  const &); /*proto*/
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(std::vector<std::vector<double> >  const &); /*proto*/
+static PyObject *__pyx_convert_vector_to_py_int(std::vector<int>  const &); /*proto*/
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(std::vector<std::vector<int> >  const &); /*proto*/
 static std::vector<std::vector<long> >  __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(PyObject *); /*proto*/
 static std::vector<double>  __pyx_convert_vector_from_py_double(PyObject *); /*proto*/
 static std::vector<std::vector<double> >  __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(PyObject *); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
-static PyObject *__pyx_convert_vector_to_py_std_3a__3a_string(const std::vector<std::string>  &); /*proto*/
-static __Pyx_TypeInfo __Pyx_TypeInfo_long = { "long", NULL, sizeof(long), { 0 }, 0, IS_UNSIGNED(long) ? 'U' : 'I', IS_UNSIGNED(long), 0 };
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_string(std::vector<std::string>  const &); /*proto*/
+static PyObject *__pyx_convert_pair_to_py_long____float(std::pair<long,float>  const &); /*proto*/
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___(std::vector<std::pair<long,float> >  const &); /*proto*/
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___(std::vector<std::vector<std::pair<long,float> > >  const &); /*proto*/
+/* #### Code section: typeinfo ### */
+static __Pyx_TypeInfo __Pyx_TypeInfo_long = { "long", NULL, sizeof(long), { 0 }, 0, __PYX_IS_UNSIGNED(long) ? 'U' : 'I', __PYX_IS_UNSIGNED(long), 0 };
 static __Pyx_TypeInfo __Pyx_TypeInfo_double = { "double", NULL, sizeof(double), { 0 }, 0, 'R', 0, 0 };
+/* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "pandana.cyaccess"
 extern int __pyx_module_is_main_pandana__cyaccess;
 int __pyx_module_is_main_pandana__cyaccess = 0;
 
-/* Implementation of 'pandana.cyaccess' */
+/* Implementation of "pandana.cyaccess" */
+/* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_TypeError;
+static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_ImportError;
+/* #### Code section: string_decls ### */
+static const char __pyx_k__3[] = "*";
+static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_np[] = "np";
+static const char __pyx_k__29[] = "?";
 static const char __pyx_k_int[] = "int";
+static const char __pyx_k_ret[] = "ret";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
+static const char __pyx_k_self[] = "self";
+static const char __pyx_k_spec[] = "__spec__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_decay[] = "decay";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_edges[] = "edges";
 static const char __pyx_k_impno[] = "impno";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_aggtyp[] = "aggtyp";
 static const char __pyx_k_double[] = "double";
+static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_radius[] = "radius";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_twoway[] = "twoway";
 static const char __pyx_k_values[] = "values";
+static const char __pyx_k_disable[] = "disable";
+static const char __pyx_k_ext_ids[] = "ext_ids";
 static const char __pyx_k_maxdist[] = "maxdist";
 static const char __pyx_k_srcnode[] = "srcnode";
 static const char __pyx_k_category[] = "category";
 static const char __pyx_k_cyaccess[] = "cyaccess";
 static const char __pyx_k_destnode[] = "destnode";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_maxitems[] = "maxitems";
 static const char __pyx_k_node_ids[] = "node_ids";
 static const char __pyx_k_node_xys[] = "node_xys";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_srcnodes[] = "srcnodes";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_destnodes[] = "destnodes";
+static const char __pyx_k_isenabled[] = "isenabled";
+static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_empty_like[] = "empty_like";
 static const char __pyx_k_ImportError[] = "ImportError";
+static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_num_of_pois[] = "num_of_pois";
 static const char __pyx_k_edge_weights[] = "edge_weights";
+static const char __pyx_k_initializing[] = "_initializing";
+static const char __pyx_k_is_coroutine[] = "_is_coroutine";
+static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_shortest_path[] = "shortest_path";
+static const char __pyx_k_nodes_in_range[] = "nodes_in_range";
+static const char __pyx_k_shortest_paths[] = "shortest_paths";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_pandana_cyaccess[] = "pandana.cyaccess";
+static const char __pyx_k_precompute_range[] = "precompute_range";
+static const char __pyx_k_src_cyaccess_pyx[] = "src/cyaccess.pyx";
+static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_initialize_category[] = "initialize_category";
+static const char __pyx_k_get_available_decays[] = "get_available_decays";
+static const char __pyx_k_find_all_nearest_pois[] = "find_all_nearest_pois";
+static const char __pyx_k_initialize_access_var[] = "initialize_access_var";
+static const char __pyx_k_cyaccess_shortest_path[] = "cyaccess.shortest_path";
+static const char __pyx_k_shortest_path_distance[] = "shortest_path_distance";
+static const char __pyx_k_cyaccess_nodes_in_range[] = "cyaccess.nodes_in_range";
+static const char __pyx_k_cyaccess_shortest_paths[] = "cyaccess.shortest_paths";
+static const char __pyx_k_shortest_path_distances[] = "shortest_path_distances";
+static const char __pyx_k_cyaccess___reduce_cython[] = "cyaccess.__reduce_cython__";
+static const char __pyx_k_cyaccess_precompute_range[] = "cyaccess.precompute_range";
+static const char __pyx_k_cyaccess___setstate_cython[] = "cyaccess.__setstate_cython__";
+static const char __pyx_k_get_available_aggregations[] = "get_available_aggregations";
+static const char __pyx_k_cyaccess_initialize_category[] = "cyaccess.initialize_category";
+static const char __pyx_k_cyaccess_get_available_decays[] = "cyaccess.get_available_decays";
+static const char __pyx_k_cyaccess_find_all_nearest_pois[] = "cyaccess.find_all_nearest_pois";
+static const char __pyx_k_cyaccess_initialize_access_var[] = "cyaccess.initialize_access_var";
+static const char __pyx_k_cyaccess_shortest_path_distance[] = "cyaccess.shortest_path_distance";
+static const char __pyx_k_get_all_aggregate_accessibility[] = "get_all_aggregate_accessibility_variables";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
+static const char __pyx_k_cyaccess_get_all_aggregate_acces[] = "cyaccess.get_all_aggregate_accessibility_variables";
+static const char __pyx_k_cyaccess_get_available_aggregati[] = "cyaccess.get_available_aggregations";
+static const char __pyx_k_cyaccess_shortest_path_distances[] = "cyaccess.shortest_path_distances";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
-static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_n_s_TypeError;
-static PyObject *__pyx_n_s_aggtyp;
-static PyObject *__pyx_n_s_category;
-static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_cyaccess;
-static PyObject *__pyx_n_s_decay;
-static PyObject *__pyx_n_s_destnode;
-static PyObject *__pyx_n_s_destnodes;
-static PyObject *__pyx_n_s_double;
-static PyObject *__pyx_n_s_dtype;
-static PyObject *__pyx_n_s_edge_weights;
-static PyObject *__pyx_n_s_edges;
-static PyObject *__pyx_n_s_empty_like;
-static PyObject *__pyx_n_s_getstate;
-static PyObject *__pyx_n_s_impno;
-static PyObject *__pyx_n_s_import;
-static PyObject *__pyx_n_s_int;
-static PyObject *__pyx_n_s_main;
-static PyObject *__pyx_n_s_maxdist;
-static PyObject *__pyx_n_s_maxitems;
-static PyObject *__pyx_n_s_name;
-static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
-static PyObject *__pyx_n_s_node_ids;
-static PyObject *__pyx_n_s_node_xys;
-static PyObject *__pyx_n_s_np;
-static PyObject *__pyx_n_s_num_of_pois;
-static PyObject *__pyx_n_s_numpy;
-static PyObject *__pyx_kp_s_numpy_core_multiarray_failed_to;
-static PyObject *__pyx_kp_s_numpy_core_umath_failed_to_impor;
-static PyObject *__pyx_n_s_radius;
-static PyObject *__pyx_n_s_range;
-static PyObject *__pyx_n_s_reduce;
-static PyObject *__pyx_n_s_reduce_cython;
-static PyObject *__pyx_n_s_reduce_ex;
-static PyObject *__pyx_n_s_setstate;
-static PyObject *__pyx_n_s_setstate_cython;
-static PyObject *__pyx_n_s_srcnode;
-static PyObject *__pyx_n_s_srcnodes;
-static PyObject *__pyx_n_s_test;
-static PyObject *__pyx_n_s_twoway;
-static PyObject *__pyx_n_s_values;
-static PyObject *__pyx_n_s_zeros;
+/* #### Code section: decls ### */
 static int __pyx_pf_7pandana_8cyaccess_8cyaccess___cinit__(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, PyArrayObject *__pyx_v_node_ids, CYTHON_UNUSED PyArrayObject *__pyx_v_node_xys, PyArrayObject *__pyx_v_edges, PyArrayObject *__pyx_v_edge_weights, bool __pyx_v_twoway); /* proto */
 static void __pyx_pf_7pandana_8cyaccess_8cyaccess_2__dealloc__(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_4initialize_category(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, double __pyx_v_maxdist, int __pyx_v_maxitems, std::string __pyx_v_category, PyArrayObject *__pyx_v_node_ids); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_6find_all_nearest_pois(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, double __pyx_v_radius, int __pyx_v_num_of_pois, std::string __pyx_v_category, int __pyx_v_impno); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_8initialize_access_var(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, std::string __pyx_v_category, PyArrayObject *__pyx_v_node_ids, PyArrayObject *__pyx_v_values); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_10get_available_aggregations(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_12get_available_decays(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_14get_all_aggregate_accessibility_variables(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, double __pyx_v_radius, PyObject *__pyx_v_category, PyObject *__pyx_v_aggtyp, PyObject *__pyx_v_decay, int __pyx_v_impno); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_16shortest_path(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, int __pyx_v_srcnode, int __pyx_v_destnode, int __pyx_v_impno); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_18shortest_paths(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, PyArrayObject *__pyx_v_srcnodes, PyArrayObject *__pyx_v_destnodes, int __pyx_v_impno); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_20shortest_path_distance(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, int __pyx_v_srcnode, int __pyx_v_destnode, int __pyx_v_impno); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_22shortest_path_distances(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, PyArrayObject *__pyx_v_srcnodes, PyArrayObject *__pyx_v_destnodes, int __pyx_v_impno); /* proto */
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_24precompute_range(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, double __pyx_v_radius); /* proto */
-static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_26__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_28__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_26nodes_in_range(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, std::vector<long>  __pyx_v_srcnodes, float __pyx_v_radius, int __pyx_v_impno, PyArrayObject *__pyx_v_ext_ids); /* proto */
+static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_28__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_30__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_7pandana_8cyaccess_cyaccess(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__4;
-/* Late includes */
+/* #### Code section: late_includes ### */
+/* #### Code section: module_state ### */
+typedef struct {
+  PyObject *__pyx_d;
+  PyObject *__pyx_b;
+  PyObject *__pyx_cython_runtime;
+  PyObject *__pyx_empty_tuple;
+  PyObject *__pyx_empty_bytes;
+  PyObject *__pyx_empty_unicode;
+  #ifdef __Pyx_CyFunction_USED
+  PyTypeObject *__pyx_CyFunctionType;
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  PyTypeObject *__pyx_FusedFunctionType;
+  #endif
+  #ifdef __Pyx_Generator_USED
+  PyTypeObject *__pyx_GeneratorType;
+  #endif
+  #ifdef __Pyx_IterableCoroutine_USED
+  PyTypeObject *__pyx_IterableCoroutineType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineAwaitType;
+  #endif
+  #ifdef __Pyx_Coroutine_USED
+  PyTypeObject *__pyx_CoroutineType;
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_7cpython_4type_type;
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  #if CYTHON_USE_MODULE_STATE
+  #endif
+  PyTypeObject *__pyx_ptype_5numpy_dtype;
+  PyTypeObject *__pyx_ptype_5numpy_flatiter;
+  PyTypeObject *__pyx_ptype_5numpy_broadcast;
+  PyTypeObject *__pyx_ptype_5numpy_ndarray;
+  PyTypeObject *__pyx_ptype_5numpy_generic;
+  PyTypeObject *__pyx_ptype_5numpy_number;
+  PyTypeObject *__pyx_ptype_5numpy_integer;
+  PyTypeObject *__pyx_ptype_5numpy_signedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_unsignedinteger;
+  PyTypeObject *__pyx_ptype_5numpy_inexact;
+  PyTypeObject *__pyx_ptype_5numpy_floating;
+  PyTypeObject *__pyx_ptype_5numpy_complexfloating;
+  PyTypeObject *__pyx_ptype_5numpy_flexible;
+  PyTypeObject *__pyx_ptype_5numpy_character;
+  PyTypeObject *__pyx_ptype_5numpy_ufunc;
+  #if CYTHON_USE_MODULE_STATE
+  PyObject *__pyx_type_7pandana_8cyaccess_cyaccess;
+  #endif
+  PyTypeObject *__pyx_ptype_7pandana_8cyaccess_cyaccess;
+  PyObject *__pyx_n_s_ImportError;
+  PyObject *__pyx_n_s_MemoryError;
+  PyObject *__pyx_n_s_TypeError;
+  PyObject *__pyx_n_s__29;
+  PyObject *__pyx_n_s__3;
+  PyObject *__pyx_n_s_aggtyp;
+  PyObject *__pyx_n_s_asyncio_coroutines;
+  PyObject *__pyx_n_s_category;
+  PyObject *__pyx_n_s_cline_in_traceback;
+  PyObject *__pyx_n_s_cyaccess;
+  PyObject *__pyx_n_s_cyaccess___reduce_cython;
+  PyObject *__pyx_n_s_cyaccess___setstate_cython;
+  PyObject *__pyx_n_s_cyaccess_find_all_nearest_pois;
+  PyObject *__pyx_n_s_cyaccess_get_all_aggregate_acces;
+  PyObject *__pyx_n_s_cyaccess_get_available_aggregati;
+  PyObject *__pyx_n_s_cyaccess_get_available_decays;
+  PyObject *__pyx_n_s_cyaccess_initialize_access_var;
+  PyObject *__pyx_n_s_cyaccess_initialize_category;
+  PyObject *__pyx_n_s_cyaccess_nodes_in_range;
+  PyObject *__pyx_n_s_cyaccess_precompute_range;
+  PyObject *__pyx_n_s_cyaccess_shortest_path;
+  PyObject *__pyx_n_s_cyaccess_shortest_path_distance;
+  PyObject *__pyx_n_s_cyaccess_shortest_path_distances;
+  PyObject *__pyx_n_s_cyaccess_shortest_paths;
+  PyObject *__pyx_n_s_decay;
+  PyObject *__pyx_n_s_destnode;
+  PyObject *__pyx_n_s_destnodes;
+  PyObject *__pyx_kp_u_disable;
+  PyObject *__pyx_n_u_double;
+  PyObject *__pyx_n_s_dtype;
+  PyObject *__pyx_n_s_edge_weights;
+  PyObject *__pyx_n_s_edges;
+  PyObject *__pyx_n_s_empty_like;
+  PyObject *__pyx_kp_u_enable;
+  PyObject *__pyx_n_s_ext_ids;
+  PyObject *__pyx_n_s_find_all_nearest_pois;
+  PyObject *__pyx_kp_u_gc;
+  PyObject *__pyx_n_s_get_all_aggregate_accessibility;
+  PyObject *__pyx_n_s_get_available_aggregations;
+  PyObject *__pyx_n_s_get_available_decays;
+  PyObject *__pyx_n_s_getstate;
+  PyObject *__pyx_n_s_impno;
+  PyObject *__pyx_n_s_import;
+  PyObject *__pyx_n_s_initialize_access_var;
+  PyObject *__pyx_n_s_initialize_category;
+  PyObject *__pyx_n_s_initializing;
+  PyObject *__pyx_n_u_int;
+  PyObject *__pyx_n_s_is_coroutine;
+  PyObject *__pyx_kp_u_isenabled;
+  PyObject *__pyx_n_s_main;
+  PyObject *__pyx_n_s_maxdist;
+  PyObject *__pyx_n_s_maxitems;
+  PyObject *__pyx_n_s_name;
+  PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
+  PyObject *__pyx_n_s_node_ids;
+  PyObject *__pyx_n_s_node_xys;
+  PyObject *__pyx_n_s_nodes_in_range;
+  PyObject *__pyx_n_s_np;
+  PyObject *__pyx_n_s_num_of_pois;
+  PyObject *__pyx_n_s_numpy;
+  PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
+  PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
+  PyObject *__pyx_n_s_pandana_cyaccess;
+  PyObject *__pyx_n_s_precompute_range;
+  PyObject *__pyx_n_s_pyx_state;
+  PyObject *__pyx_n_s_radius;
+  PyObject *__pyx_n_s_range;
+  PyObject *__pyx_n_s_reduce;
+  PyObject *__pyx_n_s_reduce_cython;
+  PyObject *__pyx_n_s_reduce_ex;
+  PyObject *__pyx_n_s_ret;
+  PyObject *__pyx_n_s_self;
+  PyObject *__pyx_n_s_setstate;
+  PyObject *__pyx_n_s_setstate_cython;
+  PyObject *__pyx_n_s_shortest_path;
+  PyObject *__pyx_n_s_shortest_path_distance;
+  PyObject *__pyx_n_s_shortest_path_distances;
+  PyObject *__pyx_n_s_shortest_paths;
+  PyObject *__pyx_n_s_spec;
+  PyObject *__pyx_kp_s_src_cyaccess_pyx;
+  PyObject *__pyx_n_s_srcnode;
+  PyObject *__pyx_n_s_srcnodes;
+  PyObject *__pyx_kp_s_stringsource;
+  PyObject *__pyx_n_s_test;
+  PyObject *__pyx_n_s_twoway;
+  PyObject *__pyx_n_s_values;
+  PyObject *__pyx_n_s_zeros;
+  PyObject *__pyx_int_0;
+  PyObject *__pyx_tuple_;
+  PyObject *__pyx_tuple__2;
+  PyObject *__pyx_tuple__4;
+  PyObject *__pyx_tuple__6;
+  PyObject *__pyx_tuple__8;
+  PyObject *__pyx_tuple__9;
+  PyObject *__pyx_tuple__11;
+  PyObject *__pyx_tuple__14;
+  PyObject *__pyx_tuple__16;
+  PyObject *__pyx_tuple__18;
+  PyObject *__pyx_tuple__22;
+  PyObject *__pyx_tuple__24;
+  PyObject *__pyx_tuple__27;
+  PyObject *__pyx_codeobj__5;
+  PyObject *__pyx_codeobj__7;
+  PyObject *__pyx_codeobj__10;
+  PyObject *__pyx_codeobj__12;
+  PyObject *__pyx_codeobj__13;
+  PyObject *__pyx_codeobj__15;
+  PyObject *__pyx_codeobj__17;
+  PyObject *__pyx_codeobj__19;
+  PyObject *__pyx_codeobj__20;
+  PyObject *__pyx_codeobj__21;
+  PyObject *__pyx_codeobj__23;
+  PyObject *__pyx_codeobj__25;
+  PyObject *__pyx_codeobj__26;
+  PyObject *__pyx_codeobj__28;
+} __pyx_mstate;
+
+#if CYTHON_USE_MODULE_STATE
+#ifdef __cplusplus
+namespace {
+  extern struct PyModuleDef __pyx_moduledef;
+} /* anonymous namespace */
+#else
+static struct PyModuleDef __pyx_moduledef;
+#endif
+
+#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+
+#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
+
+#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
+#else
+static __pyx_mstate __pyx_mstate_global_static =
+#ifdef __cplusplus
+    {};
+#else
+    {0};
+#endif
+static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
+#endif
+/* #### Code section: module_state_clear ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_clear(PyObject *m) {
+  __pyx_mstate *clear_module_state = __pyx_mstate(m);
+  if (!clear_module_state) return 0;
+  Py_CLEAR(clear_module_state->__pyx_d);
+  Py_CLEAR(clear_module_state->__pyx_b);
+  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
+  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
+  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
+  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_CLEAR(clear_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_dtype);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_generic);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_number);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_integer);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_inexact);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_floating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_flexible);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_character);
+  Py_CLEAR(clear_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_CLEAR(clear_module_state->__pyx_ptype_7pandana_8cyaccess_cyaccess);
+  Py_CLEAR(clear_module_state->__pyx_type_7pandana_8cyaccess_cyaccess);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ImportError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
+  Py_CLEAR(clear_module_state->__pyx_n_s__29);
+  Py_CLEAR(clear_module_state->__pyx_n_s__3);
+  Py_CLEAR(clear_module_state->__pyx_n_s_aggtyp);
+  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_CLEAR(clear_module_state->__pyx_n_s_category);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess___reduce_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess___setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_find_all_nearest_pois);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_get_all_aggregate_acces);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_get_available_aggregati);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_get_available_decays);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_initialize_access_var);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_initialize_category);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_nodes_in_range);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_precompute_range);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_shortest_path);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_shortest_path_distance);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_shortest_path_distances);
+  Py_CLEAR(clear_module_state->__pyx_n_s_cyaccess_shortest_paths);
+  Py_CLEAR(clear_module_state->__pyx_n_s_decay);
+  Py_CLEAR(clear_module_state->__pyx_n_s_destnode);
+  Py_CLEAR(clear_module_state->__pyx_n_s_destnodes);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
+  Py_CLEAR(clear_module_state->__pyx_n_u_double);
+  Py_CLEAR(clear_module_state->__pyx_n_s_dtype);
+  Py_CLEAR(clear_module_state->__pyx_n_s_edge_weights);
+  Py_CLEAR(clear_module_state->__pyx_n_s_edges);
+  Py_CLEAR(clear_module_state->__pyx_n_s_empty_like);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ext_ids);
+  Py_CLEAR(clear_module_state->__pyx_n_s_find_all_nearest_pois);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get_all_aggregate_accessibility);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get_available_aggregations);
+  Py_CLEAR(clear_module_state->__pyx_n_s_get_available_decays);
+  Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_impno);
+  Py_CLEAR(clear_module_state->__pyx_n_s_import);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initialize_access_var);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initialize_category);
+  Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
+  Py_CLEAR(clear_module_state->__pyx_n_u_int);
+  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
+  Py_CLEAR(clear_module_state->__pyx_n_s_main);
+  Py_CLEAR(clear_module_state->__pyx_n_s_maxdist);
+  Py_CLEAR(clear_module_state->__pyx_n_s_maxitems);
+  Py_CLEAR(clear_module_state->__pyx_n_s_name);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
+  Py_CLEAR(clear_module_state->__pyx_n_s_node_ids);
+  Py_CLEAR(clear_module_state->__pyx_n_s_node_xys);
+  Py_CLEAR(clear_module_state->__pyx_n_s_nodes_in_range);
+  Py_CLEAR(clear_module_state->__pyx_n_s_np);
+  Py_CLEAR(clear_module_state->__pyx_n_s_num_of_pois);
+  Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
+  Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pandana_cyaccess);
+  Py_CLEAR(clear_module_state->__pyx_n_s_precompute_range);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
+  Py_CLEAR(clear_module_state->__pyx_n_s_radius);
+  Py_CLEAR(clear_module_state->__pyx_n_s_range);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ret);
+  Py_CLEAR(clear_module_state->__pyx_n_s_self);
+  Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
+  Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_shortest_path);
+  Py_CLEAR(clear_module_state->__pyx_n_s_shortest_path_distance);
+  Py_CLEAR(clear_module_state->__pyx_n_s_shortest_path_distances);
+  Py_CLEAR(clear_module_state->__pyx_n_s_shortest_paths);
+  Py_CLEAR(clear_module_state->__pyx_n_s_spec);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_src_cyaccess_pyx);
+  Py_CLEAR(clear_module_state->__pyx_n_s_srcnode);
+  Py_CLEAR(clear_module_state->__pyx_n_s_srcnodes);
+  Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
+  Py_CLEAR(clear_module_state->__pyx_n_s_test);
+  Py_CLEAR(clear_module_state->__pyx_n_s_twoway);
+  Py_CLEAR(clear_module_state->__pyx_n_s_values);
+  Py_CLEAR(clear_module_state->__pyx_n_s_zeros);
+  Py_CLEAR(clear_module_state->__pyx_int_0);
+  Py_CLEAR(clear_module_state->__pyx_tuple_);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
+  Py_CLEAR(clear_module_state->__pyx_tuple__4);
+  Py_CLEAR(clear_module_state->__pyx_tuple__6);
+  Py_CLEAR(clear_module_state->__pyx_tuple__8);
+  Py_CLEAR(clear_module_state->__pyx_tuple__9);
+  Py_CLEAR(clear_module_state->__pyx_tuple__11);
+  Py_CLEAR(clear_module_state->__pyx_tuple__14);
+  Py_CLEAR(clear_module_state->__pyx_tuple__16);
+  Py_CLEAR(clear_module_state->__pyx_tuple__18);
+  Py_CLEAR(clear_module_state->__pyx_tuple__22);
+  Py_CLEAR(clear_module_state->__pyx_tuple__24);
+  Py_CLEAR(clear_module_state->__pyx_tuple__27);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__5);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__7);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__12);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__13);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__15);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__17);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__19);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__20);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__21);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__23);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__25);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__26);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__28);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_traverse ### */
+#if CYTHON_USE_MODULE_STATE
+static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
+  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
+  if (!traverse_module_state) return 0;
+  Py_VISIT(traverse_module_state->__pyx_d);
+  Py_VISIT(traverse_module_state->__pyx_b);
+  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
+  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
+  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
+  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
+  #ifdef __Pyx_CyFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
+  #endif
+  #ifdef __Pyx_FusedFunction_USED
+  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
+  #endif
+  Py_VISIT(traverse_module_state->__pyx_ptype_7cpython_4type_type);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_dtype);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flatiter);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_broadcast);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ndarray);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_generic);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_number);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_integer);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_signedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_unsignedinteger);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_inexact);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_floating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_complexfloating);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_flexible);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_character);
+  Py_VISIT(traverse_module_state->__pyx_ptype_5numpy_ufunc);
+  Py_VISIT(traverse_module_state->__pyx_ptype_7pandana_8cyaccess_cyaccess);
+  Py_VISIT(traverse_module_state->__pyx_type_7pandana_8cyaccess_cyaccess);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ImportError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
+  Py_VISIT(traverse_module_state->__pyx_n_s__29);
+  Py_VISIT(traverse_module_state->__pyx_n_s__3);
+  Py_VISIT(traverse_module_state->__pyx_n_s_aggtyp);
+  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
+  Py_VISIT(traverse_module_state->__pyx_n_s_category);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess___reduce_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess___setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_find_all_nearest_pois);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_get_all_aggregate_acces);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_get_available_aggregati);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_get_available_decays);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_initialize_access_var);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_initialize_category);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_nodes_in_range);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_precompute_range);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_shortest_path);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_shortest_path_distance);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_shortest_path_distances);
+  Py_VISIT(traverse_module_state->__pyx_n_s_cyaccess_shortest_paths);
+  Py_VISIT(traverse_module_state->__pyx_n_s_decay);
+  Py_VISIT(traverse_module_state->__pyx_n_s_destnode);
+  Py_VISIT(traverse_module_state->__pyx_n_s_destnodes);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
+  Py_VISIT(traverse_module_state->__pyx_n_u_double);
+  Py_VISIT(traverse_module_state->__pyx_n_s_dtype);
+  Py_VISIT(traverse_module_state->__pyx_n_s_edge_weights);
+  Py_VISIT(traverse_module_state->__pyx_n_s_edges);
+  Py_VISIT(traverse_module_state->__pyx_n_s_empty_like);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ext_ids);
+  Py_VISIT(traverse_module_state->__pyx_n_s_find_all_nearest_pois);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get_all_aggregate_accessibility);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get_available_aggregations);
+  Py_VISIT(traverse_module_state->__pyx_n_s_get_available_decays);
+  Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_impno);
+  Py_VISIT(traverse_module_state->__pyx_n_s_import);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initialize_access_var);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initialize_category);
+  Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
+  Py_VISIT(traverse_module_state->__pyx_n_u_int);
+  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
+  Py_VISIT(traverse_module_state->__pyx_n_s_main);
+  Py_VISIT(traverse_module_state->__pyx_n_s_maxdist);
+  Py_VISIT(traverse_module_state->__pyx_n_s_maxitems);
+  Py_VISIT(traverse_module_state->__pyx_n_s_name);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_no_default___reduce___due_to_non);
+  Py_VISIT(traverse_module_state->__pyx_n_s_node_ids);
+  Py_VISIT(traverse_module_state->__pyx_n_s_node_xys);
+  Py_VISIT(traverse_module_state->__pyx_n_s_nodes_in_range);
+  Py_VISIT(traverse_module_state->__pyx_n_s_np);
+  Py_VISIT(traverse_module_state->__pyx_n_s_num_of_pois);
+  Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
+  Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pandana_cyaccess);
+  Py_VISIT(traverse_module_state->__pyx_n_s_precompute_range);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
+  Py_VISIT(traverse_module_state->__pyx_n_s_radius);
+  Py_VISIT(traverse_module_state->__pyx_n_s_range);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ret);
+  Py_VISIT(traverse_module_state->__pyx_n_s_self);
+  Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
+  Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_shortest_path);
+  Py_VISIT(traverse_module_state->__pyx_n_s_shortest_path_distance);
+  Py_VISIT(traverse_module_state->__pyx_n_s_shortest_path_distances);
+  Py_VISIT(traverse_module_state->__pyx_n_s_shortest_paths);
+  Py_VISIT(traverse_module_state->__pyx_n_s_spec);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_src_cyaccess_pyx);
+  Py_VISIT(traverse_module_state->__pyx_n_s_srcnode);
+  Py_VISIT(traverse_module_state->__pyx_n_s_srcnodes);
+  Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
+  Py_VISIT(traverse_module_state->__pyx_n_s_test);
+  Py_VISIT(traverse_module_state->__pyx_n_s_twoway);
+  Py_VISIT(traverse_module_state->__pyx_n_s_values);
+  Py_VISIT(traverse_module_state->__pyx_n_s_zeros);
+  Py_VISIT(traverse_module_state->__pyx_int_0);
+  Py_VISIT(traverse_module_state->__pyx_tuple_);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
+  Py_VISIT(traverse_module_state->__pyx_tuple__4);
+  Py_VISIT(traverse_module_state->__pyx_tuple__6);
+  Py_VISIT(traverse_module_state->__pyx_tuple__8);
+  Py_VISIT(traverse_module_state->__pyx_tuple__9);
+  Py_VISIT(traverse_module_state->__pyx_tuple__11);
+  Py_VISIT(traverse_module_state->__pyx_tuple__14);
+  Py_VISIT(traverse_module_state->__pyx_tuple__16);
+  Py_VISIT(traverse_module_state->__pyx_tuple__18);
+  Py_VISIT(traverse_module_state->__pyx_tuple__22);
+  Py_VISIT(traverse_module_state->__pyx_tuple__24);
+  Py_VISIT(traverse_module_state->__pyx_tuple__27);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__5);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__7);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__12);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__13);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__15);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__17);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__19);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__20);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__21);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__23);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__25);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__26);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__28);
+  return 0;
+}
+#endif
+/* #### Code section: module_state_defines ### */
+#define __pyx_d __pyx_mstate_global->__pyx_d
+#define __pyx_b __pyx_mstate_global->__pyx_b
+#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
+#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
+#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
+#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
+#ifdef __Pyx_CyFunction_USED
+#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
+#endif
+#ifdef __Pyx_FusedFunction_USED
+#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
+#endif
+#ifdef __Pyx_Generator_USED
+#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
+#endif
+#ifdef __Pyx_IterableCoroutine_USED
+#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
+#endif
+#ifdef __Pyx_Coroutine_USED
+#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_7cpython_4type_type __pyx_mstate_global->__pyx_ptype_7cpython_4type_type
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#if CYTHON_USE_MODULE_STATE
+#endif
+#define __pyx_ptype_5numpy_dtype __pyx_mstate_global->__pyx_ptype_5numpy_dtype
+#define __pyx_ptype_5numpy_flatiter __pyx_mstate_global->__pyx_ptype_5numpy_flatiter
+#define __pyx_ptype_5numpy_broadcast __pyx_mstate_global->__pyx_ptype_5numpy_broadcast
+#define __pyx_ptype_5numpy_ndarray __pyx_mstate_global->__pyx_ptype_5numpy_ndarray
+#define __pyx_ptype_5numpy_generic __pyx_mstate_global->__pyx_ptype_5numpy_generic
+#define __pyx_ptype_5numpy_number __pyx_mstate_global->__pyx_ptype_5numpy_number
+#define __pyx_ptype_5numpy_integer __pyx_mstate_global->__pyx_ptype_5numpy_integer
+#define __pyx_ptype_5numpy_signedinteger __pyx_mstate_global->__pyx_ptype_5numpy_signedinteger
+#define __pyx_ptype_5numpy_unsignedinteger __pyx_mstate_global->__pyx_ptype_5numpy_unsignedinteger
+#define __pyx_ptype_5numpy_inexact __pyx_mstate_global->__pyx_ptype_5numpy_inexact
+#define __pyx_ptype_5numpy_floating __pyx_mstate_global->__pyx_ptype_5numpy_floating
+#define __pyx_ptype_5numpy_complexfloating __pyx_mstate_global->__pyx_ptype_5numpy_complexfloating
+#define __pyx_ptype_5numpy_flexible __pyx_mstate_global->__pyx_ptype_5numpy_flexible
+#define __pyx_ptype_5numpy_character __pyx_mstate_global->__pyx_ptype_5numpy_character
+#define __pyx_ptype_5numpy_ufunc __pyx_mstate_global->__pyx_ptype_5numpy_ufunc
+#if CYTHON_USE_MODULE_STATE
+#define __pyx_type_7pandana_8cyaccess_cyaccess __pyx_mstate_global->__pyx_type_7pandana_8cyaccess_cyaccess
+#endif
+#define __pyx_ptype_7pandana_8cyaccess_cyaccess __pyx_mstate_global->__pyx_ptype_7pandana_8cyaccess_cyaccess
+#define __pyx_n_s_ImportError __pyx_mstate_global->__pyx_n_s_ImportError
+#define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
+#define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
+#define __pyx_n_s__29 __pyx_mstate_global->__pyx_n_s__29
+#define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
+#define __pyx_n_s_aggtyp __pyx_mstate_global->__pyx_n_s_aggtyp
+#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
+#define __pyx_n_s_category __pyx_mstate_global->__pyx_n_s_category
+#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
+#define __pyx_n_s_cyaccess __pyx_mstate_global->__pyx_n_s_cyaccess
+#define __pyx_n_s_cyaccess___reduce_cython __pyx_mstate_global->__pyx_n_s_cyaccess___reduce_cython
+#define __pyx_n_s_cyaccess___setstate_cython __pyx_mstate_global->__pyx_n_s_cyaccess___setstate_cython
+#define __pyx_n_s_cyaccess_find_all_nearest_pois __pyx_mstate_global->__pyx_n_s_cyaccess_find_all_nearest_pois
+#define __pyx_n_s_cyaccess_get_all_aggregate_acces __pyx_mstate_global->__pyx_n_s_cyaccess_get_all_aggregate_acces
+#define __pyx_n_s_cyaccess_get_available_aggregati __pyx_mstate_global->__pyx_n_s_cyaccess_get_available_aggregati
+#define __pyx_n_s_cyaccess_get_available_decays __pyx_mstate_global->__pyx_n_s_cyaccess_get_available_decays
+#define __pyx_n_s_cyaccess_initialize_access_var __pyx_mstate_global->__pyx_n_s_cyaccess_initialize_access_var
+#define __pyx_n_s_cyaccess_initialize_category __pyx_mstate_global->__pyx_n_s_cyaccess_initialize_category
+#define __pyx_n_s_cyaccess_nodes_in_range __pyx_mstate_global->__pyx_n_s_cyaccess_nodes_in_range
+#define __pyx_n_s_cyaccess_precompute_range __pyx_mstate_global->__pyx_n_s_cyaccess_precompute_range
+#define __pyx_n_s_cyaccess_shortest_path __pyx_mstate_global->__pyx_n_s_cyaccess_shortest_path
+#define __pyx_n_s_cyaccess_shortest_path_distance __pyx_mstate_global->__pyx_n_s_cyaccess_shortest_path_distance
+#define __pyx_n_s_cyaccess_shortest_path_distances __pyx_mstate_global->__pyx_n_s_cyaccess_shortest_path_distances
+#define __pyx_n_s_cyaccess_shortest_paths __pyx_mstate_global->__pyx_n_s_cyaccess_shortest_paths
+#define __pyx_n_s_decay __pyx_mstate_global->__pyx_n_s_decay
+#define __pyx_n_s_destnode __pyx_mstate_global->__pyx_n_s_destnode
+#define __pyx_n_s_destnodes __pyx_mstate_global->__pyx_n_s_destnodes
+#define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
+#define __pyx_n_u_double __pyx_mstate_global->__pyx_n_u_double
+#define __pyx_n_s_dtype __pyx_mstate_global->__pyx_n_s_dtype
+#define __pyx_n_s_edge_weights __pyx_mstate_global->__pyx_n_s_edge_weights
+#define __pyx_n_s_edges __pyx_mstate_global->__pyx_n_s_edges
+#define __pyx_n_s_empty_like __pyx_mstate_global->__pyx_n_s_empty_like
+#define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
+#define __pyx_n_s_ext_ids __pyx_mstate_global->__pyx_n_s_ext_ids
+#define __pyx_n_s_find_all_nearest_pois __pyx_mstate_global->__pyx_n_s_find_all_nearest_pois
+#define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
+#define __pyx_n_s_get_all_aggregate_accessibility __pyx_mstate_global->__pyx_n_s_get_all_aggregate_accessibility
+#define __pyx_n_s_get_available_aggregations __pyx_mstate_global->__pyx_n_s_get_available_aggregations
+#define __pyx_n_s_get_available_decays __pyx_mstate_global->__pyx_n_s_get_available_decays
+#define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
+#define __pyx_n_s_impno __pyx_mstate_global->__pyx_n_s_impno
+#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
+#define __pyx_n_s_initialize_access_var __pyx_mstate_global->__pyx_n_s_initialize_access_var
+#define __pyx_n_s_initialize_category __pyx_mstate_global->__pyx_n_s_initialize_category
+#define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
+#define __pyx_n_u_int __pyx_mstate_global->__pyx_n_u_int
+#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
+#define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
+#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
+#define __pyx_n_s_maxdist __pyx_mstate_global->__pyx_n_s_maxdist
+#define __pyx_n_s_maxitems __pyx_mstate_global->__pyx_n_s_maxitems
+#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
+#define __pyx_kp_s_no_default___reduce___due_to_non __pyx_mstate_global->__pyx_kp_s_no_default___reduce___due_to_non
+#define __pyx_n_s_node_ids __pyx_mstate_global->__pyx_n_s_node_ids
+#define __pyx_n_s_node_xys __pyx_mstate_global->__pyx_n_s_node_xys
+#define __pyx_n_s_nodes_in_range __pyx_mstate_global->__pyx_n_s_nodes_in_range
+#define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
+#define __pyx_n_s_num_of_pois __pyx_mstate_global->__pyx_n_s_num_of_pois
+#define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
+#define __pyx_kp_u_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy_core_multiarray_failed_to
+#define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
+#define __pyx_n_s_pandana_cyaccess __pyx_mstate_global->__pyx_n_s_pandana_cyaccess
+#define __pyx_n_s_precompute_range __pyx_mstate_global->__pyx_n_s_precompute_range
+#define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
+#define __pyx_n_s_radius __pyx_mstate_global->__pyx_n_s_radius
+#define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
+#define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
+#define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
+#define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
+#define __pyx_n_s_ret __pyx_mstate_global->__pyx_n_s_ret
+#define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
+#define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
+#define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
+#define __pyx_n_s_shortest_path __pyx_mstate_global->__pyx_n_s_shortest_path
+#define __pyx_n_s_shortest_path_distance __pyx_mstate_global->__pyx_n_s_shortest_path_distance
+#define __pyx_n_s_shortest_path_distances __pyx_mstate_global->__pyx_n_s_shortest_path_distances
+#define __pyx_n_s_shortest_paths __pyx_mstate_global->__pyx_n_s_shortest_paths
+#define __pyx_n_s_spec __pyx_mstate_global->__pyx_n_s_spec
+#define __pyx_kp_s_src_cyaccess_pyx __pyx_mstate_global->__pyx_kp_s_src_cyaccess_pyx
+#define __pyx_n_s_srcnode __pyx_mstate_global->__pyx_n_s_srcnode
+#define __pyx_n_s_srcnodes __pyx_mstate_global->__pyx_n_s_srcnodes
+#define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
+#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
+#define __pyx_n_s_twoway __pyx_mstate_global->__pyx_n_s_twoway
+#define __pyx_n_s_values __pyx_mstate_global->__pyx_n_s_values
+#define __pyx_n_s_zeros __pyx_mstate_global->__pyx_n_s_zeros
+#define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
+#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
+#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
+#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
+#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
+#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
+#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
+#define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
+#define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
+#define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
+#define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
+#define __pyx_tuple__24 __pyx_mstate_global->__pyx_tuple__24
+#define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
+#define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
+#define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
+#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
+#define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
+#define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
+#define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
+#define __pyx_codeobj__17 __pyx_mstate_global->__pyx_codeobj__17
+#define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
+#define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
+#define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
+#define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
+#define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
+#define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
+#define __pyx_codeobj__28 __pyx_mstate_global->__pyx_codeobj__28
+/* #### Code section: module_code ### */
+
+/* "string.from_py":13
+ * 
+ * @cname("__pyx_convert_string_from_py_std__in_string")
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ */
+
+static std::string __pyx_convert_string_from_py_std__in_string(PyObject *__pyx_v_o) {
+  Py_ssize_t __pyx_v_length;
+  char const *__pyx_v_data;
+  std::string __pyx_r;
+  __Pyx_RefNannyDeclarations
+  char const *__pyx_t_1;
+  std::string __pyx_t_2;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_string_from_py_std__in_string", 0);
+
+  /* "string.from_py":14
+ * @cname("__pyx_convert_string_from_py_std__in_string")
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
+ *     cdef Py_ssize_t length = 0             # <<<<<<<<<<<<<<
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ *     return string(data, length)
+ */
+  __pyx_v_length = 0;
+
+  /* "string.from_py":15
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)             # <<<<<<<<<<<<<<
+ *     return string(data, length)
+ * 
+ */
+  __pyx_t_1 = __Pyx_PyObject_AsStringAndSize(__pyx_v_o, (&__pyx_v_length)); if (unlikely(__pyx_t_1 == ((char const *)NULL))) __PYX_ERR(1, 15, __pyx_L1_error)
+  __pyx_v_data = __pyx_t_1;
+
+  /* "string.from_py":16
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ *     return string(data, length)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  try {
+    __pyx_t_2 = std::string(__pyx_v_data, __pyx_v_length);
+  } catch(...) {
+    __Pyx_CppExn2PyErr();
+    __PYX_ERR(1, 16, __pyx_L1_error)
+  }
+  __pyx_r = __pyx_t_2;
+  goto __pyx_L0;
+
+  /* "string.from_py":13
+ * 
+ * @cname("__pyx_convert_string_from_py_std__in_string")
+ * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t length = 0
+ *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_long")
+ * cdef vector[X] __pyx_convert_vector_from_py_long(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+static std::vector<long>  __pyx_convert_vector_from_py_long(PyObject *__pyx_v_o) {
+  std::vector<long>  __pyx_v_v;
+  PyObject *__pyx_v_item = NULL;
+  std::vector<long>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  long __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_long", 0);
+
+  /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_long(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
+    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(1, 47, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "vector.from_py":48
+ *     cdef vector[X] v
+ *     for item in o:
+ *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
+ *     return v
+ * 
+ */
+    __pyx_t_5 = __Pyx_PyInt_As_long(__pyx_v_item); if (unlikely((__pyx_t_5 == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
+    try {
+      __pyx_v_v.push_back(((long)__pyx_t_5));
+    } catch(...) {
+      __Pyx_CppExn2PyErr();
+      __PYX_ERR(1, 48, __pyx_L1_error)
+    }
+
+    /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_long(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "vector.from_py":49
+ *     for item in o:
+ *         v.push_back(<X>item)
+ *     return v             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_v;
+  goto __pyx_L0;
+
+  /* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_long")
+ * cdef vector[X] __pyx_convert_vector_from_py_long(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_long", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_double")
+ * cdef object __pyx_convert_vector_to_py_double(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+static PyObject *__pyx_convert_vector_to_py_double(std::vector<double>  const &__pyx_v_v) {
+  Py_ssize_t __pyx_v_v_size_signed;
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_double", 0);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_double")
+ * cdef object __pyx_convert_vector_to_py_double(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py_double(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_double")
+ * cdef object __pyx_convert_vector_to_py_double(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  }
+
+  /* "vector.to_py":69
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(v_size_signed)
+ */
+  __pyx_v_v_size_signed = ((Py_ssize_t)__pyx_v_v.size());
+
+  /* "vector.to_py":71
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ *     o = PyList_New(v_size_signed)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(__pyx_v_v_size_signed); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":76
+ *     cdef object item
+ * 
+ *     for i in range(v_size_signed):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v_size_signed;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":77
+ * 
+ *     for i in range(v_size_signed):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":78
+ *     for i in range(v_size_signed):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":79
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":81
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_double")
+ * cdef object __pyx_convert_vector_to_py_double(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(std::vector<std::vector<double> >  const &__pyx_v_v) {
+  Py_ssize_t __pyx_v_v_size_signed;
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___", 0);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  }
+
+  /* "vector.to_py":69
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(v_size_signed)
+ */
+  __pyx_v_v_size_signed = ((Py_ssize_t)__pyx_v_v.size());
+
+  /* "vector.to_py":71
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ *     o = PyList_New(v_size_signed)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(__pyx_v_v_size_signed); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":76
+ *     cdef object item
+ * 
+ *     for i in range(v_size_signed):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v_size_signed;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":77
+ * 
+ *     for i in range(v_size_signed):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = __pyx_convert_vector_to_py_double((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":78
+ *     for i in range(v_size_signed):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":79
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":81
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_convert_vector_to_py_int(std::vector<int>  const &__pyx_v_v) {
+  Py_ssize_t __pyx_v_v_size_signed;
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_int", 0);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_int")
+ * cdef object __pyx_convert_vector_to_py_int(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py_int(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_int")
+ * cdef object __pyx_convert_vector_to_py_int(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  }
+
+  /* "vector.to_py":69
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(v_size_signed)
+ */
+  __pyx_v_v_size_signed = ((Py_ssize_t)__pyx_v_v.size());
+
+  /* "vector.to_py":71
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ *     o = PyList_New(v_size_signed)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(__pyx_v_v_size_signed); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":76
+ *     cdef object item
+ * 
+ *     for i in range(v_size_signed):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v_size_signed;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":77
+ * 
+ *     for i in range(v_size_signed):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = __Pyx_PyInt_From_int((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":78
+ *     for i in range(v_size_signed):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":79
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":81
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_int")
+ * cdef object __pyx_convert_vector_to_py_int(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(std::vector<std::vector<int> >  const &__pyx_v_v) {
+  Py_ssize_t __pyx_v_v_size_signed;
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___", 0);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  }
+
+  /* "vector.to_py":69
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(v_size_signed)
+ */
+  __pyx_v_v_size_signed = ((Py_ssize_t)__pyx_v_v.size());
+
+  /* "vector.to_py":71
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ *     o = PyList_New(v_size_signed)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(__pyx_v_v_size_signed); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":76
+ *     cdef object item
+ * 
+ *     for i in range(v_size_signed):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v_size_signed;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":77
+ * 
+ *     for i in range(v_size_signed):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = __pyx_convert_vector_to_py_int((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":78
+ *     for i in range(v_size_signed):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":79
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":81
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___")
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+static std::vector<std::vector<long> >  __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(PyObject *__pyx_v_o) {
+  std::vector<std::vector<long> >  __pyx_v_v;
+  PyObject *__pyx_v_item = NULL;
+  std::vector<std::vector<long> >  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  std::vector<long>  __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___", 0);
+
+  /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
+    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(1, 47, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "vector.from_py":48
+ *     cdef vector[X] v
+ *     for item in o:
+ *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
+ *     return v
+ * 
+ */
+    __pyx_t_5 = __pyx_convert_vector_from_py_long(__pyx_v_item); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
+    try {
+      __pyx_v_v.push_back(((std::vector<long> )__pyx_t_5));
+    } catch(...) {
+      __Pyx_CppExn2PyErr();
+      __PYX_ERR(1, 48, __pyx_L1_error)
+    }
+
+    /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "vector.from_py":49
+ *     for item in o:
+ *         v.push_back(<X>item)
+ *     return v             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_v;
+  goto __pyx_L0;
+
+  /* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___")
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static std::vector<double>  __pyx_convert_vector_from_py_double(PyObject *__pyx_v_o) {
+  std::vector<double>  __pyx_v_v;
+  PyObject *__pyx_v_item = NULL;
+  std::vector<double>  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  double __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_double", 0);
+
+  /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_double(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
+    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(1, 47, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "vector.from_py":48
+ *     cdef vector[X] v
+ *     for item in o:
+ *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
+ *     return v
+ * 
+ */
+    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_v_item); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
+    try {
+      __pyx_v_v.push_back(((double)__pyx_t_5));
+    } catch(...) {
+      __Pyx_CppExn2PyErr();
+      __PYX_ERR(1, 48, __pyx_L1_error)
+    }
+
+    /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_double(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "vector.from_py":49
+ *     for item in o:
+ *         v.push_back(<X>item)
+ *     return v             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_v;
+  goto __pyx_L0;
+
+  /* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_double")
+ * cdef vector[X] __pyx_convert_vector_from_py_double(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static std::vector<std::vector<double> >  __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(PyObject *__pyx_v_o) {
+  std::vector<std::vector<double> >  __pyx_v_v;
+  PyObject *__pyx_v_item = NULL;
+  std::vector<std::vector<double> >  __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  PyObject *(*__pyx_t_3)(PyObject *);
+  PyObject *__pyx_t_4 = NULL;
+  std::vector<double>  __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___", 0);
+
+  /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
+    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
+    __pyx_t_3 = NULL;
+  } else {
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_3)) {
+      if (likely(PyList_CheckExact(__pyx_t_1))) {
+        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      } else {
+        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(1, 47, __pyx_L1_error)
+        #else
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        #endif
+      }
+    } else {
+      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
+      if (unlikely(!__pyx_t_4)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(1, 47, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_4);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
+    __pyx_t_4 = 0;
+
+    /* "vector.from_py":48
+ *     cdef vector[X] v
+ *     for item in o:
+ *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
+ *     return v
+ * 
+ */
+    __pyx_t_5 = __pyx_convert_vector_from_py_double(__pyx_v_item); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
+    try {
+      __pyx_v_v.push_back(((std::vector<double> )__pyx_t_5));
+    } catch(...) {
+      __Pyx_CppExn2PyErr();
+      __PYX_ERR(1, 48, __pyx_L1_error)
+    }
+
+    /* "vector.from_py":47
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(object o) except *:
+ *     cdef vector[X] v
+ *     for item in o:             # <<<<<<<<<<<<<<
+ *         v.push_back(<X>item)
+ *     return v
+ */
+  }
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "vector.from_py":49
+ *     for item in o:
+ *         v.push_back(<X>item)
+ *     return v             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = __pyx_v_v;
+  goto __pyx_L0;
+
+  /* "vector.from_py":45
+ * 
+ * @cname("__pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___")
+ * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(object o) except *:             # <<<<<<<<<<<<<<
+ *     cdef vector[X] v
+ *     for item in o:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":31
+ * 
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":32
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyObject_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":31
+ * 
+ * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":37
+ * 
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":38
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyUnicode_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 38, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
 
-/* "src/cyaccess.pyx":33
+  /* "string.to_py":37
+ * 
+ * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":43
+ * 
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":44
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyStr_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 44, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":43
+ * 
+ * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":49
+ * 
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":50
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * cdef extern from *:
+ *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":49
+ * 
+ * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
+ * cdef extern from *:
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "string.to_py":55
+ * 
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &__pyx_v_s) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 0);
+
+  /* "string.to_py":56
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyByteArray_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 56, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "string.to_py":55
+ * 
+ * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
+ * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
+ *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_string(std::vector<std::string>  const &__pyx_v_v) {
+  Py_ssize_t __pyx_v_v_size_signed;
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_std_3a__3a_string", 0);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  }
+
+  /* "vector.to_py":69
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(v_size_signed)
+ */
+  __pyx_v_v_size_signed = ((Py_ssize_t)__pyx_v_v.size());
+
+  /* "vector.to_py":71
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ *     o = PyList_New(v_size_signed)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(__pyx_v_v_size_signed); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":76
+ *     cdef object item
+ * 
+ *     for i in range(v_size_signed):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v_size_signed;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":77
+ * 
+ *     for i in range(v_size_signed):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":78
+ *     for i in range(v_size_signed):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":79
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":81
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_std_3a__3a_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "pair.to_py":190
+ * 
+ * @cname("__pyx_convert_pair_to_py_long____float")
+ * cdef object __pyx_convert_pair_to_py_long____float(const pair[X,Y]& p):             # <<<<<<<<<<<<<<
+ *     return p.first, p.second
+ * 
+ */
+
+static PyObject *__pyx_convert_pair_to_py_long____float(std::pair<long,float>  const &__pyx_v_p) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_pair_to_py_long____float", 0);
+
+  /* "pair.to_py":191
+ * @cname("__pyx_convert_pair_to_py_long____float")
+ * cdef object __pyx_convert_pair_to_py_long____float(const pair[X,Y]& p):
+ *     return p.first, p.second             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v_p.first); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 191, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = PyFloat_FromDouble(__pyx_v_p.second); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 191, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 191, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
+  __pyx_t_1 = 0;
+  __pyx_t_2 = 0;
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* "pair.to_py":190
+ * 
+ * @cname("__pyx_convert_pair_to_py_long____float")
+ * cdef object __pyx_convert_pair_to_py_long____float(const pair[X,Y]& p):             # <<<<<<<<<<<<<<
+ *     return p.first, p.second
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("pair.to_py.__pyx_convert_pair_to_py_long____float", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___(std::vector<std::pair<long,float> >  const &__pyx_v_v) {
+  Py_ssize_t __pyx_v_v_size_signed;
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___", 0);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  }
+
+  /* "vector.to_py":69
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(v_size_signed)
+ */
+  __pyx_v_v_size_signed = ((Py_ssize_t)__pyx_v_v.size());
+
+  /* "vector.to_py":71
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ *     o = PyList_New(v_size_signed)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(__pyx_v_v_size_signed); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":76
+ *     cdef object item
+ * 
+ *     for i in range(v_size_signed):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v_size_signed;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":77
+ * 
+ *     for i in range(v_size_signed):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = __pyx_convert_pair_to_py_long____float((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":78
+ *     for i in range(v_size_signed):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":79
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":81
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___(std::vector<std::vector<std::pair<long,float> > >  const &__pyx_v_v) {
+  Py_ssize_t __pyx_v_v_size_signed;
+  PyObject *__pyx_v_o = NULL;
+  Py_ssize_t __pyx_v_i;
+  PyObject *__pyx_v_item = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___", 0);
+
+  /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  __pyx_t_1 = (__pyx_v_v.size() > ((size_t)PY_SSIZE_T_MAX));
+  if (unlikely(__pyx_t_1)) {
+
+    /* "vector.to_py":68
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()             # <<<<<<<<<<<<<<
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ */
+    PyErr_NoMemory(); __PYX_ERR(1, 68, __pyx_L1_error)
+
+    /* "vector.to_py":67
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___(const vector[X]& v):
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:             # <<<<<<<<<<<<<<
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()
+ */
+  }
+
+  /* "vector.to_py":69
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ *     v_size_signed = <Py_ssize_t> v.size()             # <<<<<<<<<<<<<<
+ * 
+ *     o = PyList_New(v_size_signed)
+ */
+  __pyx_v_v_size_signed = ((Py_ssize_t)__pyx_v_v.size());
+
+  /* "vector.to_py":71
+ *     v_size_signed = <Py_ssize_t> v.size()
+ * 
+ *     o = PyList_New(v_size_signed)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef Py_ssize_t i
+ */
+  __pyx_t_2 = PyList_New(__pyx_v_v_size_signed); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 71, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_o = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "vector.to_py":76
+ *     cdef object item
+ * 
+ *     for i in range(v_size_signed):             # <<<<<<<<<<<<<<
+ *         item = v[i]
+ *         Py_INCREF(item)
+ */
+  __pyx_t_3 = __pyx_v_v_size_signed;
+  __pyx_t_4 = __pyx_t_3;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "vector.to_py":77
+ * 
+ *     for i in range(v_size_signed):
+ *         item = v[i]             # <<<<<<<<<<<<<<
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)
+ */
+    __pyx_t_2 = __pyx_convert_vector_to_py_std_3a__3a_pair_3c_long_2c_float_3e___((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 77, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_2);
+    __pyx_t_2 = 0;
+
+    /* "vector.to_py":78
+ *     for i in range(v_size_signed):
+ *         item = v[i]
+ *         Py_INCREF(item)             # <<<<<<<<<<<<<<
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ */
+    Py_INCREF(__pyx_v_item);
+
+    /* "vector.to_py":79
+ *         item = v[i]
+ *         Py_INCREF(item)
+ *         PyList_SET_ITEM(o, i, item)             # <<<<<<<<<<<<<<
+ * 
+ *     return o
+ */
+    PyList_SET_ITEM(__pyx_v_o, __pyx_v_i, __pyx_v_item);
+  }
+
+  /* "vector.to_py":81
+ *         PyList_SET_ITEM(o, i, item)
+ * 
+ *     return o             # <<<<<<<<<<<<<<
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_o);
+  __pyx_r = __pyx_v_o;
+  goto __pyx_L0;
+
+  /* "vector.to_py":66
+ * 
+ * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___")
+ * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___(const vector[X]& v):             # <<<<<<<<<<<<<<
+ *     if v.size() > <size_t> PY_SSIZE_T_MAX:
+ *         raise MemoryError()
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_o);
+  __Pyx_XDECREF(__pyx_v_item);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
+  PyObject *__pyx_r;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_BASE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+ * 
+ *         @property
+ *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a borrowed reference to the object owning the data/memory.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+ * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ */
+
+static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
+  PyArray_Descr *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyArray_Descr *__pyx_t_1;
+  __Pyx_RefNannySetupContext("descr", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __Pyx_XDECREF((PyObject *)__pyx_r);
+  __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
+  __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
+  __pyx_r = ((PyArray_Descr *)__pyx_t_1);
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+ * 
+ *         @property
+ *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
+ *             """Returns an owned reference to the dtype of the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF((PyObject *)__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+ * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
+  int __pyx_r;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+ *             """Returns the number of dimensions in the array.
+ *             """
+ *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_NDIM(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+ * 
+ *         @property
+ *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the number of dimensions in the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+ * 
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+ *             Can return NULL for 0-dimensional arrays.
+ *             """
+ *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_DIMS(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+ * 
+ *         @property
+ *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the dimensions/shape of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+ * 
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
+  npy_intp *__pyx_r;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ *             """
+ *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_STRIDES(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+ * 
+ *         @property
+ *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns a pointer to the strides of the array.
+ *             The number of elements matches the number of dimensions of the array (ndim).
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ */
+
+static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
+  npy_intp __pyx_r;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
+ * 
+ *         @property
+ */
+  __pyx_r = PyArray_SIZE(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+ * 
+ *         @property
+ *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
+ *             """Returns the total size (in number of elements) of the array.
+ *             """
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+ * 
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
+ */
+
+static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
+  char *__pyx_r;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+ *             of `PyArray_DATA()` instead, which returns a 'void*'.
+ *             """
+ *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
+ * 
+ *     ctypedef unsigned char      npy_bool
+ */
+  __pyx_r = PyArray_BYTES(__pyx_v_self);
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+ * 
+ *         @property
+ *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
+ *             """The pointer to the data buffer as a char*.
+ *             This is provided for legacy reasons to avoid direct struct field access.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):
+ *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+ * ctypedef npy_cdouble     complex_t
+ * 
+ * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+ *     return PyArray_MultiIterNew(1, <void*>a)
+ * 
+ * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+ *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
+ * 
+ * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+ *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
+ * 
+ * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+ *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
+ * 
+ * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
+  if (__pyx_t_1) {
+
+    /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
+ *     else:
+ *         return ()
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
+    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
+    goto __pyx_L0;
+
+    /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):
+ *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
+ *         return <tuple>d.subarray.shape
+ *     else:
+ */
+  }
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+ *         return <tuple>d.subarray.shape
+ *     else:
+ *         return ()             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  /*else*/ {
+    __Pyx_XDECREF(__pyx_r);
+    __Pyx_INCREF(__pyx_empty_tuple);
+    __pyx_r = __pyx_empty_tuple;
+    goto __pyx_L0;
+  }
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+ *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
+ * 
+ * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
+ *     if PyDataType_HASSUBARRAY(d):
+ *         return <tuple>d.subarray.shape
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+
+static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("set_array_base", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ */
+  Py_INCREF(__pyx_v_base);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+ * cdef inline void set_array_base(ndarray arr, object base):
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline object get_array_base(ndarray arr):
+ */
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+ *     int _import_umath() except -1
+ * 
+ * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
+ *     Py_INCREF(base) # important to do this before stealing the reference below!
+ *     PyArray_SetBaseObject(arr, base)
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+
+static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
+  PyObject *__pyx_v_base;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  __Pyx_RefNannySetupContext("get_array_base", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+ * 
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
+ *     if base is NULL:
+ *         return None
+ */
+  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  __pyx_t_1 = (__pyx_v_base == NULL);
+  if (__pyx_t_1) {
+
+    /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ *         return None             # <<<<<<<<<<<<<<
+ *     return <object>base
+ * 
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+    goto __pyx_L0;
+
+    /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+ * cdef inline object get_array_base(ndarray arr):
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:             # <<<<<<<<<<<<<<
+ *         return None
+ *     return <object>base
+ */
+  }
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+ *     if base is NULL:
+ *         return None
+ *     return <object>base             # <<<<<<<<<<<<<<
+ * 
+ * # Versions of the import_* functions which are more suitable for
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(((PyObject *)__pyx_v_base));
+  __pyx_r = ((PyObject *)__pyx_v_base);
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+ *     PyArray_SetBaseObject(arr, base)
+ * 
+ * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
+ *     base = PyArray_BASE(arr)
+ *     if base is NULL:
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_array", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+ * cdef inline int import_array() except -1:
+ *     try:
+ *         __pyx_import_array()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ */
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
+
+      /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+ *     try:
+ *         __pyx_import_array()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+ *         __pyx_import_array()
+ *     except Exception:
+ *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_umath() except -1:
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(2, 983, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+ * # Cython code.
+ * cdef inline int import_array() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         __pyx_import_array()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+ * # Versions of the import_* functions which are more suitable for
+ * # Cython code.
+ * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         __pyx_import_array()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_umath", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+ * cdef inline int import_umath() except -1:
+ *     try:
+ *         _import_umath()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")
+ */
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
+
+      /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+ *     try:
+ *         _import_umath()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * cdef inline int import_ufunc() except -1:
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(2, 989, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+ * 
+ * cdef inline int import_umath() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+ *         raise ImportError("numpy.core.multiarray failed to import")
+ * 
+ * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  PyObject *__pyx_t_6 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("import_ufunc", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+ * cdef inline int import_ufunc() except -1:
+ *     try:
+ *         _import_umath()             # <<<<<<<<<<<<<<
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")
+ */
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
+
+      /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+
+    /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+ *     try:
+ *         _import_umath()
+ *     except Exception:             # <<<<<<<<<<<<<<
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ */
+    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_4) {
+      __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
+      __Pyx_XGOTREF(__pyx_t_5);
+      __Pyx_XGOTREF(__pyx_t_6);
+      __Pyx_XGOTREF(__pyx_t_7);
+
+      /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+ *         _import_umath()
+ *     except Exception:
+ *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __PYX_ERR(2, 995, __pyx_L5_except_error)
+    }
+    goto __pyx_L5_except_error;
+
+    /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+ * 
+ * cdef inline int import_ufunc() except -1:
+ *     try:             # <<<<<<<<<<<<<<
+ *         _import_umath()
+ *     except Exception:
+ */
+    __pyx_L5_except_error:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L8_try_end:;
+  }
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+ *         raise ImportError("numpy.core.umath failed to import")
+ * 
+ * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
+ *     try:
+ *         _import_umath()
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = -1;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+ * 
+ * 
+ * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.timedelta64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("is_datetime64_object", 0);
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+ *     bool
+ *     """
+ *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+ * 
+ * 
+ * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
+ *     """
+ *     Cython equivalent of `isinstance(obj, np.datetime64)`
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
+  npy_datetime __pyx_r;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+ *     also needed.  That can be found using `get_datetime64_unit`.
+ *     """
+ *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+ * 
+ * 
+ * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy datetime64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
+  npy_timedelta __pyx_r;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ *     """
+ *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+ * 
+ * 
+ * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the int64 value underlying scalar numpy timedelta64 object
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
+  NPY_DATETIMEUNIT __pyx_r;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ *     """
+ *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
+  goto __pyx_L0;
+
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+ * 
+ * 
+ * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
+ *     """
+ *     returns the unit part of the dtype for a numpy datetime64 object.
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "src/cyaccess.pyx":36
  * 
  * 
  * cdef np.ndarray[double] convert_vector_to_array_dbl(vector[double] vec):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray arr = np.zeros(len(vec), dtype="double")
  *     for i in range(len(vec)):
  */
 
@@ -1935,90 +6644,90 @@
   Py_ssize_t __pyx_t_6;
   Py_ssize_t __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_vector_to_array_dbl", 0);
 
-  /* "src/cyaccess.pyx":34
+  /* "src/cyaccess.pyx":37
  * 
  * cdef np.ndarray[double] convert_vector_to_array_dbl(vector[double] vec):
  *     cdef np.ndarray arr = np.zeros(len(vec), dtype="double")             # <<<<<<<<<<<<<<
  *     for i in range(len(vec)):
  *         arr[i] = vec[i]
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_convert_vector_to_py_double(__pyx_v_vec); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_double(__pyx_v_vec); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_n_s_double) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_n_u_double) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 37, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 37, __pyx_L1_error)
   __pyx_v_arr = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "src/cyaccess.pyx":35
+  /* "src/cyaccess.pyx":38
  * cdef np.ndarray[double] convert_vector_to_array_dbl(vector[double] vec):
  *     cdef np.ndarray arr = np.zeros(len(vec), dtype="double")
  *     for i in range(len(vec)):             # <<<<<<<<<<<<<<
  *         arr[i] = vec[i]
  *     return arr
  */
-  __pyx_t_5 = __pyx_convert_vector_to_py_double(__pyx_v_vec); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_5 = __pyx_convert_vector_to_py_double(__pyx_v_vec); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_3 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 38, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_6 = __pyx_t_3;
   for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
     __pyx_v_i = __pyx_t_7;
 
-    /* "src/cyaccess.pyx":36
+    /* "src/cyaccess.pyx":39
  *     cdef np.ndarray arr = np.zeros(len(vec), dtype="double")
  *     for i in range(len(vec)):
  *         arr[i] = vec[i]             # <<<<<<<<<<<<<<
  *     return arr
  * 
  */
-    __pyx_t_5 = PyFloat_FromDouble((__pyx_v_vec[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 36, __pyx_L1_error)
+    __pyx_t_5 = PyFloat_FromDouble((__pyx_v_vec[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_SetItemInt(((PyObject *)__pyx_v_arr), __pyx_v_i, __pyx_t_5, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1) < 0)) __PYX_ERR(0, 36, __pyx_L1_error)
+    if (unlikely((__Pyx_SetItemInt(((PyObject *)__pyx_v_arr), __pyx_v_i, __pyx_t_5, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 1, 1) < 0))) __PYX_ERR(0, 39, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
 
-  /* "src/cyaccess.pyx":37
+  /* "src/cyaccess.pyx":40
  *     for i in range(len(vec)):
  *         arr[i] = vec[i]
  *     return arr             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __Pyx_INCREF(((PyObject *)__pyx_v_arr));
+  __Pyx_XDECREF((PyObject *)__pyx_r);
+  __Pyx_INCREF((PyObject *)__pyx_v_arr);
   __pyx_r = ((PyArrayObject *)__pyx_v_arr);
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":33
+  /* "src/cyaccess.pyx":36
  * 
  * 
  * cdef np.ndarray[double] convert_vector_to_array_dbl(vector[double] vec):             # <<<<<<<<<<<<<<
  *     cdef np.ndarray arr = np.zeros(len(vec), dtype="double")
  *     for i in range(len(vec)):
  */
 
@@ -2033,15 +6742,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_arr);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":40
+/* "src/cyaccess.pyx":43
  * 
  * 
  * cdef np.ndarray[double, ndim = 2] convert_2D_vector_to_array_dbl(             # <<<<<<<<<<<<<<
  *         vector[vector[double]] vec):
  *     cdef np.ndarray arr = np.empty_like(vec, dtype="double")
  */
 
@@ -2051,110 +6760,113 @@
   npy_intp __pyx_v_j;
   PyArrayObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  npy_intp __pyx_t_5;
+  npy_intp *__pyx_t_5;
   npy_intp __pyx_t_6;
   npy_intp __pyx_t_7;
   npy_intp __pyx_t_8;
   npy_intp __pyx_t_9;
   npy_intp __pyx_t_10;
+  npy_intp __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_2D_vector_to_array_dbl", 0);
 
-  /* "src/cyaccess.pyx":42
+  /* "src/cyaccess.pyx":45
  * cdef np.ndarray[double, ndim = 2] convert_2D_vector_to_array_dbl(
  *         vector[vector[double]] vec):
  *     cdef np.ndarray arr = np.empty_like(vec, dtype="double")             # <<<<<<<<<<<<<<
  *     for i in range(arr.shape[0]):
  *         for j in range(arr.shape[1]):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty_like); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty_like); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(__pyx_v_vec); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(__pyx_v_vec); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_n_s_double) < 0) __PYX_ERR(0, 42, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_n_u_double) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 45, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 42, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 45, __pyx_L1_error)
   __pyx_v_arr = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "src/cyaccess.pyx":43
+  /* "src/cyaccess.pyx":46
  *         vector[vector[double]] vec):
  *     cdef np.ndarray arr = np.empty_like(vec, dtype="double")
  *     for i in range(arr.shape[0]):             # <<<<<<<<<<<<<<
  *         for j in range(arr.shape[1]):
  *             arr[i][j] = vec[i][j]
  */
-  __pyx_t_5 = (__pyx_v_arr->dimensions[0]);
-  __pyx_t_6 = __pyx_t_5;
-  for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
-    __pyx_v_i = __pyx_t_7;
+  __pyx_t_5 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_arr); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_t_6 = (__pyx_t_5[0]);
+  __pyx_t_7 = __pyx_t_6;
+  for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
+    __pyx_v_i = __pyx_t_8;
 
-    /* "src/cyaccess.pyx":44
+    /* "src/cyaccess.pyx":47
  *     cdef np.ndarray arr = np.empty_like(vec, dtype="double")
  *     for i in range(arr.shape[0]):
  *         for j in range(arr.shape[1]):             # <<<<<<<<<<<<<<
  *             arr[i][j] = vec[i][j]
  *     return arr
  */
-    __pyx_t_8 = (__pyx_v_arr->dimensions[1]);
-    __pyx_t_9 = __pyx_t_8;
-    for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
-      __pyx_v_j = __pyx_t_10;
+    __pyx_t_5 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_arr); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L1_error)
+    __pyx_t_9 = (__pyx_t_5[1]);
+    __pyx_t_10 = __pyx_t_9;
+    for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
+      __pyx_v_j = __pyx_t_11;
 
-      /* "src/cyaccess.pyx":45
+      /* "src/cyaccess.pyx":48
  *     for i in range(arr.shape[0]):
  *         for j in range(arr.shape[1]):
  *             arr[i][j] = vec[i][j]             # <<<<<<<<<<<<<<
  *     return arr
  * 
  */
-      __pyx_t_4 = PyFloat_FromDouble(((__pyx_v_vec[__pyx_v_i])[__pyx_v_j])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 45, __pyx_L1_error)
+      __pyx_t_4 = PyFloat_FromDouble(((__pyx_v_vec[__pyx_v_i])[__pyx_v_j])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 48, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_arr), __pyx_v_i, npy_intp, 1, __Pyx_PyInt_From_Py_intptr_t, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 45, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_arr), __pyx_v_i, npy_intp, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_1, __pyx_v_j, __pyx_t_4, npy_intp, 1, __Pyx_PyInt_From_Py_intptr_t, 0, 1, 1) < 0)) __PYX_ERR(0, 45, __pyx_L1_error)
+      if (unlikely((__Pyx_SetItemInt(__pyx_t_1, __pyx_v_j, __pyx_t_4, npy_intp, 1, PyInt_FromSsize_t, 0, 1, 1) < 0))) __PYX_ERR(0, 48, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
   }
 
-  /* "src/cyaccess.pyx":46
+  /* "src/cyaccess.pyx":49
  *         for j in range(arr.shape[1]):
  *             arr[i][j] = vec[i][j]
  *     return arr             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __Pyx_INCREF(((PyObject *)__pyx_v_arr));
+  __Pyx_XDECREF((PyObject *)__pyx_r);
+  __Pyx_INCREF((PyObject *)__pyx_v_arr);
   __pyx_r = ((PyArrayObject *)__pyx_v_arr);
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":40
+  /* "src/cyaccess.pyx":43
  * 
  * 
  * cdef np.ndarray[double, ndim = 2] convert_2D_vector_to_array_dbl(             # <<<<<<<<<<<<<<
  *         vector[vector[double]] vec):
  *     cdef np.ndarray arr = np.empty_like(vec, dtype="double")
  */
 
@@ -2169,15 +6881,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_arr);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":49
+/* "src/cyaccess.pyx":52
  * 
  * 
  * cdef np.ndarray[int, ndim = 2] convert_2D_vector_to_array_int(             # <<<<<<<<<<<<<<
  *         vector[vector[int]] vec):
  *     cdef np.ndarray arr = np.empty_like(vec, dtype="int")
  */
 
@@ -2187,110 +6899,113 @@
   npy_intp __pyx_v_j;
   PyArrayObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  npy_intp __pyx_t_5;
+  npy_intp *__pyx_t_5;
   npy_intp __pyx_t_6;
   npy_intp __pyx_t_7;
   npy_intp __pyx_t_8;
   npy_intp __pyx_t_9;
   npy_intp __pyx_t_10;
+  npy_intp __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_2D_vector_to_array_int", 0);
 
-  /* "src/cyaccess.pyx":51
+  /* "src/cyaccess.pyx":54
  * cdef np.ndarray[int, ndim = 2] convert_2D_vector_to_array_int(
  *         vector[vector[int]] vec):
  *     cdef np.ndarray arr = np.empty_like(vec, dtype="int")             # <<<<<<<<<<<<<<
  *     for i in range(arr.shape[0]):
  *         for j in range(arr.shape[1]):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty_like); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty_like); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(__pyx_v_vec); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(__pyx_v_vec); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_n_s_int) < 0) __PYX_ERR(0, 51, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 51, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_n_u_int) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 51, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 54, __pyx_L1_error)
   __pyx_v_arr = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "src/cyaccess.pyx":52
+  /* "src/cyaccess.pyx":55
  *         vector[vector[int]] vec):
  *     cdef np.ndarray arr = np.empty_like(vec, dtype="int")
  *     for i in range(arr.shape[0]):             # <<<<<<<<<<<<<<
  *         for j in range(arr.shape[1]):
  *             arr[i][j] = vec[i][j]
  */
-  __pyx_t_5 = (__pyx_v_arr->dimensions[0]);
-  __pyx_t_6 = __pyx_t_5;
-  for (__pyx_t_7 = 0; __pyx_t_7 < __pyx_t_6; __pyx_t_7+=1) {
-    __pyx_v_i = __pyx_t_7;
+  __pyx_t_5 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_arr); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_6 = (__pyx_t_5[0]);
+  __pyx_t_7 = __pyx_t_6;
+  for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
+    __pyx_v_i = __pyx_t_8;
 
-    /* "src/cyaccess.pyx":53
+    /* "src/cyaccess.pyx":56
  *     cdef np.ndarray arr = np.empty_like(vec, dtype="int")
  *     for i in range(arr.shape[0]):
  *         for j in range(arr.shape[1]):             # <<<<<<<<<<<<<<
  *             arr[i][j] = vec[i][j]
  *     return arr
  */
-    __pyx_t_8 = (__pyx_v_arr->dimensions[1]);
-    __pyx_t_9 = __pyx_t_8;
-    for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_9; __pyx_t_10+=1) {
-      __pyx_v_j = __pyx_t_10;
+    __pyx_t_5 = __pyx_f_5numpy_7ndarray_5shape_shape(__pyx_v_arr); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_9 = (__pyx_t_5[1]);
+    __pyx_t_10 = __pyx_t_9;
+    for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_10; __pyx_t_11+=1) {
+      __pyx_v_j = __pyx_t_11;
 
-      /* "src/cyaccess.pyx":54
+      /* "src/cyaccess.pyx":57
  *     for i in range(arr.shape[0]):
  *         for j in range(arr.shape[1]):
  *             arr[i][j] = vec[i][j]             # <<<<<<<<<<<<<<
  *     return arr
  * 
  */
-      __pyx_t_4 = __Pyx_PyInt_From_int(((__pyx_v_vec[__pyx_v_i])[__pyx_v_j])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 54, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int(((__pyx_v_vec[__pyx_v_i])[__pyx_v_j])); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_arr), __pyx_v_i, npy_intp, 1, __Pyx_PyInt_From_Py_intptr_t, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 54, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_GetItemInt(((PyObject *)__pyx_v_arr), __pyx_v_i, npy_intp, 1, PyInt_FromSsize_t, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 57, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (unlikely(__Pyx_SetItemInt(__pyx_t_1, __pyx_v_j, __pyx_t_4, npy_intp, 1, __Pyx_PyInt_From_Py_intptr_t, 0, 1, 1) < 0)) __PYX_ERR(0, 54, __pyx_L1_error)
+      if (unlikely((__Pyx_SetItemInt(__pyx_t_1, __pyx_v_j, __pyx_t_4, npy_intp, 1, PyInt_FromSsize_t, 0, 1, 1) < 0))) __PYX_ERR(0, 57, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
   }
 
-  /* "src/cyaccess.pyx":55
+  /* "src/cyaccess.pyx":58
  *         for j in range(arr.shape[1]):
  *             arr[i][j] = vec[i][j]
  *     return arr             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_XDECREF(((PyObject *)__pyx_r));
-  __Pyx_INCREF(((PyObject *)__pyx_v_arr));
+  __Pyx_XDECREF((PyObject *)__pyx_r);
+  __Pyx_INCREF((PyObject *)__pyx_v_arr);
   __pyx_r = ((PyArrayObject *)__pyx_v_arr);
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":49
+  /* "src/cyaccess.pyx":52
  * 
  * 
  * cdef np.ndarray[int, ndim = 2] convert_2D_vector_to_array_int(             # <<<<<<<<<<<<<<
  *         vector[vector[int]] vec):
  *     cdef np.ndarray arr = np.empty_like(vec, dtype="int")
  */
 
@@ -2305,15 +7020,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_arr);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":61
+/* "src/cyaccess.pyx":64
  *     cdef Accessibility * access
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *         self,
  *         np.ndarray[long] node_ids,
  */
 
@@ -2321,118 +7036,125 @@
 static int __pyx_pw_7pandana_8cyaccess_8cyaccess_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_pw_7pandana_8cyaccess_8cyaccess_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_node_ids = 0;
   CYTHON_UNUSED PyArrayObject *__pyx_v_node_xys = 0;
   PyArrayObject *__pyx_v_edges = 0;
   PyArrayObject *__pyx_v_edge_weights = 0;
   bool __pyx_v_twoway;
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node_ids,&__pyx_n_s_node_xys,&__pyx_n_s_edges,&__pyx_n_s_edge_weights,&__pyx_n_s_twoway,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_node_ids,&__pyx_n_s_node_xys,&__pyx_n_s_edges,&__pyx_n_s_edge_weights,&__pyx_n_s_twoway,0};
     PyObject* values[5] = {0,0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      switch (__pyx_nargs) {
+        case  5: values[4] = __Pyx_Arg_VARARGS(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        case  4: values[3] = __Pyx_Arg_VARARGS(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_VARARGS(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node_ids)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_node_ids)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node_xys)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_node_xys)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 1); __PYX_ERR(0, 61, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 1); __PYX_ERR(0, 64, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_edges)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_edges)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 2); __PYX_ERR(0, 61, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 2); __PYX_ERR(0, 64, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_edge_weights)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_edge_weights)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 3); __PYX_ERR(0, 61, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, 3); __PYX_ERR(0, 64, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_twoway);
+          PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_twoway);
           if (value) { values[4] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 64, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 61, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(0, 64, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      switch (__pyx_nargs) {
+        case  5: values[4] = __Pyx_Arg_VARARGS(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  4: values[3] = __Pyx_Arg_VARARGS(__pyx_args, 3);
+        values[2] = __Pyx_Arg_VARARGS(__pyx_args, 2);
+        values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
+        values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_node_ids = ((PyArrayObject *)values[0]);
     __pyx_v_node_xys = ((PyArrayObject *)values[1]);
     __pyx_v_edges = ((PyArrayObject *)values[2]);
     __pyx_v_edge_weights = ((PyArrayObject *)values[3]);
     if (values[4]) {
-      __pyx_v_twoway = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_twoway == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 67, __pyx_L3_error)
+      __pyx_v_twoway = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_twoway == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 70, __pyx_L3_error)
     } else {
 
-      /* "src/cyaccess.pyx":67
+      /* "src/cyaccess.pyx":70
  *         np.ndarray[long, ndim=2] edges,
  *         np.ndarray[double, ndim=2] edge_weights,
  *         bool twoway=True             # <<<<<<<<<<<<<<
  *     ):
  *         """
  */
       __pyx_v_twoway = ((bool)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 61, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 64, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pandana.cyaccess.cyaccess.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node_ids), __pyx_ptype_5numpy_ndarray, 1, "node_ids", 0))) __PYX_ERR(0, 63, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node_xys), __pyx_ptype_5numpy_ndarray, 1, "node_xys", 0))) __PYX_ERR(0, 64, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_edges), __pyx_ptype_5numpy_ndarray, 1, "edges", 0))) __PYX_ERR(0, 65, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_edge_weights), __pyx_ptype_5numpy_ndarray, 1, "edge_weights", 0))) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node_ids), __pyx_ptype_5numpy_ndarray, 1, "node_ids", 0))) __PYX_ERR(0, 66, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node_xys), __pyx_ptype_5numpy_ndarray, 1, "node_xys", 0))) __PYX_ERR(0, 67, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_edges), __pyx_ptype_5numpy_ndarray, 1, "edges", 0))) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_edge_weights), __pyx_ptype_5numpy_ndarray, 1, "edge_weights", 0))) __PYX_ERR(0, 69, __pyx_L1_error)
   __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess___cinit__(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_node_ids, __pyx_v_node_xys, __pyx_v_edges, __pyx_v_edge_weights, __pyx_v_twoway);
 
-  /* "src/cyaccess.pyx":61
+  /* "src/cyaccess.pyx":64
  *     cdef Accessibility * access
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *         self,
  *         np.ndarray[long] node_ids,
  */
 
@@ -2478,52 +7200,52 @@
   __pyx_pybuffernd_edges.rcbuffer = &__pyx_pybuffer_edges;
   __pyx_pybuffer_edge_weights.pybuffer.buf = NULL;
   __pyx_pybuffer_edge_weights.refcount = 0;
   __pyx_pybuffernd_edge_weights.data = NULL;
   __pyx_pybuffernd_edge_weights.rcbuffer = &__pyx_pybuffer_edge_weights;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_ids.rcbuffer->pybuffer, (PyObject*)__pyx_v_node_ids, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 61, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_ids.rcbuffer->pybuffer, (PyObject*)__pyx_v_node_ids, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 64, __pyx_L1_error)
   }
   __pyx_pybuffernd_node_ids.diminfo[0].strides = __pyx_pybuffernd_node_ids.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_node_ids.diminfo[0].shape = __pyx_pybuffernd_node_ids.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_xys.rcbuffer->pybuffer, (PyObject*)__pyx_v_node_xys, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 61, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_xys.rcbuffer->pybuffer, (PyObject*)__pyx_v_node_xys, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 64, __pyx_L1_error)
   }
   __pyx_pybuffernd_node_xys.diminfo[0].strides = __pyx_pybuffernd_node_xys.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_node_xys.diminfo[0].shape = __pyx_pybuffernd_node_xys.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_node_xys.diminfo[1].strides = __pyx_pybuffernd_node_xys.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_node_xys.diminfo[1].shape = __pyx_pybuffernd_node_xys.rcbuffer->pybuffer.shape[1];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_edges.rcbuffer->pybuffer, (PyObject*)__pyx_v_edges, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 61, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_edges.rcbuffer->pybuffer, (PyObject*)__pyx_v_edges, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 64, __pyx_L1_error)
   }
   __pyx_pybuffernd_edges.diminfo[0].strides = __pyx_pybuffernd_edges.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_edges.diminfo[0].shape = __pyx_pybuffernd_edges.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_edges.diminfo[1].strides = __pyx_pybuffernd_edges.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_edges.diminfo[1].shape = __pyx_pybuffernd_edges.rcbuffer->pybuffer.shape[1];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_edge_weights.rcbuffer->pybuffer, (PyObject*)__pyx_v_edge_weights, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 61, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_edge_weights.rcbuffer->pybuffer, (PyObject*)__pyx_v_edge_weights, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 64, __pyx_L1_error)
   }
   __pyx_pybuffernd_edge_weights.diminfo[0].strides = __pyx_pybuffernd_edge_weights.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_edge_weights.diminfo[0].shape = __pyx_pybuffernd_edge_weights.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_edge_weights.diminfo[1].strides = __pyx_pybuffernd_edge_weights.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_edge_weights.diminfo[1].shape = __pyx_pybuffernd_edge_weights.rcbuffer->pybuffer.shape[1];
 
-  /* "src/cyaccess.pyx":80
+  /* "src/cyaccess.pyx":83
  *         # anymore - I'm hesitant to out-and-out remove it as we might still use
  *         # it for something someday
  *         self.access = new Accessibility(len(node_ids), edges, edge_weights, twoway)             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
-  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_node_ids)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 80, __pyx_L1_error)
-  __pyx_t_2 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(((PyObject *)__pyx_v_edges)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
-  __pyx_t_3 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(((PyObject *)__pyx_v_edge_weights)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(((PyObject *)__pyx_v_node_ids)); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(((PyObject *)__pyx_v_edges)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(((PyObject *)__pyx_v_edge_weights)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L1_error)
   try {
     __pyx_t_4 = new MTC::accessibility::Accessibility(__pyx_t_1, __pyx_t_2, __pyx_t_3, __pyx_v_twoway);
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 80, __pyx_L1_error)
+    __PYX_ERR(0, 83, __pyx_L1_error)
   }
   __pyx_v_self->access = __pyx_t_4;
 
-  /* "src/cyaccess.pyx":61
+  /* "src/cyaccess.pyx":64
  *     cdef Accessibility * access
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *         self,
  *         np.ndarray[long] node_ids,
  */
 
@@ -2549,148 +7271,170 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_node_ids.rcbuffer->pybuffer);
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_node_xys.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":82
+/* "src/cyaccess.pyx":85
  *         self.access = new Accessibility(len(node_ids), edges, edge_weights, twoway)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         del self.access
  * 
  */
 
 /* Python wrapper */
 static void __pyx_pw_7pandana_8cyaccess_8cyaccess_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_pw_7pandana_8cyaccess_8cyaccess_3__dealloc__(PyObject *__pyx_v_self) {
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
   __pyx_pf_7pandana_8cyaccess_8cyaccess_2__dealloc__(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_7pandana_8cyaccess_8cyaccess_2__dealloc__(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "src/cyaccess.pyx":83
+  /* "src/cyaccess.pyx":86
  * 
  *     def __dealloc__(self):
  *         del self.access             # <<<<<<<<<<<<<<
  * 
  *     def initialize_category(
  */
   delete __pyx_v_self->access;
 
-  /* "src/cyaccess.pyx":82
+  /* "src/cyaccess.pyx":85
  *         self.access = new Accessibility(len(node_ids), edges, edge_weights, twoway)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         del self.access
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "src/cyaccess.pyx":85
+/* "src/cyaccess.pyx":88
  *         del self.access
  * 
  *     def initialize_category(             # <<<<<<<<<<<<<<
  *         self,
  *         double maxdist,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_5initialize_category(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pandana_8cyaccess_8cyaccess_4initialize_category[] = "\n        maxdist - the maximum distance that will later be used in\n            find_all_nearest_pois\n        maxitems - the maximum number of items that will later be requested\n            in find_all_nearest_pois\n        category - the category name\n        node_ids - an array of nodeids which are locations where this poi occurs\n        ";
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_5initialize_category(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_5initialize_category(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7pandana_8cyaccess_8cyaccess_4initialize_category, "\n        maxdist - the maximum distance that will later be used in\n            find_all_nearest_pois\n        maxitems - the maximum number of items that will later be requested\n            in find_all_nearest_pois\n        category - the category name\n        node_ids - an array of nodeids which are locations where this poi occurs\n        ");
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_5initialize_category = {"initialize_category", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_5initialize_category, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_4initialize_category};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_5initialize_category(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   double __pyx_v_maxdist;
   int __pyx_v_maxitems;
   std::string __pyx_v_category;
   PyArrayObject *__pyx_v_node_ids = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("initialize_category (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_maxdist,&__pyx_n_s_maxitems,&__pyx_n_s_category,&__pyx_n_s_node_ids,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_maxdist,&__pyx_n_s_maxitems,&__pyx_n_s_category,&__pyx_n_s_node_ids,0};
     PyObject* values[4] = {0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_maxdist)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_maxdist)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_maxitems)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_maxitems)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("initialize_category", 1, 4, 4, 1); __PYX_ERR(0, 85, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("initialize_category", 1, 4, 4, 1); __PYX_ERR(0, 88, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_category)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_category)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("initialize_category", 1, 4, 4, 2); __PYX_ERR(0, 85, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("initialize_category", 1, 4, 4, 2); __PYX_ERR(0, 88, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node_ids)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_node_ids)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("initialize_category", 1, 4, 4, 3); __PYX_ERR(0, 85, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("initialize_category", 1, 4, 4, 3); __PYX_ERR(0, 88, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "initialize_category") < 0)) __PYX_ERR(0, 85, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "initialize_category") < 0)) __PYX_ERR(0, 88, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
+    } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-      values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-    }
-    __pyx_v_maxdist = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_maxdist == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 87, __pyx_L3_error)
-    __pyx_v_maxitems = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_maxitems == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
-    __pyx_v_category = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L3_error)
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+      values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+    }
+    __pyx_v_maxdist = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_maxdist == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 90, __pyx_L3_error)
+    __pyx_v_maxitems = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_maxitems == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 91, __pyx_L3_error)
+    __pyx_v_category = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 92, __pyx_L3_error)
     __pyx_v_node_ids = ((PyArrayObject *)values[3]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("initialize_category", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 85, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("initialize_category", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 88, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pandana.cyaccess.cyaccess.initialize_category", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node_ids), __pyx_ptype_5numpy_ndarray, 1, "node_ids", 0))) __PYX_ERR(0, 90, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_4initialize_category(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_maxdist, __pyx_v_maxitems, __pyx_v_category, __pyx_v_node_ids);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node_ids), __pyx_ptype_5numpy_ndarray, 1, "node_ids", 0))) __PYX_ERR(0, 93, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_4initialize_category(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_maxdist, __pyx_v_maxitems, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_category), __pyx_v_node_ids);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -2709,29 +7453,29 @@
   __Pyx_RefNannySetupContext("initialize_category", 0);
   __pyx_pybuffer_node_ids.pybuffer.buf = NULL;
   __pyx_pybuffer_node_ids.refcount = 0;
   __pyx_pybuffernd_node_ids.data = NULL;
   __pyx_pybuffernd_node_ids.rcbuffer = &__pyx_pybuffer_node_ids;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_ids.rcbuffer->pybuffer, (PyObject*)__pyx_v_node_ids, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 85, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_ids.rcbuffer->pybuffer, (PyObject*)__pyx_v_node_ids, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 88, __pyx_L1_error)
   }
   __pyx_pybuffernd_node_ids.diminfo[0].strides = __pyx_pybuffernd_node_ids.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_node_ids.diminfo[0].shape = __pyx_pybuffernd_node_ids.rcbuffer->pybuffer.shape[0];
 
-  /* "src/cyaccess.pyx":100
+  /* "src/cyaccess.pyx":103
  *         node_ids - an array of nodeids which are locations where this poi occurs
  *         """
  *         self.access.initializeCategory(maxdist, maxitems, category, node_ids)             # <<<<<<<<<<<<<<
  * 
  *     def find_all_nearest_pois(
  */
-  __pyx_t_1 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_node_ids)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 100, __pyx_L1_error)
-  __pyx_v_self->access->initializeCategory(__pyx_v_maxdist, __pyx_v_maxitems, __pyx_v_category, __pyx_t_1);
+  __pyx_t_1 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_node_ids)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 103, __pyx_L1_error)
+  __pyx_v_self->access->initializeCategory(__pyx_v_maxdist, __pyx_v_maxitems, __pyx_v_category, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1));
 
-  /* "src/cyaccess.pyx":85
+  /* "src/cyaccess.pyx":88
  *         del self.access
  * 
  *     def initialize_category(             # <<<<<<<<<<<<<<
  *         self,
  *         double maxdist,
  */
 
@@ -2752,110 +7496,131 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_node_ids.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":102
+/* "src/cyaccess.pyx":105
  *         self.access.initializeCategory(maxdist, maxitems, category, node_ids)
  * 
  *     def find_all_nearest_pois(             # <<<<<<<<<<<<<<
  *         self,
  *         double radius,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_7find_all_nearest_pois(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pandana_8cyaccess_8cyaccess_6find_all_nearest_pois[] = "\n        radius - search radius\n        num_of_pois - number of pois to search for\n        category - the category name\n        impno - the impedance id to use\n        return_nodeids - whether to return the nodeid locations of the nearest\n            not just the distances\n        ";
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_7find_all_nearest_pois(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_7find_all_nearest_pois(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7pandana_8cyaccess_8cyaccess_6find_all_nearest_pois, "\n        radius - search radius\n        num_of_pois - number of pois to search for\n        category - the category name\n        impno - the impedance id to use\n        return_nodeids - whether to return the nodeid locations of the nearest\n            not just the distances\n        ");
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_7find_all_nearest_pois = {"find_all_nearest_pois", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_7find_all_nearest_pois, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_6find_all_nearest_pois};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_7find_all_nearest_pois(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   double __pyx_v_radius;
   int __pyx_v_num_of_pois;
   std::string __pyx_v_category;
   int __pyx_v_impno;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("find_all_nearest_pois (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_radius,&__pyx_n_s_num_of_pois,&__pyx_n_s_category,&__pyx_n_s_impno,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_radius,&__pyx_n_s_num_of_pois,&__pyx_n_s_category,&__pyx_n_s_impno,0};
     PyObject* values[4] = {0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_radius)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_radius)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_num_of_pois)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_num_of_pois)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("find_all_nearest_pois", 0, 3, 4, 1); __PYX_ERR(0, 102, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("find_all_nearest_pois", 0, 3, 4, 1); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_category)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_category)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("find_all_nearest_pois", 0, 3, 4, 2); __PYX_ERR(0, 102, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("find_all_nearest_pois", 0, 3, 4, 2); __PYX_ERR(0, 105, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_impno);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_impno);
           if (value) { values[3] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "find_all_nearest_pois") < 0)) __PYX_ERR(0, 102, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "find_all_nearest_pois") < 0)) __PYX_ERR(0, 105, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_radius = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_radius == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 104, __pyx_L3_error)
-    __pyx_v_num_of_pois = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_num_of_pois == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L3_error)
-    __pyx_v_category = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L3_error)
+    __pyx_v_radius = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_radius == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L3_error)
+    __pyx_v_num_of_pois = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_num_of_pois == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L3_error)
+    __pyx_v_category = __pyx_convert_string_from_py_std__in_string(values[2]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L3_error)
     if (values[3]) {
-      __pyx_v_impno = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 107, __pyx_L3_error)
+      __pyx_v_impno = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L3_error)
     } else {
       __pyx_v_impno = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("find_all_nearest_pois", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 102, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("find_all_nearest_pois", 0, 3, 4, __pyx_nargs); __PYX_ERR(0, 105, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pandana.cyaccess.cyaccess.find_all_nearest_pois", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_6find_all_nearest_pois(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_radius, __pyx_v_num_of_pois, __pyx_v_category, __pyx_v_impno);
+  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_6find_all_nearest_pois(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_radius, __pyx_v_num_of_pois, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_category), __pyx_v_impno);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_6find_all_nearest_pois(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, double __pyx_v_radius, int __pyx_v_num_of_pois, std::string __pyx_v_category, int __pyx_v_impno) {
@@ -2866,64 +7631,64 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("find_all_nearest_pois", 0);
 
-  /* "src/cyaccess.pyx":117
+  /* "src/cyaccess.pyx":120
  *             not just the distances
  *         """
  *         ret = self.access.findAllNearestPOIs(radius, num_of_pois, category, impno)             # <<<<<<<<<<<<<<
  * 
  *         return convert_2D_vector_to_array_dbl(ret.first),\
  */
   __pyx_v_ret = __pyx_v_self->access->findAllNearestPOIs(__pyx_v_radius, __pyx_v_num_of_pois, __pyx_v_category, __pyx_v_impno);
 
-  /* "src/cyaccess.pyx":119
+  /* "src/cyaccess.pyx":122
  *         ret = self.access.findAllNearestPOIs(radius, num_of_pois, category, impno)
  * 
  *         return convert_2D_vector_to_array_dbl(ret.first),\             # <<<<<<<<<<<<<<
  *             convert_2D_vector_to_array_int(ret.second)
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((PyObject *)__pyx_f_7pandana_8cyaccess_convert_2D_vector_to_array_dbl(__pyx_v_ret.first)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)__pyx_f_7pandana_8cyaccess_convert_2D_vector_to_array_dbl(__pyx_v_ret.first)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
 
-  /* "src/cyaccess.pyx":120
+  /* "src/cyaccess.pyx":123
  * 
  *         return convert_2D_vector_to_array_dbl(ret.first),\
  *             convert_2D_vector_to_array_int(ret.second)             # <<<<<<<<<<<<<<
  * 
  *     def initialize_access_var(
  */
-  __pyx_t_2 = ((PyObject *)__pyx_f_7pandana_8cyaccess_convert_2D_vector_to_array_int(__pyx_v_ret.second)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+  __pyx_t_2 = ((PyObject *)__pyx_f_7pandana_8cyaccess_convert_2D_vector_to_array_int(__pyx_v_ret.second)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "src/cyaccess.pyx":119
+  /* "src/cyaccess.pyx":122
  *         ret = self.access.findAllNearestPOIs(radius, num_of_pois, category, impno)
  * 
  *         return convert_2D_vector_to_array_dbl(ret.first),\             # <<<<<<<<<<<<<<
  *             convert_2D_vector_to_array_int(ret.second)
  * 
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 119, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":102
+  /* "src/cyaccess.pyx":105
  *         self.access.initializeCategory(maxdist, maxitems, category, node_ids)
  * 
  *     def find_all_nearest_pois(             # <<<<<<<<<<<<<<
  *         self,
  *         double radius,
  */
 
@@ -2936,94 +7701,114 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":122
+/* "src/cyaccess.pyx":125
  *             convert_2D_vector_to_array_int(ret.second)
  * 
  *     def initialize_access_var(             # <<<<<<<<<<<<<<
  *         self,
  *         string category,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_9initialize_access_var(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pandana_8cyaccess_8cyaccess_8initialize_access_var[] = "\n        category - category name\n        node_ids: vector of node identifiers\n        values: vector of values that are location at the nodes\n        ";
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_9initialize_access_var(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_9initialize_access_var(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7pandana_8cyaccess_8cyaccess_8initialize_access_var, "\n        category - category name\n        node_ids: vector of node identifiers\n        values: vector of values that are location at the nodes\n        ");
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_9initialize_access_var = {"initialize_access_var", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_9initialize_access_var, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_8initialize_access_var};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_9initialize_access_var(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   std::string __pyx_v_category;
   PyArrayObject *__pyx_v_node_ids = 0;
   PyArrayObject *__pyx_v_values = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("initialize_access_var (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_category,&__pyx_n_s_node_ids,&__pyx_n_s_values,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_category,&__pyx_n_s_node_ids,&__pyx_n_s_values,0};
     PyObject* values[3] = {0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_category)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_category)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 125, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_node_ids)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_node_ids)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 125, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("initialize_access_var", 1, 3, 3, 1); __PYX_ERR(0, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("initialize_access_var", 1, 3, 3, 1); __PYX_ERR(0, 125, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_values)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_values)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 125, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("initialize_access_var", 1, 3, 3, 2); __PYX_ERR(0, 122, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("initialize_access_var", 1, 3, 3, 2); __PYX_ERR(0, 125, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "initialize_access_var") < 0)) __PYX_ERR(0, 122, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "initialize_access_var") < 0)) __PYX_ERR(0, 125, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+    } else if (unlikely(__pyx_nargs != 3)) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
-      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
     }
-    __pyx_v_category = __pyx_convert_string_from_py_std__in_string(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 124, __pyx_L3_error)
+    __pyx_v_category = __pyx_convert_string_from_py_std__in_string(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 127, __pyx_L3_error)
     __pyx_v_node_ids = ((PyArrayObject *)values[1]);
     __pyx_v_values = ((PyArrayObject *)values[2]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("initialize_access_var", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 122, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("initialize_access_var", 1, 3, 3, __pyx_nargs); __PYX_ERR(0, 125, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pandana.cyaccess.cyaccess.initialize_access_var", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node_ids), __pyx_ptype_5numpy_ndarray, 1, "node_ids", 0))) __PYX_ERR(0, 125, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_values), __pyx_ptype_5numpy_ndarray, 1, "values", 0))) __PYX_ERR(0, 126, __pyx_L1_error)
-  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_8initialize_access_var(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_category, __pyx_v_node_ids, __pyx_v_values);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_node_ids), __pyx_ptype_5numpy_ndarray, 1, "node_ids", 0))) __PYX_ERR(0, 128, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_values), __pyx_ptype_5numpy_ndarray, 1, "values", 0))) __PYX_ERR(0, 129, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_8initialize_access_var(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_category), __pyx_v_node_ids, __pyx_v_values);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
@@ -3049,35 +7834,35 @@
   __pyx_pybuffernd_node_ids.rcbuffer = &__pyx_pybuffer_node_ids;
   __pyx_pybuffer_values.pybuffer.buf = NULL;
   __pyx_pybuffer_values.refcount = 0;
   __pyx_pybuffernd_values.data = NULL;
   __pyx_pybuffernd_values.rcbuffer = &__pyx_pybuffer_values;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_ids.rcbuffer->pybuffer, (PyObject*)__pyx_v_node_ids, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 122, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_node_ids.rcbuffer->pybuffer, (PyObject*)__pyx_v_node_ids, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 125, __pyx_L1_error)
   }
   __pyx_pybuffernd_node_ids.diminfo[0].strides = __pyx_pybuffernd_node_ids.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_node_ids.diminfo[0].shape = __pyx_pybuffernd_node_ids.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 122, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_values.rcbuffer->pybuffer, (PyObject*)__pyx_v_values, &__Pyx_TypeInfo_double, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 125, __pyx_L1_error)
   }
   __pyx_pybuffernd_values.diminfo[0].strides = __pyx_pybuffernd_values.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_values.diminfo[0].shape = __pyx_pybuffernd_values.rcbuffer->pybuffer.shape[0];
 
-  /* "src/cyaccess.pyx":133
+  /* "src/cyaccess.pyx":136
  *         values: vector of values that are location at the nodes
  *         """
  *         self.access.initializeAccVar(category, node_ids, values)             # <<<<<<<<<<<<<<
  * 
  *     def get_available_aggregations(self):
  */
-  __pyx_t_1 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_node_ids)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L1_error)
-  __pyx_t_2 = __pyx_convert_vector_from_py_double(((PyObject *)__pyx_v_values)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 133, __pyx_L1_error)
-  __pyx_v_self->access->initializeAccVar(__pyx_v_category, __pyx_t_1, __pyx_t_2);
+  __pyx_t_1 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_node_ids)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_vector_from_py_double(((PyObject *)__pyx_v_values)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_v_self->access->initializeAccVar(__pyx_v_category, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_2));
 
-  /* "src/cyaccess.pyx":122
+  /* "src/cyaccess.pyx":125
  *             convert_2D_vector_to_array_int(ret.second)
  * 
  *     def initialize_access_var(             # <<<<<<<<<<<<<<
  *         self,
  *         string category,
  */
 
@@ -3100,28 +7885,48 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_values.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":135
+/* "src/cyaccess.pyx":138
  *         self.access.initializeAccVar(category, node_ids, values)
  * 
  *     def get_available_aggregations(self):             # <<<<<<<<<<<<<<
  *         return self.access.aggregations
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_11get_available_aggregations(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_11get_available_aggregations(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_11get_available_aggregations(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_11get_available_aggregations = {"get_available_aggregations", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_11get_available_aggregations, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_11get_available_aggregations(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_available_aggregations (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("get_available_aggregations", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "get_available_aggregations", 0))) return NULL;
   __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_10get_available_aggregations(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3130,29 +7935,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_available_aggregations", 0);
 
-  /* "src/cyaccess.pyx":136
+  /* "src/cyaccess.pyx":139
  * 
  *     def get_available_aggregations(self):
  *         return self.access.aggregations             # <<<<<<<<<<<<<<
  * 
  *     def get_available_decays(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_vector_to_py_std_3a__3a_string(__pyx_v_self->access->aggregations); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_std_3a__3a_string(__pyx_v_self->access->aggregations); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":135
+  /* "src/cyaccess.pyx":138
  *         self.access.initializeAccVar(category, node_ids, values)
  * 
  *     def get_available_aggregations(self):             # <<<<<<<<<<<<<<
  *         return self.access.aggregations
  * 
  */
 
@@ -3163,28 +7968,48 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":138
+/* "src/cyaccess.pyx":141
  *         return self.access.aggregations
  * 
  *     def get_available_decays(self):             # <<<<<<<<<<<<<<
  *         return self.access.decays
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_13get_available_decays(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_13get_available_decays(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_13get_available_decays(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_13get_available_decays = {"get_available_decays", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_13get_available_decays, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_13get_available_decays(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_available_decays (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("get_available_decays", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "get_available_decays", 0))) return NULL;
   __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_12get_available_decays(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -3193,29 +8018,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_available_decays", 0);
 
-  /* "src/cyaccess.pyx":139
+  /* "src/cyaccess.pyx":142
  * 
  *     def get_available_decays(self):
  *         return self.access.decays             # <<<<<<<<<<<<<<
  * 
  *     def get_all_aggregate_accessibility_variables(
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_vector_to_py_std_3a__3a_string(__pyx_v_self->access->decays); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_std_3a__3a_string(__pyx_v_self->access->decays); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":138
+  /* "src/cyaccess.pyx":141
  *         return self.access.aggregations
  * 
  *     def get_available_decays(self):             # <<<<<<<<<<<<<<
  *         return self.access.decays
  * 
  */
 
@@ -3226,115 +8051,137 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":141
+/* "src/cyaccess.pyx":144
  *         return self.access.decays
  * 
  *     def get_all_aggregate_accessibility_variables(             # <<<<<<<<<<<<<<
  *         self,
  *         double radius,
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_15get_all_aggregate_accessibility_variables(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pandana_8cyaccess_8cyaccess_14get_all_aggregate_accessibility_variables[] = "\n        radius - search radius\n        category - category name\n        aggtyp - aggregation type, see docs\n        decay - decay type, see docs\n        impno - the impedance id to use\n        ";
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_15get_all_aggregate_accessibility_variables(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_15get_all_aggregate_accessibility_variables(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7pandana_8cyaccess_8cyaccess_14get_all_aggregate_accessibility_variables, "\n        radius - search radius\n        category - category name\n        aggtyp - aggregation type, see docs\n        decay - decay type, see docs\n        impno - the impedance id to use\n        ");
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_15get_all_aggregate_accessibility_variables = {"get_all_aggregate_accessibility_variables", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_15get_all_aggregate_accessibility_variables, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_14get_all_aggregate_accessibility_variables};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_15get_all_aggregate_accessibility_variables(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   double __pyx_v_radius;
   PyObject *__pyx_v_category = 0;
   PyObject *__pyx_v_aggtyp = 0;
   PyObject *__pyx_v_decay = 0;
   int __pyx_v_impno;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_all_aggregate_accessibility_variables (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_radius,&__pyx_n_s_category,&__pyx_n_s_aggtyp,&__pyx_n_s_decay,&__pyx_n_s_impno,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_radius,&__pyx_n_s_category,&__pyx_n_s_aggtyp,&__pyx_n_s_decay,&__pyx_n_s_impno,0};
     PyObject* values[5] = {0,0,0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      switch (__pyx_nargs) {
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_radius)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_radius)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 144, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_category)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_category)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 144, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("get_all_aggregate_accessibility_variables", 0, 4, 5, 1); __PYX_ERR(0, 141, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_all_aggregate_accessibility_variables", 0, 4, 5, 1); __PYX_ERR(0, 144, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_aggtyp)) != 0)) kw_args--;
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_aggtyp)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 144, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("get_all_aggregate_accessibility_variables", 0, 4, 5, 2); __PYX_ERR(0, 141, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_all_aggregate_accessibility_variables", 0, 4, 5, 2); __PYX_ERR(0, 144, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
-        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_decay)) != 0)) kw_args--;
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_decay)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 144, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("get_all_aggregate_accessibility_variables", 0, 4, 5, 3); __PYX_ERR(0, 141, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("get_all_aggregate_accessibility_variables", 0, 4, 5, 3); __PYX_ERR(0, 144, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_impno);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_impno);
           if (value) { values[4] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 144, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_all_aggregate_accessibility_variables") < 0)) __PYX_ERR(0, 141, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "get_all_aggregate_accessibility_variables") < 0)) __PYX_ERR(0, 144, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+      switch (__pyx_nargs) {
+        case  5: values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
-        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
-        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
-        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_radius = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_radius == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 143, __pyx_L3_error)
+    __pyx_v_radius = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_radius == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 146, __pyx_L3_error)
     __pyx_v_category = values[1];
     __pyx_v_aggtyp = values[2];
     __pyx_v_decay = values[3];
     if (values[4]) {
-      __pyx_v_impno = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 147, __pyx_L3_error)
+      __pyx_v_impno = __Pyx_PyInt_As_int(values[4]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 150, __pyx_L3_error)
     } else {
       __pyx_v_impno = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_all_aggregate_accessibility_variables", 0, 4, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 141, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_all_aggregate_accessibility_variables", 0, 4, 5, __pyx_nargs); __PYX_ERR(0, 144, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pandana.cyaccess.cyaccess.get_all_aggregate_accessibility_variables", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_14get_all_aggregate_accessibility_variables(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_radius, __pyx_v_category, __pyx_v_aggtyp, __pyx_v_decay, __pyx_v_impno);
 
@@ -3352,49 +8199,49 @@
   std::string __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_all_aggregate_accessibility_variables", 0);
 
-  /* "src/cyaccess.pyx":157
+  /* "src/cyaccess.pyx":160
  *         """
  *         ret = self.access.getAllAggregateAccessibilityVariables(
  *             radius, category, aggtyp, decay, impno)             # <<<<<<<<<<<<<<
  * 
  *         return convert_vector_to_array_dbl(ret)
  */
-  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_category); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L1_error)
-  __pyx_t_2 = __pyx_convert_string_from_py_std__in_string(__pyx_v_aggtyp); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L1_error)
-  __pyx_t_3 = __pyx_convert_string_from_py_std__in_string(__pyx_v_decay); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 157, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_string_from_py_std__in_string(__pyx_v_category); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_string_from_py_std__in_string(__pyx_v_aggtyp); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert_string_from_py_std__in_string(__pyx_v_decay); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 160, __pyx_L1_error)
 
-  /* "src/cyaccess.pyx":156
+  /* "src/cyaccess.pyx":159
  *         impno - the impedance id to use
  *         """
  *         ret = self.access.getAllAggregateAccessibilityVariables(             # <<<<<<<<<<<<<<
  *             radius, category, aggtyp, decay, impno)
  * 
  */
-  __pyx_v_ret = __pyx_v_self->access->getAllAggregateAccessibilityVariables(__pyx_v_radius, __pyx_t_1, __pyx_t_2, __pyx_t_3, __pyx_v_impno);
+  __pyx_v_ret = __pyx_v_self->access->getAllAggregateAccessibilityVariables(__pyx_v_radius, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_2), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_3), __pyx_v_impno);
 
-  /* "src/cyaccess.pyx":159
+  /* "src/cyaccess.pyx":162
  *             radius, category, aggtyp, decay, impno)
  * 
  *         return convert_vector_to_array_dbl(ret)             # <<<<<<<<<<<<<<
  * 
  *     def shortest_path(self, int srcnode, int destnode, int impno=0):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = ((PyObject *)__pyx_f_7pandana_8cyaccess_convert_vector_to_array_dbl(__pyx_v_ret)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_4 = ((PyObject *)__pyx_f_7pandana_8cyaccess_convert_vector_to_array_dbl(__pyx_v_ret)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":141
+  /* "src/cyaccess.pyx":144
  *         return self.access.decays
  * 
  *     def get_all_aggregate_accessibility_variables(             # <<<<<<<<<<<<<<
  *         self,
  *         double radius,
  */
 
@@ -3405,93 +8252,113 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":161
+/* "src/cyaccess.pyx":164
  *         return convert_vector_to_array_dbl(ret)
  * 
  *     def shortest_path(self, int srcnode, int destnode, int impno=0):             # <<<<<<<<<<<<<<
  *         """
  *         srcnode - node id origin
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_17shortest_path(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pandana_8cyaccess_8cyaccess_16shortest_path[] = "\n        srcnode - node id origin\n        destnode - node id destination\n        impno - the impedance id to use\n        ";
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_17shortest_path(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_17shortest_path(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7pandana_8cyaccess_8cyaccess_16shortest_path, "\n        srcnode - node id origin\n        destnode - node id destination\n        impno - the impedance id to use\n        ");
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_17shortest_path = {"shortest_path", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_17shortest_path, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_16shortest_path};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_17shortest_path(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   int __pyx_v_srcnode;
   int __pyx_v_destnode;
   int __pyx_v_impno;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shortest_path (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_srcnode,&__pyx_n_s_destnode,&__pyx_n_s_impno,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_srcnode,&__pyx_n_s_destnode,&__pyx_n_s_impno,0};
     PyObject* values[3] = {0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_srcnode)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_srcnode)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_destnode)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_destnode)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("shortest_path", 0, 2, 3, 1); __PYX_ERR(0, 161, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("shortest_path", 0, 2, 3, 1); __PYX_ERR(0, 164, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_impno);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_impno);
           if (value) { values[2] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "shortest_path") < 0)) __PYX_ERR(0, 161, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "shortest_path") < 0)) __PYX_ERR(0, 164, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_srcnode = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_srcnode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L3_error)
-    __pyx_v_destnode = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_destnode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L3_error)
+    __pyx_v_srcnode = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_srcnode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L3_error)
+    __pyx_v_destnode = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_destnode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_impno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 161, __pyx_L3_error)
+      __pyx_v_impno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 164, __pyx_L3_error)
     } else {
       __pyx_v_impno = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("shortest_path", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 161, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("shortest_path", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 164, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pandana.cyaccess.cyaccess.shortest_path", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_16shortest_path(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_srcnode, __pyx_v_destnode, __pyx_v_impno);
 
@@ -3505,29 +8372,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shortest_path", 0);
 
-  /* "src/cyaccess.pyx":167
+  /* "src/cyaccess.pyx":170
  *         impno - the impedance id to use
  *         """
  *         return self.access.Route(srcnode, destnode, impno)             # <<<<<<<<<<<<<<
  * 
  *     def shortest_paths(self, np.ndarray[long] srcnodes,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_vector_to_py_int(__pyx_v_self->access->Route(__pyx_v_srcnode, __pyx_v_destnode, __pyx_v_impno)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_to_py_int(__pyx_v_self->access->Route(__pyx_v_srcnode, __pyx_v_destnode, __pyx_v_impno)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":161
+  /* "src/cyaccess.pyx":164
  *         return convert_vector_to_array_dbl(ret)
  * 
  *     def shortest_path(self, int srcnode, int destnode, int impno=0):             # <<<<<<<<<<<<<<
  *         """
  *         srcnode - node id origin
  */
 
@@ -3538,100 +8405,120 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":169
+/* "src/cyaccess.pyx":172
  *         return self.access.Route(srcnode, destnode, impno)
  * 
  *     def shortest_paths(self, np.ndarray[long] srcnodes,             # <<<<<<<<<<<<<<
  *             np.ndarray[long] destnodes, int impno=0):
  *         """
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_19shortest_paths(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pandana_8cyaccess_8cyaccess_18shortest_paths[] = "\n        srcnodes - node ids of origins\n        destnodes - node ids of destinations\n        impno - impedance id\n        ";
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_19shortest_paths(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_19shortest_paths(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7pandana_8cyaccess_8cyaccess_18shortest_paths, "\n        srcnodes - node ids of origins\n        destnodes - node ids of destinations\n        impno - impedance id\n        ");
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_19shortest_paths = {"shortest_paths", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_19shortest_paths, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_18shortest_paths};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_19shortest_paths(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyArrayObject *__pyx_v_srcnodes = 0;
   PyArrayObject *__pyx_v_destnodes = 0;
   int __pyx_v_impno;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shortest_paths (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_srcnodes,&__pyx_n_s_destnodes,&__pyx_n_s_impno,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_srcnodes,&__pyx_n_s_destnodes,&__pyx_n_s_impno,0};
     PyObject* values[3] = {0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_srcnodes)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_srcnodes)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 172, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_destnodes)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_destnodes)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 172, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("shortest_paths", 0, 2, 3, 1); __PYX_ERR(0, 169, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("shortest_paths", 0, 2, 3, 1); __PYX_ERR(0, 172, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_impno);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_impno);
           if (value) { values[2] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 172, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "shortest_paths") < 0)) __PYX_ERR(0, 169, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "shortest_paths") < 0)) __PYX_ERR(0, 172, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_srcnodes = ((PyArrayObject *)values[0]);
     __pyx_v_destnodes = ((PyArrayObject *)values[1]);
     if (values[2]) {
-      __pyx_v_impno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 170, __pyx_L3_error)
+      __pyx_v_impno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 173, __pyx_L3_error)
     } else {
       __pyx_v_impno = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("shortest_paths", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 169, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("shortest_paths", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 172, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pandana.cyaccess.cyaccess.shortest_paths", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_srcnodes), __pyx_ptype_5numpy_ndarray, 1, "srcnodes", 0))) __PYX_ERR(0, 169, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_destnodes), __pyx_ptype_5numpy_ndarray, 1, "destnodes", 0))) __PYX_ERR(0, 170, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_srcnodes), __pyx_ptype_5numpy_ndarray, 1, "srcnodes", 0))) __PYX_ERR(0, 172, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_destnodes), __pyx_ptype_5numpy_ndarray, 1, "destnodes", 0))) __PYX_ERR(0, 173, __pyx_L1_error)
   __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_18shortest_paths(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_srcnodes, __pyx_v_destnodes, __pyx_v_impno);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -3659,40 +8546,40 @@
   __pyx_pybuffernd_srcnodes.rcbuffer = &__pyx_pybuffer_srcnodes;
   __pyx_pybuffer_destnodes.pybuffer.buf = NULL;
   __pyx_pybuffer_destnodes.refcount = 0;
   __pyx_pybuffernd_destnodes.data = NULL;
   __pyx_pybuffernd_destnodes.rcbuffer = &__pyx_pybuffer_destnodes;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_srcnodes.rcbuffer->pybuffer, (PyObject*)__pyx_v_srcnodes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 169, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_srcnodes.rcbuffer->pybuffer, (PyObject*)__pyx_v_srcnodes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 172, __pyx_L1_error)
   }
   __pyx_pybuffernd_srcnodes.diminfo[0].strides = __pyx_pybuffernd_srcnodes.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_srcnodes.diminfo[0].shape = __pyx_pybuffernd_srcnodes.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_destnodes.rcbuffer->pybuffer, (PyObject*)__pyx_v_destnodes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 169, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_destnodes.rcbuffer->pybuffer, (PyObject*)__pyx_v_destnodes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 172, __pyx_L1_error)
   }
   __pyx_pybuffernd_destnodes.diminfo[0].strides = __pyx_pybuffernd_destnodes.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_destnodes.diminfo[0].shape = __pyx_pybuffernd_destnodes.rcbuffer->pybuffer.shape[0];
 
-  /* "src/cyaccess.pyx":176
+  /* "src/cyaccess.pyx":179
  *         impno - impedance id
  *         """
  *         return self.access.Routes(srcnodes, destnodes, impno)             # <<<<<<<<<<<<<<
  * 
  *     def shortest_path_distance(self, int srcnode, int destnode, int impno=0):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_srcnodes)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L1_error)
-  __pyx_t_2 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_destnodes)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 176, __pyx_L1_error)
-  __pyx_t_3 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(__pyx_v_self->access->Routes(__pyx_t_1, __pyx_t_2, __pyx_v_impno)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_srcnodes)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_destnodes)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(__pyx_v_self->access->Routes(__PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_2), __pyx_v_impno)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":169
+  /* "src/cyaccess.pyx":172
  *         return self.access.Route(srcnode, destnode, impno)
  * 
  *     def shortest_paths(self, np.ndarray[long] srcnodes,             # <<<<<<<<<<<<<<
  *             np.ndarray[long] destnodes, int impno=0):
  *         """
  */
 
@@ -3714,93 +8601,113 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_srcnodes.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":178
+/* "src/cyaccess.pyx":181
  *         return self.access.Routes(srcnodes, destnodes, impno)
  * 
  *     def shortest_path_distance(self, int srcnode, int destnode, int impno=0):             # <<<<<<<<<<<<<<
  *         """
  *         srcnode - node id origin
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_21shortest_path_distance(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pandana_8cyaccess_8cyaccess_20shortest_path_distance[] = "\n        srcnode - node id origin\n        destnode - node id destination\n        impno - the impedance id to use\n        ";
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_21shortest_path_distance(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_21shortest_path_distance(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7pandana_8cyaccess_8cyaccess_20shortest_path_distance, "\n        srcnode - node id origin\n        destnode - node id destination\n        impno - the impedance id to use\n        ");
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_21shortest_path_distance = {"shortest_path_distance", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_21shortest_path_distance, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_20shortest_path_distance};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_21shortest_path_distance(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   int __pyx_v_srcnode;
   int __pyx_v_destnode;
   int __pyx_v_impno;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shortest_path_distance (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_srcnode,&__pyx_n_s_destnode,&__pyx_n_s_impno,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_srcnode,&__pyx_n_s_destnode,&__pyx_n_s_impno,0};
     PyObject* values[3] = {0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_srcnode)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_srcnode)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_destnode)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_destnode)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("shortest_path_distance", 0, 2, 3, 1); __PYX_ERR(0, 178, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("shortest_path_distance", 0, 2, 3, 1); __PYX_ERR(0, 181, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_impno);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_impno);
           if (value) { values[2] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "shortest_path_distance") < 0)) __PYX_ERR(0, 178, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "shortest_path_distance") < 0)) __PYX_ERR(0, 181, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_srcnode = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_srcnode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L3_error)
-    __pyx_v_destnode = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_destnode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L3_error)
+    __pyx_v_srcnode = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_srcnode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
+    __pyx_v_destnode = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_destnode == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_impno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 178, __pyx_L3_error)
+      __pyx_v_impno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 181, __pyx_L3_error)
     } else {
       __pyx_v_impno = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("shortest_path_distance", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 178, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("shortest_path_distance", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 181, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pandana.cyaccess.cyaccess.shortest_path_distance", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_20shortest_path_distance(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_srcnode, __pyx_v_destnode, __pyx_v_impno);
 
@@ -3814,29 +8721,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("shortest_path_distance", 0);
 
-  /* "src/cyaccess.pyx":184
+  /* "src/cyaccess.pyx":187
  *         impno - the impedance id to use
  *         """
  *         return self.access.Distance(srcnode, destnode, impno)             # <<<<<<<<<<<<<<
  * 
  *     def shortest_path_distances(self, np.ndarray[long] srcnodes,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->access->Distance(__pyx_v_srcnode, __pyx_v_destnode, __pyx_v_impno)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_v_self->access->Distance(__pyx_v_srcnode, __pyx_v_destnode, __pyx_v_impno)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":178
+  /* "src/cyaccess.pyx":181
  *         return self.access.Routes(srcnodes, destnodes, impno)
  * 
  *     def shortest_path_distance(self, int srcnode, int destnode, int impno=0):             # <<<<<<<<<<<<<<
  *         """
  *         srcnode - node id origin
  */
 
@@ -3847,100 +8754,120 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":186
+/* "src/cyaccess.pyx":189
  *         return self.access.Distance(srcnode, destnode, impno)
  * 
  *     def shortest_path_distances(self, np.ndarray[long] srcnodes,             # <<<<<<<<<<<<<<
  *             np.ndarray[long] destnodes, int impno=0):
  *         """
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_23shortest_path_distances(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_7pandana_8cyaccess_8cyaccess_22shortest_path_distances[] = "\n        srcnodes - node ids of origins\n        destnodes - node ids of destinations\n        impno - impedance id\n        ";
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_23shortest_path_distances(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_23shortest_path_distances(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7pandana_8cyaccess_8cyaccess_22shortest_path_distances, "\n        srcnodes - node ids of origins\n        destnodes - node ids of destinations\n        impno - impedance id\n        ");
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_23shortest_path_distances = {"shortest_path_distances", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_23shortest_path_distances, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_22shortest_path_distances};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_23shortest_path_distances(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   PyArrayObject *__pyx_v_srcnodes = 0;
   PyArrayObject *__pyx_v_destnodes = 0;
   int __pyx_v_impno;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("shortest_path_distances (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_srcnodes,&__pyx_n_s_destnodes,&__pyx_n_s_impno,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_srcnodes,&__pyx_n_s_destnodes,&__pyx_n_s_impno,0};
     PyObject* values[3] = {0,0,0};
-    if (unlikely(__pyx_kwds)) {
+    if (__pyx_kwds) {
       Py_ssize_t kw_args;
-      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
-      switch (pos_args) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = PyDict_Size(__pyx_kwds);
-      switch (pos_args) {
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_srcnodes)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_srcnodes)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_destnodes)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_destnodes)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("shortest_path_distances", 0, 2, 3, 1); __PYX_ERR(0, 186, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("shortest_path_distances", 0, 2, 3, 1); __PYX_ERR(0, 189, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
-          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_impno);
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_impno);
           if (value) { values[2] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 189, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "shortest_path_distances") < 0)) __PYX_ERR(0, 186, __pyx_L3_error)
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "shortest_path_distances") < 0)) __PYX_ERR(0, 189, __pyx_L3_error)
       }
     } else {
-      switch (PyTuple_GET_SIZE(__pyx_args)) {
-        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
-        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_srcnodes = ((PyArrayObject *)values[0]);
     __pyx_v_destnodes = ((PyArrayObject *)values[1]);
     if (values[2]) {
-      __pyx_v_impno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 187, __pyx_L3_error)
+      __pyx_v_impno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 190, __pyx_L3_error)
     } else {
       __pyx_v_impno = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("shortest_path_distances", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 186, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("shortest_path_distances", 0, 2, 3, __pyx_nargs); __PYX_ERR(0, 189, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pandana.cyaccess.cyaccess.shortest_path_distances", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_srcnodes), __pyx_ptype_5numpy_ndarray, 1, "srcnodes", 0))) __PYX_ERR(0, 186, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_destnodes), __pyx_ptype_5numpy_ndarray, 1, "destnodes", 0))) __PYX_ERR(0, 187, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_srcnodes), __pyx_ptype_5numpy_ndarray, 1, "srcnodes", 0))) __PYX_ERR(0, 189, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_destnodes), __pyx_ptype_5numpy_ndarray, 1, "destnodes", 0))) __PYX_ERR(0, 190, __pyx_L1_error)
   __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_22shortest_path_distances(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_srcnodes, __pyx_v_destnodes, __pyx_v_impno);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -3968,40 +8895,40 @@
   __pyx_pybuffernd_srcnodes.rcbuffer = &__pyx_pybuffer_srcnodes;
   __pyx_pybuffer_destnodes.pybuffer.buf = NULL;
   __pyx_pybuffer_destnodes.refcount = 0;
   __pyx_pybuffernd_destnodes.data = NULL;
   __pyx_pybuffernd_destnodes.rcbuffer = &__pyx_pybuffer_destnodes;
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_srcnodes.rcbuffer->pybuffer, (PyObject*)__pyx_v_srcnodes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 186, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_srcnodes.rcbuffer->pybuffer, (PyObject*)__pyx_v_srcnodes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 189, __pyx_L1_error)
   }
   __pyx_pybuffernd_srcnodes.diminfo[0].strides = __pyx_pybuffernd_srcnodes.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_srcnodes.diminfo[0].shape = __pyx_pybuffernd_srcnodes.rcbuffer->pybuffer.shape[0];
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
-    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_destnodes.rcbuffer->pybuffer, (PyObject*)__pyx_v_destnodes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 186, __pyx_L1_error)
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_destnodes.rcbuffer->pybuffer, (PyObject*)__pyx_v_destnodes, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 189, __pyx_L1_error)
   }
   __pyx_pybuffernd_destnodes.diminfo[0].strides = __pyx_pybuffernd_destnodes.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_destnodes.diminfo[0].shape = __pyx_pybuffernd_destnodes.rcbuffer->pybuffer.shape[0];
 
-  /* "src/cyaccess.pyx":193
+  /* "src/cyaccess.pyx":196
  *         impno - impedance id
  *         """
  *         return self.access.Distances(srcnodes, destnodes, impno)             # <<<<<<<<<<<<<<
  * 
  *     def precompute_range(self, double radius):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_srcnodes)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 193, __pyx_L1_error)
-  __pyx_t_2 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_destnodes)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 193, __pyx_L1_error)
-  __pyx_t_3 = __pyx_convert_vector_to_py_double(__pyx_v_self->access->Distances(__pyx_t_1, __pyx_t_2, __pyx_v_impno)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_srcnodes)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_destnodes)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 196, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert_vector_to_py_double(__pyx_v_self->access->Distances(__PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_2), __pyx_v_impno)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "src/cyaccess.pyx":186
+  /* "src/cyaccess.pyx":189
  *         return self.access.Distance(srcnode, destnode, impno)
  * 
  *     def shortest_path_distances(self, np.ndarray[long] srcnodes,             # <<<<<<<<<<<<<<
  *             np.ndarray[long] destnodes, int impno=0):
  *         """
  */
 
@@ -4023,2160 +8950,561 @@
   __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_srcnodes.rcbuffer->pybuffer);
   __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/cyaccess.pyx":195
+/* "src/cyaccess.pyx":198
  *         return self.access.Distances(srcnodes, destnodes, impno)
  * 
  *     def precompute_range(self, double radius):             # <<<<<<<<<<<<<<
  *         self.access.precomputeRangeQueries(radius)
+ * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_25precompute_range(PyObject *__pyx_v_self, PyObject *__pyx_arg_radius); /*proto*/
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_25precompute_range(PyObject *__pyx_v_self, PyObject *__pyx_arg_radius) {
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_25precompute_range(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_25precompute_range = {"precompute_range", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_25precompute_range, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_25precompute_range(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
   double __pyx_v_radius;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("precompute_range (wrapper)", 0);
-  assert(__pyx_arg_radius); {
-    __pyx_v_radius = __pyx_PyFloat_AsDouble(__pyx_arg_radius); if (unlikely((__pyx_v_radius == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 195, __pyx_L3_error)
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_radius,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_radius)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "precompute_range") < 0)) __PYX_ERR(0, 198, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+    }
+    __pyx_v_radius = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_radius == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 198, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("precompute_range", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 198, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("pandana.cyaccess.cyaccess.precompute_range", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_24precompute_range(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), ((double)__pyx_v_radius));
+  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_24precompute_range(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v_radius);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_24precompute_range(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, double __pyx_v_radius) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("precompute_range", 0);
 
-  /* "src/cyaccess.pyx":196
+  /* "src/cyaccess.pyx":199
  * 
  *     def precompute_range(self, double radius):
  *         self.access.precomputeRangeQueries(radius)             # <<<<<<<<<<<<<<
+ * 
+ *     def nodes_in_range(self, vector[long] srcnodes, float radius, int impno,
  */
   __pyx_v_self->access->precomputeRangeQueries(__pyx_v_radius);
 
-  /* "src/cyaccess.pyx":195
+  /* "src/cyaccess.pyx":198
  *         return self.access.Distances(srcnodes, destnodes, impno)
  * 
  *     def precompute_range(self, double radius):             # <<<<<<<<<<<<<<
  *         self.access.precomputeRangeQueries(radius)
+ * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "(tree fragment)":1
- * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
+/* "src/cyaccess.pyx":201
+ *         self.access.precomputeRangeQueries(radius)
+ * 
+ *     def nodes_in_range(self, vector[long] srcnodes, float radius, int impno,             # <<<<<<<<<<<<<<
+ *             np.ndarray[long] ext_ids):
+ *         """
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_27__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_27__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
-  PyObject *__pyx_r = 0;
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_26__reduce_cython__(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_26__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_27nodes_in_range(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_7pandana_8cyaccess_8cyaccess_26nodes_in_range, "\n        srcnodes - node ids of origins\n        radius - maximum range in which to search for nearby nodes\n        impno - the impedance id to use\n        ext_ids - all node ids in the network\n        ");
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_27nodes_in_range = {"nodes_in_range", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_27nodes_in_range, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_26nodes_in_range};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_27nodes_in_range(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  std::vector<long>  __pyx_v_srcnodes;
+  float __pyx_v_radius;
+  int __pyx_v_impno;
+  PyArrayObject *__pyx_v_ext_ids = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
-
-  /* "(tree fragment)":2
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 2, __pyx_L1_error)
-
-  /* "(tree fragment)":1
- * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pandana.cyaccess.cyaccess.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "(tree fragment)":3
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- */
-
-/* Python wrapper */
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_29__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_29__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_28__setstate_cython__(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_28__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
-
-  /* "(tree fragment)":4
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_Raise(__pyx_t_1, 0, 0, 0);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(1, 4, __pyx_L1_error)
-
-  /* "(tree fragment)":3
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("pandana.cyaccess.cyaccess.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = NULL;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":734
- * ctypedef npy_cdouble     complex_t
- * 
- * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew1(PyObject *__pyx_v_a) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":735
- * 
- * cdef inline object PyArray_MultiIterNew1(a):
- *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":734
- * ctypedef npy_cdouble     complex_t
- * 
- * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew1", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":737
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew2(PyObject *__pyx_v_a, PyObject *__pyx_v_b) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":738
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":737
- *     return PyArray_MultiIterNew(1, <void*>a)
- * 
- * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew2", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":740
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew3(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":741
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":740
- *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
- * 
- * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew3", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":743
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew4(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":744
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":743
- *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
- * 
- * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew4", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":746
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyArray_MultiIterNew5(PyObject *__pyx_v_a, PyObject *__pyx_v_b, PyObject *__pyx_v_c, PyObject *__pyx_v_d, PyObject *__pyx_v_e) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":747
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":746
- *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
- * 
- * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("numpy.PyArray_MultiIterNew5", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":749
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":750
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
- *         return <tuple>d.subarray.shape
- *     else:
- */
-  __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":751
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
- *     else:
- *         return ()
- */
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
-    __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
-    goto __pyx_L0;
-
-    /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":750
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):
- *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
- *         return <tuple>d.subarray.shape
- *     else:
- */
-  }
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":753
- *         return <tuple>d.subarray.shape
- *     else:
- *         return ()             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  /*else*/ {
-    __Pyx_XDECREF(__pyx_r);
-    __Pyx_INCREF(__pyx_empty_tuple);
-    __pyx_r = __pyx_empty_tuple;
-    goto __pyx_L0;
-  }
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":749
- *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
- * 
- * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
- *     if PyDataType_HASSUBARRAY(d):
- *         return <tuple>d.subarray.shape
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":868
- *     int _import_umath() except -1
- * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)
- */
-
-static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
-  __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("set_array_base", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":869
- * 
- * cdef inline void set_array_base(ndarray arr, object base):
- *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
- *     PyArray_SetBaseObject(arr, base)
- * 
- */
-  Py_INCREF(__pyx_v_base);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":870
- * cdef inline void set_array_base(ndarray arr, object base):
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
- * 
- * cdef inline object get_array_base(ndarray arr):
- */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":868
- *     int _import_umath() except -1
- * 
- * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
- *     Py_INCREF(base) # important to do this before stealing the reference below!
- *     PyArray_SetBaseObject(arr, base)
- */
-
-  /* function exit code */
-  __Pyx_RefNannyFinishContext();
-}
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":872
- *     PyArray_SetBaseObject(arr, base)
- * 
- * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- */
-
-static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
-  PyObject *__pyx_v_base;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  __Pyx_RefNannySetupContext("get_array_base", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":873
- * 
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
- *     if base is NULL:
- *         return None
- */
-  __pyx_v_base = PyArray_BASE(__pyx_v_arr);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":874
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)
- *     if base is NULL:             # <<<<<<<<<<<<<<
- *         return None
- *     return <object>base
- */
-  __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
-  if (__pyx_t_1) {
-
-    /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":875
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- *         return None             # <<<<<<<<<<<<<<
- *     return <object>base
- * 
- */
-    __Pyx_XDECREF(__pyx_r);
-    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
-    goto __pyx_L0;
-
-    /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":874
- * cdef inline object get_array_base(ndarray arr):
- *     base = PyArray_BASE(arr)
- *     if base is NULL:             # <<<<<<<<<<<<<<
- *         return None
- *     return <object>base
- */
-  }
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":876
- *     if base is NULL:
- *         return None
- *     return <object>base             # <<<<<<<<<<<<<<
- * 
- * # Versions of the import_* functions which are more suitable for
- */
-  __Pyx_XDECREF(__pyx_r);
-  __Pyx_INCREF(((PyObject *)__pyx_v_base));
-  __pyx_r = ((PyObject *)__pyx_v_base);
-  goto __pyx_L0;
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":872
- *     PyArray_SetBaseObject(arr, base)
- * 
- * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
- *     base = PyArray_BASE(arr)
- *     if base is NULL:
- */
-
-  /* function exit code */
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":880
- * # Versions of the import_* functions which are more suitable for
- * # Cython code.
- * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         __pyx_import_array()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_array(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_array", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":881
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
+  __Pyx_RefNannySetupContext("nodes_in_range (wrapper)", 0);
   {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":882
- * cdef inline int import_array() except -1:
- *     try:
- *         __pyx_import_array()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")
- */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 882, __pyx_L3_error)
-
-      /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":881
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":883
- *     try:
- *         __pyx_import_array()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 883, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":884
- *         __pyx_import_array()
- *     except Exception:
- *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef inline int import_umath() except -1:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 884, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 884, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":881
- * # Cython code.
- * cdef inline int import_array() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         __pyx_import_array()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_srcnodes,&__pyx_n_s_radius,&__pyx_n_s_impno,&__pyx_n_s_ext_ids,0};
+    PyObject* values[4] = {0,0,0,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_srcnodes)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_radius)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("nodes_in_range", 1, 4, 4, 1); __PYX_ERR(0, 201, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_impno)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("nodes_in_range", 1, 4, 4, 2); __PYX_ERR(0, 201, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ext_ids)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("nodes_in_range", 1, 4, 4, 3); __PYX_ERR(0, 201, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "nodes_in_range") < 0)) __PYX_ERR(0, 201, __pyx_L3_error)
+      }
+    } else if (unlikely(__pyx_nargs != 4)) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+      values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+    }
+    __pyx_v_srcnodes = __pyx_convert_vector_from_py_long(values[0]); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_radius = __pyx_PyFloat_AsFloat(values[1]); if (unlikely((__pyx_v_radius == (float)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_impno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_impno == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_ext_ids = ((PyArrayObject *)values[3]);
   }
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":880
- * # Versions of the import_* functions which are more suitable for
- * # Cython code.
- * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         __pyx_import_array()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("nodes_in_range", 1, 4, 4, __pyx_nargs); __PYX_ERR(0, 201, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pandana.cyaccess.cyaccess.nodes_in_range", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":886
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_umath(void) {
-  int __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_umath", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":887
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-  {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":888
- * cdef inline int import_umath() except -1:
- *     try:
- *         _import_umath()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
- */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 888, __pyx_L3_error)
-
-      /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":887
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":889
- *     try:
- *         _import_umath()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 889, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":890
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef inline int import_ufunc() except -1:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 890, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 890, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":887
- * 
- * cdef inline int import_umath() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
-  }
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":886
- *         raise ImportError("numpy.core.multiarray failed to import")
- * 
- * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ext_ids), __pyx_ptype_5numpy_ndarray, 1, "ext_ids", 0))) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_26nodes_in_range(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __PYX_STD_MOVE_IF_SUPPORTED(__pyx_v_srcnodes), __pyx_v_radius, __pyx_v_impno, __pyx_v_ext_ids);
 
   /* function exit code */
-  __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
+  __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":892
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-static CYTHON_INLINE int __pyx_f_5numpy_import_ufunc(void) {
-  int __pyx_r;
+static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_26nodes_in_range(struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, std::vector<long>  __pyx_v_srcnodes, float __pyx_v_radius, int __pyx_v_impno, PyArrayObject *__pyx_v_ext_ids) {
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_ext_ids;
+  __Pyx_Buffer __pyx_pybuffer_ext_ids;
+  PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
+  std::vector<long>  __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  PyObject *__pyx_t_7 = NULL;
-  PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("import_ufunc", 0);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":893
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
+  __Pyx_RefNannySetupContext("nodes_in_range", 0);
+  __pyx_pybuffer_ext_ids.pybuffer.buf = NULL;
+  __pyx_pybuffer_ext_ids.refcount = 0;
+  __pyx_pybuffernd_ext_ids.data = NULL;
+  __pyx_pybuffernd_ext_ids.rcbuffer = &__pyx_pybuffer_ext_ids;
   {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
-    __Pyx_XGOTREF(__pyx_t_1);
-    __Pyx_XGOTREF(__pyx_t_2);
-    __Pyx_XGOTREF(__pyx_t_3);
-    /*try:*/ {
-
-      /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":894
- * cdef inline int import_ufunc() except -1:
- *     try:
- *         _import_umath()             # <<<<<<<<<<<<<<
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")
- */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 894, __pyx_L3_error)
-
-      /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":893
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    }
-    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    goto __pyx_L8_try_end;
-    __pyx_L3_error:;
-
-    /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":895
- *     try:
- *         _import_umath()
- *     except Exception:             # <<<<<<<<<<<<<<
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- */
-    __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-    if (__pyx_t_4) {
-      __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 895, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_5);
-      __Pyx_GOTREF(__pyx_t_6);
-      __Pyx_GOTREF(__pyx_t_7);
-
-      /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":896
- *         _import_umath()
- *     except Exception:
- *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
- * 
- * cdef extern from *:
- */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 896, __pyx_L5_except_error)
-      __Pyx_GOTREF(__pyx_t_8);
-      __Pyx_Raise(__pyx_t_8, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 896, __pyx_L5_except_error)
-    }
-    goto __pyx_L5_except_error;
-    __pyx_L5_except_error:;
-
-    /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":893
- * 
- * cdef inline int import_ufunc() except -1:
- *     try:             # <<<<<<<<<<<<<<
- *         _import_umath()
- *     except Exception:
- */
-    __Pyx_XGIVEREF(__pyx_t_1);
-    __Pyx_XGIVEREF(__pyx_t_2);
-    __Pyx_XGIVEREF(__pyx_t_3);
-    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
-    goto __pyx_L1_error;
-    __pyx_L8_try_end:;
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_ext_ids.rcbuffer->pybuffer, (PyObject*)__pyx_v_ext_ids, &__Pyx_TypeInfo_long, PyBUF_FORMAT| PyBUF_STRIDES, 1, 0, __pyx_stack) == -1)) __PYX_ERR(0, 201, __pyx_L1_error)
   }
+  __pyx_pybuffernd_ext_ids.diminfo[0].strides = __pyx_pybuffernd_ext_ids.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_ext_ids.diminfo[0].shape = __pyx_pybuffernd_ext_ids.rcbuffer->pybuffer.shape[0];
 
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":892
- *         raise ImportError("numpy.core.umath failed to import")
- * 
- * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
- *     try:
- *         _import_umath()
- */
-
-  /* function exit code */
-  __pyx_r = 0;
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = -1;
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.from_py":13
- * 
- * @cname("__pyx_convert_string_from_py_std__in_string")
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t length = 0
- *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
- */
-
-static std::string __pyx_convert_string_from_py_std__in_string(PyObject *__pyx_v_o) {
-  Py_ssize_t __pyx_v_length;
-  char const *__pyx_v_data;
-  std::string __pyx_r;
-  __Pyx_RefNannyDeclarations
-  char const *__pyx_t_1;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_string_from_py_std__in_string", 0);
-
-  /* "string.from_py":14
- * @cname("__pyx_convert_string_from_py_std__in_string")
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
- *     cdef Py_ssize_t length = 0             # <<<<<<<<<<<<<<
- *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
- *     return string(data, length)
- */
-  __pyx_v_length = 0;
-
-  /* "string.from_py":15
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:
- *     cdef Py_ssize_t length = 0
- *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)             # <<<<<<<<<<<<<<
- *     return string(data, length)
- * 
- */
-  __pyx_t_1 = __Pyx_PyObject_AsStringAndSize(__pyx_v_o, (&__pyx_v_length)); if (unlikely(__pyx_t_1 == ((char const *)NULL))) __PYX_ERR(1, 15, __pyx_L1_error)
-  __pyx_v_data = __pyx_t_1;
-
-  /* "string.from_py":16
- *     cdef Py_ssize_t length = 0
- *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
- *     return string(data, length)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = std::string(__pyx_v_data, __pyx_v_length);
-  goto __pyx_L0;
-
-  /* "string.from_py":13
- * 
- * @cname("__pyx_convert_string_from_py_std__in_string")
- * cdef string __pyx_convert_string_from_py_std__in_string(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t length = 0
- *     cdef const char* data = __Pyx_PyObject_AsStringAndSize(o, &length)
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_double")
- * cdef object __pyx_convert_vector_to_py_double(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
- */
-
-static PyObject *__pyx_convert_vector_to_py_double(const std::vector<double>  &__pyx_v_v) {
-  size_t __pyx_v_i;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  size_t __pyx_t_2;
-  size_t __pyx_t_3;
-  size_t __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_double", 0);
-
-  /* "vector.to_py":61
- * @cname("__pyx_convert_vector_to_py_double")
- * cdef object __pyx_convert_vector_to_py_double(vector[X]& v):
- *     return [v[i] for i in range(v.size())]             # <<<<<<<<<<<<<<
- * 
- * 
+  /* "src/cyaccess.pyx":209
+ *         ext_ids - all node ids in the network
+ *         """
+ *         return self.access.Range(srcnodes, radius, impno, ext_ids)             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 61, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_v_v.size();
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_i = __pyx_t_4;
-    __pyx_t_5 = PyFloat_FromDouble((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_1 = __pyx_convert_vector_from_py_long(((PyObject *)__pyx_v_ext_ids)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_vector_to_py_std_3a__3a_vector_3c_std_3a__3a_pair_3c_long_2c_float_3e____3e___(__pyx_v_self->access->Range(__pyx_v_srcnodes, __pyx_v_radius, __pyx_v_impno, __PYX_STD_MOVE_IF_SUPPORTED(__pyx_t_1))); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_double")
- * cdef object __pyx_convert_vector_to_py_double(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
+  /* "src/cyaccess.pyx":201
+ *         self.access.precomputeRangeQueries(radius)
  * 
+ *     def nodes_in_range(self, vector[long] srcnodes, float radius, int impno,             # <<<<<<<<<<<<<<
+ *             np.ndarray[long] ext_ids):
+ *         """
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
+  __Pyx_XDECREF(__pyx_t_2);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ext_ids.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("pandana.cyaccess.cyaccess.nodes_in_range", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
   __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_ext_ids.rcbuffer->pybuffer);
+  __pyx_L2:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(const std::vector<std::vector<double> >  &__pyx_v_v) {
-  size_t __pyx_v_i;
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  size_t __pyx_t_2;
-  size_t __pyx_t_3;
-  size_t __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___", 0);
-
-  /* "vector.to_py":61
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(vector[X]& v):
- *     return [v[i] for i in range(v.size())]             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 61, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_v_v.size();
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_i = __pyx_t_4;
-    __pyx_t_5 = __pyx_convert_vector_to_py_double((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
+/* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
  */
 
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_std_3a__3a_vector_3c_double_3e___", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static PyObject *__pyx_convert_vector_to_py_int(const std::vector<int>  &__pyx_v_v) {
-  size_t __pyx_v_i;
-  PyObject *__pyx_r = NULL;
+/* Python wrapper */
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_29__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_29__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_29__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_29__reduce_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  size_t __pyx_t_2;
-  size_t __pyx_t_3;
-  size_t __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_int", 0);
-
-  /* "vector.to_py":61
- * @cname("__pyx_convert_vector_to_py_int")
- * cdef object __pyx_convert_vector_to_py_int(vector[X]& v):
- *     return [v[i] for i in range(v.size())]             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 61, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_v_v.size();
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_i = __pyx_t_4;
-    __pyx_t_5 = __Pyx_PyInt_From_int((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_int")
- * cdef object __pyx_convert_vector_to_py_int(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
- */
+  __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
+  if (unlikely(__pyx_nargs > 0)) {
+    __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
+  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
+  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_28__reduce_cython__(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self));
 
   /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_int", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(const std::vector<std::vector<int> >  &__pyx_v_v) {
-  size_t __pyx_v_i;
+static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_28__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  size_t __pyx_t_2;
-  size_t __pyx_t_3;
-  size_t __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___", 0);
+  __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
-  /* "vector.to_py":61
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(vector[X]& v):
- *     return [v[i] for i in range(v.size())]             # <<<<<<<<<<<<<<
- * 
- * 
+  /* "(tree fragment)":2
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
+ * def __setstate_cython__(self, __pyx_state):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 61, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_v_v.size();
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_i = __pyx_t_4;
-    __pyx_t_5 = __pyx_convert_vector_to_py_int((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
+  __PYX_ERR(1, 2, __pyx_L1_error)
 
-  /* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_std_3a__3a_vector_3c_int_3e___", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
+  __Pyx_AddTraceback("pandana.cyaccess.cyaccess.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "vector.from_py":45
- * 
- * @cname("__pyx_convert_vector_from_py_long")
- * cdef vector[X] __pyx_convert_vector_from_py_long(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef vector[X] v
- *     for item in o:
- */
-
-static std::vector<long>  __pyx_convert_vector_from_py_long(PyObject *__pyx_v_o) {
-  std::vector<long>  __pyx_v_v;
-  PyObject *__pyx_v_item = NULL;
-  std::vector<long>  __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *(*__pyx_t_3)(PyObject *);
-  PyObject *__pyx_t_4 = NULL;
-  long __pyx_t_5;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_long", 0);
-
-  /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_long(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
-    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-    __pyx_t_3 = NULL;
-  } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_3)) {
-      if (likely(PyList_CheckExact(__pyx_t_1))) {
-        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      } else {
-        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      }
-    } else {
-      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
-      if (unlikely(!__pyx_t_4)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 47, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_4);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "vector.from_py":48
- *     cdef vector[X] v
- *     for item in o:
- *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
- *     return v
- * 
- */
-    __pyx_t_5 = __Pyx_PyInt_As_long(__pyx_v_item); if (unlikely((__pyx_t_5 == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
-    __pyx_v_v.push_back(((long)__pyx_t_5));
-
-    /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_long(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "vector.from_py":49
- *     for item in o:
- *         v.push_back(<X>item)
- *     return v             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_v;
-  goto __pyx_L0;
-
-  /* "vector.from_py":45
- * 
- * @cname("__pyx_convert_vector_from_py_long")
- * cdef vector[X] __pyx_convert_vector_from_py_long(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef vector[X] v
- *     for item in o:
+/* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
 
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_long", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_item);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static std::vector<std::vector<long> >  __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(PyObject *__pyx_v_o) {
-  std::vector<std::vector<long> >  __pyx_v_v;
-  PyObject *__pyx_v_item = NULL;
-  std::vector<std::vector<long> >  __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *(*__pyx_t_3)(PyObject *);
-  PyObject *__pyx_t_4 = NULL;
-  std::vector<long>  __pyx_t_5;
+/* Python wrapper */
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_31__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static PyMethodDef __pyx_mdef_7pandana_8cyaccess_8cyaccess_31__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_31__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7pandana_8cyaccess_8cyaccess_31__setstate_cython__(PyObject *__pyx_v_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  CYTHON_UNUSED PyObject *__pyx_v___pyx_state = 0;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___", 0);
-
-  /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
-    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-    __pyx_t_3 = NULL;
-  } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_3)) {
-      if (likely(PyList_CheckExact(__pyx_t_1))) {
-        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      } else {
-        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      }
-    } else {
-      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
-      if (unlikely(!__pyx_t_4)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 47, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_4);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "vector.from_py":48
- *     cdef vector[X] v
- *     for item in o:
- *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
- *     return v
- * 
- */
-    __pyx_t_5 = __pyx_convert_vector_from_py_long(__pyx_v_item); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
-    __pyx_v_v.push_back(((std::vector<long> )__pyx_t_5));
-
-    /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "vector.from_py":49
- *     for item in o:
- *         v.push_back(<X>item)
- *     return v             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_v;
-  goto __pyx_L0;
-
-  /* "vector.from_py":45
- * 
- * @cname("__pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___")
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef vector[X] v
- *     for item in o:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_std_3a__3a_vector_3c_long_3e___", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_item);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static std::vector<double>  __pyx_convert_vector_from_py_double(PyObject *__pyx_v_o) {
-  std::vector<double>  __pyx_v_v;
-  PyObject *__pyx_v_item = NULL;
-  std::vector<double>  __pyx_r;
+  PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *(*__pyx_t_3)(PyObject *);
-  PyObject *__pyx_t_4 = NULL;
-  double __pyx_t_5;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_double", 0);
-
-  /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_double(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
-    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-    __pyx_t_3 = NULL;
-  } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_3)) {
-      if (likely(PyList_CheckExact(__pyx_t_1))) {
-        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      } else {
-        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
+  __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
+    PyObject* values[1] = {0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
       }
-    } else {
-      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
-      if (unlikely(!__pyx_t_4)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 47, __pyx_L1_error)
-        }
-        break;
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 3, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
       }
-      __Pyx_GOTREF(__pyx_t_4);
-    }
-    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "vector.from_py":48
- *     cdef vector[X] v
- *     for item in o:
- *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
- *     return v
- * 
- */
-    __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_v_item); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
-    __pyx_v_v.push_back(((double)__pyx_t_5));
-
-    /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_double(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "vector.from_py":49
- *     for item in o:
- *         v.push_back(<X>item)
- *     return v             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_v;
-  goto __pyx_L0;
-
-  /* "vector.from_py":45
- * 
- * @cname("__pyx_convert_vector_from_py_double")
- * cdef vector[X] __pyx_convert_vector_from_py_double(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef vector[X] v
- *     for item in o:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_item);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-static std::vector<std::vector<double> >  __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(PyObject *__pyx_v_o) {
-  std::vector<std::vector<double> >  __pyx_v_v;
-  PyObject *__pyx_v_item = NULL;
-  std::vector<std::vector<double> >  __pyx_r;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  PyObject *(*__pyx_t_3)(PyObject *);
-  PyObject *__pyx_t_4 = NULL;
-  std::vector<double>  __pyx_t_5;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___", 0);
-
-  /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
-  if (likely(PyList_CheckExact(__pyx_v_o)) || PyTuple_CheckExact(__pyx_v_o)) {
-    __pyx_t_1 = __pyx_v_o; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
-    __pyx_t_3 = NULL;
-  } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_v_o); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 47, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 47, __pyx_L1_error)
-  }
-  for (;;) {
-    if (likely(!__pyx_t_3)) {
-      if (likely(PyList_CheckExact(__pyx_t_1))) {
-        if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
-      } else {
-        if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
-        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(1, 47, __pyx_L1_error)
-        #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 47, __pyx_L1_error)
-        __Pyx_GOTREF(__pyx_t_4);
-        #endif
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 3, __pyx_L3_error)
       }
+    } else if (unlikely(__pyx_nargs != 1)) {
+      goto __pyx_L5_argtuple_error;
     } else {
-      __pyx_t_4 = __pyx_t_3(__pyx_t_1);
-      if (unlikely(!__pyx_t_4)) {
-        PyObject* exc_type = PyErr_Occurred();
-        if (exc_type) {
-          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(1, 47, __pyx_L1_error)
-        }
-        break;
-      }
-      __Pyx_GOTREF(__pyx_t_4);
+      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
-    __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_4);
-    __pyx_t_4 = 0;
-
-    /* "vector.from_py":48
- *     cdef vector[X] v
- *     for item in o:
- *         v.push_back(<X>item)             # <<<<<<<<<<<<<<
- *     return v
- * 
- */
-    __pyx_t_5 = __pyx_convert_vector_from_py_double(__pyx_v_item); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 48, __pyx_L1_error)
-    __pyx_v_v.push_back(((std::vector<double> )__pyx_t_5));
-
-    /* "vector.from_py":47
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(object o) except *:
- *     cdef vector[X] v
- *     for item in o:             # <<<<<<<<<<<<<<
- *         v.push_back(<X>item)
- *     return v
- */
+    __pyx_v___pyx_state = values[0];
   }
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-
-  /* "vector.from_py":49
- *     for item in o:
- *         v.push_back(<X>item)
- *     return v             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  __pyx_r = __pyx_v_v;
-  goto __pyx_L0;
-
-  /* "vector.from_py":45
- * 
- * @cname("__pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___")
- * cdef vector[X] __pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___(object o) except *:             # <<<<<<<<<<<<<<
- *     cdef vector[X] v
- *     for item in o:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("vector.from_py.__pyx_convert_vector_from_py_std_3a__3a_vector_3c_double_3e___", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_pretend_to_initialize(&__pyx_r);
-  __pyx_L0:;
-  __Pyx_XDECREF(__pyx_v_item);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":31
- * 
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyObject_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":32
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyUnicode_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 32, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":31
- * 
- * @cname("__pyx_convert_PyObject_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyObject_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyObject_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyObject_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":37
- * 
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyUnicode_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":38
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyStr_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyUnicode_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 38, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":37
- * 
- * @cname("__pyx_convert_PyUnicode_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyUnicode_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyUnicode_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyUnicode_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":43
- * 
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyStr_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":44
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyBytes_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyStr_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 44, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":43
- * 
- * @cname("__pyx_convert_PyStr_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyStr_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyStr_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyStr_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
-  __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":49
- * 
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyBytes_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":50
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * cdef extern from *:
- *     cdef object __Pyx_PyByteArray_FromStringAndSize(const char*, size_t)
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 50, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":49
- * 
- * @cname("__pyx_convert_PyBytes_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyBytes_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyBytes_FromStringAndSize(s.data(), s.size())
- * cdef extern from *:
- */
-
-  /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyBytes_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 3, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("pandana.cyaccess.cyaccess.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
-  return __pyx_r;
-}
-
-/* "string.to_py":55
- * 
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
- * 
- */
-
-static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &__pyx_v_s) {
-  PyObject *__pyx_r = NULL;
-  __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_PyByteArray_string_to_py_std__in_string", 0);
-
-  /* "string.to_py":56
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):
- *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())             # <<<<<<<<<<<<<<
- * 
- */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyByteArray_FromStringAndSize(__pyx_v_s.data(), __pyx_v_s.size()); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 56, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
-
-  /* "string.to_py":55
- * 
- * @cname("__pyx_convert_PyByteArray_string_to_py_std__in_string")
- * cdef inline object __pyx_convert_PyByteArray_string_to_py_std__in_string(const string& s):             # <<<<<<<<<<<<<<
- *     return __Pyx_PyByteArray_FromStringAndSize(s.data(), s.size())
- * 
- */
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_7pandana_8cyaccess_8cyaccess_30__setstate_cython__(((struct __pyx_obj_7pandana_8cyaccess_cyaccess *)__pyx_v_self), __pyx_v___pyx_state);
 
   /* function exit code */
-  __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("string.to_py.__pyx_convert_PyByteArray_string_to_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
-  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
- */
-
-static PyObject *__pyx_convert_vector_to_py_std_3a__3a_string(const std::vector<std::string>  &__pyx_v_v) {
-  size_t __pyx_v_i;
+static PyObject *__pyx_pf_7pandana_8cyaccess_8cyaccess_30__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7pandana_8cyaccess_cyaccess *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  size_t __pyx_t_2;
-  size_t __pyx_t_3;
-  size_t __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("__pyx_convert_vector_to_py_std_3a__3a_string", 0);
+  __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
-  /* "vector.to_py":61
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(vector[X]& v):
- *     return [v[i] for i in range(v.size())]             # <<<<<<<<<<<<<<
- * 
- * 
+  /* "(tree fragment)":4
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"             # <<<<<<<<<<<<<<
  */
-  __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 61, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_v_v.size();
-  __pyx_t_3 = __pyx_t_2;
-  for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
-    __pyx_v_i = __pyx_t_4;
-    __pyx_t_5 = __pyx_convert_PyBytes_string_to_py_std__in_string((__pyx_v_v[__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(1, 61, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  }
-  __pyx_r = __pyx_t_1;
-  __pyx_t_1 = 0;
-  goto __pyx_L0;
+  __Pyx_Raise(__pyx_builtin_TypeError, __pyx_kp_s_no_default___reduce___due_to_non, 0, 0);
+  __PYX_ERR(1, 4, __pyx_L1_error)
 
-  /* "vector.to_py":60
- * 
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
- * 
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("vector.to_py.__pyx_convert_vector_to_py_std_3a__3a_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __pyx_r = 0;
-  __pyx_L0:;
+  __Pyx_AddTraceback("pandana.cyaccess.cyaccess.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_tp_new_7pandana_8cyaccess_cyaccess(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o;
-  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
+  #if CYTHON_COMPILING_IN_LIMITED_API
+  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
+  o = alloc_func(t, 0);
+  #else
+  if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
+  #endif
   if (unlikely(__pyx_pw_7pandana_8cyaccess_8cyaccess_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_7pandana_8cyaccess_cyaccess(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
-    if (PyObject_CallFinalizerFromDealloc(o)) return;
+  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
+    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_7pandana_8cyaccess_cyaccess) {
+      if (PyObject_CallFinalizerFromDealloc(o)) return;
+    }
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
     __pyx_pw_7pandana_8cyaccess_8cyaccess_3__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyMethodDef __pyx_methods_7pandana_8cyaccess_cyaccess[] = {
-  {"initialize_category", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_5initialize_category, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_4initialize_category},
-  {"find_all_nearest_pois", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_7find_all_nearest_pois, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_6find_all_nearest_pois},
-  {"initialize_access_var", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_9initialize_access_var, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_8initialize_access_var},
-  {"get_available_aggregations", (PyCFunction)__pyx_pw_7pandana_8cyaccess_8cyaccess_11get_available_aggregations, METH_NOARGS, 0},
-  {"get_available_decays", (PyCFunction)__pyx_pw_7pandana_8cyaccess_8cyaccess_13get_available_decays, METH_NOARGS, 0},
-  {"get_all_aggregate_accessibility_variables", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_15get_all_aggregate_accessibility_variables, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_14get_all_aggregate_accessibility_variables},
-  {"shortest_path", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_17shortest_path, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_16shortest_path},
-  {"shortest_paths", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_19shortest_paths, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_18shortest_paths},
-  {"shortest_path_distance", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_21shortest_path_distance, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_20shortest_path_distance},
-  {"shortest_path_distances", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_23shortest_path_distances, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_22shortest_path_distances},
-  {"precompute_range", (PyCFunction)__pyx_pw_7pandana_8cyaccess_8cyaccess_25precompute_range, METH_O, 0},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_7pandana_8cyaccess_8cyaccess_27__reduce_cython__, METH_NOARGS, 0},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_7pandana_8cyaccess_8cyaccess_29__setstate_cython__, METH_O, 0},
+  {"initialize_category", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_5initialize_category, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_4initialize_category},
+  {"find_all_nearest_pois", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_7find_all_nearest_pois, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_6find_all_nearest_pois},
+  {"initialize_access_var", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_9initialize_access_var, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_8initialize_access_var},
+  {"get_available_aggregations", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_11get_available_aggregations, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"get_available_decays", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_13get_available_decays, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"get_all_aggregate_accessibility_variables", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_15get_all_aggregate_accessibility_variables, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_14get_all_aggregate_accessibility_variables},
+  {"shortest_path", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_17shortest_path, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_16shortest_path},
+  {"shortest_paths", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_19shortest_paths, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_18shortest_paths},
+  {"shortest_path_distance", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_21shortest_path_distance, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_20shortest_path_distance},
+  {"shortest_path_distances", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_23shortest_path_distances, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_22shortest_path_distances},
+  {"precompute_range", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_25precompute_range, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"nodes_in_range", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_27nodes_in_range, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_7pandana_8cyaccess_8cyaccess_26nodes_in_range},
+  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_29__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7pandana_8cyaccess_8cyaccess_31__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
 };
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_type_7pandana_8cyaccess_cyaccess_slots[] = {
+  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_7pandana_8cyaccess_cyaccess},
+  {Py_tp_methods, (void *)__pyx_methods_7pandana_8cyaccess_cyaccess},
+  {Py_tp_new, (void *)__pyx_tp_new_7pandana_8cyaccess_cyaccess},
+  {0, 0},
+};
+static PyType_Spec __pyx_type_7pandana_8cyaccess_cyaccess_spec = {
+  "pandana.cyaccess.cyaccess",
+  sizeof(struct __pyx_obj_7pandana_8cyaccess_cyaccess),
+  0,
+  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE,
+  __pyx_type_7pandana_8cyaccess_cyaccess_slots,
+};
+#else
 
 static PyTypeObject __pyx_type_7pandana_8cyaccess_cyaccess = {
   PyVarObject_HEAD_INIT(0, 0)
-  "pandana.cyaccess.cyaccess", /*tp_name*/
+  "pandana.cyaccess.""cyaccess", /*tp_name*/
   sizeof(struct __pyx_obj_7pandana_8cyaccess_cyaccess), /*tp_basicsize*/
   0, /*tp_itemsize*/
   __pyx_tp_dealloc_7pandana_8cyaccess_cyaccess, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
@@ -6211,195 +9539,393 @@
   __pyx_methods_7pandana_8cyaccess_cyaccess, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
+  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
+  #endif
   0, /*tp_init*/
   0, /*tp_alloc*/
   __pyx_tp_new_7pandana_8cyaccess_cyaccess, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
+  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
+  #else
+  NULL, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #endif
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
+  #if __PYX_NEED_TP_PRINT_SLOT == 1
   0, /*tp_print*/
   #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+  0, /*tp_watched*/
+  #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+  0, /*tp_pypy_flags*/
+  #endif
 };
+#endif
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
-
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_cyaccess(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_cyaccess},
-  {0, NULL}
-};
-#endif
-
-static struct PyModuleDef __pyx_moduledef = {
-    PyModuleDef_HEAD_INIT,
-    "cyaccess",
-    0, /* m_doc */
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    0, /* m_size */
-  #else
-    -1, /* m_size */
-  #endif
-    __pyx_methods /* m_methods */,
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-    __pyx_moduledef_slots, /* m_slots */
-  #else
-    NULL, /* m_reload */
-  #endif
-    NULL, /* m_traverse */
-    NULL, /* m_clear */
-    NULL /* m_free */
-};
-#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
+/* #### Code section: pystring_table ### */
 
-static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
-  {&__pyx_n_s_aggtyp, __pyx_k_aggtyp, sizeof(__pyx_k_aggtyp), 0, 0, 1, 1},
-  {&__pyx_n_s_category, __pyx_k_category, sizeof(__pyx_k_category), 0, 0, 1, 1},
-  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_cyaccess, __pyx_k_cyaccess, sizeof(__pyx_k_cyaccess), 0, 0, 1, 1},
-  {&__pyx_n_s_decay, __pyx_k_decay, sizeof(__pyx_k_decay), 0, 0, 1, 1},
-  {&__pyx_n_s_destnode, __pyx_k_destnode, sizeof(__pyx_k_destnode), 0, 0, 1, 1},
-  {&__pyx_n_s_destnodes, __pyx_k_destnodes, sizeof(__pyx_k_destnodes), 0, 0, 1, 1},
-  {&__pyx_n_s_double, __pyx_k_double, sizeof(__pyx_k_double), 0, 0, 1, 1},
-  {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
-  {&__pyx_n_s_edge_weights, __pyx_k_edge_weights, sizeof(__pyx_k_edge_weights), 0, 0, 1, 1},
-  {&__pyx_n_s_edges, __pyx_k_edges, sizeof(__pyx_k_edges), 0, 0, 1, 1},
-  {&__pyx_n_s_empty_like, __pyx_k_empty_like, sizeof(__pyx_k_empty_like), 0, 0, 1, 1},
-  {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
-  {&__pyx_n_s_impno, __pyx_k_impno, sizeof(__pyx_k_impno), 0, 0, 1, 1},
-  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-  {&__pyx_n_s_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 0, 1, 1},
-  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-  {&__pyx_n_s_maxdist, __pyx_k_maxdist, sizeof(__pyx_k_maxdist), 0, 0, 1, 1},
-  {&__pyx_n_s_maxitems, __pyx_k_maxitems, sizeof(__pyx_k_maxitems), 0, 0, 1, 1},
-  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-  {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
-  {&__pyx_n_s_node_ids, __pyx_k_node_ids, sizeof(__pyx_k_node_ids), 0, 0, 1, 1},
-  {&__pyx_n_s_node_xys, __pyx_k_node_xys, sizeof(__pyx_k_node_xys), 0, 0, 1, 1},
-  {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
-  {&__pyx_n_s_num_of_pois, __pyx_k_num_of_pois, sizeof(__pyx_k_num_of_pois), 0, 0, 1, 1},
-  {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
-  {&__pyx_kp_s_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 0, 1, 0},
-  {&__pyx_kp_s_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 0, 1, 0},
-  {&__pyx_n_s_radius, __pyx_k_radius, sizeof(__pyx_k_radius), 0, 0, 1, 1},
-  {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
-  {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-  {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
-  {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
-  {&__pyx_n_s_srcnode, __pyx_k_srcnode, sizeof(__pyx_k_srcnode), 0, 0, 1, 1},
-  {&__pyx_n_s_srcnodes, __pyx_k_srcnodes, sizeof(__pyx_k_srcnodes), 0, 0, 1, 1},
-  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-  {&__pyx_n_s_twoway, __pyx_k_twoway, sizeof(__pyx_k_twoway), 0, 0, 1, 1},
-  {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
-  {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
-  {0, 0, 0, 0, 0, 0, 0}
-};
+static int __Pyx_CreateStringTabAndInitStrings(void) {
+  __Pyx_StringTabEntry __pyx_string_tab[] = {
+    {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
+    {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
+    {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
+    {&__pyx_n_s__29, __pyx_k__29, sizeof(__pyx_k__29), 0, 0, 1, 1},
+    {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
+    {&__pyx_n_s_aggtyp, __pyx_k_aggtyp, sizeof(__pyx_k_aggtyp), 0, 0, 1, 1},
+    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
+    {&__pyx_n_s_category, __pyx_k_category, sizeof(__pyx_k_category), 0, 0, 1, 1},
+    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess, __pyx_k_cyaccess, sizeof(__pyx_k_cyaccess), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess___reduce_cython, __pyx_k_cyaccess___reduce_cython, sizeof(__pyx_k_cyaccess___reduce_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess___setstate_cython, __pyx_k_cyaccess___setstate_cython, sizeof(__pyx_k_cyaccess___setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_find_all_nearest_pois, __pyx_k_cyaccess_find_all_nearest_pois, sizeof(__pyx_k_cyaccess_find_all_nearest_pois), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_get_all_aggregate_acces, __pyx_k_cyaccess_get_all_aggregate_acces, sizeof(__pyx_k_cyaccess_get_all_aggregate_acces), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_get_available_aggregati, __pyx_k_cyaccess_get_available_aggregati, sizeof(__pyx_k_cyaccess_get_available_aggregati), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_get_available_decays, __pyx_k_cyaccess_get_available_decays, sizeof(__pyx_k_cyaccess_get_available_decays), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_initialize_access_var, __pyx_k_cyaccess_initialize_access_var, sizeof(__pyx_k_cyaccess_initialize_access_var), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_initialize_category, __pyx_k_cyaccess_initialize_category, sizeof(__pyx_k_cyaccess_initialize_category), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_nodes_in_range, __pyx_k_cyaccess_nodes_in_range, sizeof(__pyx_k_cyaccess_nodes_in_range), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_precompute_range, __pyx_k_cyaccess_precompute_range, sizeof(__pyx_k_cyaccess_precompute_range), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_shortest_path, __pyx_k_cyaccess_shortest_path, sizeof(__pyx_k_cyaccess_shortest_path), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_shortest_path_distance, __pyx_k_cyaccess_shortest_path_distance, sizeof(__pyx_k_cyaccess_shortest_path_distance), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_shortest_path_distances, __pyx_k_cyaccess_shortest_path_distances, sizeof(__pyx_k_cyaccess_shortest_path_distances), 0, 0, 1, 1},
+    {&__pyx_n_s_cyaccess_shortest_paths, __pyx_k_cyaccess_shortest_paths, sizeof(__pyx_k_cyaccess_shortest_paths), 0, 0, 1, 1},
+    {&__pyx_n_s_decay, __pyx_k_decay, sizeof(__pyx_k_decay), 0, 0, 1, 1},
+    {&__pyx_n_s_destnode, __pyx_k_destnode, sizeof(__pyx_k_destnode), 0, 0, 1, 1},
+    {&__pyx_n_s_destnodes, __pyx_k_destnodes, sizeof(__pyx_k_destnodes), 0, 0, 1, 1},
+    {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
+    {&__pyx_n_u_double, __pyx_k_double, sizeof(__pyx_k_double), 0, 1, 0, 1},
+    {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
+    {&__pyx_n_s_edge_weights, __pyx_k_edge_weights, sizeof(__pyx_k_edge_weights), 0, 0, 1, 1},
+    {&__pyx_n_s_edges, __pyx_k_edges, sizeof(__pyx_k_edges), 0, 0, 1, 1},
+    {&__pyx_n_s_empty_like, __pyx_k_empty_like, sizeof(__pyx_k_empty_like), 0, 0, 1, 1},
+    {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+    {&__pyx_n_s_ext_ids, __pyx_k_ext_ids, sizeof(__pyx_k_ext_ids), 0, 0, 1, 1},
+    {&__pyx_n_s_find_all_nearest_pois, __pyx_k_find_all_nearest_pois, sizeof(__pyx_k_find_all_nearest_pois), 0, 0, 1, 1},
+    {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
+    {&__pyx_n_s_get_all_aggregate_accessibility, __pyx_k_get_all_aggregate_accessibility, sizeof(__pyx_k_get_all_aggregate_accessibility), 0, 0, 1, 1},
+    {&__pyx_n_s_get_available_aggregations, __pyx_k_get_available_aggregations, sizeof(__pyx_k_get_available_aggregations), 0, 0, 1, 1},
+    {&__pyx_n_s_get_available_decays, __pyx_k_get_available_decays, sizeof(__pyx_k_get_available_decays), 0, 0, 1, 1},
+    {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+    {&__pyx_n_s_impno, __pyx_k_impno, sizeof(__pyx_k_impno), 0, 0, 1, 1},
+    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+    {&__pyx_n_s_initialize_access_var, __pyx_k_initialize_access_var, sizeof(__pyx_k_initialize_access_var), 0, 0, 1, 1},
+    {&__pyx_n_s_initialize_category, __pyx_k_initialize_category, sizeof(__pyx_k_initialize_category), 0, 0, 1, 1},
+    {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
+    {&__pyx_n_u_int, __pyx_k_int, sizeof(__pyx_k_int), 0, 1, 0, 1},
+    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
+    {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
+    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+    {&__pyx_n_s_maxdist, __pyx_k_maxdist, sizeof(__pyx_k_maxdist), 0, 0, 1, 1},
+    {&__pyx_n_s_maxitems, __pyx_k_maxitems, sizeof(__pyx_k_maxitems), 0, 0, 1, 1},
+    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+    {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
+    {&__pyx_n_s_node_ids, __pyx_k_node_ids, sizeof(__pyx_k_node_ids), 0, 0, 1, 1},
+    {&__pyx_n_s_node_xys, __pyx_k_node_xys, sizeof(__pyx_k_node_xys), 0, 0, 1, 1},
+    {&__pyx_n_s_nodes_in_range, __pyx_k_nodes_in_range, sizeof(__pyx_k_nodes_in_range), 0, 0, 1, 1},
+    {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
+    {&__pyx_n_s_num_of_pois, __pyx_k_num_of_pois, sizeof(__pyx_k_num_of_pois), 0, 0, 1, 1},
+    {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
+    {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
+    {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
+    {&__pyx_n_s_pandana_cyaccess, __pyx_k_pandana_cyaccess, sizeof(__pyx_k_pandana_cyaccess), 0, 0, 1, 1},
+    {&__pyx_n_s_precompute_range, __pyx_k_precompute_range, sizeof(__pyx_k_precompute_range), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
+    {&__pyx_n_s_radius, __pyx_k_radius, sizeof(__pyx_k_radius), 0, 0, 1, 1},
+    {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
+    {&__pyx_n_s_ret, __pyx_k_ret, sizeof(__pyx_k_ret), 0, 0, 1, 1},
+    {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
+    {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
+    {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+    {&__pyx_n_s_shortest_path, __pyx_k_shortest_path, sizeof(__pyx_k_shortest_path), 0, 0, 1, 1},
+    {&__pyx_n_s_shortest_path_distance, __pyx_k_shortest_path_distance, sizeof(__pyx_k_shortest_path_distance), 0, 0, 1, 1},
+    {&__pyx_n_s_shortest_path_distances, __pyx_k_shortest_path_distances, sizeof(__pyx_k_shortest_path_distances), 0, 0, 1, 1},
+    {&__pyx_n_s_shortest_paths, __pyx_k_shortest_paths, sizeof(__pyx_k_shortest_paths), 0, 0, 1, 1},
+    {&__pyx_n_s_spec, __pyx_k_spec, sizeof(__pyx_k_spec), 0, 0, 1, 1},
+    {&__pyx_kp_s_src_cyaccess_pyx, __pyx_k_src_cyaccess_pyx, sizeof(__pyx_k_src_cyaccess_pyx), 0, 0, 1, 0},
+    {&__pyx_n_s_srcnode, __pyx_k_srcnode, sizeof(__pyx_k_srcnode), 0, 0, 1, 1},
+    {&__pyx_n_s_srcnodes, __pyx_k_srcnodes, sizeof(__pyx_k_srcnodes), 0, 0, 1, 1},
+    {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
+    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+    {&__pyx_n_s_twoway, __pyx_k_twoway, sizeof(__pyx_k_twoway), 0, 0, 1, 1},
+    {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
+    {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
+    {0, 0, 0, 0, 0, 0, 0}
+  };
+  return __Pyx_InitStrings(__pyx_string_tab);
+}
+/* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 35, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 38, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 884, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 68, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 983, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "(tree fragment)":2
- * def __reduce_cython__(self):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
-
-  /* "(tree fragment)":4
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
- * def __setstate_cython__(self, __pyx_state):
- *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
- */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":884
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 884, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(2, 983, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../anaconda/envs/transit/lib/python3.8/site-packages/numpy/__init__.pxd":890
+  /* "../../../../opt/anaconda3/envs/p2/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 890, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(2, 989, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
+
+  /* "src/cyaccess.pyx":88
+ *         del self.access
+ * 
+ *     def initialize_category(             # <<<<<<<<<<<<<<
+ *         self,
+ *         double maxdist,
+ */
+  __pyx_tuple__4 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_maxdist, __pyx_n_s_maxitems, __pyx_n_s_category, __pyx_n_s_node_ids); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 88, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_initialize_category, 88, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 88, __pyx_L1_error)
+
+  /* "src/cyaccess.pyx":105
+ *         self.access.initializeCategory(maxdist, maxitems, category, node_ids)
+ * 
+ *     def find_all_nearest_pois(             # <<<<<<<<<<<<<<
+ *         self,
+ *         double radius,
+ */
+  __pyx_tuple__6 = PyTuple_Pack(6, __pyx_n_s_self, __pyx_n_s_radius, __pyx_n_s_num_of_pois, __pyx_n_s_category, __pyx_n_s_impno, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
+  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_find_all_nearest_pois, 105, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_int_0); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__8);
+  __Pyx_GIVEREF(__pyx_tuple__8);
+
+  /* "src/cyaccess.pyx":125
+ *             convert_2D_vector_to_array_int(ret.second)
+ * 
+ *     def initialize_access_var(             # <<<<<<<<<<<<<<
+ *         self,
+ *         string category,
+ */
+  __pyx_tuple__9 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_category, __pyx_n_s_node_ids, __pyx_n_s_values); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_initialize_access_var, 125, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 125, __pyx_L1_error)
+
+  /* "src/cyaccess.pyx":138
+ *         self.access.initializeAccVar(category, node_ids, values)
+ * 
+ *     def get_available_aggregations(self):             # <<<<<<<<<<<<<<
+ *         return self.access.aggregations
+ * 
+ */
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_get_available_aggregations, 138, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 138, __pyx_L1_error)
+
+  /* "src/cyaccess.pyx":141
+ *         return self.access.aggregations
+ * 
+ *     def get_available_decays(self):             # <<<<<<<<<<<<<<
+ *         return self.access.decays
+ * 
+ */
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_get_available_decays, 141, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 141, __pyx_L1_error)
+
+  /* "src/cyaccess.pyx":144
+ *         return self.access.decays
+ * 
+ *     def get_all_aggregate_accessibility_variables(             # <<<<<<<<<<<<<<
+ *         self,
+ *         double radius,
+ */
+  __pyx_tuple__14 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_radius, __pyx_n_s_category, __pyx_n_s_aggtyp, __pyx_n_s_decay, __pyx_n_s_impno, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(6, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_get_all_aggregate_accessibility, 144, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 144, __pyx_L1_error)
+
+  /* "src/cyaccess.pyx":164
+ *         return convert_vector_to_array_dbl(ret)
+ * 
+ *     def shortest_path(self, int srcnode, int destnode, int impno=0):             # <<<<<<<<<<<<<<
+ *         """
+ *         srcnode - node id origin
+ */
+  __pyx_tuple__16 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_srcnode, __pyx_n_s_destnode, __pyx_n_s_impno); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_shortest_path, 164, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 164, __pyx_L1_error)
+
+  /* "src/cyaccess.pyx":172
+ *         return self.access.Route(srcnode, destnode, impno)
+ * 
+ *     def shortest_paths(self, np.ndarray[long] srcnodes,             # <<<<<<<<<<<<<<
+ *             np.ndarray[long] destnodes, int impno=0):
+ *         """
+ */
+  __pyx_tuple__18 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_srcnodes, __pyx_n_s_destnodes, __pyx_n_s_impno); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_shortest_paths, 172, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 172, __pyx_L1_error)
+
+  /* "src/cyaccess.pyx":181
+ *         return self.access.Routes(srcnodes, destnodes, impno)
+ * 
+ *     def shortest_path_distance(self, int srcnode, int destnode, int impno=0):             # <<<<<<<<<<<<<<
+ *         """
+ *         srcnode - node id origin
+ */
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_shortest_path_distance, 181, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 181, __pyx_L1_error)
+
+  /* "src/cyaccess.pyx":189
+ *         return self.access.Distance(srcnode, destnode, impno)
+ * 
+ *     def shortest_path_distances(self, np.ndarray[long] srcnodes,             # <<<<<<<<<<<<<<
+ *             np.ndarray[long] destnodes, int impno=0):
+ *         """
+ */
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_shortest_path_distances, 189, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 189, __pyx_L1_error)
+
+  /* "src/cyaccess.pyx":198
+ *         return self.access.Distances(srcnodes, destnodes, impno)
+ * 
+ *     def precompute_range(self, double radius):             # <<<<<<<<<<<<<<
+ *         self.access.precomputeRangeQueries(radius)
+ * 
+ */
+  __pyx_tuple__22 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_radius); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_precompute_range, 198, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 198, __pyx_L1_error)
+
+  /* "src/cyaccess.pyx":201
+ *         self.access.precomputeRangeQueries(radius)
+ * 
+ *     def nodes_in_range(self, vector[long] srcnodes, float radius, int impno,             # <<<<<<<<<<<<<<
+ *             np.ndarray[long] ext_ids):
+ *         """
+ */
+  __pyx_tuple__24 = PyTuple_Pack(5, __pyx_n_s_self, __pyx_n_s_srcnodes, __pyx_n_s_radius, __pyx_n_s_impno, __pyx_n_s_ext_ids); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(5, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_cyaccess_pyx, __pyx_n_s_nodes_in_range, 201, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 201, __pyx_L1_error)
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(1, 1, __pyx_L1_error)
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ */
+  __pyx_tuple__27 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(1, 3, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
+/* #### Code section: init_constants ### */
+
+static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
+  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  return 0;
+  __pyx_L1_error:;
+  return -1;
+}
+/* #### Code section: init_globals ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  /* NumpyImportArray.init */
+  /*
+ * Cython has automatically inserted a call to _import_array since
+ * you didn't include one when you cimported numpy. To disable this
+ * add the line
+ *   <void>numpy._import_array
+ */
+#ifdef NPY_FEATURE_VERSION
+#if !NO_IMPORT_ARRAY
+if (unlikely(_import_array() == -1)) {
+    PyErr_SetString(PyExc_ImportError, "numpy.core.multiarray failed to import "
+    "(auto-generated because you didn't call 'numpy.import_array()' after cimporting numpy; "
+    "use '<void>numpy._import_array' to disable if you are certain you don't need it).");
+}
+#endif
+#endif
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   return 0;
   __pyx_L1_error:;
   return -1;
 }
+/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -6432,24 +9958,37 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  if (PyType_Ready(&__pyx_type_7pandana_8cyaccess_cyaccess) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
-  #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_7pandana_8cyaccess_cyaccess.tp_print = 0;
+  #if CYTHON_USE_TYPE_SPECS
+  __pyx_ptype_7pandana_8cyaccess_cyaccess = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7pandana_8cyaccess_cyaccess_spec, NULL); if (unlikely(!__pyx_ptype_7pandana_8cyaccess_cyaccess)) __PYX_ERR(0, 61, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7pandana_8cyaccess_cyaccess_spec, __pyx_ptype_7pandana_8cyaccess_cyaccess) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
+  #else
+  __pyx_ptype_7pandana_8cyaccess_cyaccess = &__pyx_type_7pandana_8cyaccess_cyaccess;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  #endif
+  #if !CYTHON_USE_TYPE_SPECS
+  if (__Pyx_PyType_Ready(__pyx_ptype_7pandana_8cyaccess_cyaccess) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7pandana_8cyaccess_cyaccess.tp_dictoffset && __pyx_type_7pandana_8cyaccess_cyaccess.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_7pandana_8cyaccess_cyaccess.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  #if PY_MAJOR_VERSION < 3
+  __pyx_ptype_7pandana_8cyaccess_cyaccess->tp_print = 0;
+  #endif
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dictoffset && __pyx_ptype_7pandana_8cyaccess_cyaccess->tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_ptype_7pandana_8cyaccess_cyaccess->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_cyaccess, (PyObject *)&__pyx_type_7pandana_8cyaccess_cyaccess) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7pandana_8cyaccess_cyaccess) < 0) __PYX_ERR(0, 58, __pyx_L1_error)
-  __pyx_ptype_7pandana_8cyaccess_cyaccess = &__pyx_type_7pandana_8cyaccess_cyaccess;
+  #endif
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_cyaccess, (PyObject *) __pyx_ptype_7pandana_8cyaccess_cyaccess) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_7pandana_8cyaccess_cyaccess) < 0) __PYX_ERR(0, 61, __pyx_L1_error)
+  #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -6459,35 +9998,41 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_0(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
+  #elif CYTHON_COMPILING_IN_LIMITED_API
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 764, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 809, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 811, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 813, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 815, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 817, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 819, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 821, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 823, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 825, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_0); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 827, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_0(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_0(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_0); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 865, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -6506,14 +10051,63 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec_cyaccess(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_cyaccess},
+  {0, NULL}
+};
+#endif
+
+#ifdef __cplusplus
+namespace {
+  struct PyModuleDef __pyx_moduledef =
+  #else
+  static struct PyModuleDef __pyx_moduledef =
+  #endif
+  {
+      PyModuleDef_HEAD_INIT,
+      "cyaccess",
+      0, /* m_doc */
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      0, /* m_size */
+    #elif CYTHON_USE_MODULE_STATE
+      sizeof(__pyx_mstate), /* m_size */
+    #else
+      -1, /* m_size */
+    #endif
+      __pyx_methods /* m_methods */,
+    #if CYTHON_PEP489_MULTI_PHASE_INIT
+      __pyx_moduledef_slots, /* m_slots */
+    #else
+      NULL, /* m_reload */
+    #endif
+    #if CYTHON_USE_MODULE_STATE
+      __pyx_m_traverse, /* m_traverse */
+      __pyx_m_clear, /* m_clear */
+      NULL /* m_free */
+    #else
+      NULL, /* m_traverse */
+      NULL, /* m_clear */
+      NULL /* m_free */
+    #endif
+  };
+  #ifdef __cplusplus
+} /* anonymous namespace */
+#endif
+#endif
+
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -6556,42 +10150,56 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
+#else
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
+#endif
+{
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
+#if CYTHON_COMPILING_IN_LIMITED_API
+            result = PyModule_AddObject(module, to_name, value);
+#else
             result = PyDict_SetItemString(moddict, to_name, value);
+#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
+    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
+#if CYTHON_COMPILING_IN_LIMITED_API
+    moddict = module;
+#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
+#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
@@ -6599,28 +10207,62 @@
 }
 
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_cyaccess(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
+  int stringtab_initialized = 0;
+  #if CYTHON_USE_MODULE_STATE
+  int pystate_addmodule_run = 0;
+  #endif
   PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'cyaccess' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("cyaccess", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #elif CYTHON_USE_MODULE_STATE
+  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
+  {
+    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to cyaccess pseudovariable */
+    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    pystate_addmodule_run = 1;
+  }
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  #endif
+  CYTHON_UNUSED_VAR(__pyx_t_1);
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
@@ -6631,143 +10273,325 @@
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("cyaccess", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  #endif
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
+  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_pandana__cyaccess) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "pandana.cyaccess")) {
-      if (unlikely(PyDict_SetItemString(modules, "pandana.cyaccess", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+      if (unlikely((PyDict_SetItemString(modules, "pandana.cyaccess", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
-  if (unlikely(__Pyx_modinit_type_import_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_init_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "src/cyaccess.pyx":7
+  /* "src/cyaccess.pyx":9
  * from libcpp.pair cimport pair
  * 
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 7, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_ImportDottedModule(__pyx_n_s_numpy, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_2) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "src/cyaccess.pyx":1
- * cimport cython             # <<<<<<<<<<<<<<
- * from libcpp cimport bool
- * from libcpp.vector cimport vector
+  /* "src/cyaccess.pyx":88
+ *         del self.access
+ * 
+ *     def initialize_category(             # <<<<<<<<<<<<<<
+ *         self,
+ *         double maxdist,
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_5initialize_category, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_initialize_category, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_initialize_category, __pyx_t_2) < 0) __PYX_ERR(0, 88, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
 
-  /* "vector.to_py":60
+  /* "src/cyaccess.pyx":105
+ *         self.access.initializeCategory(maxdist, maxitems, category, node_ids)
  * 
- * @cname("__pyx_convert_vector_to_py_std_3a__3a_string")
- * cdef object __pyx_convert_vector_to_py_std_3a__3a_string(vector[X]& v):             # <<<<<<<<<<<<<<
- *     return [v[i] for i in range(v.size())]
+ *     def find_all_nearest_pois(             # <<<<<<<<<<<<<<
+ *         self,
+ *         double radius,
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_7find_all_nearest_pois, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_find_all_nearest_pois, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__8);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_find_all_nearest_pois, __pyx_t_2) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "src/cyaccess.pyx":125
+ *             convert_2D_vector_to_array_int(ret.second)
+ * 
+ *     def initialize_access_var(             # <<<<<<<<<<<<<<
+ *         self,
+ *         string category,
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_9initialize_access_var, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_initialize_access_var, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_initialize_access_var, __pyx_t_2) < 0) __PYX_ERR(0, 125, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "src/cyaccess.pyx":138
+ *         self.access.initializeAccVar(category, node_ids, values)
+ * 
+ *     def get_available_aggregations(self):             # <<<<<<<<<<<<<<
+ *         return self.access.aggregations
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_11get_available_aggregations, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_get_available_aggregati, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_get_available_aggregations, __pyx_t_2) < 0) __PYX_ERR(0, 138, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "src/cyaccess.pyx":141
+ *         return self.access.aggregations
+ * 
+ *     def get_available_decays(self):             # <<<<<<<<<<<<<<
+ *         return self.access.decays
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_13get_available_decays, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_get_available_decays, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_get_available_decays, __pyx_t_2) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "src/cyaccess.pyx":144
+ *         return self.access.decays
+ * 
+ *     def get_all_aggregate_accessibility_variables(             # <<<<<<<<<<<<<<
+ *         self,
+ *         double radius,
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_15get_all_aggregate_accessibility_variables, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_get_all_aggregate_acces, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__8);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_get_all_aggregate_accessibility, __pyx_t_2) < 0) __PYX_ERR(0, 144, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "src/cyaccess.pyx":164
+ *         return convert_vector_to_array_dbl(ret)
+ * 
+ *     def shortest_path(self, int srcnode, int destnode, int impno=0):             # <<<<<<<<<<<<<<
+ *         """
+ *         srcnode - node id origin
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_17shortest_path, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_shortest_path, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__8);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_shortest_path, __pyx_t_2) < 0) __PYX_ERR(0, 164, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "src/cyaccess.pyx":172
+ *         return self.access.Route(srcnode, destnode, impno)
+ * 
+ *     def shortest_paths(self, np.ndarray[long] srcnodes,             # <<<<<<<<<<<<<<
+ *             np.ndarray[long] destnodes, int impno=0):
+ *         """
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_19shortest_paths, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_shortest_paths, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__8);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_shortest_paths, __pyx_t_2) < 0) __PYX_ERR(0, 172, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "src/cyaccess.pyx":181
+ *         return self.access.Routes(srcnodes, destnodes, impno)
+ * 
+ *     def shortest_path_distance(self, int srcnode, int destnode, int impno=0):             # <<<<<<<<<<<<<<
+ *         """
+ *         srcnode - node id origin
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_21shortest_path_distance, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_shortest_path_distance, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__8);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_shortest_path_distance, __pyx_t_2) < 0) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "src/cyaccess.pyx":189
+ *         return self.access.Distance(srcnode, destnode, impno)
+ * 
+ *     def shortest_path_distances(self, np.ndarray[long] srcnodes,             # <<<<<<<<<<<<<<
+ *             np.ndarray[long] destnodes, int impno=0):
+ *         """
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_23shortest_path_distances, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_shortest_path_distances, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_tuple__8);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_shortest_path_distances, __pyx_t_2) < 0) __PYX_ERR(0, 189, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "src/cyaccess.pyx":198
+ *         return self.access.Distances(srcnodes, destnodes, impno)
+ * 
+ *     def precompute_range(self, double radius):             # <<<<<<<<<<<<<<
+ *         self.access.precomputeRangeQueries(radius)
+ * 
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_25precompute_range, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_precompute_range, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_precompute_range, __pyx_t_2) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "src/cyaccess.pyx":201
+ *         self.access.precomputeRangeQueries(radius)
+ * 
+ *     def nodes_in_range(self, vector[long] srcnodes, float radius, int impno,             # <<<<<<<<<<<<<<
+ *             np.ndarray[long] ext_ids):
+ *         """
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_27nodes_in_range, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess_nodes_in_range, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_7pandana_8cyaccess_cyaccess->tp_dict, __pyx_n_s_nodes_in_range, __pyx_t_2) < 0) __PYX_ERR(0, 201, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  PyType_Modified(__pyx_ptype_7pandana_8cyaccess_cyaccess);
+
+  /* "(tree fragment)":1
+ * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_29__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess___reduce_cython, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "(tree fragment)":3
+ * def __reduce_cython__(self):
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
+ *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
+ */
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_7pandana_8cyaccess_8cyaccess_31__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_cyaccess___setstate_cython, NULL, __pyx_n_s_pandana_cyaccess, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 3, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "src/cyaccess.pyx":1
+ * #cython: language_level=3             # <<<<<<<<<<<<<<
  * 
+ * cimport cython
  */
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   if (__pyx_m) {
-    if (__pyx_d) {
+    if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init pandana.cyaccess", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
+    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
+    #else
+    Py_DECREF(__pyx_m);
+    if (pystate_addmodule_run) {
+      PyObject *tp, *value, *tb;
+      PyErr_Fetch(&tp, &value, &tb);
+      PyState_RemoveModule(&__pyx_moduledef);
+      PyErr_Restore(tp, value, tb);
+    }
+    #endif
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init pandana.cyaccess");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
+/* #### Code section: cleanup_globals ### */
+/* #### Code section: cleanup_module ### */
+/* #### Code section: main_method ### */
+/* #### Code section: utility_code_pragmas ### */
+#ifdef _MSC_VER
+#pragma warning( push )
+/* Warning 4127: conditional expression is constant
+ * Cython uses constant conditional expressions to allow in inline functions to be optimized at
+ * compile-time, so this warning is not useful
+ */
+#pragma warning( disable : 4127 )
+#endif
+
+
+
+/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -6779,42 +10603,522 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    int result;
+    PyObject *exc_type;
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *current_exception = tstate->current_exception;
+    if (unlikely(!current_exception)) return 0;
+    exc_type = (PyObject*) Py_TYPE(current_exception);
+    if (exc_type == err) return 1;
+#else
+    exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+#endif
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_INCREF(exc_type);
+    #endif
+    if (unlikely(PyTuple_Check(err))) {
+        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    } else {
+        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+    }
+    #if CYTHON_AVOID_BORROWED_REFS
+    Py_DECREF(exc_type);
+    #endif
+    return result;
+}
+#endif
+
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject *tmp_value;
+    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
+    if (value) {
+        #if CYTHON_COMPILING_IN_CPYTHON
+        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
+        #endif
+            PyException_SetTraceback(value, tb);
+    }
+    tmp_value = tstate->current_exception;
+    tstate->current_exception = value;
+    Py_XDECREF(tmp_value);
+#else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#endif
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+#if PY_VERSION_HEX >= 0x030C00A6
+    PyObject* exc_value;
+    exc_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    *value = exc_value;
+    *type = NULL;
+    *tb = NULL;
+    if (exc_value) {
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        #if CYTHON_COMPILING_IN_CPYTHON
+        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
+        Py_XINCREF(*tb);
+        #else
+        *tb = PyException_GetTraceback(exc_value);
+        #endif
+    }
+#else
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#endif
+}
+#endif
+
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro))
         return tp->tp_getattro(obj, attr_name);
 #if PY_MAJOR_VERSION < 3
     if (likely(tp->tp_getattr))
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
+}
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
+    }
+#endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
+
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
-    if (unlikely(!result)) {
+    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
+    if (unlikely(!result) && !PyErr_Occurred()) {
         PyErr_Format(PyExc_NameError,
 #if PY_MAJOR_VERSION >= 3
             "name '%U' is not defined", name);
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK && CYTHON_FAST_THREAD_STATE
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_value == NULL || exc_info->exc_value == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    PyObject *exc_value = exc_info->exc_value;
+    if (exc_value == NULL || exc_value == Py_None) {
+        *value = NULL;
+        *type = NULL;
+        *tb = NULL;
+    } else {
+        *value = exc_value;
+        Py_INCREF(*value);
+        *type = (PyObject*) Py_TYPE(exc_value);
+        Py_INCREF(*type);
+        *tb = PyException_GetTraceback(exc_value);
+    }
+  #elif CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+  #endif
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+  #if CYTHON_USE_EXC_INFO_STACK && PY_VERSION_HEX >= 0x030B00a4
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    PyObject *tmp_value = exc_info->exc_value;
+    exc_info->exc_value = value;
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+  #else
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+  #endif
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type = NULL, *local_value, *local_tb = NULL;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+  #if PY_VERSION_HEX >= 0x030C00A6
+    local_value = tstate->current_exception;
+    tstate->current_exception = 0;
+    if (likely(local_value)) {
+        local_type = (PyObject*) Py_TYPE(local_value);
+        Py_INCREF(local_type);
+        local_tb = PyException_GetTraceback(local_value);
+    }
+  #else
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+  #endif
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE && PY_VERSION_HEX >= 0x030C00A6
+    if (unlikely(tstate->current_exception))
+#elif CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+      #if PY_VERSION_HEX >= 0x030B00a4
+        tmp_value = exc_info->exc_value;
+        exc_info->exc_value = local_value;
+        tmp_type = NULL;
+        tmp_tb = NULL;
+        Py_XDECREF(local_type);
+        Py_XDECREF(local_tb);
+      #else
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+      #endif
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    CYTHON_UNUSED_VAR(cause);
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+      #if PY_VERSION_HEX >= 0x030C00A6
+        PyException_SetTraceback(value, tb);
+      #elif CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
 }
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_object_dict_version(PyObject *obj) {
@@ -6850,14 +11154,22 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
+#elif CYTHON_COMPILING_IN_LIMITED_API
+    if (unlikely(!__pyx_m)) {
+        return NULL;
+    }
+    result = PyObject_GetAttr(__pyx_m, name);
+    if (likely(result)) {
+        return result;
+    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -6868,51 +11180,38 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* PyObjectCall */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
-    if (unlikely(!call))
-        return PyObject_Call(func, arg, kw);
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
-        return NULL;
-    result = (*call)(func, arg, kw);
-    Py_LeaveRecursiveCall();
-    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
-        PyErr_SetString(
-            PyExc_SystemError,
-            "NULL result without error in PyObject_Call");
-    }
-    return result;
-}
-#endif
-
 /* ExtTypeTest */
 static CYTHON_INLINE int __Pyx_TypeTest(PyObject *obj, PyTypeObject *type) {
+    __Pyx_TypeName obj_type_name;
+    __Pyx_TypeName type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     if (likely(__Pyx_TypeCheck(obj, type)))
         return 1;
-    PyErr_Format(PyExc_TypeError, "Cannot convert %.200s to %.200s",
-                 Py_TYPE(obj)->tp_name, type->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    type_name = __Pyx_PyType_GetName(type);
+    PyErr_Format(PyExc_TypeError,
+                 "Cannot convert " __Pyx_FMT_TYPENAME " to " __Pyx_FMT_TYPENAME,
+                 obj_type_name, type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
     return 0;
 }
 
 /* SetItemInt */
 static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v) {
     int r;
-    if (!j) return -1;
+    if (unlikely(!j)) return -1;
     r = PyObject_SetItem(o, j, v);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v, int is_list,
                                                CYTHON_NCP_UNUSED int wraparound, CYTHON_NCP_UNUSED int boundscheck) {
 #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
@@ -6922,27 +11221,36 @@
             PyObject* old = PyList_GET_ITEM(o, n);
             Py_INCREF(v);
             PyList_SET_ITEM(o, n, v);
             Py_DECREF(old);
             return 1;
         }
     } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_ass_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
+        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
+        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
+        if (mm && mm->mp_ass_subscript) {
+            int r;
+            PyObject *key = PyInt_FromSsize_t(i);
+            if (unlikely(!key)) return -1;
+            r = mm->mp_ass_subscript(o, key, v);
+            Py_DECREF(key);
+            return r;
+        }
+        if (likely(sm && sm->sq_ass_item)) {
+            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
+                Py_ssize_t l = sm->sq_length(o);
                 if (likely(l >= 0)) {
                     i += l;
                 } else {
                     if (!PyErr_ExceptionMatches(PyExc_OverflowError))
                         return -1;
                     PyErr_Clear();
                 }
             }
-            return m->sq_ass_item(o, i, v);
+            return sm->sq_ass_item(o, i, v);
         }
     }
 #else
 #if CYTHON_COMPILING_IN_PYPY
     if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
 #else
     if (is_list || PySequence_Check(o))
@@ -6953,15 +11261,15 @@
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
-    if (!j) return NULL;
+    if (unlikely(!j)) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
                                                               CYTHON_NCP_UNUSED int wraparound,
                                                               CYTHON_NCP_UNUSED int boundscheck) {
@@ -7014,37 +11322,252 @@
         Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
         if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
             PyObject *r = PyTuple_GET_ITEM(o, n);
             Py_INCREF(r);
             return r;
         }
     } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
+        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
+        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
+        if (mm && mm->mp_subscript) {
+            PyObject *r, *key = PyInt_FromSsize_t(i);
+            if (unlikely(!key)) return NULL;
+            r = mm->mp_subscript(o, key);
+            Py_DECREF(key);
+            return r;
+        }
+        if (likely(sm && sm->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
+                Py_ssize_t l = sm->sq_length(o);
                 if (likely(l >= 0)) {
                     i += l;
                 } else {
                     if (!PyErr_ExceptionMatches(PyExc_OverflowError))
                         return NULL;
                     PyErr_Clear();
                 }
             }
-            return m->sq_item(o, i);
+            return sm->sq_item(o, i);
         }
     }
 #else
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
+/* TupleAndListFromArray */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
+    PyObject *v;
+    Py_ssize_t i;
+    for (i = 0; i < length; i++) {
+        v = dest[i] = src[i];
+        Py_INCREF(v);
+    }
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        Py_INCREF(__pyx_empty_tuple);
+        return __pyx_empty_tuple;
+    }
+    res = PyTuple_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
+    return res;
+}
+static CYTHON_INLINE PyObject *
+__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
+{
+    PyObject *res;
+    if (n <= 0) {
+        return PyList_New(0);
+    }
+    res = PyList_New(n);
+    if (unlikely(res == NULL)) return NULL;
+    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
+    return res;
+}
+#endif
+
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
+/* fastcall */
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
+{
+    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
+    for (i = 0; i < n; i++)
+    {
+        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
+    }
+    for (i = 0; i < n; i++)
+    {
+        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
+        if (unlikely(eq != 0)) {
+            if (unlikely(eq < 0)) return NULL;  // error
+            return kwvalues[i];
+        }
+    }
+    return NULL;  // not found (no exception set)
+}
+#endif
+
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -7080,25 +11603,37 @@
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
 static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
+    PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
-    while (PyDict_Next(kwds, &pos, &key, &value)) {
+    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
+    while (1) {
+        if (kwds_is_tuple) {
+            if (pos >= PyTuple_GET_SIZE(kwds)) break;
+            key = PyTuple_GET_ITEM(kwds, pos);
+            value = kwvalues[pos];
+            pos++;
+        }
+        else
+        {
+            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
+        }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
@@ -7124,19 +11659,20 @@
                     argname++;
                 }
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
-                int cmp = (**name == key) ? 0 :
+                int cmp = (
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
-                    PyUnicode_Compare(**name, key);
+                    PyUnicode_Compare(**name, key)
+                );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
             }
@@ -7167,44 +11703,51 @@
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     goto bad;
 invalid_keyword:
-    PyErr_Format(PyExc_TypeError,
     #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
+    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
 /* ArgTypeTest */
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
 {
+    __Pyx_TypeName type_name;
+    __Pyx_TypeName obj_type_name;
     if (unlikely(!type)) {
         PyErr_SetString(PyExc_SystemError, "Missing type object");
         return 0;
     }
     else if (exact) {
         #if PY_MAJOR_VERSION == 2
         if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
         #endif
     }
     else {
         if (likely(__Pyx_TypeCheck(obj, type))) return 1;
     }
+    type_name = __Pyx_PyType_GetName(type);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
     PyErr_Format(PyExc_TypeError,
-        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
-        name, type->tp_name, Py_TYPE(obj)->tp_name);
+        "Argument '%.200s' has incorrect type (expected " __Pyx_FMT_TYPENAME
+        ", got " __Pyx_FMT_TYPENAME ")", name, type_name, obj_type_name);
+    __Pyx_DECREF_TypeName(type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return 0;
 }
 
 /* IsLittleEndian */
 static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
 {
   union {
@@ -7287,15 +11830,15 @@
     case 'd': return (is_complex ? "'complex double'" : "'double'");
     case 'g': return (is_complex ? "'complex long double'" : "'long double'");
     case 'T': return "a struct";
     case 'O': return "Python object";
     case 'P': return "a pointer";
     case 's': case 'p': return "a string";
     case 0: return "end";
-    default: return "unparseable format string";
+    default: return "unparsable format string";
   }
 }
 static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return 2;
     case 'i': case 'I': case 'l': case 'L': return 4;
@@ -7337,15 +11880,16 @@
 typedef struct { char c; float x; } __Pyx_st_float;
 typedef struct { char c; double x; } __Pyx_st_double;
 typedef struct { char c; long double x; } __Pyx_st_longdouble;
 typedef struct { char c; void *x; } __Pyx_st_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
@@ -7369,15 +11913,16 @@
 typedef struct { float x; char c; } __Pyx_pad_float;
 typedef struct { double x; char c; } __Pyx_pad_double;
 typedef struct { long double x; char c; } __Pyx_pad_longdouble;
 typedef struct { void *x; char c; } __Pyx_pad_void_p;
 #ifdef HAVE_LONG_LONG
 typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
 #endif
-static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
+static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, int is_complex) {
+  CYTHON_UNUSED_VAR(is_complex);
   switch (ch) {
     case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
     case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
     case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
     case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
 #ifdef HAVE_LONG_LONG
     case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
@@ -7760,363 +12305,624 @@
   if (buf->suboffsets == NULL) buf->suboffsets = __Pyx_minusones;
   return 0;
 fail:;
   __Pyx_SafeReleaseBuffer(buf);
   return -1;
 }
 
-/* PyErrFetchRestore */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
-/* RaiseException */
-  #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
-                        CYTHON_UNUSED PyObject *cause) {
-    __Pyx_PyThreadState_declare
-    Py_XINCREF(type);
-    if (!value || value == Py_None)
-        value = NULL;
-    else
-        Py_INCREF(value);
-    if (!tb || tb == Py_None)
-        tb = NULL;
-    else {
-        Py_INCREF(tb);
-        if (!PyTraceBack_Check(tb)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: arg 3 must be a traceback or None");
-            goto raise_error;
-        }
-    }
-    if (PyType_Check(type)) {
+/* KeywordStringCheck */
+  static int __Pyx_CheckKeywordStrings(
+    PyObject *kw,
+    const char* function_name,
+    int kw_allowed)
+{
+    PyObject* key = 0;
+    Py_ssize_t pos = 0;
 #if CYTHON_COMPILING_IN_PYPY
-        if (!value) {
-            Py_INCREF(Py_None);
-            value = Py_None;
-        }
-#endif
-        PyErr_NormalizeException(&type, &value, &tb);
-    } else {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto raise_error;
+    if (!kw_allowed && PyDict_Next(kw, &pos, &key, 0))
+        goto invalid_keyword;
+    return 1;
+#else
+    if (CYTHON_METH_FASTCALL && likely(PyTuple_Check(kw))) {
+        if (unlikely(PyTuple_GET_SIZE(kw) == 0))
+            return 1;
+        if (!kw_allowed) {
+            key = PyTuple_GET_ITEM(kw, 0);
+            goto invalid_keyword;
         }
-        value = type;
-        type = (PyObject*) Py_TYPE(type);
-        Py_INCREF(type);
-        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
-            PyErr_SetString(PyExc_TypeError,
-                "raise: exception class must be a subclass of BaseException");
-            goto raise_error;
+#if PY_VERSION_HEX < 0x03090000
+        for (pos = 0; pos < PyTuple_GET_SIZE(kw); pos++) {
+            key = PyTuple_GET_ITEM(kw, pos);
+            if (unlikely(!PyUnicode_Check(key)))
+                goto invalid_keyword_type;
         }
+#endif
+        return 1;
     }
-    __Pyx_PyThreadState_assign
-    __Pyx_ErrRestore(type, value, tb);
-    return;
-raise_error:
-    Py_XDECREF(value);
-    Py_XDECREF(type);
-    Py_XDECREF(tb);
-    return;
+    while (PyDict_Next(kw, &pos, &key, 0)) {
+        #if PY_MAJOR_VERSION < 3
+        if (unlikely(!PyString_Check(key)))
+        #endif
+            if (unlikely(!PyUnicode_Check(key)))
+                goto invalid_keyword_type;
+    }
+    if (!kw_allowed && unlikely(key))
+        goto invalid_keyword;
+    return 1;
+invalid_keyword_type:
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() keywords must be strings", function_name);
+    return 0;
+#endif
+invalid_keyword:
+    #if PY_MAJOR_VERSION < 3
+    PyErr_Format(PyExc_TypeError,
+        "%.200s() got an unexpected keyword argument '%.200s'",
+        function_name, PyString_AsString(key));
+    #else
+    PyErr_Format(PyExc_TypeError,
+        "%s() got an unexpected keyword argument '%U'",
+        function_name, key);
+    #endif
+    return 0;
 }
+
+/* FixUpExtensionType */
+  #if CYTHON_USE_TYPE_SPECS
+static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
+#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
+    CYTHON_UNUSED_VAR(spec);
+    CYTHON_UNUSED_VAR(type);
+#else
+    const PyType_Slot *slot = spec->slots;
+    while (slot && slot->slot && slot->slot != Py_tp_members)
+        slot++;
+    if (slot && slot->slot == Py_tp_members) {
+        int changed = 0;
+#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
+        const
+#endif
+            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
+        while (memb && memb->name) {
+            if (memb->name[0] == '_' && memb->name[1] == '_') {
+#if PY_VERSION_HEX < 0x030900b1
+                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_weaklistoffset = memb->offset;
+                    changed = 1;
+                }
+                else if (strcmp(memb->name, "__dictoffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+                    type->tp_dictoffset = memb->offset;
+                    changed = 1;
+                }
+#if CYTHON_METH_FASTCALL
+                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
+                    assert(memb->type == T_PYSSIZET);
+                    assert(memb->flags == READONLY);
+#if PY_VERSION_HEX >= 0x030800b4
+                    type->tp_vectorcall_offset = memb->offset;
 #else
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
-    PyObject* owned_instance = NULL;
-    if (tb == Py_None) {
-        tb = 0;
-    } else if (tb && !PyTraceBack_Check(tb)) {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: arg 3 must be a traceback or None");
-        goto bad;
-    }
-    if (value == Py_None)
-        value = 0;
-    if (PyExceptionInstance_Check(type)) {
-        if (value) {
-            PyErr_SetString(PyExc_TypeError,
-                "instance exception may not have a separate value");
-            goto bad;
-        }
-        value = type;
-        type = (PyObject*) Py_TYPE(value);
-    } else if (PyExceptionClass_Check(type)) {
-        PyObject *instance_class = NULL;
-        if (value && PyExceptionInstance_Check(value)) {
-            instance_class = (PyObject*) Py_TYPE(value);
-            if (instance_class != type) {
-                int is_subclass = PyObject_IsSubclass(instance_class, type);
-                if (!is_subclass) {
-                    instance_class = NULL;
-                } else if (unlikely(is_subclass == -1)) {
-                    goto bad;
-                } else {
-                    type = instance_class;
+                    type->tp_print = (printfunc) memb->offset;
+#endif
+                    changed = 1;
                 }
+#endif
+#else
+                if ((0));
+#endif
+#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
+                else if (strcmp(memb->name, "__module__") == 0) {
+                    PyObject *descr;
+                    assert(memb->type == T_OBJECT);
+                    assert(memb->flags == 0 || memb->flags == READONLY);
+                    descr = PyDescr_NewMember(type, memb);
+                    if (unlikely(!descr))
+                        return -1;
+                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
+                        Py_DECREF(descr);
+                        return -1;
+                    }
+                    Py_DECREF(descr);
+                    changed = 1;
+                }
+#endif
             }
+            memb++;
         }
-        if (!instance_class) {
-            PyObject *args;
-            if (!value)
-                args = PyTuple_New(0);
-            else if (PyTuple_Check(value)) {
-                Py_INCREF(value);
-                args = value;
-            } else
-                args = PyTuple_Pack(1, value);
-            if (!args)
-                goto bad;
-            owned_instance = PyObject_Call(type, args, NULL);
-            Py_DECREF(args);
-            if (!owned_instance)
-                goto bad;
-            value = owned_instance;
-            if (!PyExceptionInstance_Check(value)) {
-                PyErr_Format(PyExc_TypeError,
-                             "calling %R should have returned an instance of "
-                             "BaseException, not %R",
-                             type, Py_TYPE(value));
-                goto bad;
-            }
-        }
-    } else {
-        PyErr_SetString(PyExc_TypeError,
-            "raise: exception class must be a subclass of BaseException");
-        goto bad;
+        if (changed)
+            PyType_Modified(type);
     }
-    if (cause) {
-        PyObject *fixed_cause;
-        if (cause == Py_None) {
-            fixed_cause = NULL;
-        } else if (PyExceptionClass_Check(cause)) {
-            fixed_cause = PyObject_CallObject(cause, NULL);
-            if (fixed_cause == NULL)
-                goto bad;
-        } else if (PyExceptionInstance_Check(cause)) {
-            fixed_cause = cause;
-            Py_INCREF(fixed_cause);
-        } else {
-            PyErr_SetString(PyExc_TypeError,
-                            "exception causes must derive from "
-                            "BaseException");
-            goto bad;
-        }
-        PyException_SetCause(value, fixed_cause);
+#endif
+    return 0;
+}
+#endif
+
+/* PyFunctionFastCall */
+  #if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
+static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
+                                               PyObject *globals) {
+    PyFrameObject *f;
+    PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject **fastlocals;
+    Py_ssize_t i;
+    PyObject *result;
+    assert(globals != NULL);
+    /* XXX Perhaps we should create a specialized
+       PyFrame_New() that doesn't take locals, but does
+       take builtins without sanity checking them.
+       */
+    assert(tstate != NULL);
+    f = PyFrame_New(tstate, co, globals, NULL);
+    if (f == NULL) {
+        return NULL;
     }
-    PyErr_SetObject(type, value);
-    if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
-        PyThreadState *tstate = __Pyx_PyThreadState_Current;
-        PyObject* tmp_tb = tstate->curexc_traceback;
-        if (tb != tmp_tb) {
-            Py_INCREF(tb);
-            tstate->curexc_traceback = tb;
-            Py_XDECREF(tmp_tb);
+    fastlocals = __Pyx_PyFrame_GetLocalsplus(f);
+    for (i = 0; i < na; i++) {
+        Py_INCREF(*args);
+        fastlocals[i] = *args++;
+    }
+    result = PyEval_EvalFrameEx(f,0);
+    ++tstate->recursion_depth;
+    Py_DECREF(f);
+    --tstate->recursion_depth;
+    return result;
+}
+static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
+    PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
+    PyObject *globals = PyFunction_GET_GLOBALS(func);
+    PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
+    PyObject *closure;
+#if PY_MAJOR_VERSION >= 3
+    PyObject *kwdefs;
+#endif
+    PyObject *kwtuple, **k;
+    PyObject **d;
+    Py_ssize_t nd;
+    Py_ssize_t nk;
+    PyObject *result;
+    assert(kwargs == NULL || PyDict_Check(kwargs));
+    nk = kwargs ? PyDict_Size(kwargs) : 0;
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
+        return NULL;
+    }
+    if (
+#if PY_MAJOR_VERSION >= 3
+            co->co_kwonlyargcount == 0 &&
+#endif
+            likely(kwargs == NULL || nk == 0) &&
+            co->co_flags == (CO_OPTIMIZED | CO_NEWLOCALS | CO_NOFREE)) {
+        if (argdefs == NULL && co->co_argcount == nargs) {
+            result = __Pyx_PyFunction_FastCallNoKw(co, args, nargs, globals);
+            goto done;
+        }
+        else if (nargs == 0 && argdefs != NULL
+                 && co->co_argcount == Py_SIZE(argdefs)) {
+            /* function called with no arguments, but all parameters have
+               a default value: use default values as arguments .*/
+            args = &PyTuple_GET_ITEM(argdefs, 0);
+            result =__Pyx_PyFunction_FastCallNoKw(co, args, Py_SIZE(argdefs), globals);
+            goto done;
+        }
+    }
+    if (kwargs != NULL) {
+        Py_ssize_t pos, i;
+        kwtuple = PyTuple_New(2 * nk);
+        if (kwtuple == NULL) {
+            result = NULL;
+            goto done;
+        }
+        k = &PyTuple_GET_ITEM(kwtuple, 0);
+        pos = i = 0;
+        while (PyDict_Next(kwargs, &pos, &k[i], &k[i+1])) {
+            Py_INCREF(k[i]);
+            Py_INCREF(k[i+1]);
+            i += 2;
         }
+        nk = i / 2;
+    }
+    else {
+        kwtuple = NULL;
+        k = NULL;
+    }
+    closure = PyFunction_GET_CLOSURE(func);
+#if PY_MAJOR_VERSION >= 3
+    kwdefs = PyFunction_GET_KW_DEFAULTS(func);
 #endif
+    if (argdefs != NULL) {
+        d = &PyTuple_GET_ITEM(argdefs, 0);
+        nd = Py_SIZE(argdefs);
     }
-bad:
-    Py_XDECREF(owned_instance);
-    return;
+    else {
+        d = NULL;
+        nd = 0;
+    }
+#if PY_MAJOR_VERSION >= 3
+    result = PyEval_EvalCodeEx((PyObject*)co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, kwdefs, closure);
+#else
+    result = PyEval_EvalCodeEx(co, globals, (PyObject *)NULL,
+                               args, (int)nargs,
+                               k, (int)nk,
+                               d, (int)nd, closure);
+#endif
+    Py_XDECREF(kwtuple);
+done:
+    Py_LeaveRecursiveCall();
+    return result;
 }
 #endif
 
-/* GetTopmostException */
-  #if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
+/* PyObjectCallMethO */
+  #if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg) {
+    PyObject *self, *result;
+    PyCFunction cfunc;
+    cfunc = PyCFunction_GET_FUNCTION(func);
+    self = PyCFunction_GET_SELF(func);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = cfunc(self, arg);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
     }
-    return exc_info;
+    return result;
 }
 #endif
 
-/* SaveResetException */
-  #if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+/* PyObjectFastCall */
+  static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
+    PyObject *argstuple;
+    PyObject *result;
+    size_t i;
+    argstuple = PyTuple_New((Py_ssize_t)nargs);
+    if (unlikely(!argstuple)) return NULL;
+    for (i = 0; i < nargs; i++) {
+        Py_INCREF(args[i]);
+        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
+    }
+    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
+    Py_DECREF(argstuple);
+    return result;
 }
+static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
+    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
+#if CYTHON_COMPILING_IN_CPYTHON
+    if (nargs == 0 && kwargs == NULL) {
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
+        if (__Pyx_IsCyOrPyCFunction(func))
+#else
+        if (PyCFunction_Check(func))
 #endif
-
-/* PyErrExceptionMatches */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
+                return __Pyx_PyObject_CallMethO(func, NULL);
+            }
+        }
+    }
+    else if (nargs == 1 && kwargs == NULL) {
+        if (PyCFunction_Check(func))
+        {
+            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+                return __Pyx_PyObject_CallMethO(func, args[0]);
+            }
+        }
     }
 #endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    #if PY_VERSION_HEX < 0x030800B1
+    #if CYTHON_FAST_PYCCALL
+    if (PyCFunction_Check(func)) {
+        if (kwargs) {
+            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
+        } else {
+            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
+        }
     }
-    return 0;
+    #if PY_VERSION_HEX >= 0x030700A1
+    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
+        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
+    }
+    #endif
+    #endif
+    #if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    }
+    #endif
+    #endif
+    #if CYTHON_VECTORCALL
+    vectorcallfunc f = _PyVectorcall_Function(func);
+    if (f) {
+        return f(func, args, (size_t)nargs, kwargs);
+    }
+    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
+    if (__Pyx_CyFunction_CheckExact(func)) {
+        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
+        if (f) return f(func, args, (size_t)nargs, kwargs);
+    }
+    #endif
+    if (nargs == 0) {
+        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
+    }
+    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
 }
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+
+/* PyObjectCallNoArg */
+  static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
+    PyObject *arg = NULL;
+    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
-#endif
 
-/* GetException */
-  #if CYTHON_FAST_THREAD_STATE
-static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+/* PyObjectCallOneArg */
+  static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *args[2] = {NULL, arg};
+    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+}
+
+/* PyObjectGetMethod */
+  static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
+    PyObject *attr;
+#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
+    __Pyx_TypeName type_name;
+    PyTypeObject *tp = Py_TYPE(obj);
+    PyObject *descr;
+    descrgetfunc f = NULL;
+    PyObject **dictptr, *dict;
+    int meth_found = 0;
+    assert (*method == NULL);
+    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
+        attr = __Pyx_PyObject_GetAttrStr(obj, name);
+        goto try_unpack;
+    }
+    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
+        return 0;
+    }
+    descr = _PyType_Lookup(tp, name);
+    if (likely(descr != NULL)) {
+        Py_INCREF(descr);
+#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
+        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
+#elif PY_MAJOR_VERSION >= 3
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
+        #endif
 #else
-static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+        #ifdef __Pyx_CyFunction_USED
+        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
+        #else
+        if (likely(PyFunction_Check(descr)))
+        #endif
 #endif
-{
-    PyObject *local_type, *local_value, *local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    local_type = tstate->curexc_type;
-    local_value = tstate->curexc_value;
-    local_tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
+        {
+            meth_found = 1;
+        } else {
+            f = Py_TYPE(descr)->tp_descr_get;
+            if (f != NULL && PyDescr_IsData(descr)) {
+                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+                Py_DECREF(descr);
+                goto try_unpack;
+            }
+        }
+    }
+    dictptr = _PyObject_GetDictPtr(obj);
+    if (dictptr != NULL && (dict = *dictptr) != NULL) {
+        Py_INCREF(dict);
+        attr = __Pyx_PyDict_GetItemStr(dict, name);
+        if (attr != NULL) {
+            Py_INCREF(attr);
+            Py_DECREF(dict);
+            Py_XDECREF(descr);
+            goto try_unpack;
+        }
+        Py_DECREF(dict);
+    }
+    if (meth_found) {
+        *method = descr;
+        return 1;
+    }
+    if (f != NULL) {
+        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
+        Py_DECREF(descr);
+        goto try_unpack;
+    }
+    if (likely(descr != NULL)) {
+        *method = descr;
+        return 0;
+    }
+    type_name = __Pyx_PyType_GetName(tp);
+    PyErr_Format(PyExc_AttributeError,
+#if PY_MAJOR_VERSION >= 3
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, name);
 #else
-    PyErr_Fetch(&local_type, &local_value, &local_tb);
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(name));
 #endif
-    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
-#if CYTHON_FAST_THREAD_STATE
-    if (unlikely(tstate->curexc_type))
+    __Pyx_DECREF_TypeName(type_name);
+    return 0;
 #else
-    if (unlikely(PyErr_Occurred()))
+    attr = __Pyx_PyObject_GetAttrStr(obj, name);
+    goto try_unpack;
 #endif
-        goto bad;
-    #if PY_MAJOR_VERSION >= 3
-    if (local_tb) {
-        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
-            goto bad;
+try_unpack:
+#if CYTHON_UNPACK_METHODS
+    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
+        PyObject *function = PyMethod_GET_FUNCTION(attr);
+        Py_INCREF(function);
+        Py_DECREF(attr);
+        *method = function;
+        return 1;
     }
-    #endif
-    Py_XINCREF(local_tb);
-    Py_XINCREF(local_type);
-    Py_XINCREF(local_value);
-    *type = local_type;
-    *value = local_value;
-    *tb = local_tb;
-#if CYTHON_FAST_THREAD_STATE
-    #if CYTHON_USE_EXC_INFO_STACK
+#endif
+    *method = attr;
+    return 0;
+}
+
+/* PyObjectCallMethod0 */
+  static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
+    PyObject *method = NULL, *result = NULL;
+    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
+    if (likely(is_method)) {
+        result = __Pyx_PyObject_CallOneArg(method, obj);
+        Py_DECREF(method);
+        return result;
+    }
+    if (unlikely(!method)) goto bad;
+    result = __Pyx_PyObject_CallNoArg(method);
+    Py_DECREF(method);
+bad:
+    return result;
+}
+
+/* ValidateBasesTuple */
+  #if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
+static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
+    Py_ssize_t i, n = PyTuple_GET_SIZE(bases);
+    for (i = 1; i < n; i++)
     {
-        _PyErr_StackItem *exc_info = tstate->exc_info;
-        tmp_type = exc_info->exc_type;
-        tmp_value = exc_info->exc_value;
-        tmp_tb = exc_info->exc_traceback;
-        exc_info->exc_type = local_type;
-        exc_info->exc_value = local_value;
-        exc_info->exc_traceback = local_tb;
+        PyObject *b0 = PyTuple_GET_ITEM(bases, i);
+        PyTypeObject *b;
+#if PY_MAJOR_VERSION < 3
+        if (PyClass_Check(b0))
+        {
+            PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
+                         PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
+            return -1;
+        }
+#endif
+        b = (PyTypeObject*) b0;
+        if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
+            __Pyx_DECREF_TypeName(b_name);
+            return -1;
+        }
+        if (dictoffset == 0 && b->tp_dictoffset)
+        {
+            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+            PyErr_Format(PyExc_TypeError,
+                "extension type '%.200s' has no __dict__ slot, "
+                "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                "either add 'cdef dict __dict__' to the extension type "
+                "or add '__slots__ = [...]' to the base type",
+                type_name, b_name);
+            __Pyx_DECREF_TypeName(b_name);
+            return -1;
+        }
     }
+    return 0;
+}
+#endif
+
+/* PyType_Ready */
+  static int __Pyx_PyType_Ready(PyTypeObject *t) {
+#if CYTHON_USE_TYPE_SPECS || !(CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API) || defined(PYSTON_MAJOR_VERSION)
+    (void)__Pyx_PyObject_CallMethod0;
+#if CYTHON_USE_TYPE_SPECS
+    (void)__Pyx_validate_bases_tuple;
+#endif
+    return PyType_Ready(t);
+#else
+    int r;
+    PyObject *bases = __Pyx_PyType_GetSlot(t, tp_bases, PyObject*);
+    if (bases && unlikely(__Pyx_validate_bases_tuple(t->tp_name, t->tp_dictoffset, bases) == -1))
+        return -1;
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+    {
+        int gc_was_enabled;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        gc_was_enabled = PyGC_Disable();
+        (void)__Pyx_PyObject_CallMethod0;
     #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = local_type;
-    tstate->exc_value = local_value;
-    tstate->exc_traceback = local_tb;
+        PyObject *ret, *py_status;
+        PyObject *gc = NULL;
+        #if PY_VERSION_HEX >= 0x030700a1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM+0 >= 0x07030400)
+        gc = PyImport_GetModule(__pyx_kp_u_gc);
+        #endif
+        if (unlikely(!gc)) gc = PyImport_Import(__pyx_kp_u_gc);
+        if (unlikely(!gc)) return -1;
+        py_status = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_isenabled);
+        if (unlikely(!py_status)) {
+            Py_DECREF(gc);
+            return -1;
+        }
+        gc_was_enabled = __Pyx_PyObject_IsTrue(py_status);
+        Py_DECREF(py_status);
+        if (gc_was_enabled > 0) {
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_disable);
+            if (unlikely(!ret)) {
+                Py_DECREF(gc);
+                return -1;
+            }
+            Py_DECREF(ret);
+        } else if (unlikely(gc_was_enabled == -1)) {
+            Py_DECREF(gc);
+            return -1;
+        }
     #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
+        t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
+#if PY_VERSION_HEX >= 0x030A0000
+        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
+#endif
 #else
-    PyErr_SetExcInfo(local_type, local_value, local_tb);
+        (void)__Pyx_PyObject_CallMethod0;
+#endif
+    r = PyType_Ready(t);
+#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
+        t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
+    #if PY_VERSION_HEX >= 0x030A00b1
+        if (gc_was_enabled)
+            PyGC_Enable();
+    #else
+        if (gc_was_enabled) {
+            PyObject *tp, *v, *tb;
+            PyErr_Fetch(&tp, &v, &tb);
+            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_enable);
+            if (likely(ret || r == -1)) {
+                Py_XDECREF(ret);
+                PyErr_Restore(tp, v, tb);
+            } else {
+                Py_XDECREF(tp);
+                Py_XDECREF(v);
+                Py_XDECREF(tb);
+                r = -1;
+            }
+        }
+        Py_DECREF(gc);
+    #endif
+    }
+#endif
+    return r;
 #endif
-    return 0;
-bad:
-    *type = 0;
-    *value = 0;
-    *tb = 0;
-    Py_XDECREF(local_type);
-    Py_XDECREF(local_value);
-    Py_XDECREF(local_tb);
-    return -1;
 }
 
 /* PyObject_GenericGetAttrNoDict */
   #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
+    __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
-                 "'%.50s' object has no attribute '%U'",
-                 tp->tp_name, attr_name);
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
+                 type_name, attr_name);
 #else
-                 "'%.50s' object has no attribute '%.400s'",
-                 tp->tp_name, PyString_AS_STRING(attr_name));
+                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
+                 type_name, PyString_AS_STRING(attr_name));
 #endif
+    __Pyx_DECREF_TypeName(type_name);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
     PyObject *descr;
     PyTypeObject *tp = Py_TYPE(obj);
     if (unlikely(!PyString_Check(attr_name))) {
         return PyObject_GenericGetAttr(obj, attr_name);
@@ -8148,41 +12954,20 @@
     if (unlikely(Py_TYPE(obj)->tp_dictoffset)) {
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
-/* PyObjectGetAttrStrNoError */
-  static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        __Pyx_PyErr_Clear();
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
-    PyObject *result;
-#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
-        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
-    }
-#endif
-    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
-    if (unlikely(!result)) {
-        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
-    }
-    return result;
-}
-
 /* SetupReduce */
-  static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
-  name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name);
+  name_attr = __Pyx_PyObject_GetAttrStrNoError(meth, __pyx_n_s_name);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
   } else {
       ret = -1;
   }
   if (unlikely(ret < 0)) {
       PyErr_Clear();
@@ -8190,25 +12975,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -8222,15 +13025,15 @@
             reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
             if (likely(reduce_cython)) {
                 ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                 ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
             } else if (reduce == object_reduce || PyErr_Occurred()) {
                 goto __PYX_BAD;
             }
-            setstate = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate);
+            setstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate);
             if (!setstate) PyErr_Clear();
             if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
                 setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
                 if (likely(setstate_cython)) {
                     ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                     ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                 } else if (!setstate || PyErr_Occurred()) {
@@ -8238,78 +13041,105 @@
                 }
             }
             PyType_Modified((PyTypeObject*)type_obj);
         }
     }
     goto __PYX_GOOD;
 __PYX_BAD:
-    if (!PyErr_Occurred())
-        PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
+    if (!PyErr_Occurred()) {
+        __Pyx_TypeName type_obj_name =
+            __Pyx_PyType_GetName((PyTypeObject*)type_obj);
+        PyErr_Format(PyExc_RuntimeError,
+            "Unable to initialize pickling for " __Pyx_FMT_TYPENAME, type_obj_name);
+        __Pyx_DECREF_TypeName(type_obj_name);
+    }
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
+#endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_0
+#define __PYX_HAVE_RT_ImportType_3_0_0
+static PyTypeObject *__Pyx_ImportType_3_0_0(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_0 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
-#ifdef Py_LIMITED_API
+    Py_ssize_t itemsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
-#ifndef Py_LIMITED_API
+#if !CYTHON_COMPILING_IN_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_0 &&
+            ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
-            "Expected %zd from C header, got %zd from PyObject",
-            module_name, class_name, size, basicsize);
+            "Expected %zd from C header, got %zd-%zd from PyObject",
+            module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_0 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -8317,121 +13147,1303 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* Import */
   static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
-    PyObject *empty_list = 0;
     PyObject *module = 0;
-    PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
-    PyObject *list;
+    PyObject *empty_list = 0;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (!py_import)
+    if (unlikely(!py_import))
         goto bad;
-    #endif
-    if (from_list)
-        list = from_list;
-    else {
+    if (!from_list) {
         empty_list = PyList_New(0);
-        if (!empty_list)
+        if (unlikely(!empty_list))
             goto bad;
-        list = empty_list;
+        from_list = empty_list;
     }
-    global_dict = PyModule_GetDict(__pyx_m);
-    if (!global_dict)
-        goto bad;
+    #endif
     empty_dict = PyDict_New();
-    if (!empty_dict)
+    if (unlikely(!empty_dict))
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
             if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+                #if CYTHON_COMPILING_IN_LIMITED_API
+                module = PyImport_ImportModuleLevelObject(
+                    name, empty_dict, empty_dict, from_list, 1);
+                #else
                 module = PyImport_ImportModuleLevelObject(
-                    name, global_dict, empty_dict, list, 1);
-                if (!module) {
-                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
+                    name, __pyx_d, empty_dict, from_list, 1);
+                #endif
+                if (unlikely(!module)) {
+                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
-            if (!py_level)
+            if (unlikely(!py_level))
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
+                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
+            #if CYTHON_COMPILING_IN_LIMITED_API
+            module = PyImport_ImportModuleLevelObject(
+                name, empty_dict, empty_dict, from_list, level);
+            #else
             module = PyImport_ImportModuleLevelObject(
-                name, global_dict, empty_dict, list, level);
+                name, __pyx_d, empty_dict, from_list, level);
+            #endif
             #endif
         }
     }
 bad:
+    Py_XDECREF(empty_dict);
+    Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
-    Py_XDECREF(empty_list);
-    Py_XDECREF(empty_dict);
     return module;
 }
 
+/* ImportDottedModule */
+  #if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Error(PyObject *name, PyObject *parts_tuple, Py_ssize_t count) {
+    PyObject *partial_name = NULL, *slice = NULL, *sep = NULL;
+    if (unlikely(PyErr_Occurred())) {
+        PyErr_Clear();
+    }
+    if (likely(PyTuple_GET_SIZE(parts_tuple) == count)) {
+        partial_name = name;
+    } else {
+        slice = PySequence_GetSlice(parts_tuple, 0, count);
+        if (unlikely(!slice))
+            goto bad;
+        sep = PyUnicode_FromStringAndSize(".", 1);
+        if (unlikely(!sep))
+            goto bad;
+        partial_name = PyUnicode_Join(sep, slice);
+    }
+    PyErr_Format(
+#if PY_MAJOR_VERSION < 3
+        PyExc_ImportError,
+        "No module named '%s'", PyString_AS_STRING(partial_name));
+#else
+#if PY_VERSION_HEX >= 0x030600B1
+        PyExc_ModuleNotFoundError,
+#else
+        PyExc_ImportError,
+#endif
+        "No module named '%U'", partial_name);
+#endif
+bad:
+    Py_XDECREF(sep);
+    Py_XDECREF(slice);
+    Py_XDECREF(partial_name);
+    return NULL;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx__ImportDottedModule_Lookup(PyObject *name) {
+    PyObject *imported_module;
+#if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
+    PyObject *modules = PyImport_GetModuleDict();
+    if (unlikely(!modules))
+        return NULL;
+    imported_module = __Pyx_PyDict_GetItemStr(modules, name);
+    Py_XINCREF(imported_module);
+#else
+    imported_module = PyImport_GetModule(name);
+#endif
+    return imported_module;
+}
+#endif
+#if PY_MAJOR_VERSION >= 3
+static PyObject *__Pyx_ImportDottedModule_WalkParts(PyObject *module, PyObject *name, PyObject *parts_tuple) {
+    Py_ssize_t i, nparts;
+    nparts = PyTuple_GET_SIZE(parts_tuple);
+    for (i=1; i < nparts && module; i++) {
+        PyObject *part, *submodule;
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        part = PyTuple_GET_ITEM(parts_tuple, i);
+#else
+        part = PySequence_ITEM(parts_tuple, i);
+#endif
+        submodule = __Pyx_PyObject_GetAttrStrNoError(module, part);
+#if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+        Py_DECREF(part);
+#endif
+        Py_DECREF(module);
+        module = submodule;
+    }
+    if (unlikely(!module)) {
+        return __Pyx__ImportDottedModule_Error(name, parts_tuple, i);
+    }
+    return module;
+}
+#endif
+static PyObject *__Pyx__ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if PY_MAJOR_VERSION < 3
+    PyObject *module, *from_list, *star = __pyx_n_s__3;
+    CYTHON_UNUSED_VAR(parts_tuple);
+    from_list = PyList_New(1);
+    if (unlikely(!from_list))
+        return NULL;
+    Py_INCREF(star);
+    PyList_SET_ITEM(from_list, 0, star);
+    module = __Pyx_Import(name, from_list, 0);
+    Py_DECREF(from_list);
+    return module;
+#else
+    PyObject *imported_module;
+    PyObject *module = __Pyx_Import(name, NULL, 0);
+    if (!parts_tuple || unlikely(!module))
+        return module;
+    imported_module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(imported_module)) {
+        Py_DECREF(module);
+        return imported_module;
+    }
+    PyErr_Clear();
+    return __Pyx_ImportDottedModule_WalkParts(module, name, parts_tuple);
+#endif
+}
+static PyObject *__Pyx_ImportDottedModule(PyObject *name, PyObject *parts_tuple) {
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030400B1
+    PyObject *module = __Pyx__ImportDottedModule_Lookup(name);
+    if (likely(module)) {
+        PyObject *spec = __Pyx_PyObject_GetAttrStrNoError(module, __pyx_n_s_spec);
+        if (likely(spec)) {
+            PyObject *unsafe = __Pyx_PyObject_GetAttrStrNoError(spec, __pyx_n_s_initializing);
+            if (likely(!unsafe || !__Pyx_PyObject_IsTrue(unsafe))) {
+                Py_DECREF(spec);
+                spec = NULL;
+            }
+            Py_XDECREF(unsafe);
+        }
+        if (likely(!spec)) {
+            PyErr_Clear();
+            return module;
+        }
+        Py_DECREF(spec);
+        Py_DECREF(module);
+    } else if (PyErr_Occurred()) {
+        PyErr_Clear();
+    }
+#endif
+    return __Pyx__ImportDottedModule(name, parts_tuple);
+}
+
+/* FetchSharedCythonModule */
+  static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
+    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
+    if (unlikely(!abi_module)) return NULL;
+    Py_INCREF(abi_module);
+    return abi_module;
+}
+
+/* FetchCommonType */
+  static int __Pyx_VerifyCachedType(PyObject *cached_type,
+                               const char *name,
+                               Py_ssize_t basicsize,
+                               Py_ssize_t expected_basicsize) {
+    if (!PyType_Check(cached_type)) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s is not a type object", name);
+        return -1;
+    }
+    if (basicsize != expected_basicsize) {
+        PyErr_Format(PyExc_TypeError,
+            "Shared Cython type %.200s has the wrong size, try recompiling",
+            name);
+        return -1;
+    }
+    return 0;
+}
+#if !CYTHON_USE_TYPE_SPECS
+static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
+    PyObject* abi_module;
+    const char* object_name;
+    PyTypeObject *cached_type = NULL;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    object_name = strrchr(type->tp_name, '.');
+    object_name = object_name ? object_name+1 : type->tp_name;
+    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        if (__Pyx_VerifyCachedType(
+              (PyObject *)cached_type,
+              object_name,
+              cached_type->tp_basicsize,
+              type->tp_basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    if (PyType_Ready(type) < 0) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
+        goto bad;
+    Py_INCREF(type);
+    cached_type = type;
+done:
+    Py_DECREF(abi_module);
+    return cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#else
+static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
+    PyObject *abi_module, *cached_type = NULL;
+    const char* object_name = strrchr(spec->name, '.');
+    object_name = object_name ? object_name+1 : spec->name;
+    abi_module = __Pyx_FetchSharedCythonABIModule();
+    if (!abi_module) return NULL;
+    cached_type = PyObject_GetAttrString(abi_module, object_name);
+    if (cached_type) {
+        Py_ssize_t basicsize;
+#if CYTHON_COMPILING_IN_LIMITED_API
+        PyObject *py_basicsize;
+        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
+        if (unlikely(!py_basicsize)) goto bad;
+        basicsize = PyLong_AsSsize_t(py_basicsize);
+        Py_DECREF(py_basicsize);
+        py_basicsize = 0;
+        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
+#else
+        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
+#endif
+        if (__Pyx_VerifyCachedType(
+              cached_type,
+              object_name,
+              basicsize,
+              spec->basicsize) < 0) {
+            goto bad;
+        }
+        goto done;
+    }
+    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
+    PyErr_Clear();
+    CYTHON_UNUSED_VAR(module);
+    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
+    if (unlikely(!cached_type)) goto bad;
+    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
+    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
+done:
+    Py_DECREF(abi_module);
+    assert(cached_type == NULL || PyType_Check(cached_type));
+    return (PyTypeObject *) cached_type;
+bad:
+    Py_XDECREF(cached_type);
+    cached_type = NULL;
+    goto done;
+}
+#endif
+
+/* PyVectorcallFastCallDict */
+  #if CYTHON_METH_FASTCALL
+static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    PyObject *res = NULL;
+    PyObject *kwnames;
+    PyObject **newargs;
+    PyObject **kwvalues;
+    Py_ssize_t i, pos;
+    size_t j;
+    PyObject *key, *value;
+    unsigned long keys_are_strings;
+    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
+    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
+    if (unlikely(newargs == NULL)) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+    for (j = 0; j < nargs; j++) newargs[j] = args[j];
+    kwnames = PyTuple_New(nkw);
+    if (unlikely(kwnames == NULL)) {
+        PyMem_Free(newargs);
+        return NULL;
+    }
+    kwvalues = newargs + nargs;
+    pos = i = 0;
+    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
+    while (PyDict_Next(kw, &pos, &key, &value)) {
+        keys_are_strings &= Py_TYPE(key)->tp_flags;
+        Py_INCREF(key);
+        Py_INCREF(value);
+        PyTuple_SET_ITEM(kwnames, i, key);
+        kwvalues[i] = value;
+        i++;
+    }
+    if (unlikely(!keys_are_strings)) {
+        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
+        goto cleanup;
+    }
+    res = vc(func, newargs, nargs, kwnames);
+cleanup:
+    Py_DECREF(kwnames);
+    for (i = 0; i < nkw; i++)
+        Py_DECREF(kwvalues[i]);
+    PyMem_Free(newargs);
+    return res;
+}
+static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
+{
+    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
+        return vc(func, args, nargs, NULL);
+    }
+    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
+}
+#endif
+
+/* CythonFunctionShared */
+  static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
+#if PY_VERSION_HEX < 0x030900B1
+    __Pyx_Py_XDECREF_SET(
+        __Pyx_CyFunction_GetClassObj(f),
+            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#else
+    __Pyx_Py_XDECREF_SET(
+        ((PyCMethodObject *) (f))->mm_class,
+        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
+#endif
+}
+static PyObject *
+__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
+{
+    CYTHON_UNUSED_VAR(closure);
+    if (unlikely(op->func_doc == NULL)) {
+        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
+#if PY_MAJOR_VERSION >= 3
+            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#else
+            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
+#endif
+            if (unlikely(op->func_doc == NULL))
+                return NULL;
+        } else {
+            Py_INCREF(Py_None);
+            return Py_None;
+        }
+    }
+    Py_INCREF(op->func_doc);
+    return op->func_doc;
+}
+static int
+__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (value == NULL) {
+        value = Py_None;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_doc, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_name == NULL)) {
+#if PY_MAJOR_VERSION >= 3
+        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#else
+        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
+#endif
+        if (unlikely(op->func_name == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_name);
+    return op->func_name;
+}
+static int
+__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__name__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_name, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_qualname);
+    return op->func_qualname;
+}
+static int
+__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+#if PY_MAJOR_VERSION >= 3
+    if (unlikely(value == NULL || !PyUnicode_Check(value)))
+#else
+    if (unlikely(value == NULL || !PyString_Check(value)))
+#endif
+    {
+        PyErr_SetString(PyExc_TypeError,
+                        "__qualname__ must be set to a string object");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(op->func_dict == NULL)) {
+        op->func_dict = PyDict_New();
+        if (unlikely(op->func_dict == NULL))
+            return NULL;
+    }
+    Py_INCREF(op->func_dict);
+    return op->func_dict;
+}
+static int
+__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(value == NULL)) {
+        PyErr_SetString(PyExc_TypeError,
+               "function's dictionary may not be deleted");
+        return -1;
+    }
+    if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+               "setting function's dictionary to a non-dict");
+        return -1;
+    }
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_dict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(op->func_globals);
+    return op->func_globals;
+}
+static PyObject *
+__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
+{
+    CYTHON_UNUSED_VAR(op);
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(Py_None);
+    return Py_None;
+}
+static PyObject *
+__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
+{
+    PyObject* result = (op->func_code) ? op->func_code : Py_None;
+    CYTHON_UNUSED_VAR(context);
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
+    int result = 0;
+    PyObject *res = op->defaults_getter((PyObject *) op);
+    if (unlikely(!res))
+        return -1;
+    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
+    Py_INCREF(op->defaults_tuple);
+    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
+    Py_INCREF(op->defaults_kwdict);
+    #else
+    op->defaults_tuple = PySequence_ITEM(res, 0);
+    if (unlikely(!op->defaults_tuple)) result = -1;
+    else {
+        op->defaults_kwdict = PySequence_ITEM(res, 1);
+        if (unlikely(!op->defaults_kwdict)) result = -1;
+    }
+    #endif
+    Py_DECREF(res);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__defaults__ must be set to a tuple object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_tuple;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_tuple;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value) {
+        value = Py_None;
+    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__kwdefaults__ must be set to a dict object");
+        return -1;
+    }
+    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
+                 "currently affect the values used in function calls", 1);
+    Py_INCREF(value);
+    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->defaults_kwdict;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        if (op->defaults_getter) {
+            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
+            result = op->defaults_kwdict;
+        } else {
+            result = Py_None;
+        }
+    }
+    Py_INCREF(result);
+    return result;
+}
+static int
+__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
+    CYTHON_UNUSED_VAR(context);
+    if (!value || value == Py_None) {
+        value = NULL;
+    } else if (unlikely(!PyDict_Check(value))) {
+        PyErr_SetString(PyExc_TypeError,
+                        "__annotations__ must be set to a dict object");
+        return -1;
+    }
+    Py_XINCREF(value);
+    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
+    return 0;
+}
+static PyObject *
+__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
+    PyObject* result = op->func_annotations;
+    CYTHON_UNUSED_VAR(context);
+    if (unlikely(!result)) {
+        result = PyDict_New();
+        if (unlikely(!result)) return NULL;
+        op->func_annotations = result;
+    }
+    Py_INCREF(result);
+    return result;
+}
+static PyObject *
+__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
+    int is_coroutine;
+    CYTHON_UNUSED_VAR(context);
+    if (op->func_is_coroutine) {
+        return __Pyx_NewRef(op->func_is_coroutine);
+    }
+    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
+#if PY_VERSION_HEX >= 0x03050000
+    if (is_coroutine) {
+        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
+        fromlist = PyList_New(1);
+        if (unlikely(!fromlist)) return NULL;
+        Py_INCREF(marker);
+        PyList_SET_ITEM(fromlist, 0, marker);
+        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
+        Py_DECREF(fromlist);
+        if (unlikely(!module)) goto ignore;
+        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
+        Py_DECREF(module);
+        if (likely(op->func_is_coroutine)) {
+            return __Pyx_NewRef(op->func_is_coroutine);
+        }
+ignore:
+        PyErr_Clear();
+    }
+#endif
+    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
+    return __Pyx_NewRef(op->func_is_coroutine);
+}
+static PyGetSetDef __pyx_CyFunction_getsets[] = {
+    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
+    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
+    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
+    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
+    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
+    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
+    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
+    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
+    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
+    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
+    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
+    {0, 0, 0, 0, 0}
+};
+static PyMemberDef __pyx_CyFunction_members[] = {
+    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
+#if CYTHON_USE_TYPE_SPECS
+    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
+#if CYTHON_METH_FASTCALL
+#if CYTHON_BACKPORT_VECTORCALL
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
+#else
+    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
+#endif
+#endif
+#if PY_VERSION_HEX < 0x030500A0
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
+#else
+    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
+#endif
+#endif
+    {0, 0, 0,  0, 0}
+};
+static PyObject *
+__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
+{
+    CYTHON_UNUSED_VAR(args);
+#if PY_MAJOR_VERSION >= 3
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
+#else
+    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
+#endif
+}
+static PyMethodDef __pyx_CyFunction_methods[] = {
+    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
+    {0, 0, 0, 0}
+};
+#if PY_VERSION_HEX < 0x030500A0
+#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
+#else
+#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
+#endif
+static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
+                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyCFunctionObject *cf = (PyCFunctionObject*) op;
+    if (unlikely(op == NULL))
+        return NULL;
+    op->flags = flags;
+    __Pyx_CyFunction_weakreflist(op) = NULL;
+    cf->m_ml = ml;
+    cf->m_self = (PyObject *) op;
+    Py_XINCREF(closure);
+    op->func_closure = closure;
+    Py_XINCREF(module);
+    cf->m_module = module;
+    op->func_dict = NULL;
+    op->func_name = NULL;
+    Py_INCREF(qualname);
+    op->func_qualname = qualname;
+    op->func_doc = NULL;
+#if PY_VERSION_HEX < 0x030900B1
+    op->func_classobj = NULL;
+#else
+    ((PyCMethodObject*)op)->mm_class = NULL;
+#endif
+    op->func_globals = globals;
+    Py_INCREF(op->func_globals);
+    Py_XINCREF(code);
+    op->func_code = code;
+    op->defaults_pyobjects = 0;
+    op->defaults_size = 0;
+    op->defaults = NULL;
+    op->defaults_tuple = NULL;
+    op->defaults_kwdict = NULL;
+    op->defaults_getter = NULL;
+    op->func_annotations = NULL;
+    op->func_is_coroutine = NULL;
+#if CYTHON_METH_FASTCALL
+    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
+    case METH_NOARGS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
+        break;
+    case METH_O:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
+        break;
+    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
+        break;
+    case METH_FASTCALL | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        __Pyx_CyFunction_func_vectorcall(op) = NULL;
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        Py_DECREF(op);
+        return NULL;
+    }
+#endif
+    return (PyObject *) op;
+}
+static int
+__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
+{
+    Py_CLEAR(m->func_closure);
+    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
+    Py_CLEAR(m->func_dict);
+    Py_CLEAR(m->func_name);
+    Py_CLEAR(m->func_qualname);
+    Py_CLEAR(m->func_doc);
+    Py_CLEAR(m->func_globals);
+    Py_CLEAR(m->func_code);
+#if PY_VERSION_HEX < 0x030900B1
+    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
+#else
+    {
+        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
+        ((PyCMethodObject *) (m))->mm_class = NULL;
+        Py_XDECREF(cls);
+    }
+#endif
+    Py_CLEAR(m->defaults_tuple);
+    Py_CLEAR(m->defaults_kwdict);
+    Py_CLEAR(m->func_annotations);
+    Py_CLEAR(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_XDECREF(pydefaults[i]);
+        PyObject_Free(m->defaults);
+        m->defaults = NULL;
+    }
+    return 0;
+}
+static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    if (__Pyx_CyFunction_weakreflist(m) != NULL)
+        PyObject_ClearWeakRefs((PyObject *) m);
+    __Pyx_CyFunction_clear(m);
+    __Pyx_PyHeapTypeObject_GC_Del(m);
+}
+static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
+{
+    PyObject_GC_UnTrack(m);
+    __Pyx__CyFunction_dealloc(m);
+}
+static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
+{
+    Py_VISIT(m->func_closure);
+    Py_VISIT(((PyCFunctionObject*)m)->m_module);
+    Py_VISIT(m->func_dict);
+    Py_VISIT(m->func_name);
+    Py_VISIT(m->func_qualname);
+    Py_VISIT(m->func_doc);
+    Py_VISIT(m->func_globals);
+    Py_VISIT(m->func_code);
+    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
+    Py_VISIT(m->defaults_tuple);
+    Py_VISIT(m->defaults_kwdict);
+    Py_VISIT(m->func_is_coroutine);
+    if (m->defaults) {
+        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
+        int i;
+        for (i = 0; i < m->defaults_pyobjects; i++)
+            Py_VISIT(pydefaults[i]);
+    }
+    return 0;
+}
+static PyObject*
+__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
+{
+#if PY_MAJOR_VERSION >= 3
+    return PyUnicode_FromFormat("<cyfunction %U at %p>",
+                                op->func_qualname, (void *)op);
+#else
+    return PyString_FromFormat("<cyfunction %s at %p>",
+                               PyString_AsString(op->func_qualname), (void *)op);
+#endif
+}
+static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
+    PyCFunctionObject* f = (PyCFunctionObject*)func;
+    PyCFunction meth = f->m_ml->ml_meth;
+    Py_ssize_t size;
+    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
+    case METH_VARARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0))
+            return (*meth)(self, arg);
+        break;
+    case METH_VARARGS | METH_KEYWORDS:
+        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
+    case METH_NOARGS:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 0))
+                return (*meth)(self, NULL);
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    case METH_O:
+        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
+            size = PyTuple_GET_SIZE(arg);
+            if (likely(size == 1)) {
+                PyObject *result, *arg0;
+                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+                arg0 = PyTuple_GET_ITEM(arg, 0);
+                #else
+                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
+                #endif
+                result = (*meth)(self, arg0);
+                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
+                Py_DECREF(arg0);
+                #endif
+                return result;
+            }
+            PyErr_Format(PyExc_TypeError,
+                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+                f->m_ml->ml_name, size);
+            return NULL;
+        }
+        break;
+    default:
+        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
+        return NULL;
+    }
+    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
+                 f->m_ml->ml_name);
+    return NULL;
+}
+static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
+}
+static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
+    PyObject *result;
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
+#if CYTHON_METH_FASTCALL
+     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
+    if (vc) {
+#if CYTHON_ASSUME_SAFE_MACROS
+        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
+#else
+        (void) &__Pyx_PyVectorcall_FastCallDict;
+        return PyVectorcall_Call(func, args, kw);
+#endif
+    }
+#endif
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        Py_ssize_t argc;
+        PyObject *new_args;
+        PyObject *self;
+        argc = PyTuple_GET_SIZE(args);
+        new_args = PyTuple_GetSlice(args, 1, argc);
+        if (unlikely(!new_args))
+            return NULL;
+        self = PyTuple_GetItem(args, 0);
+        if (unlikely(!self)) {
+            Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
+            return NULL;
+        }
+        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
+        Py_DECREF(new_args);
+    } else {
+        result = __Pyx_CyFunction_Call(func, args, kw);
+    }
+    return result;
+}
+#if CYTHON_METH_FASTCALL
+static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
+{
+    int ret = 0;
+    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
+        if (unlikely(nargs < 1)) {
+            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
+                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+            return -1;
+        }
+        ret = 1;
+    }
+    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
+        PyErr_Format(PyExc_TypeError,
+                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
+        return -1;
+    }
+    return ret;
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 0)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, NULL);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    if (unlikely(nargs != 1)) {
+        PyErr_Format(PyExc_TypeError,
+            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
+            def->ml_name, nargs);
+        return NULL;
+    }
+    return def->ml_meth(self, args[0]);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+}
+static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
+{
+    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
+    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
+    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
+#if CYTHON_BACKPORT_VECTORCALL
+    Py_ssize_t nargs = (Py_ssize_t)nargsf;
+#else
+    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
+#endif
+    PyObject *self;
+    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
+    case 1:
+        self = args[0];
+        args += 1;
+        nargs -= 1;
+        break;
+    case 0:
+        self = ((PyCFunctionObject*)cyfunc)->m_self;
+        break;
+    default:
+        return NULL;
+    }
+    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
+}
+#endif
+#if CYTHON_USE_TYPE_SPECS
+static PyType_Slot __pyx_CyFunctionType_slots[] = {
+    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
+    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
+    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
+    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
+    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
+    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
+    {Py_tp_members, (void *)__pyx_CyFunction_members},
+    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
+    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
+    {0, 0},
+};
+static PyType_Spec __pyx_CyFunctionType_spec = {
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    __pyx_CyFunctionType_slots
+};
+#else
+static PyTypeObject __pyx_CyFunctionType_type = {
+    PyVarObject_HEAD_INIT(0, 0)
+    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
+    sizeof(__pyx_CyFunctionObject),
+    0,
+    (destructor) __Pyx_CyFunction_dealloc,
+#if !CYTHON_METH_FASTCALL
+    0,
+#elif CYTHON_BACKPORT_VECTORCALL
+    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
+#else
+    offsetof(PyCFunctionObject, vectorcall),
+#endif
+    0,
+    0,
+#if PY_MAJOR_VERSION < 3
+    0,
+#else
+    0,
+#endif
+    (reprfunc) __Pyx_CyFunction_repr,
+    0,
+    0,
+    0,
+    0,
+    __Pyx_CyFunction_CallAsMethod,
+    0,
+    0,
+    0,
+    0,
+#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
+    Py_TPFLAGS_METHOD_DESCRIPTOR |
+#endif
+#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
+    _Py_TPFLAGS_HAVE_VECTORCALL |
+#endif
+    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
+    0,
+    (traverseproc) __Pyx_CyFunction_traverse,
+    (inquiry) __Pyx_CyFunction_clear,
+    0,
+#if PY_VERSION_HEX < 0x030500A0
+    offsetof(__pyx_CyFunctionObject, func_weakreflist),
+#else
+    offsetof(PyCFunctionObject, m_weakreflist),
+#endif
+    0,
+    0,
+    __pyx_CyFunction_methods,
+    __pyx_CyFunction_members,
+    __pyx_CyFunction_getsets,
+    0,
+    0,
+    __Pyx_PyMethod_New,
+    0,
+    offsetof(__pyx_CyFunctionObject, func_dict),
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+    0,
+#if PY_VERSION_HEX >= 0x030400a1
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+    0,
+#endif
+#if __PYX_NEED_TP_PRINT_SLOT
+    0,
+#endif
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
+    0,
+#endif
+};
+#endif
+static int __pyx_CyFunction_init(PyObject *module) {
+#if CYTHON_USE_TYPE_SPECS
+    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
+#else
+    CYTHON_UNUSED_VAR(module);
+    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
+#endif
+    if (unlikely(__pyx_CyFunctionType == NULL)) {
+        return -1;
+    }
+    return 0;
+}
+static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults = PyObject_Malloc(size);
+    if (unlikely(!m->defaults))
+        return PyErr_NoMemory();
+    memset(m->defaults, 0, size);
+    m->defaults_pyobjects = pyobjects;
+    m->defaults_size = size;
+    return m->defaults;
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_tuple = tuple;
+    Py_INCREF(tuple);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->defaults_kwdict = dict;
+    Py_INCREF(dict);
+}
+static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
+    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
+    m->func_annotations = dict;
+    Py_INCREF(dict);
+}
+
+/* CythonFunction */
+  static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
+                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
+    PyObject *op = __Pyx_CyFunction_Init(
+        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
+        ml, flags, qualname, closure, module, globals, code
+    );
+    if (likely(op)) {
+        PyObject_GC_Track(op);
+    }
+    return op;
+}
+
 /* CLineInTraceback */
   #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
+    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-  static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
+  #if !CYTHON_COMPILING_IN_LIMITED_API
+static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
         if (code_line < entries[mid].code_line) {
@@ -8501,84 +14513,118 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
+#endif
 
 /* AddTraceback */
   #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
+#if CYTHON_COMPILING_IN_LIMITED_API
+static void __Pyx_AddTraceback(const char *funcname, int c_line,
+                               int py_line, const char *filename) {
+    if (c_line) {
+        (void) __pyx_cfilenm;
+        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
+    }
+    _PyTraceback_Add(funcname, filename, py_line);
+}
+#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
+        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -8586,19 +14632,25 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+#endif
 
 #if PY_MAJOR_VERSION < 3
 static int __Pyx_GetBuffer(PyObject *obj, Py_buffer *view, int flags) {
+    __Pyx_TypeName obj_type_name;
     if (PyObject_CheckBuffer(obj)) return PyObject_GetBuffer(obj, view, flags);
-    PyErr_Format(PyExc_TypeError, "'%.200s' does not have the buffer interface", Py_TYPE(obj)->tp_name);
+    obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError,
+                 "'" __Pyx_FMT_TYPENAME "' does not have the buffer interface",
+                 obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
     return -1;
 }
 static void __Pyx_ReleaseBuffer(Py_buffer *view) {
     PyObject *obj = view->obj;
     if (!obj) return;
     if (PyObject_CheckBuffer(obj)) {
         PyBuffer_Release(view);
@@ -8629,78 +14681,16 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_Py_intptr_t(Py_intptr_t value) {
-    const Py_intptr_t neg_one = (Py_intptr_t) ((Py_intptr_t) 0 - (Py_intptr_t) 1), const_zero = (Py_intptr_t) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(Py_intptr_t) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(Py_intptr_t) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(Py_intptr_t) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(Py_intptr_t) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(Py_intptr_t),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return x + y*(__pyx_t_float_complex)_Complex_I;
@@ -8712,15 +14702,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_sum_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         __pyx_t_float_complex z;
         z.real = a.real + b.real;
@@ -8820,15 +14810,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -8846,15 +14836,15 @@
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return x + y*(__pyx_t_double_complex)_Complex_I;
@@ -8866,15 +14856,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+  #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
 #else
     static CYTHON_INLINE int __Pyx_c_eq_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_sum_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         __pyx_t_double_complex z;
         z.real = a.real + b.real;
@@ -8974,15 +14964,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -9001,181 +14991,265 @@
             return z;
         }
     #endif
 #endif
 
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(int) < sizeof(long)) {
+        if ((sizeof(int) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
-                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
+                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
-                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
+                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
-                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
+                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(int) <= sizeof(unsigned long)) {
+            if ((sizeof(int) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (int) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
-                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
+                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(int) <= sizeof(long)) {
+            if ((sizeof(int) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (int) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (int) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (int) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (int) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (int) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((int) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((int) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -9189,371 +15263,266 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntFromPy */
-  static CYTHON_INLINE Py_intptr_t __Pyx_PyInt_As_Py_intptr_t(PyObject *x) {
-    const Py_intptr_t neg_one = (Py_intptr_t) ((Py_intptr_t) 0 - (Py_intptr_t) 1), const_zero = (Py_intptr_t) 0;
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if (sizeof(Py_intptr_t) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (Py_intptr_t) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (Py_intptr_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(Py_intptr_t, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(Py_intptr_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(Py_intptr_t) >= 2 * PyLong_SHIFT) {
-                            return (Py_intptr_t) (((((Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(Py_intptr_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(Py_intptr_t) >= 3 * PyLong_SHIFT) {
-                            return (Py_intptr_t) (((((((Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(Py_intptr_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(Py_intptr_t) >= 4 * PyLong_SHIFT) {
-                            return (Py_intptr_t) (((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0]));
-                        }
-                    }
-                    break;
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
-#else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (Py_intptr_t) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if (sizeof(Py_intptr_t) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(Py_intptr_t) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (Py_intptr_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(Py_intptr_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(Py_intptr_t,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(Py_intptr_t) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(Py_intptr_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (Py_intptr_t) (((Py_intptr_t)-1)*(((((Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(Py_intptr_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(Py_intptr_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (Py_intptr_t) ((((((Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
-                        }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(Py_intptr_t) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(Py_intptr_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (Py_intptr_t) (((Py_intptr_t)-1)*(((((((Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(Py_intptr_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(Py_intptr_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (Py_intptr_t) ((((((((Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
-                        }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(Py_intptr_t) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(Py_intptr_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(Py_intptr_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (Py_intptr_t) (((Py_intptr_t)-1)*(((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(Py_intptr_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(Py_intptr_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(Py_intptr_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (Py_intptr_t) ((((((((((Py_intptr_t)digits[3]) << PyLong_SHIFT) | (Py_intptr_t)digits[2]) << PyLong_SHIFT) | (Py_intptr_t)digits[1]) << PyLong_SHIFT) | (Py_intptr_t)digits[0])));
-                        }
-                    }
-                    break;
-            }
-#endif
-            if (sizeof(Py_intptr_t) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, long, PyLong_AsLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(Py_intptr_t) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(Py_intptr_t, PY_LONG_LONG, PyLong_AsLongLong(x))
-#endif
-            }
-        }
-        {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
-            Py_intptr_t val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
-#endif
-            return (Py_intptr_t) -1;
-        }
-    } else {
-        Py_intptr_t val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (Py_intptr_t) -1;
-        val = __Pyx_PyInt_As_Py_intptr_t(tmp);
-        Py_DECREF(tmp);
-        return val;
-    }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to Py_intptr_t");
-    return (Py_intptr_t) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to Py_intptr_t");
-    return (Py_intptr_t) -1;
-}
-
-/* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if (sizeof(long) < sizeof(long)) {
+        if ((sizeof(long) < sizeof(long))) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
-                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
+                goto raise_neg_overflow;
+            } else if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_DigitCount(x)) {
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
+                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
-                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
+                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
-                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
+                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if (sizeof(long) <= sizeof(unsigned long)) {
+            if ((sizeof(long) <= sizeof(unsigned long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (long) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+            if (__Pyx_PyLong_IsCompact(x)) {
+                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
+            } else {
+                const digit* digits = __Pyx_PyLong_Digits(x);
+                assert(__Pyx_PyLong_DigitCount(x) > 1);
+                switch (__Pyx_PyLong_SignedDigitCount(x)) {
+                    case -2:
+                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 2:
+                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -3:
+                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 3:
+                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case -4:
+                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
-                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                        break;
+                    case 4:
+                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
+                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
+                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
+                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
+                            }
                         }
-                    }
-                    break;
+                        break;
+                }
             }
 #endif
-            if (sizeof(long) <= sizeof(long)) {
+            if ((sizeof(long) <= sizeof(long))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
+#if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
- #endif
+#endif
             if (likely(v)) {
+                int ret = -1;
+#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
+                ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                           bytes, sizeof(val),
+                                           is_little, !is_unsigned);
+#else
+                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
+                int bits, remaining_bits, is_negative = 0;
+                long idigit;
+                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
+                if (unlikely(!PyLong_CheckExact(v))) {
+                    PyObject *tmp = v;
+                    v = PyNumber_Long(v);
+                    assert(PyLong_CheckExact(v));
+                    Py_DECREF(tmp);
+                    if (unlikely(!v)) return (long) -1;
+                }
+#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                if (Py_SIZE(x) == 0)
+                    return (long) 0;
+                is_negative = Py_SIZE(x) < 0;
+#else
+                {
+                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                    if (unlikely(result < 0))
+                        return (long) -1;
+                    is_negative = result == 1;
+                }
+#endif
+                if (is_unsigned && unlikely(is_negative)) {
+                    goto raise_neg_overflow;
+                } else if (is_negative) {
+                    stepval = PyNumber_Invert(v);
+                    if (unlikely(!stepval))
+                        return (long) -1;
+                } else {
+                    stepval = __Pyx_NewRef(v);
+                }
+                val = (long) 0;
+                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
+                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
+                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
+                    PyObject *tmp, *digit;
+                    digit = PyNumber_And(stepval, mask);
+                    if (unlikely(!digit)) goto done;
+                    idigit = PyLong_AsLong(digit);
+                    Py_DECREF(digit);
+                    if (unlikely(idigit < 0)) goto done;
+                    tmp = PyNumber_Rshift(stepval, shift);
+                    if (unlikely(!tmp)) goto done;
+                    Py_DECREF(stepval); stepval = tmp;
+                    val |= ((long) idigit) << bits;
+                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+                    if (Py_SIZE(stepval) == 0)
+                        goto unpacking_done;
+                    #endif
+                }
+                idigit = PyLong_AsLong(stepval);
+                if (unlikely(idigit < 0)) goto done;
+                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
+                if (unlikely(idigit >= (1L << remaining_bits)))
+                    goto raise_overflow;
+                val |= ((long) idigit) << bits;
+            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
+            unpacking_done:
+            #endif
+                if (!is_unsigned) {
+                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
+                        goto raise_overflow;
+                    if (is_negative)
+                        val = ~val;
+                }
+                ret = 0;
+            done:
+                Py_XDECREF(shift);
+                Py_XDECREF(mask);
+                Py_XDECREF(stepval);
+#endif
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
-#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -9566,206 +15535,62 @@
     return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
-/* CIntFromPy */
-  static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
-    const size_t neg_one = (size_t) ((size_t) 0 - (size_t) 1), const_zero = (size_t) 0;
-    const int is_unsigned = neg_one > const_zero;
-#if PY_MAJOR_VERSION < 3
-    if (likely(PyInt_Check(x))) {
-        if (sizeof(size_t) < sizeof(long)) {
-            __PYX_VERIFY_RETURN_INT(size_t, long, PyInt_AS_LONG(x))
-        } else {
-            long val = PyInt_AS_LONG(x);
-            if (is_unsigned && unlikely(val < 0)) {
-                goto raise_neg_overflow;
-            }
-            return (size_t) val;
-        }
-    } else
-#endif
-    if (likely(PyLong_Check(x))) {
-        if (is_unsigned) {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case  1: __PYX_VERIFY_RETURN_INT(size_t, digit, digits[0])
-                case 2:
-                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 2 * PyLong_SHIFT) {
-                            return (size_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 3 * PyLong_SHIFT) {
-                            return (size_t) (((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
-                            return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
-                        }
-                    }
-                    break;
-            }
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-            if (unlikely(Py_SIZE(x) < 0)) {
-                goto raise_neg_overflow;
-            }
-#else
-            {
-                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                if (unlikely(result < 0))
-                    return (size_t) -1;
-                if (unlikely(result == 1))
-                    goto raise_neg_overflow;
-            }
-#endif
-            if (sizeof(size_t) <= sizeof(unsigned long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned long, PyLong_AsUnsignedLong(x))
-#ifdef HAVE_LONG_LONG
-            } else if (sizeof(size_t) <= sizeof(unsigned PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
-#endif
-            }
-        } else {
-#if CYTHON_USE_PYLONG_INTERNALS
-            const digit* digits = ((PyLongObject*)x)->ob_digit;
-            switch (Py_SIZE(x)) {
-                case  0: return (size_t) 0;
-                case -1: __PYX_VERIFY_RETURN_INT(size_t, sdigit, (sdigit) (-(sdigit)digits[0]))
-                case  1: __PYX_VERIFY_RETURN_INT(size_t,  digit, +digits[0])
-                case -2:
-                    if (8 * sizeof(size_t) - 1 > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 2:
-                    if (8 * sizeof(size_t) > 1 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                            return (size_t) ((((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case -3:
-                    if (8 * sizeof(size_t) - 1 > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 3:
-                    if (8 * sizeof(size_t) > 2 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                            return (size_t) ((((((((size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case -4:
-                    if (8 * sizeof(size_t) - 1 > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (size_t) (((size_t)-1)*(((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-                case 4:
-                    if (8 * sizeof(size_t) > 3 * PyLong_SHIFT) {
-                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
-                            __PYX_VERIFY_RETURN_INT(size_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                        } else if (8 * sizeof(size_t) - 1 > 4 * PyLong_SHIFT) {
-                            return (size_t) ((((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0])));
-                        }
-                    }
-                    break;
-            }
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
 #endif
-            if (sizeof(size_t) <= sizeof(long)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, long, PyLong_AsLong(x))
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-            } else if (sizeof(size_t) <= sizeof(PY_LONG_LONG)) {
-                __PYX_VERIFY_RETURN_INT_EXC(size_t, PY_LONG_LONG, PyLong_AsLongLong(x))
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
-            }
         }
-        {
-#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
-            PyErr_SetString(PyExc_RuntimeError,
-                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
-#else
-            size_t val;
-            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
- #if PY_MAJOR_VERSION < 3
-            if (likely(v) && !PyLong_Check(v)) {
-                PyObject *tmp = v;
-                v = PyNumber_Long(tmp);
-                Py_DECREF(tmp);
-            }
- #endif
-            if (likely(v)) {
-                int one = 1; int is_little = (int)*(unsigned char *)&one;
-                unsigned char *bytes = (unsigned char *)&val;
-                int ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                              bytes, sizeof(val),
-                                              is_little, !is_unsigned);
-                Py_DECREF(v);
-                if (likely(!ret))
-                    return val;
-            }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
-            return (size_t) -1;
         }
-    } else {
-        size_t val;
-        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
-        if (!tmp) return (size_t) -1;
-        val = __Pyx_PyInt_As_size_t(tmp);
-        Py_DECREF(tmp);
-        return val;
     }
-raise_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "value too large to convert to size_t");
-    return (size_t) -1;
-raise_neg_overflow:
-    PyErr_SetString(PyExc_OverflowError,
-        "can't convert negative value to size_t");
-    return (size_t) -1;
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
 }
 
 /* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
@@ -9786,19 +15611,34 @@
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
+/* FormatTypeName */
+  #if CYTHON_COMPILING_IN_LIMITED_API
+static __Pyx_TypeName
+__Pyx_PyType_GetName(PyTypeObject* tp)
+{
+    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
+                                               __pyx_n_s_name);
+    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
+        PyErr_Clear();
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__29));
+    }
+    return name;
+}
+#endif
+
 /* FastTypeChecks */
   #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = a->tp_base;
+        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -9811,14 +15651,30 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
+static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
+    PyObject *mro;
+    if (cls == a || cls == b) return 1;
+    mro = cls->tp_mro;
+    if (likely(mro)) {
+        Py_ssize_t i, n;
+        n = PyTuple_GET_SIZE(mro);
+        for (i = 0; i < n; i++) {
+            PyObject *base = PyTuple_GET_ITEM(mro, i);
+            if (base == (PyObject *)a || base == (PyObject *)b)
+                return 1;
+        }
+        return 0;
+    }
+    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
+}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -9835,19 +15691,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
-    if (!res) {
-        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    if (exc_type1) {
+        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
+    } else {
+        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
-    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -9888,56 +15744,88 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
-                      "compiletime version %s of module '%.100s' "
+                      "compile time version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
-  static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
+  #if PY_MAJOR_VERSION >= 3
+static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
+    if (t.is_unicode | t.is_str) {
+        if (t.intern) {
+            *str = PyUnicode_InternFromString(t.s);
+        } else if (t.encoding) {
+            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
+        } else {
+            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
+        }
+    } else {
+        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
+    }
+    if (!*str)
+        return -1;
+    if (PyObject_Hash(*str) == -1)
+        return -1;
+    return 0;
+}
+#endif
+static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION < 3
+        #if PY_MAJOR_VERSION >= 3
+        __Pyx_InitString(*t, t->p);
+        #else
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
-        #else
-        if (t->is_unicode | t->is_str) {
-            if (t->intern) {
-                *t->p = PyUnicode_InternFromString(t->s);
-            } else if (t->encoding) {
-                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
-            } else {
-                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
-            }
-        } else {
-            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
-        }
-        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
+        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -9991,15 +15879,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -10020,30 +15908,34 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
+    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type %.200s).  "
-                "The ability to return an instance of a strict subclass of int "
-                "is deprecated, and may be removed in a future version of Python.",
-                Py_TYPE(result)->tp_name)) {
+                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
+                "The ability to return an instance of a strict subclass of int is deprecated, "
+                "and may be removed in a future version of Python.",
+                result_type_name)) {
+            __Pyx_DECREF_TypeName(result_type_name);
             Py_DECREF(result);
             return NULL;
         }
+        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type %.200s)",
-                 type_name, type_name, Py_TYPE(result)->tp_name);
+                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
+                 type_name, type_name, result_type_name);
+    __Pyx_DECREF_TypeName(result_type_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -10101,21 +15993,19 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    const digit* digits = ((PyLongObject*)b)->ob_digit;
-    const Py_ssize_t size = Py_SIZE(b);
-    if (likely(__Pyx_sst_abs(size) <= 1)) {
-        ival = likely(size) ? digits[0] : 0;
-        if (size == -1) ival = -ival;
-        return ival;
+    if (likely(__Pyx_PyLong_IsCompact(b))) {
+        return __Pyx_PyLong_CompactValue(b);
     } else {
+      const digit* digits = __Pyx_PyLong_Digits(b);
+      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -10150,16 +16040,41 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
+static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
+  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
+#if PY_MAJOR_VERSION < 3
+  } else if (likely(PyInt_CheckExact(o))) {
+    return PyInt_AS_LONG(o);
+#endif
+  } else {
+    Py_ssize_t ival;
+    PyObject *x;
+    x = PyNumber_Index(o);
+    if (!x) return -1;
+    ival = PyInt_AsLong(x);
+    Py_DECREF(x);
+    return ival;
+  }
+}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
+/* #### Code section: utility_code_pragmas_end ### */
+#ifdef _MSC_VER
+#pragma warning( pop )
+#endif
+
+
+
+/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `pandana-0.6.1/src/cyaccess.pyx` & `pandana-0.7/src/cyaccess.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#cython: language_level=3
+
 cimport cython
 from libcpp cimport bool
 from libcpp.vector cimport vector
 from libcpp.string cimport string
 from libcpp.pair cimport pair
 
 import numpy as np
@@ -23,14 +25,15 @@
         void initializeAccVar(string, vector[long], vector[double])
         vector[double] getAllAggregateAccessibilityVariables(
             float, string, string, string, int)
         vector[int] Route(int, int, int)
         vector[vector[int]] Routes(vector[long], vector[long], int)
         double Distance(int, int, int)
         vector[double] Distances(vector[long], vector[long], int)
+        vector[vector[pair[long, float]]] Range(vector[long], float, int, vector[long])
         void precomputeRangeQueries(double)
 
 
 cdef np.ndarray[double] convert_vector_to_array_dbl(vector[double] vec):
     cdef np.ndarray arr = np.zeros(len(vec), dtype="double")
     for i in range(len(vec)):
         arr[i] = vec[i]
@@ -187,10 +190,20 @@
             np.ndarray[long] destnodes, int impno=0):
         """
         srcnodes - node ids of origins
         destnodes - node ids of destinations
         impno - impedance id
         """
         return self.access.Distances(srcnodes, destnodes, impno)
-
+    
     def precompute_range(self, double radius):
         self.access.precomputeRangeQueries(radius)
+
+    def nodes_in_range(self, vector[long] srcnodes, float radius, int impno, 
+            np.ndarray[long] ext_ids):
+        """
+        srcnodes - node ids of origins
+        radius - maximum range in which to search for nearby nodes
+        impno - the impedance id to use
+        ext_ids - all node ids in the network
+        """
+        return self.access.Range(srcnodes, radius, impno, ext_ids)
```

### Comparing `pandana-0.6.1/src/graphalg.cpp` & `pandana-0.7/src/graphalg.cpp`

 * *Files identical despite different names*

### Comparing `pandana-0.6.1/src/graphalg.h` & `pandana-0.7/src/graphalg.h`

 * *Files identical despite different names*

