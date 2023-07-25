# Comparing `tmp/metabengine-0.0.5.tar.gz` & `tmp/metabengine-0.0.6.tar.gz`

## Comparing `metabengine-0.0.5.tar` & `metabengine-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/__init__.py
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/alignment.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/ann_feat_quality.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/calculate_mass.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/feat_extract.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/feature_grouping.py
--rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/msms.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/params.py
--rw-r--r--   0        0        0    13699 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/peak_detect.py
--rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/raw_data_utils.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/targeted_search.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 metabengine-0.0.5/src/metabengine/visual.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 metabengine-0.0.5/LICENSE
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 metabengine-0.0.5/README.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 metabengine-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 metabengine-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/__init__.py
+-rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/alignment.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/ann_feat_quality.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/calculate_mass.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/feat_extract.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/feature_grouping.py
+-rw-r--r--   0        0        0     5705 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/msms.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/params.py
+-rw-r--r--   0        0        0    13699 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/peak_detect.py
+-rw-r--r--   0        0        0    17883 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/raw_data_utils.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/targeted_search.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 metabengine-0.0.6/src/metabengine/visual.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 metabengine-0.0.6/LICENSE
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 metabengine-0.0.6/README.md
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 metabengine-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 metabengine-0.0.6/PKG-INFO
```

### Comparing `metabengine-0.0.5/src/metabengine/__init__.py` & `metabengine-0.0.6/src/metabengine/__init__.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/src/metabengine/alignment.py` & `metabengine-0.0.6/src/metabengine/alignment.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,19 +142,23 @@
     
     def choose_best_ms2(self):
         """
         A function to choose the best MS2 for the feature. 
         The best MS2 is the one with the highest summed intensity.
         """
 
-        if len(self.ms2_seq) > 1:
-            total_ints = [np.sum(ms2.prod_int_seq) for ms2 in self.ms2_seq]
-            self.best_ms2 = self.ms2_seq[np.argmax(total_ints)]
-        elif len(self.ms2_seq) == 1:
-            self.best_ms2 = self.ms2_seq[0]
+        total_ints = []
+
+        for ms2 in self.ms2_seq:
+            if ms2 is not None:
+                total_ints.append(np.sum(ms2.ints))
+            else:
+                total_ints.append(0.0)
+
+        self.best_ms2 = self.ms2_seq[np.argmax(total_ints)]
 
 
 def find_roi_from_data(feat, d, cross_file_params):
     """
     A function to find the feature from the MS data.
 
     Parameters
```

### Comparing `metabengine-0.0.5/src/metabengine/ann_feat_quality.py` & `metabengine-0.0.6/src/metabengine/ann_feat_quality.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/src/metabengine/calculate_mass.py` & `metabengine-0.0.6/src/metabengine/calculate_mass.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/src/metabengine/feat_extract.py` & `metabengine-0.0.6/src/metabengine/feat_extract.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/src/metabengine/feature_grouping.py` & `metabengine-0.0.6/src/metabengine/feature_grouping.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/src/metabengine/msms.py` & `metabengine-0.0.6/src/metabengine/msms.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/src/metabengine/params.py` & `metabengine-0.0.6/src/metabengine/params.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/src/metabengine/peak_detect.py` & `metabengine-0.0.6/src/metabengine/peak_detect.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/src/metabengine/raw_data_utils.py` & `metabengine-0.0.6/src/metabengine/raw_data_utils.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/src/metabengine/targeted_search.py` & `metabengine-0.0.6/src/metabengine/targeted_search.py`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/LICENSE` & `metabengine-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metabengine-0.0.5/pyproject.toml` & `metabengine-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "metabengine"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 maintainers = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 description = "Data preprocessing for mass spectrometry-based metabolomics data"
```

### Comparing `metabengine-0.0.5/PKG-INFO` & `metabengine-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabengine
-Version: 0.0.5
+Version: 0.0.6
 Summary: Data preprocessing for mass spectrometry-based metabolomics data
 Project-URL: Homepage, https://github.com/Waddlessss/metabengine
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

