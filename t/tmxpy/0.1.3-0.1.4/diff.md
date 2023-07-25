# Comparing `tmp/tmxpy-0.1.3.tar.gz` & `tmp/tmxpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmxpy-0.1.3.tar", last modified: Sat Jul 22 11:39:04 2023, max compression
+gzip compressed data, was "tmxpy-0.1.4.tar", last modified: Tue Jul 25 23:32:19 2023, max compression
```

## Comparing `tmxpy-0.1.3.tar` & `tmxpy-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 11:39:04.477935 tmxpy-0.1.3/
--rw-rw-rw-   0        0        0    35802 2023-07-18 17:55:20.000000 tmxpy-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1387 2023-07-22 11:39:04.476935 tmxpy-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      820 2023-07-18 17:45:31.000000 tmxpy-0.1.3/README.md
--rw-rw-rw-   0        0        0      719 2023-07-22 11:38:46.000000 tmxpy-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 11:39:04.477935 tmxpy-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-22 11:39:04.455763 tmxpy-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 11:39:04.464769 tmxpy-0.1.3/src/tmxpy/
--rw-rw-rw-   0        0        0       46 2023-07-19 11:58:59.000000 tmxpy-0.1.3/src/tmxpy/__init__.py
--rw-rw-rw-   0        0        0     6793 2023-07-22 11:30:01.000000 tmxpy-0.1.3/src/tmxpy/tmxpy.py
-drwxrwxrwx   0        0        0        0 2023-07-22 11:39:04.474933 tmxpy-0.1.3/src/tmxpy.egg-info/
--rw-rw-rw-   0        0        0     1387 2023-07-22 11:39:04.000000 tmxpy-0.1.3/src/tmxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-07-22 11:39:04.000000 tmxpy-0.1.3/src/tmxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 11:39:04.000000 tmxpy-0.1.3/src/tmxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-22 11:39:04.000000 tmxpy-0.1.3/src/tmxpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-22 11:39:04.000000 tmxpy-0.1.3/src/tmxpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 23:32:19.466991 tmxpy-0.1.4/
+-rw-rw-rw-   0        0        0    35802 2023-07-18 17:55:20.000000 tmxpy-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1387 2023-07-25 23:32:19.465990 tmxpy-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      820 2023-07-18 17:45:31.000000 tmxpy-0.1.4/README.md
+-rw-rw-rw-   0        0        0      719 2023-07-25 12:46:37.000000 tmxpy-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 23:32:19.466991 tmxpy-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 23:32:19.443978 tmxpy-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-25 23:32:19.453979 tmxpy-0.1.4/src/tmxpy/
+-rw-rw-rw-   0        0        0       46 2023-07-19 11:58:59.000000 tmxpy-0.1.4/src/tmxpy/__init__.py
+-rw-rw-rw-   0        0        0     7744 2023-07-25 23:19:24.000000 tmxpy-0.1.4/src/tmxpy/tmxpy.py
+drwxrwxrwx   0        0        0        0 2023-07-25 23:32:19.463989 tmxpy-0.1.4/src/tmxpy.egg-info/
+-rw-rw-rw-   0        0        0     1387 2023-07-25 23:32:19.000000 tmxpy-0.1.4/src/tmxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-07-25 23:32:19.000000 tmxpy-0.1.4/src/tmxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 23:32:19.000000 tmxpy-0.1.4/src/tmxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-25 23:32:19.000000 tmxpy-0.1.4/src/tmxpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-25 23:32:19.000000 tmxpy-0.1.4/src/tmxpy.egg-info/top_level.txt
```

### Comparing `tmxpy-0.1.3/LICENSE` & `tmxpy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tmxpy-0.1.3/PKG-INFO` & `tmxpy-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmxpy
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for reading and writing TMX files.
 Author-email: AnotherPillow <redacted@email.xyz>
 Project-URL: Homepage, https://github.com/AnotherPillow/tmxpy
 Project-URL: Bug Tracker, https://github.com/AnotherPillow/tmxpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `tmxpy-0.1.3/README.md` & `tmxpy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tmxpy-0.1.3/pyproject.toml` & `tmxpy-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tmxpy"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="AnotherPillow", email="redacted@email.xyz" }
 ]
 description = "A Python library for reading and writing TMX files."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tmxpy-0.1.3/src/tmxpy/tmxpy.py` & `tmxpy-0.1.4/src/tmxpy/tmxpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,14 @@
             return "Island_FieldOffice"
         case "IslandHut":
             return "Island_Hut"
         case "IslandShrine":
             return "Island_Shrine"
         case _:
             return name
