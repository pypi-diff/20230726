# Comparing `tmp/image_frequency_analysis-0.2.5.tar.gz` & `tmp/image_frequency_analysis-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_frequency_analysis-0.2.5.tar", max compression
+gzip compressed data, was "image_frequency_analysis-0.2.6.tar", max compression
```

## Comparing `image_frequency_analysis-0.2.5.tar` & `image_frequency_analysis-0.2.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-06-04 11:25:19.929417 image_frequency_analysis-0.2.5/LICENSE
--rw-r--r--   0        0        0     1854 2023-06-04 11:25:19.929417 image_frequency_analysis-0.2.5/README.md
--rw-r--r--   0        0        0       87 2023-06-04 11:25:19.929417 image_frequency_analysis-0.2.5/image_frequency_analysis/__init__.py
--rw-r--r--   0        0        0     6317 2023-06-04 11:25:19.929417 image_frequency_analysis-0.2.5/image_frequency_analysis/frequency_analysis.py
--rw-r--r--   0        0        0      890 2023-06-04 11:25:19.929417 image_frequency_analysis-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 image_frequency_analysis-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-26 15:56:18.113658 image_frequency_analysis-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2006 2023-07-26 15:56:18.113658 image_frequency_analysis-0.2.6/README.md
+-rw-r--r--   0        0        0       87 2023-07-26 15:56:18.113658 image_frequency_analysis-0.2.6/image_frequency_analysis/__init__.py
+-rw-r--r--   0        0        0     6523 2023-07-26 15:56:18.113658 image_frequency_analysis-0.2.6/image_frequency_analysis/frequency_analysis.py
+-rw-r--r--   0        0        0      890 2023-07-26 15:56:18.113658 image_frequency_analysis-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2943 1970-01-01 00:00:00.000000 image_frequency_analysis-0.2.6/PKG-INFO
```

### Comparing `image_frequency_analysis-0.2.5/LICENSE` & `image_frequency_analysis-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `image_frequency_analysis-0.2.5/README.md` & `image_frequency_analysis-0.2.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 <div align="center">
 
 <h1> Image Frequency Analysis </h1>
   
 [![PyPI version](https://badge.fury.io/py/image-frequency-analysis.svg)](https://pypi.org/project/image-frequency-analysis/)
 [![PyPI stats](https://img.shields.io/pypi/dm/image-frequency-analysis.svg)](https://pypistats.org/packages/image-frequency-analysis)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/thivagar-manickam/image-frequency-analysis/blob/main/LICENSE)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/image-frequency-analysis.svg)](https://pypi.org/project/image-frequency-analysis/)
 
 </div>
 
 This package is build to combine all the steps that are done as part of the
 frequency analysis using the Fourier transform approach.
```

### Comparing `image_frequency_analysis-0.2.5/image_frequency_analysis/frequency_analysis.py` & `image_frequency_analysis-0.2.6/image_frequency_analysis/frequency_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,96 +42,94 @@
         self.row_center = None
         self.rows = None
         self.columns = None
         self.image_path = image_path
         self.radius = filter_radius
         self.high_pass_filter = high_pass_filter
         self.low_pass_filter = low_pass_filter
-        self.image = self.load_image(self.image_path)
-
-        self.perform_image_frequency_analysis()
+        self.image = self.__load_image(self.image_path)
 
     """
     Definition to load the image into the
     image object which will be used for further
     processing
     """
 
-    def load_image(self, image_path):
+    def __load_image(self, image_path):
         if os.path.exists(self.image_path):
             return cv2.imread(f"{image_path}", 0)
         else:
             raise FileNotFoundError(f"File not found: {image_path}")
 
     """
     Definition to find the discrete fourier
     transform value for the given image
     """
 
-    def calculate_dft_of_image(self):
+    def __calculate_dft_of_image(self):
         self.dft_image = cv2.dft(np.float32(self.image), flags=cv2.DFT_COMPLEX_OUTPUT)
 
     """
     Definition to perform the frequency shifting
     inorder to migrate the low frequency values to 
     the center and the high frequency values to the 
     edges
     """
 
-    def perform_frequency_shifting(self):
+    def __perform_frequency_shifting(self):
         self.fft_image = np.fft.fftshift(self.dft_image)
 
     """
     To visualize the frequency shifted value
     of the image
     """
 
-    def get_magnitude_spectrum(self):
+    def __get_magnitude_spectrum(self):
         return 20 * np.log(
             cv2.magnitude(self.fft_image[:, :, 0], self.fft_image[:, :, 1])
         )
 
     """
     To get the rows and column information about the
     image matrix
     """
 
-    def set_rows_columns_details(self):
+    def __set_rows_columns_details(self):
         self.rows, self.columns = self.image.shape
 
         self.row_center, self.column_center = int(self.rows / 2), int(self.columns / 2)
 
     """
     To get the high pass filter mask
     """
 
-    def get_high_pass_filter_mask_matrix(self):
+    def __get_high_pass_filter_mask_matrix(self):
         return np.ones((self.rows, self.columns, 2), np.uint8)
 
     """
     To get the low pass filter mask
     """
 
-    def get_low_pass_filter_mask_matrix(self):
+    def __get_low_pass_filter_mask_matrix(self):
         return np.zeros((self.rows, self.columns, 2), np.uint8)
 
     """
     To calculate the mask area based on the 
     the rows and column information of the image
     """
 
-    def calculate_mask_area(self):
+    def __calculate_mask_area(self):
         center = [self.row_center, self.column_center]
         x_value, y_value = np.ogrid[: self.rows, : self.columns]
 
         self.mask_area = (x_value - center[0]) ** 2 + (y_value - center[1]) ** 2 <= (
             self.radius * self.radius
         )
 
