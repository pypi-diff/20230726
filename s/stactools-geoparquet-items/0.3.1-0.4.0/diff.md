# Comparing `tmp/stactools-geoparquet-items-0.3.1.tar.gz` & `tmp/stactools-geoparquet-items-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-geoparquet-items-0.3.1.tar", last modified: Wed Jul 19 15:34:25 2023, max compression
+gzip compressed data, was "stactools-geoparquet-items-0.4.0.tar", last modified: Tue Jul 25 21:57:05 2023, max compression
```

## Comparing `stactools-geoparquet-items-0.3.1.tar` & `stactools-geoparquet-items-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:34:25.948480 stactools-geoparquet-items-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-19 15:34:05.000000 stactools-geoparquet-items-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-19 15:34:25.948480 stactools-geoparquet-items-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-19 15:34:05.000000 stactools-geoparquet-items-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-19 15:34:05.000000 stactools-geoparquet-items-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-19 15:34:25.952480 stactools-geoparquet-items-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:34:25.944480 stactools-geoparquet-items-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:34:25.944480 stactools-geoparquet-items-0.3.1/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:34:25.948480 stactools-geoparquet-items-0.3.1/src/stactools/geoparquet_items/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-19 15:34:05.000000 stactools-geoparquet-items-0.3.1/src/stactools/geoparquet_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-19 15:34:05.000000 stactools-geoparquet-items-0.3.1/src/stactools/geoparquet_items/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 15:34:25.948480 stactools-geoparquet-items-0.3.1/src/stactools_geoparquet_items.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-19 15:34:25.000000 stactools-geoparquet-items-0.3.1/src/stactools_geoparquet_items.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-19 15:34:25.000000 stactools-geoparquet-items-0.3.1/src/stactools_geoparquet_items.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 15:34:25.000000 stactools-geoparquet-items-0.3.1/src/stactools_geoparquet_items.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-19 15:34:25.000000 stactools-geoparquet-items-0.3.1/src/stactools_geoparquet_items.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 15:34:25.000000 stactools-geoparquet-items-0.3.1/src/stactools_geoparquet_items.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:57:05.301160 stactools-geoparquet-items-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-25 21:56:45.000000 stactools-geoparquet-items-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-25 21:57:05.301160 stactools-geoparquet-items-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-07-25 21:56:45.000000 stactools-geoparquet-items-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 21:56:45.000000 stactools-geoparquet-items-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-25 21:57:05.301160 stactools-geoparquet-items-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:57:05.301160 stactools-geoparquet-items-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:57:05.301160 stactools-geoparquet-items-0.4.0/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:57:05.301160 stactools-geoparquet-items-0.4.0/src/stactools/geoparquet_items/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-25 21:56:45.000000 stactools-geoparquet-items-0.4.0/src/stactools/geoparquet_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-07-25 21:56:45.000000 stactools-geoparquet-items-0.4.0/src/stactools/geoparquet_items/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:57:05.301160 stactools-geoparquet-items-0.4.0/src/stactools_geoparquet_items.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-25 21:57:05.000000 stactools-geoparquet-items-0.4.0/src/stactools_geoparquet_items.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-25 21:57:05.000000 stactools-geoparquet-items-0.4.0/src/stactools_geoparquet_items.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:57:05.000000 stactools-geoparquet-items-0.4.0/src/stactools_geoparquet_items.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-25 21:57:05.000000 stactools-geoparquet-items-0.4.0/src/stactools_geoparquet_items.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 21:57:05.000000 stactools-geoparquet-items-0.4.0/src/stactools_geoparquet_items.egg-info/top_level.txt
```

### Comparing `stactools-geoparquet-items-0.3.1/LICENSE` & `stactools-geoparquet-items-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-geoparquet-items-0.3.1/PKG-INFO` & `stactools-geoparquet-items-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-geoparquet-items
-Version: 0.3.1
+Version: 0.4.0
 Summary: Uses stac-geoparquet to generate a geoparquet for a list of STAC items
 Home-page: https://github.com/stactools-packages/geoparquet-items
 Author: Matthias Mohr
 Author-email: matthias@mohr.ws
 Project-URL: Issues, https://github.com/stactools-packages/geoparquet-items/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
