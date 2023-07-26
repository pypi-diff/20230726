# Comparing `tmp/golfy-2.3.0.tar.gz` & `tmp/golfy-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golfy-2.3.0.tar", last modified: Sun Jul 16 21:55:25 2023, max compression
+gzip compressed data, was "golfy-2.4.0.tar", last modified: Wed Jul 26 20:09:56 2023, max compression
```

## Comparing `golfy-2.3.0.tar` & `golfy-2.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-16 21:55:25.321959 golfy-2.3.0/
--rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-2.3.0/LICENSE
--rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-16 21:55:25.321832 golfy-2.3.0/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)     4495 2023-07-13 19:03:02.000000 golfy-2.3.0/README.md
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-16 21:55:25.319290 golfy-2.3.0/golfy/
--rw-r--r--   0 iskander   (501) staff       (20)      927 2023-07-16 21:53:56.000000 golfy-2.3.0/golfy/__init__.py
--rw-r--r--   0 iskander   (501) staff       (20)     3938 2023-07-13 18:48:59.000000 golfy-2.3.0/golfy/deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)     5061 2023-07-13 16:16:32.000000 golfy-2.3.0/golfy/design.py
--rw-r--r--   0 iskander   (501) staff       (20)     2455 2023-07-13 19:55:22.000000 golfy-2.3.0/golfy/evaluation.py
--rw-r--r--   0 iskander   (501) staff       (20)    18118 2023-07-13 15:48:47.000000 golfy-2.3.0/golfy/initialization.py
--rw-r--r--   0 iskander   (501) staff       (20)     9826 2023-07-16 21:53:51.000000 golfy-2.3.0/golfy/main.py
--rw-r--r--   0 iskander   (501) staff       (20)     6800 2023-07-13 15:14:16.000000 golfy-2.3.0/golfy/merging.py
--rw-r--r--   0 iskander   (501) staff       (20)    11264 2023-07-13 15:14:16.000000 golfy-2.3.0/golfy/optimization.py
--rw-r--r--   0 iskander   (501) staff       (20)     3912 2023-07-13 15:40:22.000000 golfy-2.3.0/golfy/simulation.py
--rw-r--r--   0 iskander   (501) staff       (20)      322 2023-07-13 15:17:57.000000 golfy-2.3.0/golfy/types.py
--rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-2.3.0/golfy/util.py
--rw-r--r--   0 iskander   (501) staff       (20)     3622 2023-07-13 15:14:16.000000 golfy-2.3.0/golfy/validity.py
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-16 21:55:25.319876 golfy-2.3.0/golfy.egg-info/
--rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-16 21:55:25.000000 golfy-2.3.0/golfy.egg-info/PKG-INFO
--rw-r--r--   0 iskander   (501) staff       (20)      582 2023-07-16 21:55:25.000000 golfy-2.3.0/golfy.egg-info/SOURCES.txt
--rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-16 21:55:25.000000 golfy-2.3.0/golfy.egg-info/dependency_links.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-16 21:55:25.000000 golfy-2.3.0/golfy.egg-info/requires.txt
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-16 21:55:25.000000 golfy-2.3.0/golfy.egg-info/top_level.txt
--rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-2.3.0/pyproject.toml
--rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-2.3.0/requirements.txt
--rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-16 21:55:25.321994 golfy-2.3.0/setup.cfg
-drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-16 21:55:25.321555 golfy-2.3.0/tests/
--rw-r--r--   0 iskander   (501) staff       (20)      250 2023-07-13 17:27:57.000000 golfy-2.3.0/tests/test_best_design_for_pool_budget.py
--rw-r--r--   0 iskander   (501) staff       (20)     1104 2023-07-13 18:24:30.000000 golfy-2.3.0/tests/test_deconvolution.py
--rw-r--r--   0 iskander   (501) staff       (20)      528 2023-07-13 15:17:29.000000 golfy-2.3.0/tests/test_find_best_design.py
--rw-r--r--   0 iskander   (501) staff       (20)     2226 2023-07-12 20:38:24.000000 golfy-2.3.0/tests/test_init.py
--rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-2.3.0/tests/test_optimize.py
--rw-r--r--   0 iskander   (501) staff       (20)      965 2023-07-13 15:38:34.000000 golfy-2.3.0/tests/test_simulation.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-26 20:09:56.155284 golfy-2.4.0/
+-rw-r--r--   0 iskander   (501) staff       (20)    11357 2023-06-29 21:40:41.000000 golfy-2.4.0/LICENSE
+-rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-26 20:09:56.155149 golfy-2.4.0/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)     4495 2023-07-13 19:03:02.000000 golfy-2.4.0/README.md
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-26 20:09:56.152430 golfy-2.4.0/golfy/
+-rw-r--r--   0 iskander   (501) staff       (20)      927 2023-07-26 20:05:56.000000 golfy-2.4.0/golfy/__init__.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3938 2023-07-13 18:48:59.000000 golfy-2.4.0/golfy/deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)     5061 2023-07-13 16:16:32.000000 golfy-2.4.0/golfy/design.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2549 2023-07-24 21:50:40.000000 golfy-2.4.0/golfy/evaluation.py
+-rw-r--r--   0 iskander   (501) staff       (20)    19478 2023-07-26 20:05:52.000000 golfy-2.4.0/golfy/initialization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     9826 2023-07-21 14:15:49.000000 golfy-2.4.0/golfy/main.py
+-rw-r--r--   0 iskander   (501) staff       (20)     6800 2023-07-13 15:14:16.000000 golfy-2.4.0/golfy/merging.py
+-rw-r--r--   0 iskander   (501) staff       (20)    11264 2023-07-24 21:23:13.000000 golfy-2.4.0/golfy/optimization.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3912 2023-07-13 15:40:22.000000 golfy-2.4.0/golfy/simulation.py
+-rw-r--r--   0 iskander   (501) staff       (20)      322 2023-07-21 14:15:22.000000 golfy-2.4.0/golfy/types.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1149 2023-07-07 14:26:57.000000 golfy-2.4.0/golfy/util.py
+-rw-r--r--   0 iskander   (501) staff       (20)     3622 2023-07-13 15:14:16.000000 golfy-2.4.0/golfy/validity.py
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-26 20:09:56.153157 golfy-2.4.0/golfy.egg-info/
+-rw-r--r--   0 iskander   (501) staff       (20)     5221 2023-07-26 20:09:56.000000 golfy-2.4.0/golfy.egg-info/PKG-INFO
+-rw-r--r--   0 iskander   (501) staff       (20)      582 2023-07-26 20:09:56.000000 golfy-2.4.0/golfy.egg-info/SOURCES.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        1 2023-07-26 20:09:56.000000 golfy-2.4.0/golfy.egg-info/dependency_links.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-26 20:09:56.000000 golfy-2.4.0/golfy.egg-info/requires.txt
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-26 20:09:56.000000 golfy-2.4.0/golfy.egg-info/top_level.txt
+-rw-r--r--   0 iskander   (501) staff       (20)      863 2023-07-10 19:33:19.000000 golfy-2.4.0/pyproject.toml
+-rw-r--r--   0 iskander   (501) staff       (20)        6 2023-07-07 15:53:33.000000 golfy-2.4.0/requirements.txt
+-rw-r--r--   0 iskander   (501) staff       (20)       38 2023-07-26 20:09:56.155318 golfy-2.4.0/setup.cfg
+drwxr-xr-x   0 iskander   (501) staff       (20)        0 2023-07-26 20:09:56.154760 golfy-2.4.0/tests/
+-rw-r--r--   0 iskander   (501) staff       (20)      250 2023-07-13 17:27:57.000000 golfy-2.4.0/tests/test_best_design_for_pool_budget.py
+-rw-r--r--   0 iskander   (501) staff       (20)     1104 2023-07-13 18:24:30.000000 golfy-2.4.0/tests/test_deconvolution.py
+-rw-r--r--   0 iskander   (501) staff       (20)      528 2023-07-13 15:17:29.000000 golfy-2.4.0/tests/test_find_best_design.py
+-rw-r--r--   0 iskander   (501) staff       (20)     2561 2023-07-26 20:06:54.000000 golfy-2.4.0/tests/test_init.py
+-rw-r--r--   0 iskander   (501) staff       (20)      207 2023-07-12 20:37:32.000000 golfy-2.4.0/tests/test_optimize.py
+-rw-r--r--   0 iskander   (501) staff       (20)      965 2023-07-13 15:38:34.000000 golfy-2.4.0/tests/test_simulation.py
```

### Comparing `golfy-2.3.0/LICENSE` & `golfy-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/PKG-INFO` & `golfy-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 2.3.0
+Version: 2.4.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-2.3.0/README.md` & `golfy-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/golfy/__init__.py` & `golfy-2.4.0/golfy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     simulate_elispot_counts,
     simulate_any_hits_per_pool,
     simulate_number_hits_per_pool,
 )
 from .types import SpotCounts
 from .validity import is_valid, count_violations, violations_per_replicate
 
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 
 __all__ = [
     "__version__",
     "find_best_design",
     "best_design_for_pool_budget",
     "Design",
     "init",
```

### Comparing `golfy-2.3.0/golfy/deconvolution.py` & `golfy-2.4.0/golfy/deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/golfy/design.py` & `golfy-2.4.0/golfy/design.py`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/golfy/evaluation.py` & `golfy-2.4.0/golfy/evaluation.py`

 * *Files 11% similar despite different names*

```diff
@@ -70,9 +70,11 @@
             rs.append(recall)
             f1s.append(f1)
     return EvaluationResult(
         precision=np.mean(ps),
         recall=np.mean(rs),
         f1=np.mean(f1s),
         num_pools=s.num_pools(),
-        num_violations=count_violations(s),
+        num_violations=count_violations(
+            s, error_on_duplicate=False, error_on_extra=False, error_on_missing=False
+        ),
     )
```

### Comparing `golfy-2.3.0/golfy/initialization.py` & `golfy-2.4.0/golfy/initialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,50 @@
             max_peptides_per_pool = num_pools_first_replicate
             result[replicate_idx] = int(np.ceil(num_peptides / max_peptides_per_pool))
         else:
             result[replicate_idx] = num_pools_first_replicate
     return result
 
 
+def _repeat_init(
+    num_peptides: int,
+    max_peptides_per_pool: int,
+    num_replicates: int,
+    num_pools_per_replicate: dict[Replicate, int],
+    invalid_neighbors: PeptidePairList = [],
+    preferred_neighbors: PeptidePairList = [],
+    allow_extra_pools: bool = False,
+    verbose: bool = False,
+):
+    """
+    Assign peptides to random blocks and then repeat those blocks r times
+    """
+    replicate_to_pool_to_peptides = {}
+    for i in range(num_replicates):
+        peptide_array = np.arange(num_peptides)
+        np.random.shuffle(peptide_array)
+        pool_assignments = {}
+        num_pools = num_pools_per_replicate[i]
+        peptides_per_pool = int(np.ceil(num_peptides / num_pools))
+        for j in range(num_pools):
+            start_idx = peptides_per_pool * j
+            end_idx = peptides_per_pool * (j + 1)
+            pool_assignments[j] = peptide_array[start_idx:end_idx]
+        replicate_to_pool_to_peptides[i] = pool_assignments
+    return Design(
+        num_peptides=num_peptides,
+        max_peptides_per_pool=max_peptides_per_pool,
+        num_replicates=num_replicates,
+        invalid_neighbors=invalid_neighbors,
+        preferred_neighbors=preferred_neighbors,
+        assignments=replicate_to_pool_to_peptides,
+        allow_extra_pools=allow_extra_pools,
+    )
+
+
 def _random_peptide_order(
     num_peptides: int, peptide_to_preferred: dict[Peptide, set[Peptide]]
 ):
     """
     Return the peptide indices in a random order but make sure the ones with preferred neighbors are first
     """
     random_peptide_order = np.arange(num_peptides)
@@ -383,15 +419,15 @@
 def init(
     num_peptides: int = 100,
     max_peptides_per_pool: int = 5,
     num_replicates: int = 3,
     num_pools_per_replicate: Optional[int | dict[Replicate, int]] = None,
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
-    strategy: Literal["greedy", "random", "valid", "singleton"] = "greedy",
+    strategy: Literal["greedy", "random", "valid", "singleton", "repeat"] = "greedy",
     allow_extra_pools: bool = False,
     verbose: bool = False,
 ) -> Design:
     """
     Initialize a Solution for a given configuration
 
     Args
@@ -411,27 +447,28 @@
     invalid_neighbors
         list of peptide pairs that cannot be in the same pool
 
     preferred_neighbors
         list of peptide pairs that should be in the same pool
 
     strategy
-        initialization strategy, one of {"greedy", "random", "singleton", "valid"} (default: "greedy")
+        initialization strategy, one of {"greedy", "random", "singleton", "valid", "repeat"} (default: "greedy")
 
     allow_extra_pools
         whether to allow extra pools to be created to satisfy constraints (default: False)
 
     verbose
         print diagnostic information during initialization (default: False)
     """
     fn = {
         "greedy": _greedy_init,
         "random": _random_init,
         "singleton": _singleton_init,
         "valid": _valid_init,
+        "repeat": _repeat_init,
     }.get(strategy)
     if num_pools_per_replicate is None:
         num_pools_per_replicate = _pools_per_replicate(
             num_peptides=num_peptides,
             max_peptides_per_pool=max_peptides_per_pool,
             num_replicates=num_replicates,
             allow_extra_pools=allow_extra_pools,
```

### Comparing `golfy-2.3.0/golfy/main.py` & `golfy-2.4.0/golfy/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,16 +234,16 @@
 def best_design_for_pool_budget(
     num_peptides: int = 100,
     max_pools: int = 96,
     num_simulation_iters: int = 3,
     invalid_neighbors: PeptidePairList = [],
     preferred_neighbors: PeptidePairList = [],
     min_pools: Optional[int] = None,
-    min_num_replicates: int = 2,
-    max_num_replicates: int = 5,
+    min_num_replicates: int = 3,
+    max_num_replicates: int = 8,
     min_max_peptides_per_pool: int = 2,
     max_max_peptides_per_pool: Optional[int] = None,
     verbose: bool = False,
 ):
     assert num_peptides > 1, "No need to pool if there's only one peptide"
     assert max_pools > 1, "Must have more than one pool"
     assert max_pools <= num_peptides, "Can't have more pools than peptides"
```

### Comparing `golfy-2.3.0/golfy/merging.py` & `golfy-2.4.0/golfy/merging.py`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/golfy/optimization.py` & `golfy-2.4.0/golfy/optimization.py`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/golfy/simulation.py` & `golfy-2.4.0/golfy/simulation.py`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/golfy/util.py` & `golfy-2.4.0/golfy/util.py`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/golfy/validity.py` & `golfy-2.4.0/golfy/validity.py`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/golfy.egg-info/PKG-INFO` & `golfy-2.4.0/golfy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golfy
-Version: 2.3.0
+Version: 2.4.0
 Summary: Heuristic peptide pool optimization for ELISpot and other immunological assays
 Author-email: Alex Rubinsteyn <alex.rubinsteyn@unc.edu>
 Project-URL: Homepage, https://github.com/pirl-unc/golfy
 Project-URL: Bug Tracker, https://github.com/pirl-unc/golfy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
```

### Comparing `golfy-2.3.0/golfy.egg-info/SOURCES.txt` & `golfy-2.4.0/golfy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/pyproject.toml` & `golfy-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/tests/test_deconvolution.py` & `golfy-2.4.0/tests/test_deconvolution.py`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/tests/test_find_best_design.py` & `golfy-2.4.0/tests/test_find_best_design.py`

 * *Files identical despite different names*

### Comparing `golfy-2.3.0/tests/test_init.py` & `golfy-2.4.0/tests/test_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from golfy import init
+from golfy import init, count_violations
 
 
 def test_valid_init():
     s = init(
         num_peptides=100, max_peptides_per_pool=5, num_replicates=3, strategy="valid"
     )
     assert len(s.assignments) == 3
@@ -67,7 +67,19 @@
     peptide_to_pool = s.peptide_to_pool_dict_for_replicate(0)
     print(peptide_to_pool)
 
     assert peptide_to_pool[7] == peptide_to_pool[10]
     assert peptide_to_pool[12] == peptide_to_pool[17]
     assert peptide_to_pool[14] == peptide_to_pool[15]
     assert peptide_to_pool[15] == peptide_to_pool[17]
+
+
+def test_repeat_block_init():
+    s = init(
+        num_peptides=100, max_peptides_per_pool=5, num_replicates=3, strategy="repeat"
+    )
+
+    assert len(s.assignments) == 3
+    assert len(s.assignments[0]) == 20
+    assert len(s.assignments[0][0]) == 5
+
+    assert count_violations(s, error_on_duplicate=False) > 0
```

### Comparing `golfy-2.3.0/tests/test_simulation.py` & `golfy-2.4.0/tests/test_simulation.py`

 * *Files identical despite different names*

