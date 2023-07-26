# Comparing `tmp/torchist-0.2.0.tar.gz` & `tmp/torchist-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchist-0.2.0.tar", last modified: Fri Mar  3 10:09:27 2023, max compression
+gzip compressed data, was "torchist-0.2.1.tar", last modified: Wed Jul 26 14:48:56 2023, max compression
```

## Comparing `torchist-0.2.0.tar` & `torchist-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-03-03 10:09:27.150418 torchist-0.2.0/
--rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2023-03-02 18:15:36.000000 torchist-0.2.0/LICENSE
--rw-rw-r--   0 francois  (1001) francois  (1001)     2408 2023-03-03 10:09:27.150418 torchist-0.2.0/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)     1781 2023-03-03 10:00:25.000000 torchist-0.2.0/README.md
--rw-rw-r--   0 francois  (1001) francois  (1001)      721 2023-03-03 10:09:27.150418 torchist-0.2.0/setup.cfg
--rw-rw-r--   0 francois  (1001) francois  (1001)       61 2023-03-02 18:38:57.000000 torchist-0.2.0/setup.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-03-03 10:09:27.150418 torchist-0.2.0/torchist/
--rw-rw-r--   0 francois  (1001) francois  (1001)    12762 2023-03-03 09:57:59.000000 torchist-0.2.0/torchist/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1001)     4140 2023-03-03 09:51:10.000000 torchist-0.2.0/torchist/metrics.py
-drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-03-03 10:09:27.150418 torchist-0.2.0/torchist.egg-info/
--rw-rw-r--   0 francois  (1001) francois  (1001)     2408 2023-03-03 10:09:27.000000 torchist-0.2.0/torchist.egg-info/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1001)      236 2023-03-03 10:09:27.000000 torchist-0.2.0/torchist.egg-info/SOURCES.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-03-03 10:09:27.000000 torchist-0.2.0/torchist.egg-info/dependency_links.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)       13 2023-03-03 10:09:27.000000 torchist-0.2.0/torchist.egg-info/requires.txt
--rw-rw-r--   0 francois  (1001) francois  (1001)        9 2023-03-03 10:09:27.000000 torchist-0.2.0/torchist.egg-info/top_level.txt
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-26 14:48:56.673467 torchist-0.2.1/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1072 2023-07-26 14:18:37.000000 torchist-0.2.1/LICENSE
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2317 2023-07-26 14:48:56.673467 torchist-0.2.1/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)     1762 2023-07-26 14:45:09.000000 torchist-0.2.1/README.md
+-rw-rw-r--   0 francois  (1001) francois  (1001)       13 2023-07-26 14:18:37.000000 torchist-0.2.1/requirements.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)      659 2023-07-26 14:48:56.673467 torchist-0.2.1/setup.cfg
+-rw-rw-r--   0 francois  (1001) francois  (1001)       76 2023-07-26 14:18:37.000000 torchist-0.2.1/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-26 14:48:56.669467 torchist-0.2.1/torchist/
+-rw-rw-r--   0 francois  (1001) francois  (1001)    12765 2023-07-26 14:46:59.000000 torchist-0.2.1/torchist/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1001)     4140 2023-07-26 14:19:58.000000 torchist-0.2.1/torchist/metrics.py
+drwxrwxr-x   0 francois  (1001) francois  (1001)        0 2023-07-26 14:48:56.673467 torchist-0.2.1/torchist.egg-info/
+-rw-rw-r--   0 francois  (1001) francois  (1001)     2317 2023-07-26 14:48:56.000000 torchist-0.2.1/torchist.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1001)      253 2023-07-26 14:48:56.000000 torchist-0.2.1/torchist.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        1 2023-07-26 14:48:56.000000 torchist-0.2.1/torchist.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)       13 2023-07-26 14:48:56.000000 torchist-0.2.1/torchist.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1001) francois  (1001)        9 2023-07-26 14:48:56.000000 torchist-0.2.1/torchist.egg-info/top_level.txt
```

### Comparing `torchist-0.2.0/LICENSE` & `torchist-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torchist-0.2.0/PKG-INFO` & `torchist-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: torchist
-Version: 0.2.0
+Version: 0.2.1
 Summary: NumPy-style histograms in PyTorch
 Home-page: https://github.com/francois-rozet/torchist
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
-License: MIT License
 Keywords: torch,histogram
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NumPy-style histograms in PyTorch
 
