# Comparing `tmp/bnpm-0.2.3.tar.gz` & `tmp/bnpm-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnpm-0.2.3.tar", last modified: Tue Jul 11 20:03:18 2023, max compression
+gzip compressed data, was "bnpm-0.2.4.tar", last modified: Wed Jul 26 03:45:49 2023, max compression
```

## Comparing `bnpm-0.2.3.tar` & `bnpm-0.2.4.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 20:03:18.531739 bnpm-0.2.3/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2022-09-13 02:36:53.000000 bnpm-0.2.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       24 2023-07-11 20:02:02.000000 bnpm-0.2.3/MANIFEST.in
--rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-11 20:03:18.531867 bnpm-0.2.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     2971 2023-06-16 05:27:34.000000 bnpm-0.2.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 20:03:18.530067 bnpm-0.2.3/bnpm/
--rwxrwxrwx   0 root         (0) root         (0)      907 2023-07-11 20:02:50.000000 bnpm-0.2.3/bnpm/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    37134 2023-05-18 20:21:08.000000 bnpm-0.2.3/bnpm/ca2p_preprocessing.py
--rwxrwxrwx   0 root         (0) root         (0)     4603 2023-06-25 23:47:42.000000 bnpm-0.2.3/bnpm/classification.py
--rwxrwxrwx   0 root         (0) root         (0)    49222 2023-06-17 04:47:40.000000 bnpm-0.2.3/bnpm/clustering.py
--rwxrwxrwx   0 root         (0) root         (0)    10138 2023-06-28 13:37:49.000000 bnpm-0.2.3/bnpm/container_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     4477 2021-12-28 22:22:14.000000 bnpm-0.2.3/bnpm/cross_validation.py
--rwxrwxrwx   0 root         (0) root         (0)      940 2021-12-28 19:03:39.000000 bnpm-0.2.3/bnpm/cupy_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    16674 2023-03-19 21:48:35.000000 bnpm-0.2.3/bnpm/decomposition.py
--rwxrwxrwx   0 root         (0) root         (0)     5310 2021-12-28 19:04:57.000000 bnpm-0.2.3/bnpm/dtw.py
--rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-15 17:45:20.000000 bnpm-0.2.3/bnpm/email_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    19171 2023-06-08 15:16:54.000000 bnpm-0.2.3/bnpm/featurization.py
--rwxrwxrwx   0 root         (0) root         (0)    23399 2023-06-29 05:55:34.000000 bnpm-0.2.3/bnpm/file_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    11769 2023-06-10 18:47:53.000000 bnpm-0.2.3/bnpm/h5_handling.py
--rwxrwxrwx   0 root         (0) root         (0)    57594 2023-07-01 01:57:59.000000 bnpm-0.2.3/bnpm/image_processing.py
--rwxrwxrwx   0 root         (0) root         (0)    23809 2023-07-11 01:29:59.000000 bnpm-0.2.3/bnpm/indexing.py
--rwxrwxrwx   0 root         (0) root         (0)    17856 2023-03-05 00:44:40.000000 bnpm-0.2.3/bnpm/linear_regression.py
--rwxrwxrwx   0 root         (0) root         (0)     8317 2023-04-21 04:21:03.000000 bnpm-0.2.3/bnpm/math_functions.py
--rwxrwxrwx   0 root         (0) root         (0)     6202 2023-06-17 04:51:49.000000 bnpm-0.2.3/bnpm/misc.py
--rwxrwxrwx   0 root         (0) root         (0)    10034 2023-06-24 16:25:12.000000 bnpm-0.2.3/bnpm/optimization.py
--rwxrwxrwx   0 root         (0) root         (0)     6922 2023-04-28 21:19:30.000000 bnpm-0.2.3/bnpm/other_peoples_code.py
--rwxrwxrwx   0 root         (0) root         (0)     4442 2023-04-29 05:04:13.000000 bnpm-0.2.3/bnpm/parallel_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     6370 2022-10-27 16:16:53.000000 bnpm-0.2.3/bnpm/path_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    40543 2023-07-11 00:22:09.000000 bnpm-0.2.3/bnpm/plotting_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     9811 2023-05-18 20:31:06.000000 bnpm-0.2.3/bnpm/resource_tracking.py
--rwxrwxrwx   0 root         (0) root         (0)    34760 2023-07-11 19:35:57.000000 bnpm-0.2.3/bnpm/server.py
--rwxrwxrwx   0 root         (0) root         (0)    31408 2023-07-11 01:31:23.000000 bnpm-0.2.3/bnpm/similarity.py
--rwxrwxrwx   0 root         (0) root         (0)    22632 2023-06-17 04:28:34.000000 bnpm-0.2.3/bnpm/spectral.py
--rwxrwxrwx   0 root         (0) root         (0)     1130 2023-05-18 04:27:38.000000 bnpm-0.2.3/bnpm/stats.py
--rwxrwxrwx   0 root         (0) root         (0)    35757 2023-06-17 04:42:40.000000 bnpm-0.2.3/bnpm/timeSeries.py
--rwxrwxrwx   0 root         (0) root         (0)    23576 2023-07-06 21:06:01.000000 bnpm-0.2.3/bnpm/torch_helpers.py
--rwxrwxrwx   0 root         (0) root         (0)    50036 2023-06-16 03:39:42.000000 bnpm-0.2.3/bnpm/video.py
--rwxrwxrwx   0 root         (0) root         (0)     3338 2021-12-28 19:07:58.000000 bnpm-0.2.3/bnpm/welford_moving.py
--rwxrwxrwx   0 root         (0) root         (0)     4882 2021-05-05 20:10:58.000000 bnpm-0.2.3/bnpm/welford_moving_2D.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-11 20:03:18.531503 bnpm-0.2.3/bnpm.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-11 20:03:18.000000 bnpm-0.2.3/bnpm.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      899 2023-07-11 20:03:18.000000 bnpm-0.2.3/bnpm.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-11 20:03:18.000000 bnpm-0.2.3/bnpm.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      326 2023-07-11 20:03:18.000000 bnpm-0.2.3/bnpm.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)        5 2023-07-11 20:03:18.000000 bnpm-0.2.3/bnpm.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      349 2023-06-10 00:46:32.000000 bnpm-0.2.3/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-07-11 20:03:18.532257 bnpm-0.2.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2954 2023-07-11 20:02:35.000000 bnpm-0.2.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 03:45:49.556581 bnpm-0.2.4/
+-rwxrwxrwx   0 root         (0) root         (0)     1068 2022-09-13 02:36:53.000000 bnpm-0.2.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       24 2023-07-11 20:02:02.000000 bnpm-0.2.4/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-26 03:45:49.556686 bnpm-0.2.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2971 2023-06-16 05:27:34.000000 bnpm-0.2.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 03:45:49.555116 bnpm-0.2.4/bnpm/
+-rwxrwxrwx   0 root         (0) root         (0)      941 2023-07-26 03:40:27.000000 bnpm-0.2.4/bnpm/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    37134 2023-05-18 20:21:08.000000 bnpm-0.2.4/bnpm/ca2p_preprocessing.py
+-rwxrwxrwx   0 root         (0) root         (0)     4603 2023-06-25 23:47:42.000000 bnpm-0.2.4/bnpm/classification.py
+-rwxrwxrwx   0 root         (0) root         (0)    49222 2023-06-17 04:47:40.000000 bnpm-0.2.4/bnpm/clustering.py
+-rwxrwxrwx   0 root         (0) root         (0)    10138 2023-06-28 13:37:49.000000 bnpm-0.2.4/bnpm/container_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     4477 2021-12-28 22:22:14.000000 bnpm-0.2.4/bnpm/cross_validation.py
+-rwxrwxrwx   0 root         (0) root         (0)      940 2021-12-28 19:03:39.000000 bnpm-0.2.4/bnpm/cupy_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    16674 2023-03-19 21:48:35.000000 bnpm-0.2.4/bnpm/decomposition.py
+-rwxrwxrwx   0 root         (0) root         (0)     5310 2021-12-28 19:04:57.000000 bnpm-0.2.4/bnpm/dtw.py
+-rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-15 17:45:20.000000 bnpm-0.2.4/bnpm/email_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    19171 2023-06-08 15:16:54.000000 bnpm-0.2.4/bnpm/featurization.py
+-rwxrwxrwx   0 root         (0) root         (0)    23452 2023-07-19 16:14:29.000000 bnpm-0.2.4/bnpm/file_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    11803 2023-07-24 22:33:58.000000 bnpm-0.2.4/bnpm/h5_handling.py
+-rwxrwxrwx   0 root         (0) root         (0)    22292 2023-07-19 23:16:37.000000 bnpm-0.2.4/bnpm/image_augmentation.py
+-rwxrwxrwx   0 root         (0) root         (0)    57594 2023-07-01 01:57:59.000000 bnpm-0.2.4/bnpm/image_processing.py
+-rwxrwxrwx   0 root         (0) root         (0)    24032 2023-07-26 01:32:50.000000 bnpm-0.2.4/bnpm/indexing.py
+-rwxrwxrwx   0 root         (0) root         (0)    17856 2023-03-05 00:44:40.000000 bnpm-0.2.4/bnpm/linear_regression.py
+-rwxrwxrwx   0 root         (0) root         (0)     8317 2023-04-21 04:21:03.000000 bnpm-0.2.4/bnpm/math_functions.py
+-rwxrwxrwx   0 root         (0) root         (0)     6202 2023-06-17 04:51:49.000000 bnpm-0.2.4/bnpm/misc.py
+-rwxrwxrwx   0 root         (0) root         (0)    10034 2023-06-24 16:25:12.000000 bnpm-0.2.4/bnpm/optimization.py
+-rwxrwxrwx   0 root         (0) root         (0)     6922 2023-04-28 21:19:30.000000 bnpm-0.2.4/bnpm/other_peoples_code.py
+-rwxrwxrwx   0 root         (0) root         (0)     4442 2023-04-29 05:04:13.000000 bnpm-0.2.4/bnpm/parallel_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     6585 2023-07-20 19:39:00.000000 bnpm-0.2.4/bnpm/path_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    40543 2023-07-11 00:22:09.000000 bnpm-0.2.4/bnpm/plotting_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)     9811 2023-05-18 20:31:06.000000 bnpm-0.2.4/bnpm/resource_tracking.py
+-rwxrwxrwx   0 root         (0) root         (0)    35095 2023-07-12 19:58:26.000000 bnpm-0.2.4/bnpm/server.py
+-rwxrwxrwx   0 root         (0) root         (0)    31408 2023-07-11 01:31:23.000000 bnpm-0.2.4/bnpm/similarity.py
+-rwxrwxrwx   0 root         (0) root         (0)    22632 2023-06-17 04:28:34.000000 bnpm-0.2.4/bnpm/spectral.py
+-rwxrwxrwx   0 root         (0) root         (0)     1130 2023-05-18 04:27:38.000000 bnpm-0.2.4/bnpm/stats.py
+-rwxrwxrwx   0 root         (0) root         (0)    35757 2023-06-17 04:42:40.000000 bnpm-0.2.4/bnpm/timeSeries.py
+-rwxrwxrwx   0 root         (0) root         (0)    23580 2023-07-24 17:18:00.000000 bnpm-0.2.4/bnpm/torch_helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    50036 2023-06-16 03:39:42.000000 bnpm-0.2.4/bnpm/video.py
+-rwxrwxrwx   0 root         (0) root         (0)     3338 2021-12-28 19:07:58.000000 bnpm-0.2.4/bnpm/welford_moving.py
+-rwxrwxrwx   0 root         (0) root         (0)     4882 2021-05-05 20:10:58.000000 bnpm-0.2.4/bnpm/welford_moving_2D.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-26 03:45:49.556372 bnpm-0.2.4/bnpm.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3330 2023-07-26 03:45:49.000000 bnpm-0.2.4/bnpm.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      926 2023-07-26 03:45:49.000000 bnpm-0.2.4/bnpm.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-07-26 03:45:49.000000 bnpm-0.2.4/bnpm.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      326 2023-07-26 03:45:49.000000 bnpm-0.2.4/bnpm.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)        5 2023-07-26 03:45:49.000000 bnpm-0.2.4/bnpm.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)      349 2023-06-10 00:46:32.000000 bnpm-0.2.4/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-07-26 03:45:49.557037 bnpm-0.2.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2954 2023-07-11 20:02:35.000000 bnpm-0.2.4/setup.py
```

### Comparing `bnpm-0.2.3/LICENSE` & `bnpm-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/PKG-INFO` & `bnpm-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 Provides-Extra: advanced
```

### Comparing `bnpm-0.2.3/README.md` & `bnpm-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/__init__.py` & `bnpm-0.2.4/bnpm/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,15 @@
             'cross_validation',
             'cupy_helpers',
             'decomposition',
             'email_helpers',
             'featurization',
             'file_helpers',
             'h5_handling',
