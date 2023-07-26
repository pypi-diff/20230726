# Comparing `tmp/glint_mask_tools-3.0.4.tar.gz` & `tmp/glint_mask_tools-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glint_mask_tools-3.0.4.tar", max compression
+gzip compressed data, was "glint_mask_tools-3.1.0.tar", max compression
```

## Comparing `glint_mask_tools-3.0.4.tar` & `glint_mask_tools-3.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/LICENSE
--rw-r--r--   0        0        0     7911 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/README.md
--rw-r--r--   0        0        0      369 2023-07-11 18:05:47.211939 glint_mask_tools-3.0.4/glint_mask_generator/__init__.py
--rw-r--r--   0        0        0     5914 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/glint_mask_generator/cli.py
--rw-r--r--   0        0        0     3770 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/glint_mask_generator/glint_algorithms.py
--rw-r--r--   0        0        0     7208 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/glint_mask_generator/image_loaders.py
--rw-r--r--   0        0        0     6647 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/glint_mask_generator/maskers.py
--rw-r--r--   0        0        0     1510 2023-07-11 18:04:46.726947 glint_mask_tools-3.0.4/glint_mask_generator/utils.py
--rw-r--r--   0        0        0      794 2023-07-11 18:05:47.171938 glint_mask_tools-3.0.4/pyproject.toml
--rw-r--r--   0        0        0     9132 1970-01-01 00:00:00.000000 glint_mask_tools-3.0.4/setup.py
--rw-r--r--   0        0        0     8806 1970-01-01 00:00:00.000000 glint_mask_tools-3.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-26 20:22:18.498166 glint_mask_tools-3.1.0/LICENSE
+-rw-r--r--   0        0        0     7896 2023-07-26 20:22:18.498166 glint_mask_tools-3.1.0/README.md
+-rw-r--r--   0        0        0      400 2023-07-26 20:24:46.465222 glint_mask_tools-3.1.0/glint_mask_generator/__init__.py
+-rw-r--r--   0        0        0     6255 2023-07-26 20:22:18.498166 glint_mask_tools-3.1.0/glint_mask_generator/cli.py
+-rw-r--r--   0        0        0     3738 2023-07-26 20:22:18.498166 glint_mask_tools-3.1.0/glint_mask_generator/glint_algorithms.py
+-rw-r--r--   0        0        0     7643 2023-07-26 20:22:18.498166 glint_mask_tools-3.1.0/glint_mask_generator/image_loaders.py
+-rw-r--r--   0        0        0     6891 2023-07-26 20:22:18.498166 glint_mask_tools-3.1.0/glint_mask_generator/maskers.py
+-rw-r--r--   0        0        0     1488 2023-07-26 20:22:18.498166 glint_mask_tools-3.1.0/glint_mask_generator/utils.py
+-rw-r--r--   0        0        0      843 2023-07-26 20:24:46.365220 glint_mask_tools-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     9116 1970-01-01 00:00:00.000000 glint_mask_tools-3.1.0/setup.py
+-rw-r--r--   0        0        0     8841 1970-01-01 00:00:00.000000 glint_mask_tools-3.1.0/PKG-INFO
```

### Comparing `glint_mask_tools-3.0.4/LICENSE` & `glint_mask_tools-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glint_mask_tools-3.0.4/README.md` & `glint_mask_tools-3.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -59,82 +59,82 @@
 #### Examples
 
 ```bash
 glint-mask-v*.*.* --help
 
 # NAME
 #     glint-mask-v*.*.*
-# 
+#
 # SYNOPSIS
 #     glint-mask-v*.*.* - COMMAND | VALUE
-# 
+#
 # COMMANDS
 #     COMMAND is one of the following:
-# 
+#
 #      cir_threshold
 #        Generate masks for glint regions in 4 Band CIR imagery using Tom Bell's binning algorithm.
-# 
+#
 #      micasense_threshold
 #        Generate masks for glint regions in multispectral imagery from the Micasense camera using Tom Bell's algorithm on the blue image band.
-# 
+#
 #      p4ms_threshold
 #        Generate masks for glint regions in multispectral imagery from the DJI camera using Tom Bell's algorithm on the Blue image band.
-# 
+#
 #      process
-# 
+#
 #      rgb_threshold
 #        Generate masks for glint regions in RGB imagery using Tom Bell's binning algorithm.
-# 
+#
 # VALUES
 #     VALUE is one of the following:
-# 
+#
 #      max_workers
 #        The maximum number of threads to use for processing.
 ```
 
 ```bash
 # Get addition parameters for one of the cameras/methods available
 glint-mask-v*.*.* rgb_threshold --help
 
 # NAME
 #     glint-mask-v*.*.* rgb_threshold - Generate masks for glint regions in RGB imagery using Tom Bell's binning algorithm.
-# 
+#
 # SYNOPSIS
 #     glint-mask-v*.*.* rgb_threshold IMG_DIR OUT_DIR <flags>
-# 
+#
 # DESCRIPTION
 #     Generate masks for glint regions in RGB imagery using Tom Bell's binning algorithm.
-# 
+#
 # POSITIONAL ARGUMENTS
 #     IMG_DIR
 #         The path to a named input image or directory containing images. If img_dir is a directory, all tif, jpg, jpeg, and png images in that directory will be # processed.
 #     OUT_DIR
 #         The path to send your out image including the file name and type. e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is specified as a # # # directory.
-# 
+#
 # FLAGS
 #     --thresholds=THRESHOLDS
 #         The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [1, 1, 0.875].
 #     --pixel_buffer=PIXEL_BUFFER
 #         The pixel distance to buffer out the mask. Defaults to 0 (off).
-# 
+#
 # NOTES
 #     You can also use flags syntax for POSITIONAL ARGUMENTS
 ```
 
 ```bash
 # Process rgb imagery directory with default parameters
 glint-mask-v*.*.* rgb_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/
 
 # Process PhaseONE camera imagery with image bands split over multiple files
 glint-mask-v*.*.* aco_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/
 
 # Process DJI P4MS imagery
 glint-mask-v*.*.* p4ms_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/
 
-# Process Micasense RedEdge imagery 
+# Process Micasense RedEdge imagery
 glint-mask-v*.*.* micasense_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/
 ```
 
 ### Python package
 Installing the PyPi package allows integrating the mask generation workflow into existing python scripts with ease.
 
 ```python
```

### Comparing `glint_mask_tools-3.0.4/glint_mask_generator/cli.py` & `glint_mask_tools-3.1.0/glint_mask_generator/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,19 +7,25 @@
 import os
 import sys
 from typing import List
 
 import fire
 from tqdm import tqdm
 
-from .maskers import Masker, MicasenseRedEdgeThresholdMasker, P4MSThresholdMasker, RGBThresholdMasker, CIRThresholdMasker
+from .maskers import (
+    Masker,
+    MicasenseRedEdgeThresholdMasker,
+    P4MSThresholdMasker,
+    RGBThresholdMasker,
+    CIRThresholdMasker,
+)
 
 
 class CLI(object):
-    def __init__(self, max_workers: int = os.cpu_count()):
+    def __init__(self, max_workers: int = min(4, os.cpu_count())):
         """Command Line Interface Class for glint mask generators.
 
         Parameters
         ----------
         max_workers
             The maximum number of threads to use for processing.
         """
@@ -27,116 +33,154 @@
 
     @staticmethod
     def _err_callback(path, exception):
         tqdm.write(f"{path} failed with err:\n{exception}", file=sys.stderr)
 
     def _process(self, masker: Masker):
         with tqdm(total=len(masker)) as progress:
-            masker(max_workers=self.max_workers,
-                   callback=lambda _: progress.update(1),
-                   err_callback=self._err_callback)
-
-    def rgb_threshold(self, img_dir: str, out_dir: str, thresholds: List[float] = (1, 1, 0.875),
-                      pixel_buffer: int = 0) -> None:
-        """Generate masks for glint regions in RGB imagery using Tom Bell's binning algorithm.
+            masker(
+                max_workers=self.max_workers,
+                callback=lambda _: progress.update(1),
+                err_callback=self._err_callback,
+            )
+
+    def rgb_threshold(
+        self,
+        img_dir: str,
+        out_dir: str,
+        thresholds: List[float] = (1, 1, 0.875),
+        pixel_buffer: int = 0,
+    ) -> None:
+        """Generate masks for glint regions in RGB imagery using Tom Bell's binning
+            algorithm.
 
         Parameters
         ----------
         img_dir
-            The path to a named input image or directory containing images. If img_dir is a directory, all tif, jpg, jpeg,
-            and png images in that directory will be processed.
+            The path to a named input image or directory containing images. If img_dir
+            is a directory, all tif, jpg, jpeg, and png images in that directory will
+            be processed.
         out_dir
-            The path to send your out image including the file name and type. e.g. "/path/to/mask.png".
-            out_dir must be a directory if img_dir is specified as a directory.
+            The path to send your out image including the file name and type.
+            e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is
+            specified as a directory.
         thresholds
