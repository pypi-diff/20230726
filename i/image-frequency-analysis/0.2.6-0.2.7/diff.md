# Comparing `tmp/image_frequency_analysis-0.2.6.tar.gz` & `tmp/image_frequency_analysis-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_frequency_analysis-0.2.6.tar", max compression
+gzip compressed data, was "image_frequency_analysis-0.2.7.tar", max compression
```

## Comparing `image_frequency_analysis-0.2.6.tar` & `image_frequency_analysis-0.2.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-07-26 15:56:18.113658 image_frequency_analysis-0.2.6/LICENSE
--rw-r--r--   0        0        0     2006 2023-07-26 15:56:18.113658 image_frequency_analysis-0.2.6/README.md
--rw-r--r--   0        0        0       87 2023-07-26 15:56:18.113658 image_frequency_analysis-0.2.6/image_frequency_analysis/__init__.py
--rw-r--r--   0        0        0     6523 2023-07-26 15:56:18.113658 image_frequency_analysis-0.2.6/image_frequency_analysis/frequency_analysis.py
--rw-r--r--   0        0        0      890 2023-07-26 15:56:18.113658 image_frequency_analysis-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2943 1970-01-01 00:00:00.000000 image_frequency_analysis-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-26 16:16:35.636685 image_frequency_analysis-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2061 2023-07-26 16:16:35.636685 image_frequency_analysis-0.2.7/README.md
+-rw-r--r--   0        0        0       87 2023-07-26 16:16:35.636685 image_frequency_analysis-0.2.7/image_frequency_analysis/__init__.py
+-rw-r--r--   0        0        0     6523 2023-07-26 16:16:35.636685 image_frequency_analysis-0.2.7/image_frequency_analysis/frequency_analysis.py
+-rw-r--r--   0        0        0      891 2023-07-26 16:16:35.636685 image_frequency_analysis-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2998 1970-01-01 00:00:00.000000 image_frequency_analysis-0.2.7/PKG-INFO
```

### Comparing `image_frequency_analysis-0.2.6/LICENSE` & `image_frequency_analysis-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `image_frequency_analysis-0.2.6/README.md` & `image_frequency_analysis-0.2.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 ` import image_frequency_analysis as ifa `
 
 You can then pass the image path to the function which is a required argument, to get the plot 
 of comparison between the original image and the filtered image
 
 **Example:**
 
-` ifa.FrequencyAnalysis('sandstone.tif') `
+`obj = ifa.FrequencyAnalysis('car_image.jpg')`
+
+`output = obj.perform_image_frequency_analysis()`
 
 By default the package uses the high pass filter to perform the filtering of the image. This option can be overridden using
 the optional parameters that can be sent to the function.
 
 You can find the various optional parameters and their usage in the package using the help command.
 
 ` help(ifa.FrequencyAnalysis) ` or looking through the docstring directly in the IDE
```

### Comparing `image_frequency_analysis-0.2.6/image_frequency_analysis/frequency_analysis.py` & `image_frequency_analysis-0.2.7/image_frequency_analysis/frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `image_frequency_analysis-0.2.6/pyproject.toml` & `image_frequency_analysis-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image_frequency_analysis"
-version = "0.2.6"
+version = "0.2.7"
 description = "A package to perform image frequency analysis using the Fourier Transform method"
 authors = ["M Thivagar"]
 readme = "README.md"
 homepage = "https://github.com/thivagar-manickam/image_frequency_analysis"
 repository = "https://github.com/thivagar-manickam/image_frequency_analysis"
 license = "MIT"
 classifiers = [
@@ -21,8 +21,8 @@
 opencv-python = ">=4.5.1.48"
 numpy = ">=1.21.4"
 pandas = ">=1.3.5"
 matplotlib = ">=3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `image_frequency_analysis-0.2.6/PKG-INFO` & `image_frequency_analysis-0.2.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-frequency-analysis
-Version: 0.2.6
+Version: 0.2.7
 Summary: A package to perform image frequency analysis using the Fourier Transform method
 Home-page: https://github.com/thivagar-manickam/image_frequency_analysis
 License: MIT
 Keywords: Image Processing,Fourier Transform,Edge Detection,Frequency analysis
 Author: M Thivagar
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -50,15 +50,17 @@
 ` import image_frequency_analysis as ifa `
 
 You can then pass the image path to the function which is a required argument, to get the plot 
 of comparison between the original image and the filtered image
 
 **Example:**
 
-` ifa.FrequencyAnalysis('sandstone.tif') `
+`obj = ifa.FrequencyAnalysis('car_image.jpg')`
+
+`output = obj.perform_image_frequency_analysis()`
 
 By default the package uses the high pass filter to perform the filtering of the image. This option can be overridden using
 the optional parameters that can be sent to the function.
 
 You can find the various optional parameters and their usage in the package using the help command.
 
 ` help(ifa.FrequencyAnalysis) ` or looking through the docstring directly in the IDE
```

