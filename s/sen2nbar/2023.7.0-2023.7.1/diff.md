# Comparing `tmp/sen2nbar-2023.7.0.tar.gz` & `tmp/sen2nbar-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sen2nbar-2023.7.0.tar", last modified: Sun Jul  9 18:24:22 2023, max compression
+gzip compressed data, was "dist/sen2nbar-2023.7.1.tar", last modified: Wed Jul 26 09:18:18 2023, max compression
```

## Comparing `sen2nbar-2023.7.0.tar` & `sen2nbar-2023.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 18:24:22.793621 sen2nbar-2023.7.0/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 13:18:33.000000 sen2nbar-2023.7.0/LICENSE
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-09 18:24:22.793621 sen2nbar-2023.7.0/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7217 2023-07-09 13:18:33.000000 sen2nbar-2023.7.0/README.md
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 18:24:22.790287 sen2nbar-2023.7.0/sen2nbar/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      194 2023-07-09 18:13:00.000000 sen2nbar-2023.7.0/sen2nbar/__init__.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      604 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/axioms.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1679 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/brdf.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2936 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/c_factor.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     3695 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/kernels.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4340 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/metadata.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7479 2023-07-09 18:12:35.000000 sen2nbar-2023.7.0/sen2nbar/nbar.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1558 2023-07-09 13:18:34.000000 sen2nbar-2023.7.0/sen2nbar/utils.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 18:24:22.793621 sen2nbar-2023.7.0/sen2nbar.egg-info/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-09 18:24:22.000000 sen2nbar-2023.7.0/sen2nbar.egg-info/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      339 2023-07-09 18:24:22.000000 sen2nbar-2023.7.0/sen2nbar.egg-info/SOURCES.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-09 18:24:22.000000 sen2nbar-2023.7.0/sen2nbar.egg-info/dependency_links.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       94 2023-07-09 18:24:22.000000 sen2nbar-2023.7.0/sen2nbar.egg-info/requires.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        9 2023-07-09 18:24:22.000000 sen2nbar-2023.7.0/sen2nbar.egg-info/top_level.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-09 18:24:22.793621 sen2nbar-2023.7.0/setup.cfg
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1234 2023-07-09 18:12:52.000000 sen2nbar-2023.7.0/setup.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 09:18:18.872135 sen2nbar-2023.7.1/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 13:18:33.000000 sen2nbar-2023.7.1/LICENSE
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-26 09:18:18.872135 sen2nbar-2023.7.1/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7217 2023-07-09 13:18:33.000000 sen2nbar-2023.7.1/README.md
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 09:18:18.868801 sen2nbar-2023.7.1/sen2nbar/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      194 2023-07-26 09:08:17.000000 sen2nbar-2023.7.1/sen2nbar/__init__.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      604 2023-07-09 13:18:34.000000 sen2nbar-2023.7.1/sen2nbar/axioms.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1679 2023-07-09 13:18:34.000000 sen2nbar-2023.7.1/sen2nbar/brdf.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2936 2023-07-09 13:18:34.000000 sen2nbar-2023.7.1/sen2nbar/c_factor.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     3695 2023-07-09 13:18:34.000000 sen2nbar-2023.7.1/sen2nbar/kernels.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4485 2023-07-26 08:46:17.000000 sen2nbar-2023.7.1/sen2nbar/metadata.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7546 2023-07-26 09:03:53.000000 sen2nbar-2023.7.1/sen2nbar/nbar.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1558 2023-07-09 13:18:34.000000 sen2nbar-2023.7.1/sen2nbar/utils.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 09:18:18.872135 sen2nbar-2023.7.1/sen2nbar.egg-info/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7728 2023-07-26 09:18:18.000000 sen2nbar-2023.7.1/sen2nbar.egg-info/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      339 2023-07-26 09:18:18.000000 sen2nbar-2023.7.1/sen2nbar.egg-info/SOURCES.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-26 09:18:18.000000 sen2nbar-2023.7.1/sen2nbar.egg-info/dependency_links.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       94 2023-07-26 09:18:18.000000 sen2nbar-2023.7.1/sen2nbar.egg-info/requires.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        9 2023-07-26 09:18:18.000000 sen2nbar-2023.7.1/sen2nbar.egg-info/top_level.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-26 09:18:18.872135 sen2nbar-2023.7.1/setup.cfg
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1234 2023-07-26 09:08:23.000000 sen2nbar-2023.7.1/setup.py
```

### Comparing `sen2nbar-2023.7.0/LICENSE` & `sen2nbar-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.0/PKG-INFO` & `sen2nbar-2023.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sen2nbar
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python
 Home-page: https://github.com/ESDS-Leipzig/sen2nbar
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.0 Summary: Nadir BRDF
+Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.1 Summary: Nadir BRDF
 Adjusted Reflectance (NBAR) for Sentinel-2 in Python Home-page: https://
 github.com/ESDS-Leipzig/sen2nbar Author: David Montero Loaiza Author-email:
 dml.mont@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [cubo]
