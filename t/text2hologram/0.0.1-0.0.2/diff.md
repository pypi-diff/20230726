# Comparing `tmp/text2hologram-0.0.1.tar.gz` & `tmp/text2hologram-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2hologram-0.0.1.tar", last modified: Sat Jul 22 17:12:33 2023, max compression
+gzip compressed data, was "text2hologram-0.0.2.tar", last modified: Wed Jul 26 18:34:23 2023, max compression
```

## Comparing `text2hologram-0.0.1.tar` & `text2hologram-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 17:12:33.844837 text2hologram-0.0.1/
--rw-rw-rw-   0        0        0      698 2023-07-22 17:12:33.844837 text2hologram-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-22 16:43:03.000000 text2hologram-0.0.1/README.md
--rw-rw-rw-   0        0        0      934 2023-07-22 17:10:30.000000 text2hologram-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 17:12:33.844837 text2hologram-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-22 17:12:33.830836 text2hologram-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-22 17:12:33.834837 text2hologram-0.0.1/src/text2hologram/
--rw-rw-rw-   0        0        0    14764 2023-07-22 16:24:24.000000 text2hologram-0.0.1/src/text2hologram/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-22 17:12:33.842836 text2hologram-0.0.1/src/text2hologram.egg-info/
--rw-rw-rw-   0        0        0      698 2023-07-22 17:12:33.000000 text2hologram-0.0.1/src/text2hologram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-22 17:12:33.000000 text2hologram-0.0.1/src/text2hologram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 17:12:33.000000 text2hologram-0.0.1/src/text2hologram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-22 17:12:33.000000 text2hologram-0.0.1/src/text2hologram.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2023-07-22 17:12:33.000000 text2hologram-0.0.1/src/text2hologram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-22 17:12:33.000000 text2hologram-0.0.1/src/text2hologram.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 18:34:23.869634 text2hologram-0.0.2/
+-rw-rw-rw-   0        0        0       20 2023-07-26 18:34:11.000000 text2hologram-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      698 2023-07-26 18:34:23.869634 text2hologram-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-07-22 16:43:03.000000 text2hologram-0.0.2/README.md
+-rw-rw-rw-   0        0        0      936 2023-07-26 18:33:09.000000 text2hologram-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 18:34:23.869634 text2hologram-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 18:34:23.844030 text2hologram-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 18:34:23.859116 text2hologram-0.0.2/src/text2hologram/
+-rw-rw-rw-   0        0        0     1455 2023-07-26 18:11:18.000000 text2hologram-0.0.2/src/text2hologram/__main__.py
+-rw-rw-rw-   0        0        0      964 2023-07-26 17:27:33.000000 text2hologram-0.0.2/src/text2hologram/config.json
+-rw-rw-rw-   0        0        0      338 2023-07-26 18:05:23.000000 text2hologram-0.0.2/src/text2hologram/device_setup.py
+-rw-rw-rw-   0        0        0      896 2023-07-26 18:06:20.000000 text2hologram-0.0.2/src/text2hologram/image_generation.py
+-rw-rw-rw-   0        0        0      703 2023-07-26 18:13:39.000000 text2hologram-0.0.2/src/text2hologram/model.py
+-rw-rw-rw-   0        0        0     7070 2023-07-26 18:07:58.000000 text2hologram-0.0.2/src/text2hologram/post_processing.py
+-rw-rw-rw-   0        0        0      392 2023-07-26 18:05:13.000000 text2hologram-0.0.2/src/text2hologram/settings.py
+-rw-rw-rw-   0        0        0      340 2023-07-25 22:48:04.000000 text2hologram-0.0.2/src/text2hologram/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:34:23.867634 text2hologram-0.0.2/src/text2hologram.egg-info/
+-rw-rw-rw-   0        0        0      698 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 18:34:23.000000 text2hologram-0.0.2/src/text2hologram.egg-info/top_level.txt
```

### Comparing `text2hologram-0.0.1/PKG-INFO` & `text2hologram-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2hologram
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate holograms from text
 Author-email: Pengze Li <linsonng@163.com>
 Project-URL: Homepage, https://github.com/Linsonng/text2hologram
 Keywords: text,hologram
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `text2hologram-0.0.1/pyproject.toml` & `text2hologram-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "text2hologram"
-version = "0.0.1"
+version = "0.0.2"
 description = "Generate holograms from text"
 readme = "README.md"
 authors = [{ name = "Pengze Li", email = "linsonng@163.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -33,8 +33,8 @@
 requires-python = ">=3.9"
 
 
 [project.urls]
 Homepage = "https://github.com/Linsonng/text2hologram"
 
 [project.scripts]
-text2hologram = "text2hologram.__main__:main"
+text2hologram = "text2hologram.__main__:main"
```

### Comparing `text2hologram-0.0.1/src/text2hologram.egg-info/PKG-INFO` & `text2hologram-0.0.2/src/text2hologram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2hologram
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate holograms from text
 Author-email: Pengze Li <linsonng@163.com>
 Project-URL: Homepage, https://github.com/Linsonng/text2hologram
 Keywords: text,hologram
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

