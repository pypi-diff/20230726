# Comparing `tmp/mask2bbox-0.0.8.tar.gz` & `tmp/mask2bbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask2bbox-0.0.8.tar", last modified: Tue Jun 20 14:33:55 2023, max compression
+gzip compressed data, was "mask2bbox-0.0.9.tar", last modified: Tue Jun 20 15:52:21 2023, max compression
```

## Comparing `mask2bbox-0.0.8.tar` & `mask2bbox-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.585099 mask2bbox-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-20 14:33:55.585099 mask2bbox-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:33:55.585099 mask2bbox-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.577099 mask2bbox-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.581099 mask2bbox-0.0.8/src/mask2bbox/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/src/mask2bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17797 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/src/mask2bbox/_bboxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/src/mask2bbox/mask2bbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.581099 mask2bbox-0.0.8/src/mask2bbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-06-20 14:33:55.000000 mask2bbox-0.0.8/src/mask2bbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 14:33:55.000000 mask2bbox-0.0.8/src/mask2bbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:33:55.000000 mask2bbox-0.0.8/src/mask2bbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 14:33:55.000000 mask2bbox-0.0.8/src/mask2bbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 14:33:55.000000 mask2bbox-0.0.8/src/mask2bbox.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.581099 mask2bbox-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:55.585099 mask2bbox-0.0.8/tests/test_mask2bbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/tests/test_mask2bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 14:33:42.000000 mask2bbox-0.0.8/tests/test_mask2bbox/test_mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:52:21.292110 mask2bbox-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-20 15:52:11.000000 mask2bbox-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-20 15:52:11.000000 mask2bbox-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-20 15:52:21.292110 mask2bbox-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-20 15:52:11.000000 mask2bbox-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:52:21.292110 mask2bbox-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-20 15:52:11.000000 mask2bbox-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:52:21.288110 mask2bbox-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:52:21.292110 mask2bbox-0.0.9/src/mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 15:52:11.000000 mask2bbox-0.0.9/src/mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17743 2023-06-20 15:52:11.000000 mask2bbox-0.0.9/src/mask2bbox/_bboxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-06-20 15:52:11.000000 mask2bbox-0.0.9/src/mask2bbox/mask2bbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:52:21.292110 mask2bbox-0.0.9/src/mask2bbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-06-20 15:52:21.000000 mask2bbox-0.0.9/src/mask2bbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 15:52:21.000000 mask2bbox-0.0.9/src/mask2bbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:52:21.000000 mask2bbox-0.0.9/src/mask2bbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 15:52:21.000000 mask2bbox-0.0.9/src/mask2bbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 15:52:21.000000 mask2bbox-0.0.9/src/mask2bbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:52:21.292110 mask2bbox-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:52:11.000000 mask2bbox-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:52:21.292110 mask2bbox-0.0.9/tests/test_mask2bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 15:52:11.000000 mask2bbox-0.0.9/tests/test_mask2bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-20 15:52:11.000000 mask2bbox-0.0.9/tests/test_mask2bbox/test_mask2bbox.py
```

### Comparing `mask2bbox-0.0.8/LICENSE.txt` & `mask2bbox-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.8/PKG-INFO` & `mask2bbox-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask2bbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Gets the bounding boxes from a mask file.
 Home-page: https://github.com/SchapiroLabor/mask2bbox
 Author: Miguel Ibarra
 Author-email: c180l058j@mozmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -61,14 +61,16 @@
 resize_factors = filtered_boxes.de(desired_ratio=0.7, size=(256, 256))
 
 # Extract the bounding boxes as images
 filtered_boxes.extract(resize_factors, size=(256, 256), output="path/to/save/images")
 ```
 
 ## Version Notes
+### 0.0.9 - Fix bug in `BBoxes.extract()`
+- Fix bug in `BBoxes.extract()` that caused the images to be saved with the wrong name amd created a new folder.
 
 ### 0.0.8 - Change methods, change constructor, added functionality. 
 - **Constructor:** BBox object is now constructed with the syntax `BBoxes.from_mask(mask)` instead of `BBoxes(mask)`.
 - **Operations:** BBox object operations are no longer performed in place, the affected methods are:
   - `BBoxes.remove_from_edge()`
   - `BBoxes.expand()`
   - `BBoxes.filter()`
```

