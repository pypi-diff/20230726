# Comparing `tmp/text2hologram-0.0.2.tar.gz` & `tmp/text2hologram-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2hologram-0.0.2.tar", last modified: Wed Jul 26 18:34:23 2023, max compression
+gzip compressed data, was "text2hologram-0.0.3.tar", last modified: Wed Jul 26 19:15:31 2023, max compression
```

## Comparing `text2hologram-0.0.2.tar` & `text2hologram-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 18:34:23.869634 text2hologram-0.0.2/
--rw-rw-rw-   0        0        0       20 2023-07-26 18:34:11.000000 text2hologram-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      698 2023-07-26 18:34:23.869634 text2hologram-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-22 16:43:03.000000 text2hologram-0.0.2/README.md
--rw-rw-rw-   0        0        0      936 2023-07-26 18:33:09.000000 text2hologram-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 18:34:23.869634 text2hologram-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 18:34:23.844030 text2hologram-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 18:34:23.859116 text2hologram-0.0.2/src/text2hologram/
--rw-rw-rw-   0        0        0     1455 2023-07-26 18:11:18.000000 text2hologram-0.0.2/src/text2hologram/__main__.py
--rw-rw-rw-   0        0        0      964 2023-07-26 17:27:33.000000 text2hologram-0.0.2/src/text2hologram/config.json
--rw-rw-rw-   0        0        0      338 2023-07-26 18:05:23.000000 text2hologram-0.0.2/src/text2hologram/device_setup.py
--rw-rw-rw-   0        0        0      896 2023-07-26 18:06:20.000000 text2hologram-0.0.2/src/text2hologram/image_generation.py
--rw-rw-rw-   0        0        0      703 2023-07-26 18:13:39.000000 text2hologram-0.0.2/src/text2hologram/model.py
--rw-rw-rw-   0        0        0     7070 2023-07-26 18:07:58.000000 text2hologram-0.0.2/src/text2hologram/post_processing.py
--rw-rw-rw-   0        0        0      392 2023-07-26 18:05:13.000000 text2hologram-0.0.2/src/text2hologram/settings.py
--rw-rw-rw-   0        0        0      340 2023-07-25 22:48:04.000000 text2hologram-0.0.2/src/text2hologram/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 18:34:23.867634 text2hologram-0.0.2/src/text2hologram.egg-info/
--rw-rw-rw-   0        0        0      698 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 19:15:31.715929 text2hologram-0.0.3/
+-rw-rw-rw-   0        0        0       20 2023-07-26 18:34:11.000000 text2hologram-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      698 2023-07-26 19:15:31.714245 text2hologram-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-07-22 16:43:03.000000 text2hologram-0.0.3/README.md
+-rw-rw-rw-   0        0        0      826 2023-07-26 19:15:20.000000 text2hologram-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 19:15:31.715929 text2hologram-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 19:15:31.686898 text2hologram-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 19:15:31.703726 text2hologram-0.0.3/src/text2hologram/
+-rw-rw-rw-   0        0        0     1525 2023-07-26 18:50:40.000000 text2hologram-0.0.3/src/text2hologram/__main__.py
+-rw-rw-rw-   0        0        0      964 2023-07-26 18:37:12.000000 text2hologram-0.0.3/src/text2hologram/config.json
+-rw-rw-rw-   0        0        0      338 2023-07-26 18:37:12.000000 text2hologram-0.0.3/src/text2hologram/device_setup.py
+-rw-rw-rw-   0        0        0      910 2023-07-26 18:51:12.000000 text2hologram-0.0.3/src/text2hologram/image_generation.py
+-rw-rw-rw-   0        0        0      703 2023-07-26 18:37:12.000000 text2hologram-0.0.3/src/text2hologram/model.py
+-rw-rw-rw-   0        0        0     7070 2023-07-26 18:37:12.000000 text2hologram-0.0.3/src/text2hologram/post_processing.py
+-rw-rw-rw-   0        0        0      663 2023-07-26 18:55:16.000000 text2hologram-0.0.3/src/text2hologram/settings.py
+-rw-rw-rw-   0        0        0      340 2023-07-26 18:37:12.000000 text2hologram-0.0.3/src/text2hologram/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:15:31.713245 text2hologram-0.0.3/src/text2hologram.egg-info/
+-rw-rw-rw-   0        0        0      698 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 19:15:31.000000 text2hologram-0.0.3/src/text2hologram.egg-info/top_level.txt
```

### Comparing `text2hologram-0.0.2/PKG-INFO` & `text2hologram-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2hologram
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate holograms from text
 Author-email: Pengze Li <linsonng@163.com>
 Project-URL: Homepage, https://github.com/Linsonng/text2hologram
 Keywords: text,hologram
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `text2hologram-0.0.2/pyproject.toml` & `text2hologram-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,37 +2,32 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text2hologram"
-version = "0.0.2"
+version = "0.0.3"
 description = "Generate holograms from text"
 readme = "README.md"
 authors = [{ name = "Pengze Li", email = "linsonng@163.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["text", "hologram"]
 dependencies = [
-    "xformers>=0.0.20",
-    "matplotlib",
-    "timm",
     "odak",
-    "mediapy",
+    "timm",
     "transformers",
-    "opencv-python",
     "diffusers",
     "accelerate",
     "torch>=2.0.1",
-    "torchvision>=0.15.2",
 ]
 requires-python = ">=3.9"
 
 
 [project.urls]
 Homepage = "https://github.com/Linsonng/text2hologram"
```

