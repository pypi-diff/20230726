# Comparing `tmp/scoda-tk-0.0.2.tar.gz` & `tmp/scoda-tk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-tk-0.0.2.tar", last modified: Wed Jul 26 15:53:33 2023, max compression
+gzip compressed data, was "scoda-tk-0.0.3.tar", last modified: Wed Jul 26 16:00:01 2023, max compression
```

## Comparing `scoda-tk-0.0.2.tar` & `scoda-tk-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:53:33.684393 scoda-tk-0.0.2/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/LICENSE
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       88 2023-07-26 15:22:27.000000 scoda-tk-0.0.2/MANIFEST.in
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-26 15:53:33.680393 scoda-tk-0.0.2/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/README.md
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-26 15:53:10.000000 scoda-tk-0.0.2/pyproject.toml
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-26 15:53:33.684393 scoda-tk-0.0.2/setup.cfg
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/setup.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:53:33.616394 scoda-tk-0.0.2/src/
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:53:33.620394 scoda-tk-0.0.2/src/scoda/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/__init__.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/cpdb.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:53:33.668393 scoda-tk-0.0.2/src/scoda/data/
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/data/GTmap_hg19.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/data/GTmap_hg38.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-26 05:52:26.000000 scoda-tk-0.0.2/src/scoda/data/GTmap_mm10.csv
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    14789 2023-07-26 15:27:40.000000 scoda-tk-0.0.2/src/scoda/deg.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/deiso.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/gsea.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)   157772 2023-07-26 15:28:30.000000 scoda-tk-0.0.2/src/scoda/hicat.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    36606 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/icnv.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-26 05:52:25.000000 scoda-tk-0.0.2/src/scoda/misc.py
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    51404 2023-07-26 15:52:58.000000 scoda-tk-0.0.2/src/scoda/viz.py
-drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 15:53:33.680393 scoda-tk-0.0.2/src/scoda_tk.egg-info/
--rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/PKG-INFO
--rw-rw-r--   0 syoon     (1001) syoon     (1001)      527 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/SOURCES.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/dependency_links.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/entry_points.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/requires.txt
--rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-26 15:53:33.000000 scoda-tk-0.0.2/src/scoda_tk.egg-info/top_level.txt
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 16:00:01.355520 scoda-tk-0.0.3/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    35821 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/LICENSE
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       88 2023-07-26 15:22:27.000000 scoda-tk-0.0.3/MANIFEST.in
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-26 16:00:01.355520 scoda-tk-0.0.3/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      175 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/README.md
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      826 2023-07-26 15:59:34.000000 scoda-tk-0.0.3/pyproject.toml
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       38 2023-07-26 16:00:01.355520 scoda-tk-0.0.3/setup.cfg
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       49 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/setup.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 16:00:01.287522 scoda-tk-0.0.3/src/
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 16:00:01.291522 scoda-tk-0.0.3/src/scoda/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      163 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/src/scoda/__init__.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    21388 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/src/scoda/cpdb.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 16:00:01.339521 scoda-tk-0.0.3/src/scoda/data/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 20978082 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/src/scoda/data/GTmap_hg19.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 22541574 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/src/scoda/data/GTmap_hg38.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001) 11979098 2023-07-26 05:52:26.000000 scoda-tk-0.0.3/src/scoda/data/GTmap_mm10.csv
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    14789 2023-07-26 15:27:40.000000 scoda-tk-0.0.3/src/scoda/deg.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)     6033 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/src/scoda/deiso.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    12716 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/src/scoda/gsea.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)   157772 2023-07-26 15:28:30.000000 scoda-tk-0.0.3/src/scoda/hicat.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    36606 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/src/scoda/icnv.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    30776 2023-07-26 05:52:25.000000 scoda-tk-0.0.3/src/scoda/misc.py
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    51402 2023-07-26 15:59:22.000000 scoda-tk-0.0.3/src/scoda/viz.py
+drwxrwxr-x   0 syoon     (1001) syoon     (1001)        0 2023-07-26 16:00:01.351520 scoda-tk-0.0.3/src/scoda_tk.egg-info/
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)    41230 2023-07-26 16:00:01.000000 scoda-tk-0.0.3/src/scoda_tk.egg-info/PKG-INFO
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)      527 2023-07-26 16:00:01.000000 scoda-tk-0.0.3/src/scoda_tk.egg-info/SOURCES.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        1 2023-07-26 16:00:01.000000 scoda-tk-0.0.3/src/scoda_tk.egg-info/dependency_links.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       52 2023-07-26 16:00:01.000000 scoda-tk-0.0.3/src/scoda_tk.egg-info/entry_points.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)       54 2023-07-26 16:00:01.000000 scoda-tk-0.0.3/src/scoda_tk.egg-info/requires.txt
+-rw-rw-r--   0 syoon     (1001) syoon     (1001)        6 2023-07-26 16:00:01.000000 scoda-tk-0.0.3/src/scoda_tk.egg-info/top_level.txt
```

### Comparing `scoda-tk-0.0.2/LICENSE` & `scoda-tk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/PKG-INFO` & `scoda-tk-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.0.2/pyproject.toml` & `scoda-tk-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scoda-tk"
-version = "0.0.2"
+version = "0.0.3"
 description = "Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)"
 readme = "README.md"
 authors = [{ name = "Seokhyun Yoon", email = "syoon@dku.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `scoda-tk-0.0.2/src/scoda/cpdb.py` & `scoda-tk-0.0.3/src/scoda/cpdb.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/src/scoda/data/GTmap_hg19.csv` & `scoda-tk-0.0.3/src/scoda/data/GTmap_hg19.csv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/src/scoda/data/GTmap_hg38.csv` & `scoda-tk-0.0.3/src/scoda/data/GTmap_hg38.csv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/src/scoda/data/GTmap_mm10.csv` & `scoda-tk-0.0.3/src/scoda/data/GTmap_mm10.csv`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/src/scoda/deg.py` & `scoda-tk-0.0.3/src/scoda/deg.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/src/scoda/deiso.py` & `scoda-tk-0.0.3/src/scoda/deiso.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/src/scoda/gsea.py` & `scoda-tk-0.0.3/src/scoda/gsea.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/src/scoda/hicat.py` & `scoda-tk-0.0.3/src/scoda/hicat.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/src/scoda/icnv.py` & `scoda-tk-0.0.3/src/scoda/icnv.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/src/scoda/misc.py` & `scoda-tk-0.0.3/src/scoda/misc.py`

 * *Files identical despite different names*

### Comparing `scoda-tk-0.0.2/src/scoda/viz.py` & `scoda-tk-0.0.3/src/scoda/viz.py`

 * *Files 0% similar despite different names*

```diff
@@ -829,15 +829,15 @@
 
     ## Create AnnData for plot
     ad = anndata.AnnData(X = X_cnv, var = df_chr, obs = adata.obs)
 
     cond_col = 'condition'
     clst = ad.obs[cond_col].unique()
     ad.obs['tumor_dec_rev'] = ad.obs['celltype_major'].copy(deep = True).astype(str)
-    b = ad.obs['tumor_dec_rev'].isin(adata_t.uns['Ref_celltypes_for_cnv'])
+    b = ad.obs['tumor_dec_rev'].isin(adata.uns['Ref_celltypes_for_cnv'])
     ad.obs.loc[b, 'tumor_dec_rev'] = 'Normal ref'
     for c in clst:
         b = (ad.obs[cond_col] == c) & (ad.obs['tumor_dec'] == 'Tumor')
         s = 'Tumor %s' % c
         ad.obs.loc[b, 'tumor_dec_rev'] = s
 
     X = np.abs(ad.to_df())
```

### Comparing `scoda-tk-0.0.2/src/scoda_tk.egg-info/PKG-INFO` & `scoda-tk-0.0.3/src/scoda_tk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda-tk
-Version: 0.0.2
+Version: 0.0.3
 Summary: Toolkits for single-cell omics data analysis. (including wrapper functions for CellPhoneDB, GSEApy and InferCNVpy)
 Author-email: Seokhyun Yoon <syoon@dku.edu>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `scoda-tk-0.0.2/src/scoda_tk.egg-info/SOURCES.txt` & `scoda-tk-0.0.3/src/scoda_tk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