```

### Comparing `stactools-geoparquet-items-0.3.1/README.md` & `stactools-geoparquet-items-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `stactools-geoparquet-items-0.3.1/setup.cfg` & `stactools-geoparquet-items-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `stactools-geoparquet-items-0.3.1/src/stactools/geoparquet_items/commands.py` & `stactools-geoparquet-items-0.4.0/src/stactools/geoparquet_items/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,39 @@
 import json
 import logging
 import os
 
 # Used only for partitioning / dask variant
 import pathlib
 import shutil
-from typing import Any, Optional, Sequence
+from typing import Any, Dict, Optional, Sequence
 
 import click
 import dask.bag as db
 import dask_geopandas
 import geopandas
 import pyarrow
 import pyarrow.parquet as pq
 import pyogrio
 import requests
 import stac_geoparquet
 from click import Command, Group
+from urllib.parse import urlparse, urljoin
 
 logger = logging.getLogger(__name__)
 
-IGNORE_FIELDS = ["stac_version", "type", "assets"]
+STAC_ITEM_TYPES = ["application/json", "application/geo+json"]
+SELF_LINK_COLUMN = "self_link"
 
+def is_self_link(link: Dict[str, Any]) -> bool:
+    return (
+        link["rel"] == "self"
+        and (not link["type"] or link["type"] in STAC_ITEM_TYPES)
+        and urlparse(link["href"]).netloc
+    )
 
 def create_geoparquetitems_command(cli: Group) -> Command:
     """Creates the stactools-geoparquet-items command line utility."""
 
     @cli.group(
         "geoparquet-items",
         short_help=("Commands for working with stactools-geoparquet-items"),
@@ -51,27 +59,37 @@
     @click.option(
         "--selflink",
         default=False,
         show_default=True,
         help="Tries to add the absolute link to the source STAC Item to a column named 'self_link'",
         is_flag=True,
     )
+    @click.option(
+        "--baseurl",
+        default=None,
+        help="If provided, tries to fix invalid self URLs by mapping to the source folder to the given URL. "
+        + "Only applies if the given source is a local folder. Must have a slash at the end."
+    )
     def create_command(
         source: str,
         destination: str,
         collection: str = "",
         partition: int = 1,
         selflink: bool = False,
+        baseurl: str = None
     ) -> None:
         """Create geoparquet from STAC Items
 
         Args:
             source (str): Link to a list of STAC Items (ItemCollection) or a folder with STAC files.
             destination (str): Path where the geoparquet file will be stored.
         """
+        if baseurl is not None and not baseurl.endswith("/"):
+            raise Exception("baseurl must end with a slash")
+
         p = pathlib.Path(destination)
         if p.is_dir():
             shutil.rmtree(p, ignore_errors=True)
         else:
             p.unlink(missing_ok=True)
 
         if partition > 1:
@@ -101,22 +119,51 @@
                         continue
                     else:
                         path = os.path.join(root, name)
                         paths.append(pathlib.Path(path))
 
             print("Found {} potential STAC Items".format(len(paths)))
 
+            def load_file(p: pathlib.Path):
+                with p.open() as f:
+                    stac = json.load(f)
+                    if baseurl:
+                        # remove self link
+                        for link in stac["links"]:
+                            if is_self_link(link):
+                                stac["links"].remove(link)
+                                break
+
+                        # create self link
+                        rel_path = str(p.relative_to(source)).replace('\\', '/')
+                        href = urljoin(baseurl, rel_path)
+                        self_link = {
+                            'href': href,
+                            'type': STAC_ITEM_TYPES[0],
+                            'rel': 'self'
+                        }
+
+                        stac["links"].append(self_link)
+
+                    return stac
+
             if partition > 1:
                 bag = (
                     db.from_sequence(paths, npartitions=partition)
-                    .map(lambda file: file.read_text())
-                    .map(json.loads)
-                    .filter(lambda item: item["type"] == "Feature")
+                    .map(load_file)
+                    .filter(lambda stac: stac["type"] == "Feature")
                 )
-
+            else:
+                for p in paths:
+                    stac = load_file(p)
+                    if stac["type"] == "Feature":
+                        items.append(stac)
+            
+            del paths
+        
         def create_fn(items: Sequence[dict[str, Any]]) -> geopandas.GeoDataFrame:
             return stac_geoparquet.to_geodataframe(items, add_self_link=selflink)
 
         if bag is not None:
             print("Initialized for parallel processing")
             # Taken from Tom Augpurger's notbook at
             # https://notebooksharing.space/view/1c2922b90622013d91dc22182e7f60d64e119c0f7cf1f977ccaa4dd0994bd1b6
@@ -132,21 +179,14 @@
             sample.to_parquet(buf, engine="pyarrow")
             buf.seek(0)
             schema = pq.read_schema(buf)
 
             df.to_parquet(destination, schema=schema, write_index=False)
             print("Wrote geoparquet file(s)")
         else:
-            for p in paths:
-                with p.open() as f:
-                    item = json.load(f)
-                    if item["type"] == "Feature":
-                        items.append(item)
-            del paths
-
             num = len(items)
             if num > 0:
                 print(f"Loaded {num} actual STAC Items")
                 df = create_fn(items)
                 del items
                 print("Created dataframe")
                 df.to_parquet(destination)
@@ -180,18 +220,22 @@
         "convert", short_help="Convert geoparquet to other OGR file formats"
     )
     @click.argument("source")
     @click.argument("destination")
     @click.option(
         "--exclude",
         "-e",
-        default=",".join(IGNORE_FIELDS),
-        show_default=True,
-        help="A list of comma-separated fields that should be excluded from the target file. "
-        + " Use 'none' to include all fields."
+        default=None,
+        help="A list of comma-separated fields that should be excluded from the target file."
+    )
+    @click.option(
+        "--include",
+        "-i",
+        default=None,
+        help="A list of comma-separated fields that should be included in the target file. This option takes preference over `exclude`."
     )
     @click.option(
         "--format",
         "-f",
         type=click.Choice(
             ["shapefile", "gpkg", "geojson", "geojsonseq", "flatgeobuf"],
             case_sensitive=False,
@@ -201,37 +245,35 @@
         help="File format to convert to.",
     )
     def convert_command(
         source: str,
         destination: str,
         format: str = "gpkg",
         exclude: Optional[str] = None,
+        include: Optional[str] = None,
     ) -> None:
         """Convert geoparquet to other OGR file formats
 
         Args:
             source (str): Path where the geoparquet file is located.
             destination (str): Path where the new file will be stored.
         """
         if not os.path.exists(source):
             raise Exception("Source file does not exist")
 
-        if exclude is None:
-            to_exclude = IGNORE_FIELDS
-        elif exclude == "none" or exclude == "NONE":
-            to_exclude = []
-        else:
-            to_exclude = exclude.split(",")
-
         columns = None
-        if len(to_exclude) > 0:
-            schema = pq.read_schema(source)
-            columns = schema.names.copy()
-            for col in to_exclude:
-                columns.remove(col.strip())
+        if include is not None:
+            columns = [col.strip() for col in include.split(",")]
+        elif exclude is not None:
+            to_exclude = exclude.split(",")
+            if len(to_exclude) > 0:
+                schema = pq.read_schema(source)
+                columns = schema.names.copy()
+                for col in to_exclude:
+                    columns.remove(col.strip())
 
         df = geopandas.read_parquet(source, columns=columns)
         pyogrio.write_dataframe(df, destination, driver=format)
 
         return None
 
     @geoparquetitems.command(
```

### Comparing `stactools-geoparquet-items-0.3.1/src/stactools_geoparquet_items.egg-info/PKG-INFO` & `stactools-geoparquet-items-0.4.0/src/stactools_geoparquet_items.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools-geoparquet-items
-Version: 0.3.1
+Version: 0.4.0
 Summary: Uses stac-geoparquet to generate a geoparquet for a list of STAC items
 Home-page: https://github.com/stactools-packages/geoparquet-items
 Author: Matthias Mohr
 Author-email: matthias@mohr.ws
 Project-URL: Issues, https://github.com/stactools-packages/geoparquet-items/issues
 Keywords: stactools,pystac,catalog,STAC
 Classifier: Development Status :: 4 - Beta
```

