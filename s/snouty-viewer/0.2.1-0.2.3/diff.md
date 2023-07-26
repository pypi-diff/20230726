# Comparing `tmp/snouty_viewer-0.2.1.tar.gz` & `tmp/snouty_viewer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snouty_viewer-0.2.1.tar", last modified: Wed Mar  1 19:36:34 2023, max compression
+gzip compressed data, was "snouty_viewer-0.2.3.tar", last modified: Wed Jul 26 20:36:25 2023, max compression
```

## Comparing `snouty_viewer-0.2.1.tar` & `snouty_viewer-0.2.3.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 19:36:34.911015 snouty_viewer-0.2.1/
--rw-rw-rw-   0        0        0     1114 2022-08-03 18:36:50.000000 snouty_viewer-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      101 2022-08-03 18:36:50.000000 snouty_viewer-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6239 2023-03-01 19:36:34.911015 snouty_viewer-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4954 2023-02-28 00:35:30.000000 snouty_viewer-0.2.1/README.md
--rw-rw-rw-   0        0        0      192 2022-08-03 18:36:50.000000 snouty_viewer-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0     1642 2023-03-01 19:36:34.926645 snouty_viewer-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-01 19:36:34.718014 snouty_viewer-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-01 19:36:34.809110 snouty_viewer-0.2.1/src/snouty_viewer/
--rw-rw-rw-   0        0        0      149 2023-03-01 19:34:57.000000 snouty_viewer-0.2.1/src/snouty_viewer/__init__.py
--rw-rw-rw-   0        0        0      357 2023-02-22 23:25:37.000000 snouty_viewer-0.2.1/src/snouty_viewer/_reader.py
-drwxrwxrwx   0        0        0        0 2023-03-01 19:36:34.911015 snouty_viewer-0.2.1/src/snouty_viewer/_tests/
--rw-rw-rw-   0        0        0        0 2022-08-03 18:36:50.000000 snouty_viewer-0.2.1/src/snouty_viewer/_tests/__init__.py
--rw-rw-rw-   0        0        0     8226 2022-08-31 22:44:42.000000 snouty_viewer-0.2.1/src/snouty_viewer/_tests/test_reader.py
--rw-rw-rw-   0        0        0     1286 2022-09-01 00:10:24.000000 snouty_viewer-0.2.1/src/snouty_viewer/_tests/test_widget.py
--rw-rw-rw-   0        0        0     6467 2023-02-23 00:05:05.000000 snouty_viewer-0.2.1/src/snouty_viewer/_widget.py
--rw-rw-rw-   0        0        0     1622 2023-02-28 00:28:17.000000 snouty_viewer-0.2.1/src/snouty_viewer/_writer.py
--rw-rw-rw-   0        0        0     3095 2023-02-22 23:45:52.000000 snouty_viewer-0.2.1/src/snouty_viewer/im_loader.py
--rw-rw-rw-   0        0        0     1127 2023-02-22 22:54:30.000000 snouty_viewer-0.2.1/src/snouty_viewer/napari.yaml
-drwxrwxrwx   0        0        0        0 2023-03-01 19:36:34.877925 snouty_viewer-0.2.1/src/snouty_viewer.egg-info/
--rw-rw-rw-   0        0        0     6239 2023-03-01 19:36:34.000000 snouty_viewer-0.2.1/src/snouty_viewer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-03-01 19:36:34.000000 snouty_viewer-0.2.1/src/snouty_viewer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 19:36:34.000000 snouty_viewer-0.2.1/src/snouty_viewer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-03-01 19:36:34.000000 snouty_viewer-0.2.1/src/snouty_viewer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-03-01 19:36:34.000000 snouty_viewer-0.2.1/src/snouty_viewer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-03-01 19:36:34.000000 snouty_viewer-0.2.1/src/snouty_viewer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 20:36:25.121017 snouty_viewer-0.2.3/
+-rw-rw-rw-   0        0        0     1114 2022-08-03 18:36:50.000000 snouty_viewer-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      101 2022-08-03 18:36:50.000000 snouty_viewer-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     6239 2023-07-26 20:36:25.121017 snouty_viewer-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4954 2023-02-28 00:35:30.000000 snouty_viewer-0.2.3/README.md
+-rw-rw-rw-   0        0        0      192 2022-08-03 18:36:50.000000 snouty_viewer-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1642 2023-07-26 20:36:25.136644 snouty_viewer-0.2.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 20:36:24.886639 snouty_viewer-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 20:36:24.917890 snouty_viewer-0.2.3/src/scripts/
+-rw-rw-rw-   0        0        0        0 2023-07-25 21:56:56.000000 snouty_viewer-0.2.3/src/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2869 2023-07-26 20:27:35.000000 snouty_viewer-0.2.3/src/scripts/split_positions.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:36:25.011646 snouty_viewer-0.2.3/src/snouty_viewer/
+-rw-rw-rw-   0        0        0      149 2023-03-01 19:34:57.000000 snouty_viewer-0.2.3/src/snouty_viewer/__init__.py
+-rw-rw-rw-   0        0        0      357 2023-02-22 23:25:37.000000 snouty_viewer-0.2.3/src/snouty_viewer/_reader.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:36:25.105390 snouty_viewer-0.2.3/src/snouty_viewer/_tests/
+-rw-rw-rw-   0        0        0        0 2022-08-03 18:36:50.000000 snouty_viewer-0.2.3/src/snouty_viewer/_tests/__init__.py
+-rw-rw-rw-   0        0        0     8226 2022-08-31 22:44:42.000000 snouty_viewer-0.2.3/src/snouty_viewer/_tests/test_reader.py
+-rw-rw-rw-   0        0        0     1286 2022-09-01 00:10:24.000000 snouty_viewer-0.2.3/src/snouty_viewer/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     9175 2023-07-25 21:54:24.000000 snouty_viewer-0.2.3/src/snouty_viewer/_widget.py
+-rw-rw-rw-   0        0        0     1622 2023-02-28 00:28:17.000000 snouty_viewer-0.2.3/src/snouty_viewer/_writer.py
+-rw-rw-rw-   0        0        0     5075 2023-07-26 20:26:02.000000 snouty_viewer-0.2.3/src/snouty_viewer/im_loader.py
+-rw-rw-rw-   0        0        0     1127 2023-02-22 22:54:30.000000 snouty_viewer-0.2.3/src/snouty_viewer/napari.yaml
+-rw-rw-rw-   0        0        0     6238 2023-07-25 21:54:24.000000 snouty_viewer-0.2.3/src/snouty_viewer/vol_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:36:25.074141 snouty_viewer-0.2.3/src/snouty_viewer.egg-info/
+-rw-rw-rw-   0        0        0     6239 2023-07-26 20:36:24.000000 snouty_viewer-0.2.3/src/snouty_viewer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      684 2023-07-26 20:36:24.000000 snouty_viewer-0.2.3/src/snouty_viewer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 20:36:24.000000 snouty_viewer-0.2.3/src/snouty_viewer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-26 20:36:24.000000 snouty_viewer-0.2.3/src/snouty_viewer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-07-26 20:36:24.000000 snouty_viewer-0.2.3/src/snouty_viewer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 20:36:24.000000 snouty_viewer-0.2.3/src/snouty_viewer.egg-info/top_level.txt
```

### Comparing `snouty_viewer-0.2.1/LICENSE` & `snouty_viewer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.1/PKG-INFO` & `snouty_viewer-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snouty_viewer
-Version: 0.2.1
+Version: 0.2.3
 Summary: A plugin to visualize, deskew, and combine Snouty data.
 Home-page: https://github.com/aelefebv/snouty-viewer
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aelefebv/snouty-viewer/issues
 Project-URL: Documentation, https://github.com/aelefebv/snouty-viewer#README.md
