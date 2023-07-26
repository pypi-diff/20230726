# Comparing `tmp/ohdsi-circe-0.2.2.tar.gz` & `tmp/ohdsi-circe-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-circe-0.2.2.tar", last modified: Fri Jul 14 10:13:52 2023, max compression
+gzip compressed data, was "ohdsi-circe-0.2.3.tar", last modified: Wed Jul 26 08:39:36 2023, max compression
```

## Comparing `ohdsi-circe-0.2.2.tar` & `ohdsi-circe-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/ohdsi/circe/
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-14 10:13:44.000000 ohdsi-circe-0.2.2/ohdsi/circe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/ohdsi/circe/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-14 10:13:44.000000 ohdsi-circe-0.2.2/ohdsi/circe/data/conceptSet.json
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-14 10:13:44.000000 ohdsi-circe-0.2.2/ohdsi/circe/data/conceptSetList.json
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-14 10:13:44.000000 ohdsi-circe-0.2.2/ohdsi/circe/data/simpleCohort.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-14 10:13:52.000000 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-14 10:13:52.000000 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:13:52.000000 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 10:13:52.000000 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 10:13:52.000000 ohdsi-circe-0.2.2/ohdsi_circe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:13:52.986669 ohdsi-circe-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-14 10:13:44.000000 ohdsi-circe-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:36.197812 ohdsi-circe-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-26 08:39:36.197812 ohdsi-circe-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:36.193812 ohdsi-circe-0.2.3/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:36.197812 ohdsi-circe-0.2.3/ohdsi/circe/
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-26 08:39:24.000000 ohdsi-circe-0.2.3/ohdsi/circe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:36.197812 ohdsi-circe-0.2.3/ohdsi/circe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-26 08:39:24.000000 ohdsi-circe-0.2.3/ohdsi/circe/data/conceptSet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-26 08:39:24.000000 ohdsi-circe-0.2.3/ohdsi/circe/data/conceptSetList.json
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-26 08:39:24.000000 ohdsi-circe-0.2.3/ohdsi/circe/data/simpleCohort.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:36.197812 ohdsi-circe-0.2.3/ohdsi_circe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-26 08:39:36.000000 ohdsi-circe-0.2.3/ohdsi_circe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 08:39:36.000000 ohdsi-circe-0.2.3/ohdsi_circe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:39:36.000000 ohdsi-circe-0.2.3/ohdsi_circe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 08:39:36.000000 ohdsi-circe-0.2.3/ohdsi_circe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 08:39:36.000000 ohdsi-circe-0.2.3/ohdsi_circe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 08:39:36.197812 ohdsi-circe-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-26 08:39:24.000000 ohdsi-circe-0.2.3/setup.py
```

### Comparing `ohdsi-circe-0.2.2/PKG-INFO` & `ohdsi-circe-0.2.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-circe
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python wrapper for the OHDSI R packages
 Home-page: https://github.com/vantage6/python-ohdsi
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # python-ohdsi
@@ -12,14 +12,21 @@
 supporting OMOP data sources in [vantage6](https://vantage6.ai).
 
 Make sure you have a working R environment with the OHDSI packages installed.
 
 # Building documentation
 ```bash
 cd docs
+export
+make html
+```
+
+```powershell
+cd docs
+Set-Item -Path Env:IGNORE_R_IMPORTS -Value True
 make html
 ```
 
 You can set the `IGNORE_R_IMPORTS` environment variable to ignore the R imports
 in the documentation. This is useful when you don't have the R packages
 installed but want to build the documentation anyway.
```

### Comparing `ohdsi-circe-0.2.2/ohdsi/circe/__init__.py` & `ohdsi-circe-0.2.3/ohdsi/circe/__init__.py`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.2/ohdsi/circe/data/conceptSet.json` & `ohdsi-circe-0.2.3/ohdsi/circe/data/conceptSet.json`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.2/ohdsi/circe/data/conceptSetList.json` & `ohdsi-circe-0.2.3/ohdsi/circe/data/conceptSetList.json`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.2/ohdsi/circe/data/simpleCohort.json` & `ohdsi-circe-0.2.3/ohdsi/circe/data/simpleCohort.json`

 * *Files identical despite different names*

### Comparing `ohdsi-circe-0.2.2/ohdsi_circe.egg-info/PKG-INFO` & `ohdsi-circe-0.2.3/ohdsi_circe.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-circe
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python wrapper for the OHDSI R packages
 Home-page: https://github.com/vantage6/python-ohdsi
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # python-ohdsi
@@ -12,14 +12,21 @@
 supporting OMOP data sources in [vantage6](https://vantage6.ai).
 
 Make sure you have a working R environment with the OHDSI packages installed.
 
 # Building documentation
 ```bash
 cd docs
+export
+make html
+```
+
+```powershell
+cd docs
+Set-Item -Path Env:IGNORE_R_IMPORTS -Value True
 make html
 ```
 
 You can set the `IGNORE_R_IMPORTS` environment variable to ignore the R imports
 in the documentation. This is useful when you don't have the R packages
 installed but want to build the documentation anyway.
```

### Comparing `ohdsi-circe-0.2.2/setup.py` & `ohdsi-circe-0.2.3/setup.py`

 * *Files identical despite different names*

