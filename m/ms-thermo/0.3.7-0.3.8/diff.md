# Comparing `tmp/ms_thermo-0.3.7.tar.gz` & `tmp/ms_thermo-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_thermo-0.3.7.tar", last modified: Wed Jul 26 11:00:47 2023, max compression
+gzip compressed data, was "ms_thermo-0.3.8.tar", last modified: Wed Jul 26 14:50:33 2023, max compression
```

## Comparing `ms_thermo-0.3.7.tar` & `ms_thermo-0.3.8.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.622903 ms_thermo-0.3.7/
--rw-r--r--   0 dauptain   (502) staff       (20)     1611 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/LICENSE
--rw-r--r--   0 dauptain   (502) staff       (20)        9 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/MANIFEST.in
--rw-r--r--   0 dauptain   (502) staff       (20)     3910 2023-07-26 11:00:47.623019 ms_thermo-0.3.7/PKG-INFO
--rw-r--r--   0 dauptain   (502) staff       (20)     3087 2023-07-11 08:41:34.000000 ms_thermo-0.3.7/README.md
--rw-r--r--   0 dauptain   (502) staff       (20)     1423 2023-07-26 11:00:47.623789 ms_thermo-0.3.7/setup.cfg
--rw-r--r--   0 dauptain   (502) staff       (20)       39 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/setup.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.602871 ms_thermo-0.3.7/src/
--rw-r--r--   0 dauptain   (502) staff       (20)     6148 2023-01-07 18:14:05.000000 ms_thermo-0.3.7/src/.DS_Store
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.608629 ms_thermo-0.3.7/src/ms_thermo/
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.614124 ms_thermo-0.3.7/src/ms_thermo/INPUT/
--rw-r--r--   0 dauptain   (502) staff       (20)    64672 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/src/ms_thermo/INPUT/2S_KERO_BFER.h5
--rw-r--r--   0 dauptain   (502) staff       (20)   126263 2022-08-02 19:02:02.000000 ms_thermo-0.3.7/src/ms_thermo/INPUT/Luche1.cti
--rw-r--r--   0 dauptain   (502) staff       (20)       46 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/src/ms_thermo/INPUT/__init__.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1501 2022-08-02 19:02:02.000000 ms_thermo-0.3.7/src/ms_thermo/INPUT/default_gasout_input.yml
--rw-r--r--   0 dauptain   (502) staff       (20)   140366 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/src/ms_thermo/INPUT/species_database.dat
--rw-r--r--   0 dauptain   (502) staff       (20)       22 2023-07-26 09:56:31.000000 ms_thermo-0.3.7/src/ms_thermo/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.620092 ms_thermo-0.3.7/src/ms_thermo/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)      187 2023-07-11 08:43:50.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     3933 2023-07-11 08:43:51.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/constants.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     9524 2023-07-11 08:43:51.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/flame_params.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    16092 2023-07-11 08:43:51.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/gasout.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     1473 2023-07-26 09:35:53.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/kero_prim2cons.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    18559 2023-07-11 12:13:39.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/mixture_state.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    26357 2023-07-11 08:43:51.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/species.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    25645 2023-07-11 08:49:39.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/state.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     5064 2023-07-11 12:13:39.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/tadia.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     3387 2023-07-26 09:11:05.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/yk_from_phi.cpython-311.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     7526 2023-07-11 08:41:34.000000 ms_thermo-0.3.7/src/ms_thermo/cli.py
--rw-r--r--   0 dauptain   (502) staff       (20)     3102 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/src/ms_thermo/constants.py
--rw-r--r--   0 dauptain   (502) staff       (20)     6809 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/src/ms_thermo/flame_params.py
--rw-r--r--   0 dauptain   (502) staff       (20)    13004 2023-07-11 08:41:34.000000 ms_thermo-0.3.7/src/ms_thermo/gasout.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1003 2022-08-02 19:02:02.000000 ms_thermo-0.3.7/src/ms_thermo/kero_prim2cons.py
--rw-r--r--   0 dauptain   (502) staff       (20)    13167 2023-07-11 08:41:34.000000 ms_thermo-0.3.7/src/ms_thermo/mixture_state.py
--rw-r--r--   0 dauptain   (502) staff       (20)    18061 2022-10-17 15:49:58.000000 ms_thermo-0.3.7/src/ms_thermo/species.py
--rw-r--r--   0 dauptain   (502) staff       (20)    19842 2023-07-11 08:49:31.000000 ms_thermo-0.3.7/src/ms_thermo/state.py
--rw-r--r--   0 dauptain   (502) staff       (20)     4218 2022-08-02 19:02:02.000000 ms_thermo-0.3.7/src/ms_thermo/tadia.py
--rw-r--r--   0 dauptain   (502) staff       (20)     2633 2023-07-26 10:00:57.000000 ms_thermo-0.3.7/src/ms_thermo/yk_from_phi.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.611263 ms_thermo-0.3.7/src/ms_thermo.egg-info/
--rw-r--r--   0 dauptain   (502) staff       (20)     3910 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/PKG-INFO
--rw-r--r--   0 dauptain   (502) staff       (20)     1442 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/SOURCES.txt
--rw-r--r--   0 dauptain   (502) staff       (20)        1 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/dependency_links.txt
--rw-r--r--   0 dauptain   (502) staff       (20)      295 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/entry_points.txt
--rw-r--r--   0 dauptain   (502) staff       (20)        1 2022-06-27 12:25:37.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/not-zip-safe
--rw-r--r--   0 dauptain   (502) staff       (20)      109 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/requires.txt
--rw-r--r--   0 dauptain   (502) staff       (20)       10 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/top_level.txt
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.622460 ms_thermo-0.3.7/tests/
--rw-r--r--   0 dauptain   (502) staff       (20)     1209 2023-07-26 09:54:05.000000 ms_thermo-0.3.7/tests/test_compositions.py
--rw-r--r--   0 dauptain   (502) staff       (20)      385 2022-08-02 19:02:02.000000 ms_thermo-0.3.7/tests/test_kero_prim2cons.py
--rw-r--r--   0 dauptain   (502) staff       (20)     2463 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/tests/test_mixture_state.py
--rw-r--r--   0 dauptain   (502) staff       (20)     8108 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/tests/test_state.py
--rw-r--r--   0 dauptain   (502) staff       (20)      423 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/tests/test_tadia.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 14:50:33.997134 ms_thermo-0.3.8/
+-rw-r--r--   0 dauptain   (502) staff       (20)     1611 2022-06-27 11:42:00.000000 ms_thermo-0.3.8/LICENSE
+-rw-r--r--   0 dauptain   (502) staff       (20)        9 2022-06-27 11:42:00.000000 ms_thermo-0.3.8/MANIFEST.in
+-rw-r--r--   0 dauptain   (502) staff       (20)     3910 2023-07-26 14:50:33.997228 ms_thermo-0.3.8/PKG-INFO
+-rw-r--r--   0 dauptain   (502) staff       (20)     3087 2023-07-11 08:41:34.000000 ms_thermo-0.3.8/README.md
+-rw-r--r--   0 dauptain   (502) staff       (20)     1423 2023-07-26 14:50:33.997725 ms_thermo-0.3.8/setup.cfg
+-rw-r--r--   0 dauptain   (502) staff       (20)       39 2022-06-27 11:42:00.000000 ms_thermo-0.3.8/setup.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 14:50:33.978802 ms_thermo-0.3.8/src/
+-rw-r--r--   0 dauptain   (502) staff       (20)     6148 2023-01-07 18:14:05.000000 ms_thermo-0.3.8/src/.DS_Store
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 14:50:33.984378 ms_thermo-0.3.8/src/ms_thermo/
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 14:50:33.989603 ms_thermo-0.3.8/src/ms_thermo/INPUT/
+-rw-r--r--   0 dauptain   (502) staff       (20)    64672 2022-06-27 11:42:00.000000 ms_thermo-0.3.8/src/ms_thermo/INPUT/2S_KERO_BFER.h5
+-rw-r--r--   0 dauptain   (502) staff       (20)   126263 2022-08-02 19:02:02.000000 ms_thermo-0.3.8/src/ms_thermo/INPUT/Luche1.cti
+-rw-r--r--   0 dauptain   (502) staff       (20)       46 2022-06-27 11:42:00.000000 ms_thermo-0.3.8/src/ms_thermo/INPUT/__init__.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1501 2022-08-02 19:02:02.000000 ms_thermo-0.3.8/src/ms_thermo/INPUT/default_gasout_input.yml
+-rw-r--r--   0 dauptain   (502) staff       (20)   140366 2022-06-27 11:42:00.000000 ms_thermo-0.3.8/src/ms_thermo/INPUT/species_database.dat
+-rw-r--r--   0 dauptain   (502) staff       (20)       22 2023-07-26 13:07:02.000000 ms_thermo-0.3.8/src/ms_thermo/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 14:50:33.995001 ms_thermo-0.3.8/src/ms_thermo/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)      187 2023-07-26 14:38:56.000000 ms_thermo-0.3.8/src/ms_thermo/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3933 2023-07-11 08:43:51.000000 ms_thermo-0.3.8/src/ms_thermo/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     9524 2023-07-11 08:43:51.000000 ms_thermo-0.3.8/src/ms_thermo/__pycache__/flame_params.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    16092 2023-07-11 08:43:51.000000 ms_thermo-0.3.8/src/ms_thermo/__pycache__/gasout.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1473 2023-07-26 09:35:53.000000 ms_thermo-0.3.8/src/ms_thermo/__pycache__/kero_prim2cons.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    18559 2023-07-11 12:13:39.000000 ms_thermo-0.3.8/src/ms_thermo/__pycache__/mixture_state.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    26357 2023-07-11 08:43:51.000000 ms_thermo-0.3.8/src/ms_thermo/__pycache__/species.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    25645 2023-07-11 08:49:39.000000 ms_thermo-0.3.8/src/ms_thermo/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     5064 2023-07-11 12:13:39.000000 ms_thermo-0.3.8/src/ms_thermo/__pycache__/tadia.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3549 2023-07-26 14:38:56.000000 ms_thermo-0.3.8/src/ms_thermo/__pycache__/yk_from_phi.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     7526 2023-07-11 08:41:34.000000 ms_thermo-0.3.8/src/ms_thermo/cli.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     3102 2022-06-27 11:42:00.000000 ms_thermo-0.3.8/src/ms_thermo/constants.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     6809 2022-06-27 11:42:00.000000 ms_thermo-0.3.8/src/ms_thermo/flame_params.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    13004 2023-07-11 08:41:34.000000 ms_thermo-0.3.8/src/ms_thermo/gasout.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1003 2022-08-02 19:02:02.000000 ms_thermo-0.3.8/src/ms_thermo/kero_prim2cons.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    13167 2023-07-11 08:41:34.000000 ms_thermo-0.3.8/src/ms_thermo/mixture_state.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    18061 2022-10-17 15:49:58.000000 ms_thermo-0.3.8/src/ms_thermo/species.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    19842 2023-07-11 08:49:31.000000 ms_thermo-0.3.8/src/ms_thermo/state.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     4218 2022-08-02 19:02:02.000000 ms_thermo-0.3.8/src/ms_thermo/tadia.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     2681 2023-07-26 13:08:04.000000 ms_thermo-0.3.8/src/ms_thermo/yk_from_phi.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 14:50:33.987076 ms_thermo-0.3.8/src/ms_thermo.egg-info/
+-rw-r--r--   0 dauptain   (502) staff       (20)     3910 2023-07-26 14:50:33.000000 ms_thermo-0.3.8/src/ms_thermo.egg-info/PKG-INFO
+-rw-r--r--   0 dauptain   (502) staff       (20)     1442 2023-07-26 14:50:33.000000 ms_thermo-0.3.8/src/ms_thermo.egg-info/SOURCES.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)        1 2023-07-26 14:50:33.000000 ms_thermo-0.3.8/src/ms_thermo.egg-info/dependency_links.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)      295 2023-07-26 14:50:33.000000 ms_thermo-0.3.8/src/ms_thermo.egg-info/entry_points.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)        1 2022-06-27 12:25:37.000000 ms_thermo-0.3.8/src/ms_thermo.egg-info/not-zip-safe
+-rw-r--r--   0 dauptain   (502) staff       (20)      109 2023-07-26 14:50:33.000000 ms_thermo-0.3.8/src/ms_thermo.egg-info/requires.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)       10 2023-07-26 14:50:33.000000 ms_thermo-0.3.8/src/ms_thermo.egg-info/top_level.txt
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 14:50:33.996802 ms_thermo-0.3.8/tests/
+-rw-r--r--   0 dauptain   (502) staff       (20)     1311 2023-07-26 13:05:39.000000 ms_thermo-0.3.8/tests/test_compositions.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      422 2023-07-26 14:41:56.000000 ms_thermo-0.3.8/tests/test_kero_prim2cons.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     2463 2022-06-27 11:42:00.000000 ms_thermo-0.3.8/tests/test_mixture_state.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     8108 2022-06-27 11:42:00.000000 ms_thermo-0.3.8/tests/test_state.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      461 2023-07-26 14:44:07.000000 ms_thermo-0.3.8/tests/test_tadia.py
```

### Comparing `ms_thermo-0.3.7/LICENSE` & `ms_thermo-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/PKG-INFO` & `ms_thermo-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms_thermo
-Version: 0.3.7
+Version: 0.3.8
 Summary: Utilities to work on 2D and 3D structured grids
 Home-page: https://gitlab.com/cerfacs/ms_thermo
 Author: CoopTeam-CERFACS
 Author-email: coop@cerfacs.com
 Project-URL: Homepage, https://gitlab.com/cerfacs/ms_thermo
 Project-URL: Documentation, https://ms_thermo.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/cerfacs/ms_thermo/-/issues