### Comparing `text2hologram-0.0.2/src/text2hologram/__main__.py` & `text2hologram-0.0.3/src/text2hologram/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from settings import load_settings, update_settings
-from device_setup import setup_device
-from model import load_model
-from image_generation import generate_images
-from post_processing import process_depth_map, cgh
+from text2hologram.settings import load_settings, update_settings
+from text2hologram.device_setup import setup_device
+from text2hologram.model import load_model
+from text2hologram.image_generation import generate_images
+from text2hologram.post_processing import process_depth_map, cgh
 import argparse
 import numpy as np
 
 def parse_arguments():
     # Load default settings from config.json
     settings = load_settings()
     # Define command line arguments
```

### Comparing `text2hologram-0.0.2/src/text2hologram/config.json` & `text2hologram-0.0.3/src/text2hologram/config.json`

 * *Files identical despite different names*

### Comparing `text2hologram-0.0.2/src/text2hologram/image_generation.py` & `text2hologram-0.0.3/src/text2hologram/image_generation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 import random
-from utils import create_dirs
+from text2hologram.utils import create_dirs
 from PIL import Image
 
 def generate_images(pipe, prompt, settings):
     seed = random.randint(0, 2147483647)
     negative_prompt = "nude, naked"
     print("Creating images.")
     images = pipe(
```

### Comparing `text2hologram-0.0.2/src/text2hologram/model.py` & `text2hologram-0.0.3/src/text2hologram/model.py`

 * *Files identical despite different names*

### Comparing `text2hologram-0.0.2/src/text2hologram/post_processing.py` & `text2hologram-0.0.3/src/text2hologram/post_processing.py`

 * *Files identical despite different names*

### Comparing `text2hologram-0.0.2/src/text2hologram.egg-info/PKG-INFO` & `text2hologram-0.0.3/src/text2hologram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2hologram
-Version: 0.0.2
+Version: 0.0.3
 Summary: Generate holograms from text
 Author-email: Pengze Li <linsonng@163.com>
 Project-URL: Homepage, https://github.com/Linsonng/text2hologram
 Keywords: text,hologram
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `text2hologram-0.0.2/src/text2hologram.egg-info/SOURCES.txt` & `text2hologram-0.0.3/src/text2hologram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