-            The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [1, 1, 0.875].
+            The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0).
+            Default is [1, 1, 0.875].
         pixel_buffer
             The pixel distance to buffer out the mask. Defaults to 0 (off).
 
         Returns
         -------
         None
             Side effects are that the mask is saved to the specified out_dir location.
         """
         self._process(RGBThresholdMasker(img_dir, out_dir, thresholds, pixel_buffer))
 
-    def cir_threshold(self, img_dir: str, out_dir: str, thresholds: List[float] = (1, 1, 0.875, 1),
-                      pixel_buffer: int = 0) -> None:
-        """Generate masks for glint regions in 4 Band CIR imagery using Tom Bell's binning algorithm.
+    def cir_threshold(
+        self,
+        img_dir: str,
+        out_dir: str,
+        thresholds: List[float] = (1, 1, 0.875, 1),
+        pixel_buffer: int = 0,
+    ) -> None:
+        """Generate masks for glint regions in 4 Band CIR imagery using Tom Bell's
+            binning algorithm.
 
         Parameters
         ----------
         img_dir
-            The path to a named input image or directory containing images. If img_dir is a directory, all tif, jpg, jpeg,
-            and png images in that directory will be processed.
+            The path to a named input image or directory containing images. If img_dir
+            is a directory, all tif, jpg, jpeg, and png images in that directory will
+            be processed.
         out_dir
-            The path to send your out image including the file name and type. e.g. "/path/to/mask.png".
-            out_dir must be a directory if img_dir is specified as a directory.
+            The path to send your out image including the file name and type.
+            e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is
+            specified as a directory.
         thresholds
-            The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [1, 1, 0.875].
+            The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0).
+            Default is [1, 1, 0.875].
         pixel_buffer
             The pixel distance to buffer out the mask. Defaults to 0 (off).
 
         Returns
         -------
         None
             Side effects are that the mask is saved to the specified out_dir location.
         """
         self._process(CIRThresholdMasker(img_dir, out_dir, thresholds, pixel_buffer))
 
-    def p4ms_threshold(self, img_dir: str, out_dir: str, thresholds: List[float] = (0.875, 1, 1, 1, 1),
-                       pixel_buffer: int = 0) -> None:
-        """Generate masks for glint regions in multispectral imagery from the DJI camera using Tom Bell's algorithm on
-            the Blue image band.
+    def p4ms_threshold(
+        self,
+        img_dir: str,
+        out_dir: str,
+        thresholds: List[float] = (0.875, 1, 1, 1, 1),
+        pixel_buffer: int = 0,
+    ) -> None:
+        """Generate masks for glint regions in multispectral imagery from the DJI camera
+            using Tom Bell's algorithm on the Blue image band.
 
         Parameters
         ----------
         img_dir
-            The path to a named input image or directory containing images. If img_dir is a directory, all tif, jpg, jpeg,
-            and png images in that directory will be processed.
+            The path to a named input image or directory containing images. If img_dir
+            is a directory, all tif, jpg, jpeg, and png images in that directory will
+            be processed.
         out_dir
-            The path to send your out image including the file name and type. e.g. "/path/to/mask.png".
-            out_dir must be a directory if img_dir is specified as a directory.
+            The path to send your out image including the file name and type.
+            e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is
+            specified as a directory.
         thresholds
-            The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [0.875, 1, 1, 1, 1].
+            The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0).
+            Default is [0.875, 1, 1, 1, 1].
         pixel_buffer
             The pixel distance to buffer out the mask. Defaults to 0 (off).
 
         Returns
         -------
         None
             Side effects are that the mask is saved to the specified out_dir location.
         """
         self._process(P4MSThresholdMasker(img_dir, out_dir, thresholds, pixel_buffer))
 
-    def micasense_threshold(self, img_dir: str, out_dir: str, thresholds: List[float] = (0.875, 1, 1, 1, 1),
-                            pixel_buffer: int = 0) -> None:
-        """Generate masks for glint regions in multispectral imagery from the Micasense camera using Tom Bell's
-            algorithm on the blue image band.
+    def micasense_threshold(
+        self,
+        img_dir: str,
+        out_dir: str,
+        thresholds: List[float] = (0.875, 1, 1, 1, 1),
+        pixel_buffer: int = 0,
+    ) -> None:
+        """Generate masks for glint regions in multispectral imagery from the
+            Micasense camera using Tom Bell's algorithm on the blue image band.
 
         Parameters
         ----------
         img_dir
-            The path to a named input image or directory containing images. If img_dir is a directory, all tif, jpg, jpeg,
-            and png images in that directory will be processed.
+            The path to a named input image or directory containing images.
+            If img_dir is a directory, all tif, jpg, jpeg, and png images in that
+            directory will be processed.
         out_dir
-            The path to send your out image including the file name and type. e.g. "/path/to/mask.png".
-            out_dir must be a directory if img_dir is specified as a directory.
+            The path to send your out image including the file name and type.
+            e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is
+            specified as a directory.
         thresholds
-            The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [0.875, 1, 1, 1, 1].
+            The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0).
+            Default is [0.875, 1, 1, 1, 1].
         pixel_buffer
             The pixel distance to buffer out the mask. Defaults to 0 (off).
 
         Returns
         -------
         None
             Side effects are that the mask is saved to the specified out_dir location.
         """
-        self._process(MicasenseRedEdgeThresholdMasker(img_dir, out_dir, thresholds, pixel_buffer))
+        self._process(
+            MicasenseRedEdgeThresholdMasker(img_dir, out_dir, thresholds, pixel_buffer)
+        )
 
 
 def main():
     fire.Fire(CLI)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `glint_mask_tools-3.0.4/glint_mask_generator/glint_algorithms.py` & `glint_mask_tools-3.1.0/glint_mask_generator/glint_algorithms.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 class GlintAlgorithm(ABC):
     def __init__(self):
         super().__init__()
 
     @abstractmethod
     def __call__(self, img: np.ndarray) -> np.ndarray:
-        """Return a boolean glint mask for a given image. Output mask should have 1 for masked, 0 for unmasked."""
+        """Return a boolean glint mask for a given image.
+        Output mask should have 1 for masked, 0 for unmasked.
+        """
         raise NotImplementedError
 
 
 class ThresholdAlgorithm(GlintAlgorithm):
     def __init__(self, thresholds: Sequence[float]):
         super().__init__()
         self.thresholds = thresholds
@@ -34,18 +36,18 @@
 class IntensityRatioAlgorithm(GlintAlgorithm):
     def __init__(self, percent_diffuse: float = 0.95, threshold: float = 0.99):
         """Create and return a glint mask for RGB imagery.
 
         Parameters
         ----------
         percent_diffuse
-            An estimate of the percentage of pixels in an image that show pure diffuse reflectance, and thus no specular
-            reflectance (glint).
+            An estimate of the percentage of pixels in an image that show pure diffuse
+            reflectance, and thus no specular reflectance (glint).
         threshold
-            The threshold on the specular reflectance estimate image to convert into a mask.
+            Threshold on specular reflectance estimate to binarize into a mask.
             e.g. if more than 50% specular reflectance is unacceptable, use 0.5.
         """
         super().__init__()
         self.percent_diffuse = percent_diffuse
         self.threshold = threshold
 
     def __call__(self, img: np.ndarray) -> np.ndarray:
@@ -57,50 +59,55 @@
             Path to a 3-channel RGB numpy image normalized to values in [0,1].
 
         Returns
         -------
         numpy.ndarray, shape=(H,W)
             Numpy array of glint mask for img at input_path.
         """
-        return self._estimate_specular_reflection_component(img, self.percent_diffuse) > self.threshold
+        return (
+            self._estimate_specular_reflection_component(img, self.percent_diffuse)
+            > self.threshold
+        )
 
     @staticmethod
-    def _estimate_specular_reflection_component(img: np.ndarray, percent_diffuse: float) -> np.ndarray:
+    def _estimate_specular_reflection_component(
+        img: np.ndarray, percent_diffuse: float
+    ) -> np.ndarray:
         """Estimate the specular reflection component of pixels in an image.
 
-            Based on method from:
-                Wang, S., Yu, C., Sun, Y. et al. Specular reflection removal
-                of ocean surface remote sensing images from UAVs. Multimedia Tools
-                Appl 77, 11363–11379 (2018). https://doi.org/10.1007/s11042-017-5551-7
-
-            Parameters
-            ----------
-            img: numpy.ndarray, shape=(H,W,C)
-                A numpy ndarray of an RGB image.
-            percent_diffuse
-                An estimate of the % of pixels that show purely diffuse reflection.
-
-            Returns
-            -------
-            numpy.ndarray, shape=(H,W)
-                An 1D image where values are an estimate of the component of specular reflectance.
-            """
+        Based on method from:
+            Wang, S., Yu, C., Sun, Y. et al. Specular reflection removal
+            of ocean surface remote sensing images from UAVs. Multimedia Tools
+            Appl 77, 11363–11379 (2018). https://doi.org/10.1007/s11042-017-5551-7
+
+        Parameters
+        ----------
+        img: numpy.ndarray, shape=(H,W,C)
+            A numpy ndarray of an RGB image.
+        percent_diffuse
+            An estimate of the % of pixels that show purely diffuse reflection.
+
+        Returns
+        -------
+        numpy.ndarray, shape=(H,W)
+            1D image with values being an estimate of specular reflectance.
+        """
         # Calculate the pixel-wise max intensity and intensity range over RGB channels
         i_max = np.amax(img, axis=2)
         i_min = np.amin(img, axis=2)
         i_range = i_max - i_min
 
         # Calculate intensity ratio
         q = np.divide(i_max, i_range + EPSILON)
 
         # Select diffuse only pixels using the PERCENTILE_THRESH
         # i.e. A percentage of PERCENTILE_THRESH pixels are supposed to have no
         #     specular reflection
         num_thresh = math.ceil(percent_diffuse * q.size)
 
-        # Get intensity ratio for a pixel dividing the image into diffuse and specular sections
+        # Get intensity ratio by separating the image into diffuse and specular sections
         q_x_hat = np.partition(q.ravel(), num_thresh)[num_thresh]
 
         # Estimate the spectral component of each pixel
         spec_ref_est = np.clip(i_max - (q_x_hat * i_range), 0, None)
 
         return spec_ref_est
```

