# Comparing `tmp/ms_thermo-0.3.6.tar.gz` & `tmp/ms_thermo-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_thermo-0.3.6.tar", last modified: Thu Mar 16 10:04:03 2023, max compression
+gzip compressed data, was "ms_thermo-0.3.7.tar", last modified: Wed Jul 26 11:00:47 2023, max compression
```

## Comparing `ms_thermo-0.3.6.tar` & `ms_thermo-0.3.7.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-03-16 10:04:03.363439 ms_thermo-0.3.6/
--rw-r--r--   0 dauptain   (502) staff       (20)     1611 2022-06-27 11:42:00.000000 ms_thermo-0.3.6/LICENSE
--rw-r--r--   0 dauptain   (502) staff       (20)        9 2022-06-27 11:42:00.000000 ms_thermo-0.3.6/MANIFEST.in
--rw-r--r--   0 dauptain   (502) staff       (20)     3910 2023-03-16 10:04:03.363703 ms_thermo-0.3.6/PKG-INFO
--rw-r--r--   0 dauptain   (502) staff       (20)     3087 2023-03-16 08:41:04.000000 ms_thermo-0.3.6/README.md
--rw-r--r--   0 dauptain   (502) staff       (20)     1425 2023-03-16 10:04:03.365066 ms_thermo-0.3.6/setup.cfg
--rw-r--r--   0 dauptain   (502) staff       (20)       39 2022-06-27 11:42:00.000000 ms_thermo-0.3.6/setup.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-03-16 10:04:03.326392 ms_thermo-0.3.6/src/
--rw-r--r--   0 dauptain   (502) staff       (20)     6148 2023-01-07 18:14:05.000000 ms_thermo-0.3.6/src/.DS_Store
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-03-16 10:04:03.334065 ms_thermo-0.3.6/src/ms_thermo/
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-03-16 10:04:03.348993 ms_thermo-0.3.6/src/ms_thermo/INPUT/
--rw-r--r--   0 dauptain   (502) staff       (20)    64672 2022-06-27 11:42:00.000000 ms_thermo-0.3.6/src/ms_thermo/INPUT/2S_KERO_BFER.h5
--rw-r--r--   0 dauptain   (502) staff       (20)   126263 2022-08-02 19:02:02.000000 ms_thermo-0.3.6/src/ms_thermo/INPUT/Luche1.cti
--rw-r--r--   0 dauptain   (502) staff       (20)       46 2022-06-27 11:42:00.000000 ms_thermo-0.3.6/src/ms_thermo/INPUT/__init__.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1501 2022-08-02 19:02:02.000000 ms_thermo-0.3.6/src/ms_thermo/INPUT/default_gasout_input.yml
--rw-r--r--   0 dauptain   (502) staff       (20)   140366 2022-06-27 11:42:00.000000 ms_thermo-0.3.6/src/ms_thermo/INPUT/species_database.dat
--rw-r--r--   0 dauptain   (502) staff       (20)       22 2023-03-16 09:23:17.000000 ms_thermo-0.3.6/src/ms_thermo/__init__.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-03-16 10:04:03.362789 ms_thermo-0.3.6/src/ms_thermo/__pycache__/
--rw-r--r--   0 dauptain   (502) staff       (20)      171 2023-03-16 08:00:03.000000 ms_thermo-0.3.6/src/ms_thermo/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     2103 2023-03-16 08:00:03.000000 ms_thermo-0.3.6/src/ms_thermo/__pycache__/constants.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     5453 2023-03-16 08:36:59.000000 ms_thermo-0.3.6/src/ms_thermo/__pycache__/flame_params.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    10431 2023-03-16 08:41:17.000000 ms_thermo-0.3.6/src/ms_thermo/__pycache__/gasout.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     1113 2023-03-16 09:18:37.000000 ms_thermo-0.3.6/src/ms_thermo/__pycache__/kero_prim2cons.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    12936 2023-03-16 08:07:49.000000 ms_thermo-0.3.6/src/ms_thermo/__pycache__/mixture_state.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    16044 2023-03-16 08:00:03.000000 ms_thermo-0.3.6/src/ms_thermo/__pycache__/species.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)    18355 2023-03-16 08:00:03.000000 ms_thermo-0.3.6/src/ms_thermo/__pycache__/state.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     3540 2023-03-16 09:18:38.000000 ms_thermo-0.3.6/src/ms_thermo/__pycache__/tadia.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     1862 2023-03-16 09:15:32.000000 ms_thermo-0.3.6/src/ms_thermo/__pycache__/yk_from_phi.cpython-39.pyc
--rw-r--r--   0 dauptain   (502) staff       (20)     7526 2023-03-16 08:51:56.000000 ms_thermo-0.3.6/src/ms_thermo/cli.py
--rw-r--r--   0 dauptain   (502) staff       (20)     3102 2022-06-27 11:42:00.000000 ms_thermo-0.3.6/src/ms_thermo/constants.py
--rw-r--r--   0 dauptain   (502) staff       (20)     6809 2022-06-27 11:42:00.000000 ms_thermo-0.3.6/src/ms_thermo/flame_params.py
--rw-r--r--   0 dauptain   (502) staff       (20)    13004 2023-03-16 08:41:04.000000 ms_thermo-0.3.6/src/ms_thermo/gasout.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1003 2022-08-02 19:02:02.000000 ms_thermo-0.3.6/src/ms_thermo/kero_prim2cons.py
--rw-r--r--   0 dauptain   (502) staff       (20)    13167 2023-03-16 08:07:45.000000 ms_thermo-0.3.6/src/ms_thermo/mixture_state.py
--rw-r--r--   0 dauptain   (502) staff       (20)    18061 2022-10-17 15:49:58.000000 ms_thermo-0.3.6/src/ms_thermo/species.py
--rw-r--r--   0 dauptain   (502) staff       (20)    19756 2022-08-02 19:02:02.000000 ms_thermo-0.3.6/src/ms_thermo/state.py
--rw-r--r--   0 dauptain   (502) staff       (20)     4218 2022-08-02 19:02:02.000000 ms_thermo-0.3.6/src/ms_thermo/tadia.py
--rw-r--r--   0 dauptain   (502) staff       (20)     1937 2023-03-16 09:19:30.000000 ms_thermo-0.3.6/src/ms_thermo/yk_from_phi.py
-drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-03-16 10:04:03.340486 ms_thermo-0.3.6/src/ms_thermo.egg-info/
--rw-r--r--   0 dauptain   (502) staff       (20)     3910 2023-03-16 10:04:02.000000 ms_thermo-0.3.6/src/ms_thermo.egg-info/PKG-INFO
--rw-r--r--   0 dauptain   (502) staff       (20)     1308 2023-03-16 10:04:03.000000 ms_thermo-0.3.6/src/ms_thermo.egg-info/SOURCES.txt
--rw-r--r--   0 dauptain   (502) staff       (20)        1 2023-03-16 10:04:02.000000 ms_thermo-0.3.6/src/ms_thermo.egg-info/dependency_links.txt
--rw-r--r--   0 dauptain   (502) staff       (20)      295 2023-03-16 10:04:02.000000 ms_thermo-0.3.6/src/ms_thermo.egg-info/entry_points.txt
--rw-r--r--   0 dauptain   (502) staff       (20)        1 2022-06-27 12:25:37.000000 ms_thermo-0.3.6/src/ms_thermo.egg-info/not-zip-safe
--rw-r--r--   0 dauptain   (502) staff       (20)      111 2023-03-16 10:04:02.000000 ms_thermo-0.3.6/src/ms_thermo.egg-info/requires.txt
--rw-r--r--   0 dauptain   (502) staff       (20)       10 2023-03-16 10:04:02.000000 ms_thermo-0.3.6/src/ms_thermo.egg-info/top_level.txt
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.622903 ms_thermo-0.3.7/
+-rw-r--r--   0 dauptain   (502) staff       (20)     1611 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/LICENSE
+-rw-r--r--   0 dauptain   (502) staff       (20)        9 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/MANIFEST.in
+-rw-r--r--   0 dauptain   (502) staff       (20)     3910 2023-07-26 11:00:47.623019 ms_thermo-0.3.7/PKG-INFO
+-rw-r--r--   0 dauptain   (502) staff       (20)     3087 2023-07-11 08:41:34.000000 ms_thermo-0.3.7/README.md
+-rw-r--r--   0 dauptain   (502) staff       (20)     1423 2023-07-26 11:00:47.623789 ms_thermo-0.3.7/setup.cfg
+-rw-r--r--   0 dauptain   (502) staff       (20)       39 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/setup.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.602871 ms_thermo-0.3.7/src/
+-rw-r--r--   0 dauptain   (502) staff       (20)     6148 2023-01-07 18:14:05.000000 ms_thermo-0.3.7/src/.DS_Store
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.608629 ms_thermo-0.3.7/src/ms_thermo/
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.614124 ms_thermo-0.3.7/src/ms_thermo/INPUT/
+-rw-r--r--   0 dauptain   (502) staff       (20)    64672 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/src/ms_thermo/INPUT/2S_KERO_BFER.h5
+-rw-r--r--   0 dauptain   (502) staff       (20)   126263 2022-08-02 19:02:02.000000 ms_thermo-0.3.7/src/ms_thermo/INPUT/Luche1.cti
+-rw-r--r--   0 dauptain   (502) staff       (20)       46 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/src/ms_thermo/INPUT/__init__.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1501 2022-08-02 19:02:02.000000 ms_thermo-0.3.7/src/ms_thermo/INPUT/default_gasout_input.yml
+-rw-r--r--   0 dauptain   (502) staff       (20)   140366 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/src/ms_thermo/INPUT/species_database.dat
+-rw-r--r--   0 dauptain   (502) staff       (20)       22 2023-07-26 09:56:31.000000 ms_thermo-0.3.7/src/ms_thermo/__init__.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.620092 ms_thermo-0.3.7/src/ms_thermo/__pycache__/
+-rw-r--r--   0 dauptain   (502) staff       (20)      187 2023-07-11 08:43:50.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3933 2023-07-11 08:43:51.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/constants.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     9524 2023-07-11 08:43:51.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/flame_params.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    16092 2023-07-11 08:43:51.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/gasout.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     1473 2023-07-26 09:35:53.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/kero_prim2cons.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    18559 2023-07-11 12:13:39.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/mixture_state.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    26357 2023-07-11 08:43:51.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/species.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)    25645 2023-07-11 08:49:39.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     5064 2023-07-11 12:13:39.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/tadia.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     3387 2023-07-26 09:11:05.000000 ms_thermo-0.3.7/src/ms_thermo/__pycache__/yk_from_phi.cpython-311.pyc
+-rw-r--r--   0 dauptain   (502) staff       (20)     7526 2023-07-11 08:41:34.000000 ms_thermo-0.3.7/src/ms_thermo/cli.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     3102 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/src/ms_thermo/constants.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     6809 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/src/ms_thermo/flame_params.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    13004 2023-07-11 08:41:34.000000 ms_thermo-0.3.7/src/ms_thermo/gasout.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     1003 2022-08-02 19:02:02.000000 ms_thermo-0.3.7/src/ms_thermo/kero_prim2cons.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    13167 2023-07-11 08:41:34.000000 ms_thermo-0.3.7/src/ms_thermo/mixture_state.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    18061 2022-10-17 15:49:58.000000 ms_thermo-0.3.7/src/ms_thermo/species.py
+-rw-r--r--   0 dauptain   (502) staff       (20)    19842 2023-07-11 08:49:31.000000 ms_thermo-0.3.7/src/ms_thermo/state.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     4218 2022-08-02 19:02:02.000000 ms_thermo-0.3.7/src/ms_thermo/tadia.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     2633 2023-07-26 10:00:57.000000 ms_thermo-0.3.7/src/ms_thermo/yk_from_phi.py
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.611263 ms_thermo-0.3.7/src/ms_thermo.egg-info/
+-rw-r--r--   0 dauptain   (502) staff       (20)     3910 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/PKG-INFO
+-rw-r--r--   0 dauptain   (502) staff       (20)     1442 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/SOURCES.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)        1 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/dependency_links.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)      295 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/entry_points.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)        1 2022-06-27 12:25:37.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/not-zip-safe
+-rw-r--r--   0 dauptain   (502) staff       (20)      109 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/requires.txt
+-rw-r--r--   0 dauptain   (502) staff       (20)       10 2023-07-26 11:00:47.000000 ms_thermo-0.3.7/src/ms_thermo.egg-info/top_level.txt
+drwxr-xr-x   0 dauptain   (502) staff       (20)        0 2023-07-26 11:00:47.622460 ms_thermo-0.3.7/tests/
+-rw-r--r--   0 dauptain   (502) staff       (20)     1209 2023-07-26 09:54:05.000000 ms_thermo-0.3.7/tests/test_compositions.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      385 2022-08-02 19:02:02.000000 ms_thermo-0.3.7/tests/test_kero_prim2cons.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     2463 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/tests/test_mixture_state.py
+-rw-r--r--   0 dauptain   (502) staff       (20)     8108 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/tests/test_state.py
+-rw-r--r--   0 dauptain   (502) staff       (20)      423 2022-06-27 11:42:00.000000 ms_thermo-0.3.7/tests/test_tadia.py
```

### Comparing `ms_thermo-0.3.6/LICENSE` & `ms_thermo-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/PKG-INFO` & `ms_thermo-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms_thermo
-Version: 0.3.6
+Version: 0.3.7
 Summary: Utilities to work on 2D and 3D structured grids
 Home-page: https://gitlab.com/cerfacs/ms_thermo
 Author: CoopTeam-CERFACS
 Author-email: coop@cerfacs.com
 Project-URL: Homepage, https://gitlab.com/cerfacs/ms_thermo
 Project-URL: Documentation, https://ms_thermo.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/cerfacs/ms_thermo/-/issues
```

### Comparing `ms_thermo-0.3.6/README.md` & `ms_thermo-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/setup.cfg` & `ms_thermo-0.3.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >= 3.7
 install_requires = 
 	numpy<2
-	scipy<2
+	scipy
 	h5py
 	PyYAML
 	click
 	h5cross
 zip_safe = False
 include_package_data = True