```

### Comparing `ms_thermo-0.3.7/README.md` & `ms_thermo-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/setup.cfg` & `ms_thermo-0.3.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/.DS_Store` & `ms_thermo-0.3.8/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/INPUT/2S_KERO_BFER.h5` & `ms_thermo-0.3.8/src/ms_thermo/INPUT/2S_KERO_BFER.h5`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/INPUT/Luche1.cti` & `ms_thermo-0.3.8/src/ms_thermo/INPUT/Luche1.cti`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/INPUT/default_gasout_input.yml` & `ms_thermo-0.3.8/src/ms_thermo/INPUT/default_gasout_input.yml`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/INPUT/species_database.dat` & `ms_thermo-0.3.8/src/ms_thermo/INPUT/species_database.dat`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/__pycache__/constants.cpython-311.pyc` & `ms_thermo-0.3.8/src/ms_thermo/__pycache__/constants.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/__pycache__/flame_params.cpython-311.pyc` & `ms_thermo-0.3.8/src/ms_thermo/__pycache__/flame_params.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/__pycache__/gasout.cpython-311.pyc` & `ms_thermo-0.3.8/src/ms_thermo/__pycache__/gasout.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/__pycache__/kero_prim2cons.cpython-311.pyc` & `ms_thermo-0.3.8/src/ms_thermo/__pycache__/kero_prim2cons.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/__pycache__/mixture_state.cpython-311.pyc` & `ms_thermo-0.3.8/src/ms_thermo/__pycache__/mixture_state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/__pycache__/species.cpython-311.pyc` & `ms_thermo-0.3.8/src/ms_thermo/__pycache__/species.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/__pycache__/state.cpython-311.pyc` & `ms_thermo-0.3.8/src/ms_thermo/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/__pycache__/tadia.cpython-311.pyc` & `ms_thermo-0.3.8/src/ms_thermo/__pycache__/tadia.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/__pycache__/yk_from_phi.cpython-311.pyc` & `ms_thermo-0.3.8/src/ms_thermo/__pycache__/yk_from_phi.cpython-311.pyc`

 * *Files 23% similar despite different names*

#### Python bytecode

```diff
@@ -1,97 +1,101 @@
 magic:    0xa70d0d0a
