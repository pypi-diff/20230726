# Comparing `tmp/GPyS-0.0.31.tar.gz` & `tmp/GPyS-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPyS-0.0.31.tar", last modified: Sat Jul 22 19:12:19 2023, max compression
+gzip compressed data, was "GPyS-0.0.32.tar", last modified: Tue Jul 25 23:51:37 2023, max compression
```

## Comparing `GPyS-0.0.31.tar` & `GPyS-0.0.32.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.232463 GPyS-0.0.31/
--rw-rw-rw-   0        0        0    34727 2023-07-20 16:07:58.000000 GPyS-0.0.31/LICENSE
--rw-rw-rw-   0        0        0     1891 2023-07-22 19:12:19.230409 GPyS-0.0.31/PKG-INFO
--rw-rw-rw-   0        0        0     1369 2023-07-20 16:07:58.000000 GPyS-0.0.31/README.md
--rw-rw-rw-   0        0        0      659 2023-07-22 19:11:59.000000 GPyS-0.0.31/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 19:12:19.233445 GPyS-0.0.31/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.169981 GPyS-0.0.31/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.190403 GPyS-0.0.31/src/GPyS.egg-info/
--rw-rw-rw-   0        0        0     1891 2023-07-22 19:12:19.000000 GPyS-0.0.31/src/GPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2023-07-22 19:12:19.000000 GPyS-0.0.31/src/GPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 19:12:19.000000 GPyS-0.0.31/src/GPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-22 19:12:19.000000 GPyS-0.0.31/src/GPyS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.200454 GPyS-0.0.31/src/GPyS_LOOCV_error/
--rw-rw-rw-   0        0        0     9401 2023-07-22 18:45:07.000000 GPyS-0.0.31/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py
--rw-rw-rw-   0        0        0       35 2023-07-20 16:07:58.000000 GPyS-0.0.31/src/GPyS_LOOCV_error/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.212442 GPyS-0.0.31/src/GPyS_prediction/
--rw-rw-rw-   0        0        0    20191 2023-07-22 00:10:49.000000 GPyS-0.0.31/src/GPyS_prediction/GPyS_prediction.py
--rw-rw-rw-   0        0        0       41 2023-07-20 16:07:58.000000 GPyS-0.0.31/src/GPyS_prediction/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 19:12:19.223455 GPyS-0.0.31/src/GPyS_preprocessor/
--rw-rw-rw-   0        0        0     2918 2023-07-22 15:57:37.000000 GPyS-0.0.31/src/GPyS_preprocessor/GPyS_preprocessor.py
--rw-rw-rw-   0        0        0       45 2023-07-20 16:07:58.000000 GPyS-0.0.31/src/GPyS_preprocessor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-20 16:07:58.000000 GPyS-0.0.31/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.498313 GPyS-0.0.32/
+drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.484312 GPyS-0.0.32/GPyS.egg-info/
+-rw-rw-rw-   0        0        0     1892 2023-07-25 23:51:37.000000 GPyS-0.0.32/GPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-07-25 23:51:37.000000 GPyS-0.0.32/GPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 23:51:37.000000 GPyS-0.0.32/GPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-25 23:51:37.000000 GPyS-0.0.32/GPyS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    34727 2023-07-20 16:07:58.000000 GPyS-0.0.32/LICENSE
+-rw-rw-rw-   0        0        0     1892 2023-07-25 23:51:37.498313 GPyS-0.0.32/PKG-INFO
+-rw-rw-rw-   0        0        0     1370 2023-07-22 19:21:04.000000 GPyS-0.0.32/README.md
+-rw-rw-rw-   0        0        0      758 2023-07-25 23:50:52.000000 GPyS-0.0.32/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 23:51:37.498313 GPyS-0.0.32/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.475214 GPyS-0.0.32/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.486344 GPyS-0.0.32/src/GPyS/
+-rw-rw-rw-   0        0        0        0 2023-07-20 16:07:58.000000 GPyS-0.0.32/src/GPyS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.489313 GPyS-0.0.32/src/GPyS_LOOCV_error/
+-rw-rw-rw-   0        0        0     9401 2023-07-22 18:45:07.000000 GPyS-0.0.32/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py
+-rw-rw-rw-   0        0        0       35 2023-07-20 16:07:58.000000 GPyS-0.0.32/src/GPyS_LOOCV_error/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.492312 GPyS-0.0.32/src/GPyS_prediction/
+-rw-rw-rw-   0        0        0    20190 2023-07-22 21:58:58.000000 GPyS-0.0.32/src/GPyS_prediction/GPyS_prediction.py
+-rw-rw-rw-   0        0        0       41 2023-07-20 16:07:58.000000 GPyS-0.0.32/src/GPyS_prediction/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.496313 GPyS-0.0.32/src/GPyS_preprocessor/
+-rw-rw-rw-   0        0        0     2918 2023-07-22 15:57:37.000000 GPyS-0.0.32/src/GPyS_preprocessor/GPyS_preprocessor.py
+-rw-rw-rw-   0        0        0       45 2023-07-20 16:07:58.000000 GPyS-0.0.32/src/GPyS_preprocessor/__init__.py
```

### Comparing `GPyS-0.0.31/LICENSE` & `GPyS-0.0.32/LICENSE`

 * *Files identical despite different names*

### Comparing `GPyS-0.0.31/PKG-INFO` & `GPyS-0.0.32/GPyS.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPyS
-Version: 0.0.31
+Version: 0.0.32
 Summary: Gaussian Process Subspace Prediction
 Author-email: "ZHANG, Ruda" <rudaz@Central.UH.EDU>, Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
 Project-URL: Homepage, https://github.com/UQUH/GPyS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -18,15 +18,15 @@
 
 - Ruda Zhang, Simon Mak, and David Dunson. Gaussian Process Subspace Prediction for Model Reduction. SIAM Journal on Scientific Computing, 2022. https://epubs.siam.org/doi/10.1137/21M1432739
 
 ## Installation
 
 Install the package via pip using the following command:
 
