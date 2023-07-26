# Comparing `tmp/GPyS-0.1.0.tar.gz` & `tmp/GPyS-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPyS-0.1.0.tar", last modified: Wed Jul 26 01:54:35 2023, max compression
+gzip compressed data, was "GPyS-0.1.1.tar", last modified: Wed Jul 26 02:23:21 2023, max compression
```

## Comparing `GPyS-0.1.0.tar` & `GPyS-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.708012 GPyS-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.695092 GPyS-0.1.0/GPyS/
-drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.701012 GPyS-0.1.0/GPyS/GPyS_LOOCV_error/
--rw-rw-rw-   0        0        0     9401 2023-07-22 18:45:07.000000 GPyS-0.1.0/GPyS/GPyS_LOOCV_error/GPyS_LOOCV_error.py
--rw-rw-rw-   0        0        0       35 2023-07-20 16:07:58.000000 GPyS-0.1.0/GPyS/GPyS_LOOCV_error/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.704012 GPyS-0.1.0/GPyS/GPyS_prediction/
--rw-rw-rw-   0        0        0    20190 2023-07-22 21:58:58.000000 GPyS-0.1.0/GPyS/GPyS_prediction/GPyS_prediction.py
--rw-rw-rw-   0        0        0       41 2023-07-20 16:07:58.000000 GPyS-0.1.0/GPyS/GPyS_prediction/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.706012 GPyS-0.1.0/GPyS/GPyS_preprocessor/
--rw-rw-rw-   0        0        0     2918 2023-07-22 15:57:37.000000 GPyS-0.1.0/GPyS/GPyS_preprocessor/GPyS_preprocessor.py
--rw-rw-rw-   0        0        0       45 2023-07-20 16:07:58.000000 GPyS-0.1.0/GPyS/GPyS_preprocessor/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-20 16:07:58.000000 GPyS-0.1.0/GPyS/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 01:54:35.699010 GPyS-0.1.0/GPyS.egg-info/
--rw-rw-rw-   0        0        0     1868 2023-07-26 01:54:35.000000 GPyS-0.1.0/GPyS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-26 01:54:35.000000 GPyS-0.1.0/GPyS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 01:54:35.000000 GPyS-0.1.0/GPyS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-26 01:54:35.000000 GPyS-0.1.0/GPyS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1868 2023-07-26 01:54:35.707012 GPyS-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1370 2023-07-22 19:21:04.000000 GPyS-0.1.0/README.md
--rw-rw-rw-   0        0        0      758 2023-07-26 01:45:38.000000 GPyS-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 01:54:35.708012 GPyS-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 02:23:21.038338 GPyS-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-26 02:23:21.010277 GPyS-0.1.1/GPyS/
+drwxrwxrwx   0        0        0        0 2023-07-26 02:23:21.025319 GPyS-0.1.1/GPyS/GPyS_LOOCV_error/
+-rw-rw-rw-   0        0        0     9411 2023-07-26 02:13:49.000000 GPyS-0.1.1/GPyS/GPyS_LOOCV_error/GPyS_LOOCV_error.py
+-rw-rw-rw-   0        0        0       35 2023-07-20 16:07:58.000000 GPyS-0.1.1/GPyS/GPyS_LOOCV_error/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 02:23:21.030320 GPyS-0.1.1/GPyS/GPyS_prediction/
+-rw-rw-rw-   0        0        0    20195 2023-07-26 02:13:49.000000 GPyS-0.1.1/GPyS/GPyS_prediction/GPyS_prediction.py
+-rw-rw-rw-   0        0        0       41 2023-07-20 16:07:58.000000 GPyS-0.1.1/GPyS/GPyS_prediction/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 02:23:21.035314 GPyS-0.1.1/GPyS/GPyS_preprocessor/
+-rw-rw-rw-   0        0        0     2918 2023-07-22 15:57:37.000000 GPyS-0.1.1/GPyS/GPyS_preprocessor/GPyS_preprocessor.py
+-rw-rw-rw-   0        0        0       45 2023-07-20 16:07:58.000000 GPyS-0.1.1/GPyS/GPyS_preprocessor/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-20 16:07:58.000000 GPyS-0.1.1/GPyS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 02:23:21.020312 GPyS-0.1.1/GPyS.egg-info/
+-rw-rw-rw-   0        0        0     1868 2023-07-26 02:23:20.000000 GPyS-0.1.1/GPyS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-26 02:23:20.000000 GPyS-0.1.1/GPyS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 02:23:20.000000 GPyS-0.1.1/GPyS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-26 02:23:20.000000 GPyS-0.1.1/GPyS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1868 2023-07-26 02:23:21.037318 GPyS-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1370 2023-07-22 19:21:04.000000 GPyS-0.1.1/README.md
+-rw-rw-rw-   0        0        0      758 2023-07-26 02:22:57.000000 GPyS-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 02:23:21.039276 GPyS-0.1.1/setup.cfg
```

### Comparing `GPyS-0.1.0/GPyS/GPyS_LOOCV_error/GPyS_LOOCV_error.py` & `GPyS-0.1.1/GPyS/GPyS_LOOCV_error/GPyS_LOOCV_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 
-from GPyS_preprocessor import Preprocessor
-from GPyS_prediction import Prediction as Pred
+from GPyS.GPyS_preprocessor import Preprocessor
+from GPyS.GPyS_prediction import Prediction as Pred
 
 
 import numpy as np
 import scipy
 import scipy.linalg as la
 from typing import TypeAlias, Union, Optional
```

### Comparing `GPyS-0.1.0/GPyS/GPyS_prediction/GPyS_prediction.py` & `GPyS-0.1.1/GPyS/GPyS_prediction/GPyS_prediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy
 import numpy as np
 import scipy
 import scipy.linalg as la
 
-from GPyS_preprocessor import Preprocessor
+from GPyS.GPyS_preprocessor import Preprocessor
 from typing import TypeAlias, Union, Optional
 
 
 vector: TypeAlias = list[float]
 matrix: TypeAlias = list[vector]
 
 class Prediction(object):
```

### Comparing `GPyS-0.1.0/GPyS/GPyS_preprocessor/GPyS_preprocessor.py` & `GPyS-0.1.1/GPyS/GPyS_preprocessor/GPyS_preprocessor.py`

 * *Files identical despite different names*

### Comparing `GPyS-0.1.0/GPyS.egg-info/PKG-INFO` & `GPyS-0.1.1/GPyS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPyS
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gaussian Process Subspace Prediction
 Author-email: "ZHANG, Ruda" <rudaz@Central.UH.EDU>, Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
 Project-URL: Homepage, https://github.com/UQUH/GPyS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `GPyS-0.1.0/PKG-INFO` & `GPyS-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPyS
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gaussian Process Subspace Prediction
 Author-email: "ZHANG, Ruda" <rudaz@Central.UH.EDU>, Taiwo Adebiyi <taadebi2@cougarnet.uh.edu>
 Project-URL: Homepage, https://github.com/UQUH/GPyS
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `GPyS-0.1.0/README.md` & `GPyS-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `GPyS-0.1.0/pyproject.toml` & `GPyS-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [project]
 name = "GPyS"
-version = "0.1.00"
+version = "0.1.01"
 authors = [
   { name="ZHANG, Ruda", email="rudaz@Central.UH.EDU" },
   { name="Taiwo Adebiyi", email="taadebi2@cougarnet.uh.edu" },
 ]
 description = "Gaussian Process Subspace Prediction"
 readme = "README.md"
 requires-python = ">=3.6"
```

