# Comparing `tmp/landfall-0.3.3.tar.gz` & `tmp/landfall-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landfall-0.3.3.tar", last modified: Wed Jul 26 17:59:54 2023, max compression
+gzip compressed data, was "landfall-0.3.4.tar", last modified: Wed Jul 26 18:24:54 2023, max compression
```

## Comparing `landfall-0.3.3.tar` & `landfall-0.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 17:59:54.047772 landfall-0.3.3/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.3.3/LICENSE
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1818 2023-07-26 17:59:54.047880 landfall-0.3.3/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1191 2023-07-26 17:59:17.000000 landfall-0.3.3/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.3.3/pyproject.toml
--rw-r--r--   0 odosmatthews   (501) staff       (20)      926 2023-07-26 17:59:54.050996 landfall-0.3.3/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-07-25 16:48:54.000000 landfall-0.3.3/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 17:59:54.018114 landfall-0.3.3/src/
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 17:59:54.033083 landfall-0.3.3/src/landfall/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      216 2023-07-26 17:58:31.000000 landfall-0.3.3/src/landfall/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.3.3/src/landfall/color.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.3.3/src/landfall/colorsys.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      865 2023-07-24 18:54:39.000000 landfall-0.3.3/src/landfall/combos.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      508 2023-07-25 18:14:06.000000 landfall-0.3.3/src/landfall/context.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.3.3/src/landfall/distinctipy.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     3823 2023-07-25 18:27:07.000000 landfall-0.3.3/src/landfall/points.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2356 2023-07-26 17:57:35.000000 landfall-0.3.3/src/landfall/polygons.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 17:59:54.047237 landfall-0.3.3/src/landfall.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1818 2023-07-26 17:59:54.000000 landfall-0.3.3/src/landfall.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      481 2023-07-26 17:59:54.000000 landfall-0.3.3/src/landfall.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-26 17:59:54.000000 landfall-0.3.3/src/landfall.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.3.3/src/landfall.egg-info/not-zip-safe
--rw-r--r--   0 odosmatthews   (501) staff       (20)      118 2023-07-26 17:59:54.000000 landfall-0.3.3/src/landfall.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-26 17:59:54.000000 landfall-0.3.3/src/landfall.egg-info/top_level.txt
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 17:59:54.047538 landfall-0.3.3/tests/
--rw-r--r--   0 odosmatthews   (501) staff       (20)      452 2023-07-25 18:31:53.000000 landfall-0.3.3/tests/test_points.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 18:24:54.456950 landfall-0.3.4/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-02-28 17:06:52.000000 landfall-0.3.4/LICENSE
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1818 2023-07-26 18:24:54.457063 landfall-0.3.4/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1191 2023-07-26 17:59:17.000000 landfall-0.3.4/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-02-28 17:09:25.000000 landfall-0.3.4/pyproject.toml
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      926 2023-07-26 18:24:54.457994 landfall-0.3.4/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-07-25 16:48:54.000000 landfall-0.3.4/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 18:24:54.441738 landfall-0.3.4/src/
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 18:24:54.451719 landfall-0.3.4/src/landfall/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      216 2023-07-26 18:24:02.000000 landfall-0.3.4/src/landfall/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1848 2023-03-06 19:27:35.000000 landfall-0.3.4/src/landfall/color.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      631 2023-03-06 17:06:44.000000 landfall-0.3.4/src/landfall/colorsys.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      865 2023-07-24 18:54:39.000000 landfall-0.3.4/src/landfall/combos.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      508 2023-07-25 18:14:06.000000 landfall-0.3.4/src/landfall/context.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      271 2023-03-06 17:06:44.000000 landfall-0.3.4/src/landfall/distinctipy.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     3823 2023-07-25 18:27:07.000000 landfall-0.3.4/src/landfall/points.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2384 2023-07-26 18:23:23.000000 landfall-0.3.4/src/landfall/polygons.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 18:24:54.456480 landfall-0.3.4/src/landfall.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1818 2023-07-26 18:24:54.000000 landfall-0.3.4/src/landfall.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      481 2023-07-26 18:24:54.000000 landfall-0.3.4/src/landfall.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-07-26 18:24:54.000000 landfall-0.3.4/src/landfall.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-02-28 18:06:53.000000 landfall-0.3.4/src/landfall.egg-info/not-zip-safe
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      118 2023-07-26 18:24:54.000000 landfall-0.3.4/src/landfall.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-07-26 18:24:54.000000 landfall-0.3.4/src/landfall.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-07-26 18:24:54.456743 landfall-0.3.4/tests/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      452 2023-07-25 18:31:53.000000 landfall-0.3.4/tests/test_points.py
```

### Comparing `landfall-0.3.3/LICENSE` & `landfall-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `landfall-0.3.3/PKG-INFO` & `landfall-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landfall
-Version: 0.3.3
+Version: 0.3.4
 Summary: Easy to use functions to plot geospatial data on maps using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `landfall-0.3.3/README.md` & `landfall-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `landfall-0.3.3/setup.cfg` & `landfall-0.3.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = landfall
-version = 0.3.3
+version = 0.3.4
 description = Easy to use functions to plot geospatial data on maps using staticmaps.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 author = Odos Matthews
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
```

### Comparing `landfall-0.3.3/src/landfall/color.py` & `landfall-0.3.4/src/landfall/color.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.3/src/landfall/colorsys.py` & `landfall-0.3.4/src/landfall/colorsys.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.3/src/landfall/combos.py` & `landfall-0.3.4/src/landfall/combos.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.3/src/landfall/points.py` & `landfall-0.3.4/src/landfall/points.py`

 * *Files identical despite different names*

### Comparing `landfall-0.3.3/src/landfall/polygons.py` & `landfall-0.3.4/src/landfall/polygons.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,44 +22,44 @@
 
 def plot_polygons(
         polygons,
         tileprovider=tp,
         fill_color=TRED,
         color=RED,
         width=2,
-        size=(500, 400),
+        window_size=(500, 400),
         flip_coords=False,
         context: Optional[staticmaps.Context] = None
 ) -> Image:
     if context is None:
         context = staticmaps.Context()
     context.set_tile_provider(tileprovider)
     if flip_coords:
         polygons = [flip_polygon_coords(polygon) for polygon in polygons]
     add_polygons(context, polygons, fill_color=fill_color, width=width, color=color)
-    return context.render_pillow(*size) # type: ignore
+    return context.render_pillow(*window_size) # type: ignore
 
 
 def plot_polygon(
     polygon: Iterable[Tuple[float, float]],
     tileprovider=tp,
     fill_color=TRED,
     color=RED,
     width=2,
-    size=(500, 400),
+    window_size=(500, 400),
     flip_coords=False,
     context: Optional[staticmaps.Context] = None
 ) -> Image:
     if context is None:
         context = staticmaps.Context()
     context.set_tile_provider(tileprovider)
     if flip_coords:
         polygon = flip_polygon_coords(polygon)
     add_polygon(context, polygon, fill_color=fill_color, width=width, color=color)
-    return context.render_pillow(*size) # type: ignore
+    return context.render_pillow(*window_size) # type: ignore
 
 
 def add_polygon(
     context: staticmaps.Context,
     polygon: Iterable[Tuple[float, float]],
     fill_color,
     width,
```

### Comparing `landfall-0.3.3/src/landfall.egg-info/PKG-INFO` & `landfall-0.3.4/src/landfall.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landfall
-Version: 0.3.3
+Version: 0.3.4
 Summary: Easy to use functions to plot geospatial data on maps using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

