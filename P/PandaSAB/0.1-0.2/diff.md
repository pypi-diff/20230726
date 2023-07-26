# Comparing `tmp/PandaSAB-0.1.tar.gz` & `tmp/PandaSAB-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandaSAB-0.1.tar", last modified: Wed Jul 26 16:59:18 2023, max compression
+gzip compressed data, was "PandaSAB-0.2.tar", last modified: Wed Jul 26 17:03:56 2023, max compression
```

## Comparing `PandaSAB-0.1.tar` & `PandaSAB-0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:59:18.043131 PandaSAB-0.1/
--rw-rw-rw-   0        0        0      904 2023-07-26 16:59:18.039601 PandaSAB-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 16:59:18.037601 PandaSAB-0.1/PandaSAB.egg-info/
--rw-rw-rw-   0        0        0      904 2023-07-26 16:59:17.000000 PandaSAB-0.1/PandaSAB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-07-26 16:59:17.000000 PandaSAB-0.1/PandaSAB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:59:17.000000 PandaSAB-0.1/PandaSAB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-26 16:59:17.000000 PandaSAB-0.1/PandaSAB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:59:17.000000 PandaSAB-0.1/PandaSAB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 16:59:18.044167 PandaSAB-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1484 2023-07-26 16:57:42.000000 PandaSAB-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:03:56.704436 PandaSAB-0.2/
+-rw-rw-rw-   0        0        0      904 2023-07-26 17:03:56.700437 PandaSAB-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 17:03:56.699437 PandaSAB-0.2/PandaSAB.egg-info/
+-rw-rw-rw-   0        0        0      904 2023-07-26 17:03:56.000000 PandaSAB-0.2/PandaSAB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-07-26 17:03:56.000000 PandaSAB-0.2/PandaSAB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:03:56.000000 PandaSAB-0.2/PandaSAB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-26 17:03:56.000000 PandaSAB-0.2/PandaSAB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:03:56.000000 PandaSAB-0.2/PandaSAB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:03:56.704436 PandaSAB-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1476 2023-07-26 17:03:31.000000 PandaSAB-0.2/setup.py
```

### Comparing `PandaSAB-0.1/PKG-INFO` & `PandaSAB-0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PandaSAB
-Version: 0.1
+Version: 0.2
 Summary: Pandas based Spatial Agent Based model (PandaSAB)
 Author: Yahya Gamal
 Author-email: <sable.yg@outlook.com>
 Keywords: python,Agent Based Model,Spatial,Pandas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
```

### Comparing `PandaSAB-0.1/PandaSAB.egg-info/PKG-INFO` & `PandaSAB-0.2/PandaSAB.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PandaSAB
-Version: 0.1
+Version: 0.2
 Summary: Pandas based Spatial Agent Based model (PandaSAB)
 Author: Yahya Gamal
 Author-email: <sable.yg@outlook.com>
 Keywords: python,Agent Based Model,Spatial,Pandas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 2
```

### Comparing `PandaSAB-0.1/setup.py` & `PandaSAB-0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1' 
+VERSION = '0.2' 
 DESCRIPTION = 'Pandas based Spatial Agent Based model (PandaSAB)'
 LONG_DESCRIPTION = 'An Agent Based Modelling (ABM) package that can generate grid spatial shape files or work with predefined shape files.\nThe package focuses on simplicity by assigning Agents to spatial Polygons instead of assigning x and y locations for each agents.\nThis makes it useful in situations where granual movement of agents in space is not necessary (e.g. residentail location models)'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="PandaSAB", 
         version=VERSION,
         author="Yahya Gamal",
         author_email="<sable.yg@outlook.com>",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
-        install_requires=['geopandas', 'pandas', 'fiona', 'copy', 'pyshp'], # add any additional packages that 
+        install_requires=['geopandas', 'pandas', 'fiona', 'pyshp'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
         keywords=['python', 'Agent Based Model', 'Spatial', 'Pandas'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Science/Research",
             "Programming Language :: Python :: 2",
```

