# Comparing `tmp/pymolviz-1.1.tar.gz` & `tmp/pymolviz-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymolviz-1.1.tar", last modified: Sun Jul 23 17:04:21 2023, max compression
+gzip compressed data, was "/home/highgarden/PyMolViz/module/dist/.tmp-hje4rdmx/pymolviz-1.1.1.tar", last modified: Wed Jul 26 09:42:26 2023, max compression
```

## Comparing `pymolviz-1.1.tar` & `pymolviz-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 finn      (1000) finn      (1000)        0 2023-07-23 17:04:21.954474 pymolviz-1.1/
--rw-rw-r--   0 finn      (1000) finn      (1000)      228 2023-07-23 17:04:21.954474 pymolviz-1.1/PKG-INFO
-drwxrwxr-x   0 finn      (1000) finn      (1000)        0 2023-07-23 17:04:21.950475 pymolviz-1.1/pymolviz/
--rw-rw-r--   0 finn      (1000) finn      (1000)     7883 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/ColorMap.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     1597 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/Displayable.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     1865 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/Group.py
-drwxrwxr-x   0 finn      (1000) finn      (1000)        0 2023-07-23 17:04:21.950475 pymolviz-1.1/pymolviz/PyMOLobjects/
--rw-rw-r--   0 finn      (1000) finn      (1000)      980 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/PyMOLobjects/Labels.py
--rw-rw-r--   0 finn      (1000) finn      (1000)       26 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/PyMOLobjects/__init__.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     2014 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/Script.py
--rw-rw-r--   0 finn      (1000) finn      (1000)      302 2023-07-23 16:57:38.000000 pymolviz-1.1/pymolviz/__init__.py
-drwxrwxr-x   0 finn      (1000) finn      (1000)        0 2023-07-23 17:04:21.950475 pymolviz-1.1/pymolviz/meshes/
--rw-rw-r--   0 finn      (1000) finn      (1000)     2919 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/meshes/Arrows.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     2719 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/meshes/CGOCollection.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     2777 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/meshes/Lines.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     3166 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/meshes/Mesh.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     1076 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/meshes/Plane.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     3762 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/meshes/Points.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     1172 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/meshes/Sphere.py
--rw-rw-r--   0 finn      (1000) finn      (1000)      195 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/meshes/__init__.py
-drwxrwxr-x   0 finn      (1000) finn      (1000)        0 2023-07-23 17:04:21.950475 pymolviz-1.1/pymolviz/util/
--rw-rw-r--   0 finn      (1000) finn      (1000)       81 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/util/__init__.py
--rw-rw-r--   0 finn      (1000) finn      (1000)    15459 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/util/colors.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     4799 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/util/geometries.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     1727 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/util/io.py
--rw-rw-r--   0 finn      (1000) finn      (1000)      711 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/util/math.py
-drwxrwxr-x   0 finn      (1000) finn      (1000)        0 2023-07-23 17:04:21.954474 pymolviz-1.1/pymolviz/volumetric/
--rw-rw-r--   0 finn      (1000) finn      (1000)     2266 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/volumetric/ColorRamp.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     5437 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/volumetric/GridData.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     5679 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/volumetric/IrregularData.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     1104 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/volumetric/IsoMesh.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     3355 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/volumetric/IsoSurface.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     2529 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/volumetric/IsoVolume.py
--rw-rw-r--   0 finn      (1000) finn      (1000)     4421 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/volumetric/Volume.py
--rw-rw-r--   0 finn      (1000) finn      (1000)      228 2023-07-23 16:06:34.000000 pymolviz-1.1/pymolviz/volumetric/__init__.py
-drwxrwxr-x   0 finn      (1000) finn      (1000)        0 2023-07-23 17:04:21.950475 pymolviz-1.1/pymolviz.egg-info/
--rw-rw-r--   0 finn      (1000) finn      (1000)      228 2023-07-23 17:04:21.000000 pymolviz-1.1/pymolviz.egg-info/PKG-INFO
--rw-rw-r--   0 finn      (1000) finn      (1000)      962 2023-07-23 17:04:21.000000 pymolviz-1.1/pymolviz.egg-info/SOURCES.txt
--rw-rw-r--   0 finn      (1000) finn      (1000)        1 2023-07-23 17:04:21.000000 pymolviz-1.1/pymolviz.egg-info/dependency_links.txt
--rw-rw-r--   0 finn      (1000) finn      (1000)        1 2023-07-23 16:08:50.000000 pymolviz-1.1/pymolviz.egg-info/not-zip-safe
--rw-rw-r--   0 finn      (1000) finn      (1000)       23 2023-07-23 17:04:21.000000 pymolviz-1.1/pymolviz.egg-info/requires.txt
--rw-rw-r--   0 finn      (1000) finn      (1000)        9 2023-07-23 17:04:21.000000 pymolviz-1.1/pymolviz.egg-info/top_level.txt
--rw-rw-r--   0 finn      (1000) finn      (1000)       38 2023-07-23 17:04:21.954474 pymolviz-1.1/setup.cfg
--rw-rw-r--   0 finn      (1000) finn      (1000)      575 2023-07-23 17:04:18.000000 pymolviz-1.1/setup.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 09:42:26.000000 pymolviz-1.1.1/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      264 2023-07-26 09:42:26.000000 pymolviz-1.1.1/PKG-INFO
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     9252 2023-07-24 11:53:42.000000 pymolviz-1.1.1/pymolviz/ColorMap.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2423 2023-07-24 13:12:11.000000 pymolviz-1.1.1/pymolviz/Displayable.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1842 2023-07-24 11:54:42.000000 pymolviz-1.1.1/pymolviz/Group.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz/PyMOLobjects/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1053 2023-07-24 11:47:59.000000 pymolviz-1.1.1/pymolviz/PyMOLobjects/Labels.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)       26 2023-07-20 14:22:32.000000 pymolviz-1.1.1/pymolviz/PyMOLobjects/__init__.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2025 2023-07-24 11:54:57.000000 pymolviz-1.1.1/pymolviz/Script.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      237 2023-07-21 15:03:55.000000 pymolviz-1.1.1/pymolviz/__init__.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz/meshes/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2933 2023-07-24 11:46:39.000000 pymolviz-1.1.1/pymolviz/meshes/Arrows.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2847 2023-07-24 11:45:15.000000 pymolviz-1.1.1/pymolviz/meshes/CGOCollection.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2791 2023-07-24 11:46:21.000000 pymolviz-1.1.1/pymolviz/meshes/Lines.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     3180 2023-07-24 11:46:08.000000 pymolviz-1.1.1/pymolviz/meshes/Mesh.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1167 2023-07-24 11:47:25.000000 pymolviz-1.1.1/pymolviz/meshes/Plane.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     3831 2023-07-24 11:58:38.000000 pymolviz-1.1.1/pymolviz/meshes/Points.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1338 2023-07-24 11:47:48.000000 pymolviz-1.1.1/pymolviz/meshes/Sphere.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      195 2023-07-20 14:22:32.000000 pymolviz-1.1.1/pymolviz/meshes/__init__.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz/util/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)       81 2023-07-20 14:22:32.000000 pymolviz-1.1.1/pymolviz/util/__init__.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)    15472 2023-07-24 11:12:50.000000 pymolviz-1.1.1/pymolviz/util/colors.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     4799 2023-05-12 12:56:34.000000 pymolviz-1.1.1/pymolviz/util/geometries.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1727 2023-07-20 14:22:32.000000 pymolviz-1.1.1/pymolviz/util/io.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      711 2023-05-12 08:38:42.000000 pymolviz-1.1.1/pymolviz/util/math.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz/volumetric/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2092 2023-07-24 11:51:03.000000 pymolviz-1.1.1/pymolviz/volumetric/ColorRamp.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     5708 2023-07-24 13:06:51.000000 pymolviz-1.1.1/pymolviz/volumetric/GridData.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     5679 2023-07-20 14:22:32.000000 pymolviz-1.1.1/pymolviz/volumetric/IrregularData.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     1104 2023-07-20 14:22:32.000000 pymolviz-1.1.1/pymolviz/volumetric/IsoMesh.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2932 2023-07-24 11:49:46.000000 pymolviz-1.1.1/pymolviz/volumetric/IsoSurface.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     2462 2023-07-24 11:50:16.000000 pymolviz-1.1.1/pymolviz/volumetric/IsoVolume.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)     4536 2023-07-24 11:58:03.000000 pymolviz-1.1.1/pymolviz/volumetric/Volume.py
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      228 2023-07-20 14:22:32.000000 pymolviz-1.1.1/pymolviz/volumetric/__init__.py
+drwxr-xr-x   0 highgarden  (1000) highgarden  (1000)        0 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz.egg-info/
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      264 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz.egg-info/PKG-INFO
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      962 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz.egg-info/SOURCES.txt
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)        1 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz.egg-info/dependency_links.txt
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)        1 2023-07-20 14:30:13.000000 pymolviz-1.1.1/pymolviz.egg-info/not-zip-safe
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)       30 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz.egg-info/requires.txt
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)        9 2023-07-26 09:42:26.000000 pymolviz-1.1.1/pymolviz.egg-info/top_level.txt
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)       38 2023-07-26 09:42:26.000000 pymolviz-1.1.1/setup.cfg
+-rw-r--r--   0 highgarden  (1000) highgarden  (1000)      636 2023-07-24 13:07:09.000000 pymolviz-1.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pymolviz-1.1/pymolviz/ColorMap.py` & `pymolviz-1.1.1/pymolviz/ColorMap.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,22 +5,34 @@
 import matplotlib.pyplot as plt
 import matplotlib.colors 
 import matplotlib.cm 
 from matplotlib.colors import LinearSegmentedColormap
 from .Displayable import Displayable
 
 class ColorMap(Displayable):