+            'image_augmentation',
             'image_processing',
             'indexing',
             'linear_regression',
             'math_functions',
             'misc',
             'optimization',
             'other_peoples_code',
@@ -29,8 +30,8 @@
             'torch_helpers',
             'video',
         ]
 
 for pkg in __all__:
     exec('from . import ' + pkg)
 
-__version__ = '0.2.3'
+__version__ = '0.2.4'
```

### Comparing `bnpm-0.2.3/bnpm/ca2p_preprocessing.py` & `bnpm-0.2.4/bnpm/ca2p_preprocessing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/classification.py` & `bnpm-0.2.4/bnpm/classification.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/clustering.py` & `bnpm-0.2.4/bnpm/clustering.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/container_helpers.py` & `bnpm-0.2.4/bnpm/container_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/cross_validation.py` & `bnpm-0.2.4/bnpm/cross_validation.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/cupy_helpers.py` & `bnpm-0.2.4/bnpm/cupy_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/decomposition.py` & `bnpm-0.2.4/bnpm/decomposition.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/dtw.py` & `bnpm-0.2.4/bnpm/dtw.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/email_helpers.py` & `bnpm-0.2.4/bnpm/email_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/featurization.py` & `bnpm-0.2.4/bnpm/featurization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/file_helpers.py` & `bnpm-0.2.4/bnpm/file_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,15 +539,15 @@
     with open(path_save, write_mode) as f:
         with tqdm(total=total_size, disable=(verbose==False), unit='B', unit_scale=True, unit_divisor=1024) as pbar:
             for data in response.iter_content(chunk_size):
                 wrote = wrote + len(data)
                 f.write(data)
                 pbar.update(len(data))
     if total_size != 0 and wrote != total_size:
-        print("ERROR, something went wrong")
+        print("Error downloading file. Downloaded file is not the same size as the file on the server.")
         return False
     # Check hash
     if check_hash:
         hash_local = hash_file(path_save, type_hash=hash_type)
         if hash_local == hash_hex:
             print('Hash of downloaded file matches hash_hex.') if verbose else None
             return True
@@ -673,15 +673,15 @@
         verbose (int):
             Whether to print progress.
     """
     path_zipFile = prepare_filepath_for_loading(path_zipFile, must_exist=True)
     import zipfile
     if path_extract is None:
         path_extract = str(Path(path_zipFile).parent)
-    path_extract = prepare_directory_for_saving(path_extract, mkdir=mkdir, allow_overwrite=True)
+    path_extract = prepare_directory_for_saving(path_extract, mkdir=mkdir, exist_ok=True)
 
     print(f'Extracting {path_zipFile} to {path_extract}.') if verbose else None
 
     with zipfile.ZipFile(path_zipFile, 'r') as zip_ref:
         zip_ref.extractall(path_extract)
 
     print('Completed zip extraction.') if verbose else None
```

### Comparing `bnpm-0.2.3/bnpm/h5_handling.py` & `bnpm-0.2.4/bnpm/h5_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-###########################
-####### H5_HANDLING #######
-###########################
-
 import gc
+from pathlib import Path
+
 import h5py
 
 def close_all_h5():
     '''
     Closes all h5 objects in workspace. Not tested thoroughly.
     from here: https://stackoverflow.com/questions/29863342/close-an-open-h5py-data-file
     '''
@@ -229,15 +227,16 @@
 
 def simple_save(
     dict_to_save, 
     path=None, 
     use_compression=False, 
     track_order=True, 
     write_mode='w-', 
-    verbose=False
+    mkdir=True,
+    verbose=False,
 ):
     """
     Saves a python dict to an hdf file.
     Also allows for adding new data to
      an existing hdf file.
     RH 2021
 
