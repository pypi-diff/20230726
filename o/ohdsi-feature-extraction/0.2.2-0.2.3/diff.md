# Comparing `tmp/ohdsi-feature-extraction-0.2.2.tar.gz` & `tmp/ohdsi-feature-extraction-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohdsi-feature-extraction-0.2.2.tar", last modified: Fri Jul 14 10:13:54 2023, max compression
+gzip compressed data, was "ohdsi-feature-extraction-0.2.3.tar", last modified: Wed Jul 26 08:39:38 2023, max compression
```

## Comparing `ohdsi-feature-extraction-0.2.2.tar` & `ohdsi-feature-extraction-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.714696 ohdsi-feature-extraction-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-14 10:13:54.714696 ohdsi-feature-extraction-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.710695 ohdsi-feature-extraction-0.2.2/ohdsi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.714696 ohdsi-feature-extraction-0.2.2/ohdsi/feature_extraction/
--rw-r--r--   0 runner    (1001) docker     (123)    59977 2023-07-14 10:13:44.000000 ohdsi-feature-extraction-0.2.2/ohdsi/feature_extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:13:54.714696 ohdsi-feature-extraction-0.2.2/ohdsi_feature_extraction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-14 10:13:54.000000 ohdsi-feature-extraction-0.2.2/ohdsi_feature_extraction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 10:13:54.000000 ohdsi-feature-extraction-0.2.2/ohdsi_feature_extraction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:13:54.000000 ohdsi-feature-extraction-0.2.2/ohdsi_feature_extraction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 10:13:54.000000 ohdsi-feature-extraction-0.2.2/ohdsi_feature_extraction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 10:13:54.000000 ohdsi-feature-extraction-0.2.2/ohdsi_feature_extraction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:13:54.714696 ohdsi-feature-extraction-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-14 10:13:44.000000 ohdsi-feature-extraction-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:38.033851 ohdsi-feature-extraction-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-26 08:39:38.033851 ohdsi-feature-extraction-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:38.033851 ohdsi-feature-extraction-0.2.3/ohdsi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:38.033851 ohdsi-feature-extraction-0.2.3/ohdsi/feature_extraction/
+-rw-r--r--   0 runner    (1001) docker     (123)    60176 2023-07-26 08:39:24.000000 ohdsi-feature-extraction-0.2.3/ohdsi/feature_extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 08:39:38.033851 ohdsi-feature-extraction-0.2.3/ohdsi_feature_extraction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-26 08:39:37.000000 ohdsi-feature-extraction-0.2.3/ohdsi_feature_extraction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-26 08:39:38.000000 ohdsi-feature-extraction-0.2.3/ohdsi_feature_extraction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 08:39:37.000000 ohdsi-feature-extraction-0.2.3/ohdsi_feature_extraction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 08:39:37.000000 ohdsi-feature-extraction-0.2.3/ohdsi_feature_extraction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 08:39:37.000000 ohdsi-feature-extraction-0.2.3/ohdsi_feature_extraction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 08:39:38.033851 ohdsi-feature-extraction-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-26 08:39:24.000000 ohdsi-feature-extraction-0.2.3/setup.py
```

### Comparing `ohdsi-feature-extraction-0.2.2/PKG-INFO` & `ohdsi-feature-extraction-0.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-feature-extraction
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

### Comparing `ohdsi-feature-extraction-0.2.2/ohdsi/feature_extraction/__init__.py` & `ohdsi-feature-extraction-0.2.3/ohdsi/feature_extraction/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import json
 
 from rpy2 import robjects
 from rpy2.robjects.methods import RS4
 from rpy2.robjects.vectors import ListVector
 
 from rpy2.robjects.packages import importr
 
@@ -784,18 +785,19 @@
         ...     included_covariate_concept_ids = [],
         ...     add_descendants_to_include = False,
         ...     excluded_covariate_concept_ids = [],
         ...     add_descendants_to_exclude = False,
         ...     included_covariate_ids = []
         ... )
         """
+        parameters_json = json.dumps(parameters)
         return extractor_r.createAnalysisDetails(
             analysis_id,
             sql_file_name,
-            parameters,
+            parameters_json,
             included_covariate_concept_ids,
             add_descendants_to_include,
             excluded_covariate_concept_ids,
             add_descendants_to_exclude,
             included_covariate_ids
         )
 
@@ -936,15 +938,15 @@
             temporal_end_days
         )
 
 
 class DefaultTemporalCovariateSettings:
 
     @staticmethod
-    def createTemporalCovariateSettings(
+    def create_temporal_covariate_settings(
         use_demographics_gender: bool = False,
         use_demographics_age: bool = False,
         use_demographics_age_group: bool = False,
         use_demographics_race: bool = False,
         use_demographics_ethnicity: bool = False,
         use_demographics_index_year: bool = False,
         use_demographics_index_month: bool = False,
@@ -1150,14 +1152,18 @@
         Examples
         --------
         >>> settings = create_temporal_covariate_settings(
         ...     use_demographics_gender=True,
         ...     use_demographics_age=True,
         ... )
         """
+
+        temporal_start_days_list = list(temporal_start_days)
+        temporal_end_days_list = list(temporal_end_days)
+
         return extractor_r.createTemporalCovariateSettings(
             use_demographics_gender,
             use_demographics_age,
             use_demographics_age_group,
             use_demographics_race,
             use_demographics_ethnicity,
             use_demographics_index_year,
@@ -1192,16 +1198,16 @@
             use_distinct_condition_count,
             use_distinct_ingredient_count,
             use_distinct_procedure_count,
             use_distinct_measurement_count,
             use_distinct_observation_count,
             use_visit_count,
             use_visit_concept_count,
-            temporal_start_days,
-            temporal_end_days,
+            temporal_start_days_list,
+            temporal_end_days_list,
             included_covariate_concept_ids,
             add_descendants_to_include,
             excluded_covariate_concept_ids,
             add_descendants_to_exclude,
             included_covariate_ids
         )
```

### Comparing `ohdsi-feature-extraction-0.2.2/ohdsi_feature_extraction.egg-info/PKG-INFO` & `ohdsi-feature-extraction-0.2.3/ohdsi_feature_extraction.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohdsi-feature-extraction
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

### Comparing `ohdsi-feature-extraction-0.2.2/setup.py` & `ohdsi-feature-extraction-0.2.3/setup.py`

 * *Files identical despite different names*