-    def __init__(self, values, colormap = "RdYlBu_r", values_are_single_color = None, name = None):
+    """
+    Creates a colormap from a list of values.
+    
+    Args:
+        values (list of float or list of (float, float) or list of (float, str) or list of (float, list of float)): The values to use for the colormap. If values_are_single_color is True, this is interpreted as a list of colors. If values_are_single_color is False, this is interpreted as a list of values to be mapped to a colormap. If values_are_single_color is None, this is interpreted as a list of values to be mapped to a colormap, unless it is a list of colors (strings or 3 or 4 long array-like), in which case it is interpreted as a list of colors.
+        colormap (str or matplotlib colormap or pymolviz.ColorMap): Optional. Defaults to "RdYlBu_r". The colormap to use.
+        values_are_single_color (bool): Optional. Defaults to None. If True, values is interpreted as a list of colors. If False, values is interpreted as a list of values to be mapped to a colormap. If None, values is interpreted as a list of values to be mapped to a colormap, unless it is a list of colors (strings or 3 or 4 long array-like), in which case it is interpreted as a list of colors.
+        name (str): Optional. Defaults to None. The name of the object.
+        state (int): Optional. Defaults to 1. The state of the object.
+    """
 
+    def __init__(self, values, colormap = "RdYlBu_r", values_are_single_color = None, name = None, state = 1):
+        
 
         # get colormap
         self.colormap = None
         self._color_type = None
         # differentiating between values
         self.color = None
