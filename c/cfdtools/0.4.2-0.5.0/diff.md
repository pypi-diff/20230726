# Comparing `tmp/cfdtools-0.4.2.tar.gz` & `tmp/cfdtools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfdtools-0.4.2.tar", last modified: Wed Apr  5 08:39:29 2023, max compression
+gzip compressed data, was "cfdtools-0.5.0.tar", last modified: Wed Jul 26 11:45:56 2023, max compression
```

## Comparing `cfdtools-0.4.2.tar` & `cfdtools-0.5.0.tar`

### file list

```diff
@@ -1,66 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.245315 cfdtools-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-05 08:39:14.000000 cfdtools-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-04-05 08:39:29.245315 cfdtools-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-05 08:39:14.000000 cfdtools-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.241315 cfdtools-0.4.2/cfdtools/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.241315 cfdtools-0.4.2/cfdtools/cgns/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/cgns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/cgns/cgns.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.241315 cfdtools-0.4.2/cfdtools/gmsh/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/gmsh/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9734 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/gmsh/_gmsh.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15508 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/gmsh/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.241315 cfdtools-0.4.2/cfdtools/hdf5/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/hdf5/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/hdf5/_hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.241315 cfdtools-0.4.2/cfdtools/ic3/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/ic3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/ic3/_ic3.py
--rw-r--r--   0 runner    (1001) docker     (123)    38399 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/ic3/reader_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/ic3/writerV2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/ic3/writerV3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.245315 cfdtools-0.4.2/cfdtools/meshbase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/meshbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/meshbase/_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/meshbase/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/meshbase/_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/meshbase/_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    16192 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/meshbase/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/meshbase/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.245315 cfdtools-0.4.2/cfdtools/physics/
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/physics/dicovar.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.245315 cfdtools-0.4.2/cfdtools/probes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/probes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/probes/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/probes/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.245315 cfdtools-0.4.2/cfdtools/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/utils/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.245315 cfdtools-0.4.2/cfdtools/vtk/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/vtk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-05 08:39:14.000000 cfdtools-0.4.2/cfdtools/vtk/_vtk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.241315 cfdtools-0.4.2/cfdtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-04-05 08:39:29.000000 cfdtools-0.4.2/cfdtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-05 08:39:29.000000 cfdtools-0.4.2/cfdtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 08:39:29.000000 cfdtools-0.4.2/cfdtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-05 08:39:29.000000 cfdtools-0.4.2/cfdtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-05 08:39:29.000000 cfdtools-0.4.2/cfdtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-05 08:39:29.000000 cfdtools-0.4.2/cfdtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-05 08:39:14.000000 cfdtools-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 08:39:29.245315 cfdtools-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 08:39:29.245315 cfdtools-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_0_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_0_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_1_cgns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_1_gmsh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_1_ic3.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_1_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_1_vtk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_2_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_2_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_2_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-05 08:39:14.000000 cfdtools-0.4.2/tests/test_probes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.940114 cfdtools-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-26 11:45:34.000000 cfdtools-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-26 11:45:56.940114 cfdtools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-26 11:45:34.000000 cfdtools-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.928113 cfdtools-0.5.0/cfdtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.932113 cfdtools-0.5.0/cfdtools/cgns/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/cgns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/cgns/cgns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.932113 cfdtools-0.5.0/cfdtools/gmsh/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/gmsh/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9740 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/gmsh/_gmsh.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15464 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/gmsh/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.932113 cfdtools-0.5.0/cfdtools/hdf5/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/hdf5/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1693 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/hdf5/_hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.932113 cfdtools-0.5.0/cfdtools/ic3/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/ic3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/ic3/_ic3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26510 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/ic3/reader_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/ic3/writerV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6097 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/ic3/writerV3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/cfdtools/meshbase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16506 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/meshbase/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/cfdtools/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/physics/dicovar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/cfdtools/probes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/probes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/probes/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/probes/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/cfdtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/utils/_dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/utils/maths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/utils/polybase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/cfdtools/vtk/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/vtk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-07-26 11:45:34.000000 cfdtools-0.5.0/cfdtools/vtk/_vtk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.932113 cfdtools-0.5.0/cfdtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 11:45:56.000000 cfdtools-0.5.0/cfdtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-26 11:45:34.000000 cfdtools-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:45:56.940114 cfdtools-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:45:56.936114 cfdtools-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_0_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_0_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_0_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_0_polybase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_cgns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_gmsh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_ic3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_1_vtk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_2_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_2_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_2_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_2_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-26 11:45:34.000000 cfdtools-0.5.0/tests/test_probes.py
```

### Comparing `cfdtools-0.4.2/LICENSE` & `cfdtools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfdtools-0.4.2/PKG-INFO` & `cfdtools-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdtools
-Version: 0.4.2
+Version: 0.5.0
 Summary: Tools for mesh and solution management in CFD
 Author-email: "J. Gressier" <jeremie.gressier@isae-supaero.fr>
 License: MIT License
         
         Copyright (c) 2022 Jérémie GRESSIER
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,19 +55,23 @@
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/d32cf67a5fa242c88bb1568277f1d60e)](https://app.codacy.com/gh/jgressier/cfdtools/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)[![Doc](https://readthedocs.org/projects/cfdtools/badge/?version=latest)](https://readthedocs.org/projects/cfdtools/)
 [![Slack](https://img.shields.io/static/v1?logo=slack&label=slack&message=contact&style=flat)](https://join.slack.com/t/isae-opendev/shared_invite/zt-obqywf6r-UUuHR4_hc5iTzyL5bFCwpw
 )
 
 ### Features
 
-    - IC3 v2 or v3 reader
-    - IC3 v2 or v3 writer
-    - generic format command line: `cfdinfo`, `cfdwrite_ic3v3`
-    - specific IC3 command line: `ic3brief`
+- readers: IC3, VTK, GMSH, CGNS
+- writers: IC3, VTK
+- generic options for command line writers: extrusion
+- generic format command line: `cfdinfo`
+- specific IC3 command line: `ic3brief`
+- specific VTK command line: `vtkbrief`
 
 ### Installation and usage
 
-    pip install cfdtools
+```bash
+pip install cfdtools
+```
 
 ### Requirements
 
 see [requirements.txt](https://github.com/jgressier/cfdtools/blob/master/requirements.txt)
```

### Comparing `cfdtools-0.4.2/README.md` & `cfdtools-0.5.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/d32cf67a5fa242c88bb1568277f1d60e)](https://app.codacy.com/gh/jgressier/cfdtools/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)[![Doc](https://readthedocs.org/projects/cfdtools/badge/?version=latest)](https://readthedocs.org/projects/cfdtools/)
 [![Slack](https://img.shields.io/static/v1?logo=slack&label=slack&message=contact&style=flat)](https://join.slack.com/t/isae-opendev/shared_invite/zt-obqywf6r-UUuHR4_hc5iTzyL5bFCwpw
 )
 
 ### Features
 
-    - IC3 v2 or v3 reader
-    - IC3 v2 or v3 writer
-    - generic format command line: `cfdinfo`, `cfdwrite_ic3v3`
-    - specific IC3 command line: `ic3brief`
+- readers: IC3, VTK, GMSH, CGNS
+- writers: IC3, VTK
+- generic options for command line writers: extrusion
+- generic format command line: `cfdinfo`
+- specific IC3 command line: `ic3brief`
+- specific VTK command line: `vtkbrief`
 
 ### Installation and usage
 
-    pip install cfdtools
+```bash
+pip install cfdtools
+```
 
 ### Requirements
 
 see [requirements.txt](https://github.com/jgressier/cfdtools/blob/master/requirements.txt)
```

### Comparing `cfdtools-0.4.2/cfdtools/_cli.py` & `cfdtools-0.5.0/cfdtools/_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import argparse
 from pathlib import Path
 
 import cfdtools.api as api
 
-# readers
+# readers and writers - must be imported to update api format dict
 import cfdtools.ic3 as ic3  # .reader_legacy # needed to map readers
 import cfdtools.gmsh as gmsh
 import cfdtools.cgns as cgns
 import cfdtools.vtk as vtk
+#
 import cfdtools.meshbase.simple as simplemesh
 import cfdtools.probes.plot as probeplot
 import cfdtools.probes.data as probedata
 import numpy as np
 
 # To add a command line tool, just add the function pyproject.toml in section
-# [tool.poetry.scripts]
+# [project.scripts]
 # cfdinfo = 'cfdtools._cli:info'
 
 # print(api._fileformat_map)
 
 
 def cli_header(name):
     api.io.print('std', "CFDTOOLS - " + name)
@@ -33,24 +34,20 @@
                 api._fileformat_map,
             )
         )
 
     def add_argument(self, option, **kwargs):
         return self._parser.add_argument(option, **kwargs)
 
-    def addarg_filenameformat(self):
+    def addarg_filenameformat(self, format=None):
         self.add_argument('filename', help="file")
-        self.add_argument('--fmt', help="input format", choices=self._available_readers)
-        self.add_argument('--outpath', help="output folder")
-        self.add_argument(
-            "--check", action="store_true", dest="check", help="process some checks"
-        )
-        self.add_argument(
-            "--info", action="store_true", dest="info", help="print information"
-        )
+        self.add_argument('--fmt', help="input file format", choices=self._available_readers, default=format)
+        self.add_argument('--outpath', help="output folder path")
+        self.add_argument("--check", action="store_true", dest="check", help="process some checks")
+        self.add_argument("--info", action="store_true", dest="info", help="print information")
 
     def addarg_prefix(self):
         self.add_argument('prefix', help="prefix of files")
 
     def addarg_data(self):
         self.add_argument(
             '--remove-node-data',
@@ -74,15 +71,15 @@
             type=int,
             help="total number of planes",
         )
         self.add_argument(
             '--scale',
             nargs=3,
             type=float,
-            help="x, y, z scaling coefficients00",
+            help="x, y, z scaling coefficients",
         )
 
     def parse_cli_args(self, argv):
         self._args = self._parser.parse_args(argv)
 
     def args(self, key=None):
         return self._args if key is None else vars(self._args)[key]
@@ -90,19 +87,15 @@
     def argsdict(self):
         return vars(self._args)
 
     def parse_filenameformat(self):
         """parse args to get filename, automatic or specified format"""
         if self.args().fmt is None:
             ext = Path(self._args.filename).suffix
-            thisfmt = list(
-                filter(
-                    lambda n: api._fileformat_map[n]['ext'] == ext, api._fileformat_map
-                )
-            )
+            thisfmt = list(filter(lambda n: api._fileformat_map[n]['ext'] == ext, api._fileformat_map))
         else:
             thisfmt = [self.args().fmt]
         if len(thisfmt) == 0:
             api.error_stop('no extension found')
         elif len(thisfmt) > 1:
             api.error_stop('too many extensions found, must specify format with --fmt')
         self._fileformat = thisfmt[0]
@@ -120,31 +113,44 @@
     # api.io.set_modes(api.io._available)
     parser = cli_argparser()
     parser.addarg_filenameformat()
     parser.parse_cli_args(argv)
     parser.parse_filenameformat()
     #
     inputfile = Path(parser.args('filename'))
-    r = parser._reader(str(inputfile))
+    r = parser._reader(str(inputfile), cIntegrity=parser.args('check'))
     r.read_data()
     mesh = r.export_mesh()
     mesh.printinfo()
     return True  # needed for pytest
 
 
 def ic3brief(argv=None):
     cli_header("ic3brief")
     parser = cli_argparser()
-    parser.addarg_filenameformat()
+    parser.addarg_filenameformat(format='IC3')
     parser.parse_cli_args(argv)
     parser.parse_filenameformat()
     #
     r = ic3.binreader(parser.args().filename)
     r.read_headers()
-    return True
+    return True  # needed for pytest
+
+
+def vtkbrief(argv=None):
+    cli_header("vtkbrief")
+    parser = cli_argparser()
+    parser.addarg_filenameformat(format="VTK")
+    parser.parse_cli_args(argv)
+    parser.parse_filenameformat()
+    #
+    r = vtk.vtkMesh()
+    r.read(parser.args().filename)
+    r.brief()
+    return True  # needed for pytest
 
 
 def write_generic(argv, ext, writer):
     parser = cli_argparser()
     parser.addarg_filenameformat()
     parser.addarg_data()
     parser.addarg_transform()
@@ -176,26 +182,24 @@
     file.change_suffix(ext)
     if file.find_safe_newfile() > 0:
         api.io.print("std", "change output to safe new name " + file.filename)
     if parser.args().extrude:
         timer.start()
         nz = parser.args().extrude
         api.io.print(f'> extrusion along nz={nz} cells, {nz*ncell} total cells')
-        cfdmesh = cfdmesh.export_extruded(
-            extrude=np.linspace(0.0, 1.0, nz+1, endpoint=True)
-        )
-        timer.stop(nelem=nz*ncell)
+        cfdmesh = cfdmesh.export_extruded(extrude=np.linspace(0.0, 1.0, nz + 1, endpoint=True))
+        timer.stop(nelem=nz * ncell)
     if parser.args().scale:
         cfdmesh.scale(parser.args().scale)
     if parser.args().info:
         cfdmesh.printinfo()
     output = writer(cfdmesh)
     output.write_data(file.filename)
     api.io.print('std', f"file {file.filename} written")
-    return True  # needed for pytest
+    return file.filename  # True # needed for pytest (True not needed, filename for eventual rm)
 
 
 def write_ic3v2(argv=None):
     cli_header("cfdwrite_ic3v2")
     return write_generic(argv, '.ic3', ic3.writerV2.writer)
 
 
@@ -250,45 +254,35 @@
     api.io.print('std', f"> create Cube {nx}x{ny}x{nz}")
     cube = simplemesh.Cube(nx, ny, nz)
     mesh = cube.export_mesh()
     #
     file = api._files(parser.args().filename)
     w = parser._writer(mesh)
     w.write_data(file.filename)
-    return True  # needed for pytest
+    return file.filename  # True # needed for pytest (True not needed, filename for eventual rm)
 
 
 def ic3probe_plotline(argv=None):
     cli_header("ic3probe_plotline")
     parser = cli_argparser(description="Process line probes from IC3")
     parser.addarg_prefix()
     # parser.add_argument("filenames", nargs="*", help="list of files")
-    parser.add_argument(
-        "-v", action="store_true", dest="verbose", help="verbose output"
-    )
-    parser.add_argument(
-        "--data", action="store", dest="datalist", default="P", help="quantity to plot"
-    )
-    parser.add_argument(
-        "--axis", action="store", dest="axis", default="X", help="axis to follow"
-    )
+    parser.add_argument("-v", action="store_true", dest="verbose", help="verbose output")
+    parser.add_argument("--data", action="store", dest="datalist", default="P", help="quantity to plot")
+    parser.add_argument("--axis", action="store", dest="axis", default="X", help="axis to follow")
     parser.add_argument(
         "--map",
         action="store",
         dest="map",
         default="time",
         choices=["time", "freq"],
         help="type of map",
     )
-    parser.add_argument(
-        "--check", action="store_true", dest="check", help="process some checks"
-    )
-    parser.add_argument(
-        "--cmap", action="store", dest="cmap", default="turbo", help="colormap"
-    )
+    parser.add_argument("--check", action="store_true", dest="check", help="process some checks")
+    parser.add_argument("--cmap", action="store", dest="cmap", default="turbo", help="colormap")
     parser.add_argument(
         "--cmaplevels",
         action="store",
         dest="nlevels",
         default=30,
         type=int,
         help="colormap number of levels",
@@ -301,15 +295,15 @@
     expected_data = [
         var,
         parser.args().axis,
     ]  # axis must be the last to get right time size
     # check files and read data
     data = probedata.phydata(basename, verbose=parser.args().verbose)
 
-    api.io.print('std', "> read data ")
+    api.io.printstd(f"> read data in {basename}")
     for ivar in expected_data:
         data.check_data(ivar, prefix=basename)
 
     # --- read all expected data ---
     api.io.print('std', "> processing " + parser.args().map + " map of " + var)
     run_plot = {"time": probeplot.plot_timemap, "freq": probeplot.plot_freqmap}
```

### Comparing `cfdtools-0.4.2/cfdtools/api.py` & `cfdtools-0.5.0/cfdtools/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,29 @@
     and has the following functions
     - read_data()
     - export_mesh() which returns a meshbase._mesh.mesh class
     """
 
     def decorator(thisclass):
         properties = {'reader': thisclass, 'ext': extension}
-        if name in _fileformat_map.keys():
+        if name in _fileformat_map:
             _fileformat_map[name].update(properties)
         else:
             _fileformat_map[name] = properties
         return thisclass
 
     return decorator
 
 
 def fileformat_writer(name, extension):
     """decorator to register fileformat properties for given name  in api._fileformat_map"""
 
     def decorator(thisclass):
         properties = {'writer': thisclass, 'ext': extension}
-        if name in _fileformat_map.keys():
+        if name in _fileformat_map:
             _fileformat_map[name].update(properties)
         else:
             _fileformat_map[name] = properties
         return thisclass
 
     return decorator
 
@@ -93,14 +93,17 @@
 
     def printstd(self, *args, **kwargs):
         self.print('std', *args, **kwargs)
 
     def printdebug(self, *args, **kwargs):
         self.print('debug', *args, **kwargs)
 
+    def warning(self, *args, **kwargs):
+        self.print('warning', *args, **kwargs)
+
 
 io = api_output()
 # print(io.get_modes())
 
 
 def error_stop(msg):
     # io.print('error', msg)
@@ -135,23 +138,23 @@
     def change_suffix(self, ext: str):
         self._path = self._path.with_suffix(ext)
 
     def find_safe_newfile(self):
         """Returns safe destination, adding (n) if needed"""
         safepath = self._path
         # components strings
-        dir = safepath.parent
+        folder = safepath.parent
         stem = safepath.stem
         suff = safepath.suffix
         i = 0
         while safepath.exists():
             i += 1
             # safepath = safepath.with_stem(stem+f'({i})') # only python >= 3.9
             # print(dir,stem,f'({i})',suff)
-            safepath = Path(dir / (stem + f'({i})' + suff))
+            safepath = Path(folder / (stem + f'({i})' + suff))
         self._path = safepath
         return i > 0
 
     def printinfo(self):
         print(self)
 
 
@@ -160,59 +163,71 @@
 
 
 class Timer:  # from https://realpython.com/python-timer/
     default_tab = 60
     default_msg = ""
 
     def __init__(self, task="", msg=default_msg, nelem=None, tab=default_tab):
-        self._reset()
+        self.reset()
         self._nelem = nelem
         self._tab = tab
         self._task = task
         self._msg = msg
 
-    def _reset(self):
+    def reset(self):
         self._start_time = None
         self._task = ""
         self._col = 0
+        self._elapsed = 0.
 
+    @property
+    def elapsed(self):
+        return self._elapsed
+        
     def start(self):
         """Start a new timer"""
         if self._start_time is not None:
             raise TimerError(f"Timer is running. Use .stop() to stop it")
         self._start_time = time.perf_counter()
 
+    def pause(self):
+        """Stop the timer, add elapsed and do NOT report"""
+        if self._start_time is None:
+            raise TimerError(f"Timer is not running. Use .start() to start it")
+        self._elapsed += time.perf_counter() - self._start_time
+        self._start_time = None
+
     def stop(self, nelem=None):
         """Stop the timer, and report the elapsed time"""
         if nelem is not None:
             self._nelem = nelem
-        if self._start_time is None:
-            raise TimerError(f"Timer is not running. Use .start() to start it")
-        elapsed_time = time.perf_counter() - self._start_time
+        self.pause()
         normalized_time_ms = (
-            0.0 if self._nelem is None else 1e6 * elapsed_time / self._nelem
+            0.0 if self._nelem is None else 1e6 * self._elapsed / self._nelem
         )
         if self._nelem is None:
-            io.printstd(f"{' '*(self._tab-self._col)}wtime: {elapsed_time:0.4f}s")
+            io.printstd(f"{' '*(self._tab-self._col)}wtime: {self._elapsed:0.4f}s")
         else:
-            io.printstd(f"{' '*(self._tab-self._col)}wtime: {elapsed_time:0.4f}s | {normalized_time_ms:0.4f}µs/elem",)
+            io.printstd(f"{' '*(self._tab-self._col)}wtime: {self._elapsed:0.4f}s | {normalized_time_ms:0.4f}µs/elem",)
         # reset
-        self._reset()
+        self.reset()
 
     def __enter__(self):
         io.print('std', self._task, end='')
         self._col = len(self._task) + 1
         self.start()
 
     def __exit__(self, *exitoptions):
         self.stop()
 
 
 def memoize(f):
     cache = {}
+
     @wraps(f)
     def wrapper(*args):
         if not args in cache:
             cache[args] = f(*args)
-        #Warning: You may wish to do a deepcopy here if returning objects
+        # Warning: You may wish to do a deepcopy here if returning objects
         return cache[args]
-    return wrapper
+
+    return wrapper
```

### Comparing `cfdtools-0.4.2/cfdtools/cgns/cgns.py` & `cfdtools-0.5.0/cfdtools/cgns/cgns.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # cgns.py
 from pathlib import Path
 from cfdtools.api import io, error_stop, fileformat_reader, memoize
-from cfdtools.hdf5 import h5file, h5_str
+from cfdtools.hdf5 import h5File, h5_str
 from cfdtools.meshbase._mesh import Mesh, submeshmark
 import cfdtools.meshbase._connectivity as conn
 import cfdtools.meshbase._elements as ele
 import numpy as np
 
 cgtype = {}
 ele_cgns2local = {2: 'node1', 3: 'bar2', 5: 'tri3', 7: 'quad4', 17: 'hexa8'}
@@ -112,15 +112,15 @@
             boco.geodim = 'cell'
         else:
             error_stop(f'unknown gridlocation {gridloc}')
         boco.index = conn.indexlist(ilist=nodelist)  # must start at 0
         return boco
 
 
-class cgnsfile(h5file):
+class cgnsfile(h5File):
     def __init__(self, filename: str):
         super().__init__(filename)
         self.open()
 
     def open(self):
         super().open()
         self._cgnsver = self._h5file['CGNSLibraryVersion'][' data'][0]
@@ -169,29 +169,29 @@
 
     def printinfo(self):
         # super().printinfo()
         self._file.printinfo()
         io.print('std', 'CGNS version:', self._file._cgnsver)
         io.print('std', 'bases:', self._bases)
         io.print('std', 'zones:', list(self._zones.keys()))
-        for zn, z in self._zones.items():
+        for zn, _ in self._zones.items():
             io.print('std', f"  Zone {zn}")
             # for bcn, bc in
 
     def export_mesh(self):
         # io.print('std', f"> export mesh ") # printed by parent
         cgzone = self._zone
         io.printstd(f"Parse zone {self._zonename} ({self._geodim}D) ncell: {cgzone.ncell}, nnode: {cgzone.nnode}",)
         meshdata = Mesh(ncell=cgzone.ncell, nnode=cgzone.nnode)
         # get coordinates
         meshdata.set_nodescoord_xyz(*cgzone.coords())
         # # cell connectivity
         meshdata.set_cell2node(cgzone.export_cellcon())
         # boundary conditions
-        for name, bc in cgzone._BCs.items():
+        for _, bc in cgzone._BCs.items():
             boco = cgzone.export_BC(bc)
             # filter full domain
             if boco.type in ['internal']:
                 io.print('std', f"  filter internal mark {boco.name}")
             else:
                 io.print('std', f"  add boco {boco}")
                 meshdata.add_boco(boco)
```

### Comparing `cfdtools-0.4.2/cfdtools/gmsh/_gmsh.py` & `cfdtools-0.5.0/cfdtools/gmsh/_gmsh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf8
 
 # Import modules
-import collections
-import cfdtools.meshbase._mesh as _mesh
-import cfdtools.meshbase._connectivity as _conn
+# import collections
+# import cfdtools.meshbase._mesh as _mesh
+# import cfdtools.meshbase._connectivity as _conn
 
 # import os
 
 import cfdtools.api as api
 import numpy as np
 
 # from operator import itemgetter
```

### Comparing `cfdtools-0.4.2/cfdtools/gmsh/reader.py` & `cfdtools-0.5.0/cfdtools/gmsh/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,18 +222,18 @@
             bc["type"] = "boundary"
             bc["periodic_transform"] = np.zeros((16,), dtype=np.float64)
             self._famm.append(fff)
 
     def __read_sections(self, filename):
         # Read the entire mesh.
         msh = []
-        api.io.print('std', "reading all file...", end='')
-        fid = open(filename)
-        for l in fid:
-            msh.append(l.split())
+        api.io.print('std', f"Reading file {filename!r}...", end='')
+        with open(filename) as fid:
+            for l in fid:
+                msh.append(l.split())
         api.io.print('std', " done")
 
         # Find version of the GMSH used
         ibeg = msh.index(["$MeshFormat"])  # To be safe, use these indicators
         iend = msh.index(["$EndMeshFormat"])
         version = msh[ibeg + 1 : iend]
         self.version = int(float(version[0][0]))
@@ -274,15 +274,14 @@
             ibeg = msh.index(["$Elements"])
             iend = msh.index(["$EndElements"])
             elements = msh[ibeg + 1 : iend]
             elts = []
             for i in range(1, int(elements[0][0]) + 1):
                 elts.append([int(j) for j in elements[i]])
 
-            fid.close()
             return fam, bctype, x, y, z, elts
 
         # ---------------------------------------
         # msh reading for version 4.0 and above
         # ---------------------------------------
 
         elif self.version >= 4:
@@ -325,15 +324,14 @@
             api.io.print('std', "  parse Nodes")
             ibeg = msh.index(["$Nodes"])
             iend = msh.index(["$EndNodes"])
             coordinates = msh[ibeg + 1 : iend]
             counter = 1
             maxnodes = int(coordinates[0][3])
             nodes = 1
-            rng = []
             count = 1
             x = [None] * (maxnodes)
             y = [None] * (maxnodes)
             z = [None] * (maxnodes)
             while nodes < maxnodes:
                 cnt = int(coordinates[counter][3])
                 for i in range(counter + 1, counter + cnt + 1):
@@ -376,9 +374,8 @@
 
                 count = count + nxtrange + 1
             # max_j = np.max([len(l) for l in elts])
             # np_elts = np.zeros((len(elts), max_j), dtype=np.int8)
             # elts = np.array(elts) # numpy depreciation
             # print(elts)
             # api.io.print('std',elts)
-            fid.close()
             return fam, bctype, x, y, z, elts
```

### Comparing `cfdtools-0.4.2/cfdtools/ic3/_ic3.py` & `cfdtools-0.5.0/cfdtools/ic3/_ic3.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,40 +177,39 @@
     input   : handle on an open restart file [type file identifier]
               format of the binary token [type string]
               endianness flag [type boolean]
               size of the binary token to be read [type int]
     '''
 
     # Choose the right prefix to the format string based on endianness
-    if byte_swap is True:  # little-endian
+    if byte_swap:  # little-endian
         form = '<' + form
     else:  # big-endian
         form = '>' + form
 
     # Create a "packed-binary reader structure"
     s = struct.Struct(form)
 
     # Try to read 'size' bytes from the file otherwise crash
     try:
         while True:
             record = bfile.read(size)
             if len(record) != size:
                 api.io.print(
                     'error',
-                    "mismatch record {} and expected sizes {}".format(
-                        len(record), size
+                    "mismatched record ({}) and expected ({}) sizes".format(
+                        len(record), size,
                     ),
                 )
                 break
             return s.unpack(record)
     except IOError:
         api.io.print(
             'error',
-            "Fatal error. Could not read %d bytes from %s. Exiting."
-            % (size, bfile.name),
+            "Fatal error. Could not read %d bytes from %s. Exiting." % (size, bfile.name),
         )
         exit()
 
 
 ###################################################################################################
 def BinaryWrite(bfile, endian, form, varargs):
     '''
@@ -222,26 +221,22 @@
     '''
 
     # Assume big-endian to write the file - anyways charlesx can swap
     form = struct_endian[endian] + form
 
     # Create a packer
     s = struct.Struct(form)
-    # print(len(form), form,len(varargs),':')
     # Actually pack the string now
     packed_ba = s.pack(*varargs)
 
     # Try to write the bytes to the file otherwise crash
     try:
         bfile.write(packed_ba)
     except IOError:
-        api.io.print(
-            'error', "Fatal error. Could not write to %s. Exiting." % (bfile.name)
-        )
-        exit()
+        api.error_stop("Fatal error. Could not write to %s. Exiting." % (bfile.name))
 
 
 class restartSectionHeader:
     '''
     This class is designed to handle the header that is present
     before every variable/section/category saved into the restart file.
     '''
@@ -249,56 +244,53 @@
     def __init__(self, skip=0):
         """
         Initialize a section header class, as it is always structured
         in the same way, i.e. with a name, an id, a skip bytes count,
         an information array, and an auxiliary array needed in specific
         cases like periodicity.
         """
-
-        self.name = " " * ic3_restart_codes["UGP_IO_HEADER_NAME_LEN"]
+        header_name_length = ic3_restart_codes["UGP_IO_HEADER_NAME_LEN"]
+        self.name = " " * header_name_length
         self.id = np.zeros((1,), dtype=np.int32)
         self._skip = np.array([skip], dtype=np.int64)
         self.idata = np.zeros((8,), dtype=np.int64)
         self.rdata = np.zeros((16,), dtype=np.float64)
 
         # Initialize the format string
         self.binstr = ""
         # Fill it with prior knowledge of its content
-        for i in range(ic3_restart_codes["UGP_IO_HEADER_NAME_LEN"]):
-            self.binstr += "c"  # name
+        self.binstr += "c" * header_name_length  # name
         self.binstr += "i"  # id
         self.binstr += "q"  # skip
         self.binstr += "qqqqqqqq"  # idata (long long)
         self.binstr += "dddddddddddddddd"  # rdata (double)
 
         # Keep in mind the total byte size of the header
         self.hsize = (
-            ic3_restart_codes["UGP_IO_HEADER_NAME_LEN"] * type2nbytes["char"]
+            header_name_length * type2nbytes["char"]
             + type2nbytes["int32"]
             + type2nbytes["int64"]
             + self.idata.size * type2nbytes["int64"]
             + self.rdata.size * type2nbytes["float64"]
         )
 
     def skip(self):
         return self._skip[0]  # numpy array size 1 to handle int type
 
     def readVar(self, bfile, byte_swap, nametypes, reset_offset=True):
-        '''
+        """
         Once initialization is done, this method actually reads
         the header data from the packed binary formatted string.
-        '''
+        """
         id_list = []
         for nametype in nametypes:
             id_list.append(ic3_restart_codes[nametype])
-        if reset_offset is True:
+        if reset_offset:
             bfile.seek(8, os.SEEK_SET)
-        while (self.id[0] not in id_list) and (
-            self.id[0] != ic3_restart_codes["UGP_IO_EOF"]
-        ):
+        while (self.id[0] not in id_list) and (self.id[0] != ic3_restart_codes["UGP_IO_EOF"]):
             self.name = ""
             self.id = np.zeros((1,), dtype=np.int32)
             self.idata = np.zeros((8,), dtype=np.int64)
             self.rdata = np.zeros((16,), dtype=np.float64)
 
             api.io.print('debug', "skipping data %d" % self.skip())
             if self.skip() > 0:
@@ -318,21 +310,21 @@
                 i += 1
             if self.name.startswith("DEOF"):
                 break
             # Store the rest of the tokens in the right namespace
             nlen = ic3_restart_codes["UGP_IO_HEADER_NAME_LEN"]
             self.id[0] = s[nlen]
             self._skip[0] = s[nlen + self.id.size]  # store size in skip for next read
-            for i in range(self.idata.size):
-                self.idata[i] = s[nlen + self.id.size + self._skip.size + i]
-            for i in range(self.rdata.size):
-                self.rdata[i] = s[
-                    nlen + self.id.size + self._skip.size + self.idata.size + i
-                ]
-            # print(self)
+            ibeg = nlen + self.id.size + self._skip.size
+            iend = ibeg + self.idata.size
+            self.idata = s[ibeg:iend]
+            ibeg = iend
+            iend = ibeg + self.rdata.size
+            self.rdata = s[ibeg:iend]
+
         return self.id[0] in id_list
 
     def write(self, bfile, endian):
         """
         Once initialization is done, this method actually writes
         the header data from the packed binary formatted string.
         """
@@ -340,50 +332,35 @@
         # Make a list from all the arguments
         varargs = []
         for i in range(ic3_restart_codes["UGP_IO_HEADER_NAME_LEN"]):
             if i < len(self.name):
                 varargs.append(bytes(self.name[i], 'utf-8'))
             else:
                 varargs.append(b'\0')
-        # for i in varargs:
-        #     print(">",i, type(i))
         varargs.append(self.id)
         varargs.append(self.skip)
         for kk in range(8):
             varargs.append(self.idata[kk])
         for kk in range(16):
             varargs.append(self.rdata[kk])
-        # print(varargs)
         # Now write everything at once
         BinaryWrite(bfile, endian, self.binstr, varargs)
 
     def __str__(self):
         mystring = "> Header: \n"
         mystring += "Name : %s\n" % self.name
 
         mystring += "Id   : %i %s\n" % (
             self.id,
-            list(
-                dict(
-                    filter(
-                        lambda items: items[1] == self.id[0], ic3_restart_codes.items()
-                    )
-                ).keys()
-            ),
+            list(dict(filter(lambda items: items[1] == self.id[0], ic3_restart_codes.items())).keys()),
         )
         mystring += "hsize: %i\n" % self.hsize
         mystring += "skip : %i\n" % self.skip()
-        mystring += "idata: ("
-        for i in range(8):
-            mystring += " %i," % (self.idata[i])
-        mystring += ")\n"
-        mystring += "rdata: ("
-        for i in range(16):
-            mystring += " %f," % (self.rdata[i])
-        mystring += ")"
+        mystring += "idata: (" + ", ".join(str(i) for i in self.idata) + ")\n"
+        mystring += "rdata: (" + ", ".join(str(r) for r in self.rdata) + ")"
         return mystring
 
 
 class binreader(api._files):
     '''Implementation of the reader to read IC3 restart files.'''
 
     # def __init__(self, filename):
@@ -406,53 +383,48 @@
 
         if not self.exists():
             print("Fatal error. File %s cannot be found." % (self.filename))
             exit()
 
         # Open the file for binary reading
         api.io.print('debug', 'opening ', self.filename)
-        self.fid = open(self.filename, "rb")
-
-        api.io.print('std', "reading header (first section)")
-        self._ReadRestartHeader()
-        #
-        reset_offset = True
-        skip = 0
-        while True:
-            h = restartSectionHeader(skip=skip)
-            if not h.readVar(
-                self.fid,
-                self.byte_swap,
-                ic3_restart_codes.keys(),
-                reset_offset=reset_offset,
-            ):
-                break
-            else:
+        with open(self.filename, "rb") as self.fid:
+            api.io.print('std', "reading header (first section)")
+            self._ReadRestartHeader()
+            #
+            reset_offset = True
+            skip = 0
+            while True:
+                h = restartSectionHeader(skip=skip)
+                if not h.readVar(
+                    self.fid,
+                    self.byte_swap,
+                    ic3_restart_codes.keys(),
+                    reset_offset=reset_offset,
+                ):
+                    break
                 reset_offset = False  # continue
                 skip = h.skip()
                 print(h)
                 if h.id[0] == ic3_restart_codes['UGP_IO_EOF']:
                     api.io.print('std', 'UGP EOF reached')
                     break
-        # Before returning, close the file
-        self.fid.close()
         api.io.print('debug', self.filename, ' closed')
         del self.fid
 
         return
 
     def _ReadRestartHeader(self):
         '''
         Method reading the header of a restart file.
         It is composed of two integers, the "magic number" used as a flag for endianness
         and the IC3 version number.
-        input   : handle on an open restart file, [type file identifier]
-        output  : the endianness of the open restart file [type boolean]
+        input:  handle on an open restart file, [type file identifier]
+        output: the endianness of the open restart file [type boolean]
         '''
-
         # By default suppose big-endian format
         self.byte_swap = False
 
         # Read the first integer (int64)
         s = list(BinaryRead(self.fid, "ii", False, 2 * type2nbytes["int32"]))
         # If, with big-endian assumption, the first integer comes out wrong, swap to little-endian
         if s[0] != ic3_restart_codes["UGP_IO_MAGIC_NUMBER"]:
@@ -465,10 +437,9 @@
             aux_struct = struct.Struct("<i")
             s[1] = aux_struct.unpack(packed_version)[0]
 
         # Some info for the user
         self.ic3_version = s[1]
         api.io.print(
             'std',
-            f"  version: {self.ic3_version} "
-            + ("little-endian" if self.byte_swap else "big-endian"),
+            f"  version: {self.ic3_version} " + ("little-endian" if self.byte_swap else "big-endian"),
         )
```

### Comparing `cfdtools-0.4.2/cfdtools/ic3/writerV2.py` & `cfdtools-0.5.0/cfdtools/ic3/writerV2.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         Initialization of a ic3 restart file writer.
         """
         api.io.print('std', "> Initialization of IC3 writer V" + self.__version__)
         if not endian in struct_endian.keys():
             raise ValueError("unknown endian key")
         else:
             self.endian = endian
-        self.vars = {"nodes": {}, "cells": {}}
+        #self.vars = {"nodes": {}, "cells": {}}
         self._mesh = mesh
         self.params = {}
         # Initialize the simulation state
         self.set_simstate()
         self.set_mesh()
         self.set_bocos()
         self.set_vars()
@@ -57,15 +57,15 @@
             ):
                 self._mesh.reindex_boundaryfaces()
 
         api.io.print('std', "Setting coordinates and connectivity arrays..")
 
         # Nodes
         self.coordinates = np.stack(
-            list(self._mesh._nodes[c] for c in ['x', 'y', 'z']), axis=1
+            [self._mesh._nodes[c] for c in 'xyz'], axis=1
         )
 
         # Compute the number of nodes and elements
         assert self.coordinates.shape[0] == self._mesh.nnode
         self.params["no_count"] = self.coordinates.shape[0]
         # Elements, count throughout all connectivities
         self.params["cv_count"] = self._mesh.ncell
@@ -138,77 +138,76 @@
 
     def set_vars(self):
         """
         Set the variables for the restart.
         They will be later written to the file using the
         __WriteRestartVar method.
         """
-        api.io.print(
-            'std',
-            "Setting variables..",
-        )
-        self.vars = {"nodes": {}, "cells": {}}
+        api.io.printstd("Setting variables..")
+        self.vars = {
+            "nodes": self._mesh._nodedata,
+            "cells": self._mesh._celldata
+            }
         # Start with the variables stored at the vertices
-        for key, item in self._mesh._nodedata.items():
-            api.io.print('std', "  node data: " + key)
-            self.vars["nodes"][key] = item
-
-        # Then the variables stored at the cells:
-        for key, item in self._mesh._celldata.items():
-            api.io.print('std', "  cell data: " + key)
-            self.vars["cells"][key] = item
+        # for key, item in self._mesh._nodedata.items():
+        #     api.io.print('std', "  node data: " + key)
+        #     self.vars["nodes"][key] = item
+
+        # # Then the variables stored at the cells:
+        # for key, item in self._mesh._celldata.items():
+        #     api.io.print('std', "  cell data: " + key)
+        #     self.vars["cells"][key] = item
 
     def write_data(self, filename):
         """
         Main method of the ic3 restart file writer
         """
-        api.io.print('std', f"> WRITING FILE {filename}")
+        api.io.print('std', f"> WRITING FILE {filename!r}")
         self.filename = filename
         # Open the file for binary reading
-        self.fid = open(self.filename, "wb")
-
-        api.io.print('std', "> check consistency before writing")
-        if not self.check():
-            raise RuntimeError("Inconsistent data to write")
-
-        api.io.print('std', "> Writing header")
-        self.__WriteRestartHeader()
-        #
-        api.io.print('std', "> writing connectivity")
-        self.__WriteRestartConnectivity()
-        #
-        api.io.print('std', "> writing informative values")
-        self.__WriteInformativeValues()
-        #
-        api.io.print('std', "> writing variables")
-        self.__WriteRestartVar()
-        #
-        api.io.print('std', "> end of file")
-        header = restartSectionHeader()
-        header.name = "EOF"
-        header.id = ic3_restart_codes["UGP_IO_EOF"]
-        header.skip = header.hsize
-        header.write(self.fid, self.endian)
-
-        # Before returning, close the file
-        self.fid.close()
+        with open(self.filename, "wb") as self.fid:
+            #
+            api.io.print('std', "> check consistency before writing")
+            if not self.check():
+                raise RuntimeError("Inconsistent data to write")
+            #
+            api.io.print('std', "> Writing header")
+            self.__WriteRestartHeader()
+            #
+            api.io.print('std', "> Writing connectivity")
+            self.__WriteRestartConnectivity()
+            #
+            api.io.print('std', "> Writing informative values")
+            self.__WriteInformativeValues()
+            #
+            api.io.print('std', "> Writing variables")
+            self.__WriteRestartVar()
+            #
+            api.io.print('std', "> End of file")
+            header = restartSectionHeader()
+            header.name = "EOF"
+            header.id = ic3_restart_codes["UGP_IO_EOF"]
+            header.skip = header.hsize
+            header.write(self.fid, self.endian)
+            #
+            # self.fid is closed
         del self.fid
 
     def check(self):
         check_error = True
         # bad field size
         keylist = []
-        for key, cellitem in self.vars["cells"].items():
-            if cellitem.ndof() != 1:
-                keylist.append(key)
-        if len(keylist) >= 1:
-            check_error = False
-            api.io.print(
-                'error', 'wrong size (ndof) of cell data: ' + keylist.__str__()
-            )
+        # for key, cellitem in self.vars["cells"].items():
+        #     if cellitem.ndof() != 1:
+        #         keylist.append(key)
+        # if len(keylist) >= 1:
+        #     check_error = False
+        #     api.io.print(
+        #         'error', 'wrong size (ndof) of cell data: ' + keylist.__str__()
+        #     )
         return check_error
 
     def __WriteRestartHeader(self):
         """
         Method writing the header of a restart file.
         It is composed of two integers, the "magic number" used as a flag for endianness
         and the CharlesX version number.
@@ -496,31 +495,29 @@
                 )
         for key, item in self.vars["nodes"].items():
             # Tensor
             if len(item.shape) == 3:
                 pass
 
         # Then the cell based variables
-        for key, cellitem in self.vars["cells"].items():
-            item = cellitem.data()
+        for key, item in self.vars["cells"].items():
             # Scalar
             if item.size == item.shape[0]:
                 # Header
                 header = restartSectionHeader()
                 header.name = key
                 header.id = ic3_restart_codes["UGP_IO_CV_D1"]
                 header.skip = (
                     header.hsize + type2nbytes["float64"] * self.params["cv_count"]
                 )
                 header.idata[0] = self.params["cv_count"]
                 header.write(self.fid, self.endian)
                 # Field
                 BinaryWrite(self.fid, self.endian, "d" * self.params["cv_count"], item)
-        for key, cellitem in self.vars["cells"].items():
-            item = cellitem.data()
+        for key, item in self.vars["cells"].items():
             # Vector
             if len(item.shape) == 2:
                 # Header
                 header = restartSectionHeader()
                 header.name = key
                 header.id = ic3_restart_codes["UGP_IO_CV_D3"]
                 header.skip = (
@@ -532,16 +529,15 @@
                 # Field
                 BinaryWrite(
                     self.fid,
                     self.endian,
                     "d" * self.params["cv_count"] * 3,
                     item.ravel(order='C'),
                 )
-        for key, cellitem in self.vars["cells"].items():
-            item = cellitem.data()
+        for key, item in self.vars["cells"].items():
             # Tensor
             if len(item.shape) == 3:
                 # Header
                 header = restartSectionHeader()
                 header.name = key
                 header.id = ic3_restart_codes["UGP_IO_CV_D33"]
                 header.skip = (
```

### Comparing `cfdtools-0.4.2/cfdtools/ic3/writerV3.py` & `cfdtools-0.5.0/cfdtools/ic3/writerV3.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,17 +87,17 @@
                 )
         for key, item in self.vars["nodes"].items():
             # Tensor
             if len(item.shape) == 3:
                 pass
 
         # Then the cell based variables
-        for key, item in self.vars["cells"].items():
-            ndof = item.ndof()
-            npdata = item.data()
+        if self.vars["cells"]: # if defined
+            ndof = self.vars["cells"].ndof
+        for key, npdata in self.vars["cells"].items():
             ncv = self.params["cv_count"]
             totsize = ndof * ncv
             # Scalar
             if npdata.size == npdata.shape[0]:
                 # Header
                 api.io.print('std', '  write cell scalar data ' + key)
                 header = restartSectionHeader()
@@ -109,17 +109,15 @@
                 header.skip = header.hsize + type2nbytes[npdata.dtype.name] * totsize
                 header.idata[0] = ncv
                 header.idata[1] = ndof
                 header.write(self.fid, self.endian)
                 # Field
                 chartype = properties_ugpcode[header.id]['structcode']
                 BinaryWrite(self.fid, self.endian, chartype * totsize, npdata)
-        for key, item in self.vars["cells"].items():
-            ndof = item.ndof()
-            npdata = item.data()
+        for key, npdata in self.vars["cells"].items():
             totsize = ndof * self.params["cv_count"]
             # Vector
             if len(npdata.shape) == 2:
                 # Header
                 api.io.print('std', '  write cell vector data ' + key)
                 header = restartSectionHeader()
                 header.name = key
@@ -129,17 +127,15 @@
                 header.idata[1] = ndof
                 # header.idata[1] = 3
                 header.write(self.fid, self.endian)
                 # Field
                 BinaryWrite(
                     self.fid, self.endian, "d" * totsize * 3, npdata.ravel(order='C')
                 )
-        for key, item in self.vars["cells"].items():
-            ndof = item.ndof()
-            npdata = item.data()
+        for key, npdata in self.vars["cells"].items():
             totsize = ndof * self.params["cv_count"]
             # Tensor
             if len(npdata.shape) == 3:
                 # Header
                 api.io.print('std', '  write cell tensor data ' + key)
                 header = restartSectionHeader()
                 header.name = key
```

### Comparing `cfdtools-0.4.2/cfdtools/meshbase/_connectivity.py` & `cfdtools-0.5.0/cfdtools/meshbase/_connectivity.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,19 +38,19 @@
     # @property
     def range(self):
         if self._type == 'range':
             return self._range
         else:
             api.error_stop("unable to get range from list connectivity")
 
-    def set_range(self, range):
+    def set_range(self, irange):
         """define range of index with first and last included"""
         self._delete()
         self._type = 'range'
-        self._range = [*range]
+        self._range = [*irange]
 
     def list(self):
         if self._type == 'range':
             return list(range(self._range[0], self._range[1] + 1))
         elif self._type == 'list':
             return list(self._list)  # ensure list if may be
         else:
@@ -293,15 +293,14 @@
                     mergedict[key]['index'] = elemtype['index'].shift(shift)
                     mergedict[key]['elem2node'] = elemtype['elem2node']
         for elem, elemtype in mergedict.items():
             self.add_elems(elem, elemtype['elem2node'], elemtype['index'])
 
     # @profile
     def create_faces_from_elems(self):
-
         # @profile
         def __build_face_and_neighbour():
             """build a dict of face type to a list of tuples of each (oriented) face and its neighbor
 
             Args:
                 elems (dict): dict of elements with node definition
```

### Comparing `cfdtools-0.4.2/cfdtools/meshbase/_elements.py` & `cfdtools-0.5.0/cfdtools/meshbase/_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import cfdtools.api as api
+# import cfdtools.api as api
 
 geodim = {'point': 0, 'line': 1, 'surface': 2, 'volume': 3}
 
 elem_properties = [  # itype, name, nnode, geodim, extruded
     (0, 'node1', 1, 0, 'bar2'),
     (0, 'bar2', 2, 1, 'quad4'),
     (0, 'tri3', 3, 2, 'penta6'),
```

### Comparing `cfdtools-0.4.2/cfdtools/meshbase/_mesh.py` & `cfdtools-0.5.0/cfdtools/meshbase/_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import cfdtools.api as api
 import cfdtools.meshbase._connectivity as conn
-import cfdtools.meshbase._elements as ele
-from cfdtools.utils.math import minavgmax
+# import cfdtools.meshbase._elements as ele
+from cfdtools.utils.maths import minavgmax
 import itertools
 import numpy as np
 
 
 class submeshmark:
-
     # authorized geomdim type and actual dimension
     _available_geodim = (
         'node',
         'intnode',
         'bdnode',
         'face',
         'intface',
@@ -56,17 +55,17 @@
         self._index = index
 
     @property
     def type(self):
         return self._properties['type']
 
     @type.setter
-    def type(self, type):
-        assert type in self._available_types
-        self._properties['type'] = type
+    def type(self, mtype):
+        assert mtype in self._available_types
+        self._properties['type'] = mtype
 
     def nodebased(self):
         return self._geodim in {'node', 'bdnode', 'intnode'}
 
     def facebased(self):
         return self._geodim in {'face', 'bdface', 'intface'}
 
@@ -159,20 +158,16 @@
             facetype (str): _description_
             face2node (conn.elem_connectivity): _description_
             face2cell (conn.indexindirection, optional): _description_. Defaults to None.
         """
         if facetype in self.__available_facetypes:
             self._faces[facetype] = {'face2node': face2node, 'face2cell': face2cell}
         else:
-            api.io.error_stop(
-                f"bad face type: {facetype} since {self.__available_facetypes} expected"
-            )
-        self.nface = np.sum(
-            [fcon['face2node'].nelem for _, fcon in self._faces.items()]
-        )
+            api.io.error_stop(f"bad face type: {facetype} since {self.__available_facetypes} expected")
+        self.nface = np.sum([fcon['face2node'].nelem for _, fcon in self._faces.items()])
 
     def pop_faces(self, facetype: str):
         if facetype in self.__available_facetypes:
             if facetype in self._faces.keys():
                 for key, item in self._faces[facetype].items():
                     del item
                 self._faces.pop(facetype)
@@ -211,71 +206,65 @@
         assert 'boundary' in self._faces.keys()
         index_face_tuples = self._faces['boundary']['face2node'].index_elem_tuples()
         for _, boco in self._bocos.items():
             if boco.nodebased():
                 nodeset = set(boco.index.list())
                 # get all face index whose nodes are all in nodeset
                 listface_index = [
-                    i
-                    for i, _ in filter(
-                        lambda t: face_in_nodelist(t[1], nodeset), index_face_tuples
-                    )
+                    i for i, _ in filter(lambda t: face_in_nodelist(t[1], nodeset), index_face_tuples)
                 ]
                 boco.geodim = 'bdface'
                 boco.index = conn.indexlist(ilist=listface_index)
                 # print(boco.name, len(nodeset), len(boco.index.list()))
 
     def list_boco_index(self):
-        return list(itertools.chain(
-            *[boco.index.list() for _, boco in self._bocos.items()])
-        )
+        return list(itertools.chain(*[boco.index.list() for _, boco in self._bocos.items()]))
 
     def make_unmarked_BC(self, name="unmarked_faces"):
         """check all boundaring faces are marked and create a specific boco if not"""
         if 'boundary' in self._faces.keys():
             # number of (boundary) faces in face connectivity
             # nbdface = self._faces['boundary']['face2node'].nelem
             for _, boco in self._bocos.items():
                 assert boco.geodim in ('face', 'bdface'), "boco marks must be faces index"
             list_marked = self.list_boco_index()
-            list_missing = list(set(self._faces['boundary']['face2node'].all_index())-set(list_marked))
+            list_missing = list(set(self._faces['boundary']['face2node'].all_index()) - set(list_marked))
             if list_missing:
                 boco = submeshmark(name)
                 boco.geodim = 'bdface'
                 boco.type = 'boundary'
                 boco.properties['periodic_transform'] = None
                 boco.index = conn.indexlist(ilist=list_missing)
                 self.add_boco(boco)
         else:
             list_missing = []
-            api.io.print('warning', "can only reindex faces according to boco if separated in 'boundary' list")
+            api.io.print(
+                'warning', "can only reindex faces according to boco if separated in 'boundary' list"
+            )
         return list_missing
 
-
     def seekmark(self, name: str) -> submeshmark:
         """look for diffent marks set to find mark name"""
         # only _bocos for now
         return self._bocos[name]
 
     def exportmark_asmesh(self, name):
         meshmark = self.seekmark(name)
         newmesh = Mesh()
         return newmesh
 
-    def export_extruded(
-        self, direction=np.array([0.0, 0.0, 1.0]), extrude=[0.0, 1.0], domain="fluid"
-    ):
+    def export_extruded(self, direction=np.array([0.0, 0.0, 1.0]), extrude=[0.0, 1.0], domain="fluid"):
         extrude_range = np.array(extrude)
         nrange = extrude_range.size
         assert nrange > 1, "extrusion only possible for at least 2 planes"
         newmesh = Mesh(ncell=self.ncell * nrange, nnode=self.nnode * nrange)
         # SHOULD CHECK DIRECTION AND MESH ORIENTATION
         # extrude nodes
         ntotnode = self.nnode
-        newcoords = np.tile(self.nodescoord(ndarray=True), (nrange,1))
+        newcoords = np.tile(self.nodescoord(ndarray=True), (nrange, 1))
         for i, s in enumerate(extrude_range):
             newcoords[i * ntotnode : (i + 1) * ntotnode, :] += s * np.array(direction)
         newmesh.set_nodescoord_nd(newcoords)
         # extrude cells
         newmesh.set_cell2node(self._cell2node.extrude(nrange, ntotnode))
         # extrude faces if any
         # extrude/extend existing marks
@@ -341,21 +330,27 @@
         oldindex = self.list_boco_index()
         # checks
         c_unique = np.all(np.unique(oldindex) == sorted(oldindex))
         if not c_unique:
             api.io.print('error', "  some faces are marked by several boundary marks")
         c_min0 = min(oldindex) == 0
         if not c_min0:
-            api.io.print('error', "  first face index (0) is not marked as a boundary\n"+
-                           "  some boundary faces may be missing")
+            api.io.print(
+                'error',
+                "  first face index (0) is not marked as a boundary\n"
+                + "  some boundary faces may be missing",
+            )
         c_max = max(oldindex) <= len(oldindex) - 1
         if not c_max:
-            api.io.print('error', "  max face reference is greater than the number of found faces\n"+
-                         "  boundary faces must be indexed first before reindexing")
-        c_lengths = len(oldindex)==nbdface
+            api.io.print(
+                'error',
+                "  max face reference is greater than the number of found faces\n"
+                + "  boundary faces must be indexed first before reindexing",
+            )
+        c_lengths = len(oldindex) == nbdface
         if not c_lengths:
             api.io.print('error', f"  some boundary faces are not marked: {nbdface-len(oldindex)}")
         if not (c_unique and c_min0 and c_max):
             api.error_stop("inconsistent face marks when reordering")
         newindex = np.full_like(oldindex, -1)
         newindex[oldindex] = np.arange(len(oldindex))
         assert min(newindex) >= 0, "inconsistency: there must not be -1 index"
@@ -364,39 +359,33 @@
             boco.index = conn.indexlist(ilist=newindex[boco.index.list()].tolist())
             boco.index.compress()  # try to (and must) make it a range
         # reindex boundary faces
         for _, fdict in self._faces['boundary']['face2node'].items():
             fdict['index'] = conn.indexlist(ilist=newindex[fdict['index'].list()].tolist())
             # fdict['index'].compress() # not expected
         if 'face2cell' in self._faces['boundary']:
-            self._faces['boundary']['face2cell'].conn = self._faces['boundary'][
-                'face2cell'
-            ].conn[oldindex, :]
+            self._faces['boundary']['face2cell'].conn = self._faces['boundary']['face2cell'].conn[oldindex, :]
 
     def printinfo(self, detailed=False):
         api.io.print("std", f"nnode: {self.nnode}")
         for c in ('x', 'y', 'z'):
             api.io.printstd(
-                "  {} min:avg:max = {:.3f}:{:.3f}:{:.3f}".format(
-                    c, *minavgmax(self._nodes[c])
-                ),
+                "  {} min:avg:max = {:.3f}:{:.3f}:{:.3f}".format(c, *minavgmax(self._nodes[c])),
             )
 
         api.io.print("std", f"ncell: {self.ncell}")
         if self._cell2node:
             self._cell2node.print()
         else:
             api.io.print("std", "  no cell/node connectivity")
         api.io.print('std', "nnode:", self.nnode)
         api.io.print('std', "nface:", self.nface)
         if self._faces:
             for t, facedict in self._faces.items():
-                api.io.print(
-                    "std", f"  type {t}: {' '.join(facedict['face2node'].elems())}"
-                )
+                api.io.print("std", f"  type {t}: {' '.join(facedict['face2node'].elems())}")
                 facedict['face2node'].print(prefix='  . ', detailed=detailed)
         else:
             api.io.print("std", "  no face/node connectivity")
         api.io.print('std', f"bocos: {' '.join(self._bocos.keys())}")
         for name, boco in self._bocos.items():
             api.io.print("std", f"  BC {boco}")
         api.io.print("std", "params:", self._params)
```

### Comparing `cfdtools-0.4.2/cfdtools/meshbase/simple.py` & `cfdtools-0.5.0/cfdtools/meshbase/simple.py`

 * *Files identical despite different names*

### Comparing `cfdtools-0.4.2/cfdtools/probes/data.py` & `cfdtools-0.5.0/cfdtools/probes/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 from shutil import Error
 import numpy as np
 import cfdtools.api as api
 
 # options definition
 
 varname_syn = {  # name for line_probe
-    "X": ["x"],
+    "X": ["x", "X"],
     "Y": ["y"],
     "Z": ["z"],
     "P": ["p", "ps", "Ps", "PS"],
     "U-X": ["UX", "Ux", "ux", "U_X", "U_x"],
-    "X": ["X", "x"],
 }
 
 
 def minavgmax(d):
     return (f(d) for f in [np.min, np.average, np.max])
 
 
@@ -41,17 +40,15 @@
             "INVX-": self.compute_invxm,
             "S": self.compute_entropy,
         }
 
     # TODO: this part should be moved to physics module
     def compute_U(self):
         self.alldata['U'] = np.sqrt(
-            self.alldata['U-X'] ** 2
-            + self.alldata['U-Y'] ** 2
-            + self.alldata['U-Z'] ** 2
+            self.alldata['U-X'] ** 2 + self.alldata['U-Y'] ** 2 + self.alldata['U-Z'] ** 2
         )
 
     def compute_Mach(self):
         self.alldata['Mach'] = self.alldata['U'] / self.alldata['Asound']
 
     def compute_Asound(self):
         self.alldata['Asound'] = np.sqrt(1.4 * self.alldata['P'] / self.alldata['RHO'])
@@ -59,69 +56,57 @@
     def compute_invxp(self):
         self.alldata['INVX+'] = 5 * self.alldata['Asound'] + self.alldata['U-X']
 
     def compute_invxm(self):
         self.alldata['INVX-'] = 5 * self.alldata['Asound'] - self.alldata['U-X']
 
     def compute_entropy(self):
-        self.alldata['S'] = (
-            1.0 / 0.4 * np.log(self.alldata['P'] / self.alldata['RHO'] ** 1.4)
-        )
+        self.alldata['S'] = 1.0 / 0.4 * np.log(self.alldata['P'] / self.alldata['RHO'] ** 1.4)
 
     def check_data(self, varname, prefix=""):
         if self.verbose:
-            print("- request " + varname)
+            api.io.printstd("- request " + varname)
         success = varname in self.alldata
         if not success:
             # try to directly read data
             success = self.read_data(varname, prefix)
         if not success:  # try to compute it
             if varname in self.dependency_vars:
-                success = np.all(
-                    [
-                        self.check_data(depvar)
-                        for depvar in self.dependency_vars[varname]
-                    ]
-                )
+                success = np.all([self.check_data(depvar) for depvar in self.dependency_vars[varname]])
             if success:
                 if self.verbose:
-                    print("- compute " + varname)
+                    api.io.printstd("- compute " + varname)
                 self.compute_varname[varname]()
             else:
                 raise NameError(varname + " missing or unable to compute")
         if success:
             api.io.print(
                 'std',
                 "- "
                 + varname
-                + " min:avg:max = {:.3f} : {:.3f} : {:.3f}".format(
-                    *minavgmax(self.alldata[varname])
-                ),
+                + " min:avg:max = {:.3f} : {:.3f} : {:.3f}".format(*minavgmax(self.alldata[varname])),
             )
         return success
 
     def read_data(self, varname, prefix=""):
         fname = prefix + "." + varname
         if os.path.exists(fname):
             if self.verbose:
-                print("- read " + varname + " in " + fname)
+                api.io.printstd("- read " + varname + " in " + fname)
             rdata = np.genfromtxt(fname, delimiter=" ")
             if rdata.ndim == 1:  # supposed to be coordinate
-                self.alldata[varname] = rdata[
-                    3:
-                ]  # extract only coordinate (remove time and it)
+                # extract only coordinate (remove time and it)
+                self.alldata[varname] = rdata[3:]
             elif rdata.ndim == 2:  # supposed to be data
-                self.alldata[varname] = rdata[
-                    :, 3:
-                ]  # extract data  (remove time and it)
-                if (
-                    "time" not in self.alldata
-                ):  # if time missing, get it from current data, no consistency test with other data
+                # extract data  (remove time and it)
+                self.alldata[varname] = rdata[:, 3:]
+                if ("time" not in self.alldata):  
+                    # if time missing, get it from current data, no consistency test with other data
                     if self.verbose:
-                        print(" . define 'time'")
+                        api.io.printstd(" . define 'time'")
                     self.alldata["time"] = rdata[:, 1]
             else:
                 raise Error("unexpected data size " + varname)
             return True  # success
         else:
             return False  # no file
```

### Comparing `cfdtools-0.4.2/cfdtools/probes/plot.py` & `cfdtools-0.5.0/cfdtools/probes/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt
 import cfdtools.api as api
 import cfdtools.plot as cfdplt
-from cfdtools.utils.math import minavgmax
+from cfdtools.utils.maths import minavgmax
 import numpy as np
 import numpy.fft as fftm
 
 
 def check_axis(axisdata):
     if axisdata.ndim > 1:
         axis = np.mean(axisdata, axis=0)
@@ -83,15 +83,15 @@
     # plt.legend(labels, loc='upper left',prop={'size':10})
     # plt.axis([0., 50., 0., 90.])
     fig = plt.figure(1, figsize=(10, 8))
     plt.xlabel(axis, fontsize=10)
     plt.ylabel("frequency", fontsize=10)
     n = data.alldata[var].shape[0]
     f = fftm.fftfreq(n, dtavg)
-    psdmap = np.abs(fftm.fft(data.alldata[var], axis=0))
+    psdmap = np.abs(fftm.fft(data.alldata[var]-np.average(data.alldata[var]), axis=0))
     if kwargs['verbose']:
         api.io.print('std', data.alldata[var].shape, n, psdmap.shape, f.shape)
     colmap = cfdplt.normalizeCmap(cmap, nlevels)
     axis = check_axis(data.alldata[axis])
     plt.contourf(
         axis,
         f[1 : n // 200],
```

### Comparing `cfdtools-0.4.2/cfdtools.egg-info/PKG-INFO` & `cfdtools-0.5.0/cfdtools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfdtools
-Version: 0.4.2
+Version: 0.5.0
 Summary: Tools for mesh and solution management in CFD
 Author-email: "J. Gressier" <jeremie.gressier@isae-supaero.fr>
 License: MIT License
         
         Copyright (c) 2022 Jérémie GRESSIER
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -55,19 +55,23 @@
 
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/d32cf67a5fa242c88bb1568277f1d60e)](https://app.codacy.com/gh/jgressier/cfdtools/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)[![Doc](https://readthedocs.org/projects/cfdtools/badge/?version=latest)](https://readthedocs.org/projects/cfdtools/)
 [![Slack](https://img.shields.io/static/v1?logo=slack&label=slack&message=contact&style=flat)](https://join.slack.com/t/isae-opendev/shared_invite/zt-obqywf6r-UUuHR4_hc5iTzyL5bFCwpw
 )
 
 ### Features
 
-    - IC3 v2 or v3 reader
-    - IC3 v2 or v3 writer
-    - generic format command line: `cfdinfo`, `cfdwrite_ic3v3`
-    - specific IC3 command line: `ic3brief`
+- readers: IC3, VTK, GMSH, CGNS
+- writers: IC3, VTK
+- generic options for command line writers: extrusion
+- generic format command line: `cfdinfo`
+- specific IC3 command line: `ic3brief`
+- specific VTK command line: `vtkbrief`
 
 ### Installation and usage
 
-    pip install cfdtools
+```bash
+pip install cfdtools
+```
 
 ### Requirements
 
 see [requirements.txt](https://github.com/jgressier/cfdtools/blob/master/requirements.txt)
```

### Comparing `cfdtools-0.4.2/cfdtools.egg-info/SOURCES.txt` & `cfdtools-0.5.0/cfdtools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 cfdtools/__init__.py
 cfdtools/_cli.py
 cfdtools/api.py
+cfdtools/data.py
 cfdtools/plot.py
 cfdtools.egg-info/PKG-INFO
 cfdtools.egg-info/SOURCES.txt
 cfdtools.egg-info/dependency_links.txt
 cfdtools.egg-info/entry_points.txt
 cfdtools.egg-info/requires.txt
 cfdtools.egg-info/top_level.txt
@@ -21,31 +22,36 @@
 cfdtools/ic3/__init__.py
 cfdtools/ic3/_ic3.py
 cfdtools/ic3/reader_legacy.py
 cfdtools/ic3/writerV2.py
 cfdtools/ic3/writerV3.py
 cfdtools/meshbase/__init__.py
 cfdtools/meshbase/_connectivity.py
-cfdtools/meshbase/_data.py
 cfdtools/meshbase/_elements.py
 cfdtools/meshbase/_geom.py
 cfdtools/meshbase/_mesh.py
 cfdtools/meshbase/simple.py
 cfdtools/physics/dicovar.py
 cfdtools/probes/__init__.py
 cfdtools/probes/data.py
 cfdtools/probes/plot.py
 cfdtools/utils/__init__.py
-cfdtools/utils/math.py
+cfdtools/utils/_dev.py
+cfdtools/utils/maths.py
+cfdtools/utils/polybase.py
 cfdtools/vtk/__init__.py
 cfdtools/vtk/_vtk.py
 tests/test_0_api.py
 tests/test_0_connectivity.py
+tests/test_0_h5.py
+tests/test_0_polybase.py
 tests/test_1_cgns.py
+tests/test_1_data.py
 tests/test_1_gmsh.py
 tests/test_1_ic3.py
 tests/test_1_simple.py
 tests/test_1_vtk.py
 tests/test_2_cli.py
 tests/test_2_convert.py
+tests/test_2_data.py
 tests/test_2_mesh.py
 tests/test_probes.py
```

### Comparing `cfdtools-0.4.2/pyproject.toml` & `cfdtools-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cfdtools"
-version = "0.4.2"
+version = "0.5.0"
 description = "Tools for mesh and solution management in CFD"
 authors = [{name="J. Gressier", email="jeremie.gressier@isae-supaero.fr"}]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
@@ -17,15 +17,16 @@
     "Programming Language :: Python :: 3.10",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development :: Libraries :: Python Modules" ]
 requires-python = ">=3.7"
 dependencies = [
     "numpy >= 1.15",
-    "h5py", "pyvista >= 0.38" ]
+    "scipy >= 1.6",
+    "h5py >= 3.1", "pyvista >= 0.38" ]
 
 [project.urls]
 Homepage = "https://github.com/jgressier/cfdtools"
 Documentation = "https://cfdtools.readthedocs.io/en/latest/"
 
 [tool.setuptools.packages.find] # to help find cfdtools folder as a package
 include = ["cfdtools*"]
@@ -35,14 +36,15 @@
 cfdwritecube = 'cfdtools._cli:writecube'
 ic3brief = 'cfdtools._cli:ic3brief'
 ic3probe_plotline = 'cfdtools._cli:ic3probe_plotline'
 cfdwrite_ic3v2 = 'cfdtools._cli:write_ic3v2'
 cfdwrite_ic3v3 = 'cfdtools._cli:write_ic3v3'
 cfdwrite_ic3 = 'cfdtools._cli:write_ic3v3'
 cfdwrite_vtk = 'cfdtools._cli:write_vtk'
+vtkbrief = 'cfdtools._cli:vtkbrief'
 
 [project.optional-dependencies]
 dev = [ 
     "pytest >= 6.0", 
     "pytest-cov >= 2.11.1",
     "pylint >= 2.6.0" ]
 doc = [ 
@@ -61,15 +63,15 @@
 minversion = "6.0"
 addopts = "--cov -v"
 testpaths = [
     "tests"
 ]
 
 [tool.bumpver]
-current_version = "v0.4.2"
+current_version = "v0.5.0"
 version_pattern = "vMAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} to {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `cfdtools-0.4.2/tests/test_0_connectivity.py` & `cfdtools-0.5.0/tests/test_0_connectivity.py`

 * *Files identical despite different names*

### Comparing `cfdtools-0.4.2/tests/test_1_cgns.py` & `cfdtools-0.5.0/tests/test_1_cgns.py`

 * *Files identical despite different names*

### Comparing `cfdtools-0.4.2/tests/test_1_gmsh.py` & `cfdtools-0.5.0/tests/test_1_gmsh.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,24 +21,32 @@
 def test_reader(filename):
     gmesh = gmsh.reader(_datadir.joinpath(filename))
     gmesh.read_data()
     rmesh = gmesh.export_mesh()
     assert rmesh.check()
 
 
-@pytest.mark.parametrize("filename", ["box3d-v22.msh", "box3d-v41.msh", "test_3d.msh"])
+@pytest.mark.parametrize(
+    "filename",
+    [
+        "box3d-v22.msh",
+        "box3d-v41.msh",
+        "test_3d.msh",
+    ],
+)
 def test_convert_ic3(filename):
     gmesh = gmsh.reader(_datadir.joinpath(filename))
     gmesh.read_data()
     rmesh = gmesh.export_mesh()
     ic3write = ic3writer.writer(rmesh)
     _builddir.mkdir(exist_ok=True)
     outfile = api._files(_builddir / Path(filename))
     outfile.change_suffix('.ic3')
     ic3write.write_data(outfile.filename)
+    Path(outfile.filename).unlink()
 
 
 # def test_reader3dv22():
 #     rmesh = gmsh.reader(_datadir+'box3d-v22.msh')
 #     rmesh = gmshmesh.read_data()
 #     assert rmesh.check()
```

### Comparing `cfdtools-0.4.2/tests/test_1_ic3.py` & `cfdtools-0.5.0/tests/test_1_ic3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 import pytest
 import cfdtools.ic3.reader_legacy as ic3reader
 import cfdtools.ic3.writerV2 as ic3wv2
-import cfdtools.ic3.writerV3 as ic3wv3
+# import cfdtools.ic3.writerV3 as ic3wv3
 from pathlib import Path
 import filecmp
 
-_datadir = Path("./tests/data")
-_builddir = Path("./tests/build")
-
 
 @pytest.mark.parametrize(
     "filename", ["Box3x3x2v2.ic3", "Box3x3x2v3.ic3", "nrg-tinycube-v2.ic3"]
 )
-def test_reader(filename):
-    ic3mesh = ic3reader.reader(_datadir.joinpath(filename))
+def test_reader(datadir, filename):
+    ic3mesh = ic3reader.reader(datadir / filename, cIntegrity=True)
     ic3mesh.read_data()
     ic3mesh.printinfo()
     rmesh = ic3mesh.export_mesh()
     assert rmesh.check()
 
 
 @pytest.mark.parametrize("filename", ["Box3x3x2v2.ic3", "nrg-tinycube-v2.ic3"])
-def test_writer_v2_litend(filename):
-    _builddir.mkdir(exist_ok=True)
-    basefile = _datadir / filename
-    outfile = _builddir / filename
+def test_writer_v2_litend(datadir, builddir, filename):
+    builddir.mkdir(exist_ok=True)
+    basefile = datadir / filename
+    outfile = builddir / filename
     ic3read = ic3reader.reader(basefile)
     ic3read.read_data()
     rmesh = ic3read.export_mesh()
     assert rmesh.check()
     ic3write = ic3wv2.writer(rmesh, endian='little')
     ic3write.write_data(outfile)
     assert filecmp.cmp(basefile, outfile)
+    outfile.unlink()
 
 
 # @pytest.mark.parametrize("filename", ["sam_sd3.ic3"])
 # def test_writer_v3_litend(filename):
 #     _builddir.mkdir(exist_ok = True)
 #     basefile = _datadir / filename
 #     outfile = _builddir / filename
```

### Comparing `cfdtools-0.4.2/tests/test_2_convert.py` & `cfdtools-0.5.0/tests/test_2_convert.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 _datadir = Path("./tests/data")
 _builddir = Path("./tests/build")
 
 
 @pytest.mark.parametrize("filename", ["box3d-v22.msh", "box3d-v41.msh", "test_3d.msh"])
 def test_gmsh_to_ic3(filename):
-    input = gmsh.reader(_datadir.joinpath(filename))
-    input.read_data()
-    rmesh = input.export_mesh()
+    inputm = gmsh.reader(_datadir / filename)
+    inputm.read_data()
+    rmesh = inputm.export_mesh()
     ic3write = ic3writer.writer(rmesh)
-    outfile = api._files(_builddir / Path(filename))
+    outfile = api._files(_builddir / filename)
     outfile.change_suffix('.ic3')
     ic3write.write_data(outfile.filename)
+    Path(outfile.filename).unlink()
```