-        
-
 
 class TMXpy:
     spriteSheetFolderPaths: Sequence[Path|str] = []
     inputFile: bs4.BeautifulSoup
     tileDimensions: tuple[int, int] = (0, 0)
     tmxDimensions: tuple[int, int] = (0, 0)
     tiles: dict = {}
@@ -108,14 +106,16 @@
             (int(layer['width']) * int(self.tileDimensions[0]),
                 int(layer['height']) * int(self.tileDimensions[1])))
 
         for i, tile in enumerate(tiles):
             tile = tile.strip()
             if tile == "0":
                 continue
+            if '\n' in tile:
+                tile = tile.split('\n')[0].strip()
             img.paste(self.renderTile(tile), (int(i % int(layer['width'])) * int(self.tileDimensions[0]), int(i / int(layer['width'])) * int(self.tileDimensions[1])))
 
         return img
     
     def renderAllLayers(self, blocked: list[str] = []) -> Image.Image:
         """Renders all layers in the TMX file, except for the ones in the blocked list"""
         width = int(self.tmxDimensions[0]) * int(self.tileDimensions[0])
@@ -123,21 +123,21 @@
         img = Image.new("RGBA", (width, height))
 
 
 
         
         for i, layer in enumerate(self.inputFile.find_all("layer")):
             if layer['name'] in blocked or str(i) in blocked or i in blocked:
-                print(f'Skipping layer {layer["name"]} - {i}')
+                # print(f'Skipping layer {layer["name"]} - {i}')
                 continue
-            print(f'Rendering layer {layer["name"]} - {i}')
+            # print(f'Rendering layer {layer["name"]} - {i}')
             layer = self.renderLayer(i)
             #stick it on top of the last layer, and not overwriting the transparent pixels
             img.paste(layer, (0, 0), layer)
-            print(f'Layer {i} rendered, layer width: {layer.width}, layer height: {layer.height} - img width: {width}, img height: {height}')
+            # print(f'Layer {i} rendered, layer width: {layer.width}, layer height: {layer.height} - img width: {width}, img height: {height}')
         return img
     
     def parseWarps(self) -> list[dict]:
         #extract property[name="Warp"]
         prop = cast(dict, self.inputFile.find("property", {"name": "Warp"}))
         if prop is None or prop == {}:
             return []
@@ -162,16 +162,38 @@
         return warps
     
     def replace_warp(self, index: int, warp: dict):
         if 'warps' not in self.__dict__:
             self.parseWarps()
         self.warps[index] = warp
 
+    def setTile(self, x: int, y: int, tile: str, layerID: int = -1, layerName: str = "") -> None:
+        """Sets a tile in the TMX file"""
+        if layerID > -1:
+            layer = self.inputFile.find("layer", {"id": str(layerID)})
+        elif layerName != "":
+            layer = self.inputFile.find("layer", {"name": layerName})
+        else:
+            raise Exception("TMXpy: No layerID or layerName given")
+        if layer is None:
+            raise Exception("TMXpy: Layer not found")
+        
+        rows = layer.text.split("\n")
+        columns = rows[y].split(",")
+        
+        columns[x] = tile
+        rows[y] = ",".join(columns)
+        output = "\n".join(rows)
+        
+        layer.contents[0].replace_with(output) # type: ignore <-- like wtf pylint why what is this
+        
+        
 
     def save(self, path: str or Path):
 
-        self.inputFile.find("property", {"name": "Warp"})['value'] = " ".join([f"{w['map_x']} {w['map_y']} {w['destination']} {w['dest_x']} {w['dest_y']}" for w in self.warps]) # type: ignore
+        if 'warps' in self.__dict__:
+            self.inputFile.find("property", {"name": "Warp"})['value'] = " ".join([f"{w['map_x']} {w['map_y']} {w['destination']} {w['dest_x']} {w['dest_y']}" for w in self.warps]) # type: ignore
 
         with open(path, "w") as f:
             f.write(self.inputFile.prettify())
```

### Comparing `tmxpy-0.1.3/src/tmxpy.egg-info/PKG-INFO` & `tmxpy-0.1.4/src/tmxpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmxpy
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for reading and writing TMX files.
 Author-email: AnotherPillow <redacted@email.xyz>
 Project-URL: Homepage, https://github.com/AnotherPillow/tmxpy
 Project-URL: Bug Tracker, https://github.com/AnotherPillow/tmxpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

