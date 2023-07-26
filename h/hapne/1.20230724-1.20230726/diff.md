# Comparing `tmp/hapne-1.20230724.tar.gz` & `tmp/hapne-1.20230726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hapne-1.20230724.tar", last modified: Mon Jul 24 15:29:05 2023, max compression
+gzip compressed data, was "hapne-1.20230726.tar", last modified: Wed Jul 26 08:38:05 2023, max compression
```

## Comparing `hapne-1.20230724.tar` & `hapne-1.20230726.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.987781 hapne-1.20230724/
--rw-r--r--   0 romainfournier   (501) staff       (20)    35149 2023-04-24 08:33:59.000000 hapne-1.20230724/LICENSE
--rw-r--r--   0 romainfournier   (501) staff       (20)     7002 2023-07-24 15:29:05.987889 hapne-1.20230724/PKG-INFO
--rw-r--r--   0 romainfournier   (501) staff       (20)     7452 2023-07-24 14:05:01.000000 hapne-1.20230724/README.md
--rw-r--r--   0 romainfournier   (501) staff       (20)      104 2023-04-24 08:33:59.000000 hapne-1.20230724/pyproject.toml
--rw-r--r--   0 romainfournier   (501) staff       (20)     6278 2023-07-24 14:05:01.000000 hapne-1.20230724/read_me.md
--rw-r--r--   0 romainfournier   (501) staff       (20)      999 2023-07-24 15:29:05.988514 hapne-1.20230724/setup.cfg
--rw-r--r--   0 romainfournier   (501) staff       (20)       39 2023-04-24 08:33:59.000000 hapne-1.20230724/setup.py
-drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.974085 hapne-1.20230724/src/
-drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.977811 hapne-1.20230724/src/HapNe.egg-info/
--rw-r--r--   0 romainfournier   (501) staff       (20)     7002 2023-07-24 15:29:05.000000 hapne-1.20230724/src/HapNe.egg-info/PKG-INFO
--rw-r--r--   0 romainfournier   (501) staff       (20)     1083 2023-07-24 15:29:05.000000 hapne-1.20230724/src/HapNe.egg-info/SOURCES.txt
--rw-r--r--   0 romainfournier   (501) staff       (20)        1 2023-07-24 15:29:05.000000 hapne-1.20230724/src/HapNe.egg-info/dependency_links.txt
--rw-r--r--   0 romainfournier   (501) staff       (20)      103 2023-07-24 15:29:05.000000 hapne-1.20230724/src/HapNe.egg-info/requires.txt
--rw-r--r--   0 romainfournier   (501) staff       (20)        6 2023-07-24 15:29:05.000000 hapne-1.20230724/src/HapNe.egg-info/top_level.txt
-drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.980214 hapne-1.20230724/src/hapne/
--rw-r--r--   0 romainfournier   (501) staff       (20)       88 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/__init__.py
-drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.982838 hapne-1.20230724/src/hapne/backend/
--rw-r--r--   0 romainfournier   (501) staff       (20)    12891 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/backend/DemographicHistory.py
--rw-r--r--   0 romainfournier   (501) staff       (20)     1024 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/backend/DemographicHistory2StatsModelAdapter.py
--rw-r--r--   0 romainfournier   (501) staff       (20)    20487 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/backend/HapNe.py
--rw-r--r--   0 romainfournier   (501) staff       (20)    21198 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/backend/IO.py
--rw-r--r--   0 romainfournier   (501) staff       (20)     7393 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/backend/StatsModel.py
--rw-r--r--   0 romainfournier   (501) staff       (20)        0 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/backend/__init__.py
-drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.983613 hapne-1.20230724/src/hapne/convert/
--rw-r--r--   0 romainfournier   (501) staff       (20)        0 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/convert/__init__.py
-drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.984290 hapne-1.20230724/src/hapne/convert/mathii_scripts/
--rw-r--r--   0 romainfournier   (501) staff       (20)        0 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/convert/mathii_scripts/__init__.py
--rw-r--r--   0 romainfournier   (501) staff       (20)     9597 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/convert/mathii_scripts/py3Eigenstrat.py
--rw-r--r--   0 romainfournier   (501) staff       (20)     6560 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/convert/tools.py
-drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.985091 hapne-1.20230724/src/hapne/files/
--rw-r--r--   0 romainfournier   (501) staff       (20)     2380 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/files/regions_grch37.txt
--rw-r--r--   0 romainfournier   (501) staff       (20)     2664 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/files/regions_grch38.txt
--rw-r--r--   0 romainfournier   (501) staff       (20)      314 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/fit.py
--rw-r--r--   0 romainfournier   (501) staff       (20)     1194 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/ibd.py
--rw-r--r--   0 romainfournier   (501) staff       (20)    16764 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/ld.py
--rw-r--r--   0 romainfournier   (501) staff       (20)     1727 2023-04-24 08:33:59.000000 hapne-1.20230724/src/hapne/output.py
--rw-r--r--   0 romainfournier   (501) staff       (20)     5330 2023-07-24 14:05:01.000000 hapne-1.20230724/src/hapne/utils.py
-drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-24 15:29:05.987556 hapne-1.20230724/tests/
--rw-r--r--   0 romainfournier   (501) staff       (20)      647 2023-04-24 08:33:59.000000 hapne-1.20230724/tests/test_build_hist.py
--rw-r--r--   0 romainfournier   (501) staff       (20)      809 2023-07-24 12:29:12.000000 hapne-1.20230724/tests/test_compute_ld.py
--rw-r--r--   0 romainfournier   (501) staff       (20)     1314 2023-04-24 08:33:59.000000 hapne-1.20230724/tests/test_eigenstrat2vcf.py
--rw-r--r--   0 romainfournier   (501) staff       (20)     1791 2023-04-24 08:33:59.000000 hapne-1.20230724/tests/test_hapne.py
--rw-r--r--   0 romainfournier   (501) staff       (20)     3550 2023-04-24 08:33:59.000000 hapne-1.20230724/tests/test_time_het.py
--rw-r--r--   0 romainfournier   (501) staff       (20)      329 2023-04-24 08:33:59.000000 hapne-1.20230724/tests/test_vcf2splitbed.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-26 08:38:05.223711 hapne-1.20230726/
+-rw-r--r--   0 romainfournier   (501) staff       (20)    35149 2023-04-24 08:33:59.000000 hapne-1.20230726/LICENSE
+-rw-r--r--   0 romainfournier   (501) staff       (20)     6965 2023-07-26 08:38:05.223814 hapne-1.20230726/PKG-INFO
+-rw-r--r--   0 romainfournier   (501) staff       (20)     7452 2023-07-24 14:05:01.000000 hapne-1.20230726/README.md
+-rw-r--r--   0 romainfournier   (501) staff       (20)      104 2023-04-24 08:33:59.000000 hapne-1.20230726/pyproject.toml
+-rw-r--r--   0 romainfournier   (501) staff       (20)     6278 2023-07-24 14:05:01.000000 hapne-1.20230726/read_me.md
+-rw-r--r--   0 romainfournier   (501) staff       (20)      999 2023-07-26 08:38:05.224405 hapne-1.20230726/setup.cfg
+-rw-r--r--   0 romainfournier   (501) staff       (20)       39 2023-04-24 08:33:59.000000 hapne-1.20230726/setup.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-26 08:38:05.205195 hapne-1.20230726/src/
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-26 08:38:05.212209 hapne-1.20230726/src/HapNe.egg-info/
+-rw-r--r--   0 romainfournier   (501) staff       (20)     6965 2023-07-26 08:38:05.000000 hapne-1.20230726/src/HapNe.egg-info/PKG-INFO
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1083 2023-07-26 08:38:05.000000 hapne-1.20230726/src/HapNe.egg-info/SOURCES.txt
+-rw-r--r--   0 romainfournier   (501) staff       (20)        1 2023-07-26 08:38:05.000000 hapne-1.20230726/src/HapNe.egg-info/dependency_links.txt
+-rw-r--r--   0 romainfournier   (501) staff       (20)      103 2023-07-26 08:38:05.000000 hapne-1.20230726/src/HapNe.egg-info/requires.txt
+-rw-r--r--   0 romainfournier   (501) staff       (20)        6 2023-07-26 08:38:05.000000 hapne-1.20230726/src/HapNe.egg-info/top_level.txt
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-26 08:38:05.215401 hapne-1.20230726/src/hapne/
+-rw-r--r--   0 romainfournier   (501) staff       (20)       88 2023-04-24 08:33:59.000000 hapne-1.20230726/src/hapne/__init__.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-26 08:38:05.219583 hapne-1.20230726/src/hapne/backend/
+-rw-r--r--   0 romainfournier   (501) staff       (20)    12891 2023-04-24 08:33:59.000000 hapne-1.20230726/src/hapne/backend/DemographicHistory.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1024 2023-04-24 08:33:59.000000 hapne-1.20230726/src/hapne/backend/DemographicHistory2StatsModelAdapter.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)    20920 2023-07-26 08:36:37.000000 hapne-1.20230726/src/hapne/backend/HapNe.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)    21370 2023-07-26 08:36:37.000000 hapne-1.20230726/src/hapne/backend/IO.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     7393 2023-04-24 08:33:59.000000 hapne-1.20230726/src/hapne/backend/StatsModel.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)        0 2023-04-24 08:33:59.000000 hapne-1.20230726/src/hapne/backend/__init__.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-26 08:38:05.219981 hapne-1.20230726/src/hapne/convert/
+-rw-r--r--   0 romainfournier   (501) staff       (20)        0 2023-04-24 08:33:59.000000 hapne-1.20230726/src/hapne/convert/__init__.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-26 08:38:05.220592 hapne-1.20230726/src/hapne/convert/mathii_scripts/
+-rw-r--r--   0 romainfournier   (501) staff       (20)        0 2023-04-24 08:33:59.000000 hapne-1.20230726/src/hapne/convert/mathii_scripts/__init__.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     9597 2023-04-24 08:33:59.000000 hapne-1.20230726/src/hapne/convert/mathii_scripts/py3Eigenstrat.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     6560 2023-07-24 14:05:01.000000 hapne-1.20230726/src/hapne/convert/tools.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-26 08:38:05.221291 hapne-1.20230726/src/hapne/files/
+-rw-r--r--   0 romainfournier   (501) staff       (20)     2380 2023-07-24 14:05:01.000000 hapne-1.20230726/src/hapne/files/regions_grch37.txt
+-rw-r--r--   0 romainfournier   (501) staff       (20)     2664 2023-07-24 14:05:01.000000 hapne-1.20230726/src/hapne/files/regions_grch38.txt
+-rw-r--r--   0 romainfournier   (501) staff       (20)      314 2023-04-24 08:33:59.000000 hapne-1.20230726/src/hapne/fit.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1194 2023-07-24 14:05:01.000000 hapne-1.20230726/src/hapne/ibd.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)    16764 2023-07-24 14:05:01.000000 hapne-1.20230726/src/hapne/ld.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1727 2023-04-24 08:33:59.000000 hapne-1.20230726/src/hapne/output.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     5340 2023-07-26 08:36:37.000000 hapne-1.20230726/src/hapne/utils.py
+drwxr-xr-x   0 romainfournier   (501) staff       (20)        0 2023-07-26 08:38:05.223488 hapne-1.20230726/tests/
+-rw-r--r--   0 romainfournier   (501) staff       (20)      647 2023-04-24 08:33:59.000000 hapne-1.20230726/tests/test_build_hist.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)      809 2023-07-24 12:29:12.000000 hapne-1.20230726/tests/test_compute_ld.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     1314 2023-04-24 08:33:59.000000 hapne-1.20230726/tests/test_eigenstrat2vcf.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     2224 2023-07-26 08:36:37.000000 hapne-1.20230726/tests/test_hapne.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)     3550 2023-04-24 08:33:59.000000 hapne-1.20230726/tests/test_time_het.py
+-rw-r--r--   0 romainfournier   (501) staff       (20)      329 2023-04-24 08:33:59.000000 hapne-1.20230726/tests/test_vcf2splitbed.py
```

### Comparing `hapne-1.20230724/LICENSE` & `hapne-1.20230726/LICENSE`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/PKG-INFO` & `hapne-1.20230726/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: hapne
-Version: 1.20230724
+Version: 1.20230726
 Summary: Haplotype-based inference of recent effective population size in modern and ancient DNA samples
 Home-page: https://github.com/PalamaraLab/HapNe
 Author: Romain Fournier (PalamaraLab, Department of Statistics, Oxford University)
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/PalamaraLab/HapNe/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -213,9 +211,7 @@
 If you use this software, please cite:
 
 R. Fournier, D. Reich, P. Palamara. Haplotype-based inference of recent effective population size in modern and ancient DNA samples. (preprint) bioRxiv, 2022.
 # Acknowledgments  
 Two scripts of the `convert` module were downloaded from the following repositories and edited to fit into this package:
 - "https://github.com/mathii/pyEigenstrat" 
 - "https://github.com/mathii/gdc"
-
-
```

