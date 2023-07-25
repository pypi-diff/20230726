# Comparing `tmp/cfr-graphem-0.3.0.tar.gz` & `tmp/cfr-graphem-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-graphem-0.3.0.tar", last modified: Thu Jun 22 23:59:31 2023, max compression
+gzip compressed data, was "cfr-graphem-0.3.1.tar", last modified: Tue Jul 25 22:08:00 2023, max compression
```

## Comparing `cfr-graphem-0.3.0.tar` & `cfr-graphem-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 23:59:31.365577 cfr-graphem-0.3.0/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2023-02-11 11:26:13.000000 cfr-graphem-0.3.0/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)      706 2023-06-22 23:59:31.365403 cfr-graphem-0.3.0/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      215 2023-02-11 11:26:13.000000 cfr-graphem-0.3.0/README.rst
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 23:59:31.363056 cfr-graphem-0.3.0/cfr_graphem.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)      706 2023-06-22 23:59:31.000000 cfr-graphem-0.3.0/cfr_graphem.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      370 2023-06-22 23:59:31.000000 cfr-graphem-0.3.0/cfr_graphem.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-22 23:59:31.000000 cfr-graphem-0.3.0/cfr_graphem.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-02-11 12:40:30.000000 cfr-graphem-0.3.0/cfr_graphem.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-22 23:59:31.000000 cfr-graphem-0.3.0/cfr_graphem.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       16 2023-06-22 23:59:31.000000 cfr-graphem-0.3.0/cfr_graphem.egg-info/top_level.txt
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 23:59:31.365001 cfr-graphem-0.3.0/graphem/
--rwxr-xr-x   0 fengzhu    (502) staff       (20)     9952 2023-06-22 23:58:14.000000 cfr-graphem-0.3.0/graphem/GraphEstimation.py
--rwxr-xr-x   0 fengzhu    (502) staff       (20)    15228 2023-02-11 11:26:13.000000 cfr-graphem-0.3.0/graphem/QUIC.cpp
--rwxr-xr-x   0 fengzhu    (502) staff       (20)     1709 2023-02-11 11:26:13.000000 cfr-graphem-0.3.0/graphem/QUIC.py
--rw-r--r--   0 fengzhu    (502) staff       (20)       52 2023-02-11 11:26:13.000000 cfr-graphem-0.3.0/graphem/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    13086 2023-02-11 11:26:13.000000 cfr-graphem-0.3.0/graphem/graph.py
--rwxr-xr-x   0 fengzhu    (502) staff       (20)     5846 2023-02-11 11:26:13.000000 cfr-graphem-0.3.0/graphem/iridge.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    28851 2023-03-27 02:40:31.000000 cfr-graphem-0.3.0/graphem/solver.py
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-22 23:59:31.365627 cfr-graphem-0.3.0/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1452 2023-06-22 23:59:19.000000 cfr-graphem-0.3.0/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-25 22:08:00.891713 cfr-graphem-0.3.1/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)      706 2023-07-25 22:08:00.891542 cfr-graphem-0.3.1/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      215 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/README.rst
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-25 22:08:00.888929 cfr-graphem-0.3.1/cfr_graphem.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      706 2023-07-25 22:08:00.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      370 2023-07-25 22:08:00.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-07-25 22:08:00.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-02-11 12:40:30.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-07-25 22:08:00.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       16 2023-07-25 22:08:00.000000 cfr-graphem-0.3.1/cfr_graphem.egg-info/top_level.txt
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-07-25 22:08:00.891105 cfr-graphem-0.3.1/graphem/
+-rwxr-xr-x   0 fengzhu    (502) staff       (20)     9952 2023-06-22 23:58:14.000000 cfr-graphem-0.3.1/graphem/GraphEstimation.py
+-rwxr-xr-x   0 fengzhu    (502) staff       (20)    15228 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/graphem/QUIC.cpp
+-rwxr-xr-x   0 fengzhu    (502) staff       (20)     1709 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/graphem/QUIC.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)       52 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/graphem/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    13086 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/graphem/graph.py
+-rwxr-xr-x   0 fengzhu    (502) staff       (20)     5846 2023-02-11 11:26:13.000000 cfr-graphem-0.3.1/graphem/iridge.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    28846 2023-07-25 22:04:10.000000 cfr-graphem-0.3.1/graphem/solver.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-07-25 22:08:00.891756 cfr-graphem-0.3.1/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1452 2023-07-25 22:04:31.000000 cfr-graphem-0.3.1/setup.py
```

### Comparing `cfr-graphem-0.3.0/LICENSE` & `cfr-graphem-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.0/PKG-INFO` & `cfr-graphem-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr-graphem
-Version: 0.3.0
+Version: 0.3.1
 Summary: The GraphEM component for CFR
 Home-page: https://github.com/fzhu2e/cfr-graphem
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-graphem-0.3.0/cfr_graphem.egg-info/PKG-INFO` & `cfr-graphem-0.3.1/cfr_graphem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr-graphem
-Version: 0.3.0
+Version: 0.3.1
 Summary: The GraphEM component for CFR
 Home-page: https://github.com/fzhu2e/cfr-graphem
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-graphem-0.3.0/graphem/GraphEstimation.py` & `cfr-graphem-0.3.1/graphem/GraphEstimation.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.0/graphem/QUIC.cpp` & `cfr-graphem-0.3.1/graphem/QUIC.cpp`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.0/graphem/QUIC.py` & `cfr-graphem-0.3.1/graphem/QUIC.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.0/graphem/graph.py` & `cfr-graphem-0.3.1/graphem/graph.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.0/graphem/iridge.py` & `cfr-graphem-0.3.1/graphem/iridge.py`

 * *Files identical despite different names*

### Comparing `cfr-graphem-0.3.0/graphem/solver.py` & `cfr-graphem-0.3.1/graphem/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
             X = X-Mup
             M = M + Mup
                 
             # Re-estimate C
             if use_iridge:
                 C = (X.T.dot(X) + CovRes)/(n-1)
             else:
-                C = self.fit_Sigma(np.cov(X.T) + CovRes/(n-1), self.graph)
+                C = self.fit_Sigma(np.cov(X.T) + CovRes/(n-1), graph)
             # if verbose: print("%1.3d     %1.4f     %1.4f" % (it, dXmis, rdXmis))
         X = X + M
 
         return [X, C, M]
             
     def fit_Sigma(self, S, graph):
         ''' Estimates the covariance matrix of the field using the provided graph
```

### Comparing `cfr-graphem-0.3.0/setup.py` & `cfr-graphem-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         filename = super().get_ext_filename(ext_name)
         suffix = sysconfig.get_config_var('EXT_SUFFIX')
         ext = os.path.splitext(filename)[1]
         return os.path.join('./graphem', filename.replace(suffix, "")+ext)
 
 setup(
     name='cfr-graphem',
-    version='0.3.0',
+    version='0.3.1',
     description='The GraphEM component for CFR',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr-graphem',
     packages=find_packages(),
```

