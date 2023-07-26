# Comparing `tmp/large-image-source-vips-1.23.3.dev16.tar.gz` & `tmp/large-image-source-vips-1.23.3.dev22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-vips-1.23.3.dev16.tar", last modified: Wed Jul 26 14:30:55 2023, max compression
+gzip compressed data, was "large-image-source-vips-1.23.3.dev22.tar", last modified: Wed Jul 26 15:07:17 2023, max compression
```

## Comparing `large-image-source-vips-1.23.3.dev16.tar` & `large-image-source-vips-1.23.3.dev22.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 14:30:55.763513 large-image-source-vips-1.23.3.dev16/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-07-26 14:30:55.000000 large-image-source-vips-1.23.3.dev16/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-07-26 14:30:55.763513 large-image-source-vips-1.23.3.dev16/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-07-26 14:30:55.000000 large-image-source-vips-1.23.3.dev16/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 14:30:55.759513 large-image-source-vips-1.23.3.dev16/large_image_source_vips/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24064 2023-07-26 14:29:11.000000 large-image-source-vips-1.23.3.dev16/large_image_source_vips/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-07-26 14:29:11.000000 large-image-source-vips-1.23.3.dev16/large_image_source_vips/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 14:30:55.763513 large-image-source-vips-1.23.3.dev16/large_image_source_vips.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-07-26 14:30:55.000000 large-image-source-vips-1.23.3.dev16/large_image_source_vips.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-07-26 14:30:55.000000 large-image-source-vips-1.23.3.dev16/large_image_source_vips.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 14:30:55.000000 large-image-source-vips-1.23.3.dev16/large_image_source_vips.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2023-07-26 14:30:55.000000 large-image-source-vips-1.23.3.dev16/large_image_source_vips.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2023-07-26 14:30:55.000000 large-image-source-vips-1.23.3.dev16/large_image_source_vips.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-07-26 14:30:55.000000 large-image-source-vips-1.23.3.dev16/large_image_source_vips.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-26 14:30:55.763513 large-image-source-vips-1.23.3.dev16/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-07-26 14:29:11.000000 large-image-source-vips-1.23.3.dev16/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:07:17.738043 large-image-source-vips-1.23.3.dev22/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-07-26 15:07:17.000000 large-image-source-vips-1.23.3.dev22/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-07-26 15:07:17.738043 large-image-source-vips-1.23.3.dev22/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-07-26 15:07:17.000000 large-image-source-vips-1.23.3.dev22/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:07:17.734043 large-image-source-vips-1.23.3.dev22/large_image_source_vips/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24064 2023-07-26 15:05:31.000000 large-image-source-vips-1.23.3.dev22/large_image_source_vips/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-07-26 15:05:31.000000 large-image-source-vips-1.23.3.dev22/large_image_source_vips/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-26 15:07:17.738043 large-image-source-vips-1.23.3.dev22/large_image_source_vips.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-07-26 15:07:17.000000 large-image-source-vips-1.23.3.dev22/large_image_source_vips.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      388 2023-07-26 15:07:17.000000 large-image-source-vips-1.23.3.dev22/large_image_source_vips.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-26 15:07:17.000000 large-image-source-vips-1.23.3.dev22/large_image_source_vips.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      166 2023-07-26 15:07:17.000000 large-image-source-vips-1.23.3.dev22/large_image_source_vips.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2023-07-26 15:07:17.000000 large-image-source-vips-1.23.3.dev22/large_image_source_vips.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-07-26 15:07:17.000000 large-image-source-vips-1.23.3.dev22/large_image_source_vips.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-26 15:07:17.738043 large-image-source-vips-1.23.3.dev22/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2590 2023-07-26 15:05:31.000000 large-image-source-vips-1.23.3.dev22/setup.py
```

### Comparing `large-image-source-vips-1.23.3.dev16/LICENSE` & `large-image-source-vips-1.23.3.dev22/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.3.dev16/PKG-INFO` & `large-image-source-vips-1.23.3.dev22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.23.3.dev16
+Version: 1.23.3.dev22
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.23.3.dev16/README.rst` & `large-image-source-vips-1.23.3.dev22/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.3.dev16/large_image_source_vips/__init__.py` & `large-image-source-vips-1.23.3.dev22/large_image_source_vips/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-vips-1.23.3.dev16/large_image_source_vips.egg-info/PKG-INFO` & `large-image-source-vips-1.23.3.dev22/large_image_source_vips.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-vips
-Version: 1.23.3.dev16
+Version: 1.23.3.dev22
 Summary: A libvips tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-vips-1.23.3.dev16/setup.py` & `large-image-source-vips-1.23.3.dev22/setup.py`

 * *Files identical despite different names*