+        self.state = state
         if (values_are_single_color is True) or (values_are_single_color is None):
 
             # if values is a single rgb(a) color
             try:
                 if np.issubdtype(type(values), np.str_):
                     color, alpha = self._value2color(values)
                     self.clims = [0, 1]
@@ -120,15 +132,15 @@
         from .volumetric.GridData import GridData
         dummy_data = GridData(np.zeros(8), name="cbar_dummy", step_sizes=(1e-8,1e-8,1e-8), step_counts=(1,1,1)) 
         
         sample_points = np.linspace(self.clims[0], self.clims[-1], 100)
         colors = self.get_color(sample_points)[:,:3]
         result = []
         result.append(dummy_data._script_string())
-        result.append(f"""cmd.ramp_new("{self.name}", "{dummy_data.name}", range = [{",".join([str(c) for c in sample_points])}], color = [{", ".join(["[" + ", ".join([str(c) for c in color]) + "]" for color in colors])}])""")
+        result.append(f"""cmd.ramp_new("{self.name}", "{dummy_data.name}", range = [{",".join([str(c) for c in sample_points])}], color = [{", ".join(["[" + ", ".join([str(c) for c in color]) + "]" for color in colors])}], state = {self.state})""")
         result.append(f"""cmd.delete("{dummy_data.name}")""")
 
         result = "\n".join(result)
         return result
 
     def _value2color(self, value):
         color = None
