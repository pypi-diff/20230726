# Comparing `tmp/cohort-generator-0.2.2.tar.gz` & `tmp/cohort-generator-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohort-generator-0.2.2.tar", last modified: Fri Jul 14 10:13:53 2023, max compression
+gzip compressed data, was "cohort-generator-0.2.3.tar", last modified: Wed Jul 26 08:39:36 2023, max compression
```

## Comparing `cohort-generator-0.2.2.tar` & `cohort-generator-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/cohort_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-14 10:13:53.000000 cohort-generator-0.2.2/cohort_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-14 10:13:53.000000 cohort-generator-0.2.2/cohort_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:13:53.000000 cohort-generator-0.2.2/cohort_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 10:13:53.000000 cohort-generator-0.2.2/cohort_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 10:13:53.000000 cohort-generator-0.2.2/cohort_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/ohdsi/cohort_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-14 10:13:44.000000 cohort-generator-0.2.2/ohdsi/cohort_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-14 10:13:44.000000 cohort-generator-0.2.2/ohdsi/cohort_generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:13:53.442675 cohort-generator-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-14 10:13:44.000000 cohort-generator-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:36.773823 cohort-generator-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-26 08:39:36.773823 cohort-generator-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:36.773823 cohort-generator-0.2.3/cohort_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-26 08:39:36.000000 cohort-generator-0.2.3/cohort_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-26 08:39:36.000000 cohort-generator-0.2.3/cohort_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:39:36.000000 cohort-generator-0.2.3/cohort_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 08:39:36.000000 cohort-generator-0.2.3/cohort_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 08:39:36.000000 cohort-generator-0.2.3/cohort_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:36.769822 cohort-generator-0.2.3/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:36.773823 cohort-generator-0.2.3/ohdsi/cohort_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     9835 2023-07-26 08:39:24.000000 cohort-generator-0.2.3/ohdsi/cohort_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-07-26 08:39:24.000000 cohort-generator-0.2.3/ohdsi/cohort_generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 08:39:36.773823 cohort-generator-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-26 08:39:24.000000 cohort-generator-0.2.3/setup.py
```

### Comparing `cohort-generator-0.2.2/PKG-INFO` & `cohort-generator-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohort-generator
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

### Comparing `cohort-generator-0.2.2/cohort_generator.egg-info/PKG-INFO` & `cohort-generator-0.2.3/cohort_generator.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cohort-generator
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

### Comparing `cohort-generator-0.2.2/ohdsi/cohort_generator/__init__.py` & `cohort-generator-0.2.3/ohdsi/cohort_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `cohort-generator-0.2.2/ohdsi/cohort_generator/main.py` & `cohort-generator-0.2.3/ohdsi/cohort_generator/main.py`

 * *Files identical despite different names*

### Comparing `cohort-generator-0.2.2/setup.py` & `cohort-generator-0.2.3/setup.py`

 * *Files identical despite different names*