```

### Comparing `sen2nbar-2023.7.0/README.md` & `sen2nbar-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.0/sen2nbar/axioms.py` & `sen2nbar-2023.7.1/sen2nbar/axioms.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.0/sen2nbar/brdf.py` & `sen2nbar-2023.7.1/sen2nbar/brdf.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.0/sen2nbar/c_factor.py` & `sen2nbar-2023.7.1/sen2nbar/c_factor.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.0/sen2nbar/kernels.py` & `sen2nbar-2023.7.1/sen2nbar/kernels.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.0/sen2nbar/metadata.py` & `sen2nbar-2023.7.1/sen2nbar/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import warnings
 
 import numpy as np
 import requests
 import xarray as xr
 import xmltodict
 
 
@@ -84,17 +85,19 @@
         bands_dict["Sun"][angle].append(
             _get_angle_values(Tile_Angles["Sun_Angles_Grid"], angle)
         )
 
     # Do the nanmean of the detectors angles per band
     for key, value in bands_dict.items():
         for angle in ANGLES:
-            bands_dict[key][angle] = np.nanmean(
-                np.array(bands_dict[key][angle]), axis=0
-            )
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore", category=RuntimeWarning)
+                bands_dict[key][angle] = np.nanmean(
+                    np.array(bands_dict[key][angle]), axis=0
+                )
         bands_dict[key] = np.array(
             [bands_dict[key]["Zenith"], bands_dict[key]["Azimuth"]]
         )
 
     # x and y coordinates of the array to create
     y = np.arange(ULY, ULY - 5000 * 23, -5000) - 2500
     x = np.arange(ULX, ULX + 5000 * 23, 5000) + 2500
```

### Comparing `sen2nbar-2023.7.0/sen2nbar/nbar.py` & `sen2nbar-2023.7.1/sen2nbar/nbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     # Compute c-factor
     c = c_factor_from_metadata(metadata)
 
     # Extrapolate c-factor
     c = _extrapolate_c_factor(c)
 
     # Initialize progress bar
-    pbar = tqdm(bands.items(), disable=quiet)
+    pbar = tqdm(bands.items(), disable=quiet, leave=False)
 
     # Compute NBAR per band
     for band, resolution in pbar:
         pbar.set_description(f"Processing {band}")
 
         # Image file
         img_path = glob(
@@ -145,15 +145,15 @@
     # Open catalogue
     CATALOG = pystac_client.Client.open(stac)
 
     # Do a search
     SEARCH = CATALOG.search(ids=da.id.values, collections=[collection])
 
     # Get the items
-    items = SEARCH.get_all_items()
+    items = SEARCH.item_collection()
 
     # Sign the items if using PC
     if stac == "https://planetarycomputer.microsoft.com/api/stac/v1":
         items = pc.sign(items)
 
     # Order items
     items_ids = [item.id for item in items]
@@ -161,15 +161,17 @@
         [np.where(da.id.values == item) for item in items_ids]
     ).ravel()
     ordered_items = np.array(items)[original_order]
 
     # Compute the c-factor per item and extract the processing baseline
     c_array = []
     processing_baseline = []
-    for item in tqdm(ordered_items, disable=quiet):
+    for item in tqdm(
+        ordered_items, disable=quiet, desc="Processing items", leave=False
+    ):
         c = c_factor_from_item(item, epsg)
         c = c.interp(
             y=da.y.values,
             x=da.x.values,
             method="linear",
             kwargs={"fill_value": "extrapolate"},
         )
```

### Comparing `sen2nbar-2023.7.0/sen2nbar/utils.py` & `sen2nbar-2023.7.1/sen2nbar/utils.py`

 * *Files identical despite different names*

### Comparing `sen2nbar-2023.7.0/sen2nbar.egg-info/PKG-INFO` & `sen2nbar-2023.7.1/sen2nbar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sen2nbar
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python
 Home-page: https://github.com/ESDS-Leipzig/sen2nbar
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.0 Summary: Nadir BRDF
+Metadata-Version: 2.1 Name: sen2nbar Version: 2023.7.1 Summary: Nadir BRDF
 Adjusted Reflectance (NBAR) for Sentinel-2 in Python Home-page: https://
 github.com/ESDS-Leipzig/sen2nbar Author: David Montero Loaiza Author-email:
 dml.mont@gmail.com License: MIT Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown License-File: LICENSE
                                     [cubo]
```

### Comparing `sen2nbar-2023.7.0/setup.py` & `sen2nbar-2023.7.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="sen2nbar",
-    version="2023.7.0",
+    version="2023.7.1",
     url="https://github.com/ESDS-Leipzig/sen2nbar",
     license="MIT",
     author="David Montero Loaiza",
     author_email="dml.mont@gmail.com",
     description="Nadir BRDF Adjusted Reflectance (NBAR) for Sentinel-2 in Python",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
```

