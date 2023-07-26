# Comparing `tmp/aksharify-0.1.7.tar.gz` & `tmp/aksharify-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aksharify-0.1.7.tar", max compression
+gzip compressed data, was "aksharify-0.1.8.tar", max compression
```

## Comparing `aksharify-0.1.7.tar` & `aksharify-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.7/LICENSE.md
--rw-r--r--   0        0        0      674 2023-07-25 06:50:23.423792 aksharify-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.7/README.md
--rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.7/src/aksharify/__init__.py
--rw-r--r--   0        0        0     5546 2023-07-24 11:46:55.981672 aksharify-0.1.7/src/aksharify/aksharify.py
--rw-r--r--   0        0        0     5327 2023-07-25 04:07:23.752855 aksharify-0.1.7/src/aksharify/distributions.py
--rw-r--r--   0        0        0     1615 2023-07-24 16:06:14.067631 aksharify-0.1.7/src/aksharify/image.py
--rw-r--r--   0        0        0     1191 2023-07-25 06:47:53.889912 aksharify-0.1.7/src/aksharify/interactive.py
--rw-r--r--   0        0        0     4946 2023-07-24 12:43:24.100266 aksharify-0.1.7/src/aksharify/outputs.py
--rw-r--r--   0        0        0     6659 1970-01-01 00:00:00.000000 aksharify-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-07-22 05:33:48.477839 aksharify-0.1.8/LICENSE.md
+-rw-r--r--   0        0        0      674 2023-07-26 09:26:53.034009 aksharify-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5988 2023-07-22 03:57:31.621402 aksharify-0.1.8/README.md
+-rw-r--r--   0        0        0       55 2023-07-21 04:56:00.214997 aksharify-0.1.8/src/aksharify/__init__.py
+-rw-r--r--   0        0        0     5632 2023-07-26 09:23:20.805879 aksharify-0.1.8/src/aksharify/aksharify.py
+-rw-r--r--   0        0        0     5327 2023-07-25 04:07:23.752855 aksharify-0.1.8/src/aksharify/distributions.py
+-rw-r--r--   0        0        0     1615 2023-07-24 16:06:14.067631 aksharify-0.1.8/src/aksharify/image.py
+-rw-r--r--   0        0        0     1191 2023-07-25 06:47:53.889912 aksharify-0.1.8/src/aksharify/interactive.py
+-rw-r--r--   0        0        0     4946 2023-07-24 12:43:24.100266 aksharify-0.1.8/src/aksharify/outputs.py
+-rw-r--r--   0        0        0     6659 1970-01-01 00:00:00.000000 aksharify-0.1.8/PKG-INFO
```

### Comparing `aksharify-0.1.7/LICENSE.md` & `aksharify-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.7/pyproject.toml` & `aksharify-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aksharify"
-version = "0.1.7"
+version = "0.1.8"
 description = "Ascii Art + Emoji Art python Package"
 authors = ["Prime Patel <primespatel@gmail.com>"]
 readme = "README.md"
 packages = [{include = "aksharify", from = "src"}]
 license = "MIT"
 homepage = "https://primepatel.github.io/aksharify/"
 repository = "https://github.com/primepatel/aksharify"
```

### Comparing `aksharify-0.1.7/README.md` & `aksharify-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.7/src/aksharify/aksharify.py` & `aksharify-0.1.8/src/aksharify/aksharify.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import IPython.display as ipd
 from io import BytesIO
 from cairosvg import svg2png, svg2pdf, svg2eps
 from .outputs import SVG
-
+from matplotlib.colors import cnames
 class AksharArt:
     
     def __init__(self, image, dist) -> None:
         self.image = image
         self.dist = dist
     
     def set_dim(self, width:int=None, height:int=None):
@@ -120,7 +120,10 @@
         svg2eps(file_obj=svg_io, write_to=eps.file_name + ".eps")
     
     def html_output(self, config):
         html = config
         with open(html.file_name + ".html", "w", encoding="utf-8") as file:
             file.write(html.generate_art(self.matrix, self.image.image))
 
+
+def hexify(color:str):
+    return cnames[color]
```

### Comparing `aksharify-0.1.7/src/aksharify/distributions.py` & `aksharify-0.1.8/src/aksharify/distributions.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.7/src/aksharify/image.py` & `aksharify-0.1.8/src/aksharify/image.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.7/src/aksharify/interactive.py` & `aksharify-0.1.8/src/aksharify/interactive.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.7/src/aksharify/outputs.py` & `aksharify-0.1.8/src/aksharify/outputs.py`

 * *Files identical despite different names*

### Comparing `aksharify-0.1.7/PKG-INFO` & `aksharify-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aksharify
-Version: 0.1.7
+Version: 0.1.8
 Summary: Ascii Art + Emoji Art python Package
 Home-page: https://primepatel.github.io/aksharify/
 License: MIT
 Keywords: Ascii Art,Emoji Art,Prime Patel,primepatel
 Author: Prime Patel
 Author-email: primespatel@gmail.com
 Requires-Python: >=3.10,<4.0
```