```

### Comparing `pymolviz-1.1/pymolviz/Group.py` & `pymolviz-1.1.1/pymolviz/Group.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from .Displayable import Displayable
 
 class Group(Displayable, list):
     """ A group can be used to aggregate multiple displayables into a PyMOL group.
     
     
     Attributes:
-        name (str): The name of the CGO object.
-        meshes (list): A list of meshes.
-        transformation (np.array): A 4x4 transformation matrix.
+        displayables (list): A list of displayables.
+        name (str): Optional. Defaults to None. The name of the object.
+        state (int): Optional. Defaults to 1. The state of the object.
+
     """
 
 
 
-    def __init__(self, displayables : list = None, name : str = None, state : int = 1, transparency : float = 0) -> None:
+    def __init__(self, displayables : list = None, name : str = None, state : int = 1) -> None:
         self.state = state
-        self.transparency = transparency
         
         super().__init__(name, displayables if displayables else [])
         self.extend(displayables if displayables else [])
 
     def __setitem__(self, index, item):
         if not item in self.dependencies:
             self.dependencies.append(item)
```

### Comparing `pymolviz-1.1/pymolviz/PyMOLobjects/Labels.py` & `pymolviz-1.1.1/pymolviz/PyMOLobjects/Labels.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     def __init__(self, positions, labels, name = None, state = 1, **kwargs):
         """ Represents a set of labels.
 
         Args:
             positions (np.array): The positions of the labels.
             labels (list): The labels.
             name (str): Optional. The name of the data. Defaults to None.
+            state (int): Optional. The state of the data. Defaults to 1.
 
         """
         positions = np.array(positions)
         if len(positions.shape) == 1:
             positions = np.array([positions])
             labels = [labels]
         self.positions = positions
```

### Comparing `pymolviz-1.1/pymolviz/Script.py` & `pymolviz-1.1.1/pymolviz/Script.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .Displayable import Displayable
 
 class Script(object):
     """A class wrapping one or multiple displayables to be added with a single script. Use write function to write the script to a file.
 
     Attributes:
-        collections (list): A list of collections.
+        displayables (list): A list of displayables.
+        
 
     """
 
 
     def __init__(self, displayables : list = None, *args, **kwargs) -> None:
         self.displayables = []
         if displayables:
```

### Comparing `pymolviz-1.1/pymolviz/meshes/Arrows.py` & `pymolviz-1.1.1/pymolviz/meshes/Arrows.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         transparency (float): Optional. Defaults to 0. The transparency value of the object.
         colormap: Optional. Defaults to "RdYlBu_r". Name of a colormap or a matplotlib colormap or a pymolviz.ColorMap object. Used to map values to colors.
         linewidth (float): Optional. Defaults to 1. The width of the lines. Seems to be currently not supported by PyMol.
         head_length (float): The relative length of the arrow head. Does not influence the length of the arrow itself.
         head_width (float): The relative width of the arrow head.
     """
 
-    def __init__(self, lines, color = "red", name = None, state = 1, transparency = 0, colormap = "RdYlBu_r", linewidth = 1, head_length = .2, head_width = .2, **kwargs) -> None:
+    def __init__(self, lines, color = "red", name = None, state = 1, transparency = 0, colormap = "RdYlBu_r", linewidth = 1, head_length = .2, head_width = .2, *args, **kwargs) -> None:
         try:
             if (not np.issubdtype(type(color), np.str_)):
                 if (len(color) == (len(lines.reshape(-1, 3)) / 2)):
                     color = np.repeat(color, 10, axis = 0)
                 elif (len(color) == len(lines.reshape(-1, 3))):
                     color = np.hstack([color[::2, None], np.repeat(color[1::2], 9, axis = 0).reshape(-1, 9)]).flatten()
         except TypeError:
@@ -44,9 +44,9 @@
             new_lines[i * 4] = np.hstack([end, x1])
             new_lines[i * 4 + 1] = np.hstack([end, x2])
             new_lines[i * 4 + 2] = np.hstack([end, y1])
             new_lines[i * 4 + 3] = np.hstack([end, y2])
         lines = np.hstack([original_lines, new_lines.reshape(-1, 24)])
                 
 
-        super().__init__(lines.reshape(-1, 3), color, name, state, transparency, colormap, linewidth, **kwargs)
+        super().__init__(lines.reshape(-1, 3), color, name, state, transparency, colormap, linewidth, *args, **kwargs)
         self.linewidth = linewidth
```

### Comparing `pymolviz-1.1/pymolviz/meshes/CGOCollection.py` & `pymolviz-1.1.1/pymolviz/meshes/CGOCollection.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 from ..Displayable import Displayable
 
 class CGOCollection(Displayable, list):
     """ A Collection is a container for different meshes. All meshes in a collection are rendered as a single CGO object.
     
     
     Attributes:
-        name (str): The name of the CGO object.
-        meshes (list): A list of meshes.
-        transformation (np.array): A 4x4 transformation matrix.
+        CGOs (list): A list of CGO objects.
+        name (str): Optional. Defaults to None. The name of the object.
+        state (int): Optional. Defaults to 1. The state of the object.
+        transparency (float): Optional. Defaults to 0. The transparency value of the object.
+
     """
 
 
 
     def __init__(self, CGOs : list = None, name : str = None, state : int = 1, transparency : float = 0) -> None:
         self.state = state
         self.transparency = transparency
```

### Comparing `pymolviz-1.1/pymolviz/meshes/Lines.py` & `pymolviz-1.1.1/pymolviz/meshes/Lines.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,22 @@
         state (int): Optional. Defaults to 1. The state of the object.
         transparency (float): Optional. Defaults to 0. The transparency value of the object.
         colormap: Optional. Defaults to "RdYlBu_r". Name of a colormap or a matplotlib colormap or a pymolviz.ColorMap object. Used to map values to colors.
         linewidth (float): Optional. Defaults to 1. The width of the lines. Seems to be currently not supported by PyMol.
 
     """
 
-    def __init__(self, lines : np.array, color = "red", name = None, state = 1, transparency = 0, colormap = "RdYlBu_r", linewidth = 1, **kwargs) -> None:
+    def __init__(self, lines : np.array, color = "red", name = None, state = 1, transparency = 0, colormap = "RdYlBu_r", linewidth = 1, *args, **kwargs) -> None:
         try:
             if (not np.issubdtype(type(color), np.str_)):
                 if (len(color) == (len(lines.reshape(-1, 3)) / 2)):
                     color = np.repeat(color, 2, axis = 0)
         except TypeError:
             pass
-        super().__init__(lines.reshape(-1, 3), color, name, state, transparency, colormap, **kwargs)
+        super().__init__(lines.reshape(-1, 3), color, name, state, transparency, colormap, *args, **kwargs)
         self.linewidth = linewidth
 
 
     def _create_CGO_list(self) -> str:
         """ Creates a CGO list from the mesh information. A line mesh will be created.
             CGO constants are kept as strings to avoid importing the pymol module.
```

### Comparing `pymolviz-1.1/pymolviz/meshes/Mesh.py` & `pymolviz-1.1.1/pymolviz/meshes/Mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,18 @@
         faces (np.array): A Nx3 array of faces.
         name (str): Optional. Defaults to None. The name of the object.
         state (int): Optional. Defaults to 1. The state of the object.
         transparency (float): Optional. Defaults to 0. The transparency value of the object.
         colormap: Optional. Defaults to "RdYlBu_r". Name of a colormap or a matplotlib colormap or a pymolviz.ColorMap object. Used to map values to colors.
     """
 
-    def __init__(self, vertices, color = "red", normals : np.array = None, faces : np.array = None, name = None, state = 1, transparency = 0, colormap = "RdYlBu_r", **kwargs) -> None:
+    def __init__(self, vertices, color = "red", normals : np.array = None, faces : np.array = None, name = None, state = 1, transparency = 0, colormap = "RdYlBu_r", *args, **kwargs) -> None:
         self.normals = np.array(normals, dtype=float).reshape(-1, 3) if normals is not None else np.zeros_like(vertices)
         self.faces = np.array(faces, dtype=int).reshape(-1, 3) if faces is not None else np.arange(vertices.shape[0]).reshape(-1, 3)
-        super().__init__(vertices.reshape(-1, 3), color, name, state, transparency, colormap, **kwargs)
+        super().__init__(vertices.reshape(-1, 3), color, name, state, transparency, colormap, *args, **kwargs)
         
     def to_wireframe(self, *args, **kwargs):
         """ Converts the mesh to a wireframe.
         
         Returns:
             Mesh: A wireframe mesh.
         """
