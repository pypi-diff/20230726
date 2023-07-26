# Comparing `tmp/pygeoops-0.2.0a2.tar.gz` & `tmp/pygeoops-0.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoops-0.2.0a2.tar", last modified: Mon Jul 24 17:33:39 2023, max compression
+gzip compressed data, was "pygeoops-0.2.0a3.tar", last modified: Wed Jul 26 15:14:18 2023, max compression
```

## Comparing `pygeoops-0.2.0a2.tar` & `pygeoops-0.2.0a3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:33:39.505299 pygeoops-0.2.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-24 17:33:39.505299 pygeoops-0.2.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:33:39.501299 pygeoops-0.2.0a2/pygeoops/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10309 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_simplify_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_simplify_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/_view_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pygeoops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:33:39.505299 pygeoops-0.2.0a2/pygeoops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-24 17:33:39.000000 pygeoops-0.2.0a2/pygeoops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-24 17:33:39.000000 pygeoops-0.2.0a2/pygeoops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 17:33:39.000000 pygeoops-0.2.0a2/pygeoops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 17:33:39.000000 pygeoops-0.2.0a2/pygeoops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 17:33:39.000000 pygeoops-0.2.0a2/pygeoops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 17:33:39.505299 pygeoops-0.2.0a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 17:33:39.505299 pygeoops-0.2.0a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_centerline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12597 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_simplify_lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_simplify_topo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-24 17:33:27.000000 pygeoops-0.2.0a2/tests/test_view_angles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:14:18.818250 pygeoops-0.2.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-26 15:14:18.818250 pygeoops-0.2.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:14:18.814250 pygeoops-0.2.0a3/pygeoops/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_simplify_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_simplify_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/_view_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pygeoops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:14:18.818250 pygeoops-0.2.0a3/pygeoops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-07-26 15:14:18.000000 pygeoops-0.2.0a3/pygeoops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-26 15:14:18.000000 pygeoops-0.2.0a3/pygeoops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:14:18.000000 pygeoops-0.2.0a3/pygeoops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-26 15:14:18.000000 pygeoops-0.2.0a3/pygeoops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 15:14:18.000000 pygeoops-0.2.0a3/pygeoops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-26 15:14:18.818250 pygeoops-0.2.0a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:14:18.818250 pygeoops-0.2.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_centerline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_simplify_lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_simplify_topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-26 15:14:08.000000 pygeoops-0.2.0a3/tests/test_view_angles.py
```

### Comparing `pygeoops-0.2.0a2/LICENSE.txt` & `pygeoops-0.2.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/PKG-INFO` & `pygeoops-0.2.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoops
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: Library with some less common or extended spatial functions
 Author-email: Pieter Roggemans <pieter.roggemans@gmail.com>
 Project-URL: Homepage, https://github.com/pygeoops/pygeoops
 Project-URL: Bug Tracker, https://github.com/pygeoops/pygeoops/issues
 Keywords: GIS,cartography,pandas,shapely,geopandas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pygeoops-0.2.0a2/README.md` & `pygeoops-0.2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/pygeoops/_centerline.py` & `pygeoops-0.2.0a3/pygeoops/_centerline.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/pygeoops/_general.py` & `pygeoops-0.2.0a3/pygeoops/_general.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/pygeoops/_grid.py` & `pygeoops-0.2.0a3/pygeoops/_grid.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/pygeoops/_simplify.py` & `pygeoops-0.2.0a3/pygeoops/_simplify.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,17 +43,19 @@
     Args:
         geometry (geometry or array_like): a geometry or ndarray of geometries.
         tolerance (float): mandatory for the following algorithms:
             * "rdp": distance to use as tolerance
             * "lang": distance to use as tolerance
             * "vw": area to use as tolerance
         algorithm (str, optional): algorithm to use. Defaults to "rdp".
-            * "rdp": Ramer Douglas Peuker
-            * "lang": Lang
-            * "vw": Visvalingal Whyatt
+            * "rdp": Ramer Douglas Peuker algorithm
+            * "lang": Lang algorithm
+            * "lang+": Lang-based algorithm, but without limit of having at least
+              nb_input_coordinates/lookahead points in the simplified output.
+            * "vw": Visvalingal Whyatt algorithm
         lookahead (int, optional): the number of points to consider for removing
             in a moving window. Used for LANG algorithm. Defaults to 8.
         preserve_topology (bool, optional): True to (try to) return valid
             geometries as result. Defaults to True.
         preserve_common_bounderies (bool, optional): True to (try to) maintain common
             boundaries between all geometries in the input geometry list.
             Defaults to False.
