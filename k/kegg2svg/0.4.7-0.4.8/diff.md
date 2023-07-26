# Comparing `tmp/kegg2svg-0.4.7.tar.gz` & `tmp/kegg2svg-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegg2svg-0.4.7.tar", last modified: Mon Sep 26 11:15:46 2022, max compression
+gzip compressed data, was "kegg2svg-0.4.8.tar", last modified: Wed Jul 26 12:04:21 2023, max compression
```

## Comparing `kegg2svg-0.4.7.tar` & `kegg2svg-0.4.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 11:15:46.446437 kegg2svg-0.4.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 11:15:46.442437 kegg2svg-0.4.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 11:15:46.442437 kegg2svg-0.4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/.github/workflows/pypi_cd.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-09-26 11:15:46.446437 kegg2svg-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      586 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 11:15:46.446437 kegg2svg-0.4.7/example_data/
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/example_data/metabolite_quants_example.csv
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/example_data/reaction_quants_example.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 11:15:46.446437 kegg2svg-0.4.7/kegg2svg/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/kegg2svg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/kegg2svg/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)   406609 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/kegg2svg/colors.csv
--rw-r--r--   0 runner    (1001) docker     (121)     7848 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/kegg2svg/kegg2svg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 11:15:46.446437 kegg2svg-0.4.7/kegg2svg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1006 2022-09-26 11:15:46.000000 kegg2svg-0.4.7/kegg2svg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-26 11:15:46.000000 kegg2svg-0.4.7/kegg2svg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-26 11:15:46.000000 kegg2svg-0.4.7/kegg2svg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-26 11:15:46.000000 kegg2svg-0.4.7/kegg2svg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-09-26 11:15:46.000000 kegg2svg-0.4.7/kegg2svg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-26 11:15:46.000000 kegg2svg-0.4.7/kegg2svg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-09-26 11:15:46.446437 kegg2svg-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 11:15:46.442437 kegg2svg-0.4.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-26 11:15:46.446437 kegg2svg-0.4.7/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (121)     1000 2022-09-26 11:15:30.000000 kegg2svg-0.4.7/tests/unittests/test_d3scale_linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:04:21.712320 kegg2svg-0.4.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:04:21.708320 kegg2svg-0.4.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:04:21.708320 kegg2svg-0.4.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/.github/workflows/pypi_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-26 12:04:21.712320 kegg2svg-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:04:21.708320 kegg2svg-0.4.8/example_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/example_data/metabolite_quants_example.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/example_data/reaction_quants_example.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:04:21.708320 kegg2svg-0.4.8/kegg2svg/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/kegg2svg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/kegg2svg/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   406609 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/kegg2svg/colors.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/kegg2svg/kegg2svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:04:21.712320 kegg2svg-0.4.8/kegg2svg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-26 12:04:21.000000 kegg2svg-0.4.8/kegg2svg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-26 12:04:21.000000 kegg2svg-0.4.8/kegg2svg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:04:21.000000 kegg2svg-0.4.8/kegg2svg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 12:04:21.000000 kegg2svg-0.4.8/kegg2svg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 12:04:21.000000 kegg2svg-0.4.8/kegg2svg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 12:04:21.000000 kegg2svg-0.4.8/kegg2svg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-26 12:04:21.712320 kegg2svg-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:04:21.708320 kegg2svg-0.4.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:04:21.712320 kegg2svg-0.4.8/tests/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-26 12:04:16.000000 kegg2svg-0.4.8/tests/unittests/test_d3scale_linear.py
```

### Comparing `kegg2svg-0.4.7/.github/workflows/pypi_cd.yml` & `kegg2svg-0.4.8/.github/workflows/pypi_cd.yml`

 * *Files identical despite different names*

### Comparing `kegg2svg-0.4.7/.gitignore` & `kegg2svg-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `kegg2svg-0.4.7/PKG-INFO` & `kegg2svg-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegg2svg
-Version: 0.4.7
+Version: 0.4.8
 Summary: Draw svg from KEGG Map and augment it with quant data
 Home-page: https://github.com/computational-ms/kegg2svg
 Author: Christian Fufezan
 Author-email: christian@fufezan.net
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `kegg2svg-0.4.7/example_data/reaction_quants_example.csv` & `kegg2svg-0.4.8/example_data/reaction_quants_example.csv`

 * *Files identical despite different names*

### Comparing `kegg2svg-0.4.7/kegg2svg/cli.py` & `kegg2svg-0.4.8/kegg2svg/cli.py`

 * *Files identical despite different names*

### Comparing `kegg2svg-0.4.7/kegg2svg/colors.csv` & `kegg2svg-0.4.8/kegg2svg/colors.csv`

 * *Files identical despite different names*

### Comparing `kegg2svg-0.4.7/kegg2svg/kegg2svg.py` & `kegg2svg-0.4.8/kegg2svg/kegg2svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import csv
 import re
 from pathlib import Path
 from xml import dom
 import xml.etree.ElementTree as ET
 from loguru import logger