@@ -255,14 +254,17 @@
             Whether or not to use compression when writing the h5 file
         track_order (bool):
             Whether or not to keep track of the order of the items in the dict
         verbose (bool):
             Whether or not to print out the h5 file hierarchy.
     """
 
+    if mkdir:
+        Path(path).parent.mkdir(parents=True, exist_ok=True)
+
     write_dict_to_h5(
         path, 
         dict_to_save, 
         use_compression=use_compression, 
         track_order=track_order,
         write_mode=write_mode, 
         show_item_tree_pref=verbose
```

### Comparing `bnpm-0.2.3/bnpm/image_processing.py` & `bnpm-0.2.4/bnpm/image_processing.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/indexing.py` & `bnpm-0.2.4/bnpm/indexing.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     Returns:
         idx (np.ndarray):
             1-D array of indices.
     '''
     return np.where(bool_vec)[0]
 
 
-def moduloCounter_to_linearCounter(trace, modulus, modulus_value, diff_thresh=None, plot_pref=False):
+def moduloCounter_to_linearCounter(trace, modulus, modulus_value=None, diff_thresh=None, plot_pref=False):
     '''
     Converts a (sawtooth) trace of modulo counter
      values to a linear counter.
     Useful for converting a pixel clock with a modulus
      to total times. Use this for FLIR camera top pixel
      stuff.
     The function basically just finds where the modulus
@@ -102,15 +102,16 @@
         trace (np.ndarray):
             1-D array of modulo counter values.
         modulus (scalar):
             Modulus of the counter. Values in trace
              should range from 0 to modulus-1.
         modulus_value (scalar):
             Multiplier for the modulus counter. The
-             value of a modulus event.
+             value of a modulus event. If None, then
+             modulus_value is set to modulus.
         diff_thresh (scalar):
             Threshold for defining a modulus event.
             Should typically be a negative value
              smaller than 'modulus', but larger
              than the difference between consecutive
              trace values.
         plot_pref (bool):
@@ -120,14 +121,17 @@
         linearCounter (np.ndarray):
             1-D array of linearized counter values.
     '''
 
     if diff_thresh is None:
         diff_thresh = -modulus/2
 
+    if modulus_value is None:
+        modulus_value = modulus
+
     diff_trace = np.diff(np.double(trace))
     mod_times = np.where(diff_trace<diff_thresh)[0]
 
 
     mod_times_bool = np.zeros(len(trace))
     mod_times_bool[mod_times+1] = modulus_value
     mod_times_steps = np.cumsum(mod_times_bool)
@@ -239,15 +243,16 @@
 
 def make_batches(
     iterable, 
     batch_size=None, 
     num_batches=None, 
     min_batch_size=0, 
     return_idx=False, 
-    length=None
+    length=None,
+    idx_start=0,
 ):
     """
     Make batches of data or any other iterable.
     RH 2021
 
     Args:
         iterable (iterable):