### Comparing `hapne-1.20230724/README.md` & `hapne-1.20230726/README.md`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/read_me.md` & `hapne-1.20230726/read_me.md`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/setup.cfg` & `hapne-1.20230726/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hapne
-version = 1.20230724
+version = 1.20230726
 author = Romain Fournier (PalamaraLab, Department of Statistics, Oxford University)
 description = Haplotype-based inference of recent effective population size in modern and ancient DNA samples
 long_description = file: read_me.md
 long_description_content_type = text/markdown
 url = https://github.com/PalamaraLab/HapNe
 project_urls = 
 	Bug Tracker = https://github.com/PalamaraLab/HapNe/issues
```

### Comparing `hapne-1.20230724/src/HapNe.egg-info/PKG-INFO` & `hapne-1.20230726/src/HapNe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: hapne
-Version: 1.20230724
+Version: 1.20230726
 Summary: Haplotype-based inference of recent effective population size in modern and ancient DNA samples
 Home-page: https://github.com/PalamaraLab/HapNe
 Author: Romain Fournier (PalamaraLab, Department of Statistics, Oxford University)
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/PalamaraLab/HapNe/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -213,9 +211,7 @@
 If you use this software, please cite:
 
 R. Fournier, D. Reich, P. Palamara. Haplotype-based inference of recent effective population size in modern and ancient DNA samples. (preprint) bioRxiv, 2022.
 # Acknowledgments  
 Two scripts of the `convert` module were downloaded from the following repositories and edited to fit into this package:
 - "https://github.com/mathii/pyEigenstrat" 
 - "https://github.com/mathii/gdc"