-moddate:  0x3ae6bf64 (Tue Jul 25 15:11:54 2023 UTC)
-files sz: 2480
+moddate:  0xb41ac164 (Wed Jul 26 13:08:04 2023 UTC)
+files sz: 2681
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
-      0x970064005a006401640267025a01640364046405640664079c045a0264
-      08650364096503640a65036606640b84045a04640c650364086503640965
-      03640a65036608640d84045a05640e65036408650364096503640a650366
-      08640f84045a066414640e6503640865036409650364116507640a650366
-      0a641284055a0864135300
+      0x970064005a006401640267025a0164035a02640464056406640764089c
+      045a0364096504640a6504640b65046606640c84045a05640d6504640965
+      04640a6504640b65046608640e84045a06640f650464096504640a650464
+      0b65046608641084045a076415640f650464096504640a65046412650864
+      0b6504660a641384055a0964145300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nThis script calculate mass_fraction of species from a Phi\n')
                  4 STORE_NAME               0 (__doc__)
    
      5           6 LOAD_CONST               1 ('yk_from_phi')
                  8 LOAD_CONST               2 ('phi_from_far')
                 10 BUILD_LIST               2
                 12 STORE_NAME               1 (__all__)
    
-     8          14 LOAD_CONST               3 (0.0120107)
-                16 LOAD_CONST               4 (0.00100797)
-                18 LOAD_CONST               5 (0.0319988)
-                20 LOAD_CONST               6 (0.0280134)
-                22 LOAD_CONST               7 (('C', 'H', 'O2', 'N2'))
-                24 BUILD_CONST_KEY_MAP      4
-                26 STORE_NAME               2 (MOLAR_MASSES)
+     8          14 LOAD_CONST               3 (0.2314)
+                16 STORE_NAME               2 (YO2_IN_AIR)
    
-    11          28 LOAD_CONST               8 ('c_x')
-                30 LOAD_NAME                3 (float)
-                32 LOAD_CONST               9 ('h_y')
-                34 LOAD_NAME                3 (float)
-                36 LOAD_CONST              10 ('return')
-                38 LOAD_NAME                3 (float)
-                40 BUILD_TUPLE              6
-                42 LOAD_CONST              11 (<code object far_stochio, file "/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py", line 11>)
-                44 MAKE_FUNCTION            4 (annotations)
-                46 STORE_NAME               4 (far_stochio)
+    10          18 LOAD_CONST               4 (0.0120107)
+                20 LOAD_CONST               5 (0.00100797)
+                22 LOAD_CONST               6 (0.0319988)
+                24 LOAD_CONST               7 (0.0280134)
+                26 LOAD_CONST               8 (('C', 'H', 'O2', 'N2'))
+                28 BUILD_CONST_KEY_MAP      4
+                30 STORE_NAME               3 (MOLAR_MASSES)
    
-    20          48 LOAD_CONST              12 ('far')
-                50 LOAD_NAME                3 (float)
-                52 LOAD_CONST               8 ('c_x')
-                54 LOAD_NAME                3 (float)
-                56 LOAD_CONST               9 ('h_y')
-                58 LOAD_NAME                3 (float)
-                60 LOAD_CONST              10 ('return')
-                62 LOAD_NAME                3 (float)
-                64 BUILD_TUPLE              8
-                66 LOAD_CONST              13 (<code object phi_from_far, file "/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py", line 20>)
-                68 MAKE_FUNCTION            4 (annotations)
-                70 STORE_NAME               5 (phi_from_far)
+    13          32 LOAD_CONST               9 ('c_x')
+                34 LOAD_NAME                4 (float)
+                36 LOAD_CONST              10 ('h_y')
+                38 LOAD_NAME                4 (float)
+                40 LOAD_CONST              11 ('return')
+                42 LOAD_NAME                4 (float)
+                44 BUILD_TUPLE              6
+                46 LOAD_CONST              12 (<code object far_stochio, file "/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py", line 13>)
+                48 MAKE_FUNCTION            4 (annotations)
+                50 STORE_NAME               5 (far_stochio)
    