-- pip install GPyS==0.0.3
+- pip install GPyS==0.0.31
 
 ## Example Use 
 
 After installing the package you can load it via: 
 
 #### For GPS Preprocessor: 
   - from GPyS_preprocessor import Preprocessor
```

### Comparing `GPyS-0.0.31/README.md` & `GPyS-0.0.32/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 - Ruda Zhang, Simon Mak, and David Dunson. Gaussian Process Subspace Prediction for Model Reduction. SIAM Journal on Scientific Computing, 2022. https://epubs.siam.org/doi/10.1137/21M1432739
 
 ## Installation
 
 Install the package via pip using the following command:
 
-- pip install GPyS==0.0.3
+- pip install GPyS==0.0.31
 
 ## Example Use 
 
 After installing the package you can load it via: 
 
 #### For GPS Preprocessor: 
   - from GPyS_preprocessor import Preprocessor
```

### Comparing `GPyS-0.0.31/pyproject.toml` & `GPyS-0.0.32/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.packages]
+find = {}  # Scan the project directory with the default parameters
+
 [project]
 name = "GPyS"
-version = "0.0.31"
+version = "0.0.32"
 authors = [
   { name="ZHANG, Ruda", email="rudaz@Central.UH.EDU" },
   { name="Taiwo Adebiyi", email="taadebi2@cougarnet.uh.edu" },
 ]
 description = "Gaussian Process Subspace Prediction"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `GPyS-0.0.31/src/GPyS.egg-info/PKG-INFO` & `GPyS-0.0.32/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPyS
-Version: 0.0.31
+Version: 0.0.32
 Summary: Gaussian Process Subspace Prediction
 Author-email: "ZHANG, Ruda" <rudaz@Central.UH.EDU>, Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
 Project-URL: Homepage, https://github.com/UQUH/GPyS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -18,15 +18,15 @@
 
 - Ruda Zhang, Simon Mak, and David Dunson. Gaussian Process Subspace Prediction for Model Reduction. SIAM Journal on Scientific Computing, 2022. https://epubs.siam.org/doi/10.1137/21M1432739
 
 ## Installation
 
 Install the package via pip using the following command:
 
-- pip install GPyS==0.0.3
+- pip install GPyS==0.0.31
 
 ## Example Use 
 
 After installing the package you can load it via: 
 
 #### For GPS Preprocessor: 
   - from GPyS_preprocessor import Preprocessor
```

### Comparing `GPyS-0.0.31/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py` & `GPyS-0.0.32/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py`

 * *Files identical despite different names*

### Comparing `GPyS-0.0.31/src/GPyS_prediction/GPyS_prediction.py` & `GPyS-0.0.32/src/GPyS_prediction/GPyS_prediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TypeAlias, Union, Optional
 
 
 vector: TypeAlias = list[float]
 matrix: TypeAlias = list[vector]
 
 class Prediction(object):
-    """"
+    """
     ===============================================================
     GP Subspace Regression Prediction, Eigen-Decomposition Version
     ==============================================================
     Prediction module of the GPyS primarily computes the predictive distributions from a given set observations,
     target point, and established basis which have been preprocessed by the Preprocessor module of the GPyS package.
 
     The core method of the Prediction module is Prediction.GPS_prediction() function. By calling this method, the
```

### Comparing `GPyS-0.0.31/src/GPyS_preprocessor/GPyS_preprocessor.py` & `GPyS-0.0.32/src/GPyS_preprocessor/GPyS_preprocessor.py`

 * *Files identical despite different names*

