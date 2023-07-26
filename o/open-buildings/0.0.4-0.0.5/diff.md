# Comparing `tmp/open-buildings-0.0.4.tar.gz` & `tmp/open-buildings-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-buildings-0.0.4.tar", last modified: Tue Jul 25 16:23:12 2023, max compression
+gzip compressed data, was "open-buildings-0.0.5.tar", last modified: Wed Jul 26 02:49:24 2023, max compression
```

## Comparing `open-buildings-0.0.4.tar` & `open-buildings-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:23:12.807983 open-buildings-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-25 16:22:55.000000 open-buildings-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 16:22:55.000000 open-buildings-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-25 16:23:12.807983 open-buildings-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-07-25 16:22:55.000000 open-buildings-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:23:12.807983 open-buildings-0.0.4/open_buildings/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-25 16:22:55.000000 open-buildings-0.0.4/open_buildings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-25 16:22:55.000000 open-buildings-0.0.4/open_buildings/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 16:22:55.000000 open-buildings-0.0.4/open_buildings/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-07-25 16:22:55.000000 open-buildings-0.0.4/open_buildings/open_buildings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:23:12.807983 open-buildings-0.0.4/open_buildings.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 16:23:12.000000 open-buildings-0.0.4/open_buildings.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 16:22:55.000000 open-buildings-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-25 16:23:12.807983 open-buildings-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-25 16:22:55.000000 open-buildings-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:49:24.890689 open-buildings-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-26 02:49:06.000000 open-buildings-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-26 02:49:06.000000 open-buildings-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 02:49:24.890689 open-buildings-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-07-26 02:49:06.000000 open-buildings-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:49:24.890689 open-buildings-0.0.5/open_buildings/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-26 02:49:06.000000 open-buildings-0.0.5/open_buildings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-26 02:49:06.000000 open-buildings-0.0.5/open_buildings/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-26 02:49:06.000000 open-buildings-0.0.5/open_buildings/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-07-26 02:49:06.000000 open-buildings-0.0.5/open_buildings/open_buildings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:49:24.890689 open-buildings-0.0.5/open_buildings.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 02:49:24.000000 open-buildings-0.0.5/open_buildings.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-26 02:49:06.000000 open-buildings-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-26 02:49:24.890689 open-buildings-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-26 02:49:06.000000 open-buildings-0.0.5/setup.py
```

### Comparing `open-buildings-0.0.4/LICENSE` & `open-buildings-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `open-buildings-0.0.4/PKG-INFO` & `open-buildings-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-buildings
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools for working with open building datasets
 Home-page: https://github.com/opengeos/open-buildings
 Author: Chris Holmes
 Author-email: homie@gmail.com
 License: Apache Software License 2.0
 Keywords: open_buildings
 Classifier: Intended Audience :: Developers
```

### Comparing `open-buildings-0.0.4/README.md` & `open-buildings-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `open-buildings-0.0.4/open_buildings/cli.py` & `open-buildings-0.0.5/open_buildings/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """CLI to convert Google Open Building CSV files to alternate formats."""
 import sys
 import click
+from open_buildings import process_benchmark, process_geometries
 
 
 @click.group()
 def main():
     """CLI to convert Google Open Building CSV files to alternate formats."""
     pass
```

### Comparing `open-buildings-0.0.4/open_buildings/open_buildings.py` & `open-buildings-0.0.5/open_buildings/open_buildings.py`

 * *Files identical despite different names*

### Comparing `open-buildings-0.0.4/open_buildings.egg-info/PKG-INFO` & `open-buildings-0.0.5/open_buildings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-buildings
-Version: 0.0.4
+Version: 0.0.5
 Summary: Tools for working with open building datasets
 Home-page: https://github.com/opengeos/open-buildings
 Author: Chris Holmes
 Author-email: homie@gmail.com
 License: Apache Software License 2.0
 Keywords: open_buildings
 Classifier: Intended Audience :: Developers
```

### Comparing `open-buildings-0.0.4/setup.py` & `open-buildings-0.0.5/setup.py`

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
-    version='0.0.4',
+    version='0.0.5',
     zip_safe=False,
 )
```