-    37          72 LOAD_CONST              14 ('phi')
-                74 LOAD_NAME                3 (float)
-                76 LOAD_CONST               8 ('c_x')
-                78 LOAD_NAME                3 (float)
-                80 LOAD_CONST               9 ('h_y')
-                82 LOAD_NAME                3 (float)
-                84 LOAD_CONST              10 ('return')
-                86 LOAD_NAME                3 (float)
-                88 BUILD_TUPLE              8
-                90 LOAD_CONST              15 (<code object far_from_phi, file "/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py", line 37>)
-                92 MAKE_FUNCTION            4 (annotations)
-                94 STORE_NAME               6 (far_from_phi)
+    27          52 LOAD_CONST              13 ('far')
+                54 LOAD_NAME                4 (float)
+                56 LOAD_CONST               9 ('c_x')
+                58 LOAD_NAME                4 (float)
+                60 LOAD_CONST              10 ('h_y')
+                62 LOAD_NAME                4 (float)
+                64 LOAD_CONST              11 ('return')
+                66 LOAD_NAME                4 (float)
+                68 BUILD_TUPLE              8
+                70 LOAD_CONST              14 (<code object phi_from_far, file "/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py", line 27>)
+                72 MAKE_FUNCTION            4 (annotations)
+                74 STORE_NAME               6 (phi_from_far)
    
-    55          96 LOAD_CONST              20 (('fuel',))
-                98 LOAD_CONST              14 ('phi')
-               100 LOAD_NAME                3 (float)
-               102 LOAD_CONST               8 ('c_x')
-               104 LOAD_NAME                3 (float)
-               106 LOAD_CONST               9 ('h_y')
-               108 LOAD_NAME                3 (float)
-               110 LOAD_CONST              17 ('fuel_name')
-               112 LOAD_NAME                7 (str)
-               114 LOAD_CONST              10 ('return')
-               116 LOAD_NAME                3 (float)
-               118 BUILD_TUPLE             10
-               120 LOAD_CONST              18 (<code object yk_from_phi, file "/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py", line 55>)
-               122 MAKE_FUNCTION            5 (defaults, annotations)
-               124 STORE_NAME               8 (yk_from_phi)
-               126 LOAD_CONST              19 (None)
-               128 RETURN_VALUE
+    44          76 LOAD_CONST              15 ('phi')
+                78 LOAD_NAME                4 (float)
+                80 LOAD_CONST               9 ('c_x')
+                82 LOAD_NAME                4 (float)
+                84 LOAD_CONST              10 ('h_y')
+                86 LOAD_NAME                4 (float)
+                88 LOAD_CONST              11 ('return')
+                90 LOAD_NAME                4 (float)
+                92 BUILD_TUPLE              8
+                94 LOAD_CONST              16 (<code object far_from_phi, file "/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py", line 44>)
+                96 MAKE_FUNCTION            4 (annotations)
+                98 STORE_NAME               7 (far_from_phi)
+   
+    62         100 LOAD_CONST              21 (('fuel',))
+               102 LOAD_CONST              15 ('phi')
+               104 LOAD_NAME                4 (float)
+               106 LOAD_CONST               9 ('c_x')
+               108 LOAD_NAME                4 (float)
+               110 LOAD_CONST              10 ('h_y')
+               112 LOAD_NAME                4 (float)
+               114 LOAD_CONST              18 ('fuel_name')
+               116 LOAD_NAME                8 (str)
+               118 LOAD_CONST              11 ('return')
+               120 LOAD_NAME                4 (float)
+               122 BUILD_TUPLE             10
+               124 LOAD_CONST              19 (<code object yk_from_phi, file "/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py", line 62>)
+               126 MAKE_FUNCTION            5 (defaults, annotations)
+               128 STORE_NAME               9 (yk_from_phi)
+               130 LOAD_CONST              20 (None)
+               132 RETURN_VALUE
    consts
       '\nThis script calculate mass_fraction of species from a Phi\n'
       'yk_from_phi'
       'phi_from_far'
+      0.2314
       0.0120107
       0.00100797
       0.0319988
       0.0280134
       ('C', 'H', 'O2', 'N2')
       'c_x'
       'h_y'
@@ -100,281 +104,256 @@
          argcount  : 2
          nlocals   : 7
          stacksize : 4
          flags     : 3
          code
             0x97007c007400000000000000000000006401190000000000000000007a
             0500007c017400000000000000000000006402190000000000000000007a
-            0500007a0000007d027c007c0164037a0b00007a0000007d0364047d047c
-            047c037400000000000000000000006405190000000000000000007a0500
-            007a0500007c027a0b00007d0564067c057a0b00007d067c065300
-          11           0 RESUME                   0
+            0500007a0000007d027c007c0164037a0b00007a0000007d036404740200
+            0000000000000000007a0b00007d047c047c037400000000000000000000
+            006405190000000000000000007a0500007a0500007c027a0b00007d0564
+            047c057a0b00007d067c065300
+          13           0 RESUME                   0
          
-          13           2 LOAD_FAST                0 (c_x)
+          20           2 LOAD_FAST                0 (c_x)
                        4 LOAD_GLOBAL              0 (MOLAR_MASSES)
                       16 LOAD_CONST               1 ('C')
                       18 BINARY_SUBSCR
                       28 BINARY_OP                5 (*)
                       32 LOAD_FAST                1 (h_y)
                       34 LOAD_GLOBAL              0 (MOLAR_MASSES)
                       46 LOAD_CONST               2 ('H')
                       48 BINARY_SUBSCR
                       58 BINARY_OP                5 (*)
                       62 BINARY_OP                0 (+)
                       66 STORE_FAST               2 (mass_mol_fuel)
          
-          14          68 LOAD_FAST                0 (c_x)
+          21          68 LOAD_FAST                0 (c_x)
                       70 LOAD_FAST                1 (h_y)
                       72 LOAD_CONST               3 (4)
                       74 BINARY_OP               11 (/)
                       78 BINARY_OP                0 (+)
                       82 STORE_FAST               3 (coeff_o2)
          