```

### Comparing `snouty_viewer-0.2.1/README.md` & `snouty_viewer-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.1/setup.cfg` & `snouty_viewer-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2073 6e6f 7574 795f 7669 6577 6572   = snouty_viewer
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 322e  ..version = 0.2.
-00000030: 310d 0a64 6573 6372 6970 7469 6f6e 203d  1..description =
+00000030: 330d 0a64 6573 6372 6970 7469 6f6e 203d  3..description =
 00000040: 2041 2070 6c75 6769 6e20 746f 2076 6973   A plugin to vis
 00000050: 7561 6c69 7a65 2c20 6465 736b 6577 2c20  ualize, deskew, 
 00000060: 616e 6420 636f 6d62 696e 6520 536e 6f75  and combine Snou
 00000070: 7479 2064 6174 612e 0d0a 6c6f 6e67 5f64  ty data...long_d
 00000080: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
 00000090: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
 000000a0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
```

### Comparing `snouty_viewer-0.2.1/src/snouty_viewer/_tests/test_reader.py` & `snouty_viewer-0.2.3/src/snouty_viewer/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.1/src/snouty_viewer/_tests/test_widget.py` & `snouty_viewer-0.2.3/src/snouty_viewer/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.1/src/snouty_viewer/_widget.py` & `snouty_viewer-0.2.3/src/snouty_viewer/_widget.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,81 +3,125 @@
 from typing import List, Union
 
 import napari.layers
 import napari.types
 import numpy as np
 from magicgui import magic_factory
 