@@ -263,29 +268,31 @@
             whether to return the slice indices of the batches.
             output will be [start, end] idx
         length (int):
             length of the iterable.
             if None, then length is len(iterable)
             This is useful if you want to make batches of 
              something that doesn't have a __len__ method.
+        idx_start (int):
+            starting index of the iterable.
     
     Returns:
         output (iterable):
             batches of iterable
     """
 
     if length is None:
         l = len(iterable)
     else:
         l = length
     
     if batch_size is None:
         batch_size = np.int64(np.ceil(l / num_batches))
     
-    for start in range(0, l, batch_size):
+    for start in range(idx_start, l, batch_size):
         end = min(start + batch_size, l)
         if (end-start) < min_batch_size:
             break
         else:
             if return_idx:
                 yield iterable[start:end], [start, end]
             else:
```

### Comparing `bnpm-0.2.3/bnpm/linear_regression.py` & `bnpm-0.2.4/bnpm/linear_regression.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/math_functions.py` & `bnpm-0.2.4/bnpm/math_functions.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/misc.py` & `bnpm-0.2.4/bnpm/misc.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/optimization.py` & `bnpm-0.2.4/bnpm/optimization.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/other_peoples_code.py` & `bnpm-0.2.4/bnpm/other_peoples_code.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/parallel_helpers.py` & `bnpm-0.2.4/bnpm/parallel_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/path_helpers.py` & `bnpm-0.2.4/bnpm/path_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     dir_outer, 
     reMatch='filename', 
     find_files=True, 
     find_folders=False, 
     depth=0, 
     natsorted=True, 
     alg_ns=None, 
+    verbose=False,
 ):
     """
     Search for files and/or folders recursively in a directory.
     RH 2022
 
     Args:
         dir_outer (str):