@@ -65,14 +67,15 @@
 
     Returns:
         Union[BaseGeometry, NDArray[BaseGeometry], GeoSeries, None]: the
             simplified version of the input geometry/geometries.
     """
     if geometry is None:
         return None
+    algorithm = algorithm.lower()
 
     # If common boundaries need to be preserved, use topologic implementation
     if preserve_common_boundaries:
         if not preserve_topology:
             raise ValueError(
                 "The combination of preserve_common_boundaries=True and "
                 "preserve_topology=False is not supported."
@@ -121,143 +124,56 @@
     lookahead: int = 8,
     preserve_topology: bool = True,
     keep_points_on: Optional[BaseGeometry] = None,
 ) -> Optional[BaseGeometry]:
     # Init:
     if geometry is None:
         return None
+
+    # Check algorythm
+    algorithm = algorithm.lower()
+    simplify_lookahead_points = False
     if algorithm in ["rdp", "vw"]:
         if not HAS_SIMPLIFICATION:
             raise ImportError(
                 "To use simplify_ext using rdp or vw, first install simplification "
                 "with 'pip install simplification'"
             )
     elif algorithm == "lang":
         pass
+    elif "lang+":
+        simplify_lookahead_points = True
     else:
-        raise ValueError(f"Unsupported algorythm specified: {algorithm}")
-
-    # Define some inline funtions
-    # Apply the simplification (can result in multipolygons)
-    def simplify_polygon(
-        polygon: shapely.Polygon, keep_points_on: Optional[BaseGeometry]
-    ) -> Union[shapely.Polygon, shapely.MultiPolygon, None]:
-        # First simplify exterior ring
-        assert polygon.exterior is not None
-        exterior_simplified = simplify_coords(polygon.exterior.coords, keep_points_on)
-
-        # If topology needs to be preserved, keep original ring if simplify results in
-        # None or not enough points
-        if preserve_topology is True and (
-            exterior_simplified is None or len(exterior_simplified) < 3
-        ):
-            exterior_simplified = polygon.exterior.coords
-
-        # Now simplify interior rings
-        interiors_simplified = []
-        for interior in polygon.interiors:
-            interior_simplified = simplify_coords(interior.coords, keep_points_on)
-
-            # If simplified version is ring, add it
-            if interior_simplified is not None and len(interior_simplified) >= 3:
-                interiors_simplified.append(interior_simplified)
-            elif preserve_topology is True:
-                # If result is no ring, but topology needs to be preserved,
-                # add original ring
-                interiors_simplified.append(interior.coords)
-
-        result_poly = shapely.Polygon(exterior_simplified, interiors_simplified)
-
-        # Extract only polygons as result + try to make valid
-        result_poly = general.collection_extract(
-            shapely.make_valid(result_poly), primitivetype=PrimitiveType.POLYGON
-        )
-
-        # If the result is None and the topology needs to be preserved, return
-        # original polygon
-        if preserve_topology is True and result_poly is None:
-            return polygon
-
-        return result_poly
-
-    def simplify_linestring(
-        linestring: shapely.LineString, keep_points_on: Optional[BaseGeometry]
-    ) -> shapely.LineString:
-        # If the linestring cannot be simplified, return it
-        if linestring is None or len(linestring.coords) <= 2:
-            return linestring
-
-        # Simplify
-        coords_simplified = simplify_coords(linestring.coords, keep_points_on)
-
-        # If preserve_topology is True and the result is no line anymore, return
-        # original line
-        if preserve_topology is True and (
-            coords_simplified is None or len(coords_simplified) < 2
-        ):
-            return linestring
-        else:
-            return shapely.LineString(coords_simplified)
-
-    def simplify_coords(
-        coords: Union[np.ndarray, shapely.coords.CoordinateSequence],
-        keep_points_on: Optional[BaseGeometry],
-    ) -> np.ndarray:
-        if isinstance(coords, shapely.coords.CoordinateSequence):
-            coords = np.asarray(coords)
-        # Determine the indexes of the coordinates to keep after simplification
-        if algorithm == "rdp":
-            coords_simplify_idx = simplification.simplify_coords_idx(coords, tolerance)
-        elif algorithm == "vw":
-            coords_simplify_idx = simplification.simplify_coords_vw_idx(
-                coords, tolerance
-            )
-        elif algorithm == "lang":
-            coords_simplify_idx = simplify_lang.simplify_coords_lang_idx(
-                coords, tolerance, lookahead=lookahead
-            )
-        else:
-            raise ValueError(f"Unsupported algorithm: {algorithm}")
-
-        coords_on_border_idx = []
-        if keep_points_on is not None:
-            # Check if there are coordinates that would be removed that should be kept
-            shapely.prepare(keep_points_on)
-            coords_to_drop_mask = np.ones(len(coords), dtype=int)
-            coords_to_drop_mask[coords_simplify_idx] = 0
-            coords_to_drop_idx = coords_to_drop_mask.nonzero()[0]
-
-            coords_points = shapely.points(coords[coords_to_drop_idx])
-            coords_to_drop_on_border = keep_points_on.intersects(coords_points)
-            coords_on_border_idx = coords_to_drop_idx[coords_to_drop_on_border]
-
-        # Extracts coordinates that need to be kept
-        coords_to_keep = coords_simplify_idx
-        if len(coords_on_border_idx) > 0:
-            coords_to_keep = np.concatenate(
-                [coords_to_keep, coords_on_border_idx], dtype=np.int64
-            )
-            coords_to_keep = np.sort(coords_to_keep)
-
-        return coords[coords_to_keep]
+        raise ValueError(f"Unsupported algorithm specified: {algorithm}")
 
     # Loop over the rings, and simplify them one by one...
     # If the geometry is None, just return...
-    if geometry is None:
-        raise ValueError("geom input parameter should not be None")
-    elif isinstance(geometry, shapely.Point):
-        # Point cannot be simplified
-        return geometry
-    elif isinstance(geometry, shapely.MultiPoint):
-        # MultiPoint cannot be simplified
+    if isinstance(geometry, (shapely.Point, shapely.MultiPoint)):
+        # Point or MultiPoint cannot be simplified
         return geometry
     elif isinstance(geometry, shapely.LineString):
-        result_geom = simplify_linestring(geometry, keep_points_on)
+        result_geom = simplify_linestring(
+            linestring=geometry,
+            tolerance=tolerance,
+            algorithm=algorithm,
+            lookahead=lookahead,
+            simplify_lookahead_points=simplify_lookahead_points,
+            preserve_topology=preserve_topology,
+            keep_points_on=keep_points_on,
+        )
     elif isinstance(geometry, shapely.Polygon):
-        result_geom = simplify_polygon(geometry, keep_points_on)
+        result_geom = simplify_polygon(
+            polygon=geometry,
+            tolerance=tolerance,
+            algorithm=algorithm,
+            lookahead=lookahead,
+            simplify_lookahead_points=simplify_lookahead_points,
+            preserve_topology=preserve_topology,
+            keep_points_on=keep_points_on,
+        )
     elif isinstance(geometry, BaseMultipartGeometry):
         # If it is a multi-part, recursively call simplify for all parts.
         simplified_geometries = [
             _simplify(
                 geom,
                 tolerance=tolerance,
                 algorithm=algorithm,
@@ -268,7 +184,148 @@
             for geom in geometry.geoms
         ]
         result_geom = general.collect(simplified_geometries)
     else:
         raise ValueError(f"Unsupported geometrytype: {geometry}")
 
     return shapely.make_valid(result_geom)
+
+
+# Apply the simplification (can result in multipolygons)
+def simplify_polygon(
+    polygon: shapely.Polygon,
+    tolerance: float,
+    algorithm: str,
+    lookahead: int,
+    simplify_lookahead_points: bool,
+    preserve_topology: bool,
+    keep_points_on: Optional[BaseGeometry],
+) -> Union[shapely.Polygon, shapely.MultiPolygon, None]:
+    # First simplify exterior ring
+    assert polygon.exterior is not None
+    exterior_simpl = simplify_coords(
+        polygon.exterior.coords,
+        tolerance=tolerance,
+        algorithm=algorithm,
+        lookahead=lookahead,
+        simplify_lookahead_points=simplify_lookahead_points,
+        keep_points_on=keep_points_on,
+    )
+
+    # If topology needs to be preserved, keep original ring if simplify results is
+    # None or not enough points
+    if preserve_topology and (exterior_simpl is None or len(exterior_simpl) < 3):
+        exterior_simpl = polygon.exterior.coords
+
+    # Now simplify interior rings
+    interiors_simpl = []
+    for interior in polygon.interiors:
+        interior_simpl = simplify_coords(
+            coords=interior.coords,
+            tolerance=tolerance,
+            algorithm=algorithm,
+            lookahead=lookahead,
+            simplify_lookahead_points=simplify_lookahead_points,
+            keep_points_on=keep_points_on,
+        )
+
+        # If simplified version is ring, add it
+        if interior_simpl is not None and len(interior_simpl) >= 3:
+            interiors_simpl.append(interior_simpl)
+        elif preserve_topology:
+            # If result is no ring, but topology needs to be preserved,
+            # add original ring
+            interiors_simpl.append(interior.coords)
+
+    result_poly = shapely.Polygon(exterior_simpl, interiors_simpl)
+
+    # Extract only polygons as result + try to make valid
+    result_poly = general.collection_extract(
+        shapely.make_valid(result_poly), primitivetype=PrimitiveType.POLYGON
+    )
+
+    # If the result is None and the topology needs to be preserved, return
+    # original polygon
+    if preserve_topology and result_poly is None:
+        return polygon
+
+    return result_poly
+
+
+def simplify_linestring(
+    linestring: shapely.LineString,
+    tolerance: float,
+    algorithm: str,
+    lookahead: int,
+    simplify_lookahead_points: bool,
+    preserve_topology: bool,
+    keep_points_on: Optional[BaseGeometry],
+) -> shapely.LineString:
+    # If the linestring cannot be simplified, return it
+    if linestring is None or len(linestring.coords) <= 2:
+        return linestring
+
+    # Simplify
+    coords_simpl = simplify_coords(
+        coords=linestring.coords,
+        tolerance=tolerance,
+        algorithm=algorithm,
+        lookahead=lookahead,
+        simplify_lookahead_points=simplify_lookahead_points,
+        keep_points_on=keep_points_on,
+    )
+
+    # If preserve_topology is True and the result is no line anymore, return
+    # original line
+    if preserve_topology and (coords_simpl is None or len(coords_simpl) < 2):
+        return linestring
+    else:
+        return shapely.LineString(coords_simpl)
+
+
+def simplify_coords(
+    coords: Union[np.ndarray, shapely.coords.CoordinateSequence],
+    tolerance: float,
+    algorithm: str,
+    lookahead: int,
+    simplify_lookahead_points: bool,
+    keep_points_on: Optional[BaseGeometry],
+) -> np.ndarray:
+    if isinstance(coords, shapely.coords.CoordinateSequence):
+        coords = np.asarray(coords)
+    # Determine the indexes of the coordinates to keep after simplification
+    if algorithm == "rdp":
+        coords_simplify_idx = simplification.simplify_coords_idx(coords, tolerance)
+    elif algorithm == "vw":
+        coords_simplify_idx = simplification.simplify_coords_vw_idx(coords, tolerance)
+    elif algorithm in ["lang", "lang+"]:
+        coords_simplify_idx = simplify_lang.simplify_coords_lang_idx(
+            coords=coords,
+            tolerance=tolerance,
+            lookahead=lookahead,
+            simplify_lookahead_points=simplify_lookahead_points,
+        )
+    else:
+        raise ValueError(f"Unsupported algorithm specified: {algorithm}")
+
+    coords_to_drop_onborder_idx = []
+    if keep_points_on is not None:
+        # Check if there are coordinates that would be removed that should be kept
+        shapely.prepare(keep_points_on)
+        coords_to_drop_mask = np.ones(len(coords), dtype="bool")
+        coords_to_drop_mask[coords_simplify_idx] = False
+        coords_to_drop_idx = coords_to_drop_mask.nonzero()[0]
+
+        coords_to_drop_points = shapely.points(coords[coords_to_drop_idx])
+        coords_to_drop_onborder = keep_points_on.intersects(coords_to_drop_points)
+        coords_to_drop_onborder_idx = coords_to_drop_idx[coords_to_drop_onborder]
+
+    # Extracts coordinates that need to be kept
+    coords_to_keep_idx = coords_simplify_idx
+    if len(coords_to_drop_onborder_idx) > 0:
+        coords_to_keep_idx = np.concatenate(
+            [coords_to_keep_idx, coords_to_drop_onborder_idx], dtype=np.int64
+        )
+        # Indexes of coordinates to keep need to be sorted
+        coords_to_keep_idx = np.sort(coords_to_keep_idx)
+
+    return coords[coords_to_keep_idx]
```

### Comparing `pygeoops-0.2.0a2/pygeoops/_simplify_lang.py` & `pygeoops-0.2.0a3/pygeoops/_simplify_lang.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,24 +8,40 @@
 
 logger = logging.getLogger(__name__)
 
 
 def simplify_coords_lang(
     coords: Union[np.ndarray, list, shapely.coords.CoordinateSequence],
     tolerance: float,
-    lookahead: int,
+    lookahead: int = 8,
+    simplify_lookahead_points: bool = False,
 ) -> Union[np.ndarray, list]:
     """
