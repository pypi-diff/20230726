# Comparing `tmp/bci-essentials-0.0.5.tar.gz` & `tmp/bci-essentials-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bci-essentials-0.0.5.tar", last modified: Thu Jul 13 15:36:20 2023, max compression
+gzip compressed data, was "bci-essentials-0.0.6.tar", last modified: Wed Jul 26 17:15:28 2023, max compression
```

## Comparing `bci-essentials-0.0.5.tar` & `bci-essentials-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:36:20.403694 bci-essentials-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-13 15:33:40.000000 bci-essentials-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-13 15:36:20.403694 bci-essentials-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-13 15:33:40.000000 bci-essentials-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:36:20.399694 bci-essentials-0.0.5/bci_essentials/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-13 15:33:40.000000 bci-essentials-0.0.5/bci_essentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71000 2023-07-13 15:33:40.000000 bci-essentials-0.0.5/bci_essentials/bci_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-07-13 15:33:40.000000 bci-essentials-0.0.5/bci_essentials/channel_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    54254 2023-07-13 15:33:40.000000 bci-essentials-0.0.5/bci_essentials/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-07-13 15:33:40.000000 bci-essentials-0.0.5/bci_essentials/resting_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-07-13 15:33:40.000000 bci-essentials-0.0.5/bci_essentials/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-13 15:33:40.000000 bci-essentials-0.0.5/bci_essentials/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 15:36:20.403694 bci-essentials-0.0.5/bci_essentials.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-13 15:36:20.000000 bci-essentials-0.0.5/bci_essentials.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-13 15:36:20.000000 bci-essentials-0.0.5/bci_essentials.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 15:36:20.000000 bci-essentials-0.0.5/bci_essentials.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-13 15:36:20.000000 bci-essentials-0.0.5/bci_essentials.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-13 15:36:20.000000 bci-essentials-0.0.5/bci_essentials.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-13 15:33:41.000000 bci-essentials-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 15:36:20.403694 bci-essentials-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:15:28.592472 bci-essentials-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-26 17:15:28.592472 bci-essentials-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:15:28.588472 bci-essentials-0.0.6/bci_essentials/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71000 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/bci_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16414 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/channel_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:15:28.588472 bci-essentials-0.0.6/bci_essentials/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/classification/erp_rg_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/classification/generic_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/classification/mi_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/classification/null_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/classification/ssvep_basic_tf_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/classification/ssvep_riemannian_mdm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/classification/switch_deep_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/classification/switch_mdm_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/resting_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/bci_essentials/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:15:28.588472 bci-essentials-0.0.6/bci_essentials.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-07-26 17:15:28.000000 bci-essentials-0.0.6/bci_essentials.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-26 17:15:28.000000 bci-essentials-0.0.6/bci_essentials.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:15:28.000000 bci-essentials-0.0.6/bci_essentials.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-26 17:15:28.000000 bci-essentials-0.0.6/bci_essentials.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-26 17:15:28.000000 bci-essentials-0.0.6/bci_essentials.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:15:28.592472 bci-essentials-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:15:28.588472 bci-essentials-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/tests/test_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-26 17:12:53.000000 bci-essentials-0.0.6/tests/test_smoke.py
```

### Comparing `bci-essentials-0.0.5/LICENSE` & `bci-essentials-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.5/PKG-INFO` & `bci-essentials-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bci-essentials
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python backend for bci-essentials
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bci-essentials-python
 This repository contains python modules and scripts for the processing of EEG-based BCI.
```

### Comparing `bci-essentials-0.0.5/README.md` & `bci-essentials-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.5/bci_essentials/bci_data.py` & `bci-essentials-0.0.6/bci_essentials/bci_data.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.5/bci_essentials/channel_selection.py` & `bci-essentials-0.0.6/bci_essentials/channel_selection.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.5/bci_essentials/resting_state.py` & `bci-essentials-0.0.6/bci_essentials/resting_state.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.5/bci_essentials/signal_processing.py` & `bci-essentials-0.0.6/bci_essentials/signal_processing.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 # For decision blocks
 # Inputs are N x M x P where N = number of channels, M = number of samples, and P = number of possible selections
 # Outputs are the same dimensions
 
 import numpy as np
 from scipy import signal
+import random
 
 import matplotlib.pyplot as plt
 
 # 
 
 # def common_average_reference(data):
 #     N,M,P = np.shape(data)
@@ -209,7 +210,47 @@
         return new_data
         
     except:
         N, M = np.shape(data)
         new_data = np.ndarray(shape=(N, M), dtype=float) 
         new_data = signal.filtfilt(b, a, data, axis=1, padlen=30)
         return new_data
+    
+def lico(X,y,expansion_factor=3, sum_num=2, shuffle=False):
+
+    """Oversampling (linear combination oversampling (LiCO))
+
+    Samples random linear combinations of existing epochs of X.
+
+    Parameters
+    ----------
+    X : numpy array 
+        The file location of the spreadsheet
+    y : numpy array
+        A flag used to print the columns to the console
+    expansion_factor : int, optional
+        Number of times larger to make the output set over_X (default is 3)
+    sum_num : int, optional
+        Number of signals to be summed together (default is 2)
+
+    Returns
+    -------
+    over_X : numpy array
+        oversampled X
+    over_y : numpy array
+        oversampled y
+    """
+
+    true_X = X[y == 1]
+
+    n,m,p = true_X.shape
+    print("Shape of ERPs only ", true_X.shape)
+    new_n = n*np.round(expansion_factor-1)
+    new_X = np.zeros([new_n,m,p])
+    for i in range(n):
+        for j in range(sum_num):
+            new_X[i,:,:] += true_X[random.choice(range(n)),:,:] / sum_num
+
+    over_X = np.append(X,new_X,axis=0)
+    over_y = np.append(y,np.ones([new_n]))
+
+    return over_X, over_y
```

### Comparing `bci-essentials-0.0.5/bci_essentials/visuals.py` & `bci-essentials-0.0.6/bci_essentials/visuals.py`

 * *Files identical despite different names*

### Comparing `bci-essentials-0.0.5/bci_essentials.egg-info/PKG-INFO` & `bci-essentials-0.0.6/bci_essentials.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bci-essentials
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python backend for bci-essentials
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # bci-essentials-python
 This repository contains python modules and scripts for the processing of EEG-based BCI.
```

### Comparing `bci-essentials-0.0.5/pyproject.toml` & `bci-essentials-0.0.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bci-essentials"
-version = "0.0.5"
+version = "0.0.6"
 description = "Python backend for bci-essentials"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
 	"numpy",
 	"scipy",
 	"scikit-learn",
```