```

### Comparing `ms_thermo-0.3.6/src/.DS_Store` & `ms_thermo-0.3.7/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/INPUT/2S_KERO_BFER.h5` & `ms_thermo-0.3.7/src/ms_thermo/INPUT/2S_KERO_BFER.h5`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/INPUT/Luche1.cti` & `ms_thermo-0.3.7/src/ms_thermo/INPUT/Luche1.cti`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/INPUT/default_gasout_input.yml` & `ms_thermo-0.3.7/src/ms_thermo/INPUT/default_gasout_input.yml`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/INPUT/species_database.dat` & `ms_thermo-0.3.7/src/ms_thermo/INPUT/species_database.dat`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/__pycache__/kero_prim2cons.cpython-39.pyc` & `ms_thermo-0.3.7/src/ms_thermo/__pycache__/kero_prim2cons.cpython-311.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Aug  2 19:02:02 2022 UTC, .py size: 1003 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,93 @@
-00000000: 610d 0d0a 0000 0000 aa74 e962 eb03 0000  a........t.b....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0002 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6403 6701 5a04 6404 6403  m.Z...d.g.Z.d.d.
-00000050: 8400 5a05 6405 5300 2906 e900 0000 0029  ..Z.d.S.)......)
-00000060: 01da 0553 7461 7465 2901 da0b 796b 5f66  ...State)...yk_f
-00000070: 726f 6d5f 7068 69da 0e6b 6572 6f5f 7072  rom_phi..kero_pr
-00000080: 696d 3263 6f6e 7363 0300 0000 0000 0000  im2consc........
-00000090: 0000 0000 0900 0000 0500 0000 4300 0000  ............C...
-000000a0: 7362 0000 0074 007c 0264 0164 0264 0383  sb...t.|.d.d.d..
-000000b0: 047d 0374 0164 047c 007c 017c 0383 047d  .}.t.d.|.|.|...}
-000000c0: 047c 046a 027d 057c 046a 027c 046a 0314  .|.j.}.|.j.|.j..
-000000d0: 007d 0674 0483 007d 077c 046a 05a0 06a1  .}.t...}.|.j....
-000000e0: 0044 005d 187d 087c 046a 027c 046a 057c  .D.].}.|.j.|.j.|
-000000f0: 0819 0014 007c 077c 083c 0071 3e7c 057c  .....|.|.<.q>|.|
-00000100: 067c 0766 0353 0029 0561 f701 0000 0a20  .|.f.S.).a..... 
-00000110: 2020 2043 6f6d 7075 7465 2063 6f6e 7365     Compute conse
-00000120: 7276 6174 6976 6520 7661 7269 6162 6c65  rvative variable
-00000130: 7320 6672 6f6d 2070 7269 6d69 7469 7665  s from primitive
-00000140: 2076 6172 6961 626c 6573 2069 6e20 6120   variables in a 
-00000150: 6b65 726f 7365 6e65 2d61 6972 206d 6978  kerosene-air mix
-00000160: 7475 7265 2e0a 0a20 2020 203a 7061 7261  ture...    :para
-00000170: 6d20 7465 6d70 6572 6174 7572 653a 2074  m temperature: t
-00000180: 6865 2066 7265 7368 2067 6173 2074 656d  he fresh gas tem
-00000190: 7065 7261 7475 7265 0a20 2020 203a 7479  perature.    :ty
-000001a0: 7065 2074 656d 7065 7261 7475 7265 3a20  pe temperature: 
-000001b0: 666c 6f61 740a 2020 2020 3a70 6172 616d  float.    :param
-000001c0: 2070 7265 7373 7572 653a 2070 7265 7373   pressure: press
-000001d0: 7572 6520 6f66 2074 6865 2066 7265 7368  ure of the fresh
-000001e0: 2067 6173 0a20 2020 203a 7479 7065 2070   gas.    :type p
-000001f0: 7265 7373 7572 653a 2066 6c6f 6174 0a20  ressure: float. 
-00000200: 2020 203a 7061 7261 6d20 7068 693a 2065     :param phi: e
-00000210: 7175 6976 616c 656e 6365 2072 6174 696f  quivalence ratio
-00000220: 206f 6620 7468 6520 6169 722d 6675 656c   of the air-fuel
-00000230: 206d 6978 7475 7265 0a20 2020 203a 7479   mixture.    :ty
-00000240: 7065 2070 6869 3a20 666c 6f61 740a 2020  pe phi: float.  
-00000250: 2020 3a70 6172 616d 2066 7565 6c3a 2066    :param fuel: f
-00000260: 7565 6c0a 2020 2020 3a74 7970 6520 6675  uel.    :type fu
-00000270: 656c 3a20 7374 7269 6e67 0a0a 2020 2020  el: string..    
-00000280: 3a72 6574 7572 6e73 3a0a 2020 2020 092d  :returns:.    .-
-00000290: 202a 2a72 686f 2a2a 202d 2044 656e 7369   **rho** - Densi
-000002a0: 7479 0a20 2020 2009 2d20 2a2a 7268 6f45  ty.    .- **rhoE
-000002b0: 2a2a 202d 2043 6f6e 7365 7276 6174 6976  ** - Conservativ
-000002c0: 6520 656e 6572 6779 0a20 2020 2009 2d20  e energy.    .- 
-000002d0: 2a2a 7268 6f79 6b2a 2a20 2d20 4469 6374  **rhoyk** - Dict
-000002e0: 206f 6620 636f 6e73 6572 7661 7469 7665   of conservative
-000002f0: 206d 6173 7320 6672 6163 7469 6f6e 730a   mass fractions.
-00000300: 0a20 2020 20e9 0a00 0000 e916 0000 005a  .    ..........Z
-00000310: 044b 4552 4f4e 2907 7203 0000 0072 0200  .KERON).r....r..
-00000320: 0000 da03 7268 6f5a 0665 6e65 7267 79da  ....rhoZ.energy.
-00000330: 0464 6963 745a 045f 795f 6bda 046b 6579  .dictZ._y_k..key
-00000340: 7329 095a 0b74 656d 7065 7261 7475 7265  s).Z.temperature
-00000350: 5a08 7072 6573 7375 7265 da03 7068 695a  Z.pressure..phiZ
-00000360: 0279 6b5a 0367 6173 7207 0000 00da 0472  .ykZ.gasr......r
-00000370: 686f 455a 0572 686f 796b 5a06 7370 6563  hoEZ.rhoykZ.spec
-00000380: 6965 a900 720c 0000 00fa 402f 5573 6572  ie..r.....@/User
-00000390: 732f 6461 7570 7461 696e 2f47 4954 4c41  s/dauptain/GITLA
-000003a0: 422f 6d73 5f74 6865 726d 6f2f 7372 632f  B/ms_thermo/src/
-000003b0: 6d73 5f74 6865 726d 6f2f 6b65 726f 5f70  ms_thermo/kero_p
-000003c0: 7269 6d32 636f 6e73 2e70 7972 0400 0000  rim2cons.pyr....
-000003d0: 0700 0000 7310 0000 0000 130e 020e 0106  ....s...........
-000003e0: 010c 0106 010e 0116 014e 2906 5a0f 6d73  .........N).Z.ms
-000003f0: 5f74 6865 726d 6f2e 7374 6174 6572 0200  _thermo.stater..
-00000400: 0000 da15 6d73 5f74 6865 726d 6f2e 796b  ....ms_thermo.yk
-00000410: 5f66 726f 6d5f 7068 6972 0300 0000 da07  _from_phir......
-00000420: 5f5f 616c 6c5f 5f72 0400 0000 720c 0000  __all__r....r...
-00000430: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000440: da08 3c6d 6f64 756c 653e 0100 0000 7306  ..<module>....s.
-00000450: 0000 000c 010c 0206 03                   .........
+00000000: a70d 0d0a 0000 0000 aa74 e962 eb03 0000  .........t.b....
+00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
+00000020: 0000 0000 00f3 2a00 0000 9700 6400 6401  ......*.....d.d.
+00000030: 6c00 6d01 5a01 0100 6400 6402 6c02 6d03  l.m.Z...d.d.l.m.
+00000040: 5a03 0100 6403 6701 5a04 6404 8400 5a05  Z...d.g.Z.d...Z.
+00000050: 6405 5300 2906 e900 0000 0029 01da 0553  d.S.)......)...S
+00000060: 7461 7465 2901 da0b 796b 5f66 726f 6d5f  tate)...yk_from_
+00000070: 7068 69da 0e6b 6572 6f5f 7072 696d 3263  phi..kero_prim2c
+00000080: 6f6e 7363 0300 0000 0000 0000 0000 0000  onsc............
+00000090: 0600 0000 0300 0000 f304 0100 0097 0074  ...............t
+000000a0: 0100 0000 0000 0000 0000 007c 0264 0164  ...........|.d.d
+000000b0: 0264 03a6 0400 00ab 0400 0000 0000 0000  .d..............
+000000c0: 007d 0374 0300 0000 0000 0000 0000 0064  .}.t...........d
+000000d0: 047c 007c 017c 03a6 0400 00ab 0400 0000  .|.|.|..........
+000000e0: 0000 0000 007d 047c 046a 0200 0000 0000  .....}.|.j......
+000000f0: 0000 007d 057c 046a 0200 0000 0000 0000  ...}.|.j........
+00000100: 007c 046a 0300 0000 0000 0000 007a 0500  .|.j.........z..
+00000110: 007d 0674 0900 0000 0000 0000 0000 00a6  .}.t............
+00000120: 0000 00ab 0000 0000 0000 0000 007d 077c  .............}.|
+00000130: 046a 0500 0000 0000 0000 00a0 0600 0000  .j..............
+00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000150: 00a6 0000 00ab 0000 0000 0000 0000 0044  ...............D
+00000160: 005d 1a7d 087c 046a 0200 0000 0000 0000  .].}.|.j........
+00000170: 007c 046a 0500 0000 0000 0000 007c 0819  .|.j.........|..
+00000180: 0000 0000 0000 0000 007a 0500 007c 077c  .........z...|.|
+00000190: 083c 0000 008c 1b7c 057c 067c 0766 0353  .<.....|.|.|.f.S
+000001a0: 0029 0561 f701 0000 0a20 2020 2043 6f6d  .).a.....    Com
+000001b0: 7075 7465 2063 6f6e 7365 7276 6174 6976  pute conservativ
+000001c0: 6520 7661 7269 6162 6c65 7320 6672 6f6d  e variables from
+000001d0: 2070 7269 6d69 7469 7665 2076 6172 6961   primitive varia
+000001e0: 626c 6573 2069 6e20 6120 6b65 726f 7365  bles in a kerose
+000001f0: 6e65 2d61 6972 206d 6978 7475 7265 2e0a  ne-air mixture..
+00000200: 0a20 2020 203a 7061 7261 6d20 7465 6d70  .    :param temp
+00000210: 6572 6174 7572 653a 2074 6865 2066 7265  erature: the fre
+00000220: 7368 2067 6173 2074 656d 7065 7261 7475  sh gas temperatu
+00000230: 7265 0a20 2020 203a 7479 7065 2074 656d  re.    :type tem
+00000240: 7065 7261 7475 7265 3a20 666c 6f61 740a  perature: float.
+00000250: 2020 2020 3a70 6172 616d 2070 7265 7373      :param press
+00000260: 7572 653a 2070 7265 7373 7572 6520 6f66  ure: pressure of
+00000270: 2074 6865 2066 7265 7368 2067 6173 0a20   the fresh gas. 
+00000280: 2020 203a 7479 7065 2070 7265 7373 7572     :type pressur
+00000290: 653a 2066 6c6f 6174 0a20 2020 203a 7061  e: float.    :pa
+000002a0: 7261 6d20 7068 693a 2065 7175 6976 616c  ram phi: equival
+000002b0: 656e 6365 2072 6174 696f 206f 6620 7468  ence ratio of th
+000002c0: 6520 6169 722d 6675 656c 206d 6978 7475  e air-fuel mixtu
+000002d0: 7265 0a20 2020 203a 7479 7065 2070 6869  re.    :type phi
+000002e0: 3a20 666c 6f61 740a 2020 2020 3a70 6172  : float.    :par
+000002f0: 616d 2066 7565 6c3a 2066 7565 6c0a 2020  am fuel: fuel.  
+00000300: 2020 3a74 7970 6520 6675 656c 3a20 7374    :type fuel: st
+00000310: 7269 6e67 0a0a 2020 2020 3a72 6574 7572  ring..    :retur
+00000320: 6e73 3a0a 2020 2020 092d 202a 2a72 686f  ns:.    .- **rho
+00000330: 2a2a 202d 2044 656e 7369 7479 0a20 2020  ** - Density.   
+00000340: 2009 2d20 2a2a 7268 6f45 2a2a 202d 2043   .- **rhoE** - C
+00000350: 6f6e 7365 7276 6174 6976 6520 656e 6572  onservative ener
+00000360: 6779 0a20 2020 2009 2d20 2a2a 7268 6f79  gy.    .- **rhoy
+00000370: 6b2a 2a20 2d20 4469 6374 206f 6620 636f  k** - Dict of co
+00000380: 6e73 6572 7661 7469 7665 206d 6173 7320  nservative mass 
+00000390: 6672 6163 7469 6f6e 730a 0a20 2020 20e9  fractions..    .
+000003a0: 0a00 0000 e916 0000 00da 044b 4552 4f4e  ...........KERON
+000003b0: 2907 7204 0000 0072 0300 0000 da03 7268  ).r....r......rh
+000003c0: 6fda 0665 6e65 7267 79da 0464 6963 74da  o..energy..dict.
+000003d0: 045f 795f 6bda 046b 6579 7329 09da 0b74  ._y_k..keys)...t
+000003e0: 656d 7065 7261 7475 7265 da08 7072 6573  emperature..pres
+000003f0: 7375 7265 da03 7068 69da 0279 6bda 0367  sure..phi..yk..g
+00000400: 6173 720a 0000 00da 0472 686f 45da 0572  asr......rhoE..r
+00000410: 686f 796b da06 7370 6563 6965 7309 0000  hoyk..species...
+00000420: 0020 2020 2020 2020 2020 fa40 2f55 7365  .         .@/Use
+00000430: 7273 2f64 6175 7074 6169 6e2f 4749 544c  rs/dauptain/GITL
+00000440: 4142 2f6d 735f 7468 6572 6d6f 2f73 7263  AB/ms_thermo/src
+00000450: 2f6d 735f 7468 6572 6d6f 2f6b 6572 6f5f  /ms_thermo/kero_
+00000460: 7072 696d 3263 6f6e 732e 7079 7205 0000  prim2cons.pyr...
+00000470: 0072 0500 0000 0700 0000 7387 0000 0080  .r........s.....
+00000480: 00f5 2600 0a15 9053 9822 9862 a026 d109  ..&....S.".b.&..
+00000490: 29d4 0929 8042 e50a 0f90 0490 6ba0 38a8  )..).B......k.8.
+000004a0: 52d1 0a30 d40a 3080 43d8 0a0d 8c27 8043  R..0..0.C....'.C
+000004b0: d80b 0e8c 3790 5394 5ad1 0b1f 8044 dd0c  ....7.S.Z....D..
+000004c0: 1089 468c 4680 45d8 1215 9428 972d 922d  ..F.F.E....(.-.-
+000004d0: 912f 942f f000 0105 33f0 0001 0533 8806  ././....3....3..
+000004e0: d818 1b9c 07a0 23a4 28a8 36d4 2232 d118  ......#.(.6."2..
+000004f0: 3288 0588 6689 0d88 0dd8 0b0e 9004 9065  2...f..........e
+00000500: d00b 1bd0 041b f300 0000 004e 2906 da0f  ...........N)...
+00000510: 6d73 5f74 6865 726d 6f2e 7374 6174 6572  ms_thermo.stater
+00000520: 0300 0000 da15 6d73 5f74 6865 726d 6f2e  ......ms_thermo.
+00000530: 796b 5f66 726f 6d5f 7068 6972 0400 0000  yk_from_phir....
+00000540: da07 5f5f 616c 6c5f 5f72 0500 0000 a900  ..__all__r......
+00000550: 7218 0000 0072 1700 0000 fa08 3c6d 6f64  r....r......<mod
+00000560: 756c 653e 721d 0000 0001 0000 0073 4a00  ule>r........sJ.
+00000570: 0000 f003 0101 01d8 0021 d000 21d0 0021  .........!..!..!
+00000580: d000 21d0 0021 d000 21d8 002d d000 2dd0  ..!..!..!..-..-.
+00000590: 002d d000 2dd0 002d d000 2de0 0b1b d00a  .-..-..-..-.....
+000005a0: 1c80 07f0 061b 011c f000 1b01 1cf0 001b  ................
+000005b0: 011c f000 1b01 1cf0 001b 011c 7218 0000  ............r...
+000005c0: 00                                       .
```

### Comparing `ms_thermo-0.3.6/src/ms_thermo/__pycache__/state.cpython-39.pyc` & `ms_thermo-0.3.7/src/ms_thermo/__pycache__/gasout.cpython-311.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Aug  2 19:02:02 2022 UTC, .py size: 19756 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,1148 +1,1006 @@
-00000000: 610d 0d0a 0000 0000 aa74 e962 2c4d 0000  a........t.b,M..
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 6800 0000 6400  .....@...sh...d.
-00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
-00000040: 5a03 6401 6403 6c04 6d05 5a05 0100 6401  Z.d.d.l.m.Z...d.
-00000050: 6404 6c06 6d07 5a07 0100 6401 6405 6c08  d.l.m.Z...d.d.l.
-00000060: 6d09 5a09 0100 6401 6406 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
-00000070: 6d0c 5a0c 0100 6401 6402 6c0d 5a0d 6407  m.Z...d.d.l.Z.d.
-00000080: 6701 5a0e 4700 6408 6407 8400 6407 8302  g.Z.G.d.d...d...
-00000090: 5a0f 6402 5300 2909 6169 0800 000a 6060  Z.d.S.).ai....``
-000000a0: 5374 6174 6560 6020 6973 2061 6e20 6f62  State`` is an ob
-000000b0: 6a65 6374 2068 616e 646c 696e 6720 7468  ject handling th
-000000c0: 6520 696e 7465 726e 616c 2073 7461 7465  e internal state
-000000d0: 206f 6620 6120 6761 7365 6f75 7320 6d69   of a gaseous mi
-000000e0: 7874 7572 652c 206e 616d 656c 793a 0a0a  xture, namely:..
-000000f0: 2d20 4465 6e73 6974 790a 2d20 546f 7461  - Density.- Tota
-00000100: 6c20 656e 6572 6779 0a2d 2053 7065 6369  l energy.- Speci
-00000110: 6573 206d 6173 7320 6672 6163 7469 6f6e  es mass fraction
-00000120: 730a 0a4c 696d 6974 6174 696f 6e73 206f  s..Limitations o
-00000130: 6620 7468 6520 6060 5374 6174 6560 6020  f the ``State`` 
-00000140: 6f62 6a65 6374 0a3d 3d3d 3d3d 3d3d 3d3d  object.=========
-00000150: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000160: 3d3d 3d3d 3d3d 3d3d 3d3d 0a2d 2056 656c  ==========.- Vel
-00000170: 6f63 6974 7920 6973 206e 6f74 2061 2070  ocity is not a p
-00000180: 726f 7065 7274 7920 6f66 2061 2060 6053  roperty of a ``S
-00000190: 7461 7465 6060 2061 6e64 206d 7573 7420  tate`` and must 
-000001a0: 6265 2074 7265 6174 6564 2073 6570 6172  be treated separ
-000001b0: 6174 656c 792e 0a2d 2054 6865 2073 7061  ately..- The spa
-000001c0: 7469 616c 2061 7370 6563 7473 2c20 692e  tial aspects, i.
-000001d0: 652e 2074 6865 2070 6f73 6974 696f 6e20  e. the position 
-000001e0: 6f66 2074 6865 2070 6f69 6e74 732c 206f  of the points, o
-000001f0: 7220 7468 6520 6d65 7368 2c20 6d75 7374  r the mesh, must
-00000200: 2062 6520 6861 6e64 6c65 6420 7365 7061   be handled sepa
-00000210: 7261 7465 6c79 2e0a 0a2e 2e20 7761 726e  rately..... warn
-00000220: 696e 673a 3a20 6060 5374 6174 6560 6020  ing:: ``State`` 
-00000230: 7661 7269 6162 6c65 7320 6172 6520 7265  variables are re
-00000240: 7072 6573 656e 7465 6420 6173 2073 7472  presented as str
-00000250: 7563 7475 7265 6420 6172 7261 7973 2074  uctured arrays t
-00000260: 6861 7420 6d75 7374 2068 6176 6520 7468  hat must have th
-00000270: 6520 2a73 616d 652a 2073 6861 7065 0a0a  e *same* shape..
-00000280: 496e 6974 6961 6c69 7a69 6e67 2061 2060  Initializing a `
-00000290: 6053 7461 7465 6060 0a3d 3d3d 3d3d 3d3d  `State``.=======
-000002a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000002b0: 3d0a 4120 6060 5374 6174 6560 6020 6f62  =.A ``State`` ob
-000002c0: 6a65 6374 2063 616e 2062 6520 696e 6974  ject can be init
-000002d0: 6961 6c69 7a65 6420 696e 2074 776f 2077  ialized in two w
-000002e0: 6179 733a 0a0a 2d20 4672 6f6d 2074 6865  ays:..- From the
-000002f0: 2074 656d 7065 7261 7475 7265 2c20 7072   temperature, pr
-00000300: 6573 7375 7265 2c20 616e 6420 7370 6563  essure, and spec
-00000310: 6965 7320 6d61 7373 2066 7261 6374 696f  ies mass fractio
-00000320: 6e73 203a 6d61 7468 3a60 2854 2c20 502c  ns :math:`(T, P,
-00000330: 2059 5f6b 2960 2074 6872 6f75 6768 2074   Y_k)` through t
-00000340: 6865 2064 6566 6175 6c74 2063 6f6e 7374  he default const
-00000350: 7275 6374 6f72 3a3a 0a0a 2020 2020 7374  ructor::..    st
-00000360: 6174 6520 3d20 5374 6174 6528 542c 2050  ate = State(T, P
-00000370: 2c20 596b 290a 0a2d 2046 726f 6d20 636f  , Yk)..- From co
-00000380: 6e73 6572 7661 7469 7665 2076 6172 6961  nservative varia
-00000390: 626c 6573 203a 6d61 7468 3a60 285c 7268  bles :math:`(\rh
-000003a0: 6f2c 205c 7268 6f20 452c 205c 7268 6f20  o, \rho E, \rho 
-000003b0: 595f 6b29 6020 7468 726f 7567 6820 7468  Y_k)` through th
-000003c0: 6520 6060 6672 6f6d 5f63 6f6e 7360 6020  e ``from_cons`` 
-000003d0: 636f 6e73 7472 7563 746f 723a 3a0a 0a20  constructor::.. 
-000003e0: 2020 2073 7461 7465 203d 2053 7461 7465     state = State
-000003f0: 2e66 726f 6d5f 636f 6e73 2872 686f 2c20  .from_cons(rho, 
-00000400: 7268 6f45 2c20 7268 6f59 6b29 0a0a 5468  rhoE, rhoYk)..Th
-00000410: 6520 636f 6e73 7472 7563 746f 7220 6172  e constructor ar
-00000420: 6775 6d65 6e74 7320 3a6d 6174 683a 6028  guments :math:`(
-00000430: 542c 2050 2c20 595f 6b29 6020 6f72 203a  T, P, Y_k)` or :
-00000440: 6d61 7468 3a60 285c 7268 6f2c 205c 7268  math:`(\rho, \rh
-00000450: 6f20 452c 205c 7268 6f20 595f 6b29 6020  o E, \rho Y_k)` 
-00000460: 6361 6e20 6265 2073 6361 6c61 7273 206f  can be scalars o
-00000470: 7220 6d75 6c74 6964 696d 656e 7369 6f6e  r multidimension
-00000480: 616c 2061 7272 6179 732e 0a0a 2e2e 2077  al arrays..... w
-00000490: 6172 6e69 6e67 3a3a 0a20 2020 2057 6865  arning::.    Whe
-000004a0: 6e20 696e 6974 6961 6c69 7a69 6e67 2066  n initializing f
-000004b0: 726f 6d20 636f 6e73 6572 7661 7469 7665  rom conservative
-000004c0: 2076 6172 6961 626c 6573 2c20 3a6d 6174   variables, :mat
-000004d0: 683a 6054 6020 6973 2064 6574 6572 6d69  h:`T` is determi
-000004e0: 6e65 6420 6279 2061 0a20 2020 204e 6577  ned by a.    New
-000004f0: 746f 6e2d 5261 7068 736f 6e20 6d65 7468  ton-Raphson meth
-00000500: 6f64 2074 6f20 656e 7375 7265 2074 6861  od to ensure tha
-00000510: 7420 7468 6520 6d69 7874 7572 6520 656e  t the mixture en
-00000520: 6572 6779 206d 6174 6368 6573 2074 6865  ergy matches the
-00000530: 2069 6e70 7574 2074 6f74 616c 2065 6e65   input total ene
-00000540: 7267 792e 0a20 2020 2054 6869 7320 6973  rgy..    This is
-00000550: 2061 6e20 2a2a 6578 7065 6e73 6976 652a   an **expensive*
-00000560: 2a20 7374 6570 2074 6861 7420 6d61 7920  * step that may 
-00000570: 7461 6b65 2061 206c 6f6e 6720 7469 6d65  take a long time
-00000580: 2066 6f72 206c 6172 6765 2069 6e70 7574   for large input
-00000590: 732e 0a0a 5472 616e 7366 6f72 6d69 6e67  s...Transforming
-000005a0: 2061 2060 6053 7461 7465 6060 0a3d 3d3d   a ``State``.===
-000005b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000005c0: 3d3d 3d3d 3d0a 4166 7465 7220 6120 6060  =====.After a ``
-000005d0: 5374 6174 6560 6020 6861 7320 6265 656e  State`` has been
-000005e0: 2069 6e69 7469 616c 697a 6564 2c20 3a6d   initialized, :m
-000005f0: 6174 683a 6054 602c 203a 6d61 7468 3a60  ath:`T`, :math:`
-00000600: 5060 2061 6e64 203a 6d61 7468 3a60 595f  P` and :math:`Y_
-00000610: 6b60 2063 616e 0a69 6e64 6570 656e 6465  k` can.independe
-00000620: 6e74 6c79 2062 6520 7365 7420 746f 206e  ntly be set to n
-00000630: 6577 2076 616c 7565 7320 2860 652e 672e  ew values (`e.g.
-00000640: 6020 6060 6d79 5374 6174 652e 7465 6d70  ` ``myState.temp
-00000650: 6572 6174 7572 6520 3d20 6e65 7754 656d  erature = newTem
-00000660: 7065 7261 7475 7265 6060 2920 616e 6420  perature``) and 
-00000670: 7468 6520 6f74 6865 7220 7374 6174 6520  the other state 
-00000680: 7661 7269 6162 6c65 7320 6172 6520 6d6f  variables are mo
-00000690: 6469 6669 6564 0a61 6363 6f72 6469 6e67  dified.according
-000006a0: 6c79 3a0a 0a2d 2057 6865 6e20 7365 7474  ly:..- When sett
-000006b0: 696e 6720 6120 6e65 7720 7661 6c75 6520  ing a new value 
-000006c0: 666f 7220 3a6d 6174 683a 6054 602c 2074  for :math:`T`, t
-000006d0: 6865 206f 7468 6572 2073 7461 7465 2076  he other state v
-000006e0: 6172 6961 626c 6573 2061 7265 206d 6f64  ariables are mod
-000006f0: 6966 6965 6420 6173 7375 6d69 6e67 2061  ified assuming a
-00000700: 6e20 2a2a 6973 6f62 6172 6963 2061 6e64  n **isobaric and
-00000710: 2069 736f 2d63 6f6d 706f 7369 7469 6f6e   iso-composition
-00000720: 2a2a 2074 7261 6e73 666f 726d 6174 696f  ** transformatio
-00000730: 6e20 6672 6f6d 2074 6865 2070 7265 7669  n from the previ
-00000740: 6f75 7320 7374 6174 652e 0a2d 2057 6865  ous state..- Whe
-00000750: 6e20 7365 7474 696e 6720 6120 6e65 7720  n setting a new 
-00000760: 7661 6c75 6520 666f 7220 3a6d 6174 683a  value for :math:
-00000770: 6050 602c 2074 6865 206f 7468 6572 2073  `P`, the other s
-00000780: 7461 7465 2076 6172 6961 626c 6573 2061  tate variables a
-00000790: 7265 206d 6f64 6966 6965 6420 6173 7375  re modified assu
-000007a0: 6d69 6e67 2061 6e20 2a2a 6973 6f74 6865  ming an **isothe
-000007b0: 726d 616c 2061 6e64 2069 736f 2d63 6f6d  rmal and iso-com
-000007c0: 706f 7369 7469 6f6e 2a2a 2074 7261 6e73  position** trans
-000007d0: 666f 726d 6174 696f 6e20 6672 6f6d 2074  formation from t
-000007e0: 6865 2070 7265 7669 6f75 7320 7374 6174  he previous stat
-000007f0: 652e 0a2d 2057 6865 6e20 7365 7474 696e  e..- When settin
-00000800: 6720 6120 6e65 7720 7661 6c75 6520 666f  g a new value fo
-00000810: 7220 3a6d 6174 683a 6059 5f6b 602c 2074  r :math:`Y_k`, t
-00000820: 6865 206f 7468 6572 2073 7461 7465 2076  he other state v
-00000830: 6172 6961 626c 6573 2061 7265 206d 6f64  ariables are mod
-00000840: 6966 6965 6420 6173 7375 6d69 6e67 2061  ified assuming a
-00000850: 6e20 2a2a 6973 6f74 6865 726d 616c 2061  n **isothermal a
-00000860: 6e64 2069 736f 6261 7269 632a 2a20 7472  nd isobaric** tr
-00000870: 616e 7366 6f72 6d61 7469 6f6e 2066 726f  ansformation fro
-00000880: 6d20 7468 6520 7072 6576 696f 7573 2073  m the previous s
-00000890: 7461 7465 2e0a 0a53 7461 7465 2074 7261  tate...State tra
-000008a0: 6e73 666f 726d 6174 696f 6e73 2061 6c77  nsformations alw
-000008b0: 6179 7320 7361 7469 7366 7920 7468 6520  ays satisfy the 
-000008c0: 7065 7266 6563 7420 6761 7320 6571 7561  perfect gas equa
-000008d0: 7469 6f6e 206f 6620 7374 6174 650a 0a2e  tion of state...
-000008e0: 2e20 6d61 7468 3a3a 2050 203d 205c 7268  . math:: P = \rh
-000008f0: 6f20 5c66 7261 637b 527d 7b57 5f7b 6d69  o \frac{R}{W_{mi
-00000900: 787d 7d20 540a e900 0000 004e 2901 da06  x}} T......N)...
-00000910: 6e65 7774 6f6e 2901 da04 6d6f 6465 2901  newton)...mode).
-00000920: da16 6275 696c 645f 7468 6572 6d6f 5f66  ..build_thermo_f
-00000930: 726f 6d5f 6176 6270 2902 da07 4741 535f  rom_avbp)...GAS_
-00000940: 4353 54da 0e41 544f 4d49 435f 5745 4947  CST..ATOMIC_WEIG
-00000950: 4854 53da 0553 7461 7465 6300 0000 0000  HTS..Statec.....
-00000960: 0000 0000 0000 0000 0000 0004 0000 0040  ...............@
-00000970: 0000 0073 3201 0000 6500 5a01 6400 5a02  ...s2...e.Z.d.Z.
-00000980: 6401 5a03 643c 6405 6406 8401 5a04 6407  d.Z.d<d.d...Z.d.
-00000990: 6408 8400 5a05 6506 643d 6409 640a 8401  d...Z.e.d=d.d...
-000009a0: 8301 5a07 6508 640b 640c 8400 8301 5a09  ..Z.e.d.d.....Z.
-000009b0: 6509 6a0a 640d 640c 8400 8301 5a09 6508  e.j.d.d.....Z.e.
-000009c0: 640e 640f 8400 8301 5a0b 650b 6a0a 6410  d.d.....Z.e.j.d.
-000009d0: 640f 8400 8301 5a0b 6508 6411 6412 8400  d.....Z.e.d.d...
-000009e0: 8301 5a0c 650c 6a0a 6413 6412 8400 8301  ..Z.e.j.d.d.....
-000009f0: 5a0c 6508 6414 6415 8400 8301 5a0d 6508  Z.e.d.d.....Z.e.
-00000a00: 6416 6417 8400 8301 5a0e 6508 6418 6419  d.d.....Z.e.d.d.
-00000a10: 8400 8301 5a0f 6508 641a 641b 8400 8301  ....Z.e.d.d.....
-00000a20: 5a10 6508 641c 641d 8400 8301 5a11 6508  Z.e.d.d.....Z.e.
-00000a30: 641e 641f 8400 8301 5a12 6420 6421 8400  d.d.....Z.d d!..
-00000a40: 5a13 6422 6423 8400 5a14 6424 6425 8400  Z.d"d#..Z.d$d%..
-00000a50: 5a15 6426 6427 8400 5a16 6428 6429 8400  Z.d&d'..Z.d(d)..
-00000a60: 5a17 643e 642a 642b 8401 5a18 643f 642e  Z.d>d*d+..Z.d?d.
-00000a70: 642f 8401 5a19 6430 6431 8400 5a1a 6432  d/..Z.d0d1..Z.d2
-00000a80: 6433 8400 5a1b 6434 6435 8400 5a1c 6436  d3..Z.d4d5..Z.d6
-00000a90: 6437 8400 5a1d 6438 6439 8400 5a1e 643a  d7..Z.d8d9..Z.d:
-00000aa0: 643b 8400 5a1f 6402 5300 2940 7207 0000  d;..Z.d.S.)@r...
-00000ab0: 007a 2343 6f6e 7461 696e 6572 2063 6c61  .z#Container cla
-00000ac0: 7373 2074 6f20 6861 6e64 6c65 206d 6978  ss to handle mix
-00000ad0: 7475 7265 732e 4ee7 0000 0000 00c0 7240  tures.N.......r@
-00000ae0: e700 0000 00d0 bcf8 4063 0500 0000 0000  ........@c......
-00000af0: 0000 0000 0000 0500 0000 0300 0000 4300  ..............C.
-00000b00: 0000 7372 0000 007c 017c 005f 007c 006a  ..sr...|.|._.|.j
-00000b10: 0064 0175 0072 187c 00a0 01a1 0001 0074  .d.u.r.|.......t
-00000b20: 0283 007c 005f 037c 0464 0175 0072 3664  ...|._.|.d.u.r6d
-00000b30: 0264 0364 049c 027c 005f 036e 067c 047c  .d.d...|._.n.|.|
-00000b40: 005f 037c 00a0 047c 006a 03a1 0101 007c  ._.|...|.j.....|
-00000b50: 037c 006a 0514 0074 067c 0214 001b 007c  .|.j...t.|.....|
-00000b60: 005f 077c 00a0 087c 02a1 017c 005f 097c  ._.|...|...|._.|
-00000b70: 027c 005f 0a64 0153 0029 0561 1d02 0000  .|._.d.S.).a....
-00000b80: 0a20 2020 2020 2020 2049 6e69 7469 616c  .        Initial
-00000b90: 697a 6520 6120 6060 5374 6174 6560 6020  ize a ``State`` 
-00000ba0: 6f62 6a65 6374 2e0a 0a20 2020 2020 2020  object...       
-00000bb0: 203a 7061 7261 6d20 7370 6563 6965 735f   :param species_
-00000bc0: 6462 3a20 5370 6563 6965 7320 6461 7461  db: Species data
-00000bd0: 6261 7365 2c20 6465 6661 756c 7473 2074  base, defaults t
-00000be0: 6f20 4156 4250 2073 7065 6369 6573 2064  o AVBP species d
-00000bf0: 6174 6162 6173 650a 2020 2020 2020 2020  atabase.        
-00000c00: 3a74 7970 6520 7370 6563 6965 735f 6462  :type species_db
-00000c10: 3a20 5370 6563 6965 732c 206f 7074 696f  : Species, optio
-00000c20: 6e61 6c0a 2020 2020 2020 2020 3a70 6172  nal.        :par
-00000c30: 616d 2074 656d 7065 7261 7475 7265 3a20  am temperature: 
-00000c40: 5465 6d70 6572 6174 7572 652c 2064 6566  Temperature, def
-00000c50: 6175 6c74 7320 746f 2033 3030 204b 0a20  aults to 300 K. 
-00000c60: 2020 2020 2020 203a 7479 7065 2074 656d         :type tem
-00000c70: 7065 7261 7475 7265 3a20 6e64 6172 7261  perature: ndarra
-00000c80: 7920 6f72 2073 6361 6c61 722c 206f 7074  y or scalar, opt
-00000c90: 696f 6e61 6c0a 2020 2020 2020 2020 3a70  ional.        :p
-00000ca0: 6172 616d 2070 7265 7373 7572 653a 2050  aram pressure: P
-00000cb0: 7265 7373 7572 652c 2064 6566 6175 6c74  ressure, default
-00000cc0: 7320 746f 2031 2061 746d 0a20 2020 2020  s to 1 atm.     
-00000cd0: 2020 203a 7479 7065 2070 7265 7373 7572     :type pressur
-00000ce0: 653a 206e 6461 7272 6179 206f 7220 7363  e: ndarray or sc
-00000cf0: 616c 6172 2c20 6f70 7469 6f6e 616c 0a20  alar, optional. 
-00000d00: 2020 2020 2020 203a 7061 7261 6d20 6d61         :param ma
-00000d10: 7373 5f66 7261 6374 696f 6e73 5f64 6963  ss_fractions_dic
-00000d20: 743a 2053 7065 6369 6573 206d 6173 7320  t: Species mass 
-00000d30: 6672 6163 7469 6f6e 732c 2064 6566 6175  fractions, defau
-00000d40: 6c74 7320 746f 2061 6972 0a20 2020 2020  lts to air.     
-00000d50: 2020 203a 7479 7065 206d 6173 735f 6672     :type mass_fr
-00000d60: 6163 7469 6f6e 735f 6469 6374 3a20 6469  actions_dict: di
-00000d70: 6374 5b73 7472 2c20 6e64 6172 7261 7920  ct[str, ndarray 
-00000d80: 6f72 2073 6361 6c61 725d 2c20 6f70 7469  or scalar], opti
-00000d90: 6f6e 616c 0a20 2020 2020 2020 204e 67c3  onal.        Ng.
-00000da0: f528 5c8f c2cd 3f67 8fc2 f528 5c8f e83f  .(\...?g...(\..?
-00000db0: a902 da02 4f32 da02 4e32 290b da07 7370  ....O2..N2)...sp
-00000dc0: 6563 6965 73da 185f 6465 6661 756c 745f  ecies.._default_
-00000dd0: 7468 6572 6d6f 5f64 6174 6162 6173 65da  thermo_database.
-00000de0: 0464 6963 74da 045f 795f 6bda 0e5f 6368  .dict.._y_k.._ch
-00000df0: 6563 6b5f 795f 696e 7075 74da 056d 6978  eck_y_input..mix
-00000e00: 5f77 7205 0000 00da 0372 686f da0a 6d69  _wr......rho..mi
-00000e10: 785f 656e 6572 6779 da06 656e 6572 6779  x_energy..energy
-00000e20: da0c 5f74 656d 7065 7261 7475 7265 2905  .._temperature).
-00000e30: da04 7365 6c66 da0a 7370 6563 6965 735f  ..self..species_
-00000e40: 6462 da0b 7465 6d70 6572 6174 7572 65da  db..temperature.
-00000e50: 0870 7265 7373 7572 65da 136d 6173 735f  .pressure..mass_
-00000e60: 6672 6163 7469 6f6e 735f 6469 6374 a900  fractions_dict..
-00000e70: 721c 0000 00fa 372f 5573 6572 732f 6461  r.....7/Users/da
-00000e80: 7570 7461 696e 2f47 4954 4c41 422f 6d73  uptain/GITLAB/ms
-00000e90: 5f74 6865 726d 6f2f 7372 632f 6d73 5f74  _thermo/src/ms_t
-00000ea0: 6865 726d 6f2f 7374 6174 652e 7079 da08  hermo/state.py..
-00000eb0: 5f5f 696e 6974 5f5f 3e00 0000 7316 0000  __init__>...s...
-00000ec0: 0000 1306 010a 0108 0208 0108 010e 0206  ................
-00000ed0: 010c 0214 020c 017a 0e53 7461 7465 2e5f  .......z.State._
-00000ee0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
-00000ef0: 0000 0000 0900 0000 0600 0000 4300 0000  ............C...
-00000f00: 7388 0100 0074 0083 007d 0174 0083 007d  s....t...}.t...}
-00000f10: 0274 0083 007d 0374 017c 006a 0264 0164  .t...}.t.|.j.d.d
-00000f20: 028d 0264 0319 007c 0364 043c 0074 03a0  ...d...|.d.<.t..
-00000f30: 047c 006a 02a1 017c 0164 043c 0074 03a0  .|.j...|.d.<.t..
-00000f40: 057c 006a 02a1 017c 0264 043c 0074 017c  .|.j...|.d.<.t.|
-00000f50: 006a 0664 0164 028d 0264 0319 007c 0364  .j.d.d...d...|.d
-00000f60: 053c 0074 03a0 047c 006a 06a1 017c 0164  .<.t...|.j...|.d
-00000f70: 053c 0074 03a0 057c 006a 06a1 017c 0264  .<.t...|.j...|.d
-00000f80: 053c 0074 017c 006a 0764 0164 028d 0264  .<.t.|.j.d.d...d
-00000f90: 0319 007c 0364 063c 0074 03a0 047c 006a  ...|.d.<.t...|.j
-00000fa0: 07a1 017c 0164 063c 0074 03a0 057c 006a  ...|.d.<.t...|.j
-00000fb0: 07a1 017c 0264 063c 0074 017c 006a 0864  ...|.d.<.t.|.j.d
-00000fc0: 0164 028d 0264 0319 007c 0364 073c 0074  .d...d...|.d.<.t
-00000fd0: 03a0 047c 006a 08a1 017c 0164 073c 0074  ...|.j...|.d.<.t
-00000fe0: 03a0 057c 006a 08a1 017c 0264 073c 007c  ...|.j...|.d.<.|
-00000ff0: 006a 0944 005d 4e7d 0464 087c 0417 007d  .j.D.]N}.d.|...}
-00001000: 0574 017c 006a 097c 0419 0064 0164 028d  .t.|.j.|...d.d..
-00001010: 0264 0319 007c 037c 053c 0074 03a0 047c  .d...|.|.<.t...|
-00001020: 006a 097c 0419 00a1 017c 017c 053c 0074  .j.|.....|.|.<.t
-00001030: 03a0 057c 006a 097c 0419 00a1 017c 027c  ...|.j.|.....|.|
-00001040: 053c 0071 f064 097d 067c 0664 0a37 007d  .<.q.d.}.|.d.7.}
-00001050: 067c 0664 0b37 007d 067c 0344 005d 2a7d  .|.d.7.}.|.D.]*}
-00001060: 077c 077c 037c 0719 007c 017c 0719 007c  .|.|.|...|.|...|
-00001070: 027c 0719 0066 047d 087c 0664 0c7c 0816  .|...f.}.|.d.|..
-00001080: 0037 007d 0690 0171 587c 0653 0029 0d7a  .7.}...qX|.S.).z
-00001090: 4a44 6566 696e 6520 7468 6520 7661 6c75  JDefine the valu
-000010a0: 6520 7265 7475 726e 6564 2062 7920 6361  e returned by ca
-000010b0: 6c6c 696e 6720 5374 6174 6520 7265 7072  lling State repr
-000010c0: 6573 656e 7461 7469 6f6e 2028 7072 696e  esentation (prin
-000010d0: 7469 6e67 2053 7461 7465 294e a901 da04  ting State)N....
-000010e0: 6178 6973 7201 0000 0072 1300 0000 7215  axisr....r....r.
-000010f0: 0000 0072 1900 0000 721a 0000 00da 0259  ...r....r......Y
-00001100: 5f7a 290a 4375 7272 656e 7420 7072 696d  _z).Current prim
-00001110: 6974 6976 6520 7374 6174 6520 6f66 2074  itive state of t
-00001120: 6865 206d 6978 7475 7265 200a 7a26 0909  he mixture .z&..
-00001130: 7c20 4d6f 7374 2043 6f6d 6d6f 6e20 7c20  | Most Common | 
-00001140: 2020 204d 696e 2020 2020 7c20 2020 204d     Min    |    M
-00001150: 6178 200a 7a35 2d2d 2d2d 2d2d 2d2d 2d2d  ax .z5----------
-00001160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00001180: 2d2d 2d2d 2d2d 2d2d 2d2d 0a7a 2025 3136  ----------.z %16
-00001190: 737c 2025 232e 3035 6520 7c20 2523 2e30  s| %#.05e | %#.0
-000011a0: 3365 207c 2025 232e 3033 6520 0a29 0a72  3e | %#.03e .).r
-000011b0: 0f00 0000 7203 0000 0072 1300 0000 da02  ....r....r......
-000011c0: 6e70 da03 6d69 6eda 036d 6178 7215 0000  np..min..maxr...
-000011d0: 0072 1900 0000 721a 0000 0072 1000 0000  .r....r....r....
-000011e0: 2909 7217 0000 00da 046d 696e 695a 046d  ).r......miniZ.m
-000011f0: 6178 695a 046d 6f63 6fda 0573 7065 6379  axiZ.moco..specy
-00001200: 5a0a 6672 6163 5f73 7065 6379 da08 7265  Z.frac_specy..re
-00001210: 7072 5f73 7472 da03 7661 72da 0569 6e66  pr_str..var..inf
-00001220: 6f73 721c 0000 0072 1c00 0000 721d 0000  osr....r....r...
-00001230: 00da 085f 5f72 6570 725f 5f61 0000 0073  ...__repr__a...s
-00001240: 3600 0000 0002 0601 0601 0601 1601 1001  6...............
-00001250: 1001 1601 1001 1001 1601 1001 1001 1601  ................
-00001260: 1001 1001 0a01 0801 1a01 1401 1601 0401  ................
-00001270: 0801 0801 0801 1801 1002 7a0e 5374 6174  ..........z.Stat
-00001280: 652e 5f5f 7265 7072 5f5f 6305 0000 0000  e.__repr__c.....
-00001290: 0000 0000 0000 0008 0000 0005 0000 0043  ...............C
-000012a0: 0000 0073 5600 0000 7400 8300 7d05 7c03  ...sV...t...}.|.
-000012b0: 4400 5d18 7d06 7401 a002 7c03 7c06 1900  D.].}.t...|.|...
-000012c0: 7c01 a102 7c05 7c06 3c00 710a 7c00 7c04  |...|.|.<.q.|.|.
-000012d0: 7c05 6401 8d02 7d07 7401 a002 7c02 7c01  |.d...}.t...|.|.
-000012e0: a102 7c07 5f03 7c01 7c07 5f04 7c07 a005  ..|._.|.|._.|...
-000012f0: 7c07 6a03 a101 7c07 5f06 7c07 5300 2902  |.j...|._.|.S.).
-00001300: 61cb 0100 000a 2020 2020 2020 2020 436c  a.....        Cl
-00001310: 6173 7320 636f 6e73 7472 7563 746f 7220  ass constructor 
-00001320: 6672 6f6d 2063 6f6e 7365 7276 6174 6976  from conservativ
-00001330: 6520 7661 6c75 6573 2e0a 0a20 2020 2020  e values...     
-00001340: 2020 203a 7061 7261 6d20 7268 6f3a 2044     :param rho: D
-00001350: 656e 7369 7479 0a20 2020 2020 2020 203a  ensity.        :
-00001360: 7479 7065 2072 686f 3a20 6e64 6172 7261  type rho: ndarra
-00001370: 7920 6f72 2073 6361 6c61 720a 2020 2020  y or scalar.    
-00001380: 2020 2020 3a70 6172 616d 2072 686f 5f65      :param rho_e
-00001390: 3a20 546f 7461 6c20 656e 6572 6779 2028  : Total energy (
-000013a0: 636f 6e73 6572 7661 7469 7665 2066 6f72  conservative for
-000013b0: 6d29 0a20 2020 2020 2020 203a 7479 7065  m).        :type
-000013c0: 2072 686f 5f65 3a20 6e64 6172 7261 7920   rho_e: ndarray 
-000013d0: 6f72 2073 6361 6c61 720a 2020 2020 2020  or scalar.      
-000013e0: 2020 3a70 6172 616d 2072 686f 5f79 3a20    :param rho_y: 
-000013f0: 5370 6563 6965 7320 6d61 7373 2066 7261  Species mass fra
-00001400: 6374 696f 6e73 2028 636f 6e73 6572 7661  ctions (conserva
-00001410: 7469 7665 2066 6f72 6d29 0a20 2020 2020  tive form).     
-00001420: 2020 203a 7479 7065 2072 686f 5f79 3a20     :type rho_y: 
-00001430: 6469 6374 5b73 7472 2c20 6e64 6172 7261  dict[str, ndarra
-00001440: 7920 6f72 2073 6361 6c61 725d 0a20 2020  y or scalar].   
-00001450: 2020 2020 203a 7061 7261 6d20 7370 6563       :param spec
-00001460: 6965 735f 6462 3a20 5370 6563 6965 7320  ies_db: Species 
-00001470: 6461 7461 6261 7365 2c20 6465 6661 756c  database, defaul
-00001480: 7473 2074 6f20 4156 4250 2073 7065 6369  ts to AVBP speci
-00001490: 6573 2064 6174 6162 6173 650a 2020 2020  es database.    
-000014a0: 2020 2020 3a74 7970 6520 7370 6563 6965      :type specie
-000014b0: 735f 6462 3a20 5370 6563 6965 732c 206f  s_db: Species, o
-000014c0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-000014d0: 2902 7218 0000 0072 1b00 0000 2907 720f  ).r....r....).r.
-000014e0: 0000 0072 2200 0000 da06 6469 7669 6465  ...r".....divide
-000014f0: 7215 0000 0072 1300 0000 da16 5f65 6e65  r....r......_ene
-00001500: 7267 795f 746f 5f74 656d 7065 7261 7475  rgy_to_temperatu
-00001510: 7265 7216 0000 0029 08da 0363 6c73 7213  rer....)...clsr.
-00001520: 0000 005a 0572 686f 5f65 5a05 7268 6f5f  ...Z.rho_eZ.rho_
-00001530: 7972 1800 0000 da03 795f 6b72 2600 0000  yr......y_kr&...
-00001540: da05 7374 6174 6572 1c00 0000 721c 0000  ..stater....r...
-00001550: 0072 1d00 0000 da09 6672 6f6d 5f63 6f6e  .r......from_con
-00001560: 7380 0000 0073 1000 0000 000e 0601 0801  s....s..........
-00001570: 1602 0c01 0e03 0603 0e01 7a0f 5374 6174  ..........z.Stat
-00001580: 652e 6672 6f6d 5f63 6f6e 7363 0100 0000  e.from_consc....
-00001590: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-000015a0: 4300 0000 7306 0000 007c 006a 0053 0029  C...s....|.j.S.)
-000015b0: 017a d647 6574 7465 7220 6f72 2073 6574  .z.Getter or set
-000015c0: 7465 7220 666f 7220 7468 6520 7370 6563  ter for the spec
-000015d0: 6965 7320 6d61 7373 2066 7261 6374 696f  ies mass fractio
-000015e0: 6e73 2e20 5365 7474 696e 6720 7468 6520  ns. Setting the 
-000015f0: 6d61 7373 2066 7261 6374 696f 6e73 0a20  mass fractions. 
-00001600: 2020 2020 2020 2077 696c 6c20 6d6f 6469         will modi
-00001610: 6679 2074 6865 2064 656e 7369 7479 2061  fy the density a
-00001620: 7373 756d 696e 6720 616e 2069 736f 7468  ssuming an isoth
-00001630: 6572 6d61 6c20 616e 6420 6973 6f62 6172  ermal and isobar
-00001640: 6963 2074 7261 6e73 666f 726d 6174 696f  ic transformatio
-00001650: 6e2e 0a0a 2020 2020 2020 2020 3a72 7479  n...        :rty
-00001660: 7065 3a20 6469 6374 5b73 7472 2c20 6e64  pe: dict[str, nd
-00001670: 6172 7261 7920 6f72 2073 6361 6c61 725d  array or scalar]
-00001680: 0a20 2020 2020 2020 2029 0172 1000 0000  .        ).r....
-00001690: a901 7217 0000 0072 1c00 0000 721c 0000  ..r....r....r...
-000016a0: 0072 1d00 0000 da0a 6d61 7373 5f66 7261  .r......mass_fra
-000016b0: 6373 9c00 0000 7302 0000 0000 077a 1053  cs....s......z.S
-000016c0: 7461 7465 2e6d 6173 735f 6672 6163 7363  tate.mass_fracsc
-000016d0: 0200 0000 0000 0000 0000 0000 0500 0000  ................
-000016e0: 0400 0000 4300 0000 7358 0000 007c 006a  ....C...sX...|.j
-000016f0: 007d 027c 00a0 017c 01a1 0101 0074 0283  .}.|...|.....t..
-00001700: 007c 005f 037c 0144 005d 127d 037c 017c  .|._.|.D.].}.|.|
-00001710: 0319 007c 006a 037c 033c 0071 1c7c 006a  ...|.j.|.<.q.|.j
-00001720: 007d 047c 006a 047c 0414 007c 021b 007c  .}.|.j.|...|...|
-00001730: 005f 047c 00a0 057c 006a 06a1 017c 005f  ._.|...|.j...|._
-00001740: 0764 0053 00a9 014e 2908 7212 0000 0072  .d.S...N).r....r
-00001750: 1100 0000 720f 0000 0072 1000 0000 7213  ....r....r....r.
-00001760: 0000 0072 1400 0000 7216 0000 0072 1500  ...r....r....r..
-00001770: 0000 2905 7217 0000 0072 1b00 0000 5a0e  ..).r....r....Z.
-00001780: 6d6f 6c5f 7765 6967 6874 5f6f 6c64 da01  mol_weight_old..
-00001790: 6b5a 0e6d 6f6c 5f77 6569 6768 745f 6e65  kZ.mol_weight_ne
-000017a0: 7772 1c00 0000 721c 0000 0072 1d00 0000  wr....r....r....
-000017b0: 7232 0000 00a5 0000 0073 1000 0000 0002  r2.......s......
-000017c0: 0602 0a01 0801 0801 1002 0601 1001 6301  ..............c.
-000017d0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-000017e0: 0000 0043 0000 0073 0600 0000 7c00 6a00  ...C...s....|.j.
-000017f0: 5300 2901 7acd 4765 7474 6572 206f 7220  S.).z.Getter or 
-00001800: 7365 7474 6572 2066 6f72 2074 6865 2074  setter for the t
-00001810: 656d 7065 7261 7475 7265 2e20 5365 7474  emperature. Sett
-00001820: 696e 6720 7468 6520 7465 6d70 6572 6174  ing the temperat
-00001830: 7572 6520 7769 6c6c 2072 6563 6f6d 7075  ure will recompu
-00001840: 7465 0a20 2020 2020 2020 2074 6865 2074  te.        the t
-00001850: 6f74 616c 2065 6e65 7267 7920 616e 6420  otal energy and 
-00001860: 6d6f 6469 6679 2074 6865 2064 656e 7369  modify the densi
-00001870: 7479 2061 7373 756d 696e 6720 616e 2069  ty assuming an i
-00001880: 736f 6261 7269 6320 7472 616e 7366 6f72  sobaric transfor
-00001890: 6d61 7469 6f6e 2e0a 0a20 2020 2020 2020  mation...       
-000018a0: 203a 7274 7970 653a 206e 6461 7272 6179   :rtype: ndarray
-000018b0: 206f 7220 7363 616c 6172 0a20 2020 2020   or scalar.     
-000018c0: 2020 2029 0172 1600 0000 7231 0000 0072     ).r....r1...r
-000018d0: 1c00 0000 721c 0000 0072 1d00 0000 7219  ....r....r....r.
-000018e0: 0000 00b2 0000 0073 0200 0000 0007 7a11  .......s......z.
-000018f0: 5374 6174 652e 7465 6d70 6572 6174 7572  State.temperatur
-00001900: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-00001910: 0000 0600 0000 4300 0000 7330 0000 0074  ......C...s0...t
-00001920: 00a0 0174 00a0 027c 006a 037c 006a 04a1  ...t...|.j.|.j..
-00001930: 027c 01a1 027c 005f 037c 017c 005f 057c  .|...|._.|.|._.|
-00001940: 00a0 067c 01a1 017c 005f 0764 0053 0072  ...|...|._.d.S.r
-00001950: 3300 0000 2908 7222 0000 0072 2b00 0000  3...).r"...r+...
-00001960: da08 6d75 6c74 6970 6c79 7213 0000 0072  ..multiplyr....r
-00001970: 1900 0000 7216 0000 0072 1400 0000 7215  ....r....r....r.
-00001980: 0000 00a9 0272 1700 0000 da04 7465 6d70  .....r......temp
-00001990: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-000019a0: 1900 0000 bb00 0000 7306 0000 0000 021a  ........s.......
-000019b0: 0106 0163 0100 0000 0000 0000 0000 0000  ...c............
-000019c0: 0100 0000 0200 0000 4300 0000 7316 0000  ........C...s...
-000019d0: 007c 006a 007c 006a 0114 0074 0214 007c  .|.j.|.j...t...|
-000019e0: 006a 031b 0053 0029 017a aa47 6574 7465  .j...S.).z.Gette
-000019f0: 7220 6f72 2073 6574 7465 7220 666f 7220  r or setter for 
-00001a00: 7468 6520 7072 6573 7375 7265 2e20 5365  the pressure. Se
-00001a10: 7474 696e 6720 7468 6520 7072 6573 7375  tting the pressu
-00001a20: 7265 2077 696c 6c20 6d6f 6469 6679 2074  re will modify t
-00001a30: 6865 0a20 2020 2020 2020 2064 656e 7369  he.        densi
-00001a40: 7479 2061 7373 756d 696e 6720 616e 2069  ty assuming an i
-00001a50: 736f 7468 6572 6d61 6c20 7472 616e 7366  sothermal transf
-00001a60: 6f72 6d61 7469 6f6e 2e0a 0a20 2020 2020  ormation...     
-00001a70: 2020 203a 7274 7970 653a 206e 6461 7272     :rtype: ndarr
-00001a80: 6179 206f 7220 7363 616c 6172 0a20 2020  ay or scalar.   
-00001a90: 2020 2020 2029 0472 1300 0000 7219 0000       ).r....r...
-00001aa0: 0072 0500 0000 7212 0000 0072 3100 0000  .r....r....r1...
-00001ab0: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-00001ac0: 1a00 0000 c100 0000 7302 0000 0000 077a  ........s......z
-00001ad0: 0e53 7461 7465 2e70 7265 7373 7572 6563  .State.pressurec
-00001ae0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00001af0: 0600 0000 4300 0000 731e 0000 0074 00a0  ....C...s....t..
-00001b00: 0174 00a0 027c 006a 037c 01a1 027c 006a  .t...|.j.|...|.j
-00001b10: 04a1 027c 005f 0364 0053 0072 3300 0000  ...|._.d.S.r3...
-00001b20: 2905 7222 0000 0072 2b00 0000 7235 0000  ).r"...r+...r5..
-00001b30: 0072 1300 0000 721a 0000 0029 0272 1700  .r....r....).r..
-00001b40: 0000 da05 7072 6573 7372 1c00 0000 721c  ....pressr....r.
-00001b50: 0000 0072 1d00 0000 721a 0000 00ca 0000  ...r....r.......
-00001b60: 0073 0200 0000 0002 6301 0000 0000 0000  .s......c.......
-00001b70: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00001b80: 0073 0c00 0000 7c00 6a00 7c00 6a01 1b00  .s....|.j.|.j...
-00001b90: 5300 2901 7a82 0a20 2020 2020 2020 2047  S.).z..        G
-00001ba0: 6574 2074 6865 2068 6561 7420 6361 7061  et the heat capa
-00001bb0: 6369 7479 2072 6174 696f 0a0a 2020 2020  city ratio..    
-00001bc0: 2020 2020 3a72 6574 7572 6e73 3a20 2a2a      :returns: **
-00001bd0: 6761 6d6d 612a 2a20 2d20 4865 6174 2063  gamma** - Heat c
-00001be0: 6170 6163 6974 7920 7261 7469 6f0a 2020  apacity ratio.  
-00001bf0: 2020 2020 2020 3a72 7479 7065 3a20 6e64        :rtype: nd
-00001c00: 6172 7261 7920 6f72 2073 6361 6c61 720a  array or scalar.
-00001c10: 2020 2020 2020 2020 2902 da03 635f 70da          )...c_p.
-00001c20: 0363 5f76 7231 0000 0072 1c00 0000 721c  .c_vr1...r....r.
-00001c30: 0000 0072 1d00 0000 da05 6761 6d6d 61ce  ...r......gamma.
-00001c40: 0000 0073 0200 0000 0008 7a0b 5374 6174  ...s......z.Stat
-00001c50: 652e 6761 6d6d 6163 0100 0000 0000 0000  e.gammac........
-00001c60: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00001c70: 731c 0000 007c 006a 007c 006a 017c 006a  s....|.j.|.j.|.j
-00001c80: 027c 006a 0314 001b 0017 007d 017c 0153  .|.j.......}.|.S
-00001c90: 0029 0161 5501 0000 0a20 2020 2020 2020  .).aU....       
-00001ca0: 2047 6574 2074 6865 206d 6978 7475 7265   Get the mixture
-00001cb0: 2d61 7665 7261 6765 6420 6865 6174 2063  -averaged heat c
-00001cc0: 6170 6163 6974 7920 6174 2063 6f6e 7374  apacity at const
-00001cd0: 616e 7420 7072 6573 7375 7265 0a0a 2020  ant pressure..  
-00001ce0: 2020 2020 2020 2e2e 2077 6172 6e69 6e67        .. warning
-00001cf0: 3a3a 0a20 2020 2020 2020 2020 2020 203a  ::.            :
-00001d00: 6d61 7468 3a60 435f 7060 2069 7320 636f  math:`C_p` is co
-00001d10: 6d70 7574 6564 206c 696b 6520 696e 2041  mputed like in A
-00001d20: 5642 5020 6173 203a 6d61 7468 3a60 435f  VBP as :math:`C_
-00001d30: 762b 502f 285c 7268 6f20 5429 602c 202a  v+P/(\rho T)`, *
-00001d40: 6e6f 742a 2061 730a 2020 2020 2020 2020  not* as.        
-00001d50: 2020 2020 7468 6520 7765 6967 6874 6564      the weighted
-00001d60: 2061 7665 7261 6765 206f 6620 7370 6563   average of spec
-00001d70: 6965 7320 3a6d 6174 683a 6043 5f7b 702c  ies :math:`C_{p,
-00001d80: 6b7d 600a 0a20 2020 2020 2020 203a 7265  k}`..        :re
-00001d90: 7475 726e 733a 202a 2a43 702a 2a20 2d20  turns: **Cp** - 
-00001da0: 4865 6174 2063 6170 6163 6974 7920 6174  Heat capacity at
-00001db0: 2063 6f6e 7374 616e 7420 7072 6573 7375   constant pressu
-00001dc0: 7265 0a20 2020 2020 2020 203a 7274 7970  re.        :rtyp
-00001dd0: 653a 206e 6461 7272 6179 206f 7220 7363  e: ndarray or sc
-00001de0: 616c 6172 0a20 2020 2020 2020 2029 0472  alar.        ).r
-00001df0: 3a00 0000 721a 0000 0072 1300 0000 7219  :...r....r....r.
-00001e00: 0000 0029 0272 1700 0000 7239 0000 0072  ...).r....r9...r
-00001e10: 1c00 0000 721c 0000 0072 1d00 0000 7239  ....r....r....r9
-00001e20: 0000 00d8 0000 0073 0400 0000 0012 1802  .......s........
-00001e30: 7a09 5374 6174 652e 635f 7063 0100 0000  z.State.c_pc....
-00001e40: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00001e50: 0300 0000 7320 0000 0088 006a 0089 0174  ....s .....j...t
-00001e60: 0187 0087 0166 0264 0164 0284 0888 006a  .....f.d.d.....j
-00001e70: 0244 0083 0183 0153 0029 037a aa0a 2020  .D.....S.).z..  
-00001e80: 2020 2020 2020 4765 7420 7468 6520 6d69        Get the mi
-00001e90: 7874 7572 652d 6176 6572 6167 6564 2068  xture-averaged h
-00001ea0: 6561 7420 6361 7061 6369 7479 2061 7420  eat capacity at 
-00001eb0: 636f 6e73 7461 6e74 2076 6f6c 756d 650a  constant volume.
-00001ec0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00001ed0: 733a 202a 2a43 762a 2a20 2d20 4865 6174  s: **Cv** - Heat
-00001ee0: 2063 6170 6163 6974 7920 6174 2063 6f6e   capacity at con
-00001ef0: 7374 616e 7420 766f 6c75 6d65 0a20 2020  stant volume.   
-00001f00: 2020 2020 203a 7274 7970 653a 206e 6461       :rtype: nda
-00001f10: 7272 6179 206f 7220 7363 616c 6172 0a20  rray or scalar. 
-00001f20: 2020 2020 2020 2063 0100 0000 0000 0000         c........
-00001f30: 0000 0000 0200 0000 0500 0000 3300 0000  ............3...
-00001f40: 7328 0000 007c 005d 207d 0188 006a 007c  s(...|.] }...j.|
-00001f50: 0119 0088 006a 017c 0119 00a0 0288 01a1  .....j.|........
-00001f60: 0114 0056 0001 0071 0264 0053 0072 3300  ...V...q.d.S.r3.
-00001f70: 0000 2903 7210 0000 0072 0d00 0000 723a  ..).r....r....r:
-00001f80: 0000 00a9 02da 022e 3072 3400 0000 7236  ........0r4...r6
-00001f90: 0000 0072 1c00 0000 721d 0000 00da 093c  ...r....r......<
-00001fa0: 6765 6e65 7870 723e f700 0000 7304 0000  genexpr>....s...
-00001fb0: 0004 0202 ff7a 1c53 7461 7465 2e63 5f76  .....z.State.c_v
-00001fc0: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
-00001fd0: 7072 3e29 0372 1900 0000 da03 7375 6dda  pr>).r......sum.
-00001fe0: 096c 6973 745f 7370 6563 7231 0000 0072  .list_specr1...r
-00001ff0: 1c00 0000 7236 0000 0072 1d00 0000 723a  ....r6...r....r:
-00002000: 0000 00ee 0000 0073 0800 0000 0008 0601  .......s........
-00002010: 0e02 04fe 7a09 5374 6174 652e 635f 7663  ....z.State.c_vc
-00002020: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00002030: 0400 0000 4300 0000 7320 0000 0074 00a0  ....C...s ...t..
-00002040: 017c 006a 0274 0314 007c 006a 041b 007c  .|.j.t...|.j...|
-00002050: 006a 0514 00a1 017d 017c 0153 0029 017a  .j.....}.|.S.).z
-00002060: 790a 2020 2020 2020 2020 4765 7420 7468  y.        Get th
-00002070: 6520 7370 6565 6420 6f66 2073 6f75 6e64  e speed of sound
-00002080: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00002090: 6e73 3a20 2a2a 6373 6f75 6e64 2a2a 202d  ns: **csound** -
-000020a0: 2053 7065 6564 206f 6620 736f 756e 640a   Speed of sound.
-000020b0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-000020c0: 6e64 6172 7261 7920 6f72 2073 6361 6c61  ndarray or scala
-000020d0: 720a 2020 2020 2020 2020 2906 7222 0000  r.        ).r"..
-000020e0: 00da 0473 7172 7472 3b00 0000 7205 0000  ...sqrtr;...r...
-000020f0: 0072 1200 0000 7219 0000 0029 0272 1700  .r....r....).r..
-00002100: 0000 da06 6373 6f75 6e64 721c 0000 0072  ....csoundr....r
-00002110: 1c00 0000 721d 0000 0072 4200 0000 fc00  ....r....rB.....
-00002120: 0000 7314 0000 0000 0804 0104 0102 ff02  ..s.............
-00002130: 0204 fe02 0304 fd02 ff04 057a 0c53 7461  ...........z.Sta
-00002140: 7465 2e63 736f 756e 6463 0100 0000 0000  te.csoundc......
-00002150: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00002160: 0000 730e 0000 0074 007c 006a 01a0 02a1  ..s....t.|.j....
-00002170: 0083 0153 0029 017a 850a 2020 2020 2020  ...S.).z..      
-00002180: 2020 4765 7420 7468 6520 6e61 6d65 7320    Get the names 
-00002190: 6f66 2074 6865 2073 7065 6369 6573 0a0a  of the species..
-000021a0: 2020 2020 2020 2020 3a72 6574 7572 6e73          :returns
-000021b0: 3a20 2a2a 7370 6563 6965 735f 6e61 6d65  : **species_name
-000021c0: 732a 2a20 2d20 4c69 7374 206f 6620 7370  s** - List of sp
-000021d0: 6563 6965 7320 6e61 6d65 730a 2020 2020  ecies names.    
-000021e0: 2020 2020 3a72 7479 7065 3a20 6c69 7374      :rtype: list
-000021f0: 5b73 7472 5d0a 2020 2020 2020 2020 2903  [str].        ).
-00002200: da04 6c69 7374 7210 0000 00da 046b 6579  ..listr......key
-00002210: 7372 3100 0000 721c 0000 0072 1c00 0000  sr1...r....r....
-00002220: 721d 0000 0072 4000 0000 0b01 0000 7302  r....r@.......s.
-00002230: 0000 0000 087a 0f53 7461 7465 2e6c 6973  .....z.State.lis
-00002240: 745f 7370 6563 6301 0000 0000 0000 0000  t_specc.........
-00002250: 0000 0003 0000 0005 0000 0003 0000 0073  ...............s
-00002260: 2a00 0000 8700 6601 6401 6402 8408 8800  *.....f.d.d.....
-00002270: 6a00 4400 8301 7d01 6403 7401 6a02 7c01  j.D...}.d.t.j.|.
-00002280: 6404 6405 8d02 1b00 7d02 7c02 5300 2906  d.d.....}.|.S.).
-00002290: 7ae7 0a20 2020 2020 2020 2043 6f6d 7075  z..        Compu
-000022a0: 7465 2074 6865 206d 6978 7475 7265 206d  te the mixture m
-000022b0: 6f6c 6563 756c 6172 2077 6569 6768 743a  olecular weight:
-000022c0: 0a0a 2020 2020 2020 2020 2e2e 206d 6174  ..        .. mat
-000022d0: 683a 3a20 575f 7b6d 6978 7d20 3d20 5c6c  h:: W_{mix} = \l
-000022e0: 6566 745b 205c 7375 6d5f 7b6b 3d31 7d5e  eft[ \sum_{k=1}^
-000022f0: 7b4e 5f7b 7370 7d7d 205c 6672 6163 7b59  {N_{sp}} \frac{Y
-00002300: 5f6b 7d7b 575f 6b7d 205c 7269 6768 745d  _k}{W_k} \right]
-00002310: 5e7b 2d31 7d0a 0a20 2020 2020 2020 203a  ^{-1}..        :
-00002320: 7265 7475 726e 733a 202a 2a6d 6978 5f6d  returns: **mix_m
-00002330: 772a 2a20 2d20 4d69 7874 7572 6520 6d6f  w** - Mixture mo
-00002340: 6c65 6375 6c61 7220 7765 6967 6874 0a20  lecular weight. 
-00002350: 2020 2020 2020 203a 7274 7970 653a 206e         :rtype: n
-00002360: 6461 7272 6179 206f 7220 7363 616c 6172  darray or scalar
-00002370: 0a20 2020 2020 2020 2063 0100 0000 0000  .        c......
-00002380: 0000 0000 0000 0200 0000 0700 0000 1300  ................
-00002390: 0000 7326 0000 0067 007c 005d 1e7d 0174  ..s&...g.|.].}.t
-000023a0: 00a0 0188 006a 027c 0119 0088 006a 037c  .....j.|.....j.|
-000023b0: 0119 006a 04a1 0291 0271 0453 0072 1c00  ...j.....q.S.r..
-000023c0: 0000 2905 7222 0000 0072 2b00 0000 7210  ..).r"...r+...r.
-000023d0: 0000 0072 0d00 0000 da10 6d6f 6c65 6375  ...r......molecu
-000023e0: 6c61 725f 7765 6967 6874 723c 0000 0072  lar_weightr<...r
-000023f0: 3100 0000 721c 0000 0072 1d00 0000 da0a  1...r....r......
-00002400: 3c6c 6973 7463 6f6d 703e 1f01 0000 7304  <listcomp>....s.
-00002410: 0000 0006 0202 ff7a 1f53 7461 7465 2e6d  .......z.State.m
-00002420: 6978 5f77 2e3c 6c6f 6361 6c73 3e2e 3c6c  ix_w.<locals>.<l
-00002430: 6973 7463 6f6d 703e e700 0000 0000 00f0  istcomp>........
-00002440: 3f72 0100 0000 721f 0000 0029 0372 4000  ?r....r....).r@.
-00002450: 0000 7222 0000 0072 3f00 0000 2903 7217  ..r"...r?...).r.
-00002460: 0000 005a 0679 5f6f 765f 775a 066d 6978  ...Z.y_ov_wZ.mix
-00002470: 5f6d 7772 1c00 0000 7231 0000 0072 1d00  _mwr....r1...r..
-00002480: 0000 7212 0000 0015 0100 0073 0a00 0000  ..r........s....
-00002490: 000a 0a02 04fe 0604 1201 7a0b 5374 6174  ..........z.Stat
-000024a0: 652e 6d69 785f 7763 0200 0000 0000 0000  e.mix_wc........
-000024b0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-000024c0: 730a 0000 007c 017c 006a 001b 0053 0029  s....|.|.j...S.)
-000024d0: 017a bf0a 2020 2020 2020 2020 436f 6d70  .z..        Comp
-000024e0: 7574 6520 7468 6520 4d61 6368 206e 756d  ute the Mach num
-000024f0: 6265 720a 0a20 2020 2020 2020 203a 7061  ber..        :pa
-00002500: 7261 6d20 7665 6c6f 6369 7479 3a20 5665  ram velocity: Ve
-00002510: 6c6f 6369 7479 0a20 2020 2020 2020 203a  locity.        :
-00002520: 7479 7065 2076 656c 6f63 6974 793a 206e  type velocity: n
-00002530: 6461 7272 6179 206f 7220 7363 616c 6172  darray or scalar
-00002540: 0a0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00002550: 6e73 3a20 2a2a 4d2a 2a20 2d20 4d61 6368  ns: **M** - Mach
-00002560: 206e 756d 6265 720a 2020 2020 2020 2020   number.        
-00002570: 3a72 7479 7065 3a20 6e64 6172 7261 7920  :rtype: ndarray 
-00002580: 6f72 2073 6361 6c61 720a 2020 2020 2020  or scalar.      
-00002590: 2020 2901 7242 0000 00a9 0272 1700 0000    ).rB.....r....
-000025a0: 5a08 7665 6c6f 6369 7479 721c 0000 0072  Z.velocityr....r
-000025b0: 1c00 0000 721d 0000 00da 046d 6163 6826  ....r......mach&
-000025c0: 0100 0073 0200 0000 000a 7a0a 5374 6174  ...s......z.Stat
-000025d0: 652e 6d61 6368 6302 0000 0000 0000 0000  e.machc.........
-000025e0: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
-000025f0: 2600 0000 6401 6402 7c00 6a00 6401 1800  &...d.d.|.j.d...
-00002600: 1400 7c00 a001 7c01 a101 6403 1300 1400  ..|...|...d.....
-00002610: 1700 7c00 6a02 1400 5300 2904 619f 0100  ..|.j...S.).a...
-00002620: 000a 2020 2020 2020 2020 436f 6d70 7574  ..        Comput
-00002630: 6520 7468 6520 746f 7461 6c20 7465 6d70  e the total temp
-00002640: 6572 6174 7572 653a 0a0a 2020 2020 2020  erature:..      
-00002650: 2020 2e2e 206d 6174 683a 3a20 545f 7420    .. math:: T_t 
-00002660: 3d20 5420 5c6c 6566 745b 312b 5c66 7261  = T \left[1+\fra
-00002670: 637b 5c67 616d 6d61 2d31 7d7b 327d 4d5e  c{\gamma-1}{2}M^
-00002680: 3220 5c72 6967 6874 5d0a 0a20 2020 2020  2 \right]..     
-00002690: 2020 2077 6865 7265 203a 6d61 7468 3a60     where :math:`
-000026a0: 4d60 2069 7320 7468 6520 4d61 6368 206e  M` is the Mach n
-000026b0: 756d 6265 7220 6465 7269 7665 6420 6672  umber derived fr
-000026c0: 6f6d 2074 6865 2069 6e70 7574 2076 656c  om the input vel
-000026d0: 6f63 6974 792e 0a20 2020 2020 2020 2054  ocity..        T
-000026e0: 6869 7320 6173 7375 6d65 7320 616e 2069  his assumes an i
-000026f0: 7365 6e74 726f 7069 6320 666c 6f77 2061  sentropic flow a
-00002700: 6e64 2063 6f6e 7374 616e 7420 6761 6d6d  nd constant gamm
-00002710: 612e 0a0a 2020 2020 2020 2020 3a70 6172  a...        :par
-00002720: 616d 2076 656c 6f63 6974 793a 2056 656c  am velocity: Vel
-00002730: 6f63 6974 790a 2020 2020 2020 2020 3a74  ocity.        :t
-00002740: 7970 6520 7665 6c6f 6369 7479 3a20 6e64  ype velocity: nd
-00002750: 6172 7261 7920 6f72 2073 6361 6c61 720a  array or scalar.
-00002760: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00002770: 733a 202a 2a74 656d 705f 746f 7461 6c2a  s: **temp_total*
-00002780: 2a20 2d20 546f 7461 6c20 7465 6d70 6572  * - Total temper
-00002790: 6174 7572 650a 2020 2020 2020 2020 3a72  ature.        :r
-000027a0: 7479 7065 3a20 6e64 6172 7261 7920 6f72  type: ndarray or
-000027b0: 2073 6361 6c61 720a 2020 2020 2020 2020   scalar.        
-000027c0: e901 0000 00e7 0000 0000 0000 e03f e902  .............?..
-000027d0: 0000 0029 0372 3b00 0000 7249 0000 0072  ...).r;...rI...r
-000027e0: 1900 0000 7248 0000 0072 1c00 0000 721c  ....rH...r....r.
-000027f0: 0000 0072 1d00 0000 da11 7465 6d70 6572  ...r......temper
-00002800: 6174 7572 655f 746f 7461 6c32 0100 0073  ature_total2...s
-00002810: 0800 0000 0010 1e01 04ff 02ff 7a17 5374  ............z.St
-00002820: 6174 652e 7465 6d70 6572 6174 7572 655f  ate.temperature_
-00002830: 746f 7461 6c63 0200 0000 0000 0000 0000  totalc..........
-00002840: 0000 0200 0000 0700 0000 4300 0000 733a  ..........C...s:
-00002850: 0000 0074 00a0 0164 0164 027c 006a 0264  ...t...d.d.|.j.d
-00002860: 0118 0014 007c 00a0 037c 01a1 0164 0313  .....|...|...d..
-00002870: 0014 0017 007c 006a 027c 006a 0264 0118  .....|.j.|.j.d..
-00002880: 001b 00a1 027c 006a 0414 0053 0029 0461  .....|.j...S.).a
-00002890: b301 0000 0a20 2020 2020 2020 2043 6f6d  .....        Com
-000028a0: 7075 7465 2074 6865 2074 6f74 616c 2070  pute the total p
-000028b0: 7265 7373 7572 653a 0a0a 2020 2020 2020  ressure:..      
-000028c0: 2020 2e2e 206d 6174 683a 3a20 505f 7420    .. math:: P_t 
-000028d0: 3d20 5020 5c6c 6566 745b 312b 5c66 7261  = P \left[1+\fra
-000028e0: 637b 5c67 616d 6d61 2d31 7d7b 327d 4d5e  c{\gamma-1}{2}M^
-000028f0: 3220 5c72 6967 6874 5d5e 7b5c 6672 6163  2 \right]^{\frac
-00002900: 7b5c 6761 6d6d 617d 7b5c 6761 6d6d 612d  {\gamma}{\gamma-
-00002910: 317d 7d0a 0a20 2020 2020 2020 2077 6865  1}}..        whe
-00002920: 7265 203a 6d61 7468 3a60 4d60 2069 7320  re :math:`M` is 
-00002930: 7468 6520 4d61 6368 206e 756d 6265 7220  the Mach number 
-00002940: 6465 7269 7665 6420 6672 6f6d 2074 6865  derived from the
-00002950: 2069 6e70 7574 2076 656c 6f63 6974 792e   input velocity.
-00002960: 0a20 2020 2020 2020 2054 6869 7320 6173  .        This as
-00002970: 7375 6d65 7320 616e 2069 7365 6e74 726f  sumes an isentro
-00002980: 7069 6320 666c 6f77 2061 6e64 2063 6f6e  pic flow and con
-00002990: 7374 616e 7420 6761 6d6d 612e 0a0a 2020  stant gamma...  
-000029a0: 2020 2020 2020 3a70 6172 616d 2076 656c        :param vel
-000029b0: 6f63 6974 793a 2056 656c 6f63 6974 790a  ocity: Velocity.
-000029c0: 2020 2020 2020 2020 3a74 7970 6520 7665          :type ve
-000029d0: 6c6f 6369 7479 3a20 6e64 6172 7261 7920  locity: ndarray 
-000029e0: 6f72 2073 6361 6c61 720a 2020 2020 2020  or scalar.      
-000029f0: 2020 3a72 6574 7572 6e73 3a20 2a2a 7072    :returns: **pr
-00002a00: 6573 735f 746f 7461 6c2a 2a20 2d20 546f  ess_total** - To
-00002a10: 7461 6c20 7072 6573 7375 7265 0a20 2020  tal pressure.   
-00002a20: 2020 2020 203a 7274 7970 653a 206e 6461       :rtype: nda
-00002a30: 7272 6179 206f 7220 7363 616c 6172 0a20  rray or scalar. 
-00002a40: 2020 2020 2020 2072 4a00 0000 724b 0000         rJ...rK..
-00002a50: 0072 4c00 0000 2905 7222 0000 00da 0570  .rL...).r".....p
-00002a60: 6f77 6572 723b 0000 0072 4900 0000 721a  owerr;...rI...r.
-00002a70: 0000 0072 4800 0000 721c 0000 0072 1c00  ...rH...r....r..
-00002a80: 0000 721d 0000 00da 0e70 7265 7373 7572  ..r......pressur
-00002a90: 655f 746f 7461 6c46 0100 0073 0e00 0000  e_totalF...s....
-00002aa0: 000f 0401 1e01 0efe 0203 04fd 02ff 7a14  ..............z.
-00002ab0: 5374 6174 652e 7072 6573 7375 7265 5f74  State.pressure_t
-00002ac0: 6f74 616c 6302 0000 0000 0000 0000 0000  otalc...........
-00002ad0: 0002 0000 0004 0000 0003 0000 0073 1a00  .............s..
-00002ae0: 0000 7400 8700 8701 6602 6401 6402 8408  ..t.....f.d.d...
-00002af0: 8800 6a01 4400 8301 8301 5300 2903 6117  ..j.D.....S.).a.
-00002b00: 0100 000a 2020 2020 2020 2020 436f 6d70  ....        Comp
-00002b10: 7574 6520 7468 6520 6d69 7874 7572 6520  ute the mixture 
-00002b20: 746f 7461 6c20 656e 6572 6779 3a0a 0a20  total energy:.. 
-00002b30: 2020 2020 2020 202e 2e20 6d61 7468 3a3a         .. math::
-00002b40: 2065 203d 205c 7375 6d5f 7b6b 3d31 7d5e   e = \sum_{k=1}^
-00002b50: 7b4e 5f7b 7370 7d7d 2059 5f6b 2065 5f6b  {N_{sp}} Y_k e_k
-00002b60: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00002b70: 2074 656d 7065 7261 7475 7265 3a20 5465   temperature: Te
-00002b80: 6d70 6572 6174 7572 650a 2020 2020 2020  mperature.      
-00002b90: 2020 3a74 7970 6520 7465 6d70 6572 6174    :type temperat
-00002ba0: 7572 653a 206e 6461 7272 6179 206f 7220  ure: ndarray or 
-00002bb0: 7363 616c 6172 0a0a 2020 2020 2020 2020  scalar..        
-00002bc0: 3a72 6574 7572 6e73 3a20 2a2a 6d69 785f  :returns: **mix_
-00002bd0: 656e 6572 6779 2a2a 202d 204d 6978 7475  energy** - Mixtu
-00002be0: 7265 2074 6f74 616c 2065 6e65 7267 790a  re total energy.
-00002bf0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00002c00: 6e64 6172 7261 7920 6f72 2073 6361 6c61  ndarray or scala
-00002c10: 720a 2020 2020 2020 2020 6301 0000 0000  r.        c.....
-00002c20: 0000 0000 0000 0002 0000 0005 0000 0033  ...............3
-00002c30: 0000 0073 2800 0000 7c00 5d20 7d01 8800  ...s(...|.] }...
-00002c40: 6a00 7c01 1900 8800 6a01 7c01 1900 a002  j.|.....j.|.....
-00002c50: 8801 a101 1400 5600 0100 7102 6400 5300  ......V...q.d.S.
-00002c60: 7233 0000 0029 0372 1000 0000 720d 0000  r3...).r....r...
-00002c70: 00da 0c74 6f74 616c 5f65 6e65 7267 7972  ...total_energyr
-00002c80: 3c00 0000 a902 7217 0000 0072 1900 0000  <.....r....r....
-00002c90: 721c 0000 0072 1d00 0000 723e 0000 006a  r....r....r>...j
-00002ca0: 0100 0073 0400 0000 0402 02ff 7a23 5374  ...s........z#St
-00002cb0: 6174 652e 6d69 785f 656e 6572 6779 2e3c  ate.mix_energy.<
-00002cc0: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
-00002cd0: 3ea9 0272 3f00 0000 7240 0000 0072 5100  >..r?...r@...rQ.
-00002ce0: 0000 721c 0000 0072 5100 0000 721d 0000  ..r....rQ...r...
-00002cf0: 0072 1400 0000 5b01 0000 7306 0000 0000  .r....[...s.....
-00002d00: 0f0e 0204 fe7a 1053 7461 7465 2e6d 6978  .....z.State.mix
-00002d10: 5f65 6e65 7267 7963 0200 0000 0000 0000  _energyc........
-00002d20: 0000 0000 0200 0000 0400 0000 0300 0000  ................
-00002d30: 731a 0000 0074 0087 0087 0166 0264 0164  s....t.....f.d.d
-00002d40: 0284 0888 006a 0144 0083 0183 0153 0029  .....j.D.....S.)
-00002d50: 0361 1501 0000 0a20 2020 2020 2020 2047  .a.....        G
-00002d60: 6574 206d 6978 7475 7265 2074 6f74 616c  et mixture total
-00002d70: 2065 6e74 6861 6c70 793a 0a0a 2020 2020   enthalpy:..    
-00002d80: 2020 2020 2e2e 206d 6174 683a 3a20 6820      .. math:: h 
-00002d90: 3d20 5c73 756d 5f7b 6b3d 317d 5e7b 4e5f  = \sum_{k=1}^{N_
-00002da0: 7b73 707d 7d20 595f 6b20 685f 6b0a 0a20  {sp}} Y_k h_k.. 
-00002db0: 2020 2020 2020 203a 7061 7261 6d20 7465         :param te
-00002dc0: 6d70 6572 6174 7572 653a 2054 656d 7065  mperature: Tempe
-00002dd0: 7261 7475 7265 0a20 2020 2020 2020 203a  rature.        :
-00002de0: 7479 7065 2074 656d 7065 7261 7475 7265  type temperature
-00002df0: 3a20 6e64 6172 7261 7920 6f72 2073 6361  : ndarray or sca
-00002e00: 6c61 720a 0a20 2020 2020 2020 203a 7265  lar..        :re
-00002e10: 7475 726e 733a 202a 2a6d 6978 5f65 6e74  turns: **mix_ent
-00002e20: 6861 6c70 792a 2a20 2d20 4d69 7874 7572  halpy** - Mixtur
-00002e30: 6520 746f 7461 6c20 656e 7468 616c 7079  e total enthalpy
-00002e40: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00002e50: 206e 6461 7272 6179 206f 7220 7363 616c   ndarray or scal
-00002e60: 6172 0a20 2020 2020 2020 2063 0100 0000  ar.        c....
-00002e70: 0000 0000 0000 0000 0200 0000 0500 0000  ................
-00002e80: 3300 0000 7328 0000 007c 005d 207d 0188  3...s(...|.] }..
-00002e90: 006a 007c 0119 0088 006a 017c 0119 00a0  .j.|.....j.|....
-00002ea0: 0288 01a1 0114 0056 0001 0071 0264 0053  .......V...q.d.S
-00002eb0: 0072 3300 0000 2903 7210 0000 0072 0d00  .r3...).r....r..
-00002ec0: 0000 5a0e 746f 7461 6c5f 656e 7468 616c  ..Z.total_enthal
-00002ed0: 7079 723c 0000 0072 5100 0000 721c 0000  pyr<...rQ...r...
-00002ee0: 0072 1d00 0000 723e 0000 007b 0100 0073  .r....r>...{...s
-00002ef0: 0400 0000 0402 02ff 7a25 5374 6174 652e  ........z%State.
-00002f00: 6d69 785f 656e 7468 616c 7079 2e3c 6c6f  mix_enthalpy.<lo
-00002f10: 6361 6c73 3e2e 3c67 656e 6578 7072 3e72  cals>.<genexpr>r
-00002f20: 5200 0000 7251 0000 0072 1c00 0000 7251  R...rQ...r....rQ
-00002f30: 0000 0072 1d00 0000 da0c 6d69 785f 656e  ...r......mix_en
-00002f40: 7468 616c 7079 6f01 0000 7306 0000 0000  thalpyo...s.....
-00002f50: 0c0e 0204 fe7a 1253 7461 7465 2e6d 6978  .....z.State.mix
-00002f60: 5f65 6e74 6861 6c70 7963 0400 0000 0000  _enthalpyc......
-00002f70: 0000 0000 0000 0400 0000 0200 0000 4300  ..............C.
-00002f80: 0000 732e 0000 007c 0364 0175 0172 0e7c  ..s....|.d.u.r.|
-00002f90: 037c 005f 007c 0164 0175 0172 1c7c 017c  .|._.|.d.u.r.|.|
-00002fa0: 005f 017c 0264 0175 0172 2a7c 027c 005f  ._.|.d.u.r*|.|._
-00002fb0: 0264 0153 0029 0261 7403 0000 0a20 2020  .d.S.).at....   
-00002fc0: 2020 2020 2043 6f6d 7075 7465 2064 656e       Compute den
-00002fd0: 7369 7479 2066 726f 6d20 7465 6d70 6572  sity from temper
-00002fe0: 6174 7572 652c 2070 7265 7373 7572 6520  ature, pressure 
-00002ff0: 616e 6420 6d61 7373 2066 7261 6374 696f  and mass fractio
-00003000: 6e73 2062 7920 6173 7375 6d69 6e67 2074  ns by assuming t
-00003010: 6865 0a20 2020 2020 2020 2066 6f6c 6c6f  he.        follo
-00003020: 7769 6e67 2074 7261 6e73 666f 726d 6174  wing transformat
-00003030: 696f 6e73 3a0a 0a20 2020 2020 2020 2020  ions:..         
-00003040: 2020 2031 2920 4973 6f62 6172 6963 2061     1) Isobaric a
-00003050: 6e64 2069 736f 7468 6572 6d61 6c20 7472  nd isothermal tr
-00003060: 616e 7366 6f72 6d61 7469 6f6e 2c0a 2020  ansformation,.  
-00003070: 2020 2020 2020 2020 2020 692e 6520 282a            i.e (*
-00003080: 503d 6373 742a 2c20 2a54 3d63 7374 2a20  P=cst*, *T=cst* 
-00003090: 616e 6420 6f6e 6c79 202a 2a63 6f6d 706f  and only **compo
-000030a0: 7369 7469 6f6e 2a2a 2069 7320 7661 7279  sition** is vary
-000030b0: 696e 6729 0a0a 2020 2020 2020 2020 2020  ing)..          
-000030c0: 2020 3229 2049 736f 6261 7269 6320 616e    2) Isobaric an
-000030d0: 6420 6973 6f2d 636f 6d70 6f73 6974 696f  d iso-compositio
-000030e0: 6e20 7472 616e 7366 6f72 6d61 7469 6f6e  n transformation
-000030f0: 2c0a 2020 2020 2020 2020 2020 2020 692e  ,.            i.
-00003100: 6520 282a 503d 6373 742a 2c20 2a59 3d63  e (*P=cst*, *Y=c
-00003110: 7374 2a20 616e 6420 6f6e 6c79 202a 2a74  st* and only **t
-00003120: 656d 7065 7261 7475 7265 2a2a 2069 7320  emperature** is 
-00003130: 7661 7279 696e 6729 0a0a 2020 2020 2020  varying)..      
-00003140: 2020 2020 2020 3329 2049 736f 7468 6572        3) Isother
-00003150: 6d61 6c20 616e 6420 6973 6f2d 636f 6d70  mal and iso-comp
-00003160: 6f73 6974 696f 6e20 7472 616e 7366 6f72  osition transfor
-00003170: 6d61 7469 6f6e 2c0a 2020 2020 2020 2020  mation,.        
-00003180: 2020 2020 692e 6520 282a 543d 6373 742a      i.e (*T=cst*
-00003190: 2c20 2a59 3d63 7374 2a20 616e 6420 6f6e  , *Y=cst* and on
-000031a0: 6c79 202a 2a70 7265 7373 7572 652a 2a20  ly **pressure** 
-000031b0: 6973 2076 6172 7969 6e67 290a 0a20 2020  is varying)..   
-000031c0: 2020 2020 203a 7061 7261 6d20 7465 6d70       :param temp
-000031d0: 6572 6174 7572 653a 2054 656d 7065 7261  erature: Tempera
-000031e0: 7475 7265 2074 6f20 7365 742c 2064 6566  ture to set, def
-000031f0: 6175 6c74 7320 746f 204e 6f6e 650a 2020  aults to None.  
-00003200: 2020 2020 2020 3a74 7970 6520 7465 6d70        :type temp
-00003210: 6572 6174 7572 653a 206e 6461 7272 6179  erature: ndarray
-00003220: 206f 7220 7363 616c 6172 2c20 6f70 7469   or scalar, opti
-00003230: 6f6e 616c 0a20 2020 2020 2020 203a 7061  onal.        :pa
-00003240: 7261 6d20 7072 6573 7375 7265 3a20 5072  ram pressure: Pr
-00003250: 6573 7375 7265 2074 6f20 7365 742c 2064  essure to set, d
-00003260: 6566 6175 6c74 7320 746f 204e 6f6e 650a  efaults to None.
-00003270: 2020 2020 2020 2020 3a74 7970 6520 7072          :type pr
-00003280: 6573 7375 7265 3a20 6e64 6172 7261 7920  essure: ndarray 
-00003290: 6f72 2073 6361 6c61 722c 206f 7074 696f  or scalar, optio
-000032a0: 6e61 6c0a 2020 2020 2020 2020 3a70 6172  nal.        :par
-000032b0: 616d 206d 6173 735f 6672 6163 733a 204d  am mass_fracs: M
-000032c0: 6173 7320 6672 6163 7469 6f6e 7320 746f  ass fractions to
-000032d0: 2073 6574 2c20 6465 6661 756c 7473 2074   set, defaults t
-000032e0: 6f20 4e6f 6e65 0a20 2020 2020 2020 203a  o None.        :
-000032f0: 7479 7065 206d 6173 735f 6672 6163 733a  type mass_fracs:
-00003300: 2064 6963 745b 7374 722c 206e 6461 7272   dict[str, ndarr
-00003310: 6179 206f 7220 7363 616c 6172 5d2c 206f  ay or scalar], o
-00003320: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00003330: 4e29 0372 3200 0000 7219 0000 0072 1a00  N).r2...r....r..
-00003340: 0000 2904 7217 0000 0072 1900 0000 721a  ..).r....r....r.
-00003350: 0000 0072 3200 0000 721c 0000 0072 1c00  ...r2...r....r..
-00003360: 0000 721d 0000 00da 0c75 7064 6174 655f  ..r......update_
-00003370: 7374 6174 6580 0100 0073 0c00 0000 0015  state....s......
-00003380: 0801 0601 0801 0601 0801 7a12 5374 6174  ..........z.Stat
-00003390: 652e 7570 6461 7465 5f73 7461 7465 da01  e.update_state..
-000033a0: 4346 6306 0000 0000 0000 0000 0000 000e  CFc.............
-000033b0: 0000 0006 0000 0043 0000 0073 4201 0000  .......C...sB...
-000033c0: 6401 7d06 7c02 6402 7500 727e 7400 8300  d.}.|.d.u.r~t...
-000033d0: 7d02 7401 a002 7c00 6a03 7c01 1900 a004  }.t...|.j.|.....
-000033e0: a100 a101 7d07 7c00 6a03 4400 5d1a 7d08  ....}.|.j.D.].}.
-000033f0: 7c00 6a03 7c08 1900 a004 a100 7c07 1900  |.j.|.......|...
-00003400: 7c02 7c08 3c00 712c 7c06 6403 3700 7d06  |.|.<.q,|.d.7.}.
-00003410: 7c02 4400 5d20 7d08 7c06 6404 7c08 1700  |.D.] }.|.d.|...
-00003420: 6405 1700 7405 7c02 7c08 1900 8301 1700  d...t.|.|.......
-00003430: 3700 7d06 7154 7c06 6406 3700 7d06 7c03  7.}.qT|.d.7.}.|.
-00003440: 6402 7500 7298 6407 6408 6409 9c02 7d03  d.u.r.d.d.d...}.
-00003450: 7c06 640a 3700 7d06 640b 7d09 640b 7d0a  |.d.7.}.d.}.d.}.
-00003460: 640b 7d0b 7c00 6a03 4400 5d74 7d08 7c00  d.}.|.j.D.]t}.|.
-00003470: 6a06 7c08 1900 6a07 7d0c 7c0c 7c04 1900  j.|...j.}.|.|...
-00003480: 7408 7c04 a009 a100 1900 1400 7c00 6a06  t.|.........|.j.
-00003490: 7c08 1900 6a0a 1b00 7d0d 7c09 7c00 6a03  |...j...}.|.|.j.
-000034a0: 7c08 1900 7c0d 1400 3700 7d09 7c08 7c02  |...|...7.}.|.|.
-000034b0: 7600 9001 7206 7c0a 7c02 7c08 1900 7c0d  v...r.|.|.|...|.
-000034c0: 1400 3700 7d0a 7c08 7c03 7600 72aa 7c0b  ..7.}.|.|.v.r.|.
-000034d0: 7c03 7c08 1900 7c0d 1400 3700 7d0b 71aa  |.|...|...7.}.q.
-000034e0: 7c09 7c0b 1800 7c0a 7c0b 1800 1b00 7d09  |.|...|.|.....}.
-000034f0: 7c05 9001 723e 740b 7c06 8301 0100 7c09  |...r>t.|.....|.
-00003500: 5300 290c 6194 0200 0043 6f6d 7075 7465  S.).a....Compute
-00003510: 2074 6865 205a 206d 6978 7475 7265 2066   the Z mixture f
-00003520: 7261 6374 696f 6e2e 0a0a 2020 2020 2020  raction...      
-00003530: 2020 3020 6f78 6964 697a 6572 2c20 3120    0 oxidizer, 1 
-00003540: 6675 656c 0a0a 2020 2020 2020 2020 3a70  fuel..        :p
-00003550: 6172 616d 2073 7065 6366 7565 6c3a 2046  aram specfuel: F
-00003560: 7565 6c20 7370 6563 6965 730a 2020 2020  uel species.    
-00003570: 2020 2020 3a74 7970 6520 7370 6563 6675      :type specfu
-00003580: 656c 3a20 7374 720a 2020 2020 2020 2020  el: str.        
-00003590: 3a70 6172 616d 2066 7565 6c5f 6d61 7373  :param fuel_mass
-000035a0: 5f66 7261 6373 3a20 4675 656c 206d 6173  _fracs: Fuel mas
-000035b0: 7320 6672 6163 7469 6f6e 732c 2064 6566  s fractions, def
-000035c0: 6175 6c74 7320 746f 2063 6f6d 706f 7369  aults to composi
-000035d0: 7469 6f6e 2061 7420 7065 616b 2066 7565  tion at peak fue
-000035e0: 6c20 636f 6e63 656e 7472 6174 696f 6e0a  l concentration.
-000035f0: 2020 2020 2020 2020 3a74 7970 6520 6675          :type fu
-00003600: 656c 5f6d 6173 735f 6672 6163 733a 2064  el_mass_fracs: d
-00003610: 6963 742c 206f 7074 696f 6e61 6c0a 2020  ict, optional.  
-00003620: 2020 2020 2020 3a70 6172 616d 206f 7879        :param oxy
-00003630: 645f 6d61 7373 5f66 7261 6373 3a20 4f78  d_mass_fracs: Ox
-00003640: 7964 697a 6572 206d 6173 7320 6672 6163  ydizer mass frac
-00003650: 7469 6f6e 732c 2064 6566 6175 6c74 7320  tions, defaults 
-00003660: 746f 2061 6972 0a20 2020 2020 2020 203a  to air.        :
-00003670: 7479 7065 206f 7879 645f 6d61 7373 5f66  type oxyd_mass_f
-00003680: 7261 6373 3a20 6469 6374 2c20 6f70 7469  racs: dict, opti
-00003690: 6f6e 616c 0a20 2020 2020 2020 203a 7061  onal.        :pa
-000036a0: 7261 6d20 6174 6f6d 5f72 6566 3a20 5265  ram atom_ref: Re
-000036b0: 6665 7265 6e63 6520 6174 6f6d 2c20 6465  ference atom, de
-000036c0: 6661 756c 7473 2074 6f20 430a 2020 2020  faults to C.    
-000036d0: 2020 2020 3a74 7970 6520 6174 6f6d 5f72      :type atom_r
-000036e0: 6566 3a20 7374 722c 206f 7074 696f 6e61  ef: str, optiona
-000036f0: 6c0a 2020 2020 2020 2020 3a70 6172 616d  l.        :param
-00003700: 2076 6572 626f 7365 3a20 5665 7262 6f73   verbose: Verbos
-00003710: 6974 792c 2064 6566 6175 6c74 7320 746f  ity, defaults to
-00003720: 2046 616c 7365 0a20 2020 2020 2020 203a   False.        :
-00003730: 7479 7065 2076 6572 626f 7365 3a20 626f  type verbose: bo
-00003740: 6f6c 2c20 6f70 7469 6f6e 616c 0a0a 2020  ol, optional..  
-00003750: 2020 2020 2020 3a72 6574 7572 6e73 3a20        :returns: 
-00003760: 5a20 4d69 7874 7572 6520 6672 6163 7469  Z Mixture fracti
-00003770: 6f6e 0a20 2020 2020 2020 203a 7274 7970  on.        :rtyp
-00003780: 653a 206e 6461 7272 6179 206f 7220 7363  e: ndarray or sc
-00003790: 616c 6172 0a20 2020 2020 2020 207a 1443  alar.        z.C
-000037a0: 6f6d 7075 7469 6e67 205a 2066 7261 6374  omputing Z fract
-000037b0: 696f 6e4e 7a1b 2020 2046 7565 6c20 6d69  ionNz.   Fuel mi
-000037c0: 7874 7572 6520 7461 6b65 6e20 6173 203a  xture taken as :
-000037d0: 207a 060a 2e20 202d 20da 013a da01 0a67   z...  - ..:...g
-000037e0: 6de7 fba9 f1d2 cd3f 6725 0681 9543 8be8  m......?g%...C..
-000037f0: 3f72 0a00 0000 7a22 0a2e 2020 4f78 6964  ?r....z"..  Oxid
-00003800: 697a 6572 206d 6978 7475 7265 2074 616b  izer mixture tak
-00003810: 656e 2061 7320 4149 522e 6700 0000 0000  en as AIR.g.....
-00003820: 0000 0029 0c72 0f00 0000 7222 0000 00da  ...).r....r"....
-00003830: 0661 7267 6d61 7872 3200 0000 da05 7261  .argmaxr2.....ra
-00003840: 7665 6cda 0373 7472 720d 0000 00da 0561  vel..strr......a
-00003850: 746f 6d73 7206 0000 00da 056c 6f77 6572  tomsr......lower
-00003860: 7245 0000 00da 0570 7269 6e74 290e 7217  rE.....print).r.
-00003870: 0000 005a 0873 7065 6366 7565 6c5a 0f66  ...Z.specfuelZ.f
-00003880: 7565 6c5f 6d61 7373 5f66 7261 6373 5a0f  uel_mass_fracsZ.
-00003890: 6f78 7964 5f6d 6173 735f 6672 6163 735a  oxyd_mass_fracsZ
-000038a0: 0861 746f 6d5f 7265 66da 0776 6572 626f  .atom_ref..verbo
-000038b0: 7365 da03 6c6f 67da 0369 6478 da04 7370  se..log..idx..sp
-000038c0: 6563 5a06 7a5f 6672 6163 5a06 7a5f 6675  ecZ.z_fracZ.z_fu
-000038d0: 656c 5a06 7a5f 6f78 7964 5a08 6e62 5f61  elZ.z_oxydZ.nb_a
-000038e0: 746f 6d73 5a0a 7265 6c5f 7765 6967 6874  tomsZ.rel_weight
-000038f0: 721c 0000 0072 1c00 0000 721d 0000 00da  r....r....r.....
-00003900: 0e63 6f6d 7075 7465 5f7a 5f66 7261 639c  .compute_z_frac.
-00003910: 0100 0073 4200 0000 001a 0401 0802 0601  ...sB...........
-00003920: 1401 0a01 1801 0801 0801 1e01 0801 0801  ................
-00003930: 0a01 0802 0401 0401 0402 0a01 0c03 0601  ................
-00003940: 0aff 0202 0afe 02ff 0205 1201 0a01 1001  ................
-00003950: 0801 1202 1002 0601 0801 7a14 5374 6174  ..........z.Stat
-00003960: 652e 636f 6d70 7574 655f 7a5f 6672 6163  e.compute_z_frac
-00003970: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-00003980: 0003 0000 0043 0000 0073 2000 0000 7c00  .....C...s ...|.
-00003990: a000 7c01 a101 7d02 7c00 6a01 7d03 6401  ..|...}.|.j.}.d.
-000039a0: 7c02 7c03 1b00 1800 7d04 7c04 5300 2902  |.|.....}.|.S.).
-000039b0: 7acd 436f 6d70 7574 6520 656e 6572 6779  z.Compute energy
-000039c0: 2072 6573 6964 7561 6c73 2066 726f 6d20   residuals from 
-000039d0: 7465 6d70 6572 6174 7572 652e 0a0a 2020  temperature...  
-000039e0: 2020 2020 2020 3a70 6172 616d 2074 656d        :param tem
-000039f0: 7065 7261 7475 7265 3a20 5465 6d70 6572  perature: Temper
-00003a00: 6174 7572 650a 2020 2020 2020 2020 3a74  ature.        :t
-00003a10: 7970 6520 7465 6d70 6572 6174 7572 653a  ype temperature:
-00003a20: 206e 6461 7272 6179 206f 7220 7363 616c   ndarray or scal
-00003a30: 6172 0a20 2020 2020 2020 203a 7265 7475  ar.        :retu
-00003a40: 726e 733a 2045 6e65 7267 7920 7265 7369  rns: Energy resi
-00003a50: 6475 616c 0a20 2020 2020 2020 203a 7274  dual.        :rt
-00003a60: 7970 653a 206e 6461 7272 6179 206f 7220  ype: ndarray or 
-00003a70: 7363 616c 6172 0a20 2020 2020 2020 2072  scalar.        r
-00003a80: 4700 0000 2902 7214 0000 0072 1500 0000  G...).r....r....
-00003a90: 2905 7217 0000 0072 1900 0000 5a0b 636f  ).r....r....Z.co
-00003aa0: 6d70 5f65 6e65 7267 7972 5000 0000 da04  mp_energyrP.....
-00003ab0: 6469 6666 721c 0000 0072 1c00 0000 721d  diffr....r....r.
-00003ac0: 0000 00da 105f 7465 6d70 5f65 6e65 7267  ....._temp_energ
-00003ad0: 795f 7265 73dd 0100 0073 0800 0000 0008  y_res....s......
-00003ae0: 0a01 0601 0c01 7a16 5374 6174 652e 5f74  ......z.State._t
-00003af0: 656d 705f 656e 6572 6779 5f72 6573 6301  emp_energy_resc.
-00003b00: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00003b10: 0000 0043 0000 0073 1a00 0000 7400 a001  ...C...s....t...
-00003b20: 7402 6401 a102 7d01 7403 7c01 8301 7c00  t.d...}.t.|...|.
-00003b30: 5f04 6402 5300 2903 7a8a 0a20 2020 2020  _.d.S.).z..     
-00003b40: 2020 2049 6e69 7469 616c 697a 6520 7468     Initialize th
-00003b50: 6520 7468 6572 6d6f 6479 6e61 6d69 6320  e thermodynamic 
-00003b60: 6461 7461 6261 7365 2069 6620 6e6f 6e65  database if none
-00003b70: 2069 7320 7072 6f76 6964 6564 2e0a 0a20   is provided... 
-00003b80: 2020 2020 2020 2042 7920 6465 6661 756c         By defaul
-00003b90: 7420 6974 2069 7320 7468 6520 4156 4250  t it is the AVBP
-00003ba0: 2073 7461 6e64 6172 6420 7370 6563 6965   standard specie
-00003bb0: 7320 6461 7461 6261 7365 2e0a 2020 2020  s database..    
-00003bc0: 2020 2020 7a1c 2e2f 494e 5055 542f 7370      z../INPUT/sp
-00003bd0: 6563 6965 735f 6461 7461 6261 7365 2e64  ecies_database.d
-00003be0: 6174 4e29 05da 0d70 6b67 5f72 6573 6f75  atN)...pkg_resou
-00003bf0: 7263 6573 da11 7265 736f 7572 6365 5f66  rces..resource_f
-00003c00: 696c 656e 616d 65da 085f 5f6e 616d 655f  ilename..__name_
-00003c10: 5f72 0400 0000 720d 0000 0029 0272 1700  _r....r....).r..
-00003c20: 0000 5a0e 7468 6572 6d6f 5f64 625f 6669  ..Z.thermo_db_fi
-00003c30: 6c65 721c 0000 0072 1c00 0000 721d 0000  ler....r....r...
-00003c40: 0072 0e00 0000 ea01 0000 7308 0000 0000  .r........s.....
-00003c50: 0604 0104 ff04 037a 1e53 7461 7465 2e5f  .......z.State._
-00003c60: 6465 6661 756c 745f 7468 6572 6d6f 5f64  default_thermo_d
-00003c70: 6174 6162 6173 6563 0200 0000 0000 0000  atabasec........
-00003c80: 0000 0000 0b00 0000 0600 0000 4300 0000  ............C...
-00003c90: 73bc 0000 0064 017d 0264 027d 0364 037d  s....d.}.d.}.d.}
-00003ca0: 047c 0144 005d 1e7d 057c 057c 006a 0076  .|.D.].}.|.|.j.v
-00003cb0: 0172 107c 047c 0516 007d 0674 017c 0683  .r.|.|...}.t.|..
-00003cc0: 0182 0171 1064 047d 077c 0144 005d 107d  ...q.d.}.|.D.].}
-00003cd0: 057c 077c 017c 0519 0037 007d 0771 3874  .|.|.|...7.}.q8t
-00003ce0: 02a0 037c 0764 0518 00a1 017c 026b 047d  ...|.d.....|.k.}
-00003cf0: 0874 02a0 047c 08a1 017d 097c 0972 b874  .t...|...}.|.r.t
-00003d00: 02a0 057c 08a1 0164 0419 0064 0419 007d  ...|...d...d...}
-00003d10: 0a7c 037c 0a16 007d 067c 0664 0674 0674  .|.|...}.|.d.t.t
-00003d20: 02a0 077c 07a1 0183 0117 0037 007d 067c  ...|.......7.}.|
-00003d30: 0664 0774 0674 02a0 087c 07a1 0183 0117  .d.t.t...|......
-00003d40: 0037 007d 0674 017c 0683 0182 0164 0853  .7.}.t.|.....d.S
-00003d50: 0029 097a f60a 2020 2020 2020 2020 4368  .).z..        Ch
-00003d60: 6563 6b20 6966 2074 6865 206e 616d 6573  eck if the names
-00003d70: 206f 6620 7468 6520 7370 6563 6965 7320   of the species 
-00003d80: 6172 6520 696e 2074 6865 2064 6174 6162  are in the datab
-00003d90: 6173 650a 2020 2020 2020 2020 7468 6520  ase.        the 
-00003da0: 7375 6d20 6f66 206d 6978 7475 7265 2073  sum of mixture s
-00003db0: 7065 6369 6573 206d 6173 7320 6672 6163  pecies mass frac
-00003dc0: 7469 6f6e 7320 6973 2075 6e69 7479 0a0a  tions is unity..
-00003dd0: 2020 2020 2020 2020 3a70 6172 616d 206d          :param m
-00003de0: 6173 735f 6672 6163 7469 6f6e 735f 6469  ass_fractions_di
-00003df0: 6374 3a20 4d61 7373 2066 7261 6374 696f  ct: Mass fractio
-00003e00: 6e73 0a20 2020 2020 2020 203a 7479 7065  ns.        :type
-00003e10: 206d 6173 735f 6672 6163 7469 6f6e 735f   mass_fractions_
-00003e20: 6469 6374 3a20 6469 6374 5b73 7472 2c20  dict: dict[str, 
-00003e30: 6e64 6172 7261 7920 6f72 2073 6361 6c61  ndarray or scala
-00003e40: 725d 0a20 2020 2020 2020 2067 f168 e388  r].        g.h..
-00003e50: b5f8 e43e 7a2a 4d61 7373 2066 7261 6374  ...>z*Mass fract
-00003e60: 696f 6e20 7375 6d20 6973 206e 6f74 2075  ion sum is not u
-00003e70: 6e69 7479 2061 7420 706f 696e 7420 2564  nity at point %d
-00003e80: 7a29 5370 6563 6965 7320 2573 2069 7320  z)Species %s is 
-00003e90: 6e6f 7420 7072 6573 656e 7420 696e 2074  not present in t
-00003ea0: 6865 2064 6174 6162 6173 6572 0100 0000  he databaser....
-00003eb0: 7247 0000 007a 060a 206d 696e 3a7a 060a  rG...z.. min:z..
-00003ec0: 206d 6178 3a4e 2909 720d 0000 00da 0a56   max:N).r......V
-00003ed0: 616c 7565 4572 726f 7272 2200 0000 da03  alueErrorr".....
-00003ee0: 6162 73da 0361 6e79 da05 7768 6572 6572  abs..any..wherer
-00003ef0: 5a00 0000 7223 0000 0072 2400 0000 290b  Z...r#...r$...).
-00003f00: 7217 0000 0072 1b00 0000 5a05 795f 746f  r....r....Z.y_to
-00003f10: 6c5a 0b6e 6f74 5f6f 6e65 5f6d 7367 5a0d  lZ.not_one_msgZ.
-00003f20: 6e6f 745f 696e 5f64 625f 6d73 675a 0673  not_in_db_msgZ.s
-00003f30: 7065 6369 65da 036d 7367 5a05 7375 6d5f  pecie..msgZ.sum_
-00003f40: 795a 0563 6f6e 6473 5a0a 6973 5f6e 6f74  yZ.condsZ.is_not
-00003f50: 5f6f 6e65 da05 696e 6465 7872 1c00 0000  _one..indexr....
-00003f60: 721c 0000 0072 1d00 0000 7211 0000 00f5  r....r....r.....
-00003f70: 0100 0073 2400 0000 0008 0401 0401 0403  ...s$...........
-00003f80: 0801 0a01 0801 0a03 0401 0801 0e01 1201  ................
-00003f90: 0a01 0401 1201 0801 1601 1601 7a14 5374  ............z.St
-00003fa0: 6174 652e 5f63 6865 636b 5f79 5f69 6e70  ate._check_y_inp
-00003fb0: 7574 6302 0000 0000 0000 0000 0000 0004  utc.............
-00003fc0: 0000 0005 0000 0043 0000 0073 2200 0000  .......C...s"...
-00003fd0: 7400 a001 7c01 a101 6401 1400 7d02 7402  t...|...d...}.t.
-00003fe0: 7c00 6a03 7c02 6402 6403 8d03 7d03 7c03  |.j.|.d.d...}.|.
-00003ff0: 5300 2904 614b 0100 000a 2020 2020 2020  S.).aK....      
-00004000: 2020 4669 6e64 2074 6865 2074 656d 7065    Find the tempe
-00004010: 7261 7475 7265 2060 5460 2074 6861 7420  rature `T` that 
-00004020: 7361 7469 7366 6965 7320 7468 6520 636f  satisfies the co
-00004030: 6e73 7472 6169 6e74 3a0a 0a20 2020 2020  nstraint:..     
-00004040: 2020 202e 2e20 6d61 7468 3a3a 2065 203d     .. math:: e =
-00004050: 205c 7375 6d5f 7b6b 3d31 7d5e 7b4e 5f7b   \sum_{k=1}^{N_{
-00004060: 7370 7d7d 2059 5f6b 2065 5f6b 2854 290a  sp}} Y_k e_k(T).
-00004070: 0a20 2020 2020 2020 2067 6976 656e 2061  .        given a
-00004080: 2074 6172 6765 7420 7661 6c75 6520 6f66   target value of
-00004090: 2074 6865 2074 6f74 616c 2065 6e65 7267   the total energ
-000040a0: 7920 6065 602e 0a0a 2020 2020 2020 2020  y `e`...        
-000040b0: 3a70 6172 616d 2065 6e65 7267 793a 2054  :param energy: T
-000040c0: 6172 6765 7420 746f 7461 6c20 656e 6572  arget total ener
-000040d0: 6779 0a20 2020 2020 2020 203a 7479 7065  gy.        :type
-000040e0: 2065 6e65 7267 793a 206e 6461 7272 6179   energy: ndarray
-000040f0: 206f 7220 7363 616c 6172 0a0a 2020 2020   or scalar..    
-00004100: 2020 2020 3a72 6574 7572 6e73 3a20 5465      :returns: Te
-00004110: 6d70 6572 6174 7572 650a 2020 2020 2020  mperature.      
-00004120: 2020 3a72 7479 7065 3a20 6e64 6172 7261    :rtype: ndarra
-00004130: 7920 6f72 2073 6361 6c61 720a 2020 2020  y or scalar.    
-00004140: 2020 2020 7208 0000 0067 11ea 2d81 9997      r....g..-...
-00004150: 713d 2901 da03 746f 6c29 0472 2200 0000  q=)...tol).r"...
-00004160: da09 6f6e 6573 5f6c 696b 6572 0200 0000  ..ones_liker....
-00004170: 7264 0000 0029 0472 1700 0000 7215 0000  rd...).r....r...
-00004180: 00da 0567 7565 7373 7219 0000 0072 1c00  ...guessr....r..
-00004190: 0000 721c 0000 0072 1d00 0000 722c 0000  ..r....r....r,..
-000041a0: 0014 0200 0073 0600 0000 000e 0e01 1001  .....s..........
-000041b0: 7a1c 5374 6174 652e 5f65 6e65 7267 795f  z.State._energy_
-000041c0: 746f 5f74 656d 7065 7261 7475 7265 6301  to_temperaturec.
-000041d0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000041e0: 0000 0043 0000 0073 2e00 0000 7400 a001  ...C...s....t...
-000041f0: 6401 a101 0100 6402 7d01 7c01 6403 3700  d.....d.}.|.d.7.
-00004200: 7d01 7400 a002 7c01 a101 0100 7403 7c01  }.t...|.....t.|.
-00004210: 8301 0100 7c00 6a04 5300 2904 7a82 0a20  ....|.j.S.).z.. 
-00004220: 2020 2020 2020 202a 5265 7475 726e 2070         *Return p
-00004230: 7269 6d69 7469 7665 7320 7370 6563 6965  rimitives specie
-00004240: 7320 6e61 6d65 732a 2e0a 0a20 2020 2020  s names*...     
-00004250: 2020 203a 7265 7475 726e 733a 202a 2a73     :returns: **s
-00004260: 7065 6369 6573 5f6e 616d 6573 2a2a 202d  pecies_names** -
-00004270: 2041 206c 6973 7428 2029 206f 6620 7072   A list( ) of pr
-00004280: 696d 6974 6976 6573 2073 7065 6369 6573  imitives species
-00004290: 206e 616d 6573 0a0a 2020 2020 2020 2020   names..        
-000042a0: da06 6967 6e6f 7265 7a2d 6d73 5f74 6865  ..ignorez-ms_the
-000042b0: 726d 6f2e 7374 6174 652e 6c69 7374 5f73  rmo.state.list_s
-000042c0: 7065 6369 6573 2829 2069 7320 6465 7072  pecies() is depr
-000042d0: 6563 6174 6564 2c7a 2575 7365 2069 6e73  ecated,z%use ins
-000042e0: 7465 6164 206d 735f 7468 6572 6d6f 2e73  tead ms_thermo.s
-000042f0: 7461 7465 2e6c 6973 745f 7370 6563 2905  tate.list_spec).
-00004300: da08 7761 726e 696e 6773 da0c 7369 6d70  ..warnings..simp
-00004310: 6c65 6669 6c74 6572 da04 7761 726e 725d  lefilter..warnr]
-00004320: 0000 0072 4000 0000 a902 7217 0000 005a  ...r@.....r....Z
-00004330: 076d 7367 7761 726e 721c 0000 0072 1c00  .msgwarnr....r..
-00004340: 0000 721d 0000 00da 0c6c 6973 745f 7370  ..r......list_sp
-00004350: 6563 6965 7328 0200 0073 0c00 0000 0007  ecies(...s......
-00004360: 0a01 0401 0801 0a01 0801 7a12 5374 6174  ..........z.Stat
-00004370: 652e 6c69 7374 5f73 7065 6369 6573 6301  e.list_speciesc.
-00004380: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00004390: 0000 0043 0000 0073 2e00 0000 7400 a001  ...C...s....t...
-000043a0: 6401 a101 0100 6402 7d01 7c01 6403 3700  d.....d.}.|.d.7.
-000043b0: 7d01 7400 a002 7c01 a101 0100 7403 7c01  }.t...|.....t.|.
-000043c0: 8301 0100 7c00 6a04 5300 2904 7ae2 0a20  ....|.j.S.).z.. 
-000043d0: 2020 2020 2020 202a 436f 6d70 7574 6520         *Compute 
-000043e0: 6d69 7874 7572 6520 6d6f 6c65 6375 6c61  mixture molecula
-000043f0: 7220 7765 6967 6874 2066 6f6c 6c6f 7769  r weight followi
-00004400: 6e67 2074 6865 2066 6f72 6d75 6c61 203a  ng the formula :
-00004410: 2a0a 0a20 2020 2020 2020 202e 2e20 6d61  *..        .. ma
-00004420: 7468 3a3a 2057 5f7b 6d69 787d 203d 205c  th:: W_{mix} = \
-00004430: 6c65 6674 5b20 5c73 756d 5f7b 6b3d 317d  left[ \sum_{k=1}
-00004440: 5e7b 4e5f 7b73 707d 7d20 5c66 7261 637b  ^{N_{sp}} \frac{
-00004450: 595f 6b7d 7b57 5f6b 7d20 5c72 6967 6874  Y_k}{W_k} \right
-00004460: 5d5e 7b2d 317d 0a0a 2020 2020 2020 2020  ]^{-1}..        
-00004470: 3a72 6574 7572 6e73 3a20 2a2a 6d69 785f  :returns: **mix_
-00004480: 6d77 2a2a 2028 666c 6f61 7429 202d 204d  mw** (float) - M
-00004490: 6978 7475 7265 206d 6f6c 6563 756c 6172  ixture molecular
-000044a0: 2077 6569 6768 740a 2020 2020 2020 2020   weight.        
-000044b0: 7271 0000 007a 356d 735f 7468 6572 6d6f  rq...z5ms_thermo
-000044c0: 2e73 7461 7465 2e6d 6978 5f6d 6f6c 6563  .state.mix_molec
-000044d0: 756c 6172 5f77 6569 6768 7428 2920 6973  ular_weight() is
-000044e0: 2064 6570 7265 6361 7465 642c 7a21 7573   deprecated,z!us
-000044f0: 6520 696e 7374 6561 6420 6d73 5f74 6865  e instead ms_the
-00004500: 726d 6f2e 7374 6174 652e 6d69 785f 7729  rmo.state.mix_w)
-00004510: 0572 7200 0000 7273 0000 0072 7400 0000  .rr...rs...rt...
-00004520: 725d 0000 0072 1200 0000 7275 0000 0072  r]...r....ru...r
-00004530: 1c00 0000 721c 0000 0072 1d00 0000 da14  ....r....r......
-00004540: 6d69 785f 6d6f 6c65 6375 6c61 725f 7765  mix_molecular_we
-00004550: 6967 6874 3602 0000 730c 0000 0000 080a  ight6...s.......
-00004560: 0104 0108 010a 0108 017a 1a53 7461 7465  .........z.State
-00004570: 2e6d 6978 5f6d 6f6c 6563 756c 6172 5f77  .mix_molecular_w
-00004580: 6569 6768 7429 044e 7208 0000 0072 0900  eight).Nr....r..
-00004590: 0000 4e29 014e 2903 4e4e 4e29 044e 4e72  ..N).N).NNN).NNr
-000045a0: 5500 0000 4629 2072 6700 0000 da0a 5f5f  U...F) rg.....__
-000045b0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000045c0: 6e61 6d65 5f5f da07 5f5f 646f 635f 5f72  name__..__doc__r
-000045d0: 1e00 0000 722a 0000 00da 0b63 6c61 7373  ....r*.....class
-000045e0: 6d65 7468 6f64 7230 0000 00da 0870 726f  methodr0.....pro
-000045f0: 7065 7274 7972 3200 0000 da06 7365 7474  pertyr2.....sett
-00004600: 6572 7219 0000 0072 1a00 0000 723b 0000  err....r....r;..
-00004610: 0072 3900 0000 723a 0000 0072 4200 0000  .r9...r:...rB...
-00004620: 7240 0000 0072 1200 0000 7249 0000 0072  r@...r....rI...r
-00004630: 4d00 0000 724f 0000 0072 1400 0000 7253  M...rO...r....rS
-00004640: 0000 0072 5400 0000 7262 0000 0072 6400  ...rT...rb...rd.
-00004650: 0000 720e 0000 0072 1100 0000 722c 0000  ..r....r....r,..
-00004660: 0072 7600 0000 7277 0000 0072 1c00 0000  .rv...rw...r....
-00004670: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-00004680: 0700 0000 3b00 0000 7364 0000 0008 0104  ....;...sd......
-00004690: 0400 0100 0100 0100 fb0a 2308 1f02 010c  ..........#.....
-000046a0: 1b02 010a 0804 010a 0c02 010a 0804 010a  ................
-000046b0: 0502 010a 0804 010a 0302 010a 0902 010a  ................
-000046c0: 1502 010a 0d02 010a 0e02 010a 0902 010a  ................
-000046d0: 1008 0c08 1408 1508 1408 110a 1f00 0100  ................
-000046e0: 0100 0100 fa0a 4108 0d08 0b08 1f08 1408  ......A.........
-000046f0: 0e29 1072 7a00 0000 7265 0000 00da 056e  .).rz...re.....n
-00004700: 756d 7079 7222 0000 00da 0e73 6369 7079  umpyr".....scipy
-00004710: 2e6f 7074 696d 697a 6572 0200 0000 da0b  .optimizer......
-00004720: 7363 6970 792e 7374 6174 7372 0300 0000  scipy.statsr....
-00004730: 5a11 6d73 5f74 6865 726d 6f2e 7370 6563  Z.ms_thermo.spec
-00004740: 6965 7372 0400 0000 5a13 6d73 5f74 6865  iesr....Z.ms_the
-00004750: 726d 6f2e 636f 6e73 7461 6e74 7372 0500  rmo.constantsr..
-00004760: 0000 7206 0000 0072 7200 0000 da07 5f5f  ..r....rr.....__
-00004770: 616c 6c5f 5f72 0700 0000 721c 0000 0072  all__r....r....r
-00004780: 1c00 0000 721c 0000 0072 1d00 0000 da08  ....r....r......
-00004790: 3c6d 6f64 756c 653e 0100 0000 7312 0000  <module>....s...
-000047a0: 0004 2f08 0108 010c 010c 010c 0110 0108  ../.............
-000047b0: 0206 03                                  ...
+00000000: a70d 0d0a 0000 0000 be15 ad64 cc32 0000  ...........d.2..
+00000010: e300 0000 0000 0000 0000 0000 0002 0000  ................
+00000020: 0000 0000 00f3 ac00 0000 9700 6400 5a00  ............d.Z.
+00000030: 6401 6402 6c01 5a01 6401 6402 6c02 5a02  d.d.l.Z.d.d.l.Z.
+00000040: 6401 6402 6c03 5a03 6401 6402 6c04 5a05  d.d.l.Z.d.d.l.Z.
+00000050: 6401 6403 6c06 6d07 5a07 0100 6401 6402  d.d.l.m.Z...d.d.
+00000060: 6c08 5a08 6401 6402 6c09 5a09 6401 6404  l.Z.d.d.l.Z.d.d.
+00000070: 6c0a 6d0b 5a0b 0100 6405 5a0c 6700 6406  l.m.Z...d.Z.g.d.
+00000080: a201 5a0d 6414 6408 8401 5a0e 6409 8400  ..Z.d.d...Z.d...
+00000090: 5a0f 640a 8400 5a10 0900 0900 0900 0900  Z.d...Z.........
+000000a0: 6415 640c 8401 5a11 640d 8400 5a12 640e  d.d...Z.d...Z.d.
+000000b0: 8400 5a13 640f 8400 5a14 6410 8400 5a15  ..Z.d...Z.d...Z.
+000000c0: 6411 8400 5a16 6412 8400 5a17 6413 8400  d...Z.d...Z.d...
+000000d0: 5a18 6402 5300 2916 7a3f 4d6f 6475 6c65  Z.d.S.).z?Module
+000000e0: 2077 6974 6820 6675 6e63 7469 6f6e 7320   with functions 
+000000f0: 6865 6c70 6572 7320 746f 2020 6372 6561  helpers to  crea
+00000100: 7465 2067 6173 6f75 7420 666f 7220 4346  te gasout for CF
+00000110: 4420 736f 6c76 6572 73e9 0000 0000 4e29  D solvers.....N)
+00000120: 01da 0768 6466 6469 6374 2901 da05 5374  ...hdfdict)...St
+00000130: 6174 657a 770a 2020 2023 2323 2047 6173  atezw.   ### Gas
+00000140: 6f75 7420 746f 6f6c 2066 726f 6d20 6d73  out tool from ms
+00000150: 5f74 6865 726d 6f20 7061 636b 6167 6520  _thermo package 
+00000160: 2323 230a 0a20 2020 2054 6869 7320 6973  ###..    This is
+00000170: 2061 2064 656d 6f6e 7374 7261 746f 7221   a demonstrator!
+00000180: 0a20 2020 2049 7420 6861 7320 6e6f 7420  .    It has not 
+00000190: 6265 656e 2074 686f 726f 7567 6879 2074  been thoroughy t
+000001a0: 6573 7465 6420 7965 7421 0a0a 2909 da11  ested yet!..)...
+000001b0: 6761 736f 7574 5f77 6974 685f 696e 7075  gasout_with_inpu
+000001c0: 74da 1967 6173 6f75 745f 6475 6d70 5f64  t..gasout_dump_d
+000001d0: 6566 6175 6c74 5f69 6e70 7574 da0b 616c  efault_input..al
+000001e0: 7465 725f 7374 6174 65da 1373 7068 6572  ter_state..spher
+000001f0: 6963 616c 5f74 616e 685f 6d61 736b da17  ical_tanh_mask..
+00000200: 6469 7265 6374 696f 6e61 6c5f 6c69 6e65  directional_line
+00000210: 6172 5f6d 6173 6bda 0f66 7261 6374 696f  ar_mask..fractio
+00000220: 6e5f 7a5f 6d61 736b da16 6c6f 6164 5f6d  n_z_mask..load_m
+00000230: 6573 685f 616e 645f 736f 6c75 7469 6f6e  esh_and_solution
+00000240: da12 7361 7665 5f64 6174 615f 666f 725f  ..save_data_for_
+00000250: 6176 6270 da0b 6761 736f 7574 5f74 6f6f  avbp..gasout_too
+00000260: 6c46 6306 0000 0000 0000 0000 0000 0006  lFc.............
+00000270: 0000 0003 0000 00f3 a202 0000 9700 7401  ..............t.
+00000280: 0000 0000 0000 0000 0000 a600 0000 ab00  ................
+00000290: 0000 0000 0000 0000 7d06 7c04 81c6 7403  ........}.|...t.
+000002a0: 0000 0000 0000 0000 0000 a600 0000 ab00  ................
+000002b0: 0000 0000 0000 0000 7d07 7405 0000 0000  ........}.t.....
+000002c0: 0000 0000 0000 7c00 6a03 0000 0000 0000  ......|.j.......
+000002d0: 0000 a004 0000 0000 0000 0000 0000 0000  ................
+000002e0: 0000 0000 0000 0000 a600 0000 ab00 0000  ................
+000002f0: 0000 0000 0000 a601 0000 ab01 0000 0000  ................
+00000300: 0000 0000 7d08 7c04 4400 5d4c 7d09 7c09  ....}.|.D.]L}.|.
+00000310: 7c08 7601 7246 6402 7d0a 7c0a 6403 7401  |.v.rFd.}.|.d.t.
+00000320: 0000 0000 0000 0000 0000 7c09 a601 0000  ..........|.....
+00000330: ab01 0000 0000 0000 0000 7a00 0000 6404  ..........z...d.
+00000340: 7a00 0000 7a0d 0000 7d0a 7c0a 6405 a005  z...z...}.|.d...
+00000350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000360: 0000 0000 7c08 a601 0000 ab01 0000 0000  ....|...........
+00000370: 0000 0000 7a0d 0000 7d0a 7c0a 6406 7a0d  ....z...}.|.d.z.
+00000380: 0000 7d0a 740d 0000 0000 0000 0000 0000  ..}.t...........
+00000390: 7c0a a601 0000 ab01 0000 0000 0000 0000  |...............
+000003a0: 8201 8c4d 7c00 6a03 0000 0000 0000 0000  ...M|.j.........
+000003b0: 4400 5d34 7d09 6407 7d0b 7c09 7c04 7600  D.]4}.d.}.|.|.v.
+000003c0: 7208 7c04 7c09 1900 0000 0000 0000 0000  r.|.|...........
+000003d0: 7d0b 7c00 6a03 0000 0000 0000 0000 7c09  }.|.j.........|.
+000003e0: 1900 0000 0000 0000 0000 7c01 7c0b 7c00  ..........|.|.|.
+000003f0: 6a03 0000 0000 0000 0000 7c09 1900 0000  j.........|.....
+00000400: 0000 0000 0000 7a0a 0000 7a05 0000 7a00  ......z...z...z.
+00000410: 0000 7c07 7c09 3c00 0000 8c35 7c07 7c00  ..|.|.<....5|.|.
+00000420: 5f03 0000 0000 0000 0000 7c02 8129 740f  _.........|..)t.
+00000430: 0000 0000 0000 0000 0000 6a08 0000 0000  ..........j.....
+00000440: 0000 0000 7c00 6a09 0000 0000 0000 0000  ....|.j.........
+00000450: a601 0000 ab01 0000 0000 0000 0000 7d0c  ..............}.
+00000460: 7c0c 7c01 7c02 7c0c 7a0a 0000 7a05 0000  |.|.|.|.z...z...
+00000470: 7a00 0000 7c00 5f09 0000 0000 0000 0000  z...|._.........
+00000480: 7c03 811a 7c00 6a0a 0000 0000 0000 0000  |...|.j.........
+00000490: 7c01 7c03 7c00 6a0a 0000 0000 0000 0000  |.|.|.j.........
+000004a0: 7a0a 0000 7a05 0000 7a00 0000 7c00 5f0a  z...z...z...|._.
+000004b0: 0000 0000 0000 0000 7c05 722f 6408 740f  ........|.r/d.t.
+000004c0: 0000 0000 0000 0000 0000 6a0b 0000 0000  ..........j.....
+000004d0: 0000 0000 7c01 a601 0000 ab01 0000 0000  ....|...........
+000004e0: 0000 0000 7a05 0000 7c01 6a0c 0000 0000  ....z...|.j.....
+000004f0: 0000 0000 6407 1900 0000 0000 0000 0000  ....d...........
+00000500: 7a0b 0000 7d0d 7c06 6409 7c0d 640a 9b04  z...}.|.d.|.d...
+00000510: 640b 9d03 7a0d 0000 7d06 7c06 5300 290c  d...z...}.|.S.).
+00000520: 61cb 0200 000a 2020 2020 4170 706c 7920  a.....    Apply 
+00000530: 6761 736f 7574 2061 6c74 6572 6174 696f  gasout alteratio
+00000540: 6e73 2074 6f20 6120 5374 6174 652e 0a0a  ns to a State...
+00000550: 2020 2020 3a70 6172 616d 2073 7461 7465      :param state
+00000560: 3a20 5374 6174 6520 6265 666f 7265 2061  : State before a
+00000570: 6c74 6572 6174 696f 6e73 0a20 2020 203a  lterations.    :
+00000580: 7479 7065 2073 7461 7465 3a20 5374 6174  type state: Stat
+00000590: 650a 2020 2020 3a70 6172 616d 2061 6c70  e.    :param alp
+000005a0: 6861 3a20 416c 7465 7261 7469 6f6e 206d  ha: Alteration m
+000005b0: 6173 6b20 7769 7468 2076 616c 7565 7320  ask with values 
+000005c0: 6672 6f6d 2030 2028 6e6f 2061 6c74 6572  from 0 (no alter
+000005d0: 6174 696f 6e29 2074 6f20 3120 2866 756c  ation) to 1 (ful
+000005e0: 6c20 616c 7465 7261 7469 6f6e 290a 2020  l alteration).  
+000005f0: 2020 3a74 7970 6520 616c 7068 613a 206e    :type alpha: n
+00000600: 6461 7272 6179 206f 7220 7363 616c 6172  darray or scalar
+00000610: 0a20 2020 203a 7061 7261 6d20 7465 6d70  .    :param temp
+00000620: 5f6e 6577 3a20 4e65 7720 7465 6d70 6572  _new: New temper
+00000630: 6174 7572 6520 746f 2061 7070 6c79 2c20  ature to apply, 
+00000640: 6465 6661 756c 7473 2074 6f20 4e6f 6e65  defaults to None
+00000650: 0a20 2020 203a 7479 7065 2074 656d 705f  .    :type temp_
+00000660: 6e65 773a 206e 6461 7272 6179 206f 7220  new: ndarray or 
+00000670: 7363 616c 6172 2c20 6f70 7469 6f6e 616c  scalar, optional
+00000680: 0a20 2020 203a 7061 7261 6d20 7072 6573  .    :param pres
+00000690: 735f 6e65 773a 204e 6577 2074 656d 7065  s_new: New tempe
+000006a0: 7261 7475 7265 2074 6f20 6170 706c 792c  rature to apply,
+000006b0: 2064 6566 6175 6c74 7320 746f 204e 6f6e   defaults to Non
+000006c0: 650a 2020 2020 3a74 7970 6520 7072 6573  e.    :type pres
+000006d0: 735f 6e65 773a 206e 6461 7272 6179 206f  s_new: ndarray o
+000006e0: 7220 7363 616c 6172 2c20 6f70 7469 6f6e  r scalar, option
+000006f0: 616c 0a20 2020 203a 7061 7261 6d20 795f  al.    :param y_
+00000700: 6e65 773a 204e 6577 206d 6173 7320 6672  new: New mass fr
+00000710: 6163 7469 6f6e 7320 746f 2061 7070 6c79  actions to apply
+00000720: 2c20 6465 6661 756c 7473 2074 6f20 4e6f  , defaults to No
+00000730: 6e65 0a20 2020 203a 7479 7065 2079 5f6e  ne.    :type y_n
+00000740: 6577 3a20 6469 6374 5b73 7472 2c20 6e64  ew: dict[str, nd
+00000750: 6172 7261 7920 6f72 2073 6361 6c61 725d  array or scalar]
+00000760: 2c20 6f70 7469 6f6e 616c 0a20 2020 203a  , optional.    :
+00000770: 7061 7261 6d20 7665 7262 6f73 653a 2056  param verbose: V
+00000780: 6572 626f 7369 7479 2c20 6465 6661 756c  erbosity, defaul
+00000790: 7473 2074 6f20 4661 6c73 650a 2020 2020  ts to False.    
+000007a0: 3a74 7970 6520 7665 7262 6f73 653a 2062  :type verbose: b
+000007b0: 6f6f 6c2c 206f 7074 696f 6e61 6c0a 0a20  ool, optional.. 
+000007c0: 2020 203a 7265 7475 726e 733a 206c 6f67     :returns: log
+000007d0: 2c20 6465 6275 6720 6c6f 670a 2020 2020  , debug log.    
+000007e0: 3a72 7479 7065 3a20 7374 720a 2020 2020  :rtype: str.    
+000007f0: 4e7a 140a 0a20 5370 6563 6965 7320 6d69  Nz... Species mi
+00000800: 736d 6174 6368 3ada 010a 7a1d 2069 7320  smatch:...z. is 
+00000810: 6e6f 7420 7061 7274 206f 6620 7468 6520  not part of the 
+00000820: 6d69 7874 7572 653a 0afa 012f fa27 0a43  mixture:.../.'.C
+00000830: 6865 636b 2079 6f75 7220 696e 7075 7420  heck your input 
+00000840: 6669 6c65 2070 7265 7474 7920 706c 6561  file pretty plea
+00000850: 7365 2e2e 2e72 0200 0000 6700 0000 0000  se...r....g.....
+00000860: 0059 407a 0c46 6f6f 7470 7269 6e74 203a  .Y@z.Footprint :
+00000870: 207a 0420 2e33 667a 0220 2529 0dda 0373   z. .3fz. %)...s
+00000880: 7472 da04 6469 6374 da04 6c69 7374 da0a  tr..dict..list..
+00000890: 6d61 7373 5f66 7261 6373 da04 6b65 7973  mass_fracs..keys
+000008a0: da04 6a6f 696e da0e 5275 6e74 696d 6557  ..join..RuntimeW
+000008b0: 6172 6e69 6e67 da02 6e70 da05 6172 7261  arning..np..arra
+000008c0: 79da 0b74 656d 7065 7261 7475 7265 da08  y..temperature..
+000008d0: 7072 6573 7375 7265 da03 7375 6dda 0573  pressure..sum..s
+000008e0: 6861 7065 290e da05 7374 6174 65da 0561  hape)...state..a
+000008f0: 6c70 6861 da08 7465 6d70 5f6e 6577 da09  lpha..temp_new..
+00000900: 7072 6573 735f 6e65 77da 0579 5f6e 6577  press_new..y_new
+00000910: da07 7665 7262 6f73 65da 036c 6f67 da05  ..verbose..log..
+00000920: 795f 6d69 78da 0d73 7461 7465 5f73 7065  y_mix..state_spe
+00000930: 6369 6573 da04 7370 6563 da06 6d73 6765  cies..spec..msge
+00000940: 7272 da05 7661 6c75 65da 0474 656d 70da  rr..value..temp.
+00000950: 0966 6f6f 7470 7269 6e74 730e 0000 0020  .footprints.... 
+00000960: 2020 2020 2020 2020 2020 2020 20fa 382f               .8/
+00000970: 5573 6572 732f 6461 7570 7461 696e 2f47  Users/dauptain/G
+00000980: 4954 4c41 422f 6d73 5f74 6865 726d 6f2f  ITLAB/ms_thermo/
+00000990: 7372 632f 6d73 5f74 6865 726d 6f2f 6761  src/ms_thermo/ga
+000009a0: 736f 7574 2e70 7972 0700 0000 7207 0000  sout.pyr....r...
+000009b0: 0022 0000 0073 9d01 0000 8000 f528 000b  ."...s.......(..
+000009c0: 0e89 258c 2580 43f0 0600 080d d007 18dd  ..%.%.C.........
+000009d0: 1014 9106 9406 8805 dd18 1c98 55d4 1d2d  ............U..-
+000009e0: d71d 32d2 1d32 d11d 34d4 1d34 d118 35d4  ..2..2..4..4..5.
+000009f0: 1835 880d e014 19f0 0006 092d f000 0609  .5.........-....
+00000a00: 2d88 44d8 0f13 983d d00f 28d0 0f28 d819  -.D....=..(..(..
+00000a10: 3190 06d8 1016 9824 a513 a054 a119 a419  1......$...T....
+00000a20: d11a 2ad0 2d4d d11a 4dd1 104d 9006 d810  ..*.-M..M..M....
+00000a30: 1698 239f 289a 28a0 3dd1 1a31 d41a 31d1  ..#.(.(.=..1..1.
+00000a40: 1031 9006 d810 16d0 1a44 d110 4490 06dd  .1.......D..D...
+00000a50: 1624 a056 d116 2cd4 162c d010 2cf0 0b00  .$.V..,..,..,...
+00000a60: 1029 f00e 0015 1ad4 1424 f000 0709 0ef0  .).......$......
+00000a70: 0007 090e 8844 d814 1588 45d8 0f13 9075  .....D....E....u
+00000a80: 887d 887d d818 1d98 649c 0b90 05e0 1a1f  .}.}....d.......
+00000a90: d41a 2aa8 34d4 1a30 b035 d810 1598 05d4  ..*.4..0.5......
+00000aa0: 1828 a814 d418 2ed1 102e f103 0234 0ef1  .(...........4..
+00000ab0: 0002 1b0e 8845 9024 894b 884b f006 001c  .....E.$.K.K....
+00000ac0: 2188 05d4 0818 e007 0fd0 071b dd0f 118c  !...............
+00000ad0: 7898 05d4 1829 d10f 2ad4 0f2a 8804 d81c  x....)..*..*....
+00000ae0: 20a0 35a8 48b0 74a9 4fd1 233c d11c 3c88   .5.H.t.O.#<..<.
+00000af0: 05d4 0819 e007 10d0 071c d819 1e9c 1ea8  ................
+00000b00: 25b0 39b8 75bc 7ed1 334d d12a 4ed1 194e  %.9.u.~.3M.*N..N
+00000b10: 8805 8c0e e007 0ef0 0002 0531 d814 199d  ...........1....
+00000b20: 429c 46a0 3599 4d9c 4dd1 1429 a845 ac4b  B.F.5.M.M..).E.K
+00000b30: b801 ac4e d114 3a88 09d8 080b d00f 3098  ...N..:.......0.
+00000b40: 69d0 0f30 d00f 30d0 0f30 d00f 30d1 0830  i..0..0..0..0..0
+00000b50: 8803 d80b 0e80 4af3 0000 0000 6304 0000  ......J.....c...
+00000b60: 0000 0000 0000 0000 0007 0000 0003 0000  ................
+00000b70: 00f3 8801 0000 9700 7401 0000 0000 0000  ........t.......
+00000b80: 0000 0000 6a01 0000 0000 0000 0000 7c01  ....j.........|.
+00000b90: a601 0000 ab01 0000 0000 0000 0000 7d01  ..............}.
+00000ba0: 7c01 6a02 0000 0000 0000 0000 6401 1900  |.j.........d...
+00000bb0: 0000 0000 0000 0000 7d04 7c00 6a02 0000  ........}.|.j...
+00000bc0: 0000 0000 0000 6402 1900 0000 0000 0000  ......d.........
+00000bd0: 0000 7d05 7c04 7c05 6b03 0000 0000 7246  ..}.|.|.k.....rF
+00000be0: 6403 7d06 7c06 6404 7407 0000 0000 0000  d.}.|.d.t.......
+00000bf0: 0000 0000 7c04 a601 0000 ab01 0000 0000  ....|...........
+00000c00: 0000 0000 7a00 0000 6405 7a00 0000 7a0d  ....z...d.z...z.
+00000c10: 0000 7d06 7c06 6406 7407 0000 0000 0000  ..}.|.d.t.......
+00000c20: 0000 0000 7c05 a601 0000 ab01 0000 0000  ....|...........
+00000c30: 0000 0000 7a00 0000 6405 7a00 0000 7a0d  ....z...d.z...z.
+00000c40: 0000 7d06 7c06 6407 7a0d 0000 7d06 7409  ..}.|.d.z...}.t.
+00000c50: 0000 0000 0000 0000 0000 7c06 a601 0000  ..........|.....
+00000c60: ab01 0000 0000 0000 0000 8201 7400 0000  ............t...
+00000c70: 0000 0000 0000 0000 6a05 0000 0000 0000  ........j.......
+00000c80: 0000 a006 0000 0000 0000 0000 0000 0000  ................
+00000c90: 0000 0000 0000 0000 7c00 7c01 7a0a 0000  ........|.|.z...
+00000ca0: 6408 ac09 a602 0000 ab02 0000 0000 0000  d...............
+00000cb0: 0000 7d07 640a 640b 7401 0000 0000 0000  ..}.d.d.t.......
+00000cc0: 0000 0000 6a07 0000 0000 0000 0000 7c07  ....j.........|.
+00000cd0: 7c02 7a0a 0000 7c03 640c 7a0b 0000 7a0b  |.z...|.d.z...z.
+00000ce0: 0000 a601 0000 ab01 0000 0000 0000 0000  ................
+00000cf0: 7a0a 0000 7a05 0000 7d08 7c08 5300 290d  z...z...}.|.S.).
+00000d00: 61f4 0100 000a 2020 2020 4465 6669 6e65  a.....    Define
+00000d10: 2061 2073 7068 6572 6963 616c 206d 6173   a spherical mas
+00000d20: 6b2e 2030 2069 6e73 6964 6520 7468 6520  k. 0 inside the 
+00000d30: 7370 6865 7265 2c20 3120 6f75 7473 6964  sphere, 1 outsid
+00000d40: 652c 2077 6974 6820 6120 7461 6e68 2074  e, with a tanh t
+00000d50: 7261 6e73 6974 696f 6e2e 0a0a 2020 2020  ransition...    
+00000d60: 3a70 6172 616d 2063 6f6f 723a 2041 7272  :param coor: Arr
+00000d70: 6179 206f 6620 7370 6174 6961 6c20 636f  ay of spatial co
+00000d80: 6f72 6469 6e61 7465 7320 2873 6861 7065  ordinates (shape
+00000d90: 2028 6e2c 206e 6469 6d29 290a 2020 2020   (n, ndim)).    
+00000da0: 3a74 7970 6520 636f 6f72 3a20 6e64 6172  :type coor: ndar
+00000db0: 7261 790a 2020 2020 3a70 6172 616d 2063  ray.    :param c
+00000dc0: 656e 7465 723a 2041 7272 6179 206f 6620  enter: Array of 
+00000dd0: 7370 6865 7265 2063 656e 7465 7220 636f  sphere center co
+00000de0: 6f72 6469 6e61 7465 7320 2873 6861 7065  ordinates (shape
+00000df0: 2028 6e64 696d 2c29 290a 2020 2020 3a74   (ndim,)).    :t
+00000e00: 7970 6520 6365 6e74 6572 3a20 6c69 7374  ype center: list
+00000e10: 2c20 7475 706c 6520 6f72 206e 6461 7272  , tuple or ndarr
+00000e20: 6179 0a20 2020 203a 7061 7261 6d20 7261  ay.    :param ra
+00000e30: 6469 7573 3a20 5261 6469 7573 206f 6620  dius: Radius of 
+00000e40: 7468 6520 7370 6865 7265 0a20 2020 203a  the sphere.    :
+00000e50: 7479 7065 2072 6164 6975 733a 2066 6c6f  type radius: flo
+00000e60: 6174 0a20 2020 203a 7061 7261 6d20 6465  at.    :param de
+00000e70: 6c74 613a 2054 7261 6e73 6974 696f 6e20  lta: Transition 
+00000e80: 7468 6963 6b6e 6573 7320 6174 2074 6865  thickness at the
+00000e90: 2065 6467 6520 6f66 2074 6865 2073 7068   edge of the sph
+00000ea0: 6572 650a 2020 2020 3a74 7970 6520 6465  ere.    :type de
+00000eb0: 6c74 613a 2066 6c6f 6174 0a0a 2020 2020  lta: float..    
+00000ec0: 3a72 6574 7572 6e73 3a20 616c 7068 612c  :returns: alpha,
+00000ed0: 2061 6c74 6572 6174 696f 6e20 6d61 736b   alteration mask
+00000ee0: 0a20 2020 203a 7274 7970 653a 206e 6461  .    :rtype: nda
+00000ef0: 7272 6179 0a20 2020 2072 0200 0000 e9ff  rray.    r......
+00000f00: ffff ff7a 2c0a 0a44 696d 656e 7369 6f6e  ...z,..Dimension
+00000f10: 206d 6973 6d61 7463 6820 696e 2074 6865   mismatch in the
+00000f20: 2073 7068 6572 6963 616c 2063 656e 7465   spherical cente
+00000f30: 727a 0b0a 4365 6e74 6572 2069 7320 da01  rz..Center is ..
+00000f40: 447a 0c0a 436f 6f72 6473 2061 7265 2072  Dz..Coords are r
+00000f50: 1100 0000 e901 0000 00a9 01da 0461 7869  .............axi
+00000f60: 73e7 0000 0000 0000 e03f e700 0000 0000  s........?......
+00000f70: 00f0 3fe9 0200 0000 2908 7219 0000 0072  ..?.....).r....r
+00000f80: 1a00 0000 721e 0000 0072 1200 0000 7218  ....r....r....r.
+00000f90: 0000 00da 066c 696e 616c 67da 046e 6f72  .....linalg..nor
+00000fa0: 6dda 0474 616e 6829 09da 0463 6f6f 72da  m..tanh)...coor.
+00000fb0: 0663 656e 7465 72da 0672 6164 6975 73da  .center..radius.
+00000fc0: 0564 656c 7461 da0b 6365 6e74 6572 5f6e  .delta..center_n
+00000fd0: 6469 6dda 0963 6f6f 725f 6e64 696d da07  dim..coor_ndim..
+00000fe0: 6d73 675f 6572 72da 0672 5f63 6f6f 7272  msg_err..r_coorr
+00000ff0: 2000 0000 7309 0000 0020 2020 2020 2020   ...s....       
+00001000: 2020 722d 0000 0072 0800 0000 7208 0000    r-...r....r...
+00001010: 005c 0000 0073 ce00 0000 8000 f520 000e  .\...s....... ..
+00001020: 108c 5890 66d1 0d1d d40d 1d80 46d8 1218  ..X.f.......F...
+00001030: 942c 9871 942f 804b d810 1494 0a98 3294  .,.q./.K......2.
+00001040: 0e80 49d8 0712 9069 d207 1fd0 071f d812  ..I....i........
+00001050: 4288 07d8 080f 903e a543 a80b d124 34d4  B......>.C...$4.
+00001060: 2434 d113 34b0 73d1 133a d108 3a88 07d8  $4..4.s..:..:...
+00001070: 080f 903f a553 a819 a15e a45e d113 33b0  ...?.S...^.^..3.
+00001080: 63d1 1339 d108 3988 07d8 080f d013 3dd1  c..9..9.......=.
+00001090: 083d 8807 dd0e 1c98 57d1 0e25 d40e 25d0  .=......W..%..%.
+000010a0: 0825 e50d 0f8c 598f 5e8a 5e98 44a0 3699  .%....Y.^.^.D.6.
+000010b0: 4db0 0188 5ed1 0d32 d40d 3280 46d8 0c0f  M...^..2..2.F...
+000010c0: 9033 9d12 9c17 a026 a836 a12f b065 b861  .3.....&.6./.e.a
+000010d0: b169 d121 40d1 1941 d419 41d1 1341 d10c  .i.!@..A..A..A..
+000010e0: 4280 45d8 0b10 804c 722e 0000 0063 0400  B.E....Lr....c..
+000010f0: 0000 0000 0000 0000 0000 0500 0000 0300  ................
+00001100: 0000 f360 0000 0097 007c 0064 0164 0185  ...`.....|.d.d..
+00001110: 027c 0166 0219 0000 0000 0000 0000 007d  .|.f...........}
+00001120: 047c 047c 027a 0a00 007c 037c 027a 0a00  .|.|.z...|.|.z..
+00001130: 007a 0b00 007d 0574 0100 0000 0000 0000  .z...}.t........
+00001140: 0000 006a 0100 0000 0000 0000 007c 0564  ...j.........|.d
+00001150: 0264 03a6 0300 00ab 0300 0000 0000 0000  .d..............
+00001160: 007d 057c 0553 0029 0461 2903 0000 0a20  .}.|.S.).a).... 
+00001170: 2020 2044 6566 696e 6520 6120 6469 7265     Define a dire
+00001180: 6374 696f 6e61 6c20 6d61 736b 2061 6c69  ctional mask ali
+00001190: 676e 6564 2077 6974 6820 7468 6520 6061  gned with the `a
+000011a0: 7869 7360 2063 6f6f 7264 696e 6174 6520  xis` coordinate 
+000011b0: 6178 6973 2e0a 0a20 2020 2049 6620 6074  axis...    If `t
+000011c0: 7261 6e73 6974 696f 6e5f 656e 6460 203e  ransition_end` >
+000011d0: 2060 7472 616e 7369 7469 6f6e 5f73 7461   `transition_sta
+000011e0: 7274 602c 2074 6865 206d 6173 6b20 6973  rt`, the mask is
+000011f0: 2030 2062 6566 6f72 6520 6074 7261 6e73   0 before `trans
+00001200: 6974 696f 6e5f 7374 6172 7460 2061 6e64  ition_start` and
+00001210: 0a20 2020 2031 2061 6674 6572 2060 7472  .    1 after `tr
+00001220: 616e 7369 7469 6f6e 5f65 6e64 2e0a 2020  ansition_end..  
+00001230: 2020 4966 2060 7472 616e 7369 7469 6f6e    If `transition
+00001240: 5f73 7461 7274 6020 3e20 6074 7261 6e73  _start` > `trans
+00001250: 6974 696f 6e5f 656e 6460 2c20 7468 6520  ition_end`, the 
+00001260: 6d61 736b 2069 7320 3120 6265 666f 7265  mask is 1 before
+00001270: 2060 7472 616e 7369 7469 6f6e 5f65 6e64   `transition_end
+00001280: 6020 616e 640a 2020 2020 3020 6166 7465  ` and.    0 afte
+00001290: 7220 6074 7261 6e73 6974 696f 6e5f 7374  r `transition_st
+000012a0: 6172 742e 0a20 2020 2041 206c 696e 6561  art..    A linea
+000012b0: 7220 7472 616e 7369 7469 6f6e 2069 7320  r transition is 
+000012c0: 696d 706f 7365 6420 6265 7477 6565 6e20  imposed between 
+000012d0: 6074 7261 6e73 6974 696f 6e5f 7374 6172  `transition_star
+000012e0: 7460 2061 6e64 2060 7472 616e 7369 7469  t` and `transiti
+000012f0: 6f6e 5f65 6e64 602e 0a0a 2020 2020 3a70  on_end`...    :p
+00001300: 6172 616d 2063 6f6f 723a 2041 7272 6179  aram coor: Array
+00001310: 206f 6620 7370 6174 6961 6c20 636f 6f72   of spatial coor
+00001320: 6469 6e61 7465 7320 2873 6861 7065 2028  dinates (shape (
+00001330: 6e2c 206e 6469 6d29 290a 2020 2020 3a74  n, ndim)).    :t
+00001340: 7970 6520 636f 6f72 3a20 6e64 6172 7261  ype coor: ndarra
+00001350: 790a 2020 2020 3a70 6172 616d 2061 7869  y.    :param axi
+00001360: 733a 2043 6f6f 7264 696e 6174 6520 6178  s: Coordinate ax
+00001370: 6973 206f 6620 7468 6520 6d61 736b 2028  is of the mask (
+00001380: 3020 782c 2031 2079 2c20 3220 7a29 0a20  0 x, 1 y, 2 z). 
+00001390: 2020 203a 7479 7065 2061 7869 733a 2069     :type axis: i
+000013a0: 6e74 0a20 2020 203a 7061 7261 6d20 7472  nt.    :param tr
+000013b0: 616e 7369 7469 6f6e 5f73 7461 7274 3a20  ansition_start: 
+000013c0: 5374 6172 7420 706f 696e 7420 6f66 2074  Start point of t
+000013d0: 6865 206c 696e 6561 7220 6d61 736b 0a20  he linear mask. 
+000013e0: 2020 203a 7479 7065 2074 7261 6e73 6974     :type transit
+000013f0: 696f 6e5f 7374 6172 743a 2066 6c6f 6174  ion_start: float
+00001400: 0a20 2020 203a 7061 7261 6d20 7472 616e  .    :param tran
+00001410: 7369 7469 6f6e 5f65 6e64 3a20 456e 6420  sition_end: End 
+00001420: 706f 696e 7420 6f66 2074 6865 206c 696e  point of the lin
+00001430: 6561 7220 6d61 736b 0a20 2020 203a 7479  ear mask.    :ty
+00001440: 7065 2074 7261 6e73 6974 696f 6e5f 656e  pe transition_en
+00001450: 643a 2066 6c6f 6174 0a0a 2020 2020 3a72  d: float..    :r
+00001460: 6574 7572 6e73 3a20 616c 7068 612c 2061  eturns: alpha, a
+00001470: 6c74 6572 6174 696f 6e20 6d61 736b 0a20  lteration mask. 
+00001480: 2020 203a 7274 7970 653a 206e 6461 7272     :rtype: ndarr
+00001490: 6179 0a20 2020 204e 6700 0000 0000 0000  ay.    Ng.......
+000014a0: 0072 3600 0000 2902 7219 0000 00da 0463  .r6...).r......c
+000014b0: 6c69 7029 0672 3b00 0000 7234 0000 00da  lip).r;...r4....
+000014c0: 1074 7261 6e73 6974 696f 6e5f 7374 6172  .transition_star
+000014d0: 74da 0e74 7261 6e73 6974 696f 6e5f 656e  t..transition_en
+000014e0: 64da 0964 6972 6563 7469 6f6e 7220 0000  d..directionr ..
+000014f0: 0073 0600 0000 2020 2020 2020 722d 0000  .s....      r-..
+00001500: 0072 0900 0000 7209 0000 007b 0000 0073  .r....r....{...s
+00001510: 4300 0000 8000 f030 0011 1590 5190 5190  C......0....Q.Q.
+00001520: 5198 0490 5794 0d80 49e0 0d16 d019 29d1  Q...W...I.....).
+00001530: 0d29 a86e d03f 4fd1 2e4f d10c 5080 45dd  .).n.?O..O..P.E.
+00001540: 0c0e 8c47 9045 9833 a003 d10c 24d4 0c24  ...G.E.3....$..$
+00001550: 8045 e00b 1080 4c72 2e00 0000 da01 4363  .E....Lr......Cc
+00001560: 0800 0000 0000 0000 0000 0000 0700 0000  ................
+00001570: 0300 0000 f3ac 0000 0097 007c 00a0 0000  ...........|....
+00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001590: 0000 007c 017c 047c 057c 067c 07a6 0500  ...|.|.|.|.|....
+000015a0: 00ab 0500 0000 0000 0000 007d 0864 017c  ...........}.d.|
+000015b0: 037c 027a 0000 007a 0500 007d 0964 017c  .|.z...z...}.d.|
+000015c0: 037c 027a 0a00 007a 0500 007d 0a74 0300  .|.z...z...}.t..
+000015d0: 0000 0000 0000 0000 006a 0200 0000 0000  .........j......
+000015e0: 0000 0074 0700 0000 0000 0000 0000 007c  ...t...........|
+000015f0: 087c 097a 0a00 00a6 0100 00ab 0100 0000  .|.z............
+00001600: 0000 0000 007c 0a6b 0000 0000 0064 0264  .....|.k.....d.d
+00001610: 03a6 0300 00ab 0300 0000 0000 0000 007d  ...............}
+00001620: 0b7c 0b53 0029 0461 6703 0000 0a20 2020  .|.S.).ag....   
+00001630: 2043 6f6d 7075 7465 2061 206d 6173 6b20   Compute a mask 
+00001640: 6261 7365 6420 6f6e 2074 6865 206d 6978  based on the mix
+00001650: 7475 7265 2066 7261 6374 696f 6e20 5a2e  ture fraction Z.
+00001660: 0a0a 2020 2020 5468 6520 6d61 736b 2069  ..    The mask i
+00001670: 7320 3120 6265 7477 6565 6e20 607a 6d69  s 1 between `zmi
+00001680: 6e60 2061 6e64 2060 7a6d 6178 6020 616e  n` and `zmax` an
+00001690: 6420 3020 6f75 7473 6964 652e 0a0a 2020  d 0 outside...  
+000016a0: 2020 3a70 6172 616d 2073 7461 7465 3a20    :param state: 
+000016b0: 6d73 5f74 6865 726d 6f20 5374 6174 6520  ms_thermo State 
+000016c0: 6f62 6a65 6374 0a20 2020 203a 7479 7065  object.    :type
+000016d0: 2073 7461 7465 3a20 5374 6174 650a 2020   state: State.  
+000016e0: 2020 3a70 6172 616d 2073 7065 6366 7565    :param specfue
+000016f0: 6c3a 2046 7565 6c20 7370 6563 6965 7320  l: Fuel species 
+00001700: 6e61 6d65 0a20 2020 203a 7479 7065 2073  name.    :type s
+00001710: 7065 6366 7565 6c3a 2073 7472 0a20 2020  pecfuel: str.   
+00001720: 203a 7061 7261 6d20 7a6d 696e 3a20 6d61   :param zmin: ma
+00001730: 736b 2064 6973 6162 6c65 6420 2830 2920  sk disabled (0) 
+00001740: 6265 6c6f 7720 7468 6973 2076 616c 7565  below this value
+00001750: 0a20 2020 203a 7479 7065 207a 6d69 6e3a  .    :type zmin:
+00001760: 2066 6c6f 6174 0a20 2020 203a 7061 7261   float.    :para
+00001770: 6d20 7a6d 6178 3a20 6d61 736b 2064 6973  m zmax: mask dis
+00001780: 6162 6c65 6420 2830 2920 6f76 6572 2074  abled (0) over t
+00001790: 6869 7320 7661 6c75 650a 2020 2020 3a74  his value.    :t
+000017a0: 7970 6520 7a6d 6178 3a20 666c 6f61 740a  ype zmax: float.
+000017b0: 2020 2020 3a70 6172 616d 2066 7565 6c5f      :param fuel_
+000017c0: 6d61 7373 5f66 7261 6373 3a20 4675 656c  mass_fracs: Fuel
+000017d0: 206d 6173 7320 6672 6163 7469 6f6e 732c   mass fractions,
+000017e0: 2064 6566 6175 6c74 7320 746f 2063 6f6d   defaults to com
+000017f0: 706f 7369 7469 6f6e 2061 7420 7065 616b  position at peak
+00001800: 2066 7565 6c20 636f 6e63 656e 7472 6174   fuel concentrat
+00001810: 696f 6e0a 2020 2020 3a74 7970 6520 6675  ion.    :type fu
+00001820: 656c 5f6d 6173 735f 6672 6163 733a 2064  el_mass_fracs: d
+00001830: 6963 742c 206f 7074 696f 6e61 6c0a 2020  ict, optional.  
+00001840: 2020 3a70 6172 616d 206f 7879 645f 6d61    :param oxyd_ma
+00001850: 7373 5f66 7261 6373 3a20 4f78 7964 697a  ss_fracs: Oxydiz
+00001860: 6572 206d 6173 7320 6672 6163 7469 6f6e  er mass fraction
+00001870: 732c 2064 6566 6175 6c74 7320 746f 2061  s, defaults to a
+00001880: 6972 0a20 2020 203a 7479 7065 206f 7879  ir.    :type oxy
+00001890: 645f 6d61 7373 5f66 7261 6373 3a20 6469  d_mass_fracs: di
+000018a0: 6374 2c20 6f70 7469 6f6e 616c 0a20 2020  ct, optional.   
+000018b0: 203a 7061 7261 6d20 6174 6f6d 5f72 6566   :param atom_ref
+000018c0: 3a20 5265 6665 7265 6e63 6520 6174 6f6d  : Reference atom
+000018d0: 2c20 6465 6661 756c 7473 2074 6f20 430a  , defaults to C.
+000018e0: 2020 2020 3a74 7970 6520 6174 6f6d 5f72      :type atom_r
+000018f0: 6566 3a20 7374 722c 206f 7074 696f 6e61  ef: str, optiona
+00001900: 6c0a 2020 2020 3a70 6172 616d 2076 6572  l.    :param ver
+00001910: 626f 7365 3a20 5665 7262 6f73 6974 792c  bose: Verbosity,
+00001920: 2064 6566 6175 6c74 7320 746f 2046 616c   defaults to Fal
+00001930: 7365 0a20 2020 203a 7479 7065 2076 6572  se.    :type ver
+00001940: 626f 7365 3a20 626f 6f6c 2c20 6f70 7469  bose: bool, opti
+00001950: 6f6e 616c 0a0a 2020 2020 3a72 6574 7572  onal..    :retur
+00001960: 6e73 3a20 616c 7068 612c 2061 6c74 6572  ns: alpha, alter
+00001970: 6174 696f 6e20 6d61 736b 0a20 2020 203a  ation mask.    :
+00001980: 7274 7970 653a 206e 6461 7272 6179 0a20  rtype: ndarray. 
+00001990: 2020 2072 3500 0000 7236 0000 0072 0200     r5...r6...r..
+000019a0: 0000 2904 da0e 636f 6d70 7574 655f 7a5f  ..)...compute_z_
+000019b0: 6672 6163 7219 0000 00da 0577 6865 7265  fracr......where
+000019c0: da03 6162 7329 0c72 1f00 0000 da08 7370  ..abs).r......sp
+000019d0: 6563 6675 656c da04 7a6d 696e da04 7a6d  ecfuel..zmin..zm
+000019e0: 6178 da0f 6675 656c 5f6d 6173 735f 6672  ax..fuel_mass_fr
+000019f0: 6163 73da 0f6f 7879 645f 6d61 7373 5f66  acs..oxyd_mass_f
+00001a00: 7261 6373 da08 6174 6f6d 5f72 6566 7224  racs..atom_refr$
+00001a10: 0000 00da 067a 5f66 7261 63da 057a 5f6d  .....z_frac..z_m
+00001a20: 6964 da05 7a5f 6761 7072 2000 0000 730c  id..z_gapr ...s.
+00001a30: 0000 0020 2020 2020 2020 2020 2020 2072  ...            r
+00001a40: 2d00 0000 720a 0000 0072 0a00 0000 9b00  -...r....r......
+00001a50: 0000 7370 0000 0080 00f0 4601 000e 13d7  ..sp......F.....
+00001a60: 0d21 d20d 21d8 0810 d808 17d8 0817 d808  .!..!...........
+00001a70: 10d8 080f f10b 060e 06f4 0006 0e06 8046  ...............F
+00001a80: f010 000d 1090 3498 2491 3bd1 0c1f 8045  ......4.$.;....E
+00001a90: d80c 0f90 3498 2491 3bd1 0c1f 8045 dd0c  ....4.$.;....E..
+00001aa0: 0e8c 4895 5398 16a0 2599 1ed1 1528 d415  ..H.S...%....(..
+00001ab0: 28a8 35d2 1530 b023 b071 d10c 39d4 0c39  (.5..0.#.q..9..9
+00001ac0: 8045 d80b 1080 4c72 2e00 0000 6303 0000  .E....Lr....c...
+00001ad0: 0000 0000 0000 0000 000b 0000 0003 0000  ................
+00001ae0: 00f3 6205 0000 9700 7401 0000 0000 0000  ..b.....t.......
+00001af0: 0000 0000 7402 0000 0000 0000 0000 0000  ....t...........
+00001b00: a601 0000 ab01 0000 0000 0000 0000 7d03  ..............}.
+00001b10: 7c03 6401 7a0d 0000 7d03 7c03 6402 7a0d  |.d.z...}.|.d.z.
+00001b20: 0000 7d03 7c03 6403 7c01 a002 0000 0000  ..}.|.d.|.......
+00001b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001b40: a600 0000 ab00 0000 0000 0000 0000 7a00  ..............z.
+00001b50: 0000 7a0d 0000 7d03 7407 0000 0000 0000  ..z...}.t.......
+00001b60: 0000 0000 7c02 6404 1900 0000 0000 0000  ....|.d.........
+00001b70: 0000 a601 0000 ab01 0000 0000 0000 0000  ................
+00001b80: 4400 9002 5d39 5c02 0000 7d04 7d05 7c03  D...]9\...}.}.|.
+00001b90: 6405 7401 0000 0000 0000 0000 0000 7c04  d.t...........|.
+00001ba0: a601 0000 ab01 0000 0000 0000 0000 7a00  ..............z.
+00001bb0: 0000 6406 7a00 0000 7c05 6407 1900 0000  ..d.z...|.d.....
+00001bc0: 0000 0000 0000 7a00 0000 7a0d 0000 7d03  ......z...z...}.
+00001bd0: 7c05 6407 1900 0000 0000 0000 0000 6408  |.d...........d.
+00001be0: 6b02 0000 0000 72ad 6700 6409 a201 7d06  k.....r.g.d...}.
+00001bf0: 7409 0000 0000 0000 0000 0000 7c06 740b  t...........|.t.
+00001c00: 0000 0000 0000 0000 0000 7c05 a006 0000  ..........|.....
+00001c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001c20: 0000 a600 0000 ab00 0000 0000 0000 0000  ................
+00001c30: a601 0000 ab01 0000 0000 0000 0000 a602  ................
+00001c40: 0000 ab02 0000 0000 0000 0000 7d07 7c07  ............}.|.
+00001c50: 640a 6b03 0000 0000 7212 740f 0000 0000  d.k.....r.t.....
+00001c60: 0000 0000 0000 7c03 7c07 7a00 0000 a601  ......|.|.z.....
+00001c70: 0000 ab01 0000 0000 0000 0000 8201 7c05  ..............|.
+00001c80: 640b 1900 0000 0000 0000 0000 640c 6b02  d...........d.k.
+00001c90: 0000 0000 7203 640d 7d08 6e32 7c05 640b  ....r.d.}.n2|.d.
+00001ca0: 1900 0000 0000 0000 0000 640e 6b02 0000  ..........d.k...
+00001cb0: 0000 7203 640f 7d08 6e23 7c05 640b 1900  ..r.d.}.n#|.d...
+00001cc0: 0000 0000 0000 0000 6410 6b02 0000 0000  ........d.k.....
+00001cd0: 7203 6411 7d08 6e14 6412 7d09 740f 0000  r.d.}.n.d.}.t...
+00001ce0: 0000 0000 0000 0000 7c03 7c09 7a00 0000  ........|.|.z...
+00001cf0: a601 0000 ab01 0000 0000 0000 0000 8201  ................
+00001d00: 7411 0000 0000 0000 0000 0000 7c00 7c08  t...........|.|.
+00001d10: 7c05 6413 1900 0000 0000 0000 0000 7c05  |.d...........|.
+00001d20: 6414 1900 0000 0000 0000 0000 ac15 a604  d...............
+00001d30: 0000 ab04 0000 0000 0000 0000 7d0a 9001  ............}...
+00001d40: 6e0f 7c05 6407 1900 0000 0000 0000 0000  n.|.d...........
+00001d50: 6416 6b02 0000 0000 7271 6700 6417 a201  d.k.....rqg.d...
+00001d60: 7d06 7409 0000 0000 0000 0000 0000 7c06  }.t...........|.
+00001d70: 740b 0000 0000 0000 0000 0000 7c05 a006  t...........|...
+00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001d90: 0000 0000 a600 0000 ab00 0000 0000 0000  ................
+00001da0: 0000 a601 0000 ab01 0000 0000 0000 0000  ................
+00001db0: a602 0000 ab02 0000 0000 0000 0000 7d07  ..............}.
+00001dc0: 7c07 640a 6b03 0000 0000 7212 740f 0000  |.d.k.....r.t...
+00001dd0: 0000 0000 0000 0000 7c03 7c07 7a00 0000  ........|.|.z...
+00001de0: a601 0000 ab01 0000 0000 0000 0000 8201  ................
+00001df0: 7413 0000 0000 0000 0000 0000 7c00 7c05  t...........|.|.
+00001e00: 6418 1900 0000 0000 0000 0000 7c05 6419  d...........|.d.
+00001e10: 1900 0000 0000 0000 0000 7c05 641a 1900  ..........|.d...
+00001e20: 0000 0000 0000 0000 ac17 a604 0000 ab04  ................
+00001e30: 0000 0000 0000 0000 7d0a 6e92 7c05 6407  ........}.n.|.d.
+00001e40: 1900 0000 0000 0000 0000 641b 6b02 0000  ..........d.k...
+00001e50: 0000 7286 6700 641c a201 7d06 7409 0000  ..r.g.d...}.t...
+00001e60: 0000 0000 0000 0000 7c06 740b 0000 0000  ........|.t.....
+00001e70: 0000 0000 0000 7c05 a006 0000 0000 0000  ......|.........
+00001e80: 0000 0000 0000 0000 0000 0000 0000 a600  ................
+00001e90: 0000 ab00 0000 0000 0000 0000 a601 0000  ................
+00001ea0: ab01 0000 0000 0000 0000 a602 0000 ab02  ................
+00001eb0: 0000 0000 0000 0000 7d07 7c07 640a 6b03  ........}.|.d.k.
+00001ec0: 0000 0000 7212 740f 0000 0000 0000 0000  ....r.t.........
+00001ed0: 0000 7c03 7c07 7a00 0000 a601 0000 ab01  ..|.|.z.........
+00001ee0: 0000 0000 0000 0000 8201 7415 0000 0000  ..........t.....
+00001ef0: 0000 0000 0000 7c01 7c05 641d 1900 0000  ......|.|.d.....
+00001f00: 0000 0000 0000 7c05 641e 1900 0000 0000  ......|.d.......
+00001f10: 0000 0000 7c05 641f 1900 0000 0000 0000  ....|.d.........
+00001f20: 0000 7c05 6420 1900 0000 0000 0000 0000  ..|.d ..........
+00001f30: 7c05 6421 1900 0000 0000 0000 0000 7c05  |.d!..........|.
+00001f40: 641d 1900 0000 0000 0000 0000 6422 ac23  d...........d".#
+00001f50: a608 0000 ab08 0000 0000 0000 0000 7d0a  ..............}.
+00001f60: 6424 7c05 7601 7205 6425 7c05 6424 3c00  d$|.v.r.d%|.d$<.
+00001f70: 0000 6426 7c05 7601 7205 6425 7c05 6426  ..d&|.v.r.d%|.d&
+00001f80: 3c00 0000 6427 7c05 7601 7205 6425 7c05  <...d'|.v.r.d%|.
+00001f90: 6427 3c00 0000 7417 0000 0000 0000 0000  d'<...t.........
+00001fa0: 0000 7c01 7c0a 7c05 6424 1900 0000 0000  ..|.|.|.d$......
+00001fb0: 0000 0000 7c05 6426 1900 0000 0000 0000  ....|.d&........
+00001fc0: 0000 7c05 6427 1900 0000 0000 0000 0000  ..|.d'..........
+00001fd0: 6422 ac28 a606 0000 ab06 0000 0000 0000  d".(............
+00001fe0: 0000 7d0b 7c03 6403 7c0b 7a00 0000 7a0d  ..}.|.d.|.z...z.
+00001ff0: 0000 7d03 9002 8c3b 7c03 6429 7a0d 0000  ..}....;|.d)z...
+00002000: 7d03 7c03 6402 7a0d 0000 7d03 7c03 6403  }.|.d.z...}.|.d.
+00002010: 7c01 a002 0000 0000 0000 0000 0000 0000  |...............
+00002020: 0000 0000 0000 0000 a600 0000 ab00 0000  ................
+00002030: 0000 0000 0000 7a00 0000 7a0d 0000 7d03  ......z...z...}.
+00002040: 7c01 7c03 6602 5300 292a 6159 0100 000a  |.|.f.S.)*aY....
+00002050: 2020 2020 5570 6461 7465 2061 2053 7461      Update a Sta
+00002060: 7465 2077 6974 6820 6761 736f 7574 2061  te with gasout a
+00002070: 6374 696f 6e73 2e0a 0a20 2020 203a 7061  ctions...    :pa
+00002080: 7261 6d20 636f 6f72 3a20 4172 7261 7920  ram coor: Array 
+00002090: 6f66 2073 7061 7469 616c 2063 6f6f 7264  of spatial coord
+000020a0: 696e 6174 6573 2028 7368 6170 6520 286e  inates (shape (n
+000020b0: 2c20 6e64 696d 2929 0a20 2020 203a 7479  , ndim)).    :ty
+000020c0: 7065 2063 6f6f 723a 206e 6461 7272 6179  pe coor: ndarray
+000020d0: 0a20 2020 203a 7061 7261 6d20 7374 6174  .    :param stat
+000020e0: 653a 206d 735f 7468 6572 6d6f 2053 7461  e: ms_thermo Sta
+000020f0: 7465 206f 626a 6563 740a 2020 2020 3a74  te object.    :t
+00002100: 7970 6520 7374 6174 653a 2053 7461 7465  ype state: State
+00002110: 0a20 2020 203a 7061 7261 6d20 696e 5f6e  .    :param in_n
+00002120: 6f62 3a20 436f 6e74 656e 7473 206f 6620  ob: Contents of 
+00002130: 7468 6520 696e 7075 7420 6669 6c65 0a20  the input file. 
+00002140: 2020 203a 7479 7065 2069 6e5f 6e6f 623a     :type in_nob:
+00002150: 2064 6963 740a 0a20 2020 203a 7265 7475   dict..    :retu
+00002160: 726e 733a 2054 7570 6c65 2063 6f6e 7461  rns: Tuple conta
+00002170: 696e 696e 6720 7468 6520 7570 6461 7465  ining the update
+00002180: 6420 5374 6174 6520 616e 6420 6120 6c6f  d State and a lo
+00002190: 670a 2020 2020 3a72 7479 7065 3a20 7475  g.    :rtype: tu
+000021a0: 706c 650a 2020 2020 7a0e 0a49 6e69 7469  ple.    z..Initi
+000021b0: 616c 2073 7461 7465 7a0d 0a20 3d3d 3d3d  al statez.. ====
+000021c0: 3d3d 3d3d 3d3d 3d72 0f00 0000 da07 6163  =======r......ac
+000021d0: 7469 6f6e 737a 090a 0a41 6374 696f 6e20  tionsz...Action 
+000021e0: fa01 3ada 0474 7970 6572 0900 0000 2903  ..:..typer....).
+000021f0: 7247 0000 0072 4500 0000 da0f 7472 616e  rG...rE.....tran
+00002200: 7369 7469 6f6e 5f73 746f 70da 0072 4700  sition_stop..rG.
+00002210: 0000 da01 7872 0200 0000 da01 7972 3200  ....xr......yr2.
+00002220: 0000 da01 7a72 3700 0000 7a32 0a20 494e  ....zr7...z2. IN
+00002230: 5055 5420 4552 524f 5220 3a20 4469 7265  PUT ERROR : Dire
+00002240: 6374 696f 6e20 6d75 7374 2062 6520 6f6e  ction must be on
+00002250: 6520 6f66 2078 2c20 7920 6f72 207a 7245  e of x, y or zrE
+00002260: 0000 0072 5a00 0000 2903 7234 0000 0072  ...rZ...).r4...r
+00002270: 4500 0000 725a 0000 0072 0800 0000 2903  E...rZ...r....).
+00002280: 723c 0000 0072 3d00 0000 723e 0000 0072  r<...r=...r>...r
+00002290: 3c00 0000 723d 0000 0072 3e00 0000 720a  <...r=...r>...r.
+000022a0: 0000 0029 0672 4d00 0000 7252 0000 0072  ...).rM...rR...r
+000022b0: 5100 0000 7250 0000 0072 4f00 0000 724e  Q...rP...rO...rN
+000022c0: 0000 0072 4d00 0000 724e 0000 0072 4f00  ...rM...rN...rO.
+000022d0: 0000 7250 0000 0072 5100 0000 5429 0672  ..rP...rQ...T).r
+000022e0: 4e00 0000 724f 0000 0072 5000 0000 7251  N...rO...rP...rQ
+000022f0: 0000 0072 5200 0000 7224 0000 00da 0f6e  ...rR...r$.....n
+00002300: 6577 5f74 656d 7065 7261 7475 7265 4eda  ew_temperatureN.
+00002310: 0c6e 6577 5f70 7265 7373 7572 65da 066e  .new_pressure..n
+00002320: 6577 5f79 6b29 0472 2100 0000 7222 0000  ew_yk).r!...r"..
+00002330: 0072 2300 0000 7224 0000 007a 0e0a 0a20  .r#...r$...z... 
+00002340: 4669 6e61 6c20 7374 6174 6529 0c72 1200  Final state).r..
+00002350: 0000 da07 4845 4144 4c4f 47da 085f 5f72  ....HEADLOG..__r
+00002360: 6570 725f 5fda 0965 6e75 6d65 7261 7465  epr__..enumerate
+00002370: da14 5f63 6865 636b 5f61 6374 696f 6e5f  .._check_action_
+00002380: 7061 7261 6d73 7214 0000 0072 1600 0000  paramsr....r....
+00002390: 7218 0000 0072 0900 0000 7208 0000 0072  r....r....r....r
+000023a0: 0a00 0000 7207 0000 0029 0c72 3b00 0000  ....r....).r;...
+000023b0: 721f 0000 00da 0669 6e5f 6e6f 6272 2500  r......in_nobr%.
+000023c0: 0000 da01 69da 0661 6374 696f 6eda 0972  ....i..action..r
+000023d0: 6571 645f 6b65 7973 da05 6368 6563 6b72  eqd_keys..checkr
+000023e0: 3400 0000 7229 0000 0072 2000 0000 da03  4...r)...r .....
+000023f0: 6f75 7473 0c00 0000 2020 2020 2020 2020  outs....        
+00002400: 2020 2020 722d 0000 0072 0500 0000 7205      r-...r....r.
+00002410: 0000 00cc 0000 0073 6503 0000 8000 f51e  .......se.......
+00002420: 000b 0e8d 6789 2c8c 2c80 43d8 0407 d00b  ....g.,.,.C.....
+00002430: 1cd1 041c 8043 d804 07d0 0b1b d104 1b80  .....C..........
+00002440: 43d8 0407 8834 9025 972e 922e d112 22d4  C....4.%......".
+00002450: 1222 d10b 22d1 0422 8043 e515 1e98 76a0  .".."..".C....v.
+00002460: 69d4 1f30 d115 31d4 1531 f000 5801 051a  i..0..1..1..X...
+00002470: f100 5801 051a 8909 8801 8836 e008 0b88  ..X........6....
+00002480: 7d9d 73a0 3199 769c 76d1 0f25 a803 d10f  }.s.1.v.v..%....
+00002490: 2ba8 66b0 56ac 6ed1 0f3c d108 3c88 03e0  +.f.V.n..<..<...
+000024a0: 0b11 9026 8c3e d01d 36d2 0b36 d00b 36f0  ...&.>..6..6..6.
+000024b0: 0204 190e f000 0419 0ef0 0004 190e 8849  ...............I
+000024c0: f50a 0015 29a8 19b5 44b8 16bf 1bba 1bb9  ....)...D.......
+000024d0: 1dbc 1dd1 3447 d434 47d1 1448 d414 4888  ....4G.4G..H..H.
+000024e0: 45d8 0f14 9802 8a7b 887b dd16 24a0 53a8  E......{.{..$.S.
+000024f0: 35a1 5bd1 1631 d416 31d0 1031 e00f 1590  5.[..1..1..1....
+00002500: 6bd4 0f22 a063 d20f 29d0 0f29 d817 1890  k..".c..)..)....
+00002510: 0490 04d8 1117 980b d411 24a8 03d2 112b  ..........$....+
+00002520: d011 2bd8 1718 9004 9004 d811 1798 0bd4  ..+.............
+00002530: 1124 a803 d211 2bd0 112b d817 1890 0490  .$....+..+......
+00002540: 04e0 1953 9006 dd16 24a0 53a8 36a1 5cd1  ...S....$.S.6.\.
+00002550: 1632 d416 32d0 1032 e514 2bd8 1014 d815  .2..2..2..+.....
+00002560: 19d8 2127 d028 3ad4 213b d820 26d0 2738  ..!'.(:.!;. &.'8
+00002570: d420 39f0 0905 150e f100 0515 0ef4 0005  . 9.............
+00002580: 150e 8845 8945 f00e 000e 1490 468c 5ed0  ...E.E......F.^.
+00002590: 1f34 d20d 34d0 0d34 f002 0419 0ef0 0004  .4..4..4........
+000025a0: 190e f000 0419 0e88 49f5 0a00 1529 a819  ........I....)..
+000025b0: b544 b816 bf1b ba1b b91d bc1d d134 47d4  .D...........4G.
+000025c0: 3447 d114 48d4 1448 8845 d80f 1498 028a  4G..H..H.E......
+000025d0: 7b88 7bdd 1624 a053 a835 a15b d116 31d4  {.{..$.S.5.[..1.
+000025e0: 1631 d010 31e5 1427 d810 14d8 171d 9868  .1..1..'.......h
+000025f0: d417 27d8 171d 9868 d417 27d8 161c 9857  ..'....h..'....W
+00002600: 946f f009 0515 0ef1 0005 150e f400 0515  .o..............
+00002610: 0e88 4588 45f0 0e00 0e14 9046 8c5e d01f  ..E.E......F.^..
+00002620: 30d2 0d30 d00d 30f0 0207 190e f000 0719  0..0..0.........
+00002630: 0ef0 0007 190e 8849 f512 0015 29a8 19b5  .......I....)...
+00002640: 44b8 16bf 1bba 1bb9 1dbc 1dd1 3447 d434  D...........4G.4
+00002650: 47d1 1448 d414 4888 45d8 0f14 9802 8a7b  G..H..H.E......{
+00002660: 887b dd16 24a0 53a8 35a1 5bd1 1631 d416  .{..$.S.5.[..1..
+00002670: 31d0 1031 e514 23d8 1015 d810 1690 7ad4  1..1..#.......z.
+00002680: 1022 d815 1b98 4694 5ed8 151b 9846 945e  ."....F.^....F.^
+00002690: d820 26d0 2738 d420 39d8 2026 d027 38d4  . &.'8. 9. &.'8.
+000026a0: 2039 d819 1fa0 0ad4 192b d818 1cf0 1109   9.......+......
+000026b0: 150e f100 0915 0ef4 0009 150e 8845 f016  .............E..
+000026c0: 000c 1da0 46d0 0b2a d00b 2ad8 282c 8846  ....F..*..*.(,.F
+000026d0: d013 24d1 0c25 d80b 19a0 16d0 0b27 d00b  ..$..%.......'..
+000026e0: 27d8 2529 8846 903e d10c 22d8 0b13 9836  '.%).F.>.."....6
+000026f0: d00b 21d0 0b21 d81f 2388 4690 38d1 0c1c  ..!..!..#.F.8...
+00002700: e50e 19d8 0c11 d80c 11d8 151b d01c 2dd4  ..............-.
+00002710: 152e d816 1c98 5ed4 162c d812 1898 18d4  ......^..,......
+00002720: 1222 d814 18f0 0d07 0f0a f100 070f 0af4  ."..............
+00002730: 0007 0f0a 8803 f010 0009 0c88 7490 6389  ............t.c.
+00002740: 7ad1 0819 8803 8903 e004 07d0 0b1d d104  z...............
+00002750: 1d80 43d8 0407 d00b 1bd1 041b 8043 e004  ..C..........C..
+00002760: 0788 3490 2597 2e92 2ed1 1222 d412 22d1  ..4.%......"..".
+00002770: 0b22 d104 2280 43e0 0b10 9023 883a d004  ."..".C....#.:..
+00002780: 1572 2e00 0000 6301 0000 0000 0000 0000  .r....c.........
+00002790: 0000 0004 0000 0003 0000 00f3 6400 0000  ............d...
+000027a0: 9700 7401 0000 0000 0000 0000 0000 6a01  ..t...........j.
+000027b0: 0000 0000 0000 0000 7404 0000 0000 0000  ........t.......
+000027c0: 0000 0000 6401 a602 0000 ab02 0000 0000  ....d...........
+000027d0: 0000 0000 7d01 7407 0000 0000 0000 0000  ....}.t.........
+000027e0: 0000 6a04 0000 0000 0000 0000 7c01 7c00  ..j.........|.|.
+000027f0: a602 0000 ab02 0000 0000 0000 0000 0100  ................
+00002800: 6402 5300 2903 7a22 4475 6d70 2074 6865  d.S.).z"Dump the
+00002810: 2064 6566 6175 6c74 2067 6173 6f75 7420   default gasout 
+00002820: 696e 7075 7420 6669 6c65 7a1e 494e 5055  input filez.INPU
+00002830: 542f 6465 6661 756c 745f 6761 736f 7574  T/default_gasout
+00002840: 5f69 6e70 7574 2e79 6d6c 4e29 05da 0d70  _input.ymlN)...p
+00002850: 6b67 5f72 6573 6f75 7263 6573 da11 7265  kg_resources..re
+00002860: 736f 7572 6365 5f66 696c 656e 616d 65da  source_filename.
+00002870: 085f 5f6e 616d 655f 5fda 0673 6875 7469  .__name__..shuti
+00002880: 6cda 0863 6f70 7966 696c 6529 02da 0566  l..copyfile)...f
+00002890: 6e61 6d65 da14 6465 6661 756c 745f 6761  name..default_ga
+000028a0: 736f 7574 5f69 6e70 7574 7302 0000 0020  sout_inputs.... 
+000028b0: 2072 2d00 0000 7206 0000 0072 0600 0000   r-...r....r....
+000028c0: 4201 0000 7336 0000 0080 00e5 1b28 d41b  B...s6.......(..
+000028d0: 3add 0810 d012 32f1 0302 1c06 f400 021c  :.....2.........
+000028e0: 06d0 0418 f506 0005 0b84 4fd0 1428 a825  ..........O..(.%
+000028f0: d104 30d4 0430 d004 30d0 0430 d004 3072  ..0..0..0..0..0r
+00002900: 2e00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00002910: 0005 0000 0003 0000 00f3 c200 0000 9700  ................
+00002920: 7401 0000 0000 0000 0000 0000 a600 0000  t...............
+00002930: ab00 0000 0000 0000 0000 7d02 7c01 4400  ..........}.|.D.
+00002940: 5d16 7d03 7c03 7c00 6700 6401 a201 7a00  ].}.|.|.g.d...z.
+00002950: 0000 7601 720b 7c02 6402 7c03 7a00 0000  ..v.r.|.d.|.z...
+00002960: 6403 7a00 0000 7a0d 0000 7d02 8c17 7c02  d.z...z...}...|.
+00002970: 6404 6b03 0000 0000 721d 7c02 6405 7a0d  d.k.....r.|.d.z.
+00002980: 0000 7d02 7c02 6406 a001 0000 0000 0000  ..}.|.d.........
+00002990: 0000 0000 0000 0000 0000 0000 0000 7c00  ..............|.
+000029a0: a601 0000 ab01 0000 0000 0000 0000 7a0d  ..............z.
+000029b0: 0000 7d02 7c00 4400 5d11 7d03 7c03 7c01  ..}.|.D.].}.|.|.
+000029c0: 7601 720b 7c02 6407 7c03 7a00 0000 6408  v.r.|.d.|.z...d.
+000029d0: 7a00 0000 7a0d 0000 7d02 8c12 7c02 5300  z...z...}...|.S.
+000029e0: 2909 610e 0100 000a 2020 2020 4368 6563  ).a.....    Chec
+000029f0: 6b20 6761 736f 7574 2061 6374 696f 6e20  k gasout action 
+00002a00: 6b65 7973 0a0a 2020 2020 3a70 6172 616d  keys..    :param
+00002a10: 2072 6571 645f 6b65 7973 3a20 4c69 7374   reqd_keys: List
+00002a20: 206f 6620 7265 7175 6972 6564 206b 6579   of required key
+00002a30: 730a 2020 2020 3a74 7970 6520 7265 7164  s.    :type reqd
+00002a40: 5f6b 6579 733a 206c 6973 745b 7374 725d  _keys: list[str]
+00002a50: 0a20 2020 203a 7061 7261 6d20 7072 6f76  .    :param prov
+00002a60: 6964 6564 5f6b 6579 733a 204c 6973 7420  ided_keys: List 
+00002a70: 6f66 206b 6579 7320 696e 2074 6865 2069  of keys in the i
+00002a80: 6e70 7574 2066 696c 650a 2020 2020 3a74  nput file.    :t
+00002a90: 7970 6520 7072 6f76 6964 6564 5f6b 6579  ype provided_key
+00002aa0: 733a 206c 6973 745b 7374 725d 0a0a 2020  s: list[str]..  
+00002ab0: 2020 3a72 6574 7572 6e73 3a20 4c6f 6720    :returns: Log 
+00002ac0: 6f66 2074 6865 2061 6363 6570 7465 6420  of the accepted 
+00002ad0: 616e 6420 6d69 7373 696e 6720 6b65 7973  and missing keys
+00002ae0: 0a20 2020 203a 7274 7970 653a 2073 7472  .    :rtype: str
+00002af0: 0a20 2020 2029 0472 5900 0000 725f 0000  .    ).rY...r_..
+00002b00: 0072 6000 0000 7261 0000 007a 0b0a 2e20  .r`...ra...z... 
+00002b10: 2020 2d20 6b65 7920 7a0d 206e 6f74 2061    - key z. not a
+00002b20: 6363 6570 7465 6472 5b00 0000 7a13 0a2e  cceptedr[...z...
+00002b30: 2020 2d20 4163 6365 7074 6564 206b 6579    - Accepted key
+00002b40: 737a 090a 2e20 2020 2020 203e 7a06 0a20  sz...      >z.. 
+00002b50: 6b65 7920 7a0c 2069 7320 6d69 7373 696e  key z. is missin
+00002b60: 672e 2902 7212 0000 0072 1700 0000 2904  g.).r....r....).
+00002b70: 7269 0000 00da 0d70 726f 7669 6465 645f  ri.....provided_
+00002b80: 6b65 7973 7225 0000 00da 036b 6579 7304  keysr%.....keys.
+00002b90: 0000 0020 2020 2072 2d00 0000 7265 0000  ...    r-...re..
+00002ba0: 0072 6500 0000 4a01 0000 73a7 0000 0080  .re...J...s.....
+00002bb0: 00f5 1800 0b0e 8925 8c25 8043 d80f 1cf0  .......%.%.C....
+00002bc0: 0002 053a f000 0205 3a88 03d8 0b0e 9069  ...:....:......i
+00002bd0: d022 57d0 2257 d022 57d1 1657 d00b 57d0  ."W."W."W..W..W.
+00002be0: 0b57 d80c 0f90 3ea0 43d1 1327 a82f d113  .W....>.C..'./..
+00002bf0: 39d1 0c39 8843 f8d8 070a 8862 8279 8079  9..9.C.....b.y.y
+00002c00: d808 0bd0 0f25 d108 2588 03d8 080b 887c  .....%..%......|
+00002c10: d70f 20d2 0f20 a019 d10f 2bd4 0f2b d108  .. .. ....+..+..
+00002c20: 2b88 03e0 0f18 f000 0205 34f0 0002 0534  +.........4....4
+00002c30: 8803 d80b 0e90 6dd0 0b23 d00b 23d8 0c0f  ......m..#..#...
+00002c40: 9039 9873 913f a05e d113 33d1 0c33 8843  .9.s.?.^..3..3.C
+00002c50: f8d8 0b0e 804a 722e 0000 0063 0200 0000  .....Jr....c....
+00002c60: 0000 0000 0000 0000 0600 0000 0300 0000  ................
+00002c70: f356 0100 0097 0074 0100 0000 0000 0000  .V.....t........
+00002c80: 0000 0064 017c 00a6 0200 00ab 0200 0000  ...d.|..........
+00002c90: 0000 0000 0001 0074 0300 0000 0000 0000  .......t........
+00002ca0: 0000 006a 0200 0000 0000 0000 007c 0064  ...j.........|.d
+00002cb0: 02a6 0200 00ab 0200 0000 0000 0000 0035  ...............5
+00002cc0: 007d 0274 0700 0000 0000 0000 0000 006a  .}.t...........j
+00002cd0: 0400 0000 0000 0000 007c 0264 03ac 04a6  .........|.d....
+00002ce0: 0200 00ab 0200 0000 0000 0000 007d 0364  .............}.d
+00002cf0: 0564 0564 05a6 0200 00ab 0200 0000 0000  .d.d............
+00002d00: 0000 0001 006e 0b23 0031 0073 0477 0278  .....n.#.1.s.w.x
+00002d10: 0359 0077 0101 0059 0001 0001 0074 0100  .Y.w...Y.....t..
+00002d20: 0000 0000 0000 0000 0064 067c 01a6 0200  .........d.|....
+00002d30: 00ab 0200 0000 0000 0000 0001 0074 0300  .............t..
+00002d40: 0000 0000 0000 0000 006a 0200 0000 0000  .........j......
+00002d50: 0000 007c 0164 02a6 0200 00ab 0200 0000  ...|.d..........
+00002d60: 0000 0000 0035 007d 0274 0700 0000 0000  .....5.}.t......
+00002d70: 0000 0000 006a 0400 0000 0000 0000 007c  .....j.........|
+00002d80: 0264 03ac 04a6 0200 00ab 0200 0000 0000  .d..............
+00002d90: 0000 007d 0464 0564 0564 05a6 0200 00ab  ...}.d.d.d......
+00002da0: 0200 0000 0000 0000 0001 006e 0b23 0031  ...........n.#.1
+00002db0: 0073 0477 0278 0359 0077 0101 0059 0001  .s.w.x.Y.w...Y..
+00002dc0: 0001 007c 047c 0366 0253 0029 077a b10a  ...|.|.f.S.).z..
+00002dd0: 2020 2020 4c6f 6164 2061 206d 6573 6820      Load a mesh 
+00002de0: 616e 6420 736f 6c75 7469 6f6e 2069 6e74  and solution int
+00002df0: 6f20 4844 4635 206f 626a 6563 7473 0a0a  o HDF5 objects..
+00002e00: 2020 2020 3a70 6172 616d 2066 6e61 6d65      :param fname
+00002e10: 3a20 4669 6c65 6e61 6d65 206f 6620 7468  : Filename of th
+00002e20: 6520 736f 6c75 7469 6f6e 0a20 2020 203a  e solution.    :
+00002e30: 7479 7065 2066 6e61 6d65 3a20 7374 720a  type fname: str.
+00002e40: 2020 2020 3a70 6172 616d 206d 6e61 6d65      :param mname
+00002e50: 3a20 4669 6c65 6e61 6d65 206f 6620 7468  : Filename of th
+00002e60: 6520 6d65 7368 0a20 2020 203a 7479 7065  e mesh.    :type
+00002e70: 206d 6e61 6d65 3a20 7374 720a 2020 2020   mname: str.    
+00002e80: 7a14 5265 6164 696e 6720 736f 6c75 7469  z.Reading soluti
+00002e90: 6f6e 2069 6e20 da01 7246 2901 da04 6c61  on in ..rF)...la
+00002ea0: 7a79 4e7a 1052 6561 6469 6e67 206d 6573  zyNz.Reading mes
+00002eb0: 6820 696e 2029 05da 0570 7269 6e74 da04  h in )...print..
+00002ec0: 6835 7079 da04 4669 6c65 7203 0000 00da  h5py..Filer.....
+00002ed0: 046c 6f61 6429 0572 7200 0000 da05 6d6e  .load).rr.....mn
+00002ee0: 616d 65da 0366 696e da03 736f 6cda 046d  ame..fin..sol..m
+00002ef0: 6573 6873 0500 0000 2020 2020 2072 2d00  eshs....     r-.
+00002f00: 0000 720b 0000 0072 0b00 0000 6401 0000  ..r....r....d...
+00002f10: 7320 0100 0080 00f5 1200 050a d00a 20a0  s ............ .
+00002f20: 25d1 0428 d404 28d0 0428 dd09 0d8c 1990  %..(..(..(......
+00002f30: 3598 23d1 091e d409 1ef0 0001 052c a023  5.#..........,.#
+00002f40: dd0e 158c 6c98 33a0 55d0 0e2b d10e 2bd4  ....l.3.U..+..+.
+00002f50: 0e2b 8803 f003 0105 2cf0 0001 052c f000  .+......,....,..
+00002f60: 0105 2cf1 0001 052c f400 0105 2cf0 0001  ..,....,....,...
+00002f70: 052c f000 0105 2cf0 0001 052c f000 0105  .,....,....,....
+00002f80: 2cf0 0001 052c f000 0105 2cf8 f8f8 f000  ,....,....,.....
+00002f90: 0105 2cf0 0001 052c f000 0105 2cf0 0001  ..,....,....,...
+00002fa0: 052c e504 09d0 0a1c 9865 d104 24d4 0424  .,.......e..$..$
+00002fb0: d004 24dd 090d 8c19 9035 9823 d109 1ed4  ..$......5.#....
+00002fc0: 091e f000 0105 2da0 23dd 0f16 8c7c 9843  ......-.#....|.C
+00002fd0: a065 d00f 2cd1 0f2c d40f 2c88 04f0 0301  .e..,..,..,.....
+00002fe0: 052d f000 0105 2df0 0001 052d f100 0105  .-....-....-....
+00002ff0: 2df4 0001 052d f000 0105 2df0 0001 052d  -....-....-....-
+00003000: f000 0105 2df0 0001 052d f000 0105 2df0  ....-....-....-.
+00003010: 0001 052d f8f8 f8f0 0001 052d f000 0105  ...-.......-....
+00003020: 2df0 0001 052d f000 0105 2de0 0b0f 9013  -....-....-.....
+00003030: 8839 d004 1473 2300 0000 a617 4109 03c1  .9...s#.....A...
+00003040: 0904 410d 07c1 1001 410d 07c1 3917 421c  ..A.....A...9.B.
+00003050: 03c2 1c04 4220 07c2 2301 4220 0763 0200  ....B ..#.B .c..
+00003060: 0000 0000 0000 0000 0000 0600 0000 0300  ................
+00003070: 0000 f34c 0100 0097 0074 0100 0000 0000  ...L.....t......
+00003080: 0000 0000 006a 0100 0000 0000 0000 007c  .....j.........|
+00003090: 0164 0119 0000 0000 0000 0000 0064 0219  .d...........d..
+000030a0: 0000 0000 0000 0000 007c 0164 0119 0000  .........|.d....
+000030b0: 0000 0000 0000 0064 0319 0000 0000 0000  .......d........
+000030c0: 0000 007c 0164 0419 0000 0000 0000 0000  ...|.d..........
+000030d0: 00a6 0300 00ab 0300 0000 0000 0000 007d  ...............}
+000030e0: 027c 0064 0519 0000 0000 0000 0000 0064  .|.d...........d
+000030f0: 0619 0000 0000 0000 0000 007d 037c 0064  ...........}.|.d
+00003100: 0519 0000 0000 0000 0000 0064 0719 0000  ...........d....
+00003110: 0000 0000 0000 007d 0409 007c 0064 0519  .......}...|.d..
+00003120: 0000 0000 0000 0000 0064 0819 0000 0000  .........d......
+00003130: 0000 0000 007d 0574 0500 0000 0000 0000  .....}.t........
+00003140: 0000 006a 0300 0000 0000 0000 007c 037c  ...j.........|.|
+00003150: 047c 0566 0364 09ac 0aa6 0200 00ab 0200  .|.f.d..........
+00003160: 0000 0000 0000 007d 066e 2823 0074 0800  .......}.n(#.t..
+00003170: 0000 0000 0000 0000 0024 0072 1b01 0074  .........$.r...t
+00003180: 0500 0000 0000 0000 0000 006a 0300 0000  ...........j....
+00003190: 0000 0000 007c 037c 0466 0264 09ac 0aa6  .....|.|.f.d....
+000031a0: 0200 00ab 0200 0000 0000 0000 007d 0659  .............}.Y
+000031b0: 006e 0477 0078 0359 0077 017c 067c 0266  .n.w.x.Y.w.|.|.f
+000031c0: 0253 0029 0b7a f70a 2020 2020 4275 696c  .S.).z..    Buil
+000031d0: 6420 636f 6f72 6469 6e61 7465 7320 616e  d coordinates an
+000031e0: 6420 6120 5374 6174 6520 6672 6f6d 2061  d a State from a
+000031f0: 6e20 4156 4250 206d 6573 6820 616e 6420  n AVBP mesh and 
+00003200: 736f 6c75 7469 6f6e 0a0a 2020 2020 3a70  solution..    :p
+00003210: 6172 616d 206d 6573 683a 2041 5642 5020  aram mesh: AVBP 
+00003220: 6d65 7368 0a20 2020 203a 7479 7065 206d  mesh.    :type m
+00003230: 6573 683a 2048 4446 3520 6f62 6a65 6374  esh: HDF5 object
+00003240: 0a20 2020 203a 7061 7261 6d20 736f 6c3a  .    :param sol:
+00003250: 2041 5642 5020 736f 6c75 7469 6f6e 0a20   AVBP solution. 
+00003260: 2020 203a 7479 7065 2073 6f6c 3a20 4844     :type sol: HD
+00003270: 4635 206f 626a 6563 740a 0a20 2020 203a  F5 object..    :
+00003280: 7265 7475 726e 733a 2054 7570 6c65 206f  returns: Tuple o
+00003290: 6620 636f 6f72 6469 6e61 7465 7320 616e  f coordinates an
+000032a0: 6420 5374 6174 650a 2020 2020 3a72 7479  d State.    :rty
+000032b0: 7065 3a20 7475 706c 650a 2020 2020 da0c  pe: tuple.    ..
+000032c0: 4761 7365 6f75 7350 6861 7365 da03 7268  GaseousPhase..rh
+000032d0: 6fda 0472 686f 45da 0a52 686f 5370 6563  o..rhoE..RhoSpec
+000032e0: 6965 73da 0b43 6f6f 7264 696e 6174 6573  ies..Coordinates
+000032f0: 725c 0000 0072 5d00 0000 725e 0000 0072  r\...r]...r^...r
+00003300: 3000 0000 7233 0000 0029 0572 0400 0000  0...r3...).r....
+00003310: da09 6672 6f6d 5f63 6f6e 7372 1900 0000  ..from_consr....
+00003320: da05 7374 6163 6bda 084b 6579 4572 726f  ..stack..KeyErro
+00003330: 7229 0772 8100 0000 7280 0000 0072 1f00  r).r....r....r..
+00003340: 0000 da06 785f 636f 6f72 da06 795f 636f  ....x_coor..y_co
+00003350: 6f72 da06 7a5f 636f 6f72 723b 0000 0073  or..z_coorr;...s
+00003360: 0700 0000 2020 2020 2020 2072 2d00 0000  ....       r-...
+00003370: da14 6275 696c 645f 6461 7461 5f66 726f  ..build_data_fro
+00003380: 6d5f 6176 6270 728e 0000 0076 0100 0073  m_avbpr....v...s
+00003390: ca00 0000 8000 f518 000d 128c 4fd8 080b  ............O...
+000033a0: 884e d408 1b98 45d4 0822 a043 a80e d424  .N....E..".C...$
+000033b0: 37b8 06d4 243f c013 c05c d441 52f1 0302  7...$?...\.AR...
+000033c0: 0d06 f400 020d 0680 45f0 0800 0e12 902d  ........E......-
+000033d0: d40d 20a0 13d4 0d25 8046 d80d 1190 2dd4  .. ....%.F....-.
+000033e0: 0d20 a013 d40d 2580 46f0 0204 0533 d811  . ....%.F....3..
+000033f0: 1590 6dd4 1124 a053 d411 2988 06dd 0f11  ..m..$.S..).....
+00003400: 8c78 9816 a016 a816 d018 30b0 72d0 0f3a  .x........0.r..:
+00003410: d10f 3ad4 0f3a 8804 8804 f8dd 0b13 f000  ..:..:..........
+00003420: 0105 33f0 0001 0533 f000 0105 33dd 0f11  ..3....3....3...
+00003430: 8c78 9816 a016 d018 28a8 72d0 0f32 d10f  .x......(.r..2..
+00003440: 32d4 0f32 8804 8804 8804 f003 0105 33f8  2..2..........3.
+00003450: f8f8 f006 000c 1090 1588 3bd0 0416 7312  ..........;...s.
+00003460: 0000 00c1 1227 413a 00c1 3a22 421f 03c2  .....'A:..:"B...
+00003470: 1e01 421f 0363 0300 0000 0000 0000 0000  ..B..c..........
+00003480: 0000 0600 0000 0300 0000 f3f8 0100 0097  ................
+00003490: 0074 0100 0000 0000 0000 0000 006a 0100  .t...........j..
+000034a0: 0000 0000 0000 007c 01a6 0100 00ab 0100  .......|........
+000034b0: 0000 0000 0000 007d 037c 006a 0200 0000  .......}.|.j....
+000034c0: 0000 0000 007c 0364 0119 0000 0000 0000  .....|.d........
+000034d0: 0000 0064 023c 0000 007c 006a 0200 0000  ...d.<...|.j....
+000034e0: 0000 0000 007c 006a 0300 0000 0000 0000  .....|.j........
+000034f0: 007a 0500 007c 0364 0119 0000 0000 0000  .z...|.d........
+00003500: 0000 0064 033c 0000 007c 0364 0419 0000  ...d.<...|.d....
+00003510: 0000 0000 0000 0044 005d 207d 047c 006a  .......D.] }.|.j
+00003520: 0200 0000 0000 0000 007c 006a 0400 0000  .........|.j....
+00003530: 0000 0000 007c 0419 0000 0000 0000 0000  .....|..........
+00003540: 007a 0500 007c 0364 0419 0000 0000 0000  .z...|.d........
+00003550: 0000 007c 043c 0000 008c 2109 007c 006a  ...|.<....!..|.j
+00003560: 0500 0000 0000 0000 007c 0364 0519 0000  .........|.d....
+00003570: 0000 0000 0000 0064 063c 0000 007c 006a  .......d.<...|.j
+00003580: 0600 0000 0000 0000 007c 0364 0519 0000  .........|.d....
+00003590: 0000 0000 0000 0064 073c 0000 006e 1f23  .......d.<...n.#
+000035a0: 0074 0e00 0000 0000 0000 0000 0024 0072  .t...........$.r
+000035b0: 1201 0074 1100 0000 0000 0000 0000 0064  ...t...........d
+000035c0: 08a6 0100 00ab 0100 0000 0000 0000 0001  ................
+000035d0: 0059 006e 0477 0078 0359 0077 0174 1100  .Y.n.w.x.Y.w.t..
+000035e0: 0000 0000 0000 0000 0064 097c 02a6 0200  .........d.|....
+000035f0: 00ab 0200 0000 0000 0000 0001 0074 1300  .............t..
+00003600: 0000 0000 0000 0000 006a 0a00 0000 0000  .........j......
+00003610: 0000 007c 0264 0aa6 0200 00ab 0200 0000  ...|.d..........
+00003620: 0000 0000 0035 007d 0574 1700 0000 0000  .....5.}.t......
+00003630: 0000 0000 006a 0c00 0000 0000 0000 007c  .....j.........|
+00003640: 037c 05a6 0200 00ab 0200 0000 0000 0000  .|..............
+00003650: 0001 0064 0b64 0b64 0ba6 0200 00ab 0200  ...d.d.d........
+00003660: 0000 0000 0000 0001 0064 0b53 0023 0031  .........d.S.#.1
+00003670: 0073 0477 0278 0359 0077 0101 0059 0001  .s.w.x.Y.w...Y..
+00003680: 0001 0064 0b53 0029 0c7a 3255 7064 6174  ...d.S.).z2Updat
+00003690: 6520 7468 6520 6675 6c6c 2073 6f6c 7574  e the full solut
+000036a0: 696f 6e20 7769 7468 2074 6865 2073 7461  ion with the sta
+000036b0: 7465 2070 6172 616d 6574 6572 7372 8300  te parametersr..
+000036c0: 0000 7284 0000 0072 8500 0000 7286 0000  ..r....r....r...
+000036d0: 00da 0b41 6464 6974 696f 6e61 6c73 721b  ...Additionalsr.
+000036e0: 0000 0072 1c00 0000 7a30 2d41 6464 6974  ...r....z0-Addit
+000036f0: 696f 6e61 6c73 2d20 6772 6f75 7020 6973  ionals- group is
+00003700: 206e 6f74 2070 6172 7420 6f66 2074 6865   not part of the
+00003710: 2073 6f6c 7574 696f 6e2e 7a13 5361 7669   solution.z.Savi
+00003720: 6e67 2073 6f6c 7574 696f 6e20 696e 20da  ng solution in .
+00003730: 0177 4e29 0dda 0463 6f70 79da 0864 6565  .wN)...copy..dee
+00003740: 7063 6f70 7972 8400 0000 da06 656e 6572  pcopyr......ener
+00003750: 6779 7215 0000 0072 1b00 0000 721c 0000  gyr....r....r...
+00003760: 0072 8a00 0000 727a 0000 0072 7b00 0000  .r....rz...r{...
+00003770: 727c 0000 0072 0300 0000 da04 6475 6d70  r|...r......dump
+00003780: 2906 721f 0000 0072 8000 0000 7272 0000  ).r....r....rr..
+00003790: 00da 0773 6f6c 5f6e 6577 7228 0000 00da  ...sol_newr(....
+000037a0: 0466 6f75 7473 0600 0000 2020 2020 2020  .fouts....      
+000037b0: 722d 0000 0072 0c00 0000 720c 0000 0091  r-...r....r.....
+000037c0: 0100 0073 6901 0000 8000 e50e 128c 6d98  ...si.........m.
+000037d0: 43d1 0e20 d40e 2080 47d8 252a a459 8047  C.. .. .G.%*.Y.G
+000037e0: 884e d404 1b98 45d1 0422 d826 2ba4 69b0  .N....E..".&+.i.
+000037f0: 25b4 2cd1 263e 8047 884e d404 1b98 46d1  %.,.&>.G.N....F.
+00003800: 0423 d810 1798 0cd4 1025 f000 0105 4901  .#.......%....I.
+00003810: f000 0105 4901 8804 d826 2ba4 69b0 25d4  ....I....&+.i.%.
+00003820: 3242 c034 d432 48d1 2648 8807 900c d408  2B.4.2H.&H......
+00003830: 1d98 64d1 0823 d008 23f0 0404 0542 01d8  ..d..#..#....B..
+00003840: 3035 d430 4188 0790 0dd4 081e 987d d108  05.0A........}..
+00003850: 2dd8 2d32 ac5e 8807 900d d408 1e98 7ad1  -.-2.^........z.
+00003860: 082a d008 2af8 dd0b 13f0 0001 0542 01f0  .*..*........B..
+00003870: 0001 0542 01f0 0001 0542 01dd 080d d00e  ...B.....B......
+00003880: 40d1 0841 d408 41d0 0841 d008 41d0 0841  @..A..A..A..A..A
+00003890: f003 0105 4201 f8f8 f8f5 0600 050a d00a  ....B...........
+000038a0: 1fa0 15d1 0427 d404 27d0 0427 dd09 0d8c  .....'..'..'....
+000038b0: 1990 3598 23d1 091e d409 1ef0 0001 0524  ..5.#..........$
+000038c0: a024 dd08 0f8c 0c90 5798 64d1 0823 d408  .$......W.d..#..
+000038d0: 23d0 0823 f003 0105 24f0 0001 0524 f000  #..#....$....$..
+000038e0: 0105 24f1 0001 0524 f400 0105 24f0 0001  ..$....$....$...
+000038f0: 0524 f000 0105 24f0 0001 0524 f000 0105  .$....$....$....
+00003900: 24f0 0001 0524 f000 0105 24f0 0001 0524  $....$....$....$
+00003910: f8f8 f8f0 0001 0524 f000 0105 24f0 0001  .......$....$...
+00003920: 0524 f000 0105 24f0 0001 0524 f000 0105  .$....$....$....
+00003930: 2473 2400 0000 c127 2042 0800 c208 1942  $s$....' B.....B
+00003940: 2403 c223 0142 2403 c30c 1643 2f03 c32f  $..#.B$....C/../
+00003950: 0443 3307 c336 0143 3307 6301 0000 0000  .C3..6.C3.c.....
+00003960: 0000 0000 0000 0006 0000 0003 0000 00f3  ................
+00003970: 6e01 0000 9700 7401 0000 0000 0000 0000  n.....t.........
+00003980: 0000 7c00 6401 a602 0000 ab02 0000 0000  ..|.d...........
+00003990: 0000 0000 3500 7d01 7403 0000 0000 0000  ....5.}.t.......
+000039a0: 0000 0000 6a02 0000 0000 0000 0000 7c01  ....j.........|.
+000039b0: 7402 0000 0000 0000 0000 0000 6a03 0000  t...........j...
+000039c0: 0000 0000 0000 ac02 a602 0000 ab02 0000  ................
+000039d0: 0000 0000 0000 7d02 6403 6403 6403 a602  ......}.d.d.d...
+000039e0: 0000 ab02 0000 0000 0000 0000 0100 6e0b  ..............n.
+000039f0: 2300 3100 7304 7702 7803 5900 7701 0100  #.1.s.w.x.Y.w...
+00003a00: 5900 0100 0100 7409 0000 0000 0000 0000  Y.....t.........
+00003a10: 0000 7c02 6404 1900 0000 0000 0000 0000  ..|.d...........
+00003a20: 7c02 6405 1900 0000 0000 0000 0000 a602  |.d.............
+00003a30: 0000 ab02 0000 0000 0000 0000 5c02 0000  ............\...
+00003a40: 7d03 7d04 740b 0000 0000 0000 0000 0000  }.}.t...........
+00003a50: 7c03 7c04 a602 0000 ab02 0000 0000 0000  |.|.............
+00003a60: 0000 5c02 0000 7d05 7d06 740d 0000 0000  ..\...}.}.t.....
+00003a70: 0000 0000 0000 7c05 7c06 7c02 a603 0000  ......|.|.|.....
+00003a80: ab03 0000 0000 0000 0000 5c02 0000 7d07  ..........\...}.
+00003a90: 7d08 740f 0000 0000 0000 0000 0000 7c08  }.t...........|.
+00003aa0: a601 0000 ab01 0000 0000 0000 0000 0100  ................
+00003ab0: 7411 0000 0000 0000 0000 0000 7c07 7c04  t...........|.|.
+00003ac0: 7c02 6406 1900 0000 0000 0000 0000 a603  |.d.............
+00003ad0: 0000 ab03 0000 0000 0000 0000 0100 6403  ..............d.
+00003ae0: 5300 2907 7a09 4d61 696e 2063 616c 6c72  S.).z.Main callr
+00003af0: 7800 0000 2901 da06 4c6f 6164 6572 4eda  x...)...LoaderN.
+00003b00: 0a69 6e73 745f 736f 6c75 7472 8100 0000  .inst_solutr....
+00003b10: da11 696e 7374 5f73 6f6c 7574 5f6f 7574  ..inst_solut_out
+00003b20: 7075 7429 09da 046f 7065 6eda 0479 616d  put)...open..yam
+00003b30: 6c72 7d00 0000 7299 0000 0072 0b00 0000  lr}...r....r....
+00003b40: 728e 0000 0072 0500 0000 727a 0000 0072  r....r....rz...r
+00003b50: 0c00 0000 2909 da09 696e 7075 7466 696c  ....)...inputfil
+00003b60: 6572 7f00 0000 7266 0000 0072 8100 0000  er....rf...r....
+00003b70: 7280 0000 0072 3b00 0000 721f 0000 00da  r....r;...r.....
+00003b80: 0973 7461 7465 5f6e 6577 7225 0000 0073  .state_newr%...s
+00003b90: 0900 0000 2020 2020 2020 2020 2072 2d00  ....         r-.
+00003ba0: 0000 720d 0000 0072 0d00 0000 a401 0000  ..r....r........
+00003bb0: 73eb 0000 0080 00f5 0600 0a0e 8869 9813  s............i..
+00003bc0: d109 1dd4 091d f000 0105 34a0 13dd 1115  ..........4.....
+00003bd0: 9419 9833 a574 a47b d011 33d1 1133 d411  ...3.t.{..3..3..
+00003be0: 3388 06f0 0301 0534 f000 0105 34f0 0001  3......4....4...
+00003bf0: 0534 f100 0105 34f4 0001 0534 f000 0105  .4....4....4....
+00003c00: 34f0 0001 0534 f000 0105 34f0 0001 0534  4....4....4....4
+00003c10: f000 0105 34f0 0001 0534 f8f8 f8f0 0001  ....4....4......
+00003c20: 0534 f000 0105 34f0 0001 0534 f000 0105  .4....4....4....
+00003c30: 34f5 0600 1127 a076 a86c d427 3bb8 56c0  4....'.v.l.';.V.
+00003c40: 46bc 5ed1 104c d410 4c81 4980 4488 23e5  F.^..L..L.I.D.#.
+00003c50: 1226 a074 a853 d112 31d4 1231 814b 8044  .&.t.S..1..1.K.D
+00003c60: 8825 e515 26a0 74a8 55b0 46d1 153b d415  .%..&.t.U.F..;..
+00003c70: 3b81 4e80 4988 73e5 0409 8823 814a 844a  ;.N.I.s....#.J.J
+00003c80: 804a e504 1690 79a0 23a0 76d0 2e41 d427  .J....y.#.v..A.'
+00003c90: 42d1 0443 d404 43d0 0443 d004 43d0 0443  B..C..C..C..C..C
+00003ca0: 730f 0000 0091 213e 03be 0441 0207 c105  s.....!>...A....
+00003cb0: 0141 0207 2904 4e4e 4e46 2904 4e4e 7248  .A..).NNNF).NNrH
+00003cc0: 0000 0046 2919 da07 5f5f 646f 635f 5f72  ...F)...__doc__r
+00003cd0: 9d00 0000 7292 0000 0072 7b00 0000 da05  ....r....r{.....
+00003ce0: 6e75 6d70 7972 1900 0000 da07 6835 6372  numpyr......h5cr
+00003cf0: 6f73 7372 0300 0000 7270 0000 0072 6d00  ossr....rp...rm.
+00003d00: 0000 da0f 6d73 5f74 6865 726d 6f2e 7374  ....ms_thermo.st
+00003d10: 6174 6572 0400 0000 7262 0000 00da 075f  ater....rb....._
+00003d20: 5f61 6c6c 5f5f 7207 0000 0072 0800 0000  _all__r....r....
+00003d30: 7209 0000 0072 0a00 0000 7205 0000 0072  r....r....r....r
+00003d40: 0600 0000 7265 0000 0072 0b00 0000 728e  ....re...r....r.
+00003d50: 0000 0072 0c00 0000 720d 0000 00a9 0072  ...r....r......r
+00003d60: 2e00 0000 722d 0000 00fa 083c 6d6f 6475  ....r-.....<modu
+00003d70: 6c65 3e72 a600 0000 0100 0000 7356 0100  le>r........sV..
+00003d80: 00f0 0301 0101 d800 45d0 0045 e000 0b80  ........E..E....
+00003d90: 0b80 0b80 0bd8 000b 800b 800b 800b d800  ................
+00003da0: 0b80 0b80 0b80 0bd8 0012 d000 12d0 0012  ................
+00003db0: d000 12d8 001b d000 1bd0 001b d000 1bd0  ................
+00003dc0: 001b d000 1bd8 000d 800d 800d 800d d800  ................
+00003dd0: 14d0 0014 d000 14d0 0014 d800 21d0 0021  ............!..!
+00003de0: d000 21d0 0021 d000 21d0 0021 f006 060b  ..!..!..!..!....
+00003df0: 0480 07f0 100a 0b02 f000 0a0b 02f0 000a  ................
+00003e00: 0b02 8007 f01a 3701 0ff0 0037 010f f000  ......7....7....
+00003e10: 3701 0ff0 0037 010f f074 011c 0111 f000  7....7...t......
+00003e20: 1c01 11f0 001c 0111 f03e 1d01 11f0 001d  .........>......
+00003e30: 0111 f000 1d01 11f0 4a01 0015 19d8 1418  ........J.......
+00003e40: d80d 10d8 0c11 f011 2e01 11f0 002e 0111  ................
+00003e50: f000 2e01 11f0 002e 0111 f062 0173 0101  ...........b.s..
+00003e60: 16f0 0073 0101 16f0 0073 0101 16f0 6c03  ...s.....s....l.
+00003e70: 0501 31f0 0005 0131 f000 0501 31f0 1017  ..1....1....1...
+00003e80: 010f f000 1701 0ff0 0017 010f f034 0f01  .............4..
+00003e90: 15f0 000f 0115 f000 0f01 15f0 2418 0117  ............$...
+00003ea0: f000 1801 17f0 0018 0117 f036 1001 24f0  ...........6..$.
+00003eb0: 0010 0124 f000 1001 24f0 260e 0144 01f0  ...$....$.&..D..
+00003ec0: 000e 0144 01f0 000e 0144 01f0 000e 0144  ...D.....D.....D
+00003ed0: 01f0 000e 0144 0172 2e00 0000            .....D.r....
```

### Comparing `ms_thermo-0.3.6/src/ms_thermo/cli.py` & `ms_thermo-0.3.7/src/ms_thermo/cli.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/constants.py` & `ms_thermo-0.3.7/src/ms_thermo/constants.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/flame_params.py` & `ms_thermo-0.3.7/src/ms_thermo/flame_params.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/gasout.py` & `ms_thermo-0.3.7/src/ms_thermo/gasout.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/kero_prim2cons.py` & `ms_thermo-0.3.7/src/ms_thermo/kero_prim2cons.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/mixture_state.py` & `ms_thermo-0.3.7/src/ms_thermo/mixture_state.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/species.py` & `ms_thermo-0.3.7/src/ms_thermo/species.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/state.py` & `ms_thermo-0.3.7/src/ms_thermo/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,29 +95,29 @@
         self._temperature = temperature
 
     def __repr__(self):
         """Define the value returned by calling State representation (printing State)"""
         mini = dict()
         maxi = dict()
         moco = dict()
-        moco["rho"] = mode(self.rho, axis=None)[0]
+        moco["rho"] = mode(self.rho, axis=None, keepdims=False)[0]
         mini["rho"] = np.min(self.rho)
         maxi["rho"] = np.max(self.rho)
-        moco["energy"] = mode(self.energy, axis=None)[0]
+        moco["energy"] = mode(self.energy, axis=None, keepdims=False)[0]
         mini["energy"] = np.min(self.energy)
         maxi["energy"] = np.max(self.energy)
-        moco["temperature"] = mode(self.temperature, axis=None)[0]
+        moco["temperature"] = mode(self.temperature, axis=None, keepdims=False)[0]
         mini["temperature"] = np.min(self.temperature)
         maxi["temperature"] = np.max(self.temperature)
-        moco["pressure"] = mode(self.pressure, axis=None)[0]
+        moco["pressure"] = mode(self.pressure, axis=None, keepdims=False)[0]
         mini["pressure"] = np.min(self.pressure)
         maxi["pressure"] = np.max(self.pressure)
         for specy in self._y_k:
             frac_specy = "Y_" + specy
-            moco[frac_specy] = mode(self._y_k[specy], axis=None)[0]
+            moco[frac_specy] = mode(self._y_k[specy], axis=None, keepdims=False)[0]
             mini[frac_specy] = np.min(self._y_k[specy])
             maxi[frac_specy] = np.max(self._y_k[specy])
         repr_str = "\nCurrent primitive state of the mixture \n"
         repr_str += "\t\t| Most Common |    Min    |    Max \n"
         repr_str += "-" * 52 + "\n"
         for var in moco:
             infos = (var, moco[var], mini[var], maxi[var])
@@ -573,7 +573,9 @@
         """
         warnings.simplefilter("ignore")
         msgwarn = "ms_thermo.state.mix_molecular_weight() is deprecated,"
         msgwarn += "use instead ms_thermo.state.mix_w"
         warnings.warn(msgwarn)
         print(msgwarn)
         return self.mix_w
+    
+
```

### Comparing `ms_thermo-0.3.6/src/ms_thermo/tadia.py` & `ms_thermo-0.3.7/src/ms_thermo/tadia.py`

 * *Files identical despite different names*

### Comparing `ms_thermo-0.3.6/src/ms_thermo/yk_from_phi.py` & `ms_thermo-0.3.7/src/ms_thermo/yk_from_phi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,63 @@
 """
 This script calculate mass_fraction of species from a Phi
 """
 
 __all__ = ["yk_from_phi", "phi_from_far"]
 
 
+MOLAR_MASSES =  {"C": 0.0120107, "H": 0.00100797, "O2": 0.0319988, "N2": 0.0280134}
+
+
+def far_stochio(c_x:float, h_y:float)-> float:
+    """Return the fuel air ratio stoechiometric according to c_x h_y
+    
+    valid for AIR , not for PURE OXYGEN!!!
+
+    BTW, the example in https://en.wikipedia.org/wiki/Air%E2%80%93fuel_ratio is for pure oxygen...
+    """
+    mass_mol_fuel = c_x * MOLAR_MASSES["C"] + h_y * MOLAR_MASSES["H"]
+    coeff_o2 = c_x + (h_y / 4)
+    coef_air=1./0.2314
+    afr_sto = coef_air*(coeff_o2 * MOLAR_MASSES["O2"]) / mass_mol_fuel
+    far_sto = 1./afr_sto
+    return far_sto
+
 def phi_from_far(far:float, c_x:float, h_y:float)-> float:
     """
     *Return phi coefficient with the fuel air ratio coeff + fuel composition*
 
     :param far: the air-fuel ratio
     :type far: float
     :param c_x: stoechio coeff of Carbone
     :type c_x: float
     :param h_y: stoechio coeff of hydrogene
     :type h_y: float
 
     :returns:
         - **phi** - Equivalence ratio
     """
-    mass_molar = {"C": 0.0120107, "H": 0.00100797, "O2": 0.0319988, "N2": 0.0280134}
-    mass_mol_fuel = c_x * mass_molar["C"] + h_y * mass_molar["H"]
-    coeff_o2 = c_x + (h_y / 4)
-    y_o2_fuel_sto = (coeff_o2 * mass_molar["O2"]) / mass_mol_fuel
-    phi = far / y_o2_fuel_sto
+    return  far /far_stochio(c_x, h_y)
 
-    return phi
+
+def far_from_phi(phi:float, c_x:float, h_y:float)-> float:
+    """
+    *Return fuel air ratio coeff  with the phi coefficient + fuel composition*
+
+    :param phi: eq. ratio coef
+    :type far: float
+    :param c_x: stoechio coeff of Carbone
+    :type c_x: float
+    :param h_y: stoechio coeff of hydrogene
+    :type h_y: float
+
+    :returns:
+        - **far** - Equivalence ratio
+    """
+    return phi * far_stochio(c_x, h_y)
 
 
 # use "fuel" here as default. Beware it important for pyavbp.
 def yk_from_phi(phi:float, c_x:float, h_y:float, fuel_name:str="fuel")-> float:
     """
     *Return the species mass fractions in a fresh fuel-air mixture*
 
@@ -43,26 +71,24 @@
     :type fuel_name: str
 
     :returns:
         - **y_k** - A dict of mass fractions
 
     """
     y_k = dict()
-    mass_molar = {"C": 0.0120107, "H": 0.00100797, "O2": 0.0319988, "N2": 0.0280134}
-
-    mass_mol_fuel = c_x * mass_molar["C"] + h_y * mass_molar["H"]
+    mass_mol_fuel = c_x * MOLAR_MASSES["C"] + h_y * MOLAR_MASSES["H"]
     coeff_o2 = c_x + (h_y / 4)
-    y_o2_fuel_sto = (coeff_o2 * mass_molar["O2"]) / mass_mol_fuel
+    y_o2_fuel_sto = (coeff_o2 * MOLAR_MASSES["O2"]) / mass_mol_fuel
 
     if phi == 0.0:
         y_k[fuel_name] = 0.0
     else:
         y_k[fuel_name] = 1.0 / (
             1.0
-            + (1.0 + 3.76 * (mass_molar["N2"] / mass_molar["O2"]))
+            + (1.0 + 3.76 * (MOLAR_MASSES["N2"] / MOLAR_MASSES["O2"]))
             * (y_o2_fuel_sto / phi)
         )
     y_air = 1 - y_k[fuel_name]
     y_k["N2"] = y_air / 1.303794
     y_k["O2"] = 0.303794 * y_k["N2"]
 
     return y_k
```

### Comparing `ms_thermo-0.3.6/src/ms_thermo.egg-info/PKG-INFO` & `ms_thermo-0.3.7/src/ms_thermo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-thermo
-Version: 0.3.6
+Version: 0.3.7
 Summary: Utilities to work on 2D and 3D structured grids
 Home-page: https://gitlab.com/cerfacs/ms_thermo
 Author: CoopTeam-CERFACS
 Author-email: coop@cerfacs.com
 Project-URL: Homepage, https://gitlab.com/cerfacs/ms_thermo
 Project-URL: Documentation, https://ms_thermo.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.com/cerfacs/ms_thermo/-/issues
```

### Comparing `ms_thermo-0.3.6/src/ms_thermo.egg-info/SOURCES.txt` & `ms_thermo-0.3.7/src/ms_thermo.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -23,17 +23,22 @@
 src/ms_thermo.egg-info/requires.txt
 src/ms_thermo.egg-info/top_level.txt
 src/ms_thermo/INPUT/2S_KERO_BFER.h5
 src/ms_thermo/INPUT/Luche1.cti
 src/ms_thermo/INPUT/__init__.py
 src/ms_thermo/INPUT/default_gasout_input.yml
 src/ms_thermo/INPUT/species_database.dat
-src/ms_thermo/__pycache__/__init__.cpython-39.pyc
-src/ms_thermo/__pycache__/constants.cpython-39.pyc
-src/ms_thermo/__pycache__/flame_params.cpython-39.pyc
-src/ms_thermo/__pycache__/gasout.cpython-39.pyc
-src/ms_thermo/__pycache__/kero_prim2cons.cpython-39.pyc
-src/ms_thermo/__pycache__/mixture_state.cpython-39.pyc
-src/ms_thermo/__pycache__/species.cpython-39.pyc
-src/ms_thermo/__pycache__/state.cpython-39.pyc
-src/ms_thermo/__pycache__/tadia.cpython-39.pyc
-src/ms_thermo/__pycache__/yk_from_phi.cpython-39.pyc
+src/ms_thermo/__pycache__/__init__.cpython-311.pyc
+src/ms_thermo/__pycache__/constants.cpython-311.pyc
+src/ms_thermo/__pycache__/flame_params.cpython-311.pyc
+src/ms_thermo/__pycache__/gasout.cpython-311.pyc
+src/ms_thermo/__pycache__/kero_prim2cons.cpython-311.pyc
+src/ms_thermo/__pycache__/mixture_state.cpython-311.pyc
+src/ms_thermo/__pycache__/species.cpython-311.pyc
+src/ms_thermo/__pycache__/state.cpython-311.pyc
+src/ms_thermo/__pycache__/tadia.cpython-311.pyc
+src/ms_thermo/__pycache__/yk_from_phi.cpython-311.pyc
+tests/test_compositions.py
+tests/test_kero_prim2cons.py
+tests/test_mixture_state.py
+tests/test_state.py
+tests/test_tadia.py
```

