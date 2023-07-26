# Comparing `tmp/landfall-0.3.2.tar.gz` & `tmp/landfall-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landfall-0.3.2.tar", last modified: Tue Jul 25 16:57:28 2023, max compression
+gzip compressed data, was "landfall-0.3.3.tar", last modified: Wed Jul 26 17:59:54 2023, max compression
```

## Comparing `landfall-0.3.2.tar` & `landfall-0.3.3.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 16:57:28.968345 landfall-0.3.2/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.3.2/LICENSE
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1822 2023-07-25 16:57:28.968497 landfall-0.3.2/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1195 2023-07-25 16:31:00.000000 landfall-0.3.2/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.3.2/pyproject.toml
--rw-r--r--   0 odosmatthews   (501) staff       (20)      926 2023-07-25 16:57:28.969753 landfall-0.3.2/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-07-25 16:48:54.000000 landfall-0.3.2/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 16:57:28.955928 landfall-0.3.2/src/
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 16:57:28.964081 landfall-0.3.2/src/landfall/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      216 2023-07-25 16:49:22.000000 landfall-0.3.2/src/landfall/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.3.2/src/landfall/color.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.3.2/src/landfall/colorsys.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      865 2023-07-24 18:54:39.000000 landfall-0.3.2/src/landfall/combos.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      484 2023-07-25 14:24:09.000000 landfall-0.3.2/src/landfall/context.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.3.2/src/landfall/distinctipy.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     3526 2023-07-25 15:14:16.000000 landfall-0.3.2/src/landfall/points.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2213 2023-07-24 18:49:22.000000 landfall-0.3.2/src/landfall/polygons.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-25 16:57:28.968023 landfall-0.3.2/src/landfall.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1822 2023-07-25 16:57:28.000000 landfall-0.3.2/src/landfall.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      460 2023-07-25 16:57:28.000000 landfall-0.3.2/src/landfall.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-25 16:57:28.000000 landfall-0.3.2/src/landfall.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.3.2/src/landfall.egg-info/not-zip-safe
--rw-r--r--   0 odosmatthews   (501) staff       (20)      118 2023-07-25 16:57:28.000000 landfall-0.3.2/src/landfall.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-25 16:57:28.000000 landfall-0.3.2/src/landfall.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 17:59:54.047772 landfall-0.3.3/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.3.3/LICENSE
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1818 2023-07-26 17:59:54.047880 landfall-0.3.3/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1191 2023-07-26 17:59:17.000000 landfall-0.3.3/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.3.3/pyproject.toml
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      926 2023-07-26 17:59:54.050996 landfall-0.3.3/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-07-25 16:48:54.000000 landfall-0.3.3/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 17:59:54.018114 landfall-0.3.3/src/
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 17:59:54.033083 landfall-0.3.3/src/landfall/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      216 2023-07-26 17:58:31.000000 landfall-0.3.3/src/landfall/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.3.3/src/landfall/color.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.3.3/src/landfall/colorsys.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      865 2023-07-24 18:54:39.000000 landfall-0.3.3/src/landfall/combos.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      508 2023-07-25 18:14:06.000000 landfall-0.3.3/src/landfall/context.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.3.3/src/landfall/distinctipy.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     3823 2023-07-25 18:27:07.000000 landfall-0.3.3/src/landfall/points.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2356 2023-07-26 17:57:35.000000 landfall-0.3.3/src/landfall/polygons.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 17:59:54.047237 landfall-0.3.3/src/landfall.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1818 2023-07-26 17:59:54.000000 landfall-0.3.3/src/landfall.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      481 2023-07-26 17:59:54.000000 landfall-0.3.3/src/landfall.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-26 17:59:54.000000 landfall-0.3.3/src/landfall.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.3.3/src/landfall.egg-info/not-zip-safe
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      118 2023-07-26 17:59:54.000000 landfall-0.3.3/src/landfall.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-26 17:59:54.000000 landfall-0.3.3/src/landfall.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 17:59:54.047538 landfall-0.3.3/tests/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      452 2023-07-25 18:31:53.000000 landfall-0.3.3/tests/test_points.py
```

### Comparing `landfall-0.3.2/LICENSE` & `landfall-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `landfall-0.3.2/PKG-INFO` & `landfall-0.3.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landfall
-Version: 0.3.2
+Version: 0.3.3
 Summary: Easy to use functions to plot geospatial data on maps using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
@@ -18,21 +18,21 @@
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE
 
 ![Landfall Logo](https://raw.githubusercontent.com/eddiethedean/landfall/main/docs/landfall_logo.png)
 -----------------
 
-# Landfall: Easy to use functions for plotting geographic points on static maps
+# Landfall: Easy to use functions for plotting geographic data on static maps
 [![PyPI Latest Release](https://img.shields.io/pypi/v/landfall.svg)](https://pypi.org/project/landfall/)
 ![Tests](https://github.com/eddiethedean/landfall/actions/workflows/tests.yml/badge.svg)
 
 ## What is it?
 
-**Landfall** is a Python package with easy to use functions for plotting geographic points on a static map.
+**Landfall** is a Python package with easy to use functions for plotting geographic data on a static map.
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/eddiethedean/landfall
 
 ```sh
 # PyPI
