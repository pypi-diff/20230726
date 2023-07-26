# Comparing `tmp/annb-0.1.1.tar.gz` & `tmp/annb-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annb-0.1.1.tar", last modified: Wed Jul 26 03:21:25 2023, max compression
+gzip compressed data, was "annb-0.1.2.tar", last modified: Wed Jul 26 03:42:07 2023, max compression
```

## Comparing `annb-0.1.1.tar` & `annb-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:21:25.133608 annb-0.1.1/
--rw-r--r--   0 jibin      (501) staff       (20)    11357 2023-06-23 11:24:40.000000 annb-0.1.1/LICENSE
--rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-26 03:21:25.133694 annb-0.1.1/PKG-INFO
--rw-r--r--   0 jibin      (501) staff       (20)      297 2023-07-25 03:49:16.000000 annb-0.1.1/README.md
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:21:25.130932 annb-0.1.1/annb/
--rw-r--r--   0 jibin      (501) staff       (20)      385 2023-07-26 03:20:38.000000 annb-0.1.1/annb/__init__.py
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:21:25.128669 annb-0.1.1/annb/anns/
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:21:25.132318 annb-0.1.1/annb/anns/faiss/
--rw-r--r--   0 jibin      (501) staff       (20)      489 2023-06-23 14:28:30.000000 annb-0.1.1/annb/anns/faiss/deploy.py
--rw-r--r--   0 jibin      (501) staff       (20)     3284 2023-07-25 03:07:57.000000 annb-0.1.1/annb/anns/faiss/indexes.py
--rw-r--r--   0 jibin      (501) staff       (20)     9413 2023-07-26 03:19:49.000000 annb-0.1.1/annb/cli.py
--rw-r--r--   0 jibin      (501) staff       (20)     1853 2023-07-25 03:08:09.000000 annb-0.1.1/annb/config.py
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:21:25.133391 annb-0.1.1/annb/dataset/
--rw-r--r--   0 jibin      (501) staff       (20)      213 2023-07-25 03:44:19.000000 annb-0.1.1/annb/dataset/__init__.py
--rw-r--r--   0 jibin      (501) staff       (20)     1267 2023-07-25 03:08:09.000000 annb-0.1.1/annb/dataset/base_dataset.py
--rw-r--r--   0 jibin      (501) staff       (20)     6734 2023-07-25 03:08:09.000000 annb-0.1.1/annb/dataset/hdf5_dataset.py
--rw-r--r--   0 jibin      (501) staff       (20)     1946 2023-07-25 03:08:09.000000 annb-0.1.1/annb/dataset/random_dataset.py
--rw-r--r--   0 jibin      (501) staff       (20)     2416 2023-07-25 03:08:09.000000 annb-0.1.1/annb/dataset/utils.py
--rw-r--r--   0 jibin      (501) staff       (20)       75 2023-06-23 13:33:53.000000 annb-0.1.1/annb/envs.py
--rw-r--r--   0 jibin      (501) staff       (20)     7929 2023-07-25 03:08:09.000000 annb-0.1.1/annb/indexes.py
--rw-r--r--   0 jibin      (501) staff       (20)     1431 2023-07-25 03:07:57.000000 annb-0.1.1/annb/plot.py
--rw-r--r--   0 jibin      (501) staff       (20)     6405 2023-07-25 03:08:09.000000 annb-0.1.1/annb/result.py
--rw-r--r--   0 jibin      (501) staff       (20)     7718 2023-07-25 03:07:57.000000 annb-0.1.1/annb/runner.py
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:21:25.131961 annb-0.1.1/annb.egg-info/
--rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-26 03:21:25.000000 annb-0.1.1/annb.egg-info/PKG-INFO
--rw-r--r--   0 jibin      (501) staff       (20)      517 2023-07-26 03:21:25.000000 annb-0.1.1/annb.egg-info/SOURCES.txt
--rw-r--r--   0 jibin      (501) staff       (20)        1 2023-07-26 03:21:25.000000 annb-0.1.1/annb.egg-info/dependency_links.txt
--rw-r--r--   0 jibin      (501) staff       (20)       84 2023-07-26 03:21:25.000000 annb-0.1.1/annb.egg-info/entry_points.txt
--rw-r--r--   0 jibin      (501) staff       (20)       49 2023-07-26 03:21:25.000000 annb-0.1.1/annb.egg-info/requires.txt
--rw-r--r--   0 jibin      (501) staff       (20)        5 2023-07-26 03:21:25.000000 annb-0.1.1/annb.egg-info/top_level.txt
--rw-r--r--   0 jibin      (501) staff       (20)       99 2023-07-25 03:07:57.000000 annb-0.1.1/pyproject.toml
--rw-r--r--   0 jibin      (501) staff       (20)      668 2023-07-26 03:21:25.133985 annb-0.1.1/setup.cfg
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.324287 annb-0.1.2/
+-rw-r--r--   0 jibin      (501) staff       (20)    11357 2023-06-23 11:24:40.000000 annb-0.1.2/LICENSE
+-rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-26 03:42:07.324397 annb-0.1.2/PKG-INFO
+-rw-r--r--   0 jibin      (501) staff       (20)      297 2023-07-25 03:49:16.000000 annb-0.1.2/README.md
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.320634 annb-0.1.2/annb/
+-rw-r--r--   0 jibin      (501) staff       (20)      385 2023-07-26 03:41:45.000000 annb-0.1.2/annb/__init__.py
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.318123 annb-0.1.2/annb/anns/
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.322253 annb-0.1.2/annb/anns/faiss/
+-rw-r--r--   0 jibin      (501) staff       (20)      489 2023-06-23 14:28:30.000000 annb-0.1.2/annb/anns/faiss/deploy.py
+-rw-r--r--   0 jibin      (501) staff       (20)     3595 2023-07-26 03:41:08.000000 annb-0.1.2/annb/anns/faiss/indexes.py
+-rw-r--r--   0 jibin      (501) staff       (20)     9413 2023-07-26 03:19:49.000000 annb-0.1.2/annb/cli.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1853 2023-07-25 03:08:09.000000 annb-0.1.2/annb/config.py
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.324035 annb-0.1.2/annb/dataset/
+-rw-r--r--   0 jibin      (501) staff       (20)      213 2023-07-25 03:44:19.000000 annb-0.1.2/annb/dataset/__init__.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1267 2023-07-25 03:08:09.000000 annb-0.1.2/annb/dataset/base_dataset.py
+-rw-r--r--   0 jibin      (501) staff       (20)     6734 2023-07-25 03:08:09.000000 annb-0.1.2/annb/dataset/hdf5_dataset.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1946 2023-07-25 03:08:09.000000 annb-0.1.2/annb/dataset/random_dataset.py
+-rw-r--r--   0 jibin      (501) staff       (20)     2416 2023-07-25 03:08:09.000000 annb-0.1.2/annb/dataset/utils.py
+-rw-r--r--   0 jibin      (501) staff       (20)       75 2023-06-23 13:33:53.000000 annb-0.1.2/annb/envs.py
+-rw-r--r--   0 jibin      (501) staff       (20)     7996 2023-07-26 03:37:36.000000 annb-0.1.2/annb/indexes.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1431 2023-07-25 03:07:57.000000 annb-0.1.2/annb/plot.py
+-rw-r--r--   0 jibin      (501) staff       (20)     6405 2023-07-25 03:08:09.000000 annb-0.1.2/annb/result.py
+-rw-r--r--   0 jibin      (501) staff       (20)     7718 2023-07-25 03:07:57.000000 annb-0.1.2/annb/runner.py
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.321696 annb-0.1.2/annb.egg-info/
+-rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/PKG-INFO
+-rw-r--r--   0 jibin      (501) staff       (20)      517 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/SOURCES.txt
+-rw-r--r--   0 jibin      (501) staff       (20)        1 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/dependency_links.txt
+-rw-r--r--   0 jibin      (501) staff       (20)       84 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/entry_points.txt
+-rw-r--r--   0 jibin      (501) staff       (20)       49 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/requires.txt
+-rw-r--r--   0 jibin      (501) staff       (20)        5 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/top_level.txt
+-rw-r--r--   0 jibin      (501) staff       (20)       99 2023-07-25 03:07:57.000000 annb-0.1.2/pyproject.toml
+-rw-r--r--   0 jibin      (501) staff       (20)      668 2023-07-26 03:42:07.324710 annb-0.1.2/setup.cfg
```

### Comparing `annb-0.1.1/LICENSE` & `annb-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/PKG-INFO` & `annb-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple ANN benchmark tools
 Home-page: https://github.com/matrixji/annb
 Author: Ji Bin
 Author-email: matrixji@live.com
 License: Apache-2.0
 Keywords: ANN benchmark,Test tools
 Requires-Python: >=3.6