-    Simplify a line using lang algorithm.
+    Simplify a line using the lang algorithm.
+
+    The implementation also supports an alternative behaviour of the standard lang
+    algorithm to increase the potential number of points removed from the input
+    coordinates, without violating the tolerance specified. The standard lang algorithm
+    will always retain at least ~ len(coords) / lookahead points in the output, even for
+    a line with all collinear point. Par example when lookahead=3, this leads to keeping
+    at least 33% of the input points in the output. Using simplify_lookahead_points=True
+    will remove this limitation, at the cost of some extra processing time.
+
+    Inspiration for the standard lang implementation came from:
+        * https://github.com/giscan/Generalizer/blob/master/simplify.py
+        * https://github.com/keszegrobert/polyline-simplification/blob/master/6.%20Lang.ipynb
+        * https://web.archive.org/web/20171005193700/http://web.cs.sunyit.edu/~poissad/projects/Curve/about_algorithms/lang.php
 
     Args:
         coords (Union[np.ndarray, list]): list of coordinates to be simplified.
         tolerance (float): distance tolerance to use.
         lookahead (int, optional): the number of points to consider for removing
             in a moving window. Defaults to 8.
+        simplify_lookahead_points (bool, optional): True to also simplify the lookahead
+            points. Defaults to False. More info available in the function description.
 
     Returns:
         Return the coordinates kept after simplification.
         If input coords is np.ndarray or CoordinateSequence, returns np.ndarray,
         otherwise returns a list.
     """
 
@@ -35,68 +51,56 @@
     elif isinstance(coords, shapely.coords.CoordinateSequence):
         coords_arr = np.asarray(coords)
     else:
         coords_arr = np.array(list(coords))
 
     # Determine the coordinates that need to be kept
     coords_to_keep_idx = simplify_coords_lang_idx(
-        coords=coords_arr, tolerance=tolerance, lookahead=lookahead
+        coords=coords_arr,
+        tolerance=tolerance,
+        lookahead=lookahead,
+        simplify_lookahead_points=simplify_lookahead_points,
     )
     coords_simplified_arr = coords_arr[coords_to_keep_idx]
 
     # If input was np.ndarray, return np.ndarray, otherwise list
     if isinstance(coords, (np.ndarray, shapely.coords.CoordinateSequence)):
         return coords_simplified_arr
     else:
         return coords_simplified_arr.tolist()
 
 
 def simplify_coords_lang_idx(
     coords: Union[np.ndarray, list, shapely.coords.CoordinateSequence],
     tolerance: float,
     lookahead: int = 8,
+    simplify_lookahead_points: bool = False,
 ) -> Union[np.ndarray, list]:
     """