```

### Comparing `landfall-0.3.2/README.md` & `landfall-0.3.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ![Landfall Logo](https://raw.githubusercontent.com/eddiethedean/landfall/main/docs/landfall_logo.png)
 -----------------
 
-# Landfall: Easy to use functions for plotting geographic points on static maps
+# Landfall: Easy to use functions for plotting geographic data on static maps
 [![PyPI Latest Release](https://img.shields.io/pypi/v/landfall.svg)](https://pypi.org/project/landfall/)
 ![Tests](https://github.com/eddiethedean/landfall/actions/workflows/tests.yml/badge.svg)
 
 ## What is it?
 
-**Landfall** is a Python package with easy to use functions for plotting geographic points on a static map.
+**Landfall** is a Python package with easy to use functions for plotting geographic data on a static map.
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/eddiethedean/landfall
 
 ```sh
 # PyPI
```

### Comparing `landfall-0.3.2/setup.cfg` & `landfall-0.3.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = landfall
-version = 0.3.2
+version = 0.3.3
 description = Easy to use functions to plot geospatial data on maps using staticmaps.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 author = Odos Matthews
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
```

### Comparing `landfall-0.3.2/src/landfall/color.py` & `landfall-0.3.3/src/landfall/color.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.2/src/landfall/colorsys.py` & `landfall-0.3.3/src/landfall/colorsys.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.2/src/landfall/combos.py` & `landfall-0.3.3/src/landfall/combos.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.2/src/landfall/points.py` & `landfall-0.3.3/src/landfall/points.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,17 +22,20 @@
     id_colors: Optional[Union[Mapping, str]] = None,
     tile_provider=tp,
     point_size=10,
     window_size=(500, 400),
     zoom=0,
     color=staticmaps.color.BLUE,
     set_zoom=None,
-    flip_coords=False
+    flip_coords=False,
+    context: Optional[staticmaps.Context] = None
 ) -> Image:
-    context = staticmaps.Context()
+    if context is None:
+        context = staticmaps.Context()
+
     context.set_tile_provider(tile_provider)
     count = len(latitudes)
 
     if longitudes is None:
         latitudes, longitudes = points_to_lats_lons(latitudes)
 
     if flip_coords:
@@ -68,15 +71,16 @@
     ids_name: Optional[str] = None,
     id_colors: Optional[Union[Mapping, str]] = None,
     tile_provider=tp,
     point_size=10,
     window_size=(500, 400),
     zoom=0,
     color=staticmaps.color.BLUE,
-    set_zoom=None
+    set_zoom=None,
+    context: Optional[staticmaps.Context] = None
 ) -> Image:
     lats = data[latitude_name]
     lons = data[longitude_name]
     colors_values = None if color_name is None else data[color_name]
     if colors_values is None and colors is not None:
         colors_values = colors
     ids_values = None if ids_name is None else data[ids_name]
@@ -88,15 +92,16 @@
         ids=ids_values,
         id_colors=id_colors,
         tile_provider=tile_provider,
         point_size=point_size,
         window_size=window_size,
         zoom=zoom,
         color=color,
-        set_zoom=set_zoom)
+        set_zoom=set_zoom,
+        context=context)
 
 
 def points_to_lats_lons(
     points: Sequence[Sequence[float]]
 ) -> Tuple[Sequence[float], Sequence[float]]:
     latitudes, longitudes = zip(*points)
     return latitudes, longitudes