### Comparing `mask2bbox-0.0.8/README.md` & `mask2bbox-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 resize_factors = filtered_boxes.de(desired_ratio=0.7, size=(256, 256))
 
 # Extract the bounding boxes as images
 filtered_boxes.extract(resize_factors, size=(256, 256), output="path/to/save/images")
 ```
 
 ## Version Notes
+### 0.0.9 - Fix bug in `BBoxes.extract()`
+- Fix bug in `BBoxes.extract()` that caused the images to be saved with the wrong name amd created a new folder.
 
 ### 0.0.8 - Change methods, change constructor, added functionality. 
 - **Constructor:** BBox object is now constructed with the syntax `BBoxes.from_mask(mask)` instead of `BBoxes(mask)`.
 - **Operations:** BBox object operations are no longer performed in place, the affected methods are:
   - `BBoxes.remove_from_edge()`
   - `BBoxes.expand()`
   - `BBoxes.filter()`
```

### Comparing `mask2bbox-0.0.8/setup.py` & `mask2bbox-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mask2bbox",
-    version="0.0.8",
+    version="0.0.9",
     description="Gets the bounding boxes from a mask file.",
     url="https://github.com/SchapiroLabor/mask2bbox",
     author="Miguel Ibarra",
     author_email="c180l058j@mozmail.com",
     license="MIT",
     classifiers=[
         "Development Status :: 3 - Alpha",
```

### Comparing `mask2bbox-0.0.8/src/mask2bbox/_bboxes.py` & `mask2bbox-0.0.9/src/mask2bbox/_bboxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,15 +448,14 @@
         for ds, (k, x1, x2, y1, y2) in zip(resize_factors, self.bboxes):
             sc = self.image[x1:x2, y1:y2]
             sc = transform.rescale(sc, ds, anti_aliasing=True)
             sc = self._pad_crop(sc, size)
             sc = exposure.rescale_intensity(sc, out_range=(0, 255)).astype(np.uint8)
 
             # Save the sc image
-            output.mkdir(parents=True, exist_ok=True)
             io.imsave(f"{output}_{k}.png", sc)
 
     # Saving
     def save_iou(self,
                  output_file: str) -> None:
         """
         Saves the IoU matrix to a csv file.
```

### Comparing `mask2bbox-0.0.8/src/mask2bbox/mask2bbox.py` & `mask2bbox-0.0.9/src/mask2bbox/mask2bbox.py`

 * *Files identical despite different names*

### Comparing `mask2bbox-0.0.8/src/mask2bbox.egg-info/PKG-INFO` & `mask2bbox-0.0.9/src/mask2bbox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask2bbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Gets the bounding boxes from a mask file.
 Home-page: https://github.com/SchapiroLabor/mask2bbox
 Author: Miguel Ibarra
 Author-email: c180l058j@mozmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -61,14 +61,16 @@
 resize_factors = filtered_boxes.de(desired_ratio=0.7, size=(256, 256))
 
 # Extract the bounding boxes as images
 filtered_boxes.extract(resize_factors, size=(256, 256), output="path/to/save/images")
 ```
 
 ## Version Notes
+### 0.0.9 - Fix bug in `BBoxes.extract()`
+- Fix bug in `BBoxes.extract()` that caused the images to be saved with the wrong name amd created a new folder.
 
 ### 0.0.8 - Change methods, change constructor, added functionality. 
 - **Constructor:** BBox object is now constructed with the syntax `BBoxes.from_mask(mask)` instead of `BBoxes(mask)`.
 - **Operations:** BBox object operations are no longer performed in place, the affected methods are:
   - `BBoxes.remove_from_edge()`
   - `BBoxes.expand()`
   - `BBoxes.filter()`
```

