# Comparing `tmp/open-buildings-0.0.5.tar.gz` & `tmp/open-buildings-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-buildings-0.0.5.tar", last modified: Wed Jul 26 02:49:24 2023, max compression
+gzip compressed data, was "open-buildings-0.0.6.tar", last modified: Wed Jul 26 03:00:04 2023, max compression
```

## Comparing `open-buildings-0.0.5.tar` & `open-buildings-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:49:24.890689 open-buildings-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-26 02:49:06.000000 open-buildings-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-26 02:49:06.000000 open-buildings-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 02:49:24.890689 open-buildings-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-07-26 02:49:06.000000 open-buildings-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:49:24.890689 open-buildings-0.0.5/open_buildings/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-26 02:49:06.000000 open-buildings-0.0.5/open_buildings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-26 02:49:06.000000 open-buildings-0.0.5/open_buildings/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-26 02:49:06.000000 open-buildings-0.0.5/open_buildings/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-07-26 02:49:06.000000 open-buildings-0.0.5/open_buildings/open_buildings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:49:24.890689 open-buildings-0.0.5/open_buildings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 02:49:06.000000 open-buildings-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-26 02:49:24.890689 open-buildings-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-26 02:49:06.000000 open-buildings-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:00:04.089462 open-buildings-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-26 02:59:53.000000 open-buildings-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-26 02:59:53.000000 open-buildings-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 03:00:04.089462 open-buildings-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-07-26 02:59:53.000000 open-buildings-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:00:04.089462 open-buildings-0.0.6/open_buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 02:59:53.000000 open-buildings-0.0.6/open_buildings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-26 02:59:53.000000 open-buildings-0.0.6/open_buildings/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-26 02:59:53.000000 open-buildings-0.0.6/open_buildings/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16781 2023-07-26 02:59:53.000000 open-buildings-0.0.6/open_buildings/open_buildings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:00:04.089462 open-buildings-0.0.6/open_buildings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 03:00:04.000000 open-buildings-0.0.6/open_buildings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 02:59:53.000000 open-buildings-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-26 03:00:04.089462 open-buildings-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-26 02:59:53.000000 open-buildings-0.0.6/setup.py
```

### Comparing `open-buildings-0.0.5/LICENSE` & `open-buildings-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `open-buildings-0.0.5/PKG-INFO` & `open-buildings-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-buildings
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tools for working with open building datasets
 Home-page: https://github.com/opengeos/open-buildings
 Author: Chris Holmes
 Author-email: homie@gmail.com
 License: Apache Software License 2.0
 Keywords: open_buildings
 Classifier: Intended Audience :: Developers
```

### Comparing `open-buildings-0.0.5/README.md` & `open-buildings-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `open-buildings-0.0.5/open_buildings/cli.py` & `open-buildings-0.0.6/open_buildings/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """CLI to convert Google Open Building CSV files to alternate formats."""
 import sys
 import click
+import pandas as pd
 from open_buildings import process_benchmark, process_geometries
+from tabulate import tabulate
 
 
 @click.group()
 def main():
     """CLI to convert Google Open Building CSV files to alternate formats."""
     pass
```

### Comparing `open-buildings-0.0.5/open_buildings/open_buildings.py` & `open-buildings-0.0.6/open_buildings/open_buildings.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 import glob
 import duckdb
 import pandas as pd
 import geopandas as gpd
 from shapely import wkt
 from shapely.geometry import mapping
 from openlocationcode import openlocationcode as olc
-from tabulate import tabulate
 
 # Global variable, that runs GPQ (https://github.com/planetlabs/gpq) after DuckDB writes the Parquet file.
 # This is necessary because DuckDB does not write the GeoParquet metadata (yet). Once DuckDB implements
 # this feature can be removed. Setting it to false will give a sense of how fast DuckDB will be, but
 # if you want to actually use the output GeoParquet files, set it to True.
 RUN_GPQ_CONVERSION = False
```

### Comparing `open-buildings-0.0.5/open_buildings.egg-info/PKG-INFO` & `open-buildings-0.0.6/open_buildings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-buildings
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tools for working with open building datasets
 Home-page: https://github.com/opengeos/open-buildings
 Author: Chris Holmes
 Author-email: homie@gmail.com
 License: Apache Software License 2.0
 Keywords: open_buildings
 Classifier: Intended Audience :: Developers
```

### Comparing `open-buildings-0.0.5/setup.py` & `open-buildings-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords='open_buildings',
     name='open-buildings',
     packages=find_packages(include=['open_buildings', 'open_buildings.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/open-buildings',
-    version='0.0.5',
+    version='0.0.6',
     zip_safe=False,
 )
```

