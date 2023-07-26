# Comparing `tmp/picframe-2023.7.26.tar.gz` & `tmp/picframe-2023.7.26.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picframe-2023.7.26.tar", last modified: Wed Jul 26 09:07:52 2023, max compression
+gzip compressed data, was "picframe-2023.7.26.post1.tar", last modified: Wed Jul 26 11:47:36 2023, max compression
```

## Comparing `picframe-2023.7.26.tar` & `picframe-2023.7.26.post1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.033271 picframe-2023.7.26/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 09:07:33.000000 picframe-2023.7.26/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-26 09:07:52.033271 picframe-2023.7.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-26 09:07:33.000000 picframe-2023.7.26/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-26 09:07:33.000000 picframe-2023.7.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 09:07:52.033271 picframe-2023.7.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 09:07:33.000000 picframe-2023.7.26/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.025271 picframe-2023.7.26/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.029271 picframe-2023.7.26/src/picframe/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-26 09:07:52.033271 picframe-2023.7.26/src/picframe/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.029271 picframe-2023.7.26/src/picframe/config/
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/config/configuration_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.029271 picframe-2023.7.26/src/picframe/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.029271 picframe-2023.7.26/src/picframe/data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/fonts/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   455164 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/fonts/NotoSans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   471004 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/fonts/NotoSans-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   470472 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/fonts/NotoSans-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   455188 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/fonts/NotoSans-Regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.033271 picframe-2023.7.26/src/picframe/data/mat/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/mat/9_patch_bevel.png
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/mat/9_patch_drop_shadow.png
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/mat/9_patch_highlight.png
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/mat/9_patch_inner_shadow.png
--rw-r--r--   0 runner    (1001) docker     (123)  2081776 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/mat/mat_texture.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   160442 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/no_pictures.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.033271 picframe-2023.7.26/src/picframe/data/shaders/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/shaders/blend_new.fs
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/data/shaders/blend_new.vs
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/geo_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/get_image_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.033271 picframe-2023.7.26/src/picframe/html/
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/html/pf_functions.js
--rw-r--r--   0 runner    (1001) docker     (123)    24184 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/interface_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/interface_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/interface_peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/mat_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/start.py
--rw-r--r--   0 runner    (1001) docker     (123)    27228 2023-07-26 09:07:33.000000 picframe-2023.7.26/src/picframe/viewer_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.029271 picframe-2023.7.26/src/picframe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-26 09:07:52.000000 picframe-2023.7.26/src/picframe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-26 09:07:52.000000 picframe-2023.7.26/src/picframe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:07:52.000000 picframe-2023.7.26/src/picframe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 09:07:52.000000 picframe-2023.7.26/src/picframe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-26 09:07:52.000000 picframe-2023.7.26/src/picframe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 09:07:52.000000 picframe-2023.7.26/src/picframe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:07:52.033271 picframe-2023.7.26/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-26 09:07:33.000000 picframe-2023.7.26/test/test_get_image_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-26 09:07:33.000000 picframe-2023.7.26/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.272265 picframe-2023.7.26.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-26 11:47:36.272265 picframe-2023.7.26.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-26 11:47:36.272265 picframe-2023.7.26.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.260265 picframe-2023.7.26.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.264265 picframe-2023.7.26.post1/src/picframe/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-26 11:47:36.272265 picframe-2023.7.26.post1/src/picframe/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.264265 picframe-2023.7.26.post1/src/picframe/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/config/configuration_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13775 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.264265 picframe-2023.7.26.post1/src/picframe/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.268265 picframe-2023.7.26.post1/src/picframe/data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/fonts/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   455164 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   471004 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   470472 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   455188 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.268265 picframe-2023.7.26.post1/src/picframe/data/mat/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/mat/9_patch_bevel.png
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/mat/9_patch_drop_shadow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/mat/9_patch_highlight.png
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/mat/9_patch_inner_shadow.png
+-rw-r--r--   0 runner    (1001) docker     (123)  2081776 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/mat/mat_texture.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   160442 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/no_pictures.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.268265 picframe-2023.7.26.post1/src/picframe/data/shaders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/shaders/blend_new.fs
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/data/shaders/blend_new.vs
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/geo_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/get_image_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.268265 picframe-2023.7.26.post1/src/picframe/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/html/pf_functions.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24184 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/interface_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23963 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/interface_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/interface_peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17726 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/mat_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17397 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27228 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/src/picframe/viewer_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.264265 picframe-2023.7.26.post1/src/picframe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 11:47:36.000000 picframe-2023.7.26.post1/src/picframe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:47:36.268265 picframe-2023.7.26.post1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/test/test_get_image_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-26 11:47:21.000000 picframe-2023.7.26.post1/versioneer.py
```

### Comparing `picframe-2023.7.26/LICENSE` & `picframe-2023.7.26.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/PKG-INFO` & `picframe-2023.7.26.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: picframe
-Version: 2023.7.26
+Version: 2023.7.26.post1
 Summary: Picture frame viewer powered by raspberry with homeassistant integration
 Author: Paddy Gaunt, Jeff Godfrey
 Author-email: Helge Erbe <helge@erbehome.de>
 Maintainer-email: Helge Erbe <helge@erbehome.de>
 License: MIT
 Project-URL: Homepage, https://github.com/helgeerbe/picframe
 Keywords: picframe,viewer,raspberry,raspi,homeassistant,hass
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,14 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PictureFrame powered by pi3d
 
 ![picframe logo](https://github.com/helgeerbe/picframe/wiki/images/Picframe_Logo.png)
 
+- [![PyPI version](https://badge.fury.io/py/picframe.svg)](https://badge.fury.io/py/picframe)
 - [PictureFrame powered by pi3d](#pictureframe-powered-by-pi3d)
 - [What Is PictureFrame?](#what-is-pictureframe)
 - [History of PictureFrame](#history-of-pictureframe)
 - [Highlights of PictureFrame](#highlights-of-pictureframe)
 - [Documentation](#documentation)
 - [Acknowledgement](#acknowledgement)
```

### Comparing `picframe-2023.7.26/README.md` & `picframe-2023.7.26.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ## PictureFrame powered by pi3d
 
 ![picframe logo](https://github.com/helgeerbe/picframe/wiki/images/Picframe_Logo.png)
 
+- [![PyPI version](https://badge.fury.io/py/picframe.svg)](https://badge.fury.io/py/picframe)
 - [PictureFrame powered by pi3d](#pictureframe-powered-by-pi3d)
 - [What Is PictureFrame?](#what-is-pictureframe)
 - [History of PictureFrame](#history-of-pictureframe)
 - [Highlights of PictureFrame](#highlights-of-pictureframe)
 - [Documentation](#documentation)
 - [Acknowledgement](#acknowledgement)
```

### Comparing `picframe-2023.7.26/pyproject.toml` & `picframe-2023.7.26.post1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -20,27 +20,27 @@
 maintainers = [
   { name = "Helge Erbe", email = "helge@erbehome.de"  },
 ]
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.7"
 classifiers=[
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Multimedia :: Graphics :: Viewers",
 ]
 dynamic = ["version"]
 dependencies = [
-    "Pillow>=10.0.0",
+    "Pillow==9.5.0",
     "defusedxml",
     "pi3d>=2.49",
     "PyYAML",
     "paho-mqtt",
     "IPTCInfo3",
     "numpy",
     "ninepatch",
```

### Comparing `picframe-2023.7.26/src/picframe/config/configuration_example.yaml` & `picframe-2023.7.26.post1/src/picframe/config/configuration_example.yaml`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/controller.py` & `picframe-2023.7.26.post1/src/picframe/controller.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/data/fonts/LICENSE.txt` & `picframe-2023.7.26.post1/src/picframe/data/fonts/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/data/fonts/NotoSans-Bold.ttf` & `picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/data/fonts/NotoSans-BoldItalic.ttf` & `picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/data/fonts/NotoSans-Italic.ttf` & `picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/data/fonts/NotoSans-Regular.ttf` & `picframe-2023.7.26.post1/src/picframe/data/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/data/mat/9_patch_drop_shadow.png` & `picframe-2023.7.26.post1/src/picframe/data/mat/9_patch_drop_shadow.png`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/data/mat/mat_texture.jpg` & `picframe-2023.7.26.post1/src/picframe/data/mat/mat_texture.jpg`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/data/no_pictures.jpg` & `picframe-2023.7.26.post1/src/picframe/data/no_pictures.jpg`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/data/shaders/blend_new.fs` & `picframe-2023.7.26.post1/src/picframe/data/shaders/blend_new.fs`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/geo_reverse.py` & `picframe-2023.7.26.post1/src/picframe/geo_reverse.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/get_image_meta.py` & `picframe-2023.7.26.post1/src/picframe/get_image_meta.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/html/index.html` & `picframe-2023.7.26.post1/src/picframe/html/index.html`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/html/pf_functions.js` & `picframe-2023.7.26.post1/src/picframe/html/pf_functions.js`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/image_cache.py` & `picframe-2023.7.26.post1/src/picframe/image_cache.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/interface_http.py` & `picframe-2023.7.26.post1/src/picframe/interface_http.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/interface_mqtt.py` & `picframe-2023.7.26.post1/src/picframe/interface_mqtt.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/interface_peripherals.py` & `picframe-2023.7.26.post1/src/picframe/interface_peripherals.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/mat_image.py` & `picframe-2023.7.26.post1/src/picframe/mat_image.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/model.py` & `picframe-2023.7.26.post1/src/picframe/model.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/start.py` & `picframe-2023.7.26.post1/src/picframe/start.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe/viewer_display.py` & `picframe-2023.7.26.post1/src/picframe/viewer_display.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/src/picframe.egg-info/PKG-INFO` & `picframe-2023.7.26.post1/src/picframe.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: picframe
-Version: 2023.7.26
+Version: 2023.7.26.post1
 Summary: Picture frame viewer powered by raspberry with homeassistant integration
 Author: Paddy Gaunt, Jeff Godfrey
 Author-email: Helge Erbe <helge@erbehome.de>
 Maintainer-email: Helge Erbe <helge@erbehome.de>
 License: MIT
 Project-URL: Homepage, https://github.com/helgeerbe/picframe
 Keywords: picframe,viewer,raspberry,raspi,homeassistant,hass
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,14 +21,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## PictureFrame powered by pi3d
 
 ![picframe logo](https://github.com/helgeerbe/picframe/wiki/images/Picframe_Logo.png)
 
+- [![PyPI version](https://badge.fury.io/py/picframe.svg)](https://badge.fury.io/py/picframe)
 - [PictureFrame powered by pi3d](#pictureframe-powered-by-pi3d)
 - [What Is PictureFrame?](#what-is-pictureframe)
 - [History of PictureFrame](#history-of-pictureframe)
 - [Highlights of PictureFrame](#highlights-of-pictureframe)
 - [Documentation](#documentation)
 - [Acknowledgement](#acknowledgement)
```

### Comparing `picframe-2023.7.26/src/picframe.egg-info/SOURCES.txt` & `picframe-2023.7.26.post1/src/picframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/test/test_get_image_meta.py` & `picframe-2023.7.26.post1/test/test_get_image_meta.py`

 * *Files identical despite different names*

### Comparing `picframe-2023.7.26/versioneer.py` & `picframe-2023.7.26.post1/versioneer.py`

 * *Files identical despite different names*

