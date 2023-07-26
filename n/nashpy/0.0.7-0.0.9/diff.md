# Comparing `tmp/nashpy-0.0.7.tar.gz` & `tmp/nashpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nashpy-0.0.7.tar", last modified: Sat Jun 17 18:57:00 2017, max compression
+gzip compressed data, was "dist/nashpy-0.0.9.tar", last modified: Tue Jun 20 21:12:48 2017, max compression
```

## Comparing `nashpy-0.0.7.tar` & `nashpy-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-17 18:57:00.000000 nashpy-0.0.7/
--rw-rw-r--   0 vince     (1000) vince     (1000)       38 2017-06-17 18:57:00.000000 nashpy-0.0.7/setup.cfg
-drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-17 18:57:00.000000 nashpy-0.0.7/src/
-drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-17 18:57:00.000000 nashpy-0.0.7/src/nash/
--rw-rw-r--   0 vince     (1000) vince     (1000)       53 2017-06-14 18:23:30.000000 nashpy-0.0.7/src/nash/__init__.py
--rw-rw-r--   0 vince     (1000) vince     (1000)       22 2017-06-17 18:54:07.000000 nashpy-0.0.7/src/nash/version.py
-drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-17 18:57:00.000000 nashpy-0.0.7/src/nash/algorithms/
--rw-rw-r--   0 vince     (1000) vince     (1000)     4867 2017-06-17 17:41:01.000000 nashpy-0.0.7/src/nash/algorithms/support_enumeration.py
--rw-rw-r--   0 vince     (1000) vince     (1000)       34 2017-06-14 18:59:07.000000 nashpy-0.0.7/src/nash/algorithms/__init__.py
--rw-rw-r--   0 vince     (1000) vince     (1000)     1343 2017-06-17 17:38:57.000000 nashpy-0.0.7/src/nash/algorithms/vertex_enumeration.py
-drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-17 18:57:00.000000 nashpy-0.0.7/src/nash/polytope/
--rw-rw-r--   0 vince     (1000) vince     (1000)       24 2017-06-14 18:59:07.000000 nashpy-0.0.7/src/nash/polytope/__init__.py
--rw-rw-r--   0 vince     (1000) vince     (1000)     2428 2017-06-17 11:59:44.000000 nashpy-0.0.7/src/nash/polytope/polytope.py
--rw-rw-r--   0 vince     (1000) vince     (1000)     2568 2017-06-17 17:09:55.000000 nashpy-0.0.7/src/nash/game.py
-drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-17 18:57:00.000000 nashpy-0.0.7/src/nashpy.egg-info/
--rw-rw-r--   0 vince     (1000) vince     (1000)      412 2017-06-17 18:57:00.000000 nashpy-0.0.7/src/nashpy.egg-info/SOURCES.txt
--rw-rw-r--   0 vince     (1000) vince     (1000)        5 2017-06-17 18:57:00.000000 nashpy-0.0.7/src/nashpy.egg-info/top_level.txt
--rw-rw-r--   0 vince     (1000) vince     (1000)       28 2017-06-17 18:57:00.000000 nashpy-0.0.7/src/nashpy.egg-info/requires.txt
--rw-rw-r--   0 vince     (1000) vince     (1000)        1 2017-06-17 18:57:00.000000 nashpy-0.0.7/src/nashpy.egg-info/dependency_links.txt
--rw-rw-r--   0 vince     (1000) vince     (1000)      284 2017-06-17 18:57:00.000000 nashpy-0.0.7/src/nashpy.egg-info/PKG-INFO
--rw-rw-r--   0 vince     (1000) vince     (1000)      284 2017-06-17 18:57:00.000000 nashpy-0.0.7/PKG-INFO
--rw-rw-r--   0 vince     (1000) vince     (1000)     1152 2017-06-17 17:12:27.000000 nashpy-0.0.7/setup.py
+drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-20 21:12:48.000000 nashpy-0.0.9/
+-rw-rw-r--   0 vince     (1000) vince     (1000)       38 2017-06-20 21:12:48.000000 nashpy-0.0.9/setup.cfg
+drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/
+drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/nash/
+-rw-rw-r--   0 vince     (1000) vince     (1000)       53 2017-06-14 18:23:30.000000 nashpy-0.0.9/src/nash/__init__.py
+-rw-rw-r--   0 vince     (1000) vince     (1000)       22 2017-06-20 16:48:13.000000 nashpy-0.0.9/src/nash/version.py
+drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/nash/integer_pivoting/
+-rw-rw-r--   0 vince     (1000) vince     (1000)     1541 2017-06-20 16:47:29.000000 nashpy-0.0.9/src/nash/integer_pivoting/integer_pivoting.py
+-rw-rw-r--   0 vince     (1000) vince     (1000)       32 2017-06-20 16:47:29.000000 nashpy-0.0.9/src/nash/integer_pivoting/__init__.py
+drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/nash/algorithms/
+-rw-rw-r--   0 vince     (1000) vince     (1000)     4867 2017-06-17 17:41:01.000000 nashpy-0.0.9/src/nash/algorithms/support_enumeration.py
+-rw-rw-r--   0 vince     (1000) vince     (1000)       34 2017-06-19 21:24:18.000000 nashpy-0.0.9/src/nash/algorithms/__init__.py
+-rw-rw-r--   0 vince     (1000) vince     (1000)     1343 2017-06-20 07:39:11.000000 nashpy-0.0.9/src/nash/algorithms/vertex_enumeration.py
+-rw-rw-r--   0 vince     (1000) vince     (1000)     3153 2017-06-20 16:47:29.000000 nashpy-0.0.9/src/nash/algorithms/lemke_howson.py
+drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/nash/polytope/
+-rw-rw-r--   0 vince     (1000) vince     (1000)       24 2017-06-14 18:59:07.000000 nashpy-0.0.9/src/nash/polytope/__init__.py
+-rw-rw-r--   0 vince     (1000) vince     (1000)     2428 2017-06-17 11:59:44.000000 nashpy-0.0.9/src/nash/polytope/polytope.py
+-rw-rw-r--   0 vince     (1000) vince     (1000)     3443 2017-06-20 16:47:29.000000 nashpy-0.0.9/src/nash/game.py
+drwxrwxr-x   0 vince     (1000) vince     (1000)        0 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/nashpy.egg-info/
+-rw-rw-r--   0 vince     (1000) vince     (1000)      532 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/nashpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 vince     (1000) vince     (1000)        5 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/nashpy.egg-info/top_level.txt
+-rw-rw-r--   0 vince     (1000) vince     (1000)       28 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/nashpy.egg-info/requires.txt
+-rw-rw-r--   0 vince     (1000) vince     (1000)        1 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/nashpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 vince     (1000) vince     (1000)      284 2017-06-20 21:12:48.000000 nashpy-0.0.9/src/nashpy.egg-info/PKG-INFO
+-rw-rw-r--   0 vince     (1000) vince     (1000)      284 2017-06-20 21:12:48.000000 nashpy-0.0.9/PKG-INFO
+-rw-rw-r--   0 vince     (1000) vince     (1000)     1152 2017-06-17 17:12:27.000000 nashpy-0.0.9/setup.py
```

### Comparing `nashpy-0.0.7/src/nash/algorithms/support_enumeration.py` & `nashpy-0.0.9/src/nash/algorithms/support_enumeration.py`

 * *Files identical despite different names*

### Comparing `nashpy-0.0.7/src/nash/algorithms/vertex_enumeration.py` & `nashpy-0.0.9/src/nash/algorithms/vertex_enumeration.py`

 * *Files identical despite different names*

### Comparing `nashpy-0.0.7/src/nash/polytope/polytope.py` & `nashpy-0.0.9/src/nash/polytope/polytope.py`

 * *Files identical despite different names*

### Comparing `nashpy-0.0.7/src/nash/game.py` & `nashpy-0.0.9/src/nash/game.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """A class for a normal form game"""
 import numpy as np