```

### Comparing `pymolviz-1.1/pymolviz/meshes/Plane.py` & `pymolviz-1.1.1/pymolviz/meshes/Plane.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     def __init__(self, position, normal, scale = 5, color = "red", *args, **kwargs) -> None:
         """ Creates a plane mesh at the given position and with the given normal.
         
         Args:
             position (np.array): The position of the plane.
             normal (np.array): The normal of the plane.
             scale (float): The scale of the plane.
+            color (str): Optional. Defaults to "red". The color of the plane.
+            
             
             """
 
 
         self.position = position
         self.normal = normal / np.linalg.norm(normal)
```

### Comparing `pymolviz-1.1/pymolviz/meshes/Points.py` & `pymolviz-1.1.1/pymolviz/meshes/Points.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,24 +17,24 @@
         state (int): Optional. Defaults to 1. The state of the object.
         transparency (float): Optional. Defaults to 0. The transparency value of the object.
         colormap: Optional. Defaults to "RdYlBu_r". Name of a colormap or a matplotlib colormap or a pymolviz.ColorMap object. Used to map values to colors.
         render_as (str): Optional. Defaults to "Spheres". How to display the points. Can be "Spheres" or "Dots" or None. If None, the points are not displayed.
         radius (float): Optional. Defaults to .3. Only relevant if render_as is "Spheres". The radius of the spheres.
     """
 
-    def __init__(self, vertices, color = "red", name = None, state = 1, transparency = 0, colormap = "RdYlBu_r", render_as = "Spheres", radius = .3, **kwargs) -> None:
+    def __init__(self, vertices, color = "red", name = None, state = 1, transparency = 0, colormap = "RdYlBu_r", render_as = "Spheres", radius = .3, *args, **kwargs) -> None:
         super().__init__(name)
         if type(colormap) != ColorMap:
-            self.colormap = ColorMap(color, colormap, **kwargs)
+            self.colormap = ColorMap(color, colormap, state = state, name=f"{self.name}_colormap", *args, **kwargs)
         else:
             self.colormap = colormap
         if "single" in self.colormap._color_type: # colors were not inferred
             self.color = np.arange(vertices.shape[0]) # color is just the index
         else:
-            self.color = color.flatten()
+            self.color = np.array(color).flatten()
 
         self.vertices = np.array(vertices, dtype=float).reshape(-1, 3)
         self.render_as = render_as
         self.radius = radius
         self.state = state
         self.transparency = transparency
```

### Comparing `pymolviz-1.1/pymolviz/util/colors.py` & `pymolviz-1.1.1/pymolviz/util/colors.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,20 +21,23 @@
 			colormap = cm.get_cmap(colormap)
 	return colormap
 
 
 def _convert_string_color(color):
 		from .colors import get_AA_color, get_element_color
 		from matplotlib import colors
-		if not (c := get_AA_color(color)) is None:
-			color = c
-		elif not (c := get_element_color(color)) is None:
+		c = get_AA_color(color)
+		if not c is None:
 			color = c
 		else:
-			color = colors.to_rgb(color)
+			c = get_element_color(color)
+			if not c is None:
+				color = c
+			else:
+				color = colors.to_rgb(color)
 		return color
 #deprecated
 element_colors_jmol = {"H":	np.array([255,255,255]),
 "He":	np.array([217,255,255]),
 "Li":	np.array([204,128,255]),
 "Be":	np.array([194,255,0]),
 "B":	np.array([255,181,181]),
```

### Comparing `pymolviz-1.1/pymolviz/util/geometries.py` & `pymolviz-1.1.1/pymolviz/util/geometries.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1/pymolviz/util/io.py` & `pymolviz-1.1.1/pymolviz/util/io.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1/pymolviz/util/math.py` & `pymolviz-1.1.1/pymolviz/util/math.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1/pymolviz/volumetric/GridData.py` & `pymolviz-1.1.1/pymolviz/volumetric/GridData.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
         """
 
 
         self.step_sizes = step_sizes
         self.step_counts = step_counts
         self.origin = origin
 
+        values = np.array(values).flatten()
+
         # no grid points given: infer grid from parameters
         if positions is None:
             if (self.step_counts is None) or (self.step_sizes is None):
                 raise ValueError("Either positions or step_sizes and step_counts must be given.")
             else:
                 sorted_indices = np.arange(len(values))
             if origin is None:
@@ -47,17 +49,19 @@
                     self.step_counts[i] = np.round(length / self.step_sizes[i])
             # determine origin
             if self.origin is None:
                 self.origin = np.min(positions, axis=0)
 
 
         # sort values
+        self.step_counts = np.array(self.step_counts, dtype=int)
+        if len(values) != np.product(self.step_counts + 1):
+            raise ValueError(f"Number of values ({len(values)}) does not match number of grid points ({np.product(self.step_counts + 1)}).")
         self.values = values[sorted_indices]
         self.step_sizes = np.array(self.step_sizes)
-        self.step_counts = np.array(self.step_counts, dtype=int)
 
         super().__init__(name = name)
           
 
     def get_positions(self):
         x = np.linspace(self.origin[0], self.origin[0] + self.step_sizes[0] * self.step_counts[0], self.step_counts[0] + 1)
         y = np.linspace(self.origin[1], self.origin[1] + self.step_sizes[1] * self.step_counts[1], self.step_counts[1] + 1)
@@ -92,14 +96,16 @@
 
     def _script_string(self):
         values = self.values.reshape(self.step_counts.astype(int) + 1)
         result = f"""
 {self.name}_data = np.array({np.array2string(values, threshold=1e15, separator=",")})
 {self.name} = Brick.from_numpy({self.name}_data, {np.array2string(self.step_sizes, separator = ",")}, origin={np.array2string(self.origin, separator=",")})
 cmd.load_brick({self.name}, "{self.name}")
+{self.name}_data = None
+
 """
         return result
 
     def from_ccp4(path):
         """
         Creates a RegularData object from a CCP4 file.
```

### Comparing `pymolviz-1.1/pymolviz/volumetric/IrregularData.py` & `pymolviz-1.1.1/pymolviz/volumetric/IrregularData.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1/pymolviz/volumetric/IsoMesh.py` & `pymolviz-1.1.1/pymolviz/volumetric/IsoMesh.py`

 * *Files identical despite different names*

### Comparing `pymolviz-1.1/pymolviz/volumetric/IsoSurface.py` & `pymolviz-1.1.1/pymolviz/volumetric/IsoSurface.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 class IsoSurface(Displayable):
     def __init__(self, grid_data : GridData, level: float, name = None, color = None, transparency = 0, selection = None, carve = None, side = 1):
         """ 
         Computes and collects pymol commands to load in regular data and display an iso mesh at the given level.
         Note that, since this is based on volumetric data it is different from the pmv.Mesh class.
 
         Args:
-            grid_data (pymolviz.RegularData): Regular data for which to show the isomesh.
-            level (float): The level at which to display the isomesh.
-            name (str, optional): The name of the mesh as displayed in PyMOL. Defaults to {grid_data.name}_{value_label}_IsoMesh_{i}.
-            value_label (str, optional): The name of the value to use from the regular data. Defaults to None. Must be passed if grid_data has multiple values.
-            color (str or rgb or pymolviz.ColorRamp, optional): The name of the color to use or rgb values or a pymolviz ColorRamp which will be used to color based on position. Defaults to white. 
-            transparency (float): Transparancy of the surface, defaults to 1.
-            selection (str, optional): The selection to use. Defaults to None.
-            carve (float, optional): The carve to use. Defaults to None.
-            side (int, optional): The side of the isosurface to show. Defaults to 1 (outside/gradient facing).
-            in_sigma (bool, optional): Whether the level is in sigma. Defaults to False.
+            grid_data (pymolviz.GridData): The data to use for the iso surface.
+            level (float): The level at which to display the iso surface.
+            name (str): Optional. Defaults to None. The name of the object.
+            color (str or list of float): Optional. Defaults to None. The color of the object.
+            transparency (float): Optional. Defaults to 0. The transparency value of the object.
+            selection (str): Optional. Defaults to None. The selection to use.
+            carve (float): Optional. Defaults to None. The carve value to use.
+            side (int): Optional. Defaults to 1. The side to use.
+            
         """
         
         self.side = side
         self.transparency = transparency
         self.grid_data = grid_data
 
         self.level = level
```

### Comparing `pymolviz-1.1/pymolviz/volumetric/IsoVolume.py` & `pymolviz-1.1.1/pymolviz/volumetric/IsoVolume.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 
 class IsoVolume(Volume):
     def __init__(self, grid_data : GridData, name = None, colormap = "RdYlBu_r", alphas = None, clims = None, selection = None, carve = None, margin = 0.05, state = 1):
         """ 
         Computes and collects pymol commands to load in regular data and display it as multiple, transparent, same colored iso-surfaces using PyMOLs volume command.
 
         Args:
