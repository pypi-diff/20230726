# Comparing `tmp/xugrid-0.6.1.tar.gz` & `tmp/xugrid-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xugrid-0.6.1.tar", last modified: Fri Jul  7 15:08:05 2023, max compression
+gzip compressed data, was "xugrid-0.6.2.tar", last modified: Wed Jul 26 11:24:59 2023, max compression
```

## Comparing `xugrid-0.6.1.tar` & `xugrid-0.6.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.837699 xugrid-0.6.1/
--rw-rw-rw-   0        0        0     1079 2021-09-15 16:10:43.000000 xugrid-0.6.1/LICENSE
--rw-rw-rw-   0        0        0       34 2021-10-06 12:44:47.000000 xugrid-0.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3298 2023-07-07 15:08:05.837699 xugrid-0.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     2157 2023-03-13 10:25:22.000000 xugrid-0.6.1/README.rst
--rw-rw-rw-   0        0        0     2199 2023-07-07 15:03:53.000000 xugrid-0.6.1/pyproject.toml
--rw-rw-rw-   0        0        0      178 2023-07-07 15:08:05.840699 xugrid-0.6.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.595715 xugrid-0.6.1/tests/
--rw-rw-rw-   0        0        0    17755 2023-07-05 13:51:43.000000 xugrid-0.6.1/tests/test_connectivity.py
--rw-rw-rw-   0        0        0    10108 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_conventions.py
--rw-rw-rw-   0        0        0     9008 2023-07-05 13:51:43.000000 xugrid-0.6.1/tests/test_conversion.py
--rw-rw-rw-   0        0        0     1008 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_data.py
--rw-rw-rw-   0        0        0      851 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_interpolate.py
--rw-rw-rw-   0        0        0     1219 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_meshkernel_utils.py
--rw-rw-rw-   0        0        0     8494 2023-06-26 11:20:36.000000 xugrid-0.6.1/tests/test_partitioning.py
--rw-rw-rw-   0        0        0     9084 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_plot.py
--rw-rw-rw-   0        0        0     4245 2023-03-13 10:25:22.000000 xugrid-0.6.1/tests/test_snap.py
--rw-rw-rw-   0        0        0    11263 2023-07-05 13:51:43.000000 xugrid-0.6.1/tests/test_ugrid1d.py
--rw-rw-rw-   0        0        0    32742 2023-06-26 11:20:36.000000 xugrid-0.6.1/tests/test_ugrid2d.py
--rw-rw-rw-   0        0        0    34035 2023-07-07 15:02:46.000000 xugrid-0.6.1/tests/test_ugrid_dataset.py
--rw-rw-rw-   0        0        0    10444 2023-04-21 11:32:07.000000 xugrid-0.6.1/tests/test_voronoi.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.619697 xugrid-0.6.1/xugrid/
--rw-rw-rw-   0        0        0     1020 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/__init__.py
--rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/constants.py
--rw-rw-rw-   0        0        0     8398 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/conversion.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.667696 xugrid-0.6.1/xugrid/core/
--rw-rw-rw-   0        0        0     4322 2023-06-26 11:20:36.000000 xugrid-0.6.1/xugrid/core/accessorbase.py
--rw-rw-rw-   0        0        0     3516 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/core/common.py
--rw-rw-rw-   0        0        0    18334 2023-04-21 11:32:07.000000 xugrid-0.6.1/xugrid/core/dataarray_accessor.py
--rw-rw-rw-   0        0        0    13439 2023-04-21 11:32:07.000000 xugrid-0.6.1/xugrid/core/dataset_accessor.py
--rw-rw-rw-   0        0        0    11821 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/core/wrap.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.687699 xugrid-0.6.1/xugrid/data/
--rw-rw-rw-   0        0        0      126 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/data/__init__.py
--rw-rw-rw-   0        0        0      331 2023-04-21 11:32:07.000000 xugrid-0.6.1/xugrid/data/registry.txt
--rw-rw-rw-   0        0        0     2109 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/data/sample_data.py
--rw-rw-rw-   0        0        0     3083 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/data/synthetic.py
--rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/meshkernel_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.700696 xugrid-0.6.1/xugrid/plot/
--rw-rw-rw-   0        0        0      149 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/plot/__init__.py
--rw-rw-rw-   0        0        0    24101 2023-06-26 11:20:36.000000 xugrid-0.6.1/xugrid/plot/plot.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.739698 xugrid-0.6.1/xugrid/regrid/
--rw-rw-rw-   0        0        0     7616 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/regrid/overlap_1d.py
--rw-rw-rw-   0        0        0     5015 2023-03-14 17:12:37.000000 xugrid-0.6.1/xugrid/regrid/reduce.py
--rw-rw-rw-   0        0        0    18493 2023-07-05 13:51:43.000000 xugrid-0.6.1/xugrid/regrid/regridder.py
--rw-rw-rw-   0        0        0    23864 2023-07-05 13:51:43.000000 xugrid-0.6.1/xugrid/regrid/structured.py
--rw-rw-rw-   0        0        0     4883 2023-06-26 11:20:36.000000 xugrid-0.6.1/xugrid/regrid/unstructured.py
--rw-rw-rw-   0        0        0     1245 2023-05-25 15:11:34.000000 xugrid-0.6.1/xugrid/regrid/utils.py
--rw-rw-rw-   0        0        0     3661 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/regrid/weight_matrix.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.835699 xugrid-0.6.1/xugrid/ugrid/
--rw-rw-rw-   0        0        0        0 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/ugrid/__init__.py
--rw-rw-rw-   0        0        0    24707 2023-07-05 13:51:43.000000 xugrid-0.6.1/xugrid/ugrid/connectivity.py
--rw-rw-rw-   0        0        0    14841 2023-04-21 11:32:07.000000 xugrid-0.6.1/xugrid/ugrid/conventions.py
--rw-rw-rw-   0        0        0     4996 2023-03-13 10:25:22.000000 xugrid-0.6.1/xugrid/ugrid/interpolate.py
--rw-rw-rw-   0        0        0    11044 2023-06-26 11:20:36.000000 xugrid-0.6.1/xugrid/ugrid/partitioning.py
--rw-rw-rw-   0        0        0    15005 2023-07-05 13:51:43.000000 xugrid-0.6.1/xugrid/ugrid/snapping.py
--rw-rw-rw-   0        0        0    19654 2023-07-05 13:51:43.000000 xugrid-0.6.1/xugrid/ugrid/ugrid1d.py
--rw-rw-rw-   0        0        0    56167 2023-07-07 15:02:46.000000 xugrid-0.6.1/xugrid/ugrid/ugrid2d.py
--rw-rw-rw-   0        0        0    22700 2023-07-07 15:02:46.000000 xugrid-0.6.1/xugrid/ugrid/ugridbase.py
--rw-rw-rw-   0        0        0    14113 2023-04-21 11:32:07.000000 xugrid-0.6.1/xugrid/ugrid/voronoi.py
-drwxrwxrwx   0        0        0        0 2023-07-07 15:08:05.634697 xugrid-0.6.1/xugrid.egg-info/
--rw-rw-rw-   0        0        0     3298 2023-07-07 15:08:05.000000 xugrid-0.6.1/xugrid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1338 2023-07-07 15:08:05.000000 xugrid-0.6.1/xugrid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 15:08:05.000000 xugrid-0.6.1/xugrid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      252 2023-07-07 15:08:05.000000 xugrid-0.6.1/xugrid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-07 15:08:05.000000 xugrid-0.6.1/xugrid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:59.886352 xugrid-0.6.2/
+-rw-rw-rw-   0        0        0     1079 2021-09-15 16:10:43.000000 xugrid-0.6.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2021-10-06 12:44:47.000000 xugrid-0.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3298 2023-07-26 11:24:59.886352 xugrid-0.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2157 2023-03-13 10:25:22.000000 xugrid-0.6.2/README.rst
+-rw-rw-rw-   0        0        0     2199 2023-07-26 11:23:41.000000 xugrid-0.6.2/pyproject.toml
+-rw-rw-rw-   0        0        0      178 2023-07-26 11:24:59.887352 xugrid-0.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:59.811427 xugrid-0.6.2/tests/
+-rw-rw-rw-   0        0        0    17755 2023-07-05 13:51:43.000000 xugrid-0.6.2/tests/test_connectivity.py
+-rw-rw-rw-   0        0        0    10108 2023-03-13 10:25:22.000000 xugrid-0.6.2/tests/test_conventions.py
+-rw-rw-rw-   0        0        0     9008 2023-07-05 13:51:43.000000 xugrid-0.6.2/tests/test_conversion.py
+-rw-rw-rw-   0        0        0     1008 2023-03-13 10:25:22.000000 xugrid-0.6.2/tests/test_data.py
+-rw-rw-rw-   0        0        0      851 2023-03-13 10:25:22.000000 xugrid-0.6.2/tests/test_interpolate.py
+-rw-rw-rw-   0        0        0     1219 2023-03-13 10:25:22.000000 xugrid-0.6.2/tests/test_meshkernel_utils.py
+-rw-rw-rw-   0        0        0     8494 2023-06-26 11:20:36.000000 xugrid-0.6.2/tests/test_partitioning.py
+-rw-rw-rw-   0        0        0     9084 2023-03-13 10:25:22.000000 xugrid-0.6.2/tests/test_plot.py
+-rw-rw-rw-   0        0        0     4245 2023-03-13 10:25:22.000000 xugrid-0.6.2/tests/test_snap.py
+-rw-rw-rw-   0        0        0    11263 2023-07-05 13:51:43.000000 xugrid-0.6.2/tests/test_ugrid1d.py
+-rw-rw-rw-   0        0        0    32742 2023-06-26 11:20:36.000000 xugrid-0.6.2/tests/test_ugrid2d.py
+-rw-rw-rw-   0        0        0    34477 2023-07-26 11:02:31.000000 xugrid-0.6.2/tests/test_ugrid_dataset.py
+-rw-rw-rw-   0        0        0    10444 2023-04-21 11:32:07.000000 xugrid-0.6.2/tests/test_voronoi.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:59.817355 xugrid-0.6.2/xugrid/
+-rw-rw-rw-   0        0        0     1020 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/constants.py
+-rw-rw-rw-   0        0        0     8398 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/conversion.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:59.834362 xugrid-0.6.2/xugrid/core/
+-rw-rw-rw-   0        0        0     4322 2023-06-26 11:20:36.000000 xugrid-0.6.2/xugrid/core/accessorbase.py
+-rw-rw-rw-   0        0        0     3516 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/core/common.py
+-rw-rw-rw-   0        0        0    18334 2023-04-21 11:32:07.000000 xugrid-0.6.2/xugrid/core/dataarray_accessor.py
+-rw-rw-rw-   0        0        0    13439 2023-04-21 11:32:07.000000 xugrid-0.6.2/xugrid/core/dataset_accessor.py
+-rw-rw-rw-   0        0        0    11821 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/core/wrap.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:59.841354 xugrid-0.6.2/xugrid/data/
+-rw-rw-rw-   0        0        0      126 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/data/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-04-21 11:32:07.000000 xugrid-0.6.2/xugrid/data/registry.txt
+-rw-rw-rw-   0        0        0     2109 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/data/sample_data.py
+-rw-rw-rw-   0        0        0     3083 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/data/synthetic.py
+-rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/meshkernel_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:59.845354 xugrid-0.6.2/xugrid/plot/
+-rw-rw-rw-   0        0        0      149 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/plot/__init__.py
+-rw-rw-rw-   0        0        0    24080 2023-07-26 11:02:31.000000 xugrid-0.6.2/xugrid/plot/plot.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:59.860353 xugrid-0.6.2/xugrid/regrid/
+-rw-rw-rw-   0        0        0     7616 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/regrid/overlap_1d.py
+-rw-rw-rw-   0        0        0     5015 2023-03-14 17:12:37.000000 xugrid-0.6.2/xugrid/regrid/reduce.py
+-rw-rw-rw-   0        0        0    18883 2023-07-26 11:02:31.000000 xugrid-0.6.2/xugrid/regrid/regridder.py
+-rw-rw-rw-   0        0        0    24230 2023-07-26 11:02:31.000000 xugrid-0.6.2/xugrid/regrid/structured.py
+-rw-rw-rw-   0        0        0     4883 2023-06-26 11:20:36.000000 xugrid-0.6.2/xugrid/regrid/unstructured.py
+-rw-rw-rw-   0        0        0     1245 2023-05-25 15:11:34.000000 xugrid-0.6.2/xugrid/regrid/utils.py
+-rw-rw-rw-   0        0        0     3661 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/regrid/weight_matrix.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:59.884354 xugrid-0.6.2/xugrid/ugrid/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/ugrid/__init__.py
+-rw-rw-rw-   0        0        0    24707 2023-07-05 13:51:43.000000 xugrid-0.6.2/xugrid/ugrid/connectivity.py
+-rw-rw-rw-   0        0        0    14841 2023-04-21 11:32:07.000000 xugrid-0.6.2/xugrid/ugrid/conventions.py
+-rw-rw-rw-   0        0        0     4996 2023-03-13 10:25:22.000000 xugrid-0.6.2/xugrid/ugrid/interpolate.py
+-rw-rw-rw-   0        0        0    11044 2023-06-26 11:20:36.000000 xugrid-0.6.2/xugrid/ugrid/partitioning.py
+-rw-rw-rw-   0        0        0    15005 2023-07-05 13:51:43.000000 xugrid-0.6.2/xugrid/ugrid/snapping.py
+-rw-rw-rw-   0        0        0    19654 2023-07-05 13:51:43.000000 xugrid-0.6.2/xugrid/ugrid/ugrid1d.py
+-rw-rw-rw-   0        0        0    56167 2023-07-07 15:02:46.000000 xugrid-0.6.2/xugrid/ugrid/ugrid2d.py
+-rw-rw-rw-   0        0        0    22700 2023-07-07 15:02:46.000000 xugrid-0.6.2/xugrid/ugrid/ugridbase.py
+-rw-rw-rw-   0        0        0    14113 2023-04-21 11:32:07.000000 xugrid-0.6.2/xugrid/ugrid/voronoi.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:24:59.823357 xugrid-0.6.2/xugrid.egg-info/
+-rw-rw-rw-   0        0        0     3298 2023-07-26 11:24:59.000000 xugrid-0.6.2/xugrid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2023-07-26 11:24:59.000000 xugrid-0.6.2/xugrid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 11:24:59.000000 xugrid-0.6.2/xugrid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      252 2023-07-26 11:24:59.000000 xugrid-0.6.2/xugrid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 11:24:59.000000 xugrid-0.6.2/xugrid.egg-info/top_level.txt
```

### Comparing `xugrid-0.6.1/LICENSE` & `xugrid-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/PKG-INFO` & `xugrid-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.6.1
+Version: 0.6.2
 Summary: Xarray extension for unstructured grids
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Keywords: mesh,ugrid,unstructured grid,xarray
```

### Comparing `xugrid-0.6.1/README.rst` & `xugrid-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/pyproject.toml` & `xugrid-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xugrid"
 description = "Xarray extension for unstructured grids"
 readme = { file = "README.rst", content-type = "text/x-rst" }
