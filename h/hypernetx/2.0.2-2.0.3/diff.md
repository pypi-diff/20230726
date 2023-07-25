# Comparing `tmp/hypernetx-2.0.2.tar.gz` & `tmp/hypernetx-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypernetx-2.0.2.tar", last modified: Thu Jun 29 16:08:54 2023, max compression
+gzip compressed data, was "hypernetx-2.0.3.tar", last modified: Tue Jul 25 22:59:37 2023, max compression
```

## Comparing `hypernetx-2.0.2.tar` & `hypernetx-2.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.379040 hypernetx-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-29 16:08:45.000000 hypernetx-2.0.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-29 16:08:45.000000 hypernetx-2.0.2/LONG_DESCRIPTION.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-29 16:08:54.379040 hypernetx-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-06-29 16:08:45.000000 hypernetx-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.371040 hypernetx-2.0.2/hypernetx/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.371040 hypernetx-2.0.2/hypernetx/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40009 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/contagion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/generative_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    24275 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/homology_mod2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/hypergraph_modularity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/laplacians_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/algorithms/s_centrality_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.375040 hypernetx-2.0.2/hypernetx/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55664 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/classes/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    27383 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/classes/entityset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/classes/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    82331 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/classes/hypergraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.375040 hypernetx-2.0.2/hypernetx/drawing/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/drawing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/drawing/rubber_band.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/drawing/two_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/drawing/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/read_write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.375040 hypernetx-2.0.2/hypernetx/reports/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/reports/descriptive_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.375040 hypernetx-2.0.2/hypernetx/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/extras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.379040 hypernetx-2.0.2/hypernetx/utils/toys/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/toys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/toys/gene_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/toys/harrypotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/toys/lesmis.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-29 16:08:45.000000 hypernetx-2.0.2/hypernetx/utils/toys/transmission_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:08:54.371040 hypernetx-2.0.2/hypernetx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-29 16:08:54.000000 hypernetx-2.0.2/hypernetx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-29 16:08:54.000000 hypernetx-2.0.2/hypernetx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:08:54.000000 hypernetx-2.0.2/hypernetx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-29 16:08:54.000000 hypernetx-2.0.2/hypernetx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 16:08:54.000000 hypernetx-2.0.2/hypernetx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 16:08:45.000000 hypernetx-2.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-29 16:08:54.379040 hypernetx-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-29 16:08:45.000000 hypernetx-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:59:37.359034 hypernetx-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-25 22:59:28.000000 hypernetx-2.0.3/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-25 22:59:28.000000 hypernetx-2.0.3/LONG_DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-25 22:59:37.359034 hypernetx-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13839 2023-07-25 22:59:28.000000 hypernetx-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:59:37.355034 hypernetx-2.0.3/hypernetx/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:59:37.359034 hypernetx-2.0.3/hypernetx/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40009 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/algorithms/contagion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/algorithms/generative_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24275 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/algorithms/homology_mod2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/algorithms/hypergraph_modularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/algorithms/laplacians_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/algorithms/s_centrality_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:59:37.359034 hypernetx-2.0.3/hypernetx/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55664 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/classes/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27383 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/classes/entityset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/classes/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82642 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/classes/hypergraph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:59:37.359034 hypernetx-2.0.3/hypernetx/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/drawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/drawing/rubber_band.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/drawing/two_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/drawing/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/read_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:59:37.359034 hypernetx-2.0.3/hypernetx/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/reports/descriptive_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:59:37.359034 hypernetx-2.0.3/hypernetx/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/utils/extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:59:37.359034 hypernetx-2.0.3/hypernetx/utils/toys/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/utils/toys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/utils/toys/gene_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/utils/toys/harrypotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/utils/toys/lesmis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-25 22:59:28.000000 hypernetx-2.0.3/hypernetx/utils/toys/transmission_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:59:37.355034 hypernetx-2.0.3/hypernetx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-25 22:59:37.000000 hypernetx-2.0.3/hypernetx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-07-25 22:59:37.000000 hypernetx-2.0.3/hypernetx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:59:37.000000 hypernetx-2.0.3/hypernetx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-25 22:59:37.000000 hypernetx-2.0.3/hypernetx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 22:59:37.000000 hypernetx-2.0.3/hypernetx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-25 22:59:28.000000 hypernetx-2.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-25 22:59:37.359034 hypernetx-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-25 22:59:28.000000 hypernetx-2.0.3/setup.py
```

### Comparing `hypernetx-2.0.2/LICENSE.rst` & `hypernetx-2.0.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/LONG_DESCRIPTION.rst` & `hypernetx-2.0.3/LONG_DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/PKG-INFO` & `hypernetx-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypernetx
-Version: 2.0.2
+Version: 2.0.3
 Summary: HyperNetX is a Python library for the creation and study of hypergraphs.
 Home-page: https://github.com/pnnl/HyperNetX
 Author: Brenda Praggastis, Dustin Arendt, Sinan Aksoy, Emilie Purvine, Cliff Joslyn
 Author-email: hypernetx@pnnl.gov
 License: 3-Clause BSD license
 Description-Content-Type: text/x-rst
 Provides-Extra: releases