@@ -134,14 +135,16 @@
         alg_ns (str):
             Algorithm to use for natural sorting.
             See natsort.ns or
              https://natsort.readthedocs.io/en/4.0.4/ns_class.html
              for options.
             Default is PATH.
             Other commons are INT, FLOAT, VERSION.
+        verbose (bool):
+            Whether to print the paths as they are found.
 
     Returns:
         paths (List of str):
             Paths to matched files and/or folders in the directory
     """
     import natsort
     if alg_ns is None:
@@ -151,20 +154,22 @@
         paths = []
         for path in os.listdir(dir_inner):
             path = os.path.join(dir_inner, path)
             if os.path.isdir(path):
                 if find_folders:
                     if re.search(reMatch, path) is not None:
                         paths.append(path)
+                        print(path) if verbose else None
                 if depth < depth_end:
                     paths += get_paths_recursive_inner(path, depth_end, depth=depth+1)
             else:
                 if find_files:
                     if re.search(reMatch, path) is not None:
                         paths.append(path)
+                        print(path) if verbose else None
         return paths
 
     paths = get_paths_recursive_inner(dir_outer, depth, depth=0)
     if natsorted:
         paths = natsort.natsorted(paths, alg=alg_ns)
     return paths
```

### Comparing `bnpm-0.2.3/bnpm/plotting_helpers.py` & `bnpm-0.2.4/bnpm/plotting_helpers.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/resource_tracking.py` & `bnpm-0.2.4/bnpm/resource_tracking.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/server.py` & `bnpm-0.2.4/bnpm/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,40 +576,46 @@
                 Path to the source directory (local).
             target (str):
                 Path to the target directory (remote).
         '''
         source = Path(source).resolve()
         target = Path(target).resolve()
         
-        
         for item in os.listdir(source):
             if os.path.isfile(source / item):
                 if verbose:
                     print(f'uploading {source / item}   to   {target / item}')
                 self.sftp.put(str(source / item) , str(target / item))
             else:
                 self.mkdir_safe(str(target / item) , ignore_existing=True)
                 self.put_dir(source / item , target / item)
 
-    def get_dir(self, source, target, verbose=True):
+    def get_dir(self, source, target, mkdir=True, verbose=True):
         '''
-        Downloads the contents of the source directory to the target path.
-        All subdirectories in source are created under target recusively.
+        Downloads the contents of the source directory to the target path. All
+        subdirectories in source are created under target recusively.
+        
         Args:
             source (str):
                 Path to the source directory (remote).
             target (str):
                 Path to the target directory (local).
+            mkdir (bool):
+                Whether or not to create the target directory.
+            verbose (bool):
+                Whether or not to print progress of files being downloaded.
         '''
+        if mkdir:
+            Path(target).mkdir(parents=True, exist_ok=True)
         source = Path(source).resolve()
         target = Path(target).resolve()
         
         for item in self.sftp.listdir(str(source)):
             if self.isdir_remote(str(source / item)):
-                (target / item).mkdir(parents=True, exist_ok=True)
+                (target / item).mkdir(parents=True, exist_ok=True)  ## probably not necessary anymore since done above
                 self.get_dir(source / item , target / item)
             else:
                 if verbose:
                     print(f'downloading {source / item}   to   {target / item}')
                 self.sftp.get(str(source / item) , str(target / item))
```

### Comparing `bnpm-0.2.3/bnpm/similarity.py` & `bnpm-0.2.4/bnpm/similarity.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/spectral.py` & `bnpm-0.2.4/bnpm/spectral.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/stats.py` & `bnpm-0.2.4/bnpm/stats.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/timeSeries.py` & `bnpm-0.2.4/bnpm/timeSeries.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/torch_helpers.py` & `bnpm-0.2.4/bnpm/torch_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         (str): 
             device (str): 
                 A string specifying the device, either *"cpu"* or
                 *"cuda:<device_num>"*.
     """
     if use_GPU:
         print(f'devices available: {[torch.cuda.get_device_properties(ii) for ii in range(torch.cuda.device_count())]}') if verbose else None