-          15          84 LOAD_CONST               4 (4.32152117545376)
-                      86 STORE_FAST               4 (coef_air)
-         
-          16          88 LOAD_FAST                4 (coef_air)
-                      90 LOAD_FAST                3 (coeff_o2)
-                      92 LOAD_GLOBAL              0 (MOLAR_MASSES)
-                     104 LOAD_CONST               5 ('O2')
-                     106 BINARY_SUBSCR
-                     116 BINARY_OP                5 (*)
-                     120 BINARY_OP                5 (*)
-                     124 LOAD_FAST                2 (mass_mol_fuel)
-                     126 BINARY_OP               11 (/)
-                     130 STORE_FAST               5 (afr_sto)
-         
-          17         132 LOAD_CONST               6 (1.0)
-                     134 LOAD_FAST                5 (afr_sto)
-                     136 BINARY_OP               11 (/)
-                     140 STORE_FAST               6 (far_sto)
+          22          84 LOAD_CONST               4 (1.0)
+                      86 LOAD_GLOBAL              2 (YO2_IN_AIR)
+                      98 BINARY_OP               11 (/)
+                     102 STORE_FAST               4 (coef_air)
+         
+          23         104 LOAD_FAST                4 (coef_air)
+                     106 LOAD_FAST                3 (coeff_o2)
+                     108 LOAD_GLOBAL              0 (MOLAR_MASSES)
+                     120 LOAD_CONST               5 ('O2')
+                     122 BINARY_SUBSCR
+                     132 BINARY_OP                5 (*)
+                     136 BINARY_OP                5 (*)
+                     140 LOAD_FAST                2 (mass_mol_fuel)
+                     142 BINARY_OP               11 (/)
+                     146 STORE_FAST               5 (afr_sto)
+         
+          24         148 LOAD_CONST               4 (1.0)
+                     150 LOAD_FAST                5 (afr_sto)
+                     152 BINARY_OP               11 (/)
+                     156 STORE_FAST               6 (far_sto)
          
-          18         142 LOAD_FAST                6 (far_sto)
-                     144 RETURN_VALUE
+          25         158 LOAD_FAST                6 (far_sto)
+                     160 RETURN_VALUE
          consts
-            'Return the fuel air ratio stoechiometric according to c_x h_y'
+            'Return the fuel air ratio stoechiometric according to c_x h_y\n    \n    valid for AIR , not for PURE OXYGEN!!!\n\n    BTW, the example in https://en.wikipedia.org/wiki/Air%E2%80%93fuel_ratio is for pure oxygen...\n    '
             'C'
             'H'
             4
-            4.32152117545376
-            'O2'
             1.0
-         names      ('MOLAR_MASSES',)
+            'O2'
+         names      ('MOLAR_MASSES', 'YO2_IN_AIR')
          varnames   ('c_x', 'h_y', 'mass_mol_fuel', 'coeff_o2', 'coef_air', 'afr_sto', 'far_sto')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py'
          name       'far_stochio'
-         firstlineno 11
-         lnotab 0x02024201100104012c010a01
+         firstlineno 13
+         lnotab 0x02074201100114012c010a01
       'far'
       code
          argcount  : 3
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x97007c007401000000000000000000007c017c02a6020000ab02000000
             00000000007a0b00005300
-          20           0 RESUME                   0
+          27           0 RESUME                   0
          
-          34           2 LOAD_FAST                0 (far)
+          41           2 LOAD_FAST                0 (far)
                        4 LOAD_GLOBAL              1 (NULL + far_stochio)
                       16 LOAD_FAST                1 (c_x)
                       18 LOAD_FAST                2 (h_y)
                       20 PRECALL                  2
                       24 CALL                     2
                       34 BINARY_OP               11 (/)
                       38 RETURN_VALUE
          consts
-            '\n    *Return phi coefficient with the fuel air ratio coeff + fuel composition*\n\n    :param far: the air-fuel ratio\n    :type far: float\n    :param c_x: stoechio coeff of Carbone\n    :type c_x: float\n    :param h_y: stoechio coeff of hydrogene\n    :type h_y: float\n\n    :returns:\n        - **phi** - Equivalence ratio\n    '
+            '\n    *Return phi coefficient with the fuel air ratio coeff + fuel composition (Valid for AIR, Not  PURE OXYGEN!!)**\n\n    :param far: the air-fuel ratio\n    :type far: float\n    :param c_x: stoechio coeff of Carbone\n    :type c_x: float\n    :param h_y: stoechio coeff of hydrogene\n    :type h_y: float\n\n    :returns:\n        - **phi** - Equivalence ratio\n    '
          names      ('far_stochio',)
          varnames   ('far', 'c_x', 'h_y')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py'
          name       'phi_from_far'
-         firstlineno 20
+         firstlineno 27
          lnotab 0x020e
       'phi'
       code
          argcount  : 3
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x97007c007401000000000000000000007c017c02a6020000ab02000000
             00000000007a0500005300
-          37           0 RESUME                   0
+          44           0 RESUME                   0
          
-          51           2 LOAD_FAST                0 (phi)
+          58           2 LOAD_FAST                0 (phi)
                        4 LOAD_GLOBAL              1 (NULL + far_stochio)
                       16 LOAD_FAST                1 (c_x)
                       18 LOAD_FAST                2 (h_y)
                       20 PRECALL                  2
                       24 CALL                     2
                       34 BINARY_OP                5 (*)
                       38 RETURN_VALUE
          consts
-            '\n    *Return fuel air ratio coeff  with the phi coefficient + fuel composition*\n\n    :param phi: eq. ratio coef\n    :type far: float\n    :param c_x: stoechio coeff of Carbone\n    :type c_x: float\n    :param h_y: stoechio coeff of hydrogene\n    :type h_y: float\n\n    :returns:\n        - **far** - Equivalence ratio\n    '
+            '\n    *Return fuel air ratio coeff  with the phi coefficient + fuel composition (Valid for AIR, Not  PURE OXYGEN!!)*\n\n    :param phi: eq. ratio coef\n    :type far: float\n    :param c_x: stoechio coeff of Carbone\n    :type c_x: float\n    :param h_y: stoechio coeff of hydrogene\n    :type h_y: float\n\n    :returns:\n        - **far** - Equivalence ratio\n    '
          names      ('far_stochio',)
          varnames   ('phi', 'c_x', 'h_y')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py'
          name       'far_from_phi'
-         firstlineno 37
+         firstlineno 44
          lnotab 0x020e
       'fuel'
       'fuel_name'
       code
          argcount  : 4
