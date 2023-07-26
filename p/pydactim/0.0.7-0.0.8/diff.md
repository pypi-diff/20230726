# Comparing `tmp/pydactim-0.0.7.tar.gz` & `tmp/pydactim-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pydactim-0.0.7.tar", last modified: Wed Jul 26 09:26:05 2023, max compression
+gzip compressed data, was "dist\pydactim-0.0.8.tar", last modified: Wed Jul 26 12:04:20 2023, max compression
```

## Comparing `pydactim-0.0.7.tar` & `pydactim-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:05.420567 pydactim-0.0.7/
--rw-rw-rw-   0        0        0      384 2023-07-26 09:26:05.420567 pydactim-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1868 2023-05-05 09:52:11.000000 pydactim-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:05.400567 pydactim-0.0.7/pydactim/
--rw-rw-rw-   0        0        0      161 2023-07-26 09:25:32.000000 pydactim-0.0.7/pydactim/__init__.py
--rw-rw-rw-   0        0        0     4245 2023-05-04 09:31:52.000000 pydactim-0.0.7/pydactim/anonymization.py
--rw-rw-rw-   0        0        0    30210 2023-06-19 09:22:31.000000 pydactim-0.0.7/pydactim/brain_extraction.py
--rw-rw-rw-   0        0        0      927 2023-07-26 08:11:37.000000 pydactim-0.0.7/pydactim/computation.py
--rw-rw-rw-   0        0        0     3935 2023-05-03 14:18:41.000000 pydactim-0.0.7/pydactim/conversion.py
--rw-rw-rw-   0        0        0     1744 2023-07-26 07:37:37.000000 pydactim-0.0.7/pydactim/data.py
--rw-rw-rw-   0        0        0    24158 2023-07-26 07:52:07.000000 pydactim-0.0.7/pydactim/new_transformation.py
--rw-rw-rw-   0        0        0     2411 2023-07-26 09:22:09.000000 pydactim-0.0.7/pydactim/sorting.py
--rw-rw-rw-   0        0        0     3100 2023-07-26 09:22:13.000000 pydactim-0.0.7/pydactim/spectroscopy.py
--rw-rw-rw-   0        0        0    23291 2023-07-26 07:56:30.000000 pydactim-0.0.7/pydactim/transformation.py
--rw-rw-rw-   0        0        0      996 2022-12-12 13:23:53.000000 pydactim-0.0.7/pydactim/utils.py
--rw-rw-rw-   0        0        0     6361 2023-07-26 09:22:21.000000 pydactim-0.0.7/pydactim/visualization.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:26:05.413568 pydactim-0.0.7/pydactim.egg-info/
--rw-rw-rw-   0        0        0      384 2023-07-26 09:26:05.000000 pydactim-0.0.7/pydactim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-07-26 09:26:05.000000 pydactim-0.0.7/pydactim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:26:05.000000 pydactim-0.0.7/pydactim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-07-26 09:26:05.000000 pydactim-0.0.7/pydactim.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 09:26:05.000000 pydactim-0.0.7/pydactim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      317 2023-07-26 08:45:46.000000 pydactim-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      174 2023-07-26 09:26:05.421567 pydactim-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      968 2023-07-26 09:26:00.000000 pydactim-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:04:20.334938 pydactim-0.0.8/
+-rw-rw-rw-   0        0        0      384 2023-07-26 12:04:20.335938 pydactim-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1868 2023-05-05 09:52:11.000000 pydactim-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 12:04:20.316938 pydactim-0.0.8/pydactim/
+-rw-rw-rw-   0        0        0      521 2023-07-26 10:50:30.000000 pydactim-0.0.8/pydactim/__init__.py
+-rw-rw-rw-   0        0        0     4245 2023-05-04 09:31:52.000000 pydactim-0.0.8/pydactim/anonymization.py
+-rw-rw-rw-   0        0        0    30210 2023-06-19 09:22:31.000000 pydactim-0.0.8/pydactim/brain_extraction.py
+-rw-rw-rw-   0        0        0      927 2023-07-26 08:11:37.000000 pydactim-0.0.8/pydactim/computation.py
+-rw-rw-rw-   0        0        0     3935 2023-05-03 14:18:41.000000 pydactim-0.0.8/pydactim/conversion.py
+-rw-rw-rw-   0        0        0     1744 2023-07-26 07:37:37.000000 pydactim-0.0.8/pydactim/data.py
+-rw-rw-rw-   0        0        0    24158 2023-07-26 07:52:07.000000 pydactim-0.0.8/pydactim/new_transformation.py
+-rw-rw-rw-   0        0        0     4554 2023-07-26 12:02:51.000000 pydactim-0.0.8/pydactim/preprocessing.py
+-rw-rw-rw-   0        0        0     2411 2023-07-26 09:22:09.000000 pydactim-0.0.8/pydactim/sorting.py
+-rw-rw-rw-   0        0        0     3100 2023-07-26 09:22:13.000000 pydactim-0.0.8/pydactim/spectroscopy.py
+-rw-rw-rw-   0        0        0    23509 2023-07-26 09:51:17.000000 pydactim-0.0.8/pydactim/transformation.py
+-rw-rw-rw-   0        0        0     3101 2023-07-26 11:51:44.000000 pydactim-0.0.8/pydactim/utils.py
+-rw-rw-rw-   0        0        0     6334 2023-07-26 09:33:51.000000 pydactim-0.0.8/pydactim/visualization.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:04:20.333938 pydactim-0.0.8/pydactim.egg-info/
+-rw-rw-rw-   0        0        0      384 2023-07-26 12:04:20.000000 pydactim-0.0.8/pydactim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      515 2023-07-26 12:04:20.000000 pydactim-0.0.8/pydactim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:04:20.000000 pydactim-0.0.8/pydactim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2023-07-26 12:04:20.000000 pydactim-0.0.8/pydactim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 12:04:20.000000 pydactim-0.0.8/pydactim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      317 2023-07-26 08:45:46.000000 pydactim-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      174 2023-07-26 12:04:20.336938 pydactim-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      986 2023-07-26 12:03:53.000000 pydactim-0.0.8/setup.py
```

### Comparing `pydactim-0.0.7/README.md` & `pydactim-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.7/pydactim/anonymization.py` & `pydactim-0.0.8/pydactim/anonymization.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.7/pydactim/brain_extraction.py` & `pydactim-0.0.8/pydactim/brain_extraction.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.7/pydactim/computation.py` & `pydactim-0.0.8/pydactim/computation.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.7/pydactim/conversion.py` & `pydactim-0.0.8/pydactim/conversion.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.7/pydactim/data.py` & `pydactim-0.0.8/pydactim/data.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.7/pydactim/new_transformation.py` & `pydactim-0.0.8/pydactim/new_transformation.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.7/pydactim/sorting.py` & `pydactim-0.0.8/pydactim/sorting.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.7/pydactim/spectroscopy.py` & `pydactim-0.0.8/pydactim/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `pydactim-0.0.7/pydactim/transformation.py` & `pydactim-0.0.8/pydactim/transformation.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import nibabel as nib
 import numpy as np
 from skimage import morphology
 import matplotlib.pyplot as plt
 from .brain_extraction import run_hd_bet
 from dipy.segment.tissue import TissueClassifierHMRF
 import itk
+from numba import jit
 
 def n4_bias_field_correction(input_path, mask=False, force=True, suffix="corrected"):
     """ Correct the bias field correction.
 
     Parameters
     ----------
     input_path : str
@@ -318,46 +319,54 @@
     output_path = input_path.replace(".nii.gz", "_" + suffix + ".nii.gz")
     print(f"INFO - Saving generated image at\n\t{output_path :}")
 
     nib.save(nib.Nifti1Image(sub, img.affine), output_path)
 
     return output_path
 
-def variance(input_path, offset=9, force=True, suffix="var"):
-    """ Amplify borders by creating a variance map.
+def susan(input_path, offset=3, force=True, suffix="susan"):
+    """ Amplify borders by creating a susan variance map.
+    Based on https://users.fmrib.ox.ac.uk/~steve/susan/susan/node2.html
 
     Parameters
     ----------
     input_path : str
-        The image that will be used to create the variance map
+        The image that will be used to create the susan variance map
 
     offset : int
-        offset of the variance, the highest it is, the strongest the borders
+        Size of the kernel
 
     suffix : str
         Nifti file suffixe for the new generated image
     """
     output_path = input_path.replace(".nii.gz", "_" + suffix + ".nii.gz")
     if os.path.exists(output_path) and not force:
-        print(f"INFO - Variance map already computed for\n\t{input_path :}")
+        print(f"INFO - Susan variance map already computed for\n\t{input_path :}")
         return output_path
 
-    print(f"INFO - Starting variance map creation for\n\t{input_path :}")
+    print(f"INFO - Starting Susan variance map creation for\n\t{input_path :}")
     img = nib.load(input_path)
     img_data = img.get_fdata()
-    var_data = np.zeros_like(img_data)
-    for x in range(img_data.shape[0]):
-        for y in range(img_data.shape[1]):
-            for z in range(img_data.shape[2]):
-                if img_data[x,y,z] != 0:
-                    variance = np.var(img_data[x-offset//2+1:x+offset//2+1,y-offset//2+1:y+offset//2+1,z-offset//2+1:z+offset//2+1])
-                    var_data[x,y,z] = variance
+
+    @jit
+    def susan(img_data):
+        susan_data = np.zeros_like(img_data)
+        for x in range(img_data.shape[0]):
+            for y in range(img_data.shape[1]):
+                for z in range(img_data.shape[2]):
+                        values = img_data[x:x + offset, y:y + offset, z:z + offset]
+                        mean = np.mean(values)
+                        var = np.var(values)
+                        susan_data[x,y,z] = np.abs(var - mean**2)
+        return susan_data
     
+    susan_data = susan(img_data)
+
     print(f"INFO - Saving generated image at\n\t{output_path :}")
-    nib.save(nib.Nifti1Image(var_data, img.affine), output_path)
+    nib.save(nib.Nifti1Image(susan_data, img.affine), output_path)
     
     return output_path
 
 def normalize(input_path, force=True, suffix="minmax"):
     """ Normalize image between 0 and 1.
 
     Parameters
@@ -480,15 +489,15 @@
 
     cropped_mri_image = mri_image[crop[0]:crop[1], crop[2]:crop[3], crop[4]:crop[5]]
     nib.save(nib.Nifti1Image(cropped_mri_image, mri.affine), output_path)
 
     print(f"INFO - Saving generated image at\n\t{output_path :}")
     return output_path
 
-def copy_affine(input_ref_path, input_path, force=True, suffix="aff"):
+def copy_affine(input_ref_path, input_path, force=True, suffix="affined"):
     """ Match the histogram of two images.
 
     Parameters
     ----------
     input_ref_path : str
         The image used as reference
 
@@ -567,15 +576,15 @@
     if mask == True:
         print(f"\n\t{mask_path :}")
         nib.save(nib.Nifti1Image(mask_out, img.affine), mask_path)
         return output_path, mask_path
     else:
         return output_path
 
-def remove_small_object(input_path, min_size, force=False, suffix="opened"):
+def remove_small_object(input_path, min_size, force=False, suffix="filtered"):
     """ Remove small objects above a minimum size
 
     Parameters
     ----------
     input_path : str
         Nifti file path
```

