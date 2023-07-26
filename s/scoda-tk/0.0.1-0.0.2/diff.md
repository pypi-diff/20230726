# Comparing `tmp/scoda-tk-0.0.1.tar.gz` & `tmp/scoda-tk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.0.1.tar", last modified: Wed Jul 26 15:39:28 2023, max compression
+gzip compressed data, was "scoda-tk-0.0.2.tar", last modified: Wed Jul 26 15:53:33 2023, max compression
```

## Comparing `scoda-tk-0.0.1.tar` & `scoda-tk-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:39:28.107091 scoda-tk-0.0.1/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       88 2023-07-26 15:22:27.000000 scoda-tk-0.0.1/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-26 15:39:28.107091 scoda-tk-0.0.1/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-26 15:39:07.000000 scoda-tk-0.0.1/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-26 15:39:28.107091 scoda-tk-0.0.1/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:39:28.039093 scoda-tk-0.0.1/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:39:28.043093 scoda-tk-0.0.1/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:39:28.091092 scoda-tk-0.0.1/src/scoda/data/
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/src/scoda/data/GTmap_hg19.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/src/scoda/data/GTmap_hg38.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-26 05:52:26.000000 scoda-tk-0.0.1/src/scoda/data/GTmap_mm10.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    14789 2023-07-26 15:27:40.000000 scoda-tk-0.0.1/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/src/scoda/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157772 2023-07-26 15:28:30.000000 scoda-tk-0.0.1/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36606 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-26 05:52:25.000000 scoda-tk-0.0.1/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    51389 2023-07-26 15:29:52.000000 scoda-tk-0.0.1/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:39:28.107091 scoda-tk-0.0.1/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-26 15:39:28.000000 scoda-tk-0.0.1/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      527 2023-07-26 15:39:28.000000 scoda-tk-0.0.1/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-26 15:39:28.000000 scoda-tk-0.0.1/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-26 15:39:28.000000 scoda-tk-0.0.1/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-26 15:39:28.000000 scoda-tk-0.0.1/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-26 15:39:28.000000 scoda-tk-0.0.1/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:53:33.684393 scoda-tk-0.0.2/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       88 2023-07-26 15:22:27.000000 scoda-tk-0.0.2/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-26 15:53:33.680393 scoda-tk-0.0.2/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-26 15:53:10.000000 scoda-tk-0.0.2/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-26 15:53:33.684393 scoda-tk-0.0.2/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:53:33.616394 scoda-tk-0.0.2/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:53:33.620394 scoda-tk-0.0.2/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:53:33.668393 scoda-tk-0.0.2/src/scoda/data/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/data/GTmap_hg19.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/data/GTmap_hg38.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-26 05:52:26.000000 scoda-tk-0.0.2/src/scoda/data/GTmap_mm10.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14789 2023-07-26 15:27:40.000000 scoda-tk-0.0.2/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157772 2023-07-26 15:28:30.000000 scoda-tk-0.0.2/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36606 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    51404 2023-07-26 15:52:58.000000 scoda-tk-0.0.2/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:53:33.680393 scoda-tk-0.0.2/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      527 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.0.1/LICENSE` & `scoda-tk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/PKG-INFO` & `scoda-tk-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.0.1/pyproject.toml` & `scoda-tk-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.0.1"
+version = "0.0.2"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.0.1/src/scoda/cpdb.py` & `scoda-tk-0.0.2/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/src/scoda/data/GTmap_hg19.csv` & `scoda-tk-0.0.2/src/scoda/data/GTmap_hg19.csv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/src/scoda/data/GTmap_hg38.csv` & `scoda-tk-0.0.2/src/scoda/data/GTmap_hg38.csv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/src/scoda/data/GTmap_mm10.csv` & `scoda-tk-0.0.2/src/scoda/data/GTmap_mm10.csv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/src/scoda/deg.py` & `scoda-tk-0.0.2/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/src/scoda/deiso.py` & `scoda-tk-0.0.2/src/scoda/deiso.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/src/scoda/gsea.py` & `scoda-tk-0.0.2/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/src/scoda/hicat.py` & `scoda-tk-0.0.2/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/src/scoda/icnv.py` & `scoda-tk-0.0.2/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/src/scoda/misc.py` & `scoda-tk-0.0.2/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.1/src/scoda/viz.py` & `scoda-tk-0.0.2/src/scoda/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import time, os, copy, datetime, math, random, warnings
+import anndata
 import numpy as np
 import pandas as pd
 from scipy import stats
 import seaborn as sns
 from statannot import add_stat_annotation
 import matplotlib.pyplot as plt
 from matplotlib import cm, colormaps
```

### Comparing `scoda-tk-0.0.1/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.0.2/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.0.1
+Version: 0.0.2
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.0.1/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.0.2/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