-         nlocals   : 9
+         nlocals   : 7
          stacksize : 7
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
-            047c017402000000000000000000006401190000000000000000007a0500
-            007c027402000000000000000000006402190000000000000000007a0500
-            007a0000007d057c017c0264037a0b00007a0000007d067c067402000000
-            000000000000006404190000000000000000007a0500007c057a0b00007d
-            077c0064056b0200000000720664057c047c033c0000006e306406640664
-            066407740200000000000000000000640819000000000000000000740200
-            0000000000000000006404190000000000000000007a0b00007a0500007a
-            0000007c077c007a0b00007a0500007a0000007a0b00007c047c033c0000
-            0064097c047c03190000000000000000007a0a00007d087c08640a7a0b00
-            007c0464083c000000640b7c046408190000000000000000007a0500007c
-            0464043c0000007c045300
-          55           0 RESUME                   0
+            047c0064016b0200000000720664017c047c033c0000006e436402740300
+            0000000000000000007c017c02a6020000ab0200000000000000007a0b00
+            007d05640264026402640374040000000000000000000064041900000000
+            00000000007404000000000000000000006405190000000000000000007a
+            0b00007a0500007a0000007c057c007a0b00007a0500007a0000007a0b00
+            007c047c033c00000064067c047c03190000000000000000007a0a00007d
+            0664067406000000000000000000007a0a00007c067a0500007c0464043c
+            0000007406000000000000000000007c067a0500007c0464053c0000007c
+            045300
+          62           0 RESUME                   0
          
-          72           2 LOAD_GLOBAL              1 (NULL + dict)
+          79           2 LOAD_GLOBAL              1 (NULL + dict)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               4 (y_k)
          
-          73          30 LOAD_FAST                1 (c_x)
-                      32 LOAD_GLOBAL              2 (MOLAR_MASSES)
-                      44 LOAD_CONST               1 ('C')
-                      46 BINARY_SUBSCR
-                      56 BINARY_OP                5 (*)
-                      60 LOAD_FAST                2 (h_y)
-                      62 LOAD_GLOBAL              2 (MOLAR_MASSES)
-                      74 LOAD_CONST               2 ('H')
-                      76 BINARY_SUBSCR
-                      86 BINARY_OP                5 (*)
-                      90 BINARY_OP                0 (+)
-                      94 STORE_FAST               5 (mass_mol_fuel)
-         
-          74          96 LOAD_FAST                1 (c_x)
-                      98 LOAD_FAST                2 (h_y)
-                     100 LOAD_CONST               3 (4)
-                     102 BINARY_OP               11 (/)
-                     106 BINARY_OP                0 (+)
-                     110 STORE_FAST               6 (coeff_o2)
-         
-          75         112 LOAD_FAST                6 (coeff_o2)
-                     114 LOAD_GLOBAL              2 (MOLAR_MASSES)
-                     126 LOAD_CONST               4 ('O2')
-                     128 BINARY_SUBSCR
-                     138 BINARY_OP                5 (*)
-                     142 LOAD_FAST                5 (mass_mol_fuel)
-                     144 BINARY_OP               11 (/)
-                     148 STORE_FAST               7 (y_o2_fuel_sto)
-         
-          77         150 LOAD_FAST                0 (phi)
-                     152 LOAD_CONST               5 (0.0)
-                     154 COMPARE_OP               2 (==)
-                     160 POP_JUMP_FORWARD_IF_FALSE     6 (to 174)
-         
-          78         162 LOAD_CONST               5 (0.0)
-                     164 LOAD_FAST                4 (y_k)
-                     166 LOAD_FAST                3 (fuel_name)
-                     168 STORE_SUBSCR
-                     172 JUMP_FORWARD            48 (to 270)
-         
-          80     >>  174 LOAD_CONST               6 (1.0)
-         
-          81         176 LOAD_CONST               6 (1.0)
-         
-          82         178 LOAD_CONST               6 (1.0)
-                     180 LOAD_CONST               7 (3.76)
-                     182 LOAD_GLOBAL              2 (MOLAR_MASSES)
-                     194 LOAD_CONST               8 ('N2')
-                     196 BINARY_SUBSCR
-                     206 LOAD_GLOBAL              2 (MOLAR_MASSES)
-                     218 LOAD_CONST               4 ('O2')
-                     220 BINARY_SUBSCR
-                     230 BINARY_OP               11 (/)
-                     234 BINARY_OP                5 (*)
-                     238 BINARY_OP                0 (+)
-         
-          83         242 LOAD_FAST                7 (y_o2_fuel_sto)
-                     244 LOAD_FAST                0 (phi)
-                     246 BINARY_OP               11 (/)
-         
-          82         250 BINARY_OP                5 (*)
-         
-          81         254 BINARY_OP                0 (+)
-         
-          80         258 BINARY_OP               11 (/)
-                     262 LOAD_FAST                4 (y_k)
-                     264 LOAD_FAST                3 (fuel_name)
-                     266 STORE_SUBSCR
-         
-          85     >>  270 LOAD_CONST               9 (1)
-                     272 LOAD_FAST                4 (y_k)
-                     274 LOAD_FAST                3 (fuel_name)
-                     276 BINARY_SUBSCR
-                     286 BINARY_OP               10 (-)
-                     290 STORE_FAST               8 (y_air)
-         
-          86         292 LOAD_FAST                8 (y_air)
-                     294 LOAD_CONST              10 (1.303794)
-                     296 BINARY_OP               11 (/)
-                     300 LOAD_FAST                4 (y_k)
-                     302 LOAD_CONST               8 ('N2')
-                     304 STORE_SUBSCR
-         
-          87         308 LOAD_CONST              11 (0.303794)
-                     310 LOAD_FAST                4 (y_k)
-                     312 LOAD_CONST               8 ('N2')
-                     314 BINARY_SUBSCR
-                     324 BINARY_OP                5 (*)
-                     328 LOAD_FAST                4 (y_k)
-                     330 LOAD_CONST               4 ('O2')
-                     332 STORE_SUBSCR
+          80          30 LOAD_FAST                0 (phi)
+                      32 LOAD_CONST               1 (0.0)
+                      34 COMPARE_OP               2 (==)
+                      40 POP_JUMP_FORWARD_IF_FALSE     6 (to 54)
+         
+          81          42 LOAD_CONST               1 (0.0)
+                      44 LOAD_FAST                4 (y_k)
+                      46 LOAD_FAST                3 (fuel_name)
+                      48 STORE_SUBSCR
+                      52 JUMP_FORWARD            67 (to 188)
+         
+          83     >>   54 LOAD_CONST               2 (1.0)
+                      56 LOAD_GLOBAL              3 (NULL + far_stochio)
+                      68 LOAD_FAST                1 (c_x)
+                      70 LOAD_FAST                2 (h_y)
+                      72 PRECALL                  2
+                      76 CALL                     2
+                      86 BINARY_OP               11 (/)
+                      90 STORE_FAST               5 (afr_stochio)
+         
+          84          92 LOAD_CONST               2 (1.0)
+         
+          85          94 LOAD_CONST               2 (1.0)
+         
+          86          96 LOAD_CONST               2 (1.0)
+                      98 LOAD_CONST               3 (3.76)
+                     100 LOAD_GLOBAL              4 (MOLAR_MASSES)
+                     112 LOAD_CONST               4 ('N2')
+                     114 BINARY_SUBSCR
+                     124 LOAD_GLOBAL              4 (MOLAR_MASSES)
+                     136 LOAD_CONST               5 ('O2')
+                     138 BINARY_SUBSCR
+                     148 BINARY_OP               11 (/)
+                     152 BINARY_OP                5 (*)
+                     156 BINARY_OP                0 (+)
+         
+          87         160 LOAD_FAST                5 (afr_stochio)
+                     162 LOAD_FAST                0 (phi)
+                     164 BINARY_OP               11 (/)
+         
+          86         168 BINARY_OP                5 (*)
+         
+          85         172 BINARY_OP                0 (+)
+         
+          84         176 BINARY_OP               11 (/)
+                     180 LOAD_FAST                4 (y_k)
+                     182 LOAD_FAST                3 (fuel_name)
+                     184 STORE_SUBSCR
+         
+          90     >>  188 LOAD_CONST               6 (1)
+                     190 LOAD_FAST                4 (y_k)
+                     192 LOAD_FAST                3 (fuel_name)
+                     194 BINARY_SUBSCR
+                     204 BINARY_OP               10 (-)
+                     208 STORE_FAST               6 (y_air)
+         
+          91         210 LOAD_CONST               6 (1)
+                     212 LOAD_GLOBAL              6 (YO2_IN_AIR)
+                     224 BINARY_OP               10 (-)
+                     228 LOAD_FAST                6 (y_air)
+                     230 BINARY_OP                5 (*)
+                     234 LOAD_FAST                4 (y_k)
+                     236 LOAD_CONST               4 ('N2')
+                     238 STORE_SUBSCR
+         
+          92         242 LOAD_GLOBAL              6 (YO2_IN_AIR)
+                     254 LOAD_FAST                6 (y_air)
+                     256 BINARY_OP                5 (*)
+                     260 LOAD_FAST                4 (y_k)
+                     262 LOAD_CONST               5 ('O2')
+                     264 STORE_SUBSCR
          
