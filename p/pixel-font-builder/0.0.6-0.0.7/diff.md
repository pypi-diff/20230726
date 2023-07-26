# Comparing `tmp/pixel-font-builder-0.0.6.tar.gz` & `tmp/pixel-font-builder-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixel-font-builder-0.0.6.tar", last modified: Tue Jul 25 14:21:46 2023, max compression
+gzip compressed data, was "pixel-font-builder-0.0.7.tar", last modified: Wed Jul 26 11:13:40 2023, max compression
```

## Comparing `pixel-font-builder-0.0.6.tar` & `pixel-font-builder-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:21:46.778327 pixel-font-builder-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-25 14:21:46.778327 pixel-font-builder-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:21:46.778327 pixel-font-builder-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:21:46.770327 pixel-font-builder-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:21:46.774327 pixel-font-builder-0.0.6/src/pixel_font_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/bdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/src/pixel_font_builder/opentype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:21:46.774327 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-25 14:21:46.000000 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-25 14:21:46.000000 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:21:46.000000 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-25 14:21:46.000000 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 14:21:46.000000 pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:21:46.778327 pixel-font-builder-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-25 14:21:34.000000 pixel-font-builder-0.0.6/tests/test_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/src/pixel_font_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/bdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/src/pixel_font_builder/opentype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-07-26 11:13:40.000000 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-26 11:13:40.000000 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:13:40.000000 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-26 11:13:40.000000 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 11:13:40.000000 pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:13:40.620792 pixel-font-builder-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-26 11:13:23.000000 pixel-font-builder-0.0.7/tests/test_.py
```

### Comparing `pixel-font-builder-0.0.6/LICENSE` & `pixel-font-builder-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.6/PKG-INFO` & `pixel-font-builder-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
```

### Comparing `pixel-font-builder-0.0.6/README.md` & `pixel-font-builder-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.6/pyproject.toml` & `pixel-font-builder-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pixel-font-builder"
-version = "0.0.6"
+version = "0.0.7"
 description = "A library that helps create pixel style fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.11"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `pixel-font-builder-0.0.6/src/pixel_font_builder/bdf.py` & `pixel-font-builder-0.0.7/src/pixel_font_builder/bdf.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.6/src/pixel_font_builder/font.py` & `pixel-font-builder-0.0.7/src/pixel_font_builder/font.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,19 +31,14 @@
         self.opentype_configs = opentype.Configs()
         self.bdf_configs = bdf.Configs()
 
     @property
     def line_height(self) -> int:
         return self.ascent - self.descent
 
-    def get_character_mapping_sequence(self) -> list[tuple[int, str]]:
-        sequence = list(self.character_mapping.items())
-        sequence.sort()
-        return sequence
-
     def get_glyph(self, name: str) -> Glyph | None:
         return self._name_to_glyph.get(name, None)
 
     def get_glyphs(self) -> list[Glyph]:
         return list(self._name_to_glyph.values())
 
     def get_glyphs_count(self) -> int:
```

### Comparing `pixel-font-builder-0.0.6/src/pixel_font_builder/glyph.py` & `pixel-font-builder-0.0.7/src/pixel_font_builder/glyph.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.6/src/pixel_font_builder/info.py` & `pixel-font-builder-0.0.7/src/pixel_font_builder/info.py`

 * *Files identical despite different names*

### Comparing `pixel-font-builder-0.0.6/src/pixel_font_builder/opentype.py` & `pixel-font-builder-0.0.7/src/pixel_font_builder/opentype.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,27 +178,27 @@
             if (x == xl and x == xr) or (y == yl and y == yr):
                 solved_line_segment.pop()
             # 添加到轮廓
             outlines.append(solved_line_segment)
     return outlines
 
 
-def _create_glyph(outlines: list[list[tuple[int, int]]], glyph: Glyph, px_to_units: int, is_ttf: bool) -> OTFGlyph | TTFGlyph:
+def _create_glyph(outlines: list[list[tuple[int, int]]], glyph_context: Glyph, px_to_units: int, is_ttf: bool) -> OTFGlyph | TTFGlyph:
     if is_ttf:
         pen = TTFGlyphPen()
     else:
-        pen = OTFGlyphPen(glyph.advance_width * px_to_units, None)
+        pen = OTFGlyphPen(glyph_context.advance_width * px_to_units, None)
     if len(outlines) > 0:
         for outline_index, outline in enumerate(outlines):
             for point_index, point in enumerate(outline):
 
                 # 转换左上角原点坐标系为左下角原点坐标系
                 x, y = point
-                x += glyph.offset_x * px_to_units
-                y = (glyph.height + glyph.offset_y) * px_to_units - y
+                x += glyph_context.offset_x * px_to_units
+                y = (glyph_context.height + glyph_context.offset_y) * px_to_units - y
                 point = x, y
 
                 if point_index == 0:
                     pen.moveTo(point)
                 else:
                     pen.lineTo(point)
             if outline_index < len(outlines) - 1:
@@ -210,63 +210,60 @@
         pen.closePath()
     if is_ttf:
         return pen.glyph()
     else:
         return pen.getCharString()
 
 
-def create_builder(context: 'font.FontBuilder', is_ttf: bool, flavor: Flavor = None) -> FontBuilder:
-    xtf_name = 'TTF' if is_ttf else 'OTF'
+def _get_glyph_with_cache(glyph_context: Glyph, px_to_units: int, is_ttf: bool) -> OTFGlyph | TTFGlyph:
+    cache_tag = f'{glyph_context.advance_width}#{glyph_context.offset}#{glyph_context.data}'.replace(' ', '')
+    if getattr(glyph_context, _CACHE_NAME_TAG, None) != cache_tag:
+        setattr(glyph_context, _CACHE_NAME_OUTLINES, None)
+        setattr(glyph_context, _CACHE_NAME_OTF_GLYPH, None)
+        setattr(glyph_context, _CACHE_NAME_TTF_GLYPH, None)
+        setattr(glyph_context, _CACHE_NAME_TAG, cache_tag)
+
+    outlines = getattr(glyph_context, _CACHE_NAME_OUTLINES, None)
+    if outlines is None:
+        logger.debug("Create 'Outlines': %s", glyph_context.name)
+        outlines = _create_outlines(glyph_context.data, px_to_units)
+        setattr(glyph_context, _CACHE_NAME_OUTLINES, outlines)
+    else:
+        logger.debug("Use cached 'Outlines': %s", glyph_context.name)
+
+    cache_name_xtf_glyph = _CACHE_NAME_TTF_GLYPH if is_ttf else _CACHE_NAME_OTF_GLYPH
+    glyph = getattr(glyph_context, cache_name_xtf_glyph, None)
+    if glyph is None:
+        logger.debug("Create '%sGlyph': %s", 'TTF' if is_ttf else 'OTF', glyph_context.name)
+        glyph = _create_glyph(outlines, glyph_context, px_to_units, is_ttf)
+        setattr(glyph_context, cache_name_xtf_glyph, glyph)
+    else:
+        logger.debug("Use cached '%sGlyph': %s", 'TTF' if is_ttf else 'OTF', glyph_context.name)
+    return glyph
+
 
-    logger.debug("Create '%sBuilder': %s", xtf_name, context.meta_infos.family_name)
+def create_builder(context: 'font.FontBuilder', is_ttf: bool, flavor: Flavor = None) -> FontBuilder:
+    logger.debug("Create '%sBuilder': %s", 'TTF' if is_ttf else 'OTF', context.meta_infos.family_name)
     context.check_ready()
 
     units_per_em = context.size * context.opentype_configs.px_to_units
     builder = FontBuilder(units_per_em, isTTF=is_ttf)
 
     logger.debug("Setup 'Name Strings'")
     name_strings = _create_name_strings(context.meta_infos)
     builder.setupNameTable(name_strings)
 
-    logger.debug("Setup 'Glyph Order'")
+    logger.debug("Setup 'Glyph Order' and 'Glyphs'")
     glyph_order = ['.notdef']
-    for _, glyph_name in context.get_character_mapping_sequence():
-        if glyph_name not in glyph_order:
-            glyph_order.append(glyph_name)
-    builder.setupGlyphOrder(glyph_order)
-    logger.debug("Setup 'Character Mapping'")
-    builder.setupCharacterMap(context.character_mapping)
-
-    logger.debug("Setup 'Glyphs'")
     glyphs = {}
     for glyph_context in context.get_glyphs():