-
-
```

### Comparing `hapne-1.20230724/src/HapNe.egg-info/SOURCES.txt` & `hapne-1.20230726/src/HapNe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/backend/DemographicHistory.py` & `hapne-1.20230726/src/hapne/backend/DemographicHistory.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/backend/DemographicHistory2StatsModelAdapter.py` & `hapne-1.20230726/src/hapne/backend/DemographicHistory2StatsModelAdapter.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/backend/HapNe.py` & `hapne-1.20230726/src/hapne/backend/HapNe.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,19 @@
         # Method specific instances
         self.io = self.get_loader()
         self.stats_model = self.get_stats_model()
 
         # Parameter related to the model
         nb_points = 7 if self.method == "ld" else 8
         start = -5 if self.method == "ld" else -6
-        self.parameter_grid = np.array([10.**(start + ii) for ii in range(0, nb_points)])
+        if self.config.getfloat("CONFIG", "sigma2", fallback=None) is None:
+            self.parameter_grid = np.array([10.**(start + ii) for ii in range(0, nb_points)])
+        else:
+            logging.info("Using user-provided sigma2")
+            self.parameter_grid = np.array([self.config.getfloat("CONFIG", "sigma2")])
         self.u_min = self.get_default_u_min()  # Minimum value of u
         self.u_quantile = self.config.getfloat("CONFIG", "u_quantile", fallback=self.u_min)
         self.dt_min = max(0.25, self.config.getint("CONFIG", "dt_min", fallback=1))
         self.dt_max = self.config.getint("CONFIG", "dt_max", fallback=5000)
         self.t_max = self.config.getint("CONFIG", "t_max", fallback=125)
         self.buffer_time = self.t_max - 25  # the times averages the deep time effect
         # Parameters related to the fitting procedure