```

### Comparing `hypernetx-2.0.2/README.md` & `hypernetx-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/algorithms/__init__.py` & `hypernetx-2.0.3/hypernetx/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/algorithms/contagion.py` & `hypernetx-2.0.3/hypernetx/algorithms/contagion.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/algorithms/generative_models.py` & `hypernetx-2.0.3/hypernetx/algorithms/generative_models.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/algorithms/homology_mod2.py` & `hypernetx-2.0.3/hypernetx/algorithms/homology_mod2.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/algorithms/hypergraph_modularity.py` & `hypernetx-2.0.3/hypernetx/algorithms/hypergraph_modularity.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/algorithms/laplacians_clustering.py` & `hypernetx-2.0.3/hypernetx/algorithms/laplacians_clustering.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/algorithms/s_centrality_measures.py` & `hypernetx-2.0.3/hypernetx/algorithms/s_centrality_measures.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/classes/entity.py` & `hypernetx-2.0.3/hypernetx/classes/entity.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/classes/entityset.py` & `hypernetx-2.0.3/hypernetx/classes/entityset.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/classes/helpers.py` & `hypernetx-2.0.3/hypernetx/classes/helpers.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/classes/hypergraph.py` & `hypernetx-2.0.3/hypernetx/classes/hypergraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # All rights reserved.
 from __future__ import annotations
 
 import pickle
 import warnings
 from collections import defaultdict
 from collections.abc import Sequence, Iterable
-from typing import Optional, Any, TypeVar, Union, Mapping
+from typing import Optional, Any, TypeVar, Union, Mapping, Hashable
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 from networkx.algorithms import bipartite
 from scipy.sparse import coo_matrix, csr_matrix
 
@@ -1509,57 +1509,65 @@
     def remove(self, keys, level=None, name=None):
         """Creates a new hypergraph with nodes and/or edges indexed by keys
         removed. More efficient for creating a restricted hypergraph if the
         restricted set is greater than what is being removed.
 
         Parameters
         ----------
-        keys : list | tuple | set
-            node and/or edge id to restrict to
+        keys : list | tuple | set | Hashable
+            node and/or edge id(s) to restrict to
         level : None, optional
             Enter 0 to remove edges with ids in keys.
             Enter 1 to remove nodes with ids in keys.
             If None then all objects in nodes and edges with the id will
             be removed.
+        name : str, optional
+            Name of new hypergraph
 
         Returns
         -------
         : hnx.Hypergraph
 
         """
         rdfprop = self.properties.copy()
         rdf = self.dataframe.copy()
-        if not isinstance(keys, (list, tuple, set)):
-            keys = list(keys)
+        if isinstance(keys, (list, tuple, set)):
+            nkeys = keys
+        elif isinstance(keys, Hashable):
+            nkeys = list()
+            nkeys.append(keys)
+        else:
+            raise TypeError("`keys` parameter must be list | tuple | set | Hashable")
         if level == 0:
