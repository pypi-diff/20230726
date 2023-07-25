# Comparing `tmp/tecton_utils-0.0.1.tar.gz` & `tmp/tecton_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecton_utils-0.0.1.tar", last modified: Mon Jul 24 18:13:48 2023, max compression
+gzip compressed data, was "tecton_utils-0.0.2.tar", last modified: Tue Jul 25 22:30:01 2023, max compression
```

## Comparing `tecton_utils-0.0.1.tar` & `tecton_utils-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-24 18:13:48.423842 tecton_utils-0.0.1/
--rw-r--r--   0 alex       (501) staff       (20)      195 2023-07-24 18:13:48.423735 tecton_utils-0.0.1/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)       44 2023-07-24 18:06:17.000000 tecton_utils-0.0.1/README.md
--rw-r--r--   0 alex       (501) staff       (20)       38 2023-07-24 18:13:48.423872 tecton_utils-0.0.1/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      496 2023-07-24 18:06:45.000000 tecton_utils-0.0.1/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-24 18:13:48.423078 tecton_utils-0.0.1/tecton_utils/
--rw-r--r--   0 alex       (501) staff       (20)       63 2023-07-22 02:17:40.000000 tecton_utils-0.0.1/tecton_utils/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4250 2023-07-22 01:51:33.000000 tecton_utils-0.0.1/tecton_utils/utils.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-24 18:13:48.423611 tecton_utils-0.0.1/tecton_utils.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)      195 2023-07-24 18:13:48.000000 tecton_utils-0.0.1/tecton_utils.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      244 2023-07-24 18:13:48.000000 tecton_utils-0.0.1/tecton_utils.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-24 18:13:48.000000 tecton_utils-0.0.1/tecton_utils.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       15 2023-07-24 18:13:48.000000 tecton_utils-0.0.1/tecton_utils.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       13 2023-07-24 18:13:48.000000 tecton_utils-0.0.1/tecton_utils.egg-info/top_level.txt
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-25 22:30:01.331562 tecton_utils-0.0.2/
+-rw-r--r--   0 alex       (501) staff       (20)      195 2023-07-25 22:30:01.331446 tecton_utils-0.0.2/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)       44 2023-07-24 18:06:17.000000 tecton_utils-0.0.2/README.md
+-rw-r--r--   0 alex       (501) staff       (20)       38 2023-07-25 22:30:01.331604 tecton_utils-0.0.2/setup.cfg
+-rw-r--r--   0 alex       (501) staff       (20)      496 2023-07-25 22:29:58.000000 tecton_utils-0.0.2/setup.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-25 22:30:01.330762 tecton_utils-0.0.2/tecton_utils/
+-rw-r--r--   0 alex       (501) staff       (20)       63 2023-07-22 02:17:40.000000 tecton_utils-0.0.2/tecton_utils/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     4328 2023-07-25 22:29:44.000000 tecton_utils-0.0.2/tecton_utils/utils.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-07-25 22:30:01.331310 tecton_utils-0.0.2/tecton_utils.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)      195 2023-07-25 22:30:01.000000 tecton_utils-0.0.2/tecton_utils.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      244 2023-07-25 22:30:01.000000 tecton_utils-0.0.2/tecton_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-07-25 22:30:01.000000 tecton_utils-0.0.2/tecton_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       15 2023-07-25 22:30:01.000000 tecton_utils-0.0.2/tecton_utils.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)       13 2023-07-25 22:30:01.000000 tecton_utils-0.0.2/tecton_utils.egg-info/top_level.txt
```

### Comparing `tecton_utils-0.0.1/tecton_utils/utils.py` & `tecton_utils-0.0.2/tecton_utils/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from datetime import timedelta
 from typing import Optional
 from typing import Union
 
+import logging
+
 import pyspark
 from pyspark.sql import SparkSession
 from pyspark.sql import functions as F
 from pyspark.sql.utils import AnalysisException
 
 import tecton
 
+logger = logging.getLogger(__name__)
+
 
 def _get_partitions(output_path, partition_col):
     try:
         spark = SparkSession.getActiveSession()
         df = spark.read.parquet(output_path)
     except AnalysisException as e:
         if "Path does not exist" in str(e):
@@ -63,38 +67,38 @@
     ]
     min_ds = row["min_ts"].date()
     max_ds = row["max_ts"].date() + timedelta(days=1)
     total_days = (max_ds - min_ds).days
 
     existing_partitions = _get_partitions(output_path, partition_col)
 
-    print(f"{len(existing_partitions)} existing partitions found: {_format_partition_list(existing_partitions)}")
+    logger.info(f"{len(existing_partitions)} existing partitions found: {_format_partition_list(existing_partitions)}")
 
     partitions_to_compute = []
 
     for i in range(total_days):
         ds = min_ds + timedelta(days=i)
         if ds not in existing_partitions:
             partitions_to_compute.append(ds)
 
     partitions_to_compute = sorted(partitions_to_compute)
 
-    print(
+    logger.info(
         f"Computing the following {len(partitions_to_compute)} partitions: {_format_partition_list(partitions_to_compute)}"
     )
 
     splits = _chunkify(partitions_to_compute, split_size_days)
 
     for partition_list in splits:
-        print(f"Starting GHF computation for partitions {_format_partition_list(partition_list)}")
+        logger.info(f"Starting GHF computation for partitions {_format_partition_list(partition_list)}")
         filtered_spine = spine.filter(F.to_date(F.col(timestamp_key)).isin(partition_list))
         ghf_result = fv_or_fs.get_historical_features(
             spine=filtered_spine, timestamp_key=timestamp_key, **get_historical_features_kwargs
         ).to_spark()
         if repartition:
             ghf_result = ghf_result.repartition(repartition)
         ghf_result = ghf_result.withColumn(partition_col, F.expr(f"to_date({timestamp_key})"))
         ghf_result.write.option("partitionOverwriteMode", "dynamic").partitionBy(partition_col).parquet(
             output_path, mode="overwrite"
         )
-        print(f"GHF result saved for partitions {_format_partition_list(partition_list)}")
+        logger.info(f"GHF result saved for partitions {_format_partition_list(partition_list)}")
     return spark.read.parquet(output_path)
```