-          89         336 LOAD_FAST                4 (y_k)
-                     338 RETURN_VALUE
+          94         268 LOAD_FAST                4 (y_k)
+                     270 RETURN_VALUE
          consts
-            '\n    *Return the species mass fractions in a fresh fuel-air mixture*\n\n    :param phi: equivalence ratio\n    :type phi: float\n    :param c_x: stoechio coeff of Carbone\n    :type c_x: float\n    :param h_y: stoechio coeff of hydrogene\n    :type h_y: float\n    :param fuel_name: Name of the fuel\n    :type fuel_name: str\n\n    :returns:\n        - **y_k** - A dict of mass fractions\n\n    '
-            'C'
-            'H'
-            4
-            'O2'
+            '\n    *Return the species mass fractions in a fresh fuel-air mixture (Valid for AIR, Not  PURE OXYGEN!!)*\n\n    :param phi: equivalence ratio\n    :type phi: float\n    :param c_x: stoechio coeff of Carbone\n    :type c_x: float\n    :param h_y: stoechio coeff of hydrogene\n    :type h_y: float\n    :param fuel_name: Name of the fuel\n    :type fuel_name: str\n\n    :returns:\n        - **y_k** - A dict of mass fractions\n\n    '
             0.0
             1.0
             3.76
             'N2'
+            'O2'
             1
-            1.303794
-            0.303794
-         names      ('dict', 'MOLAR_MASSES')
-         varnames   ('phi', 'c_x', 'h_y', 'fuel_name', 'y_k', 'mass_mol_fuel', 'coeff_o2', 'y_o2_fuel_sto', 'y_air')
+         names      ('dict', 'far_stochio', 'MOLAR_MASSES', 'YO2_IN_AIR')
+         varnames   ('phi', 'c_x', 'h_y', 'fuel_name', 'y_k', 'afr_stochio', 'y_air')
          freevars   ()
          cellvars   ()
          filename   '/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py'
          name       'yk_from_phi'
-         firstlineno 55
+         firstlineno 62
          lnotab
-            0x02111c014201100126020c010c0202010201400108ff04ff04ff0c0516
-            0110011c02
+            0x02111c010c010c02260102010201400108ff04ff04ff0c06160120011a
+            02
       None
       ('fuel',)
-   names      ('__doc__', '__all__', 'MOLAR_MASSES', 'float', 'far_stochio', 'phi_from_far', 'far_from_phi', 'str', 'yk_from_phi')
+   names      ('__doc__', '__all__', 'YO2_IN_AIR', 'MOLAR_MASSES', 'float', 'far_stochio', 'phi_from_far', 'far_from_phi', 'str', 'yk_from_phi')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/dauptain/GITLAB/ms_thermo/src/ms_thermo/yk_from_phi.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff0201040408030e03140918111812
+   lnotab 0x00ff02010404080304020e03140e18111812
```

### Comparing `ms_thermo-0.3.7/src/ms_thermo/cli.py` & `ms_thermo-0.3.8/src/ms_thermo/cli.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/constants.py` & `ms_thermo-0.3.8/src/ms_thermo/constants.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/flame_params.py` & `ms_thermo-0.3.8/src/ms_thermo/flame_params.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/gasout.py` & `ms_thermo-0.3.8/src/ms_thermo/gasout.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/kero_prim2cons.py` & `ms_thermo-0.3.8/src/ms_thermo/kero_prim2cons.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/mixture_state.py` & `ms_thermo-0.3.8/src/ms_thermo/mixture_state.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/species.py` & `ms_thermo-0.3.8/src/ms_thermo/species.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/state.py` & `ms_thermo-0.3.8/src/ms_thermo/state.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/tadia.py` & `ms_thermo-0.3.8/src/ms_thermo/tadia.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/src/ms_thermo/yk_from_phi.py` & `ms_thermo-0.3.8/src/ms_thermo/yk_from_phi.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 """
 This script calculate mass_fraction of species from a Phi
 """
 
 __all__ = ["yk_from_phi", "phi_from_far"]
 
 