### Comparing `glint_mask_tools-3.0.4/glint_mask_generator/image_loaders.py` & `glint_mask_tools-3.1.0/glint_mask_generator/image_loaders.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,26 +3,31 @@
 Organization: Hakai Institute
 Date: 2020-09-18
 """
 import re
 from abc import ABC, ABCMeta, abstractmethod
 from functools import singledispatchmethod
 from pathlib import Path
-from typing import Iterable, List, Union
+from typing import Iterable, List, Union, TYPE_CHECKING
 
 import numpy as np
 from PIL import Image
 
 from .utils import list_images, normalize_img
 
+if TYPE_CHECKING:
+    from .maskers import Masker
+
 Image.MAX_IMAGE_PIXELS = None
 
 
 class ImageLoader(ABC):
-    def __init__(self, image_directory: str, mask_directory: str):
+    def __init__(
+        self, image_directory: Union[str, Path], mask_directory: Union[str, Path]
+    ):
         super().__init__()
         self.image_directory = Path(image_directory)
         self.mask_directory = Path(mask_directory)
 
     def __len__(self):
         return sum(1 for _ in self.paths)
 
@@ -34,16 +39,16 @@
     @property
     @abstractmethod
     def paths(self) -> Iterable[Union[List[str], str]]:
         raise NotImplementedError
 
     @property
     @abstractmethod
-    def _bit_depth(self):
-        return NotImplementedError
+    def _bit_depth(self) -> int:
+        raise NotImplementedError
 
     def preprocess_image(self, img: np.ndarray) -> np.ndarray:
         return normalize_img(img, bit_depth=self._bit_depth)
 
     @singledispatchmethod
     def get_mask_save_paths(self, img_paths: List[str]) -> Iterable[str]:
         img_names = (Path(p).stem for p in img_paths)
@@ -60,149 +65,169 @@
         Parameters
         ----------
         mask
             2D image mask to save into the image format specified in the out_path.
         out_path
             The path where the file should be saved, including img extension.
         """
-        mask_img = Image.fromarray(mask, mode='L')
+        mask_img = Image.fromarray(mask, mode="L")
         mask_img.save(str(out_path))
 
-    def apply_masker(self, img_paths: Union[List[str], str], masker: "Masker"):  # noqa: F821
+    def apply_masker(
+        self, img_paths: Union[List[str], str], masker: "Masker"
+    ):  # noqa: F821
         img = self.load_image(img_paths)
         img = self.preprocess_image(img)
         mask = masker.algorithm(img)
         mask = masker.postprocess_mask(mask)
         mask = masker.to_metashape_mask(mask)
 
         for path in self.get_mask_save_paths(img_paths):
             self.save_mask(mask, path)
 
 
 class SingleFileImageLoader(ImageLoader, metaclass=ABCMeta):
     @staticmethod
     def load_image(path: str) -> np.ndarray:
         img = Image.open(path)
-        return np.array(img).astype(np.float)
+        # noinspection PyTypeChecker
+        return np.array(img).astype(float)
 
     @property
     def paths(self) -> Iterable[str]:
         return list_images(self.image_directory)
 
 
 class RGBLoader(SingleFileImageLoader):
     _bit_depth = 8
 
 
 class CIRLoader(SingleFileImageLoader):
     _bit_depth = 8
     _crop_size = 256
 
-    def apply_masker(self, img_paths: Union[List[str], str], masker: 'Masker'):  # noqa: F821
-        """ Compute the image mask by moving a window over the input.
-            These CIR images are too large to be read into memory simultaneously so this image masking routine is special.
-
-            This is the setup in the following logic:
-            The inner square is the region to be written to the output.
-            The outer square is a padding section used to ensure the pixel buffers are computed properly.
-            x1,y1
-               ,-----------------,
-               |  x,y            |
-               |   ,--------,    |
-               |   |        |    |
-               |   |        |    |
-               |   |________|    |
-               |          xc,yc  |
-               |_________________|
-                               x2,y2
+    def apply_masker(
+        self, img_paths: Union[List[str], str], masker: "Masker"
+    ):  # noqa: F821
+        """Compute the image mask by moving a window over the input.
+        These CIR images are too large to be read into memory simultaneously so this
+        image masking routine is special.
+
+        This is the setup in the following logic:
+        The inner square is the region to be written to the output.
+        The outer square is a padding section used to ensure the pixel buffers are
+        computed properly.
+        x1,y1
+           ,-----------------,
+           |  x,y            |
+           |   ,--------,    |
+           |   |        |    |
+           |   |        |    |
+           |   |________|    |
+           |          xc,yc  |
+           |_________________|
+                           x2,y2
         """
         if not isinstance(img_paths, str):
             raise RuntimeError("CIRLoader can only operate on images at a single path")
         else:
             img_path = img_paths
             mask_path = next(self.get_mask_save_paths(img_paths))
 
-        with Image.open(img_path, 'r') as src:
+        with Image.open(img_path, "r") as src:
             height = src.height
             width = src.width
 
             pad = masker.pixel_buffer
 
             # Make an all black image to store the data
-            with Image.new('L', (width, height)) as dest:
+            with Image.new("L", (width, height)) as dest:
                 for y in range(0, height, self._crop_size):
                     for x in range(0, width, self._crop_size):
                         xc = min(x + self._crop_size, width)
                         yc = min(y + self._crop_size, height)
 
                         x0 = max(x - pad, 0)
                         x1 = min(xc + pad, width)
                         y0 = max(y - pad, 0)
                         y1 = min(yc + pad, height)
 
+                        # noinspection PyTypeChecker
                         img = np.array(src.crop((x0, y0, x1, y1)))
                         img = self.preprocess_image(img)
                         mask = masker.algorithm(img)
                         mask = masker.postprocess_mask(mask)
                         mask = masker.to_metashape_mask(mask)
 
                         # Remove padding
-                        mask = mask[y - y0:, x - x0:]
-                        mask = mask[:self._crop_size + pad - (y1 - yc), :self._crop_size + pad - (x1 - xc)]
+                        mask = mask[(y - y0) :, (x - x0) :]
+                        mask = mask[
+                            : self._crop_size + pad - (y1 - yc),
+                            : self._crop_size + pad - (x1 - xc),
+                        ]
 
                         # Write the mask section
                         dest.paste(Image.fromarray(mask), (x, y))
                 dest.save(mask_path)
 
 
 class MultiFileImageLoader(ImageLoader, metaclass=ABCMeta):
     @staticmethod
-    def load_image(paths: List[str]) -> np.ndarray:
+    def load_image(paths: List[Union[str, Path]]) -> np.ndarray:
+        # noinspection PyTypeChecker
         imgs = [np.asarray(Image.open(p)) for p in paths]
-        return np.stack(imgs, axis=2).astype(np.float)
+        return np.stack(imgs, axis=2).astype(float)
 
     @property
     @abstractmethod
     def paths(self) -> Iterable[List[str]]:
         raise NotImplementedError
 
 
 class MicasenseRedEdgeLoader(MultiFileImageLoader):
-    _blue_band_pattern = re.compile("(.*[\\\\/])?IMG_[0-9]{4}_1.tif", flags=re.IGNORECASE)
+    _blue_band_pattern = re.compile(
+        "(.*[\\\\/])?IMG_[0-9]{4}_1.tif", flags=re.IGNORECASE
+    )
     _bit_depth = 16
 
-    def _is_blue_band_path(self, path: str) -> bool:
+    def _is_blue_band_path(self, path: Union[str, Path]) -> bool:
         return self._blue_band_pattern.match(str(path)) is not None
 
     @property
     def _blue_band_paths(self) -> Iterable[str]:
         return filter(self._is_blue_band_path, list_images(self.image_directory))
 
     @staticmethod
     def _blue_band_path_to_band_paths(path: str) -> List[str]:
         in_path_root = Path(path).stem[:-1]
-        return [str(Path(path).with_name(f"{in_path_root}{i}.tif")) for i in range(1, 6)]
+        return [
+            str(Path(path).with_name(f"{in_path_root}{i}.tif")) for i in range(1, 6)
+        ]
 
     @property
     def paths(self) -> Iterable[List[str]]:
         return map(self._blue_band_path_to_band_paths, self._blue_band_paths)
 
 
 class P4MSLoader(MultiFileImageLoader):
-    _blue_band_pattern = re.compile("(.*[\\\\/])?DJI_[0-9]{3}1.TIF", flags=re.IGNORECASE)
+    _blue_band_pattern = re.compile(
+        "(.*[\\\\/])?DJI_[0-9]{3}1.TIF", flags=re.IGNORECASE
+    )
     _bit_depth = 16
 
-    def _is_blue_band_path(self, path: str) -> bool:
+    def _is_blue_band_path(self, path: Union[str, Path]) -> bool:
         return self._blue_band_pattern.match(str(path)) is not None
 
     @property
     def _blue_band_paths(self) -> Iterable[str]:
         return filter(self._is_blue_band_path, list_images(self.image_directory))
 
     @staticmethod
-    def _blue_band_path_to_band_paths(path: str) -> List[str]:
+    def _blue_band_path_to_band_paths(path: Union[str, Path]) -> List[str]:
         in_path_root = Path(path).stem[:-1]
-        return [str(Path(path).with_name(f"{in_path_root}{i}.TIF")) for i in range(1, 6)]
+        return [
+            str(Path(path).with_name(f"{in_path_root}{i}.TIF")) for i in range(1, 6)
+        ]
 
     @property
     def paths(self) -> Iterable[List[str]]:
         return map(self._blue_band_path_to_band_paths, self._blue_band_paths)
```

### Comparing `glint_mask_tools-3.0.4/glint_mask_generator/maskers.py` & `glint_mask_tools-3.1.0/glint_mask_generator/maskers.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,31 +7,44 @@
 import os
 from typing import Callable, List, Optional, Sequence, Union
 
 import numpy as np
 from scipy.ndimage import convolve
 
 from .glint_algorithms import GlintAlgorithm, ThresholdAlgorithm
-from .image_loaders import CIRLoader, ImageLoader, MicasenseRedEdgeLoader, P4MSLoader, RGBLoader
+from .image_loaders import (
+    CIRLoader,
+    ImageLoader,
+    MicasenseRedEdgeLoader,
+    P4MSLoader,
+    RGBLoader,
+)
 from .utils import make_circular_kernel
 
 
 class Masker(object):
-    def __init__(self, algorithm: GlintAlgorithm, image_loader: ImageLoader, pixel_buffer: int = 0):
+    def __init__(
+        self,
+        algorithm: GlintAlgorithm,
+        image_loader: ImageLoader,
+        pixel_buffer: int = 0,
+    ):
         self.algorithm = algorithm
         self.image_loader = image_loader
         self.pixel_buffer = pixel_buffer
         self.buffer_kernel = make_circular_kernel(self.pixel_buffer)
 
     # noinspection PyMethodMayBeStatic
     def postprocess_mask(self, mask: np.ndarray) -> np.ndarray:
-        """Method which can be overridden to do any postprocessing on the generated boolean numpy mask."""
+        """Hook to do any postprocessing on the generated boolean numpy mask."""
         if self.pixel_buffer <= 0:
             return mask
-        return (convolve(mask, self.buffer_kernel, mode='constant', cval=0) > 0).astype(int)
+        return (convolve(mask, self.buffer_kernel, mode="constant", cval=0) > 0).astype(
+            int
+        )
 
     @staticmethod
     def to_metashape_mask(mask: np.ndarray):
         return np.logical_not(mask).astype(np.uint8) * 255
 
     def __len__(self) -> int:
         """Get and return the number of files to process.