-from snouty_viewer._writer import write_single_image
-from snouty_viewer.im_loader import ImPathInfo, load_full
+from snouty_viewer.im_loader import (
+    ImPathInfo,
+    allocate_memory_return_memmap,
+    load_full,
+)
 
 
 class PseudoImage:
     def __init__(self, im_tuple: tuple):
         self.data = im_tuple[0]
         self.metadata = im_tuple[1]["metadata"]
         self.name = im_tuple[1]["name"]
         self.dtype = im_tuple[0].dtype
 
 
 class ImInfo:
-    def __init__(self, im):
+    def __init__(self, im, im_shape=None):
+        if im_shape is None:
+            im_shape = im.shape
         (
             self.num_t,
             self.num_c,
             self.num_z,
             self.num_y,
             self.num_x,
-        ) = im.data.shape
+        ) = im_shape
         self.scan_step_size_px = int(
             im.metadata["snouty_metadata"]["scan_step_size_px"]
         )
         self.max_deshear_shift = int(
             np.rint(self.scan_step_size_px * (self.num_z - 1))
         )
-        self.im_desheared = np.zeros(
-            (
-                self.num_t,
-                self.num_c,
-                self.num_z,
-                self.num_y + self.max_deshear_shift,
-                self.num_x,
-            ),
-            im.dtype,
+        self.im_desheared_shape = (
+            self.num_t,
+            self.num_c,
+            self.num_z,
+            self.num_y + self.max_deshear_shift,
+            self.num_x,
         )
+        self.im_desheared = None
+        # get desheared image memmap
+        # self.im_desheared = np.zeros(
+        #     (
+        #         self.num_t,
+        #         self.num_c,
+        #         self.num_z,
+        #         self.num_y + self.max_deshear_shift,
+        #         self.num_x,
+        #     ),
+        #     im.dtype,
+        # )
         self.px_size = float(im.metadata["snouty_metadata"]["sample_px_um"])
         self.z_px_size = self.px_size * float(
             im.metadata["snouty_metadata"]["voxel_aspect_ratio"]
         )
         self.scale = (self.z_px_size, self.px_size, self.px_size)
         self.dtype = im.dtype
         self.metadata = im.metadata
         self.data = im.data
         self.wavelengths = ast.literal_eval(
             im.metadata["snouty_metadata"]["channels_per_slice"]
         )
         self.name = im.name
         self.displayed_images = []
 
+    # def _allocate_memory(self,
+    #                      path_im: str,
+    #                      dtype: Union[Type, str] = 'float', data = None,
+    #                      shape: tuple = None,
+    #                      description: str = 'No description.'):
+    #     axes = 'TCZYX'
+    #     if shape is None:
+    #
+    #
+    #     if data is None:
+    #         assert shape is not None
+    #         tifffile.imwrite(
+    #             path_im, shape=shape, dtype=dtype, bigtiff=True,
+    #             metadata={"axes": axes}
+    #         )
+    #     else:
+    #         tifffile.imwrite(
+    #             path_im, data, bigtiff=True, metadata={"axes": axes}
+    #         )
+    #     ome_xml = tifffile.tiffcomment(path_im)
+    #     ome = ome_types.from_xml(ome_xml, parser="lxml")
+    #     ome.images[0].pixels.physical_size_x = self.dim_sizes['X']
+    #     ome.images[0].pixels.physical_size_y = self.dim_sizes['Y']
+    #     ome.images[0].pixels.physical_size_z = self.dim_sizes['Z']
+    #     ome.images[0].pixels.time_increment = self.dim_sizes['T']
+    #     ome.images[0].description = description
+    #     ome.images[0].pixels.type = dtype
+    # note: numpy uses 8 bits as smallest, so 'bit' type does nothing for bool.
+    #     ome_xml = ome.to_xml()
+    #     tifffile.tiffcomment(path_im, ome_xml)
+
     def _deshear_channel(self, ch_num):
-        desheard_ch = np.zeros(
-            (
-                self.num_t,
-                1,
-                self.num_z,
-                self.num_y + self.max_deshear_shift,
-                self.num_x,
-            ),
-            self.dtype,
-        )
-        for z in range(self.num_z):
-            deshear_shift = int(np.rint(z * self.scan_step_size_px))
-            desheard_ch[
-                :, 0, z, deshear_shift : (deshear_shift + self.num_y), :
-            ] = self.data[:, ch_num, z, :, :]
+        if self.num_c == 1:
+            desheard_ch = self.im_desheared
+            for z in range(self.num_z):
+                deshear_shift = int(np.rint(z * self.scan_step_size_px))
+                desheard_ch[
+                    :, z, deshear_shift : (deshear_shift + self.num_y), :
+                ] = self.data[:, z, :, :]
+        else:
+            desheard_ch = self.im_desheared[:, ch_num, :, :, :]
+            for z in range(self.num_z):
+                deshear_shift = int(np.rint(z * self.scan_step_size_px))
+                desheard_ch[
+                    :, z, deshear_shift : (deshear_shift + self.num_y), :
+                ] = self.data[:, ch_num, z, :, :]
         return desheard_ch
 
     def _display_image(
         self, im, wavelength=0, color="gray", multichannel=False
     ):
         if multichannel:
             self.displayed_images.insert(
@@ -107,16 +151,21 @@
                     "image",
                 )
             )
         return None
 
     def deshear_all_channels(self, batch=False, show_multi=False):
         for ch in range(self.num_c):
