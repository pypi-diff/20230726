# Comparing `tmp/wafermap-clustering-0.3.4.tar.gz` & `tmp/wafermap-clustering-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wafermap-clustering-0.3.4.tar", last modified: Mon Jul 24 08:17:26 2023, max compression
+gzip compressed data, was "wafermap-clustering-0.3.5.tar", last modified: Wed Jul 26 15:01:34 2023, max compression
```

## Comparing `wafermap-clustering-0.3.4.tar` & `wafermap-clustering-0.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.167187 wafermap-clustering-0.3.4/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.4/LICENSE.txt
--rw-rw-rw-   0        0        0      568 2023-07-24 08:17:26.165084 wafermap-clustering-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-24 08:17:26.168229 wafermap-clustering-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0      960 2023-07-24 08:17:03.000000 wafermap-clustering-0.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.088218 wafermap-clustering-0.3.4/tests/
--rw-rw-rw-   0        0        0     9605 2023-07-24 08:04:37.000000 wafermap-clustering-0.3.4/tests/test_clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.094459 wafermap-clustering-0.3.4/wafermap_clustering/
-drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.130603 wafermap-clustering-0.3.4/wafermap_clustering/configs/
--rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.4/wafermap_clustering/configs/config.py
-drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.135368 wafermap-clustering-0.3.4/wafermap_clustering/libs/
--rw-rw-rw-   0        0        0     4479 2023-07-19 09:07:18.000000 wafermap-clustering-0.3.4/wafermap_clustering/libs/klarf_lib.py
-drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.157861 wafermap-clustering-0.3.4/wafermap_clustering/models/
--rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.4/wafermap_clustering/models/clustered_defect.py
--rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.4/wafermap_clustering/models/clustering_performance.py
--rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.4/wafermap_clustering/models/clustering_result.py
--rw-rw-rw-   0        0        0     6705 2023-07-24 08:15:55.000000 wafermap-clustering-0.3.4/wafermap_clustering/wafermap_clustering.py
-drwxrwxrwx   0        0        0        0 2023-07-24 08:17:26.124300 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/
--rw-rw-rw-   0        0        0      568 2023-07-24 08:17:26.000000 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-07-24 08:17:26.000000 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 08:17:26.000000 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-24 08:17:26.000000 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-24 08:17:26.000000 wafermap-clustering-0.3.4/wafermap_clustering.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 15:01:34.082036 wafermap-clustering-0.3.5/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 wafermap-clustering-0.3.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      568 2023-07-26 15:01:34.075908 wafermap-clustering-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-27 14:30:27.000000 wafermap-clustering-0.3.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-26 15:01:34.082724 wafermap-clustering-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-07-26 14:49:57.000000 wafermap-clustering-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:01:33.989505 wafermap-clustering-0.3.5/tests/
+-rw-rw-rw-   0        0        0    12755 2023-07-26 14:59:03.000000 wafermap-clustering-0.3.5/tests/test_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:01:33.996645 wafermap-clustering-0.3.5/wafermap_clustering/
+drwxrwxrwx   0        0        0        0 2023-07-26 15:01:34.040639 wafermap-clustering-0.3.5/wafermap_clustering/configs/
+-rw-rw-rw-   0        0        0     3472 2023-06-27 08:34:33.000000 wafermap-clustering-0.3.5/wafermap_clustering/configs/config.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:01:34.049032 wafermap-clustering-0.3.5/wafermap_clustering/libs/
+-rw-rw-rw-   0        0        0     4572 2023-07-26 14:53:07.000000 wafermap-clustering-0.3.5/wafermap_clustering/libs/klarf_lib.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:01:34.071885 wafermap-clustering-0.3.5/wafermap_clustering/models/
+-rw-rw-rw-   0        0        0      125 2023-03-09 12:31:13.000000 wafermap-clustering-0.3.5/wafermap_clustering/models/clustered_defect.py
+-rw-rw-rw-   0        0        0      468 2023-07-19 09:50:06.000000 wafermap-clustering-0.3.5/wafermap_clustering/models/clustering_performance.py
+-rw-rw-rw-   0        0        0      854 2023-06-27 08:43:17.000000 wafermap-clustering-0.3.5/wafermap_clustering/models/clustering_result.py
+-rw-rw-rw-   0        0        0     6949 2023-07-26 14:32:07.000000 wafermap-clustering-0.3.5/wafermap_clustering/wafermap_clustering.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:01:34.033777 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-07-26 15:01:33.000000 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      536 2023-07-26 15:01:33.000000 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 15:01:33.000000 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-26 15:01:33.000000 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-26 15:01:33.000000 wafermap-clustering-0.3.5/wafermap_clustering.egg-info/top_level.txt
```

### Comparing `wafermap-clustering-0.3.4/LICENSE.txt` & `wafermap-clustering-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.4/PKG-INFO` & `wafermap-clustering-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.4
+Version: 0.3.5
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.4.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.5.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.4/setup.py` & `wafermap-clustering-0.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.4"
+version = "0.3.5"
 
 setup(
     name="wafermap-clustering",
     version=version,
     packages=[
         "wafermap_clustering",
         "wafermap_clustering.configs",
```

### Comparing `wafermap-clustering-0.3.4/tests/test_clustering.py` & `wafermap-clustering-0.3.5/tests/test_clustering.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         logger.addHandler(time_rotating_handler)
 
     return logger
 
 
 class TestClustering(unittest.TestCase):
     def setUp(self) -> None:
+        self.path_klarf_single_wafer_no_defect = ASSETS_PATH / "klarf_no_defect.000"
         self.path_klarf_single_wafer = ASSETS_PATH / "J052SBN_8196_J052SBN-01.000"
         self.path_klarf_multi_wafers = ASSETS_PATH / "J237DTA_3236.000"
         self.path_klarf_single_wafer_large_klarf = ASSETS_PATH / "LARGE_KLARF.000"
 
         self.config = Config(
             platform="windows",
             conf_path=ASSETS_PATH / "conf" / "config.json",
@@ -70,14 +71,50 @@
                 ):
                     continue
 
                 self.assertEqual(line1, line2)
 
         return True
 
+    def test_clustering_dbscan_single_wafer_no_defect(self):
+        # GIVEN
+        expected_summary = [
+            {
+                "result_timestamp": "01-24-23 12:08:00",
+                "lot_id": "J247LFS",
+                "step_id": "8625",
+                "wafer_id": "02",
+                "clusters": 0,
+                "clustering": {},
+            }
+        ]
+
+        # WHEN
+        clustering = Clustering(config=self.config, logger=self.logger)
+        results = clustering.apply_from_klarf_path(
+            self.path_klarf_single_wafer_no_defect
+        )
+
+        summary = [
+            {
+                "result_timestamp": res.result_timestamp,
+                "lot_id": res.lot_id,
+                "step_id": res.step_id,
+                "wafer_id": res.wafer_id,
+                "clusters": res.clusters,
+                "clustering": dict(
+                    Counter([cluster.bin for cluster in res.clustered_defects])
+                ),
+            }
+            for res in results
+        ]
+
+        # THEN
+        self.assertEqual(summary, expected_summary)
+
     def test_clustering_dbscan_single_wafer(self):
         # GIVEN
         expected_summary = [
             {
                 "result_timestamp": "02-23-21 06:10:02",
                 "lot_id": "J052SBN",
                 "step_id": "8196",
@@ -237,14 +274,67 @@
             }
             for res in results
         ]
 
         # THEN
         self.assertEqual(summary, expected_summary)
 
+    def test_clustering_dbscan_no_defect_with_baby_klarf_returned(self):
+        # GIVEN
+        saved_klarf_paths = sorted(
+            [
+                ASSETS_PATH
+                / "saved"
+                / "klarf_baby"
+                / "J247LFS_8625_02_dbscan_no_defect.000"
+            ]
+        )
+
+        # WHEN
+        clustering = Clustering(config=self.config, logger=self.logger)
+        results = clustering.apply_from_klarf_path(
+            klarf_path=self.path_klarf_single_wafer_no_defect,
+            output_directory=ASSETS_OUPUT_PATH,
+            klarf_format=KlarfFormat.BABY.value,
+        )
+        results = sorted(results, key=lambda x: x.output_filename)
+
+        # THEN
+        self.assertEqual(len(results), len(saved_klarf_paths))
+        for index, result in enumerate(results):
+            self.assertFileEqual(
+                saved_klarf_paths[index],
+                result.output_filename,
+                ignore_rows=["FileTimestamp"],
+            )
+
+    def test_clustering_dbscan_no_defect_with_full_klarf_returned(self):
+        # GIVEN
+        saved_klarf_paths = sorted(
+            [ASSETS_PATH / "saved" / "klarf_full" / "klarf_no_defect_dbscan.000"]
+        )
+
+        # WHEN
+        clustering = Clustering(config=self.config, logger=self.logger)
+        results = clustering.apply_from_klarf_path(
+            klarf_path=self.path_klarf_single_wafer_no_defect,
+            output_directory=ASSETS_OUPUT_PATH,
+            klarf_format=KlarfFormat.FULL.value,
+        )
+        results = sorted(results, key=lambda x: x.output_filename)
+
+        # THEN
+        self.assertEqual(len(results), len(saved_klarf_paths))
+        for index, result in enumerate(results):
+            self.assertFileEqual(
+                saved_klarf_paths[index],
+                result.output_filename,
+                ignore_rows=["FileTimestamp"],
+            )
+
     def test_clustering_dbscan_multi_wafers_with_baby_klarf_returned(self):
         # GIVEN
         saved_klarf_paths = sorted(
             [
                 ASSETS_PATH / "saved" / "klarf_baby" / "J237DTA_3236_01_dbscan.000",
                 ASSETS_PATH / "saved" / "klarf_baby" / "J237DTA_3236_02_dbscan.000",
                 ASSETS_PATH / "saved" / "klarf_baby" / "J237DTA_3236_06_dbscan.000",
```

### Comparing `wafermap-clustering-0.3.4/wafermap_clustering/configs/config.py` & `wafermap-clustering-0.3.5/wafermap_clustering/configs/config.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.4/wafermap_clustering/libs/klarf_lib.py` & `wafermap-clustering-0.3.5/wafermap_clustering/libs/klarf_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,16 +101,19 @@
         f.write(f"FileVersion {file_version};\n")
         f.write(f"ResultTimestamp {single_klarf.result_timestamp};\n")
         f.write(f'LotID "{single_klarf.lot_id}";\n')
         f.write(f'DeviceID "{single_klarf.device_id}";\n')
         f.write(f'StepID "{single_klarf.step_id}";\n')
         f.write(f'WaferID "{single_klarf.wafer.id}";\n')
         f.write(f"DefectRecordSpec 2 DEFECTID {attribute} ;\n")
-        f.write(f"DefectList\n")
-        f.write("".join(defects))
+        if len(defects) == 0:
+            f.write(f"DefectList;\n")
+        else:
+            f.write(f"DefectList\n")
+            f.write("".join(defects))
         f.write("EndOfFile;")
 
     return time.time() - tic
 
 
 def create_baby_defect_row(
     defect_id: int,
```

### Comparing `wafermap-clustering-0.3.4/wafermap_clustering/models/clustering_result.py` & `wafermap-clustering-0.3.5/wafermap_clustering/models/clustering_result.py`

 * *Files identical despite different names*

### Comparing `wafermap-clustering-0.3.4/wafermap_clustering/wafermap_clustering.py` & `wafermap-clustering-0.3.5/wafermap_clustering/wafermap_clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,36 +67,41 @@
         for index, wafer in enumerate(klarf_content.wafers):
             tic = time.time()
 
             single_klarf = klarf_convert.convert_to_single_klarf_content(
                 klarf_content=klarf_content, wafer_index=index
             )
 
-            defect_ids = np.array([defect.id for defect in wafer.defects])
-            defect_points = np.array(
-                [
-                    (defect.point[0] / 1000, defect.point[1] / 1000)
-                    for defect in wafer.defects
-                ]
-            )
+            if len(wafer.defects) == 0:
+                clusters = 0
+                clustered_defects = []
+                clustering_timestamp = 0
+            else:
+                defect_ids = np.array([defect.id for defect in wafer.defects])
+                defect_points = np.array(
+                    [
+                        (defect.point[0] / 1000, defect.point[1] / 1000)
+                        for defect in wafer.defects
+                    ]
+                )
 
-            labels = clustering.fit_predict(defect_points)
+                labels = clustering.fit_predict(defect_points)
 
-            clustering_values = np.column_stack((defect_ids, labels))
-            clusters = len(np.unique(labels, axis=0))
+                clustering_values = np.column_stack((defect_ids, labels))
+                clusters = len(np.unique(labels, axis=0))
 
-            clustered_defects = [
-                ClusteredDefect(
-                    defect_id=defect_id,
-                    bin=cluster_label,
-                )
-                for defect_id, cluster_label in clustering_values
-            ]
+                clustered_defects = [
+                    ClusteredDefect(
+                        defect_id=defect_id,
+                        bin=cluster_label,
+                    )
+                    for defect_id, cluster_label in clustering_values
+                ]
 
-            clustering_timestamp = time.time() - tic
+                clustering_timestamp = time.time() - tic
 
             clustering_result = ClusteringResult(
                 file_version=single_klarf.file_version,
                 result_timestamp=single_klarf.result_timestamp,
                 lot_id=single_klarf.lot_id,
                 device_id=single_klarf.device_id,
                 step_id=single_klarf.step_id,
```

### Comparing `wafermap-clustering-0.3.4/wafermap_clustering.egg-info/PKG-INFO` & `wafermap-clustering-0.3.5/wafermap_clustering.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: wafermap-clustering
-Version: 0.3.4
+Version: 0.3.5
 Summary: A project to apply clustering on wafermaps
 Home-page: https://github.com/Impro02/wafermap-clustering
-Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.4.tar.gz
+Download-URL: https://github.com/Impro02/wafermap-clustering/archive/refs/tags/0.3.5.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wafermap-clustering-0.3.4/wafermap_clustering.egg-info/SOURCES.txt` & `wafermap-clustering-0.3.5/wafermap_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