@@ -39,62 +52,75 @@
         Returns
         -------
         int
             The number of files that need to be processed.
         """
         return len(self.image_loader)
 
-    def __call__(self, max_workers: int,
-                 callback: Optional[Callable[[str], None]] = None,
-                 err_callback: Optional[Callable[[str, Exception], None]] = None
-                 ) -> None:
-        """Allows calling self.process by calling the object as a function.
+    def __call__(
+        self,
+        max_workers: int,
+        callback: Optional[Callable[[str], None]] = None,
+        err_callback: Optional[Callable[[str, Exception], None]] = None,
+    ) -> None:
+        """Calling Masker.process by calling the instance as a function.
 
         Parameters
         ----------
         max_workers
-            The number of threads to use during processing. Useful for limiting memory consumption.
+            The number of threads to use during processing. Useful for limiting memory
+            consumption.
         callback
-            Optional callback that receives the img_path as an arg after it is successfully processed.
+            Optional callback that receives the img_path as an arg after it is
+            successfully processed.
         err_callback
-            Optional callback that receives the img_path and an Exception as args after a processing failure.
+            Optional callback that receives the img_path and an Exception as args after
+            a processing failure.
         """
         if max_workers == 0:
             return self.process_unthreaded(callback, err_callback)
         else:
             return self.process(max_workers, callback, err_callback)
 
     # noinspection SpellCheckingInspection
-    def process_unthreaded(self, callback: Optional[Callable[[List[str]], None]] = None,
-                           err_callback: Optional[Callable[[List[str], Exception], None]] = None) -> None:
+    def process_unthreaded(
+        self,
+        callback: Optional[Callable[[List[str]], None]] = None,
+        err_callback: Optional[Callable[[List[str], Exception], None]] = None,
+    ) -> None:
         for paths in self.image_loader.paths:
             try:
                 self._process_one(paths)
                 if callback is not None:
                     callback(paths)
 
             except Exception as exc:
                 if err_callback is not None:
                     err_callback(paths, exc)
                 return
 