### Comparing `pydactim-0.0.7/pydactim/visualization.py` & `pydactim-0.0.8/pydactim/visualization.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
         title = get_name_of_path(os.path.basename(images[0]).replace(".nii.gz", ""))
         subject.add_image(tio.ScalarImage(images[0]), title)
 
     subject.remove_image("temp")
     subject.plot()
 
 def plot(input_data, pixdim=None, slice=None, save=None):
-    """ Plot a nifti file or an array.
-        If using this function with array, make sure to precise the pixdim value or the data might have default pixdim value [1,1,1]
+    """ Plot image from a nifti file path or from an array.
+        If using this function with an array, make sure to specify the pixdim value.
 
         Parameters
         ----------
         input_data : str/array
             Nifti file path or array that will be plotted
 
         pixdim : list, optional
```

### Comparing `pydactim-0.0.7/setup.py` & `pydactim-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # from sphinx.setup_command import BuildDoc
 # cmdclass = {'build_sphinx': BuildDoc}
 
 from setuptools import setup, find_packages
 
 setup(name='pydactim',
       python_requires='>=3.7',
-      version='0.0.7',
+      version='0.0.8',
       packages=find_packages(),
       install_requires=[
         "torch>=1.13.1",
         "torchio>=0.18.86",
         "SimpleITK",
         "numpy",
         "nibabel",
         "matplotlib",
         "pydicom>=2.3.1",
         "dicom2nifti",
         "itk-elastix==0.17.1",
         "dipy>=1.7.0",
-        "scikit-image"
+        "scikit-image",
+        "numba"
       ],
       classifiers=[
           'Intended Audience :: Science/Research',
           'Programming Language :: Python',
           'Topic :: Scientific/Engineering',
           'Operating System :: Microsoft :: Windows :: Windows 10'
       ],
```