@@ -178,19 +182,14 @@
     def fit_regularized(self):
         """
         Perform HapNe fitting procedure and save the results.
         """
         # Step 1 : calibrate times and get MAP Ne and best regularisation
         logging.info("Starting the calibration step...")
         ne_hat, sig2 = self.calibrate_method()
-        logging.info(f"Calibration step done, {sig2:.5f} selected!")
-        if sig2 < self.parameter_grid[2]:
-            sig2message = "The evidence for fluctuation is weak, the results may be unreliable (looking too constant)"
-            logging.warning(sig2message)
-            self.io.summary_message += "\n" + sig2message + "\n"
         # Step 2 : bootstrap results
         logging.info("Starting the bootstrapping procedure...")
         ne_bootstrap = self.bootstrap(ne_hat, sig2)
         # Step 3 : save results
         logging.info("Saving results...")
         return ne_bootstrap
 
@@ -212,14 +211,24 @@
             logging.info(f"Iteration {ii+1}/{nb_iterations} : {sig2:.5f} - {sse:.2f} ")
             nes[ii, :] = ne_hat.ravel().copy()
             self.update_times(ne_hat)
             # Escape the iterations if time intervals have converged
             if self.time_intervals_have_converged(old_times=times[ii, :]):
                 logging.info(f"Converged at iteration {ii}")
                 return self.select_calibration(times[:ii + 1, :], nes[:ii + 1, :], sigmas[:ii + 1], sses[:ii + 1])
