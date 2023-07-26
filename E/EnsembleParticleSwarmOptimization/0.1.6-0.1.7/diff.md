# Comparing `tmp/EnsembleParticleSwarmOptimization-0.1.6.tar.gz` & `tmp/EnsembleParticleSwarmOptimization-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.6.tar", last modified: Wed Jul 26 14:48:38 2023, max compression
+gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.7.tar", last modified: Wed Jul 26 15:05:02 2023, max compression
```

## Comparing `EnsembleParticleSwarmOptimization-0.1.6.tar` & `EnsembleParticleSwarmOptimization-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-26 14:48:38.770998 EnsembleParticleSwarmOptimization-0.1.6/
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-26 14:48:38.770998 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-26 14:48:38.000000 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-07-26 14:48:38.000000 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-07-26 14:48:38.000000 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-07-26 14:48:38.000000 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/requires.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-07-26 14:48:38.000000 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-26 14:48:38.770998 EnsembleParticleSwarmOptimization-0.1.6/PKG-INFO
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-26 14:48:38.770998 EnsembleParticleSwarmOptimization-0.1.6/PySO/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/Clustering_Swarms.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/HierarchicalSwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30623 2023-07-26 14:39:38.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/MWE_Swarm.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/Model.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/SwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-07-26 14:41:02.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/__init__.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.6/README.md
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-07-26 14:48:38.770998 EnsembleParticleSwarmOptimization-0.1.6/setup.cfg
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-07-26 14:41:18.000000 EnsembleParticleSwarmOptimization-0.1.6/setup.py
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-26 15:05:02.929178 EnsembleParticleSwarmOptimization-0.1.7/
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-26 15:05:02.929178 EnsembleParticleSwarmOptimization-0.1.7/EnsembleParticleSwarmOptimization.egg-info/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-26 15:05:02.000000 EnsembleParticleSwarmOptimization-0.1.7/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-07-26 15:05:02.000000 EnsembleParticleSwarmOptimization-0.1.7/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-07-26 15:05:02.000000 EnsembleParticleSwarmOptimization-0.1.7/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-07-26 15:05:02.000000 EnsembleParticleSwarmOptimization-0.1.7/EnsembleParticleSwarmOptimization.egg-info/requires.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-07-26 15:05:02.000000 EnsembleParticleSwarmOptimization-0.1.7/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-26 15:05:02.929178 EnsembleParticleSwarmOptimization-0.1.7/PKG-INFO
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-26 15:05:02.929178 EnsembleParticleSwarmOptimization-0.1.7/PySO/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.7/PySO/Clustering_Swarms.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.7/PySO/HierarchicalSwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30843 2023-07-26 15:04:25.000000 EnsembleParticleSwarmOptimization-0.1.7/PySO/MWE_Swarm.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.7/PySO/Model.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.7/PySO/SwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-07-26 15:04:47.000000 EnsembleParticleSwarmOptimization-0.1.7/PySO/__init__.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.7/README.md
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-07-26 15:05:02.929178 EnsembleParticleSwarmOptimization-0.1.7/setup.cfg
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-07-26 15:04:54.000000 EnsembleParticleSwarmOptimization-0.1.7/setup.py
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.7/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.6
+Version: 0.1.7
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.6/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.6
+Version: 0.1.7
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.6/PySO/Clustering_Swarms.py` & `EnsembleParticleSwarmOptimization-0.1.7/PySO/Clustering_Swarms.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.6/PySO/HierarchicalSwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.7/PySO/HierarchicalSwarmHandler.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.6/PySO/MWE_Swarm.py` & `EnsembleParticleSwarmOptimization-0.1.7/PySO/MWE_Swarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,18 @@
         upper_mask_indices = np.where((self.Points - self.BoundsArray[:,1])>0)
         lower_mask_indices = np.where((self.Points - self.BoundsArray[:,0])<0)
 
         # Reflective boundary conditions
         self.Points[upper_mask_indices] = self.BoundsArray[upper_mask_indices[1],1] - np.abs(self.Points[upper_mask_indices] - self.BoundsArray[upper_mask_indices[1],1])
         self.Points[lower_mask_indices] = self.BoundsArray[lower_mask_indices[1],0] + np.abs(self.Points[lower_mask_indices] - self.BoundsArray[lower_mask_indices[1],0])
 
+	
+        # Hard edges (Catching particles going completely out of bounds) (Hopefully should only be a few particles)
+        self.Points = np.clip(self.Points, a_min=self.BoundsArray[:,0], a_max=self.BoundsArray[:,1])
+
 
     def PSO_VelocityRule(self):
         """
         The standard PSO rule for updating the velocities with a jitter component added to reduce the chance of a particle
         stuck in a local maxima
 
         RETURN:
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.6/PySO/Model.py` & `EnsembleParticleSwarmOptimization-0.1.7/PySO/Model.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.6/PySO/SwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.7/PySO/SwarmHandler.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.6/setup.py` & `EnsembleParticleSwarmOptimization-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EnsembleParticleSwarmOptimization",
-    version="0.1.6",
+    version="0.1.7",
     author="Christopher Moore and Diganta Bandopadhyay",
     author_email="diganta@star.sr.bham.ac.uk",
     description="Ensemble of particle swarms together with various velocity rules for function optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dig07/PySO",
     packages=setuptools.find_packages(),
```