-    def plot_graph(self, frequency_shift_magnitude, image):
+    def __plot_graph(self, frequency_shift_magnitude, image):
         plt.figure(figsize=(20, 10))
 
         plt.subplot(1, 3, 1)
         plt.title("Original Image")
         plt.imshow(self.image, cmap="gray")
 
         plt.subplot(1, 3, 2)
@@ -139,65 +137,70 @@
         plt.imshow(frequency_shift_magnitude, cmap="gray")
 
         plt.subplot(1, 3, 3)
         filter_type = "Low Pass filter" if self.low_pass_filter else "High Pass Filter"
         plt.title(f"Image post applying the {filter_type} mask")
         plt.imshow(image, cmap="gray")
 
-    def perform_filtering_and_inverse_transform(self, mask):
+    def __perform_filtering_and_inverse_transform(self, mask):
         frequency_shift = self.fft_image * mask
 
         frequency_mask_magnitude = 20 * np.log(
             cv2.magnitude(frequency_shift[:, :, 0], frequency_shift[:, :, 1]) + 1
         )
 
         frequency_shift_inverse = np.fft.ifftshift(frequency_shift)
 
         inverse_discrete_transform = cv2.idft(frequency_shift_inverse)
 
         original_image = cv2.magnitude(
             inverse_discrete_transform[:, :, 0], inverse_discrete_transform[:, :, 1]
         )
 
-        self.plot_graph(frequency_mask_magnitude, original_image)
+        self.__plot_graph(frequency_mask_magnitude, original_image)
 
         return original_image
 
-    def perform_high_pass_filter_analysis(self):
-        hpf_mask = self.get_high_pass_filter_mask_matrix()
+    def __perform_high_pass_filter_analysis(self):
+        hpf_mask = self.__get_high_pass_filter_mask_matrix()
         hpf_mask[self.mask_area] = 0
 
-        return self.perform_filtering_and_inverse_transform(hpf_mask)
+        return self.__perform_filtering_and_inverse_transform(hpf_mask)
 
-    def perform_low_pass_filter_analysis(self):
-        lpf_mask = self.get_low_pass_filter_mask_matrix()
+    def __perform_low_pass_filter_analysis(self):
+        lpf_mask = self.__get_low_pass_filter_mask_matrix()
         lpf_mask[self.mask_area] = 1
 
-        return self.perform_filtering_and_inverse_transform(lpf_mask)
+        return self.__perform_filtering_and_inverse_transform(lpf_mask)
 
-    def perform_image_frequency_analysis(self):
+    def perform_image_frequency_analysis(self) -> np.ndarray:
+        """
+        Definition to initiate the Fourier Transformation
+        on the specified Image
+        Returns: numpy.ndarray - returns the transformed image as a numpy array
+        """
         if self.high_pass_filter and self.low_pass_filter:
             raise ValueError(
                         "Both high_pass_filter and low_pass_filter flag cannot be True. Please choose only one type "
                         "of filter"
                     )
 
         if not self.high_pass_filter and not self.low_pass_filter:
             self.high_pass_filter = True
 
-        self.calculate_dft_of_image()
+        self.__calculate_dft_of_image()
 
-        self.perform_frequency_shifting()
+        self.__perform_frequency_shifting()
 
-        self.set_rows_columns_details()
+        self.__set_rows_columns_details()
 
-        self.calculate_mask_area()
+        self.__calculate_mask_area()
 
         if self.high_pass_filter:
-            final_image = self.perform_high_pass_filter_analysis()
+            final_image = self.__perform_high_pass_filter_analysis()
         else:
-            final_image = self.perform_low_pass_filter_analysis()
+            final_image = self.__perform_low_pass_filter_analysis()
 
-        final_image = (final_image / final_image.max() * 255).astype("uint8")
+        final_image = (final_image / final_image.max() * 255).astype('uint8')
 
         return final_image
```

### Comparing `image_frequency_analysis-0.2.5/pyproject.toml` & `image_frequency_analysis-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "image_frequency_analysis"
-version = "0.2.5"
+version = "0.2.6"
 description = "A package to perform image frequency analysis using the Fourier Transform method"
 authors = ["M Thivagar"]
 readme = "README.md"
 homepage = "https://github.com/thivagar-manickam/image_frequency_analysis"
 repository = "https://github.com/thivagar-manickam/image_frequency_analysis"
 license = "MIT"
 classifiers = [
```

### Comparing `image_frequency_analysis-0.2.5/PKG-INFO` & `image_frequency_analysis-0.2.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-frequency-analysis
-Version: 0.2.5
+Version: 0.2.6
 Summary: A package to perform image frequency analysis using the Fourier Transform method
 Home-page: https://github.com/thivagar-manickam/image_frequency_analysis
 License: MIT
 Keywords: Image Processing,Fourier Transform,Edge Detection,Frequency analysis
 Author: M Thivagar
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -22,14 +22,15 @@
 
 <div align="center">
 
 <h1> Image Frequency Analysis </h1>
   
 [![PyPI version](https://badge.fury.io/py/image-frequency-analysis.svg)](https://pypi.org/project/image-frequency-analysis/)
 [![PyPI stats](https://img.shields.io/pypi/dm/image-frequency-analysis.svg)](https://pypistats.org/packages/image-frequency-analysis)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/thivagar-manickam/image-frequency-analysis/blob/main/LICENSE)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/image-frequency-analysis.svg)](https://pypi.org/project/image-frequency-analysis/)
 
 </div>
 
 This package is build to combine all the steps that are done as part of the
 frequency analysis using the Fourier transform approach.
```