+
+        if self.config.getfloat("CONFIG", "sigma2", fallback=None) is None:
+            sig2message = f"Calibration step done, {sig2:.5f} selected!"
+            logging.info(sig2message)
+            self.io.summary_message += "\n" + sig2message + "\n"
+            if sig2 < self.parameter_grid[2]:
+                sig2message = "Evidence for fluctuation is weak, the results may be unreliable (looking too constant)"
+                logging.warning(sig2message)
+                self.io.summary_message += "\n" + sig2message + "\n"
+
         return self.select_calibration(times, nes, sigmas, sses)
 
     def run_relaxation(self):
         """
         Run a grid-search over different values of the hyperparameters
         Select the highest regularisation consistent with the signal.
         """
```

### Comparing `hapne-1.20230724/src/hapne/backend/IO.py` & `hapne-1.20230726/src/hapne/backend/IO.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
         self.suffix = suffix
         self.extension = extension
 
         self.sample_size = self.get_sample_size()
 
         message = f"Analysing {self.sample_size} "
-        message += "diploid individuals"
+        message += "haplotypes"
         logging.info(message)
 
         self._bins = self.read_bins()
         bin_from = self.apply_filter_u(self._bins[0, :].reshape(-1, 1))
         bin_to = self.apply_filter_u(self._bins[1, :].reshape(-1, 1))
         self.bins = np.append(bin_from.reshape(-1), bin_to[-1, 0]).reshape(-1)
         self._mu = None
@@ -471,15 +471,17 @@
             delta_t_density_binned[tau, 0] = 1 / n_terms * \
                 cross_terms(self.age_density_in_bin[:, tau], self.age_density_in_bin[:, tau])
             for jj in range(0, tau):
                 delta_t_density_binned[tau, tau - jj] = 1 / n_terms * \
                     2 * cross_terms(self.age_density_in_bin[:, tau], self.age_density_in_bin[:, jj])
 
         tau_density_binned = np.sum(delta_t_density_binned, axis=1)
-        delta_t_density_binned = delta_t_density_binned / tau_density_binned[:, None]
+        delta_t_density_binned = np.divide(delta_t_density_binned, tau_density_binned[:, None],
+                                           out=np.zeros_like(delta_t_density_binned),
+                                           where=(tau_density_binned[:, None] != 0))
         return tau_density_binned, delta_t_density_binned
 
     def _compute_offset_correction(self, u):
         delta_ts = self.delta_ts.reshape((-1, 1))
         u = u.reshape((1, -1))
         exponential_decays = np.exp(- (delta_ts - 0.75) * u)
```

### Comparing `hapne-1.20230724/src/hapne/backend/StatsModel.py` & `hapne-1.20230726/src/hapne/backend/StatsModel.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/convert/mathii_scripts/py3Eigenstrat.py` & `hapne-1.20230726/src/hapne/convert/mathii_scripts/py3Eigenstrat.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/convert/tools.py` & `hapne-1.20230726/src/hapne/convert/tools.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/files/regions_grch37.txt` & `hapne-1.20230726/src/hapne/files/regions_grch37.txt`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/files/regions_grch38.txt` & `hapne-1.20230726/src/hapne/files/regions_grch38.txt`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/ibd.py` & `hapne-1.20230726/src/hapne/ibd.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/ld.py` & `hapne-1.20230726/src/hapne/ld.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/output.py` & `hapne-1.20230726/src/hapne/output.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/src/hapne/utils.py` & `hapne-1.20230726/src/hapne/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,28 +54,28 @@
         makedirs(save_as)
     to_save.to_csv(save_as + f"/{popname}.age", index=False)
 
 
 def get_age_samples_in_bp(config: ConfigParser):
     anno_file = pd.read_csv(config.get("CONFIG", "anno_file"), sep="\t")
 