-            kdx = set(keys).intersection(set(self._state_dict["labels"]["edges"]))
+            kdx = set(nkeys).intersection(set(self._state_dict["labels"]["edges"]))
             for k in kdx:
                 rdfprop = rdfprop.drop((0, k))
-            rdf = rdf.loc[~rdf[self._edge_col].isin(kdx)]
+            rdf = rdf.loc[~(rdf[self._edge_col].isin(kdx))]
         elif level == 1:
-            kdx = set(keys).intersection(set(self._state_dict["labels"]["nodes"]))
+            kdx = set(nkeys).intersection(set(self._state_dict["labels"]["nodes"]))
             for k in kdx:
                 rdfprop = rdfprop.drop((1, k))
-            rdf = rdf.loc[~rdf[self._node_col].isin(kdx)]
+            rdf = rdf.loc[~(rdf[self._node_col].isin(kdx))]
         else:
             rdfprop = rdfprop.reset_index()
-            kdx = set(keys).intersection(rdfprop.id.unique())
+            kdx = set(nkeys).intersection(rdfprop.id.unique())
             rdfprop = rdfprop.set_index("id")
             rdfprop = rdfprop.drop(index=kdx)
-            rdf = rdf.loc[~rdf[self._edge_col].isin(kdx)]
-            rdf = rdf.loc[~rdf[self._node_col].isin(kdx)]
+            rdf = rdf.loc[~(rdf[self._edge_col].isin(kdx))]
+            rdf = rdf.loc[~(rdf[self._node_col].isin(kdx))]
 
         return Hypergraph(
             setsystem=rdf,
             edge_col=self._edge_col,
             node_col=self._node_col,
             cell_weight_col=self._cell_weight_col,
             misc_cell_properties_col=self.edges._misc_cell_props_col,
             properties=rdfprop,
             misc_properties_col=self.edges._misc_props_col,
+            name=name
         )
 
     def toplexes(self, name=None):
         """
         Returns a :term:`simple hypergraph` corresponding to self.
 
         Warning
```

### Comparing `hypernetx-2.0.2/hypernetx/drawing/rubber_band.py` & `hypernetx-2.0.3/hypernetx/drawing/rubber_band.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/drawing/two_column.py` & `hypernetx-2.0.3/hypernetx/drawing/two_column.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/drawing/util.py` & `hypernetx-2.0.3/hypernetx/drawing/util.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/exception.py` & `hypernetx-2.0.3/hypernetx/exception.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/reports/descriptive_stats.py` & `hypernetx-2.0.3/hypernetx/reports/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/utils/__init__.py` & `hypernetx-2.0.3/hypernetx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/utils/decorators.py` & `hypernetx-2.0.3/hypernetx/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/utils/extras.py` & `hypernetx-2.0.3/hypernetx/utils/extras.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/utils/log.py` & `hypernetx-2.0.3/hypernetx/utils/log.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/utils/toys/harrypotter.py` & `hypernetx-2.0.3/hypernetx/utils/toys/harrypotter.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/utils/toys/lesmis.py` & `hypernetx-2.0.3/hypernetx/utils/toys/lesmis.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx/utils/toys/transmission_problem.py` & `hypernetx-2.0.3/hypernetx/utils/toys/transmission_problem.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx.egg-info/PKG-INFO` & `hypernetx-2.0.3/hypernetx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypernetx
-Version: 2.0.2
+Version: 2.0.3
 Summary: HyperNetX is a Python library for the creation and study of hypergraphs.
 Home-page: https://github.com/pnnl/HyperNetX
 Author: Brenda Praggastis, Dustin Arendt, Sinan Aksoy, Emilie Purvine, Cliff Joslyn
 Author-email: hypernetx@pnnl.gov
 License: 3-Clause BSD license
 Description-Content-Type: text/x-rst
 Provides-Extra: releases
```

### Comparing `hypernetx-2.0.2/hypernetx.egg-info/SOURCES.txt` & `hypernetx-2.0.3/hypernetx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/hypernetx.egg-info/requires.txt` & `hypernetx-2.0.3/hypernetx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hypernetx-2.0.2/setup.cfg` & `hypernetx-2.0.3/setup.cfg`

 * *Files identical despite different names*