-The `torchist` package implements NumPy's [`histogram`](https://numpy.org/doc/stable/reference/generated/numpy.histogram.html) and [`histogramdd`](https://numpy.org/doc/stable/reference/generated/numpy.histogramdd.html) functions in PyTorch with support for non-uniform binning. The package also features implementations of [`ravel_multi_index`](https://numpy.org/doc/stable/reference/generated/numpy.ravel_multi_index.html), [`unravel_index`](https://numpy.org/doc/stable/reference/generated/numpy.unravel_index.html) and some useful functionals like `entropy` or `kl_divergence`.
+The `torchist` package implements NumPy's [`histogram`](https://numpy.org/doc/stable/reference/generated/numpy.histogram.html) and [`histogramdd`](https://numpy.org/doc/stable/reference/generated/numpy.histogramdd.html) functions in PyTorch with CUDA support. The package also features implementations of [`ravel_multi_index`](https://numpy.org/doc/stable/reference/generated/numpy.ravel_multi_index.html), [`unravel_index`](https://numpy.org/doc/stable/reference/generated/numpy.unravel_index.html) and some useful functionals like `entropy` or `kl_divergence`.
 
 ## Installation
 
 The `torchist` package is available on [PyPI](https://pypi.org/project/torchist), which means it is installable with `pip`.
 
 ```
 pip install torchist
```

### Comparing `torchist-0.2.0/README.md` & `torchist-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # NumPy-style histograms in PyTorch
 
-The `torchist` package implements NumPy's [`histogram`](https://numpy.org/doc/stable/reference/generated/numpy.histogram.html) and [`histogramdd`](https://numpy.org/doc/stable/reference/generated/numpy.histogramdd.html) functions in PyTorch with support for non-uniform binning. The package also features implementations of [`ravel_multi_index`](https://numpy.org/doc/stable/reference/generated/numpy.ravel_multi_index.html), [`unravel_index`](https://numpy.org/doc/stable/reference/generated/numpy.unravel_index.html) and some useful functionals like `entropy` or `kl_divergence`.
+The `torchist` package implements NumPy's [`histogram`](https://numpy.org/doc/stable/reference/generated/numpy.histogram.html) and [`histogramdd`](https://numpy.org/doc/stable/reference/generated/numpy.histogramdd.html) functions in PyTorch with CUDA support. The package also features implementations of [`ravel_multi_index`](https://numpy.org/doc/stable/reference/generated/numpy.ravel_multi_index.html), [`unravel_index`](https://numpy.org/doc/stable/reference/generated/numpy.unravel_index.html) and some useful functionals like `entropy` or `kl_divergence`.
 
 ## Installation
 
 The `torchist` package is available on [PyPI](https://pypi.org/project/torchist), which means it is installable with `pip`.
 
 ```
 pip install torchist
```

### Comparing `torchist-0.2.0/setup.cfg` & `torchist-0.2.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 version = attr: torchist.__version__
 description = NumPy-style histograms in PyTorch
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = torch, histogram
 author = François Rozet
 author_email = francois.rozet@outlook.com
-license = MIT License
 url = https://github.com/francois-rozet/torchist
 classifiers = 
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
-	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 
 [options]
 packages = find:
 python_requires = >=3.6
```

### Comparing `torchist-0.2.0/torchist/__init__.py` & `torchist-0.2.1/torchist/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 r"""NumPy-style histograms in PyTorch"""
 
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 import torch
 
 from torch import Size, Tensor, BoolTensor
 from typing import *
 
 
@@ -77,15 +77,15 @@
 
     Returns:
         The quantized tensor, (*, D).
     """
 
     x = (x - low) / (upp - low)  # in [0.0, 1.0]
     x = (bins * x).long()  # in [0, bins]
-    x = torch.clip(x, min=0, max=bins - 1)  # in [0, bins)
+    x = torch.clip(x, min=None, max=bins - 1)  # in [0, bins)
 
     return x
 
 
 def histogramdd(
     x: Tensor,
     bins: Union[int, Sequence[int]] = 10,
@@ -145,20 +145,20 @@
         pack = x.new_full((D, max(bins) + 1), float('inf'))
 
         for i, e in enumerate(edges):
             pack[i, :e.numel()] = e.to(x)  # pad with inf
 
         edges = pack
 
-    assert torch.all(upp > low), "The upper bound must be strictly larger than the lower bound"
-
     bins = torch.as_tensor(bins).squeeze().long()
     low = torch.as_tensor(low).squeeze().to(x)
     upp = torch.as_tensor(upp).squeeze().to(x)
 
+    assert torch.all(upp > low), "The upper bound must be strictly larger than the lower bound"
+
     if weights is not None:
         weights = weights.flatten()
 
     # Filter out-of-bound values
     if not bounded:
         mask = ~out_of_bounds(x, low, upp)
```

### Comparing `torchist-0.2.0/torchist/metrics.py` & `torchist-0.2.1/torchist/metrics.py`

 * *Files identical despite different names*

### Comparing `torchist-0.2.0/torchist.egg-info/PKG-INFO` & `torchist-0.2.1/torchist.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: torchist
-Version: 0.2.0
+Version: 0.2.1
 Summary: NumPy-style histograms in PyTorch
 Home-page: https://github.com/francois-rozet/torchist
 Author: François Rozet
 Author-email: francois.rozet@outlook.com
-License: MIT License
 Keywords: torch,histogram
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NumPy-style histograms in PyTorch
 
-The `torchist` package implements NumPy's [`histogram`](https://numpy.org/doc/stable/reference/generated/numpy.histogram.html) and [`histogramdd`](https://numpy.org/doc/stable/reference/generated/numpy.histogramdd.html) functions in PyTorch with support for non-uniform binning. The package also features implementations of [`ravel_multi_index`](https://numpy.org/doc/stable/reference/generated/numpy.ravel_multi_index.html), [`unravel_index`](https://numpy.org/doc/stable/reference/generated/numpy.unravel_index.html) and some useful functionals like `entropy` or `kl_divergence`.
+The `torchist` package implements NumPy's [`histogram`](https://numpy.org/doc/stable/reference/generated/numpy.histogram.html) and [`histogramdd`](https://numpy.org/doc/stable/reference/generated/numpy.histogramdd.html) functions in PyTorch with CUDA support. The package also features implementations of [`ravel_multi_index`](https://numpy.org/doc/stable/reference/generated/numpy.ravel_multi_index.html), [`unravel_index`](https://numpy.org/doc/stable/reference/generated/numpy.unravel_index.html) and some useful functionals like `entropy` or `kl_divergence`.
 
 ## Installation
 
 The `torchist` package is available on [PyPI](https://pypi.org/project/torchist), which means it is installable with `pip`.
 
 ```
 pip install torchist
```