+    individuals_in_study = get_individuals_in_study(config)
+    individuals_in_study.columns = [anno_file.columns[1]]
+    anno = pd.merge(individuals_in_study, anno_file, how='inner', on=[anno_file.columns[1]])
     col_bp_index = config.getint("CONFIG", "anno_bp_column", fallback=8)
     col_stdbp_index = col_bp_index + 1
 
     # Convert the `col_bp` and `col_stdbp` columns to int
     try:
-        anno_file[anno_file.columns[col_bp_index]] = anno_file[anno_file.columns[col_bp_index]].astype(int)
-        anno_file[anno_file.columns[col_stdbp_index]] = anno_file[anno_file.columns[col_stdbp_index]].astype(int)
+        anno[anno.columns[col_bp_index]] = anno[anno.columns[col_bp_index]].astype(int)
+        anno[anno.columns[col_stdbp_index]] = anno[anno.columns[col_stdbp_index]].astype(int)
     except ValueError:
-        print("Columns referring to age of samples cannot be converted to int. Please check the anno_bp_column.")
-
-    individuals_in_study = get_individuals_in_study(config)
-    individuals_in_study.columns = [anno_file.columns[1]]
-    anno = pd.merge(individuals_in_study, anno_file, how='inner', on=[anno_file.columns[1]]).values
-
+        raise ValueError(f"Columns {anno.columns[col_bp_index]} and {anno.columns[col_stdbp_index]} "
+                         f"should be integers")
+    anno = anno.values
     # Clip the uncertainty value to avoid having samples from the future
     uncertainty = np.minimum(anno[:, col_bp_index], 2 * anno[:, col_stdbp_index])
 
     age_from = (anno[:, col_bp_index] - uncertainty).reshape((-1, 1)).astype(int)
     age_to = (anno[:, col_bp_index] + uncertainty).reshape((-1, 1)).astype(int)
     return age_from, age_to
```

### Comparing `hapne-1.20230724/tests/test_build_hist.py` & `hapne-1.20230726/tests/test_build_hist.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/tests/test_compute_ld.py` & `hapne-1.20230726/tests/test_compute_ld.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/tests/test_eigenstrat2vcf.py` & `hapne-1.20230726/tests/test_eigenstrat2vcf.py`

 * *Files identical despite different names*

### Comparing `hapne-1.20230724/tests/test_hapne.py` & `hapne-1.20230726/tests/test_hapne.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,25 @@
     config["CONFIG"]["nb_bootstraps"] = "10"
     hapne_ld(config)
     inferred_ne = pd.read_csv("tests/files/const_test_ld/HapNe/hapne.csv")["Q0.5"].values
     true_ne = np.ones_like(inferred_ne) * 20_000
     assert np.mean((inferred_ne - true_ne) / true_ne) < 0.01
 
 
+def test_hapne_ld_sigma_hook():
+    config = ConfigParser()
+    config.read("tests/files/const_hapne_ld.ini")
+    config["CONFIG"]["nb_bootstraps"] = "10"
+    config["CONFIG"]["sigma2"] = "0.000001"
+    hapne_ld(config)
+    inferred_ne = pd.read_csv("tests/files/const_test_ld/HapNe/hapne.csv")["Q0.5"].values
+    true_ne = np.ones_like(inferred_ne) * 20_000
+    assert np.mean((inferred_ne - true_ne) / true_ne) < 0.01
+
+
 def test_hapne_ld_fixed():
     config = ConfigParser()
     config.read("tests/files/const_hapne_ld_fixed.ini")
     config["CONFIG"]["nb_bootstraps"] = "10"
     hapne_ld(config)
     inferred_ne = pd.read_csv("tests/files/const_test_ld_fixed/HapNe/hapne.csv")["Q0.5"].values
     true_ne = np.ones_like(inferred_ne) * 20_000
@@ -44,9 +55,9 @@
     true_ne = np.ones_like(inferred_ne) * 20_000
     assert np.mean((inferred_ne - true_ne) / true_ne) < 0.01
 
 
 if __name__ == "__main__":
     # set logging level to INFO
     logging.basicConfig(level=logging.INFO)
-    test_hapne_ld()
+    test_hapne_ld_sigma_hook()
     # test_hapne_ibd()
```

### Comparing `hapne-1.20230724/tests/test_time_het.py` & `hapne-1.20230726/tests/test_time_het.py`

 * *Files identical despite different names*