-    Simplify a line using lang algorithm and return the coordinate indexes to
+    Simplify a line using the lang algorithm and return the coordinate indexes to
     be kept.
 
-    Inspiration for the implementation came from:
-        * https://github.com/giscan/Generalizer/blob/master/simplify.py
-        * https://github.com/keszegrobert/polyline-simplification/blob/master/6.%20Lang.ipynb
-        * https://web.archive.org/web/20171005193700/http://web.cs.sunyit.edu/~poissad/projects/Curve/about_algorithms/lang.php
+    More info about the implemtation + simplify_lookahead_points can be found in the
+    description of function simplify_coords_lang.
 
     Args:
         coords (Union[np.ndarray, list]): list of coordinates to be simplified.
         tolerance (float): distance tolerance to use.
         lookahead (int, optional): the number of points to consider for removing
             in a moving window. Defaults to 8.
+        simplify_lookahead_points (bool, optional): True to also simplify the lookahead
+            points, resulting in more points being able to be removed in some cases.
+            Defaults to False.
 
     Returns:
-        Return the indexes of coordinates that need to be kept after
-        simplification.
-        If input coords is np.ndarray or CoordinateSequence, returns np.ndarray,
+        Return the indexes of coordinates that need to be kept after simplification.
+        If input coords is an np.ndarray or CoordinateSequence, returns np.ndarray,
         otherwise returns a list.
     """
 
-    def point_line_distance(
-        point_x, point_y, line_x1, line_y1, line_x2, line_y2
-    ) -> float:
-        denominator = math.sqrt(
-            (line_x2 - line_x1) * (line_x2 - line_x1)
-            + (line_y2 - line_y1) * (line_y2 - line_y1)
-        )
-        if denominator == 0:
-            return float("Inf")
-        else:
-            numerator = abs(
-                (line_x2 - line_x1) * (line_y1 - point_y)
-                - (line_x1 - point_x) * (line_y2 - line_y1)
-            )
-            return numerator / denominator
-
     # Init variables
     if isinstance(coords, np.ndarray):
         line_arr = coords
     elif isinstance(coords, shapely.coords.CoordinateSequence):
         line_arr = np.asarray(coords)
     else:
         line_arr = np.array(list(coords))
@@ -104,58 +108,119 @@
     # Prepare lookahead
     nb_points = len(line_arr)
     if lookahead == -1:
         window_size = nb_points - 1
     else:
         window_size = min(lookahead, nb_points - 1)
 
-    # mask = np.ones(nb_points), dtype='bool')
-    mask = np.zeros(nb_points, dtype="bool")
-    mask[0] = True
+    mask_idx_to_keep = np.ones(nb_points, dtype="bool")
     window_start = 0
     window_end = window_size
 
     # Apply simplification till the window_start arrives at the last point.
-    ready = False
-    while ready is False:
+    while True:
         # Check if all points between window_start and window_end are within
         # tolerance distance to the line (window_start, window_end).
-        all_points_in_tolerance = True
+        points_outside_tolerance_found = False
         for i in range(window_start + 1, window_end):
-            distance = point_line_distance(
+            distance = _point_line_distance(
                 line_arr[i, 0],
                 line_arr[i, 1],
                 line_arr[window_start, 0],
                 line_arr[window_start, 1],
                 line_arr[window_end, 0],
                 line_arr[window_end, 1],
             )
             # If distance is nan (= linepoint1 == linepoint2) or > tolerance
             if distance > tolerance:
-                all_points_in_tolerance = False
+                points_outside_tolerance_found = True
                 break
 
-        # If not all the points are within the tolerance distance...
-        if not all_points_in_tolerance:
+        # If there were points found outside tolerance distance, we make window smaller
+        if points_outside_tolerance_found:
             # Move window_end to previous point, and try again
             window_end -= 1
         else:
-            # All points are within the tolerance, so they can be masked
-            mask[window_end] = True
-            # mask[window_start+1:window_end-1] = False
-
-            # Move the window forward
-            window_start = window_end
-            if window_start == nb_points - 1:
-                ready = True
-            window_end = window_start + window_size
+            # No point outside tolerance found, so mask points in window and move
+            # window_start.
+            if not simplify_lookahead_points:
+                # In the standard lang implementation the next window always starts with
+                # the end point of the previous window.
+                mask_idx_to_keep[window_start + 1 : window_end] = False
+                window_start = window_end
+            else:
+                # To be able to also mask the "lookahead points", this code path doesn't
+                # move the window_start if the current window contained points to be
+                # masked. Only the window_end will be moved.
+                # This has as effect that the current window_end point will be
+                # considered for masking, but increases the effective window_size to
+                # check distances for to double when many points are within tolerance,
+                # so this will affect performance!
+                #
+                # Other considered options:
+                #   - setting window_start to (window_end -1) would also enable
+                #     window_end to be masked in theory, but this doesn't work because
+                #     with eg. 90° corners consisting of 2 point within tolerance
+                #     "disappear".
+                #   - doing two passes, but this effectively at least doubles the
+                #     effective tolerance.
+                #   - using the mask for not calculating distances for points that are
+                #     already masked, but this also increases the effective tolerance
+
+                # Check if there are points in tolerance in the window
+                if not mask_idx_to_keep[window_start + 1 : window_end].any():
+                    # No points within tolerance found, so move window forward
+                    window_start = window_end
+                else:
+                    # There are points found, so mask them, but don't move window_start
+                    mask_idx_to_keep[window_start + 1 : window_end] = False
+
+            if window_start >= nb_points - 1 or window_end >= nb_points - 1:
+                break
+            window_end += window_size
             if window_end >= nb_points:
                 window_end = nb_points - 1
 
     # Prepare result: convert the mask to a list of indices of points to keep.
-    idx_to_keep_arr = mask.nonzero()[0]
+    idx_to_keep_arr = mask_idx_to_keep.nonzero()[0]
 
     # If input was np.ndarray, return np.ndarray, otherwise list
     if isinstance(coords, (np.ndarray, shapely.coords.CoordinateSequence)):
         return idx_to_keep_arr
     else:
         return idx_to_keep_arr.tolist()
+
+
+def _point_line_distance(
+    point_x: float,
+    point_y: float,
+    line_x1: float,
+    line_y1: float,
+    line_x2: float,
+    line_y2: float,
+) -> float:
+    """
+    Calculate the orthogonal distance between the point and line specified.
+
+    Args:
+        point_x (float): x coordinate of the point
+        point_y (float): y coordinate of the point
+        line_x1 (float): x coordinate of the 1st point of the line
+        line_y1 (float): y coordinate of the 1st point of the line
+        line_x2 (float): x coordinate of the 2nd point of the line
+        line_y2 (float): y coordinate of the 2nd point of the line
+
+    Returns:
+        float: the orthogonal distance.
+    """
+    denominator = math.sqrt(
+        (line_x2 - line_x1) * (line_x2 - line_x1)
+        + (line_y2 - line_y1) * (line_y2 - line_y1)
+    )
+    if denominator == 0:
+        return float("Inf")
+    else:
+        numerator = abs(
+            (line_x2 - line_x1) * (line_y1 - point_y)
+            - (line_x1 - point_x) * (line_y2 - line_y1)
+        )
+        return numerator / denominator
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pygeoops-0.2.0a2/pygeoops/_simplify_topo.py` & `pygeoops-0.2.0a3/pygeoops/_simplify_topo.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 
     Returns:
         The simplified geometry/geometries. If the input is a GeoSeries the result is
         returned like that, otherwise the result is returned as an ndarray.
     """
     if geometry is None:
         return None