-from .algorithms.vertex_enumeration import vertex_enumeration
+from .algorithms.lemke_howson import lemke_howson
 from .algorithms.support_enumeration import support_enumeration
-from itertools import chain, combinations
+from .algorithms.vertex_enumeration import vertex_enumeration
+from itertools import combinations
 
 
 class Game:
     """
     A class for a normal form game.
 
     Parameters
@@ -44,16 +45,15 @@
                          for m in self.payoff_matrices])
 
     def vertex_enumeration(self):
         """
         Obtain the Nash equilibria using enumeration of the vertices of the best
         response polytopes.
 
-        Algorithm implemented here is Algorithm 3.5 of Nisan, Noam, et al., eds.
-        Algorithmic game theory. Cambridge University Press, 2007.
+        Algorithm implemented here is Algorithm 3.5 of [Nisan2007]_.
 
         1. Build best responses polytopes of both players
         2. For each vertex pair of both polytopes
         3. Check if pair is fully labelled
         4. Return the normalised pair
 
         Returns
@@ -63,21 +63,49 @@
         """
         return vertex_enumeration(*self.payoff_matrices)
 
     def support_enumeration(self):
         """
         Obtain the Nash equilibria using support enumeration.
 
-        Algorithm implemented here is Algorithm 3.4 of Nisan, Noam, et al., eds.
-        Algorithmic game theory. Cambridge University Press, 2007.
+        Algorithm implemented here is Algorithm 3.4 of [Nisan2007]_.
 
         1. For each k in 1...min(size of strategy sets)
         2. For each I,J supports of size k
         3. Solve indifference conditions
         4. Check that have Nash Equilibrium.
 
         Returns
         -------
 
             equilibria: A generator.
         """
         return support_enumeration(*self.payoff_matrices)
+
+    def lemke_howson(self, initial_dropped_label):
+        """
+        Obtain the Nash equilibria using the Lemke Howson algorithm implemented
+        using integer pivoting.
+
+        Algorithm implemented here is Algorithm 3.6 of [Nisan2007]_.
+
+        1. Start at the artificial equilibrium (which is fully labeled)
+        2. Choose an initial label to drop and move in the polytope for which
+           the vertex has that label to the edge
+           that does not share that label. (This is implemented using integer
+           pivoting)
+        3. A label will now be duplicated in the other polytope, drop it in a
+           similar way.
+        4. Repeat steps 2 and 3 until have Nash Equilibrium.
+
+        Parameters
+        ----------
+
+            initial_dropped_label: int
+
+        Returns
+        -------
+
+            equilibria: A tuple.
+        """
+        return lemke_howson(*self.payoff_matrices,
+                            initial_dropped_label=initial_dropped_label)
```

### Comparing `nashpy-0.0.7/setup.py` & `nashpy-0.0.9/setup.py`

 * *Files identical despite different names*