-import drawSvg as draw
+import drawsvg as draw
 
 
 class Hyperlink(draw.DrawingParentElement):
     TAG_NAME = "a"
 
     def __init__(self, href, target=None, **kwargs):
         # Other init logic...
@@ -62,15 +62,15 @@
         kegg_html (html): use `curl -O <your_mal_link> map0.htlm` to get the html
 
     Returns:
         ElementTree: Matabolite and Path elements from HTML page
     """
     tree_data = []
     found_map_tag = False
-    for line in open(kegg_html, "r"):
+    for line in open(kegg_html, "r", encoding='utf-8'):
         if "<map id=" in line:
             found_map_tag = True
         if found_map_tag is True:
             tree_data.append(line.strip())
         if "</map>" in line:
             break
     return ET.fromstring("".join(tree_data))
@@ -200,15 +200,15 @@
             line_attributes["fill"] = (
                 color_lookup.get(reactions[0], {"Color": "#cccccc"})["Color"] + "77"
             )
             quant_value = quant_lookup.get(reactions[0], None)
             if quant_value is not None:
                 logger.debug("Reaction path scaling not implemented yet.")
         element = draw.Lines(*coords, **line_attributes)
-        element.appendTitle(f"{g.attrib['title']}")
+        element.append_title(f"{g.attrib['title']}")
         hlink = Hyperlink(f"https://www.genome.jp{g.attrib['href']}", target="_blank")
         hlink.append(element)
         d.append(hlink)
 
     for g in root.findall("area[@shape='circle']"):
         x, y, r = g.attrib["data-coords"].split(",")
         circle_attributes = {
@@ -232,21 +232,21 @@
 
         element = draw.Circle(
             int(x),
             params["max_y"] - int(y),
             radius,
             **circle_attributes,
         )
-        element.appendTitle(f"{g.attrib['title']}")
+        element.append_title(f"{g.attrib['title']}")
         hlink = Hyperlink(f"https://www.genome.jp{g.attrib['href']}", target="_blank")
         hlink.append(element)
         d.append(hlink)
 
     ratio = params["max_y"] / params["max_x"]
-    d.setRenderSize(
+    d.set_render_size(
         1200,
         1200 * ratio,
     )
     if output_filename.endswith(".svg") is False:
         output_filename += ".svg"
-    d.saveSvg(output_filename)
+    d.save_svg(output_filename)
     logger.debug(f"Wrote {output_filename}")
```

### Comparing `kegg2svg-0.4.7/kegg2svg.egg-info/PKG-INFO` & `kegg2svg-0.4.8/kegg2svg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegg2svg
-Version: 0.4.7
+Version: 0.4.8
 Summary: Draw svg from KEGG Map and augment it with quant data
 Home-page: https://github.com/computational-ms/kegg2svg
 Author: Christian Fufezan
 Author-email: christian@fufezan.net
 License: Apache 2
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `kegg2svg-0.4.7/setup.cfg` & `kegg2svg-0.4.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 	Topic :: Scientific/Engineering :: Bio-Informatics
 	Topic :: Scientific/Engineering :: Chemistry
 	Topic :: Scientific/Engineering :: Medical Science Apps.
 
 [options]
 packages = find:
 install_requires = 
-	drawSvg
+	drawSvg~=2.2.0
 	click
 	loguru
 
 [options.package_data]
 kegg2svg = *.csv
 
 [options.entry_points]
```

### Comparing `kegg2svg-0.4.7/setup.py` & `kegg2svg-0.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `kegg2svg-0.4.7/tests/unittests/test_d3scale_linear.py` & `kegg2svg-0.4.8/tests/unittests/test_d3scale_linear.py`

 * *Files identical despite different names*