-            wavelength = int(self.wavelengths[ch])
-            if wavelength < 430:
+            try:
+                wavelength = int(self.wavelengths[ch])
+            except ValueError:
+                wavelength = 0
+            if wavelength == 0:
+                color = "gray"
+            elif wavelength < 430:
                 color = "bop purple"
             elif wavelength < 480:
                 color = "blue"
             elif wavelength < 500:
                 color = "cyan"
             elif wavelength < 570:
                 color = "green"
@@ -126,16 +175,16 @@
                 color = "bop orange"
             elif wavelength < 700:
                 color = "red"
             else:
                 color = "magenta"
             ch_desheared = self._deshear_channel(ch)
             if self.num_c > 1:
-                self.im_desheared[:, ch, ...] = ch_desheared[:, 0, ...]
-                ch_desheared = ch_desheared[:, 0, ...]
+                self.im_desheared[:, ch, ...] = ch_desheared[:, ...]
+                ch_desheared = ch_desheared[:, ...]
             else:
                 self.im_desheared = ch_desheared
             if not batch:
                 self._display_image(ch_desheared, wavelength, color)
 
         if (self.num_c > 1 and not batch) or show_multi:
             self._display_image(self.im_desheared, multichannel=True)
@@ -158,32 +207,48 @@
         )
     ]
     return snouty_subdirectories
 
 
 @magic_factory(call_button="Deskew and save")
 def batch_deskew_and_save(
-    path: str, show_deskewed_ims: bool = False, auto_save: bool = True
+    path_in: str,
+    path_out: str = "",
+    show_deskewed_ims: bool = False,
+    auto_save: bool = True,
 ) -> Union[List[napari.types.LayerDataTuple], None]:
-    snouty_dirs = list_subdirectories(path)
+    snouty_dirs = list_subdirectories(path_in)
     tuple_list = []
     for snouty_dir in snouty_dirs:
+        if path_out == "":
+            path_out = snouty_dir
         im_path_info = ImPathInfo(snouty_dir)
-        loaded_im = PseudoImage(load_full(im_path_info)[0])
-        im_info = ImInfo(loaded_im)
+        skewed_memmap = PseudoImage(load_full(im_path_info, path_out)[0])
+        im_info = ImInfo(skewed_memmap, im_path_info.im_shape)
+        name = im_path_info.path.rsplit(os.sep)[-1]
+        # skewed_memmap_path = os.path.join(path_out, f"skewed-{name}.ome.tif")
+        save_path = os.path.join(path_out, f"deskewed-{name}.ome.tif")
+        deskewed_memmap = allocate_memory_return_memmap(
+            "TCZYX",
+            im_info.im_desheared_shape,
+            im_path_info.metadata,
+            save_path,
+            im_info.dtype,
+        )
+        im_info.im_desheared = deskewed_memmap
         im_info.deshear_all_channels(batch=True, show_multi=show_deskewed_ims)
         if show_deskewed_ims:
             tuple_list.append(im_info.displayed_images[0])
-        if auto_save:
-            save_path = os.path.join(
-                snouty_dir, f"deskewed-{im_info.name}.ome.tif"
-            )
-            attributes = {"metadata": im_info.metadata}
-            write_single_image(save_path, im_info.im_desheared, attributes)
-
+        # if auto_save:
+        #     save_path = os.path.join(
+        #         path_out, f"deskewed-{im_info.name}.ome.tif"
+        #     )
+        #     attributes = {"metadata": im_info.metadata}
+        #     write_single_image(save_path, im_info.im_desheared, attributes)
+        # os.remove(skewed_memmap_path)
     if show_deskewed_ims:
         return tuple_list
     return None
 
 
 @magic_factory(call_button="Deskew")
 def native_view(
```

### Comparing `snouty_viewer-0.2.1/src/snouty_viewer/_writer.py` & `snouty_viewer-0.2.3/src/snouty_viewer/_writer.py`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.1/src/snouty_viewer/napari.yaml` & `snouty_viewer-0.2.3/src/snouty_viewer/napari.yaml`

 * *Files identical despite different names*

### Comparing `snouty_viewer-0.2.1/src/snouty_viewer.egg-info/PKG-INFO` & `snouty_viewer-0.2.3/src/snouty_viewer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snouty-viewer
-Version: 0.2.1
+Version: 0.2.3
 Summary: A plugin to visualize, deskew, and combine Snouty data.
 Home-page: https://github.com/aelefebv/snouty-viewer
 Author: Austin E. Y. T. Lefebvre
 Author-email: austin.e.lefebvre@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/aelefebv/snouty-viewer/issues
 Project-URL: Documentation, https://github.com/aelefebv/snouty-viewer#README.md
```

### Comparing `snouty_viewer-0.2.1/src/snouty_viewer.egg-info/SOURCES.txt` & `snouty_viewer-0.2.3/src/snouty_viewer.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
+src/scripts/__init__.py
+src/scripts/split_positions.py
 src/snouty_viewer/__init__.py
 src/snouty_viewer/_reader.py
 src/snouty_viewer/_widget.py
 src/snouty_viewer/_writer.py
 src/snouty_viewer/im_loader.py
 src/snouty_viewer/napari.yaml
+src/snouty_viewer/vol_loader.py
 src/snouty_viewer.egg-info/PKG-INFO
 src/snouty_viewer.egg-info/SOURCES.txt
 src/snouty_viewer.egg-info/dependency_links.txt
 src/snouty_viewer.egg-info/entry_points.txt
 src/snouty_viewer.egg-info/requires.txt
 src/snouty_viewer.egg-info/top_level.txt
 src/snouty_viewer/_tests/__init__.py
```