-        cache_tag = f'{glyph_context.advance_width}#{glyph_context.offset}#{glyph_context.data}'.replace(' ', '')
-        if getattr(glyph_context, _CACHE_NAME_TAG, None) != cache_tag:
-            setattr(glyph_context, _CACHE_NAME_OUTLINES, None)
-            setattr(glyph_context, _CACHE_NAME_OTF_GLYPH, None)
-            setattr(glyph_context, _CACHE_NAME_TTF_GLYPH, None)
-            setattr(glyph_context, _CACHE_NAME_TAG, cache_tag)
-
-        outlines = getattr(glyph_context, _CACHE_NAME_OUTLINES, None)
-        if outlines is None:
-            logger.debug("Create 'Outlines': %s", glyph_context.name)
-            outlines = _create_outlines(glyph_context.data, context.opentype_configs.px_to_units)
-            setattr(glyph_context, _CACHE_NAME_OUTLINES, outlines)
-        else:
-            logger.debug("Use cached 'Outlines': %s", glyph_context.name)
-
-        cache_name_xtf_glyph = _CACHE_NAME_TTF_GLYPH if is_ttf else _CACHE_NAME_OTF_GLYPH
-        glyph = getattr(glyph_context, cache_name_xtf_glyph, None)
-        if glyph is None:
-            logger.debug("Create '%sGlyph': %s", xtf_name, glyph_context.name)
-            glyph = _create_glyph(outlines, glyph_context, context.opentype_configs.px_to_units, is_ttf)
-            setattr(glyph_context, cache_name_xtf_glyph, glyph)
-        else:
-            logger.debug("Use cached '%sGlyph': %s", xtf_name, glyph_context.name)
-        glyphs[glyph_context.name] = glyph
+        if glyph_context.name != '.notdef':
+            glyph_order.append(glyph_context.name)
+        glyphs[glyph_context.name] = _get_glyph_with_cache(glyph_context, context.opentype_configs.px_to_units, is_ttf)
+    builder.setupGlyphOrder(glyph_order)
     if is_ttf:
         builder.setupGlyf(glyphs)
     else:
         if context.opentype_configs.cff_family_name is not None:
             cff_family_name = context.opentype_configs.cff_family_name
         else:
             cff_family_name = context.meta_infos.family_name
@@ -276,14 +273,17 @@
             'FullName': f'{cff_family_name} {context.meta_infos.style_name}',
             'Weight': context.meta_infos.style_name,
         }
         if context.meta_infos.copyright_info is not None:
             cff_font_infos['Notice'] = context.meta_infos.copyright_info
         builder.setupCFF(cff_ps_name, cff_font_infos, glyphs, {})
 
+    logger.debug("Setup 'Character Mapping'")
+    builder.setupCharacterMap(context.character_mapping)
+
     logger.debug("Setup 'Horizontal Metrics'")
     horizontal_metrics = {}
     for glyph_name in glyph_order:
         advance_width = context.get_glyph(glyph_name).advance_width * context.opentype_configs.px_to_units
         if is_ttf:
             lsb = glyphs[glyph_name].xMin
         else:
@@ -313,15 +313,15 @@
     logger.debug("Setup 'Post'")
     builder.setupPost()
 
     if flavor is not None:
         logger.debug("Setup 'Flavor': %s", flavor)
         builder.font.flavor = flavor
 
-    logger.debug("Create '%sBuilder' finished", xtf_name)
+    logger.debug("Create '%sBuilder' finished", 'TTF' if is_ttf else 'OTF')
     return builder
 
 
 def create_collection_builder(context: 'font.FontCollectionBuilder', is_ttf: bool) -> TTCollection:
     collection_builder = TTCollection()
     for font_context in context.font_builders:
         collection_builder.fonts.append(create_builder(font_context, is_ttf).font)
```

### Comparing `pixel-font-builder-0.0.6/src/pixel_font_builder.egg-info/PKG-INFO` & `pixel-font-builder-0.0.7/src/pixel_font_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixel-font-builder
-Version: 0.0.6
+Version: 0.0.7
 Summary: A library that helps create pixel style fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/pixel-font-builder
 Project-URL: source, https://github.com/TakWolf/pixel-font-builder
 Project-URL: issues, https://github.com/TakWolf/pixel-font-builder/issues
```

