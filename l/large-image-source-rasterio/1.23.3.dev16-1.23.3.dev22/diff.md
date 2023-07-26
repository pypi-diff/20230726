# Comparing `tmp/large-image-source-rasterio-1.23.3.dev16.tar.gz` & `tmp/large-image-source-rasterio-1.23.3.dev22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-rasterio-1.23.3.dev16.tar", last modified: Wed Jul 26 14:30:38 2023, max compression
+gzip compressed data, was "large-image-source-rasterio-1.23.3.dev22.tar", last modified: Wed Jul 26 15:07:00 2023, max compression
```

## Comparing `large-image-source-rasterio-1.23.3.dev16.tar` & `large-image-source-rasterio-1.23.3.dev22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 14:30:38.987482 large-image-source-rasterio-1.23.3.dev16/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-07-26 14:30:38.000000 large-image-source-rasterio-1.23.3.dev16/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      846 2023-07-26 14:30:38.987482 large-image-source-rasterio-1.23.3.dev16/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-07-26 14:30:38.000000 large-image-source-rasterio-1.23.3.dev16/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 14:30:38.987482 large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43030 2023-07-26 14:29:11.000000 large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-07-26 14:29:11.000000 large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 14:30:38.987482 large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      846 2023-07-26 14:30:38.000000 large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-07-26 14:30:38.000000 large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 14:30:38.000000 large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-07-26 14:30:38.000000 large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-07-26 14:30:38.000000 large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-07-26 14:30:38.000000 large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-26 14:30:38.987482 large-image-source-rasterio-1.23.3.dev16/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2615 2023-07-26 14:29:11.000000 large-image-source-rasterio-1.23.3.dev16/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:07:00.078172 large-image-source-rasterio-1.23.3.dev22/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-07-26 15:06:59.000000 large-image-source-rasterio-1.23.3.dev22/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      846 2023-07-26 15:07:00.078172 large-image-source-rasterio-1.23.3.dev22/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-07-26 15:06:59.000000 large-image-source-rasterio-1.23.3.dev22/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:07:00.078172 large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43030 2023-07-26 15:05:31.000000 large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-07-26 15:05:31.000000 large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:07:00.078172 large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      846 2023-07-26 15:06:59.000000 large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-07-26 15:07:00.000000 large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 15:06:59.000000 large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-07-26 15:06:59.000000 large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-07-26 15:06:59.000000 large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-07-26 15:06:59.000000 large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-26 15:07:00.078172 large-image-source-rasterio-1.23.3.dev22/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2615 2023-07-26 15:05:31.000000 large-image-source-rasterio-1.23.3.dev22/setup.py
```

### Comparing `large-image-source-rasterio-1.23.3.dev16/LICENSE` & `large-image-source-rasterio-1.23.3.dev22/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.3.dev16/PKG-INFO` & `large-image-source-rasterio-1.23.3.dev22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.23.3.dev16
+Version: 1.23.3.dev22
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.23.3.dev16/README.rst` & `large-image-source-rasterio-1.23.3.dev22/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio/__init__.py` & `large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio/girder_source.py` & `large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.3.dev16/large_image_source_rasterio.egg-info/PKG-INFO` & `large-image-source-rasterio-1.23.3.dev22/large_image_source_rasterio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.23.3.dev16
+Version: 1.23.3.dev22
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.23.3.dev16/setup.py` & `large-image-source-rasterio-1.23.3.dev22/setup.py`

 * *Files identical despite different names*

