# Comparing `tmp/EnsembleParticleSwarmOptimization-0.1.5.tar.gz` & `tmp/EnsembleParticleSwarmOptimization-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.5.tar", last modified: Tue Jul 25 14:01:53 2023, max compression
+gzip compressed data, was "EnsembleParticleSwarmOptimization-0.1.6.tar", last modified: Wed Jul 26 14:48:38 2023, max compression
```

## Comparing `EnsembleParticleSwarmOptimization-0.1.5.tar` & `EnsembleParticleSwarmOptimization-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-25 14:01:53.919572 EnsembleParticleSwarmOptimization-0.1.5/
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-25 14:01:53.919572 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-25 14:01:53.000000 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-07-25 14:01:53.000000 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-07-25 14:01:53.000000 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-07-25 14:01:53.000000 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/requires.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-07-25 14:01:53.000000 EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-25 14:01:53.919572 EnsembleParticleSwarmOptimization-0.1.5/PKG-INFO
-drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-25 14:01:53.919572 EnsembleParticleSwarmOptimization-0.1.5/PySO/
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/Clustering_Swarms.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/HierarchicalSwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30629 2023-07-25 13:56:21.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/MWE_Swarm.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/Model.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/SwarmHandler.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-07-25 13:58:45.000000 EnsembleParticleSwarmOptimization-0.1.5/PySO/__init__.py
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.5/README.md
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-07-25 14:01:53.919572 EnsembleParticleSwarmOptimization-0.1.5/setup.cfg
--rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-07-25 13:58:52.000000 EnsembleParticleSwarmOptimization-0.1.5/setup.py
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-26 14:48:38.770998 EnsembleParticleSwarmOptimization-0.1.6/
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-26 14:48:38.770998 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-26 14:48:38.000000 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      431 2023-07-26 14:48:38.000000 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/SOURCES.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        1 2023-07-26 14:48:38.000000 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/dependency_links.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       77 2023-07-26 14:48:38.000000 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/requires.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)        5 2023-07-26 14:48:38.000000 EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/top_level.txt
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      730 2023-07-26 14:48:38.770998 EnsembleParticleSwarmOptimization-0.1.6/PKG-INFO
+drwxr-xr-x   0 dxb792   (1939480938) domain users (1734600513)        0 2023-07-26 14:48:38.770998 EnsembleParticleSwarmOptimization-0.1.6/PySO/
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    10064 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/Clustering_Swarms.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    34011 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/HierarchicalSwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)    30623 2023-07-26 14:39:38.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/MWE_Swarm.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     2174 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/Model.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)     8369 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/SwarmHandler.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      288 2023-07-26 14:41:02.000000 EnsembleParticleSwarmOptimization-0.1.6/PySO/__init__.py
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      212 2023-07-21 11:31:24.000000 EnsembleParticleSwarmOptimization-0.1.6/README.md
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)       38 2023-07-26 14:48:38.770998 EnsembleParticleSwarmOptimization-0.1.6/setup.cfg
+-rw-r--r--   0 dxb792   (1939480938) domain users (1734600513)      885 2023-07-26 14:41:18.000000 EnsembleParticleSwarmOptimization-0.1.6/setup.py
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.5/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.6/EnsembleParticleSwarmOptimization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.5
+Version: 0.1.6
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.5/PKG-INFO` & `EnsembleParticleSwarmOptimization-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EnsembleParticleSwarmOptimization
-Version: 0.1.5
+Version: 0.1.6
 Summary: Ensemble of particle swarms together with various velocity rules for function optimization
 Home-page: https://github.com/dig07/PySO
 Author: Christopher Moore and Diganta Bandopadhyay
 Author-email: diganta@star.sr.bham.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.5/PySO/Clustering_Swarms.py` & `EnsembleParticleSwarmOptimization-0.1.6/PySO/Clustering_Swarms.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.5/PySO/HierarchicalSwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.6/PySO/HierarchicalSwarmHandler.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.5/PySO/MWE_Swarm.py` & `EnsembleParticleSwarmOptimization-0.1.6/PySO/MWE_Swarm.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,25 +341,23 @@
     def EnforceBoundaries(self):
         """
         Boundary conditions on the edge of the search region
         """
         # Periodic BCs
         self.Points[:,self.Periodic_params] = self.BoundsArray[self.Periodic_params,0] + np.mod(self.Points[:,self.Periodic_params]-self.BoundsArray[self.Periodic_params,0],self.PeriodicParamRanges[self.Periodic_params])
 
-        # Hard edges
-        clipped_points = np.clip(self.Points, a_min=self.BoundsArray[:,0], a_max=self.BoundsArray[:,1])
 
-        # Reflective boundary velocities
-        # This does mess with the MH MCMC part of the velocity rule, so proposals near prior boundary in the case MH_fraction=1.0 will be affected
-        velocity_reflection_indices = np.where(clipped_points != self.Points)
+        # Mask for points that are clipped
+        upper_mask_indices = np.where((self.Points - self.BoundsArray[:,1])>0)
+        lower_mask_indices = np.where((self.Points - self.BoundsArray[:,0])<0)
+
+        # Reflective boundary conditions
+        self.Points[upper_mask_indices] = self.BoundsArray[upper_mask_indices[1],1] - np.abs(self.Points[upper_mask_indices] - self.BoundsArray[upper_mask_indices[1],1])
+        self.Points[lower_mask_indices] = self.BoundsArray[lower_mask_indices[1],0] + np.abs(self.Points[lower_mask_indices] - self.BoundsArray[lower_mask_indices[1],0])
 
-        self.Points = clipped_points
-
-        for particle,param_index in zip(velocity_reflection_indices[0],velocity_reflection_indices[1]):
-            self.Velocities[particle,param_index] *= -1
 
     def PSO_VelocityRule(self):
         """
         The standard PSO rule for updating the velocities with a jitter component added to reduce the chance of a particle
         stuck in a local maxima
 
         RETURN:
```

### Comparing `EnsembleParticleSwarmOptimization-0.1.5/PySO/Model.py` & `EnsembleParticleSwarmOptimization-0.1.6/PySO/Model.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.5/PySO/SwarmHandler.py` & `EnsembleParticleSwarmOptimization-0.1.6/PySO/SwarmHandler.py`

 * *Files identical despite different names*

### Comparing `EnsembleParticleSwarmOptimization-0.1.5/setup.py` & `EnsembleParticleSwarmOptimization-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="EnsembleParticleSwarmOptimization",
-    version="0.1.5",
+    version="0.1.6",
     author="Christopher Moore and Diganta Bandopadhyay",
     author_email="diganta@star.sr.bham.ac.uk",
     description="Ensemble of particle swarms together with various velocity rules for function optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dig07/PySO",
     packages=setuptools.find_packages(),
```