-version = "0.6.1"
+version = "0.6.2"
 maintainers = [{ name = "Huite Bootsma", email = "huite.bootsma@deltares.nl" }]
 requires-python = ">=3.7"
 dependencies = [
     'pandas',
     'numba',
     'numba_celltree',
     'numpy',
```

### Comparing `xugrid-0.6.1/tests/test_connectivity.py` & `xugrid-0.6.2/tests/test_connectivity.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_conventions.py` & `xugrid-0.6.2/tests/test_conventions.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_conversion.py` & `xugrid-0.6.2/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_data.py` & `xugrid-0.6.2/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_interpolate.py` & `xugrid-0.6.2/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_meshkernel_utils.py` & `xugrid-0.6.2/tests/test_meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_partitioning.py` & `xugrid-0.6.2/tests/test_partitioning.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_plot.py` & `xugrid-0.6.2/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_snap.py` & `xugrid-0.6.2/tests/test_snap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_ugrid1d.py` & `xugrid-0.6.2/tests/test_ugrid1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_ugrid2d.py` & `xugrid-0.6.2/tests/test_ugrid2d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/tests/test_ugrid_dataset.py` & `xugrid-0.6.2/tests/test_ugrid_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,14 +373,25 @@
 
         path = tmp_path / "test.nc"
         uda.ugrid.to_netcdf(path)
         back = xugrid.open_dataarray(path, chunks={"time": 1})
         primitive = back.isel(time=0).ugrid.plot()
         assert primitive is not None
 
+    def test_plot_contourf_with_chunks(self, tmp_path):
+        time = xr.DataArray([0.0, 1.0, 2.0], coords={"time": [0, 1, 2]})
+        uda = (self.uda * time).transpose()
+        uda.name = "test"
+
+        path = tmp_path / "test.nc"
+        uda.ugrid.to_netcdf(path)
+        back = xugrid.open_dataarray(path, chunks={"time": 1})
+        primitive = back.isel(time=0).ugrid.plot.contourf()
+        assert primitive is not None
+
 
 class TestUgridDataset:
     @pytest.fixture(autouse=True)
     def setup(self):
         ds = xr.Dataset()
         ds["a"] = DARRAY()
         ds["b"] = DARRAY() * 2
```

### Comparing `xugrid-0.6.1/tests/test_voronoi.py` & `xugrid-0.6.2/tests/test_voronoi.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/__init__.py` & `xugrid-0.6.2/xugrid/__init__.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/constants.py` & `xugrid-0.6.2/xugrid/constants.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/conversion.py` & `xugrid-0.6.2/xugrid/conversion.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/core/accessorbase.py` & `xugrid-0.6.2/xugrid/core/accessorbase.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/core/common.py` & `xugrid-0.6.2/xugrid/core/common.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/core/dataarray_accessor.py` & `xugrid-0.6.2/xugrid/core/dataarray_accessor.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/core/dataset_accessor.py` & `xugrid-0.6.2/xugrid/core/dataset_accessor.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/core/wrap.py` & `xugrid-0.6.2/xugrid/core/wrap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/data/sample_data.py` & `xugrid-0.6.2/xugrid/data/sample_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/data/synthetic.py` & `xugrid-0.6.2/xugrid/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/meshkernel_utils.py` & `xugrid-0.6.2/xugrid/meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/plot/plot.py` & `xugrid-0.6.2/xugrid/plot/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -584,15 +584,14 @@
     Parameters
     ----------
     darray : DataArray
     grid: Union[Ugrid1d, Ugrid2d]
     **kwargs : optional
         Additional keyword arguments for Matplotlib.
     """
-    darray = darray.squeeze().compute()
 
     dim = darray.dims[0]
     kwargs["ax"] = ax
     if grid.topology_dimension == 1:
         if dim == grid.edge_dimension:
             return line(grid, darray, **kwargs)
         elif dim == grid.node_dimension:
@@ -630,15 +629,15 @@
         if invalid:
             raise ValueError(
                 f"UgridDataArray contains non-topology dimensions: {invalid}.\n"
                 f"Expected only one of {set(grid.dimensions.keys())}."
             )
 
         self.grid = grid
-        self.darray = darray
+        self.darray = darray.squeeze().compute()
 
     def __call__(self, **kwargs):
         return plot(self.grid, self.darray, **kwargs)
 
     @functools.wraps(contour)
     def contour(self, *args, **kwargs):
         return contour(self.grid, self.darray, *args, **kwargs)
```

### Comparing `xugrid-0.6.1/xugrid/regrid/overlap_1d.py` & `xugrid-0.6.2/xugrid/regrid/overlap_1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/regrid/reduce.py` & `xugrid-0.6.2/xugrid/regrid/reduce.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/regrid/regridder.py` & `xugrid-0.6.2/xugrid/regrid/regridder.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,16 +140,25 @@
         #   * ("time", "layer", "y", "x") -> ("stacked_time_layer", "stacked_y_x")
         #   * ("time", "layer", "face") -> ("stacked_time_layer", "face")
         #
         # Source is always 2D after this step, sized: (n_extra, size).
         source = source.reshape((-1, source_grid.size))
 
         size = self._target.size
+
         if isinstance(source, DaskArray):
-            chunks = source.chunks[: -source_grid.ndim] + (self._target.shape,)
+            # It's possible that the topology dimensions are chunked (e.g. from
+            # reading multiple partitions). The regrid operation does not
+            # support this, since we might need multiple source chunks for a
+            # single target chunk, which destroys the 1:1 relation between
+            # chunks. Here we ensure that the topology dimensions are contained
+            # in a single contiguous chunk.
+            contiguous_chunks = (source.chunks[0], (source.shape[-1],))
+            source = source.rechunk(contiguous_chunks)
+            chunks = source.chunks[:-1] + (self._target.size,)
             out = dask.array.map_blocks(
                 self._regrid,  # func
                 source,  # *args
                 self._weights,  # *args
                 size,  # *args
                 dtype=np.float64,
                 chunks=chunks,
@@ -158,15 +167,14 @@
         elif isinstance(source, np.ndarray):
             out = self._regrid(source, self._weights, size)
         else:
             raise TypeError(
                 "Expected dask.array.Array or numpy.ndarray. Received: "
                 f"{type(source).__name__}"
             )
-
         # E.g.: sizes of ("time", "layer") + ("y", "x")
         out_shape = first_dims_shape + self._target.shape
         return out.reshape(out_shape)
 
     def regrid_dataarray(self, source: xr.DataArray, source_dims: Tuple[str]):
         # Do not set vectorize=True: numba will run the for loop more
         # efficiently, and guarantees a single large allocation.
@@ -199,20 +207,15 @@
         -------
         regridded: UgridDataArray or xarray.DataArray
         """
 
         if type(self._target) is StructuredGrid2d:
             source_dims = ("y", "x")
             regridded = self.regrid_dataarray(object, source_dims)
-            regridded = regridded.assign_coords(
-                coords={
-                    "y": np.flip(self._target.ybounds.midpoints),
-                    "x": self._target.xbounds.midpoints,
-                }
-            )
+            regridded = regridded.assign_coords(coords=self._target.coords)
             return regridded
         else:
             source_dims = (object.ugrid.grid.face_dimension,)
             regridded = self.regrid_dataarray(object.ugrid.obj, source_dims)
             return UgridDataArray(
                 regridded,
                 self._target.ugrid_topology,
```

### Comparing `xugrid-0.6.1/xugrid/regrid/structured.py` & `xugrid-0.6.2/xugrid/regrid/structured.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,24 @@
             bounds = np.column_stack((start, end))
 
         self.name = name
         self.midpoints = midpoints
         self.bounds = bounds
         self.flipped = flipped
         self.side = side
-        self.grid = obj
+        self.dname = size_name
+        self.dvalue = obj[size_name].values
+        self.index = obj.indexes[name].values
+
+    @property
+    def coords(self) -> dict:
+        return {
+            self.name: self.index,
+            self.dname: self.dvalue,
+        }
 
     @property
     def ndim(self) -> int:
         return 1
 
     @property
     def dims(self) -> Tuple[str]:
@@ -86,15 +95,15 @@
 
     @property
     def size(self) -> int:
         return len(self.bounds)
 
     @property
     def length(self) -> FloatArray:
-        return abs(np.diff(self.bounds, axis=1))
+        return np.squeeze(abs(np.diff(self.bounds, axis=1)))
 
     def flip_if_needed(self, index: IntArray) -> IntArray:
         if self.flipped:
             return self.size - index - 1
         else:
             return index
 
@@ -335,15 +344,15 @@
         source_index: np.array
         target_index: np.array
         weights: np.array
             Overlapping length
         """
         source_index, target_index, weights = self.overlap_1d_structured(other)
         if relative:
-            weights /= self.length()[source_index]
+            weights /= self.length[source_index]
         return self.sorted_output(source_index, target_index, weights)
 
     def locate_centroids(
         self, other: "StructuredGrid1d"
     ) -> Tuple[IntArray, IntArray, FloatArray]:
         """
         Returns source and target indexes based on nearest neighbor of
@@ -417,14 +426,18 @@
         name_x: str,
         name_y: str,
     ):
         self.xbounds = StructuredGrid1d(obj, name_x)
         self.ybounds = StructuredGrid1d(obj, name_y)
 
     @property
+    def coords(self) -> dict:
+        return self.ybounds.coords | self.xbounds.coords
+
+    @property
     def ndim(self) -> int:
         return 2
 
     @property
     def dims(self) -> Tuple[str, str]:
         return self.ybounds.dims + self.xbounds.dims  # ("y", "x")
```

### Comparing `xugrid-0.6.1/xugrid/regrid/unstructured.py` & `xugrid-0.6.2/xugrid/regrid/unstructured.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/regrid/utils.py` & `xugrid-0.6.2/xugrid/regrid/utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/regrid/weight_matrix.py` & `xugrid-0.6.2/xugrid/regrid/weight_matrix.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/ugrid/connectivity.py` & `xugrid-0.6.2/xugrid/ugrid/connectivity.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/ugrid/conventions.py` & `xugrid-0.6.2/xugrid/ugrid/conventions.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/ugrid/interpolate.py` & `xugrid-0.6.2/xugrid/ugrid/interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/ugrid/partitioning.py` & `xugrid-0.6.2/xugrid/ugrid/partitioning.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/ugrid/snapping.py` & `xugrid-0.6.2/xugrid/ugrid/snapping.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/ugrid/ugrid1d.py` & `xugrid-0.6.2/xugrid/ugrid/ugrid1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/ugrid/ugrid2d.py` & `xugrid-0.6.2/xugrid/ugrid/ugrid2d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/ugrid/ugridbase.py` & `xugrid-0.6.2/xugrid/ugrid/ugridbase.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid/ugrid/voronoi.py` & `xugrid-0.6.2/xugrid/ugrid/voronoi.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.6.1/xugrid.egg-info/PKG-INFO` & `xugrid-0.6.2/xugrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.6.1
+Version: 0.6.2
 Summary: Xarray extension for unstructured grids
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Keywords: mesh,ugrid,unstructured grid,xarray
```

### Comparing `xugrid-0.6.1/xugrid.egg-info/SOURCES.txt` & `xugrid-0.6.2/xugrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