-    def process(self, max_workers: int = os.cpu_count(), callback: Optional[Callable[[List[str]], None]] = None,
-                err_callback: Optional[Callable[[List[str], Exception], None]] = None) -> None:
+    def process(
+        self,
+        max_workers: int = os.cpu_count(),
+        callback: Optional[Callable[[List[str]], None]] = None,
+        err_callback: Optional[Callable[[List[str], Exception], None]] = None,
+    ) -> None:
         """Compute all glint masks.
 
-        Computes masks for all images in self.img_paths using the process_func and save to the mask_out_paths.
+        Computes masks for all images in self.img_paths using the process_func and save
+        to the mask_out_paths.
 
         Parameters
         ----------
         max_workers
             The maximum number of image processing workers.
             Useful for limiting memory usage.
         callback
-            Optional callback function passed the name of each input and output mask files after processing it.
-            Will receive img_path: str as arg.
+            Optional callback function passed the name of each input and output mask
+            files after processing it. Will receive img_path: str as arg.
         err_callback
             Optional callback function passed exception object on processing failure.
             Will receive img_path: str, and the Exception as args.
         """
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
             future_to_paths = {
                 executor.submit(self._process_one, paths): paths
@@ -112,50 +138,81 @@
                         err_callback(paths, exc)
                     executor.shutdown(wait=False)
                     return
 
     def _process_one(self, paths: Union[List[str], str]) -> None:
         """Generates and saves a glint mask for the image located at img_path.
 
-        Saves the generated mask to all path locations returned by self.get_mask_save_paths(img_path).
+        Saves the generated mask to all path locations returned by
+        self.get_mask_save_paths(img_path).
 
         Parameters
         ----------
         paths
-            The file paths used to create the image. Can be single file path or list of path to multiple files
+            The file paths used to create the image. Can be single file path or list of
+            path to multiple files
         """
         self.image_loader.apply_masker(paths, self)
 
 
 class RGBThresholdMasker(Masker):
-    def __init__(self, img_dir: str, mask_dir: str,
-                 thresholds: Sequence[float] = (1, 1, 0.875), pixel_buffer: int = 0):
-        super().__init__(algorithm=ThresholdAlgorithm(thresholds),
-                         image_loader=RGBLoader(img_dir, mask_dir),
-                         pixel_buffer=pixel_buffer)
+    def __init__(
+        self,
+        img_dir: str,
+        mask_dir: str,
+        thresholds: Sequence[float] = (1, 1, 0.875),
+        pixel_buffer: int = 0,
+    ):
+        super().__init__(
+            algorithm=ThresholdAlgorithm(thresholds),
+            image_loader=RGBLoader(img_dir, mask_dir),
+            pixel_buffer=pixel_buffer,
+        )
 
 
 class CIRThresholdMasker(Masker):
-    def __init__(self, img_dir: str, mask_dir: str,
-                 thresholds: Sequence[float] = (1, 1, 0.875, 1), pixel_buffer: int = 0):
-        super().__init__(algorithm=ThresholdAlgorithm(thresholds),
-                         image_loader=CIRLoader(img_dir, mask_dir),
-                         pixel_buffer=pixel_buffer)
+    def __init__(
+        self,
+        img_dir: str,
+        mask_dir: str,
+        thresholds: Sequence[float] = (1, 1, 0.875, 1),
+        pixel_buffer: int = 0,
+    ):
+        super().__init__(
+            algorithm=ThresholdAlgorithm(thresholds),
+            image_loader=CIRLoader(img_dir, mask_dir),
+            pixel_buffer=pixel_buffer,
+        )
 
 
 class P4MSThresholdMasker(Masker):
-    def __init__(self, img_dir: str, mask_dir: str,
-                 thresholds: Sequence[float] = (0.875, 1, 1, 1, 1), pixel_buffer: int = 0):
-        super().__init__(algorithm=ThresholdAlgorithm(thresholds),
-                         image_loader=P4MSLoader(img_dir, mask_dir),
-                         pixel_buffer=pixel_buffer)
+    def __init__(
+        self,
+        img_dir: str,
+        mask_dir: str,
+        thresholds: Sequence[float] = (0.875, 1, 1, 1, 1),
+        pixel_buffer: int = 0,
+    ):
+        super().__init__(
+            algorithm=ThresholdAlgorithm(thresholds),
+            image_loader=P4MSLoader(img_dir, mask_dir),
+            pixel_buffer=pixel_buffer,
+        )
 
 
 class MicasenseRedEdgeThresholdMasker(Masker):
-    def __init__(self, img_dir: str, mask_dir: str,
-                 thresholds: Sequence[float] = (0.875, 1, 1, 1, 1), pixel_buffer: int = 0):
-        super().__init__(algorithm=ThresholdAlgorithm(thresholds),
-                         image_loader=MicasenseRedEdgeLoader(img_dir, mask_dir),
-                         pixel_buffer=pixel_buffer)
+    def __init__(
+        self,
+        img_dir: str,
+        mask_dir: str,
+        thresholds: Sequence[float] = (0.875, 1, 1, 1, 1),
+        pixel_buffer: int = 0,
+    ):
+        super().__init__(
+            algorithm=ThresholdAlgorithm(thresholds),
+            image_loader=MicasenseRedEdgeLoader(img_dir, mask_dir),
+            pixel_buffer=pixel_buffer,
+        )
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     CIRThresholdMasker("ignore/in", "ignore/out", pixel_buffer=10).process_unthreaded()
```

### Comparing `glint_mask_tools-3.0.4/glint_mask_generator/utils.py` & `glint_mask_tools-3.1.0/glint_mask_generator/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pathlib import Path
 from typing import Iterable
 
 import numpy as np
 
 
 def normalize_img(img: np.ndarray, bit_depth: int) -> np.ndarray:
-    """Utility function to normalize the values of an image with arbitrary bit_depth to range [0, 1].
+    """Normalize the values of an image with arbitrary bit_depth to range [0, 1].
 
     Parameters
     ----------
     img
         The image data
     bit_depth
         The bit depth of the image.
@@ -27,17 +27,17 @@
     """
     return img / ((1 << bit_depth) - 1)
 
 
 def list_images(img_dir) -> Iterable[str]:
     """List all image files in img_dir.
 
-    Returns an iterator that lists the files to process. Subclasses may want to override this to return specific
-    image types or filter the results. By default, will list all images in self.img_dir if the file extension is in
-    the extensions list.
+    Returns an iterator that lists the files to process. Subclasses may want to override
+    this to return specific image types or filter the results. By default, will list all
+    images in self.img_dir if the file extension is in the extensions list.
 
     Returns
     -------
     Iterable[str]
         The list of files to be used for generating the masks.
     """
     extensions = (".png", ".jpg", ".jpeg", ".tif", ".tiff")
@@ -45,10 +45,10 @@
     paths = Path(img_dir).glob("**/*")
     paths = filter(lambda p: p.is_file() and p.suffix.lower() in extensions, paths)
     return (str(p) for p in paths)
 
 
 def make_circular_kernel(size: int) -> np.ndarray:
     """Create circular kernel"""
-    y, x = np.ogrid[-size:size + 1, -size:size + 1]
-    dist_m: np.ndarray = x ** 2 + y ** 2
-    return dist_m <= size ** 2
+    y, x = np.ogrid[-size : size + 1, -size : size + 1]
+    dist_m: np.ndarray = x**2 + y**2
+    return dist_m <= size**2
```

### Comparing `glint_mask_tools-3.0.4/pyproject.toml` & `glint_mask_tools-3.1.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 [tool.poetry]
 name = "glint-mask-tools"
-version = "3.0.4"
+version = "3.1.0"
 description = "Create masks for specular reflection in UAV and aerial imagery"
 authors = ["Taylor Denouden <taylor.denouden@hakai.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/HakaiInstitute/GlintMaskGenerator"
 packages = [
     { include = "glint_mask_generator" }
 ]
 
 [tool.poetry.scripts]
 glint-mask = 'glint_mask_generator.cli:main'
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.11"
-numpy = "~=1.23.5"
-fire = "~=0.4.0"
+python = ">=3.9,<3.12"
+numpy = "~=1.25.1"
+fire = "~=0.5.0"
 Pillow = "~=9.3.0"
-scipy = ">=1.9.3,<1.11.0"
-tqdm = "~=4.64.1"
-loguru = "~=0.6.0"
+scipy = "~=1.11.1"
+tqdm = "~=4.65.0"
+loguru = "~=0.7.0"
 pyqt6 = "^6.4.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 flake8 = "^6.0.0"
 pyinstaller = "^5.6.2"
+pre-commit = "^3.3.3"
+ruff = "^0.0.280"
+black = "^23.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `glint_mask_tools-3.0.4/setup.py` & `glint_mask_tools-3.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 ['glint_mask_generator']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Pillow>=9.3.0,<9.4.0',
- 'fire>=0.4.0,<0.5.0',
- 'loguru>=0.6.0,<0.7.0',
- 'numpy>=1.23.5,<1.24.0',
+ 'fire>=0.5.0,<0.6.0',
+ 'loguru>=0.7.0,<0.8.0',
+ 'numpy>=1.25.1,<1.26.0',
  'pyqt6>=6.4.0,<7.0.0',
- 'scipy>=1.9.3,<1.11.0',
- 'tqdm>=4.64.1,<4.65.0']
+ 'scipy>=1.11.1,<1.12.0',
+ 'tqdm>=4.65.0,<4.66.0']
 
 entry_points = \
 {'console_scripts': ['glint-mask = glint_mask_generator.cli:main']}
 
 setup_kwargs = {
     'name': 'glint-mask-tools',
-    'version': '3.0.4',
+    'version': '3.1.0',
     'description': 'Create masks for specular reflection in UAV and aerial imagery',
-    'long_description': '# Glint Mask Tools\n\n<div style="overflow: hidden; display: flex; justify-content:flex-start; gap:10px;">\n<a href="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml">\n    <img alt="Tests" src="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml/badge.svg"/>\n</a>\n\n<a href="https://github.com/HakaiInstitute/GlintMaskGenerator/blob/main/LICENSE.txt">\n    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-black.svg" height="20px" />\n</a>\n\n<a href="https://badge.fury.io/py/glint-mask-tools">\n    <img alt="PyPI version" src="https://badge.fury.io/py/glint-mask-tools.svg" height="20">\n</a>\n\n<a href="https://zenodo.org/badge/latestdoi/266147098">\n    <img src="https://zenodo.org/badge/266147098.svg" alt="DOI">\n</a>\n</div>\n\n## Description\n\nGlintMaskGenerator generates image masks for regions in RGB and multispectral image files that have high levels of specular reflection.\n\nThese masks can be used in 3rd party structure-from-motion programs to replace these high glint regions with more useful data from adjacent, overlapping imagery.\n\n## Installation\n\n1. Go to the [releases page](https://github.com/HakaiInstitute/glint-mask-tools/releases)\n2. Download the latest release file for your operating system.\n3. Extract the compressed binary files from the gzipped archive.\n4. This archive contains a file named GlintMaskGenerator-v*.\\*.\\*.exe that provides a GUI interface to the glint mask generation program.\n5. You can copy these files to any location that is convenient for you.\n\n### PyPi package\n\nThere also a python package version of the code available for Python 3.8 and 3.9.\n\n1. `pip install glint-mask-tools` to install the tools.\n2. Then, `import glint_mask_generator` in your Python script.\n3. Installing with pip also installs the CLI tool, detailed below.\n\n## Usage\n\n### GUI\n\nIn Windows, launch the GUI by double clicking the executable file. In Linux, you\'ll have to launch the GUI from the\nterminal, e.g. `./GlintMaskGenerator`.\n\nFor now, generating masks by passing directory paths containing images is the supported workflow. Be sure to change the\nimage type option when processing imagery for cameras other than RGB cameras (e.g. Micasense RedEdge or DJI P4MS cameras). You will be notified of any\nprocessing errors via a pop-up dialog.\n\n### CLI\n\nFor information about the parameters expected by the CLI, run `glint-mask --help` in a bash terminal or command\nline interface. All the functionality of the CLI is documented there.\n\n#### Examples\n\n```bash\nglint-mask-v*.*.* --help\n\n# NAME\n#     glint-mask-v*.*.*\n# \n# SYNOPSIS\n#     glint-mask-v*.*.* - COMMAND | VALUE\n# \n# COMMANDS\n#     COMMAND is one of the following:\n# \n#      cir_threshold\n#        Generate masks for glint regions in 4 Band CIR imagery using Tom Bell\'s binning algorithm.\n# \n#      micasense_threshold\n#        Generate masks for glint regions in multispectral imagery from the Micasense camera using Tom Bell\'s algorithm on the blue image band.\n# \n#      p4ms_threshold\n#        Generate masks for glint regions in multispectral imagery from the DJI camera using Tom Bell\'s algorithm on the Blue image band.\n# \n#      process\n# \n#      rgb_threshold\n#        Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n# \n# VALUES\n#     VALUE is one of the following:\n# \n#      max_workers\n#        The maximum number of threads to use for processing.\n```\n\n```bash\n# Get addition parameters for one of the cameras/methods available\nglint-mask-v*.*.* rgb_threshold --help\n\n# NAME\n#     glint-mask-v*.*.* rgb_threshold - Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n# \n# SYNOPSIS\n#     glint-mask-v*.*.* rgb_threshold IMG_DIR OUT_DIR <flags>\n# \n# DESCRIPTION\n#     Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n# \n# POSITIONAL ARGUMENTS\n#     IMG_DIR\n#         The path to a named input image or directory containing images. If img_dir is a directory, all tif, jpg, jpeg, and png images in that directory will be # processed.\n#     OUT_DIR\n#         The path to send your out image including the file name and type. e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is specified as a # # # directory.\n# \n# FLAGS\n#     --thresholds=THRESHOLDS\n#         The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [1, 1, 0.875].\n#     --pixel_buffer=PIXEL_BUFFER\n#         The pixel distance to buffer out the mask. Defaults to 0 (off).\n# \n# NOTES\n#     You can also use flags syntax for POSITIONAL ARGUMENTS\n```\n\n```bash\n# Process rgb imagery directory with default parameters\nglint-mask-v*.*.* rgb_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process PhaseONE camera imagery with image bands split over multiple files\nglint-mask-v*.*.* aco_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process DJI P4MS imagery\nglint-mask-v*.*.* p4ms_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process Micasense RedEdge imagery \nglint-mask-v*.*.* micasense_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n```\n\n### Python package\nInstalling the PyPi package allows integrating the mask generation workflow into existing python scripts with ease.\n\n```python\nfrom glint_mask_generator import MicasenseRedEdgeThresholdMasker\n\n# Also available: P4MSThresholdMasker, RGBIntensityRatioMasker, RGBThresholdMasker\n\nmasker = MicasenseRedEdgeThresholdMasker(img_dir="path/to/micasense/images/", mask_dir="path/to/output/dir/",\n                                         thresholds=(0.875, 1, 1, 1, 1), pixel_buffer=5)\nmasker.process(max_workers=5, callback=print, err_callback=print)\n```\n\n## Notes\n\n### Directory of images processing\n\n- All files with "jpg", "jpeg", "tif", "tiff" and "png" extensions will be processed. This can be extended as needed.\n  File extension matching is case-insensitive.\n- Output mask files with be in the specified directory, and have the same name as the input file with "_mask" appended\n  to the end of the file name stem. The file type will match the input type.\n\n### Multi-band image processing\n- For imagery types where each band is spread over multiple files, a mask will be generated for all the sibling band images.\n    - For example, if a mask is generated using a threshold on the blue band image, identical masks are saved for sibling red, green, blue, nir, and red_edge bands as well.\n    - If thresholds are passed for multiple bands, these mask outputs combined with a union operator before being saved for all the sibling bands associated with that capture event.\n\n## Bugs and Feature Requests\n\nThis software is under active development. Bugs and feature requests can be filed using issues page located [here](https://github.com/HakaiInstitute/glint-mask-tools/issues).\n\n## Citation\n\nResearch using these tools or code should cite the following resources\n\n```bibtext\n@article{Cavanaugh2021,\n\ttitle        = {An Automated Method for Mapping Giant Kelp Canopy Dynamics from UAV},\n\tauthor       = {Cavanaugh, K.C. and Cavanaugh, K.C. and Bell, T.W. and Hockridge, E.G.},\n\tyear         = 2021,\n\tjournal      = {Front. Environ. Sci.},\n\tvolume       = {8:587354},\n\tdoi          = {10.3389/fenvs.2020.587354}\n}\n@misc{Denouden2021,\n\ttitle        = {GlintMaskGenerator},\n\tauthor       = {Denouden, T. and Timmer, B. and Reshitnyk, L.},\n\tyear         = 2021,\n\tjournal      = {GitHub repository},\n\tpublisher    = {GitHub},\n\tdoi          = {10.21966/3cpa-2e10},\n\thowpublished = {\\url{https://github.com/HakaiInstitute/GlintMaskGenerator}},\n\tcommit       = {8cb19e55f128da86bf0dbd312bc360ac89fe71c3}\n}\n```\n\n## Development\n\nSee [DEVELOPMENT.md](DEVELOPMENT.md) for development and software maintenance instructions.\n\n## License\nGlintMaskGenerator is released under a MIT license, as found in the [LICENSE](LICENSE) file.\n',
+    'long_description': '# Glint Mask Tools\n\n<div style="overflow: hidden; display: flex; justify-content:flex-start; gap:10px;">\n<a href="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml">\n    <img alt="Tests" src="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml/badge.svg"/>\n</a>\n\n<a href="https://github.com/HakaiInstitute/GlintMaskGenerator/blob/main/LICENSE.txt">\n    <img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-black.svg" height="20px" />\n</a>\n\n<a href="https://badge.fury.io/py/glint-mask-tools">\n    <img alt="PyPI version" src="https://badge.fury.io/py/glint-mask-tools.svg" height="20">\n</a>\n\n<a href="https://zenodo.org/badge/latestdoi/266147098">\n    <img src="https://zenodo.org/badge/266147098.svg" alt="DOI">\n</a>\n</div>\n\n## Description\n\nGlintMaskGenerator generates image masks for regions in RGB and multispectral image files that have high levels of specular reflection.\n\nThese masks can be used in 3rd party structure-from-motion programs to replace these high glint regions with more useful data from adjacent, overlapping imagery.\n\n## Installation\n\n1. Go to the [releases page](https://github.com/HakaiInstitute/glint-mask-tools/releases)\n2. Download the latest release file for your operating system.\n3. Extract the compressed binary files from the gzipped archive.\n4. This archive contains a file named GlintMaskGenerator-v*.\\*.\\*.exe that provides a GUI interface to the glint mask generation program.\n5. You can copy these files to any location that is convenient for you.\n\n### PyPi package\n\nThere also a python package version of the code available for Python 3.8 and 3.9.\n\n1. `pip install glint-mask-tools` to install the tools.\n2. Then, `import glint_mask_generator` in your Python script.\n3. Installing with pip also installs the CLI tool, detailed below.\n\n## Usage\n\n### GUI\n\nIn Windows, launch the GUI by double clicking the executable file. In Linux, you\'ll have to launch the GUI from the\nterminal, e.g. `./GlintMaskGenerator`.\n\nFor now, generating masks by passing directory paths containing images is the supported workflow. Be sure to change the\nimage type option when processing imagery for cameras other than RGB cameras (e.g. Micasense RedEdge or DJI P4MS cameras). You will be notified of any\nprocessing errors via a pop-up dialog.\n\n### CLI\n\nFor information about the parameters expected by the CLI, run `glint-mask --help` in a bash terminal or command\nline interface. All the functionality of the CLI is documented there.\n\n#### Examples\n\n```bash\nglint-mask-v*.*.* --help\n\n# NAME\n#     glint-mask-v*.*.*\n#\n# SYNOPSIS\n#     glint-mask-v*.*.* - COMMAND | VALUE\n#\n# COMMANDS\n#     COMMAND is one of the following:\n#\n#      cir_threshold\n#        Generate masks for glint regions in 4 Band CIR imagery using Tom Bell\'s binning algorithm.\n#\n#      micasense_threshold\n#        Generate masks for glint regions in multispectral imagery from the Micasense camera using Tom Bell\'s algorithm on the blue image band.\n#\n#      p4ms_threshold\n#        Generate masks for glint regions in multispectral imagery from the DJI camera using Tom Bell\'s algorithm on the Blue image band.\n#\n#      process\n#\n#      rgb_threshold\n#        Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n#\n# VALUES\n#     VALUE is one of the following:\n#\n#      max_workers\n#        The maximum number of threads to use for processing.\n```\n\n```bash\n# Get addition parameters for one of the cameras/methods available\nglint-mask-v*.*.* rgb_threshold --help\n\n# NAME\n#     glint-mask-v*.*.* rgb_threshold - Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n#\n# SYNOPSIS\n#     glint-mask-v*.*.* rgb_threshold IMG_DIR OUT_DIR <flags>\n#\n# DESCRIPTION\n#     Generate masks for glint regions in RGB imagery using Tom Bell\'s binning algorithm.\n#\n# POSITIONAL ARGUMENTS\n#     IMG_DIR\n#         The path to a named input image or directory containing images. If img_dir is a directory, all tif, jpg, jpeg, and png images in that directory will be # processed.\n#     OUT_DIR\n#         The path to send your out image including the file name and type. e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is specified as a # # # directory.\n#\n# FLAGS\n#     --thresholds=THRESHOLDS\n#         The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [1, 1, 0.875].\n#     --pixel_buffer=PIXEL_BUFFER\n#         The pixel distance to buffer out the mask. Defaults to 0 (off).\n#\n# NOTES\n#     You can also use flags syntax for POSITIONAL ARGUMENTS\n```\n\n```bash\n# Process rgb imagery directory with default parameters\nglint-mask-v*.*.* rgb_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process PhaseONE camera imagery with image bands split over multiple files\nglint-mask-v*.*.* aco_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process DJI P4MS imagery\nglint-mask-v*.*.* p4ms_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n# Process Micasense RedEdge imagery\nglint-mask-v*.*.* micasense_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n```\n\n### Python package\nInstalling the PyPi package allows integrating the mask generation workflow into existing python scripts with ease.\n\n```python\nfrom glint_mask_generator import MicasenseRedEdgeThresholdMasker\n\n# Also available: P4MSThresholdMasker, RGBIntensityRatioMasker, RGBThresholdMasker\n\nmasker = MicasenseRedEdgeThresholdMasker(img_dir="path/to/micasense/images/", mask_dir="path/to/output/dir/",\n                                         thresholds=(0.875, 1, 1, 1, 1), pixel_buffer=5)\nmasker.process(max_workers=5, callback=print, err_callback=print)\n```\n\n## Notes\n\n### Directory of images processing\n\n- All files with "jpg", "jpeg", "tif", "tiff" and "png" extensions will be processed. This can be extended as needed.\n  File extension matching is case-insensitive.\n- Output mask files with be in the specified directory, and have the same name as the input file with "_mask" appended\n  to the end of the file name stem. The file type will match the input type.\n\n### Multi-band image processing\n- For imagery types where each band is spread over multiple files, a mask will be generated for all the sibling band images.\n    - For example, if a mask is generated using a threshold on the blue band image, identical masks are saved for sibling red, green, blue, nir, and red_edge bands as well.\n    - If thresholds are passed for multiple bands, these mask outputs combined with a union operator before being saved for all the sibling bands associated with that capture event.\n\n## Bugs and Feature Requests\n\nThis software is under active development. Bugs and feature requests can be filed using issues page located [here](https://github.com/HakaiInstitute/glint-mask-tools/issues).\n\n## Citation\n\nResearch using these tools or code should cite the following resources\n\n```bibtext\n@article{Cavanaugh2021,\n\ttitle        = {An Automated Method for Mapping Giant Kelp Canopy Dynamics from UAV},\n\tauthor       = {Cavanaugh, K.C. and Cavanaugh, K.C. and Bell, T.W. and Hockridge, E.G.},\n\tyear         = 2021,\n\tjournal      = {Front. Environ. Sci.},\n\tvolume       = {8:587354},\n\tdoi          = {10.3389/fenvs.2020.587354}\n}\n@misc{Denouden2021,\n\ttitle        = {GlintMaskGenerator},\n\tauthor       = {Denouden, T. and Timmer, B. and Reshitnyk, L.},\n\tyear         = 2021,\n\tjournal      = {GitHub repository},\n\tpublisher    = {GitHub},\n\tdoi          = {10.21966/3cpa-2e10},\n\thowpublished = {\\url{https://github.com/HakaiInstitute/GlintMaskGenerator}},\n\tcommit       = {8cb19e55f128da86bf0dbd312bc360ac89fe71c3}\n}\n```\n\n## Development\n\nSee [DEVELOPMENT.md](DEVELOPMENT.md) for development and software maintenance instructions.\n\n## License\nGlintMaskGenerator is released under a MIT license, as found in the [LICENSE](LICENSE) file.\n',
     'author': 'Taylor Denouden',
     'author_email': 'taylor.denouden@hakai.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/HakaiInstitute/GlintMaskGenerator',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<3.11',
+    'python_requires': '>=3.9,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['glint_mask_generator'] package_data = \ {'': ['*']} install_requires = \
-['Pillow>=9.3.0,<9.4.0', 'fire>=0.4.0,<0.5.0', 'loguru>=0.6.0,<0.7.0',
-'numpy>=1.23.5,<1.24.0', 'pyqt6>=6.4.0,<7.0.0', 'scipy>=1.9.3,<1.11.0',
-'tqdm>=4.64.1,<4.65.0'] entry_points = \ {'console_scripts': ['glint-mask =
+['Pillow>=9.3.0,<9.4.0', 'fire>=0.5.0,<0.6.0', 'loguru>=0.7.0,<0.8.0',
+'numpy>=1.25.1,<1.26.0', 'pyqt6>=6.4.0,<7.0.0', 'scipy>=1.11.1,<1.12.0',
+'tqdm>=4.65.0,<4.66.0'] entry_points = \ {'console_scripts': ['glint-mask =
 glint_mask_generator.cli:main']} setup_kwargs = { 'name': 'glint-mask-tools',
-'version': '3.0.4', 'description': 'Create masks for specular reflection in UAV
+'version': '3.1.0', 'description': 'Create masks for specular reflection in UAV
 and aerial imagery', 'long_description': '# Glint Mask Tools\n\n
 \n\n_[Tests]\n\n\n\n_[License:_MIT]\n\n\n\n_[PyPI_version]\n\n\n\n_[DOI]\n\n
 \n\n## Description\n\nGlintMaskGenerator generates image masks for regions in
 RGB and multispectral image files that have high levels of specular
 reflection.\n\nThese masks can be used in 3rd party structure-from-motion
 programs to replace these high glint regions with more useful data from
 adjacent, overlapping imagery.\n\n## Installation\n\n1. Go to the [releases
@@ -27,48 +27,47 @@
 passing directory paths containing images is the supported workflow. Be sure to
 change the\nimage type option when processing imagery for cameras other than
 RGB cameras (e.g. Micasense RedEdge or DJI P4MS cameras). You will be notified
 of any\nprocessing errors via a pop-up dialog.\n\n### CLI\n\nFor information
 about the parameters expected by the CLI, run `glint-mask --help` in a bash
 terminal or command\nline interface. All the functionality of the CLI is
 documented there.\n\n#### Examples\n\n```bash\nglint-mask-v*.*.* --help\n\n#
-NAME\n# glint-mask-v*.*.*\n# \n# SYNOPSIS\n# glint-mask-v*.*.* - COMMAND |
-VALUE\n# \n# COMMANDS\n# COMMAND is one of the following:\n# \n#
-cir_threshold\n# Generate masks for glint regions in 4 Band CIR imagery using
-Tom Bell\'s binning algorithm.\n# \n# micasense_threshold\n# Generate masks for
-glint regions in multispectral imagery from the Micasense camera using Tom
-Bell\'s algorithm on the blue image band.\n# \n# p4ms_threshold\n# Generate
-masks for glint regions in multispectral imagery from the DJI camera using Tom
-Bell\'s algorithm on the Blue image band.\n# \n# process\n# \n#
-rgb_threshold\n# Generate masks for glint regions in RGB imagery using Tom
-Bell\'s binning algorithm.\n# \n# VALUES\n# VALUE is one of the following:\n#
-\n# max_workers\n# The maximum number of threads to use for
-processing.\n```\n\n```bash\n# Get addition parameters for one of the cameras/
-methods available\nglint-mask-v*.*.* rgb_threshold --help\n\n# NAME\n# glint-
-mask-v*.*.* rgb_threshold - Generate masks for glint regions in RGB imagery
-using Tom Bell\'s binning algorithm.\n# \n# SYNOPSIS\n# glint-mask-v*.*.*
-rgb_threshold IMG_DIR OUT_DIR \n# \n# DESCRIPTION\n# Generate masks for glint
-regions in RGB imagery using Tom Bell\'s binning algorithm.\n# \n# POSITIONAL
-ARGUMENTS\n# IMG_DIR\n# The path to a named input image or directory containing
-images. If img_dir is a directory, all tif, jpg, jpeg, and png images in that
-directory will be # processed.\n# OUT_DIR\n# The path to send your out image
-including the file name and type. e.g. "/path/to/mask.png". out_dir must be a
-directory if img_dir is specified as a # # # directory.\n# \n# FLAGS\n# --
-thresholds=THRESHOLDS\n# The pixel band thresholds indicating glint. Domain for
-values is (0.0, 1.0). Default is [1, 1, 0.875].\n# --
-pixel_buffer=PIXEL_BUFFER\n# The pixel distance to buffer out the mask.
-Defaults to 0 (off).\n# \n# NOTES\n# You can also use flags syntax for
+NAME\n# glint-mask-v*.*.*\n#\n# SYNOPSIS\n# glint-mask-v*.*.* - COMMAND |
+VALUE\n#\n# COMMANDS\n# COMMAND is one of the following:\n#\n# cir_threshold\n#
+Generate masks for glint regions in 4 Band CIR imagery using Tom Bell\'s
+binning algorithm.\n#\n# micasense_threshold\n# Generate masks for glint
+regions in multispectral imagery from the Micasense camera using Tom Bell\'s
+algorithm on the blue image band.\n#\n# p4ms_threshold\n# Generate masks for
+glint regions in multispectral imagery from the DJI camera using Tom Bell\'s
+algorithm on the Blue image band.\n#\n# process\n#\n# rgb_threshold\n# Generate
+masks for glint regions in RGB imagery using Tom Bell\'s binning
+algorithm.\n#\n# VALUES\n# VALUE is one of the following:\n#\n# max_workers\n#
+The maximum number of threads to use for processing.\n```\n\n```bash\n# Get
+addition parameters for one of the cameras/methods available\nglint-mask-v*.*.*
+rgb_threshold --help\n\n# NAME\n# glint-mask-v*.*.* rgb_threshold - Generate
+masks for glint regions in RGB imagery using Tom Bell\'s binning
+algorithm.\n#\n# SYNOPSIS\n# glint-mask-v*.*.* rgb_threshold IMG_DIR OUT_DIR
+\n#\n# DESCRIPTION\n# Generate masks for glint regions in RGB imagery using Tom
+Bell\'s binning algorithm.\n#\n# POSITIONAL ARGUMENTS\n# IMG_DIR\n# The path to
+a named input image or directory containing images. If img_dir is a directory,
+all tif, jpg, jpeg, and png images in that directory will be # processed.\n#
+OUT_DIR\n# The path to send your out image including the file name and type.
+e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is specified
+as a # # # directory.\n#\n# FLAGS\n# --thresholds=THRESHOLDS\n# The pixel band
+thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [1, 1,
+0.875].\n# --pixel_buffer=PIXEL_BUFFER\n# The pixel distance to buffer out the
+mask. Defaults to 0 (off).\n#\n# NOTES\n# You can also use flags syntax for
 POSITIONAL ARGUMENTS\n```\n\n```bash\n# Process rgb imagery directory with
 default parameters\nglint-mask-v*.*.* rgb_threshold /path/to/dir/with/images/ /
 path/to/out_masks/dir/\n\n# Process PhaseONE camera imagery with image bands
 split over multiple files\nglint-mask-v*.*.* aco_threshold /path/to/dir/with/
 images/ /path/to/out_masks/dir/\n\n# Process DJI P4MS imagery\nglint-mask-
 v*.*.* p4ms_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/\n\n#
-Process Micasense RedEdge imagery \nglint-mask-v*.*.* micasense_threshold /
-path/to/dir/with/images/ /path/to/out_masks/dir/\n```\n\n### Python
+Process Micasense RedEdge imagery\nglint-mask-v*.*.* micasense_threshold /path/
+to/dir/with/images/ /path/to/out_masks/dir/\n```\n\n### Python
 package\nInstalling the PyPi package allows integrating the mask generation
 workflow into existing python scripts with ease.\n\n```python\nfrom
 glint_mask_generator import MicasenseRedEdgeThresholdMasker\n\n# Also
 available: P4MSThresholdMasker, RGBIntensityRatioMasker,
 RGBThresholdMasker\n\nmasker = MicasenseRedEdgeThresholdMasker(img_dir="path/
 to/micasense/images/", mask_dir="path/to/output/dir/",\n thresholds=(0.875, 1,
 1, 1, 1), pixel_buffer=5)\nmasker.process(max_workers=5, callback=print,
@@ -101,8 +100,8 @@
 [DEVELOPMENT.md](DEVELOPMENT.md) for development and software maintenance
 instructions.\n\n## License\nGlintMaskGenerator is released under a MIT
 license, as found in the [LICENSE](LICENSE) file.\n', 'author': 'Taylor
 Denouden', 'author_email': 'taylor.denouden@hakai.org', 'maintainer': 'None',
 'maintainer_email': 'None', 'url': 'https://github.com/HakaiInstitute/
 GlintMaskGenerator', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'entry_points': entry_points,
-'python_requires': '>=3.8.1,<3.11', } setup(**setup_kwargs)
+'python_requires': '>=3.9,<3.12', } setup(**setup_kwargs)
```

### Comparing `glint_mask_tools-3.0.4/PKG-INFO` & `glint_mask_tools-3.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: glint-mask-tools
-Version: 3.0.4
+Version: 3.1.0
 Summary: Create masks for specular reflection in UAV and aerial imagery
 Home-page: https://github.com/HakaiInstitute/GlintMaskGenerator
 License: MIT
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
-Requires-Python: >=3.8.1,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pillow (>=9.3.0,<9.4.0)
-Requires-Dist: fire (>=0.4.0,<0.5.0)
-Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: numpy (>=1.23.5,<1.24.0)
+Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: loguru (>=0.7.0,<0.8.0)
+Requires-Dist: numpy (>=1.25.1,<1.26.0)
 Requires-Dist: pyqt6 (>=6.4.0,<7.0.0)
-Requires-Dist: scipy (>=1.9.3,<1.11.0)
-Requires-Dist: tqdm (>=4.64.1,<4.65.0)
+Requires-Dist: scipy (>=1.11.1,<1.12.0)
+Requires-Dist: tqdm (>=4.65.0,<4.66.0)
 Project-URL: Repository, https://github.com/HakaiInstitute/GlintMaskGenerator
 Description-Content-Type: text/markdown
 
 # Glint Mask Tools
 
 <div style="overflow: hidden; display: flex; justify-content:flex-start; gap:10px;">
 <a href="https://github.com/HakaiInstitute/GlintMaskGenerator/actions/workflows/test_code.yml">
@@ -82,82 +83,82 @@
 #### Examples
 
 ```bash
 glint-mask-v*.*.* --help
 
 # NAME
 #     glint-mask-v*.*.*
-# 
+#
 # SYNOPSIS
 #     glint-mask-v*.*.* - COMMAND | VALUE
-# 
+#
 # COMMANDS
 #     COMMAND is one of the following:
-# 
+#
 #      cir_threshold
 #        Generate masks for glint regions in 4 Band CIR imagery using Tom Bell's binning algorithm.
-# 
+#
 #      micasense_threshold
 #        Generate masks for glint regions in multispectral imagery from the Micasense camera using Tom Bell's algorithm on the blue image band.
-# 
+#
 #      p4ms_threshold
 #        Generate masks for glint regions in multispectral imagery from the DJI camera using Tom Bell's algorithm on the Blue image band.
-# 
+#
 #      process
-# 
+#
 #      rgb_threshold
 #        Generate masks for glint regions in RGB imagery using Tom Bell's binning algorithm.
-# 
+#
 # VALUES
 #     VALUE is one of the following:
-# 
+#
 #      max_workers
 #        The maximum number of threads to use for processing.
 ```
 
 ```bash
 # Get addition parameters for one of the cameras/methods available
 glint-mask-v*.*.* rgb_threshold --help
 
 # NAME
 #     glint-mask-v*.*.* rgb_threshold - Generate masks for glint regions in RGB imagery using Tom Bell's binning algorithm.
-# 
+#
 # SYNOPSIS
 #     glint-mask-v*.*.* rgb_threshold IMG_DIR OUT_DIR <flags>
-# 
+#
 # DESCRIPTION
 #     Generate masks for glint regions in RGB imagery using Tom Bell's binning algorithm.
-# 
+#
 # POSITIONAL ARGUMENTS
 #     IMG_DIR
 #         The path to a named input image or directory containing images. If img_dir is a directory, all tif, jpg, jpeg, and png images in that directory will be # processed.
 #     OUT_DIR
 #         The path to send your out image including the file name and type. e.g. "/path/to/mask.png". out_dir must be a directory if img_dir is specified as a # # # directory.
-# 
+#
 # FLAGS
 #     --thresholds=THRESHOLDS
 #         The pixel band thresholds indicating glint. Domain for values is (0.0, 1.0). Default is [1, 1, 0.875].
 #     --pixel_buffer=PIXEL_BUFFER
 #         The pixel distance to buffer out the mask. Defaults to 0 (off).
-# 
+#
 # NOTES
 #     You can also use flags syntax for POSITIONAL ARGUMENTS
 ```
 
 ```bash
 # Process rgb imagery directory with default parameters
 glint-mask-v*.*.* rgb_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/
 
 # Process PhaseONE camera imagery with image bands split over multiple files
 glint-mask-v*.*.* aco_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/
 
 # Process DJI P4MS imagery
 glint-mask-v*.*.* p4ms_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/
 
-# Process Micasense RedEdge imagery 
+# Process Micasense RedEdge imagery
 glint-mask-v*.*.* micasense_threshold /path/to/dir/with/images/ /path/to/out_masks/dir/
 ```
 
 ### Python package
 Installing the PyPi package allows integrating the mask generation workflow into existing python scripts with ease.
 
 ```python
```

#### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: glint-mask-tools Version: 3.0.4 Summary: Create
+Metadata-Version: 2.1 Name: glint-mask-tools Version: 3.1.0 Summary: Create
 masks for specular reflection in UAV and aerial imagery Home-page: https://
 github.com/HakaiInstitute/GlintMaskGenerator License: MIT Author: Taylor
-Denouden Author-email: taylor.denouden@hakai.org Requires-Python: >=3.8.1,<3.11
+Denouden Author-email: taylor.denouden@hakai.org Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Pillow
-(>=9.3.0,<9.4.0) Requires-Dist: fire (>=0.4.0,<0.5.0) Requires-Dist: loguru
-(>=0.6.0,<0.7.0) Requires-Dist: numpy (>=1.23.5,<1.24.0) Requires-Dist: pyqt6
-(>=6.4.0,<7.0.0) Requires-Dist: scipy (>=1.9.3,<1.11.0) Requires-Dist: tqdm
-(>=4.64.1,<4.65.0) Project-URL: Repository, https://github.com/HakaiInstitute/
-GlintMaskGenerator Description-Content-Type: text/markdown # Glint Mask Tools
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Requires-Dist: Pillow (>=9.3.0,<9.4.0) Requires-
+Dist: fire (>=0.5.0,<0.6.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-
+Dist: numpy (>=1.25.1,<1.26.0) Requires-Dist: pyqt6 (>=6.4.0,<7.0.0) Requires-
+Dist: scipy (>=1.11.1,<1.12.0) Requires-Dist: tqdm (>=4.65.0,<4.66.0) Project-
+URL: Repository, https://github.com/HakaiInstitute/GlintMaskGenerator
+Description-Content-Type: text/markdown # Glint Mask Tools
 [Tests] [License:_MIT] [PyPI_version] [DOI]
 ## Description GlintMaskGenerator generates image masks for regions in RGB and
 multispectral image files that have high levels of specular reflection. These
 masks can be used in 3rd party structure-from-motion programs to replace these
 high glint regions with more useful data from adjacent, overlapping imagery. ##
 Installation 1. Go to the [releases page](https://github.com/HakaiInstitute/
 glint-mask-tools/releases) 2. Download the latest release file for your
```