```

### Comparing `annb-0.1.1/annb/anns/faiss/indexes.py` & `annb-0.1.2/annb/anns/faiss/indexes.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,74 +13,82 @@
 
     def create_index(self) -> Union[faiss.Index, None]:
         faiss_metric = (
             faiss.METRIC_L2
             if self.metric_type == MetricType.L2
             else faiss.METRIC_INNER_PRODUCT
         )
-        using_gpu = str(self.kwargs.get('gpu', 'no')).lower() in [
-            'yes',
-            'true',
-            '1',
-            'on',
+        using_gpu = str(self.kwargs.get("gpu", "no")).lower() in [
+            "yes",
+            "true",
+            "1",
+            "on",
         ]
-        index_string = self.kwargs.get('index', 'flat')
+        index_string = self.kwargs.get("index", "flat")
         index = None
-        if index_string == 'flat':
+        if index_string == "flat":
             index = faiss.IndexFlat(self.dimension, faiss_metric)
-        elif index_string == 'ivfflat':
+        elif index_string == "ivfflat":
             quantizer = faiss.IndexFlat(self.dimension, faiss_metric)
             index = faiss.IndexIVFFlat(
-                quantizer, self.dimension, self.kwargs.get('nlist', 128), faiss_metric
+                quantizer, self.dimension, self.kwargs.get("nlist", 128), faiss_metric
             )
-        elif index_string == 'ivfpq':
+        elif index_string == "ivfpq":
             quantizer = faiss.IndexFlat(self.dimension, faiss_metric)
             index = faiss.IndexIVFPQ(
                 quantizer,
                 self.dimension,
-                self.kwargs.get('nlist', 128),
-                self.kwargs.get('m', 8),
-                self.kwargs.get('nbits', 8),
+                self.kwargs.get("nlist", 128),
+                self.kwargs.get("m", 8),
+                self.kwargs.get("nbits", 8),
             )
-        elif index_string == 'ivfsq':
+        elif index_string == "ivfsq":
             quantizer = faiss.IndexFlat(self.dimension, faiss_metric)
             index = faiss.IndexIVFScalarQuantizer(
                 quantizer,
                 self.dimension,
-                self.kwargs.get('nlist', 128),
+                self.kwargs.get("nlist", 128),
                 faiss.ScalarQuantizer.QT_8bit,
             )
         else:
             index = faiss.index_factory(self.dimension, index_string, faiss_metric)
         if (
             using_gpu
-            and hasattr(faiss, 'index_cpu_to_gpu')
-            and hasattr(faiss, 'StandardGpuResources')
+            and hasattr(faiss, "index_cpu_to_gpu")
+            and hasattr(faiss, "StandardGpuResources")
         ):
+            self.log.debug("copy index to gpu")
             index = faiss.index_cpu_to_gpu(faiss.StandardGpuResources(), 0, index)
+        else:
+            self.log.debug(
+                "use cpu index, gpu: %s, faiss has gpu support: %s",
+                using_gpu,
+                hasattr(faiss, "index_cpu_to_gpu")
+                and hasattr(faiss, "StandardGpuResources"),
+            )
         return index
 
     def train(self, data: np.ndarray) -> None:
         return self.index.train(data)
 
     def add(self, data: np.ndarray) -> None:
         return self.index.add(data)
 
     def warmup(self) -> None:
         for _ in range(3):
-            random_data = np.random.rand(10, self.dimension).astype('float32')
+            random_data = np.random.rand(10, self.dimension).astype("float32")
             random_data /= np.linalg.norm(random_data, axis=1)[:, None]
             self.search(random_data, 10)
 
     def search(self, query: np.ndarray, k: int) -> Tuple[List[float], List[int]]:
         return self.index.search(query, k)
 
     def update_search_args(self, **kwargs):
-        if 'nprobe' in kwargs:
-            self.index.nprobe = kwargs['nprobe']
+        if "nprobe" in kwargs:
+            self.index.nprobe = kwargs["nprobe"]
 
     def cleanup(self) -> None:
         self.index.reset()
 
 
 class FaissIndexUnderTestFactory(IndexUnderTestFactory):
     def create(
```

### Comparing `annb-0.1.1/annb/cli.py` & `annb-0.1.2/annb/cli.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/annb/config.py` & `annb-0.1.2/annb/config.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/annb/dataset/base_dataset.py` & `annb-0.1.2/annb/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/annb/dataset/hdf5_dataset.py` & `annb-0.1.2/annb/dataset/hdf5_dataset.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/annb/dataset/random_dataset.py` & `annb-0.1.2/annb/dataset/random_dataset.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/annb/dataset/utils.py` & `annb-0.1.2/annb/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/annb/indexes.py` & `annb-0.1.2/annb/indexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Tuple, List, Union, Dict
 from hashlib import sha1
+from logging import getLogger
 
 import numpy as np
 from .envs import get_run_dir
 
 
 class MetricType(Enum):
     INNER_PRODUCT = 1
@@ -41,14 +42,15 @@
         :param dimension: Dimension of the index.
         :param metric_type: Metric type of the index.
         """
         self.name = index_name
         self.dimension = dimension
         self.metric_type = metric_type
         self.kwargs = kwargs
+        self.log = getLogger('annb')
 
     def verify(self) -> bool:
         """
         Verify the index.
         :return: True if the index is valid, False otherwise.
 
         This method is used to verify that the index is valid.
```

### Comparing `annb-0.1.1/annb/plot.py` & `annb-0.1.2/annb/plot.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/annb/result.py` & `annb-0.1.2/annb/result.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/annb/runner.py` & `annb-0.1.2/annb/runner.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/annb.egg-info/PKG-INFO` & `annb-0.1.2/annb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annb
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple ANN benchmark tools
 Home-page: https://github.com/matrixji/annb
 Author: Ji Bin
 Author-email: matrixji@live.com
 License: Apache-2.0
 Keywords: ANN benchmark,Test tools
 Requires-Python: >=3.6
```

### Comparing `annb-0.1.1/annb.egg-info/SOURCES.txt` & `annb-0.1.2/annb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `annb-0.1.1/setup.cfg` & `annb-0.1.2/setup.cfg`

 * *Files identical despite different names*

