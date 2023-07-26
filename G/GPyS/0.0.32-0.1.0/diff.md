# Comparing `tmp/GPyS-0.0.32.tar.gz` & `tmp/GPyS-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPyS-0.0.32.tar", last modified: Tue Jul 25 23:51:37 2023, max compression
+gzip compressed data, was "GPyS-0.1.0.tar", last modified: Wed Jul 26 01:54:35 2023, max compression
```

## Comparing `GPyS-0.0.32.tar` & `GPyS-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.498313 GPyS-0.0.32/
-drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.484312 GPyS-0.0.32/GPyS.egg-info/
--rw-rw-rw-   0        0        0     1892 2023-07-25 23:51:37.000000 GPyS-0.0.32/GPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-07-25 23:51:37.000000 GPyS-0.0.32/GPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 23:51:37.000000 GPyS-0.0.32/GPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 23:51:37.000000 GPyS-0.0.32/GPyS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    34727 2023-07-20 16:07:58.000000 GPyS-0.0.32/LICENSE
--rw-rw-rw-   0        0        0     1892 2023-07-25 23:51:37.498313 GPyS-0.0.32/PKG-INFO
--rw-rw-rw-   0        0        0     1370 2023-07-22 19:21:04.000000 GPyS-0.0.32/README.md
--rw-rw-rw-   0        0        0      758 2023-07-25 23:50:52.000000 GPyS-0.0.32/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 23:51:37.498313 GPyS-0.0.32/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.475214 GPyS-0.0.32/src/
-drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.486344 GPyS-0.0.32/src/GPyS/
--rw-rw-rw-   0        0        0        0 2023-07-20 16:07:58.000000 GPyS-0.0.32/src/GPyS/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.489313 GPyS-0.0.32/src/GPyS_LOOCV_error/
--rw-rw-rw-   0        0        0     9401 2023-07-22 18:45:07.000000 GPyS-0.0.32/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py
--rw-rw-rw-   0        0        0       35 2023-07-20 16:07:58.000000 GPyS-0.0.32/src/GPyS_LOOCV_error/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.492312 GPyS-0.0.32/src/GPyS_prediction/
--rw-rw-rw-   0        0        0    20190 2023-07-22 21:58:58.000000 GPyS-0.0.32/src/GPyS_prediction/GPyS_prediction.py
--rw-rw-rw-   0        0        0       41 2023-07-20 16:07:58.000000 GPyS-0.0.32/src/GPyS_prediction/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 23:51:37.496313 GPyS-0.0.32/src/GPyS_preprocessor/
--rw-rw-rw-   0        0        0     2918 2023-07-22 15:57:37.000000 GPyS-0.0.32/src/GPyS_preprocessor/GPyS_preprocessor.py
--rw-rw-rw-   0        0        0       45 2023-07-20 16:07:58.000000 GPyS-0.0.32/src/GPyS_preprocessor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.708012 GPyS-0.1.0/
+drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.695092 GPyS-0.1.0/GPyS/
+drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.701012 GPyS-0.1.0/GPyS/GPyS_LOOCV_error/
+-rw-rw-rw-   0        0        0     9401 2023-07-22 18:45:07.000000 GPyS-0.1.0/GPyS/GPyS_LOOCV_error/GPyS_LOOCV_error.py
+-rw-rw-rw-   0        0        0       35 2023-07-20 16:07:58.000000 GPyS-0.1.0/GPyS/GPyS_LOOCV_error/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.704012 GPyS-0.1.0/GPyS/GPyS_prediction/
+-rw-rw-rw-   0        0        0    20190 2023-07-22 21:58:58.000000 GPyS-0.1.0/GPyS/GPyS_prediction/GPyS_prediction.py
+-rw-rw-rw-   0        0        0       41 2023-07-20 16:07:58.000000 GPyS-0.1.0/GPyS/GPyS_prediction/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.706012 GPyS-0.1.0/GPyS/GPyS_preprocessor/
+-rw-rw-rw-   0        0        0     2918 2023-07-22 15:57:37.000000 GPyS-0.1.0/GPyS/GPyS_preprocessor/GPyS_preprocessor.py
+-rw-rw-rw-   0        0        0       45 2023-07-20 16:07:58.000000 GPyS-0.1.0/GPyS/GPyS_preprocessor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-20 16:07:58.000000 GPyS-0.1.0/GPyS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.699010 GPyS-0.1.0/GPyS.egg-info/
+-rw-rw-rw-   0        0        0     1868 2023-07-26 01:54:35.000000 GPyS-0.1.0/GPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-26 01:54:35.000000 GPyS-0.1.0/GPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 01:54:35.000000 GPyS-0.1.0/GPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-26 01:54:35.000000 GPyS-0.1.0/GPyS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1868 2023-07-26 01:54:35.707012 GPyS-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1370 2023-07-22 19:21:04.000000 GPyS-0.1.0/README.md
+-rw-rw-rw-   0        0        0      758 2023-07-26 01:45:38.000000 GPyS-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 01:54:35.708012 GPyS-0.1.0/setup.cfg
```

### Comparing `GPyS-0.0.32/GPyS.egg-info/PKG-INFO` & `GPyS-0.1.0/GPyS.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: GPyS
-Version: 0.0.32
+Version: 0.1.0
 Summary: Gaussian Process Subspace Prediction
 Author-email: "ZHANG, Ruda" <rudaz@Central.UH.EDU>, Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
 Project-URL: Homepage, https://github.com/UQUH/GPyS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 This is a prototypical implementation of GPS in the Python programming language. 
 For the original research article documenting the method, see the Citation section.
 
 ## Citation
 
 - Ruda Zhang, Simon Mak, and David Dunson. Gaussian Process Subspace Prediction for Model Reduction. SIAM Journal on Scientific Computing, 2022. https://epubs.siam.org/doi/10.1137/21M1432739
```

### Comparing `GPyS-0.0.32/PKG-INFO` & `GPyS-0.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: GPyS
-Version: 0.0.32
+Version: 0.1.0
 Summary: Gaussian Process Subspace Prediction
 Author-email: "ZHANG, Ruda" <rudaz@Central.UH.EDU>, Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
 Project-URL: Homepage, https://github.com/UQUH/GPyS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 This is a prototypical implementation of GPS in the Python programming language. 
 For the original research article documenting the method, see the Citation section.
 
 ## Citation
 
 - Ruda Zhang, Simon Mak, and David Dunson. Gaussian Process Subspace Prediction for Model Reduction. SIAM Journal on Scientific Computing, 2022. https://epubs.siam.org/doi/10.1137/21M1432739
```

### Comparing `GPyS-0.0.32/README.md` & `GPyS-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `GPyS-0.0.32/src/GPyS_LOOCV_error/GPyS_LOOCV_error.py` & `GPyS-0.1.0/GPyS/GPyS_LOOCV_error/GPyS_LOOCV_error.py`

 * *Files identical despite different names*

### Comparing `GPyS-0.0.32/src/GPyS_prediction/GPyS_prediction.py` & `GPyS-0.1.0/GPyS/GPyS_prediction/GPyS_prediction.py`

 * *Files identical despite different names*

### Comparing `GPyS-0.0.32/src/GPyS_preprocessor/GPyS_preprocessor.py` & `GPyS-0.1.0/GPyS/GPyS_preprocessor/GPyS_preprocessor.py`

 * *Files identical despite different names*