+    algorithm = algorithm.lower()
 
     # If input isn't arraylike or if the arraylike only has one element, just apply
     # simplify as creating a topology first is useless.
     if not hasattr(geometry, "__len__") or len(geometry) <= 1:
         return pygeoops.simplify(
             geometry=geometry,
             tolerance=tolerance,
```

### Comparing `pygeoops-0.2.0a2/pygeoops/_types.py` & `pygeoops-0.2.0a3/pygeoops/_types.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/pygeoops/_view_angles.py` & `pygeoops-0.2.0a3/pygeoops/_view_angles.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/pygeoops.egg-info/PKG-INFO` & `pygeoops-0.2.0a3/pygeoops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoops
-Version: 0.2.0a2
+Version: 0.2.0a3
 Summary: Library with some less common or extended spatial functions
 Author-email: Pieter Roggemans <pieter.roggemans@gmail.com>
 Project-URL: Homepage, https://github.com/pygeoops/pygeoops
 Project-URL: Bug Tracker, https://github.com/pygeoops/pygeoops/issues
 Keywords: GIS,cartography,pandas,shapely,geopandas
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pygeoops-0.2.0a2/pygeoops.egg-info/SOURCES.txt` & `pygeoops-0.2.0a3/pygeoops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/pyproject.toml` & `pygeoops-0.2.0a3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoops"
-version = "0.2.0a2"
+version = "0.2.0a3"
 authors = [
   { name="Pieter Roggemans", email="pieter.roggemans@gmail.com" },
 ]
 description = "Library with some less common or extended spatial functions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -26,18 +26,14 @@
 [project.urls]
 "Homepage" = "https://github.com/pygeoops/pygeoops"
 "Bug Tracker" = "https://github.com/pygeoops/pygeoops/issues"
 
 [tool.black]
 line-length = 88
 
-[tool.pyright]
-reportGeneralTypeIssues = false
-reportOptionalMemberAccess = false
-
 [tool.pytest.ini_options]
 pythonpath = "."
 testpaths = [
     "tests",
 ]
 
 [tool.ruff]
```

### Comparing `pygeoops-0.2.0a2/tests/test_centerline.py` & `pygeoops-0.2.0a3/tests/test_centerline.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/tests/test_general.py` & `pygeoops-0.2.0a3/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/tests/test_grid.py` & `pygeoops-0.2.0a3/tests/test_grid.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/tests/test_helper.py` & `pygeoops-0.2.0a3/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/tests/test_simplify.py` & `pygeoops-0.2.0a3/tests/test_simplify.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,29 +157,29 @@
 
 
 @pytest.mark.parametrize("preserve_common_boundaries", [True, False])
 def test_simplify_input_geoseries(preserve_common_boundaries: bool):
     """Test simplify of a geoseries of linestrings."""
     line1 = shapely.LineString([(0, 0), (10, 10), (20, 20)])
     line2 = shapely.LineString([(0, 0), (10, 0), (20, 0)])
-    lines_gs = gpd.GeoSeries([line1, line2, line2])
-    lines_gs = lines_gs.drop(index=1)
-    simplified_lines_gs = pygeoops.simplify(
-        geometry=lines_gs,
+    lines = gpd.GeoSeries([line1, line2, line2])
+    lines = lines.drop(index=1)
+    simplified_lines = pygeoops.simplify(
+        geometry=lines,
         algorithm="lang",
         tolerance=1,
         preserve_common_boundaries=preserve_common_boundaries,
     )
-    assert simplified_lines_gs is not None
-    assert isinstance(simplified_lines_gs, gpd.GeoSeries)
-    assert len(simplified_lines_gs) == len(lines_gs)
-    assert simplified_lines_gs.index.to_list() == lines_gs.index.to_list()
-    for test_idx, simplified_line in simplified_lines_gs.items():
+    assert simplified_lines is not None
+    assert isinstance(simplified_lines, gpd.GeoSeries)
+    assert len(simplified_lines) == len(lines)
+    assert simplified_lines.index.to_list() == lines.index.to_list()
+    for test_idx, simplified_line in simplified_lines.items():
         assert isinstance(simplified_line, shapely.LineString)
-        assert len(simplified_line.coords) < len(lines_gs.geometry[test_idx].coords)
+        assert len(simplified_line.coords) < len(lines.geometry[test_idx].coords)
         assert len(simplified_line.coords) == 2
 
 
 def test_simplify_invalid_geometry():
     # Test Polygon simplification, with invalid exterior ring
     poly = shapely.Polygon(
         shell=[(0, 0), (0, 10), (5, 10), (3, 12), (3, 9), (10, 10), (10, 0), (0, 0)],
@@ -249,19 +249,19 @@
     assert geom_simplified is not None
     assert geom_simplified.is_valid
     assert isinstance(geom_simplified, shapely.MultiPolygon)
     assert len(geom_simplified.geoms) == 3
 
 
 def test_simplify_invalid_params():
-    with pytest.raises(ValueError, match="Unsupported algorythm specified: invalid!"):
+    with pytest.raises(ValueError, match="Unsupported algorithm specified: invalid"):
         pygeoops.simplify(
             geometry=shapely.LineString([(0, 0), (10, 10), (20, 20)]),
             tolerance=1,
-            algorithm="invalid!",
+            algorithm="invalid_algorithm",
         )
 
     expected_error = (
         "The combination of preserve_common_boundaries=True and "
         "preserve_topology=False is not supported."
     )
     with pytest.raises(ValueError, match=expected_error):
@@ -272,15 +272,16 @@
             preserve_common_boundaries=True,
         )
 
 
 @pytest.mark.parametrize("algorithm, tolerance", [("lang", 2), ("rdp", 2), ("vw", 15)])
 def test_simplify_keep_points_on(tmp_path, algorithm, tolerance):
     # Skip test if simplification is not available
-    _ = pytest.importorskip("simplification")
+    if algorithm != "lang":
+        _ = pytest.importorskip("simplification")
 
     # Prepare test data
     poly_input = shapely.Polygon(
         shell=[(0, 0), (0, 10), (5, 12), (10, 10), (10, 0), (5, 0), (0, 0)]
     )
     # Create geometry where we want the points kept
     keep_points_on_line = shapely.LineString([(0, 0), (0, 12), (10, 12)])
```

### Comparing `pygeoops-0.2.0a2/tests/test_simplify_topo.py` & `pygeoops-0.2.0a3/tests/test_simplify_topo.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/tests/test_types.py` & `pygeoops-0.2.0a3/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pygeoops-0.2.0a2/tests/test_view_angles.py` & `pygeoops-0.2.0a3/tests/test_view_angles.py`

 * *Files identical despite different names*