-        device = f"cuda:{device_num}" if torch.cuda.is_available() else "cpu"
+        device = torch.device(device_num) if torch.cuda.is_available() else "cpu"
         if device == "cpu":
             print("no GPU available. Using CPU.") if verbose else None
         else:
             print(f"Using device: '{device}': {torch.cuda.get_device_properties(device_num)}") if verbose else None
     else:
         device = "cpu"
         print(f"device: '{device}'") if verbose else None
```

### Comparing `bnpm-0.2.3/bnpm/video.py` & `bnpm-0.2.4/bnpm/video.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/welford_moving.py` & `bnpm-0.2.4/bnpm/welford_moving.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm/welford_moving_2D.py` & `bnpm-0.2.4/bnpm/welford_moving_2D.py`

 * *Files identical despite different names*

### Comparing `bnpm-0.2.3/bnpm.egg-info/PKG-INFO` & `bnpm-0.2.4/bnpm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bnpm
-Version: 0.2.3
+Version: 0.2.4
 Summary: A library of useful modules for data analysis.
 Home-page: https://github.com/RichieHakim/basic_neural_processing_modules
 Author: Richard Hakim
 License: LICENSE
 Keywords: data analysis,machine learning,neuroscience
 Description-Content-Type: text/markdown
 Provides-Extra: advanced
```

### Comparing `bnpm-0.2.3/bnpm.egg-info/SOURCES.txt` & `bnpm-0.2.4/bnpm.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 bnpm/cupy_helpers.py
 bnpm/decomposition.py
 bnpm/dtw.py
 bnpm/email_helpers.py
 bnpm/featurization.py
 bnpm/file_helpers.py
 bnpm/h5_handling.py
+bnpm/image_augmentation.py
 bnpm/image_processing.py
 bnpm/indexing.py
 bnpm/linear_regression.py
 bnpm/math_functions.py
 bnpm/misc.py
 bnpm/optimization.py
 bnpm/other_peoples_code.py
```

### Comparing `bnpm-0.2.3/setup.py` & `bnpm-0.2.4/setup.py`

 * *Files identical despite different names*