-            grid_data (pymolviz.RegularData): Regular data for which to show the volume.
-            name (str, optional): The name of the volume as displayed in PyMOL. Defaults to {grid_data.name}_{value_label}_IsoVolume_{i}.
-            value_label (str, optional): The name of the value to use from the regular data. Defaults to None. Must be passed if grid_data has multiple values.
-            colormap (str, optional): The name of the colormap to use. Defaults to coolwarm.
-            alphas (np.array, optional): The alphas to use. Defaults to [0.1, 0.5, 0.8].
-            clims (np.array, optional): The clims to use. Defaults to [mean - 2 stddev, mean, mean + 2 stddev].
-            selection (str, optional): The selection to use. Defaults to None.
-            carve (float, optional): The carve to use. Defaults to None.
+            grid_data (pymolviz.GridData): The data to use for the iso surface.
+            name (str): Optional. Defaults to None. The name of the object.
+            colormap (str or list of float): Optional. Defaults to "RdYlBu_r". The colormap of the object.
+            alphas (list of float): Optional. Defaults to None. The alpha values to use.
+            clims (list of float): Optional. Defaults to None. The color limits to use.
+            selection (str): Optional. Defaults to None. The selection to use.
+            carve (float): Optional. Defaults to None. The carve value to use.
+            margin (float): Optional. Defaults to 0.05. The margin to use.
+            state (int): Optional. Defaults to 1. The state to use.
+            
+           
         """
         if clims is None:
             # for some reason it seems that isolines are only shown on 16th of 5*std + mean
             self.clims = np.linspace(-np.std(grid_data.values) * 5 + np.mean(grid_data.values), np.std(grid_data.values) * 5 + np.mean(grid_data.values), 33)
         else:
             self.clims = clims
```

### Comparing `pymolviz-1.1/pymolviz/volumetric/Volume.py` & `pymolviz-1.1.1/pymolviz/volumetric/Volume.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
             grid_data (pymolviz.RegularData): Regular data for which to show the volume.
             name (str, optional): The name of the volume as displayed in PyMOL. Defaults to {grid_data.name}_{value_label}_Volume_{i}.
             colormap (str, optional): The name of the colormap to use. Defaults to coolwarm.
             alphas (np.array, optional): The alphas to use. Defaults to [0.03, 0.005, 0.1].
             clims (np.array, optional): The clims to use. Defaults to [mean - 2 stddev, mean, mean + 2 stddev].
             selection (str, optional): The selection to use. Defaults to None.
             carve (float, optional): The carve to use. Defaults to None.
+            state (int, optional): The state to use. Defaults to 1.
         """
 
         self.grid_data = grid_data
         self.selection = selection
         self.carve = carve
         self.state = state
 
@@ -33,15 +34,15 @@
             # getting number of values within each bin
             self.clims = np.vstack([self.clims[:-1], self.clims[1:]]).T.flatten()
             self.clims = np.hstack([self.clims, self.clims[-1]])
         else:
             self.clims = clims
 
         if not issubclass(type(colormap), ColorMap):
-            colormap = ColorMap(self.grid_data.values, colormap)
+            colormap = ColorMap(self.grid_data.values, colormap, state = state, name = f"{self.name}_colormap")
         self.colormap = colormap
 
         if alphas is None:
             used_length = len(self.clims)-(len(self.clims) % 2) # if length is uneven, we forgo the last value for binning
             bins = np.reshape(self.clims[:used_length], (-1, 2))
             densities = np.sum((bins[:,0] < self.grid_data.values[:, None]) & (bins[:,1] >= self.grid_data.values[:, None]), axis = 0)
             densities = densities / np.sum(densities)
```

### Comparing `pymolviz-1.1/pymolviz.egg-info/SOURCES.txt` & `pymolviz-1.1.1/pymolviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

