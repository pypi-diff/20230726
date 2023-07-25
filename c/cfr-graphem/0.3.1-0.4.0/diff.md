# Comparing `tmp/cfr-graphem-0.3.1.tar.gz` & `tmp/cfr-graphem-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-graphem-0.3.1.tar", last modified: Tue Jul 25 22:08:00 2023, max compression
+gzip compressed data, was "cfr-graphem-0.4.0.tar", last modified: Tue Jul 25 22:20:19 2023, max compression
```

## Comparing `cfr-graphem-0.3.1.tar` & `cfr-graphem-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-25 22:08:00.891713 cfr-graphem-0.3.1/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)      706 2023-07-25 22:08:00.891542 cfr-graphem-0.3.1/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      215 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/README.rst
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-25 22:08:00.888929 cfr-graphem-0.3.1/cfr_graphem.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)      706 2023-07-25 22:08:00.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      370 2023-07-25 22:08:00.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-07-25 22:08:00.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-02-11 12:40:30.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-07-25 22:08:00.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       16 2023-07-25 22:08:00.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/top_level.txt
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-25 22:08:00.891105 cfr-graphem-0.3.1/graphem/
--rwxr-xr-x   0 fengzhu    (502) staff       (20)     9952 2023-06-22 23:58:14.000000 cfr-graphem-0.3.1/graphem/GraphEstimation.py
--rwxr-xr-x   0 fengzhu    (502) staff       (20)    15228 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/graphem/QUIC.cpp
--rwxr-xr-x   0 fengzhu    (502) staff       (20)     1709 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/graphem/QUIC.py
--rw-r--r--   0 fengzhu    (502) staff       (20)       52 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/graphem/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    13086 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/graphem/graph.py
--rwxr-xr-x   0 fengzhu    (502) staff       (20)     5846 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/graphem/iridge.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    28846 2023-07-25 22:04:10.000000 cfr-graphem-0.3.1/graphem/solver.py
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-07-25 22:08:00.891756 cfr-graphem-0.3.1/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1452 2023-07-25 22:04:31.000000 cfr-graphem-0.3.1/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-25 22:20:19.196283 cfr-graphem-0.4.0/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2023-02-11 11:26:13.000000 cfr-graphem-0.4.0/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)      706 2023-07-25 22:20:19.196135 cfr-graphem-0.4.0/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      215 2023-02-11 11:26:13.000000 cfr-graphem-0.4.0/README.rst
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-25 22:20:19.193399 cfr-graphem-0.4.0/cfr_graphem.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      706 2023-07-25 22:20:19.000000 cfr-graphem-0.4.0/cfr_graphem.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      370 2023-07-25 22:20:19.000000 cfr-graphem-0.4.0/cfr_graphem.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-07-25 22:20:19.000000 cfr-graphem-0.4.0/cfr_graphem.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-02-11 12:40:30.000000 cfr-graphem-0.4.0/cfr_graphem.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-07-25 22:20:19.000000 cfr-graphem-0.4.0/cfr_graphem.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       16 2023-07-25 22:20:19.000000 cfr-graphem-0.4.0/cfr_graphem.egg-info/top_level.txt
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-25 22:20:19.195817 cfr-graphem-0.4.0/graphem/
+-rwxr-xr-x   0 fengzhu    (502) staff       (20)     9952 2023-06-22 23:58:14.000000 cfr-graphem-0.4.0/graphem/GraphEstimation.py
+-rwxr-xr-x   0 fengzhu    (502) staff       (20)    15228 2023-02-11 11:26:13.000000 cfr-graphem-0.4.0/graphem/QUIC.cpp
+-rwxr-xr-x   0 fengzhu    (502) staff       (20)     1709 2023-02-11 11:26:13.000000 cfr-graphem-0.4.0/graphem/QUIC.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)       52 2023-02-11 11:26:13.000000 cfr-graphem-0.4.0/graphem/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    13086 2023-02-11 11:26:13.000000 cfr-graphem-0.4.0/graphem/graph.py
+-rwxr-xr-x   0 fengzhu    (502) staff       (20)     5846 2023-02-11 11:26:13.000000 cfr-graphem-0.4.0/graphem/iridge.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    28850 2023-07-25 22:19:58.000000 cfr-graphem-0.4.0/graphem/solver.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-07-25 22:20:19.196333 cfr-graphem-0.4.0/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1452 2023-07-25 22:19:14.000000 cfr-graphem-0.4.0/setup.py
```

### Comparing `cfr-graphem-0.3.1/LICENSE` & `cfr-graphem-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.1/PKG-INFO` & `cfr-graphem-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr-graphem
-Version: 0.3.1
+Version: 0.4.0
 Summary: The GraphEM component for CFR
 Home-page: https://github.com/fzhu2e/cfr-graphem
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-graphem-0.3.1/cfr_graphem.egg-info/PKG-INFO` & `cfr-graphem-0.4.0/cfr_graphem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr-graphem
-Version: 0.3.1
+Version: 0.4.0
 Summary: The GraphEM component for CFR
 Home-page: https://github.com/fzhu2e/cfr-graphem
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-graphem-0.3.1/graphem/GraphEstimation.py` & `cfr-graphem-0.4.0/graphem/GraphEstimation.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.1/graphem/QUIC.cpp` & `cfr-graphem-0.4.0/graphem/QUIC.cpp`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.1/graphem/QUIC.py` & `cfr-graphem-0.4.0/graphem/QUIC.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.1/graphem/graph.py` & `cfr-graphem-0.4.0/graphem/graph.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.1/graphem/iridge.py` & `cfr-graphem-0.4.0/graphem/iridge.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.1/graphem/solver.py` & `cfr-graphem-0.4.0/graphem/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.tol = tol
         self.field_r = []
         self.proxy_r = []
         self.calib = []
         self.Sigma = []
         self.mu = []
 
-    def fit(self, field, proxy, calib, graph=[], lonlat=[], sp_FF=3.0, sp_FP=3.0, sp_PP=3.0, N_graph=30, C0=[], M0=[], maxit=200,
+    def fit(self, field, proxy, calib, graph=None, lonlat=[], sp_FF=3.0, sp_FP=3.0, sp_PP=3.0, N_graph=30, C0=[], M0=[], maxit=200,
         bootstrap=False, N_boot=20, cutoff_radius=1000, graph_method='neighborhood', estimate_graph=True, save_graphs=False, verbose=False):
         '''
         Estimates the parameters of the GraphEM model and reconstruct the missing values of the climate
         and proxy fields.
 
         Parameters
         ----------
@@ -127,15 +127,15 @@
                         [self.graph, self.sparsity] = graph_greedy_search(Xridge[:,ind_F], Xridge[:,ind_P], sp_FF, sp_FP, sp_PP, N_graph)
                     else:
                         [self.graph, self.sparsity] = graph_greedy_search(field[calib,:], proxy[calib,:], sp_FF, sp_FP, sp_PP, N_graph)
                 else:
                     return "Error: graph can't be generated! Please choose a graph option."
 
             else:
-                if graph == []:
+                if graph is None:
                     return "Error: you need to specify a graph if estimate_graph = False."
                 else:
                     if verbose: print("Using specified graph")
 
             [X,C,M] = self.EM(X, self.graph, C0, M0, maxit, verbose=verbose)
             self.field_r = X[:,ind_F]
             self.proxy_r = X[:,ind_P]
```

### Comparing `cfr-graphem-0.3.1/setup.py` & `cfr-graphem-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         filename = super().get_ext_filename(ext_name)
         suffix = sysconfig.get_config_var('EXT_SUFFIX')
         ext = os.path.splitext(filename)[1]
         return os.path.join('./graphem', filename.replace(suffix, "")+ext)
 
 setup(
     name='cfr-graphem',
-    version='0.3.1',
+    version='0.4.0',
     description='The GraphEM component for CFR',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr-graphem',
     packages=find_packages(),
```