@@ -107,24 +112,26 @@
     return plot_points(latitudes, longitudes, **kwargs)
 
 
 def add_point(
     context: staticmaps.Context,
     lat: float,
     lon: float,
-    color: staticmaps.Color,
-    point_size: int
+    color: staticmaps.Color = staticmaps.color.BLUE,
+    point_size: int = 10
 ) -> None:
     point = staticmaps.create_latlng(lat, lon)
     marker = staticmaps.Marker(point, color=color, size=point_size)
     context.add_object(marker)
 
 
 def add_points(
         context: staticmaps.Context,
         latitudes: Sequence[float],
         longitudes: Sequence[float],
-        colors: Sequence[staticmaps.Color],
-        point_size: int
+        colors: Optional[Sequence[staticmaps.Color]] = None,
+        point_size: int = 10
 ) -> None:
+    if colors is None:
+        colors = list(repeat(staticmaps.color.BLUE, len(latitudes)))
     for lat, lon, clr in zip(latitudes, longitudes, colors):
         add_point(context, lat, lon, clr, point_size)
```

### Comparing `landfall-0.3.2/src/landfall/polygons.py` & `landfall-0.3.3/src/landfall/polygons.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Functions for plotting polygons.
 """
-from typing import Iterable, List, Tuple
+from typing import Iterable, List, Optional, Tuple
 import staticmaps
 from PIL.Image import Image
 
 tp = staticmaps.tile_provider_OSM
 TRED = staticmaps.Color(255, 0, 0, 100)
 RED = staticmaps.RED
 
@@ -22,49 +22,53 @@
 
 def plot_polygons(
         polygons,
         tileprovider=tp,
         fill_color=TRED,
         color=RED,
         width=2,
-        size=(800, 600),
-        flip_coords=False
+        size=(500, 400),
+        flip_coords=False,
+        context: Optional[staticmaps.Context] = None
 ) -> Image:
-    context = staticmaps.Context()
+    if context is None:
+        context = staticmaps.Context()
     context.set_tile_provider(tileprovider)
     if flip_coords:
         polygons = [flip_polygon_coords(polygon) for polygon in polygons]
     add_polygons(context, polygons, fill_color=fill_color, width=width, color=color)
     return context.render_pillow(*size) # type: ignore
 
 
 def plot_polygon(
-        polygon: Iterable[Tuple[float, float]],
-        tileprovider=tp,
-        fill_color=TRED,
-        color=RED,
-        width=2,
-        size=(800, 600),
-        flip_coords=False
+    polygon: Iterable[Tuple[float, float]],
+    tileprovider=tp,
+    fill_color=TRED,
+    color=RED,
+    width=2,
+    size=(500, 400),
+    flip_coords=False,
+    context: Optional[staticmaps.Context] = None
 ) -> Image:
-    context = staticmaps.Context()
+    if context is None:
+        context = staticmaps.Context()
     context.set_tile_provider(tileprovider)
     if flip_coords:
         polygon = flip_polygon_coords(polygon)
     add_polygon(context, polygon, fill_color=fill_color, width=width, color=color)
     return context.render_pillow(*size) # type: ignore
 
 
 def add_polygon(
     context: staticmaps.Context,
     polygon: Iterable[Tuple[float, float]],
     fill_color,
     width,
     color,
-    flip_coords=False
+    flip_coords=False,
 ) -> None:
     if flip_coords:
         polygon = flip_polygon_coords(polygon)
     context.add_object(staticmaps.Area(
         create_polygon_points(polygon),
         fill_color=fill_color,
         width=width,
```

### Comparing `landfall-0.3.2/src/landfall.egg-info/PKG-INFO` & `landfall-0.3.3/src/landfall.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landfall
-Version: 0.3.2
+Version: 0.3.3
 Summary: Easy to use functions to plot geospatial data on maps using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
@@ -18,21 +18,21 @@
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE
 
 ![Landfall Logo](https://raw.githubusercontent.com/eddiethedean/landfall/main/docs/landfall_logo.png)
 -----------------
 
-# Landfall: Easy to use functions for plotting geographic points on static maps
+# Landfall: Easy to use functions for plotting geographic data on static maps
 [![PyPI Latest Release](https://img.shields.io/pypi/v/landfall.svg)](https://pypi.org/project/landfall/)
 ![Tests](https://github.com/eddiethedean/landfall/actions/workflows/tests.yml/badge.svg)
 
 ## What is it?
 
-**Landfall** is a Python package with easy to use functions for plotting geographic points on a static map.
+**Landfall** is a Python package with easy to use functions for plotting geographic data on a static map.
 
 ## Where to get it
 The source code is currently hosted on GitHub at:
 https://github.com/eddiethedean/landfall
 
 ```sh
 # PyPI
```