+YO2_IN_AIR = 0.2314
+
 MOLAR_MASSES =  {"C": 0.0120107, "H": 0.00100797, "O2": 0.0319988, "N2": 0.0280134}
 
 
 def far_stochio(c_x:float, h_y:float)-> float:
     """Return the fuel air ratio stoechiometric according to c_x h_y
     
     valid for AIR , not for PURE OXYGEN!!!
 
     BTW, the example in https://en.wikipedia.org/wiki/Air%E2%80%93fuel_ratio is for pure oxygen...
     """
     mass_mol_fuel = c_x * MOLAR_MASSES["C"] + h_y * MOLAR_MASSES["H"]
     coeff_o2 = c_x + (h_y / 4)
-    coef_air=1./0.2314
+    coef_air=1./YO2_IN_AIR
     afr_sto = coef_air*(coeff_o2 * MOLAR_MASSES["O2"]) / mass_mol_fuel
     far_sto = 1./afr_sto
     return far_sto
 
 def phi_from_far(far:float, c_x:float, h_y:float)-> float:
     """
-    *Return phi coefficient with the fuel air ratio coeff + fuel composition*
+    *Return phi coefficient with the fuel air ratio coeff + fuel composition (Valid for AIR, Not  PURE OXYGEN!!)**
 
     :param far: the air-fuel ratio
     :type far: float
     :param c_x: stoechio coeff of Carbone
     :type c_x: float
     :param h_y: stoechio coeff of hydrogene
     :type h_y: float
@@ -37,15 +39,15 @@
         - **phi** - Equivalence ratio
     """
     return  far /far_stochio(c_x, h_y)
 
 
 def far_from_phi(phi:float, c_x:float, h_y:float)-> float:
     """
-    *Return fuel air ratio coeff  with the phi coefficient + fuel composition*
+    *Return fuel air ratio coeff  with the phi coefficient + fuel composition (Valid for AIR, Not  PURE OXYGEN!!)*
 
     :param phi: eq. ratio coef
     :type far: float
     :param c_x: stoechio coeff of Carbone
     :type c_x: float
     :param h_y: stoechio coeff of hydrogene
     :type h_y: float
@@ -55,15 +57,15 @@
     """
     return phi * far_stochio(c_x, h_y)
 
 
 # use "fuel" here as default. Beware it important for pyavbp.
 def yk_from_phi(phi:float, c_x:float, h_y:float, fuel_name:str="fuel")-> float:
     """
-    *Return the species mass fractions in a fresh fuel-air mixture*
+    *Return the species mass fractions in a fresh fuel-air mixture (Valid for AIR, Not  PURE OXYGEN!!)*
 
     :param phi: equivalence ratio
     :type phi: float
     :param c_x: stoechio coeff of Carbone
     :type c_x: float
     :param h_y: stoechio coeff of hydrogene
     :type h_y: float
@@ -71,24 +73,22 @@
     :type fuel_name: str
 
     :returns:
         - **y_k** - A dict of mass fractions
 
     """
     y_k = dict()
-    mass_mol_fuel = c_x * MOLAR_MASSES["C"] + h_y * MOLAR_MASSES["H"]
-    coeff_o2 = c_x + (h_y / 4)
-    y_o2_fuel_sto = (coeff_o2 * MOLAR_MASSES["O2"]) / mass_mol_fuel
-
     if phi == 0.0:
         y_k[fuel_name] = 0.0
     else:
+        afr_stochio = 1./far_stochio(c_x, h_y)
         y_k[fuel_name] = 1.0 / (
             1.0
             + (1.0 + 3.76 * (MOLAR_MASSES["N2"] / MOLAR_MASSES["O2"]))
-            * (y_o2_fuel_sto / phi)
-        )
+            * (afr_stochio / phi)
+        )  # TNC Poinsot Veynante , pp 11-12
+
     y_air = 1 - y_k[fuel_name]
-    y_k["N2"] = y_air / 1.303794
-    y_k["O2"] = 0.303794 * y_k["N2"]
+    y_k["N2"] =(1-YO2_IN_AIR) * y_air
+    y_k["O2"] = YO2_IN_AIR * y_air
 
     return y_k
```

### Comparing `ms_thermo-0.3.7/src/ms_thermo.egg-info/PKG-INFO` & `ms_thermo-0.3.8/src/ms_thermo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-thermo
-Version: 0.3.7
+Version: 0.3.8
 Summary: Utilities to work on 2D and 3D structured grids
 Home-page: https://gitlab.com/cerfacs/ms_thermo
 Author: CoopTeam-CERFACS
 Author-email: coop@cerfacs.com
 Project-URL: Homepage, https://gitlab.com/cerfacs/ms_thermo
 Project-URL: Documentation, https://ms_thermo.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/cerfacs/ms_thermo/-/issues
```

### Comparing `ms_thermo-0.3.7/src/ms_thermo.egg-info/SOURCES.txt` & `ms_thermo-0.3.8/src/ms_thermo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/tests/test_compositions.py` & `ms_thermo-0.3.8/tests/test_compositions.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,11 +32,12 @@
     assert phi == 1.525253699761879 
 
 def test_ykfromphi():
     yf_methane = yk_from_phi(1.0, 1, 4, "CH4")["CH4"]
     yf_c3h8 = yk_from_phi(1.0, 3, 8, "C3H8")["C3H8"]
     yf_c8h18 = yk_from_phi(1.0, 8, 18, "C8H18")["C8H18"]
     yf_h2 = yk_from_phi(1.0, 0, 2, "H2")["H2"]
-    pytest.approx(yf_methane, 0.001) == 0.055
-    pytest.approx(yf_c3h8, 0.001) == 0.06
-    pytest.approx(yf_c8h18, 0.001) == 0.062
-    pytest.approx(yf_h2, 0.001) == 0.028
+    
+    assert pytest.approx(yf_methane, 0.00001) == 0.01333564942487222
+    assert pytest.approx(yf_c3h8, 0.00001) == 0.014642729952608102
+    assert pytest.approx(yf_c8h18, 0.00001) == 0.015164593008774152
+    assert pytest.approx(yf_h2, 0.00001) ==  0.006747884056174038
```

### Comparing `ms_thermo-0.3.7/tests/test_mixture_state.py` & `ms_thermo-0.3.8/tests/test_mixture_state.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.7/tests/test_state.py` & `ms_thermo-0.3.8/tests/test_state.py`

 * *Files identical despite different names*

