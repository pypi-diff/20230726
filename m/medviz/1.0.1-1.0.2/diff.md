# Comparing `tmp/medviz-1.0.1.tar.gz` & `tmp/medviz-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medviz-1.0.1.tar", last modified: Fri Jul 21 18:42:09 2023, max compression
+gzip compressed data, was "medviz-1.0.2.tar", last modified: Wed Jul 26 04:21:19 2023, max compression
```

## Comparing `medviz-1.0.1.tar` & `medviz-1.0.2.tar`

### file list

```diff
@@ -1,67 +1,71 @@
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)    36861 2023-05-31 20:04:32.000000 medviz-1.0.1/LICENSE
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      180 2023-06-01 05:23:25.000000 medviz-1.0.1/MANIFEST.in
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2274 2023-07-21 18:42:09.764025 medviz-1.0.1/PKG-INFO
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     1803 2023-04-27 15:46:29.000000 medviz-1.0.1/README.rst
--rw-r-----   0 mohsen    (1000) mohsen    (1000)        5 2023-07-21 18:33:23.000000 medviz-1.0.1/VERSION
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.760025 medviz-1.0.1/medviz/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     2325 2023-07-21 18:33:53.000000 medviz-1.0.1/medviz/__init__.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/collage/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)       41 2023-06-01 02:13:13.000000 medviz-1.0.1/medviz/collage/__init__.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     1982 2023-06-01 02:40:53.000000 medviz-1.0.1/medviz/collage/compute_collage.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)    24895 2023-05-31 20:21:55.000000 medviz-1.0.1/medviz/collage/main.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     2122 2023-06-01 02:47:15.000000 medviz-1.0.1/medviz/collage/stats.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/multimodal/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)       85 2023-05-22 16:27:34.000000 medviz-1.0.1/medviz/multimodal/__init__.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     1065 2023-05-24 22:21:17.000000 medviz-1.0.1/medviz/multimodal/save_dicom_metadata.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      509 2023-05-22 16:27:37.000000 medviz-1.0.1/medviz/multimodal/stats.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/nifti/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     4367 2023-06-08 00:11:51.000000 medviz-1.0.1/medviz/nifti/helper.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/pkg2_local/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      134 2023-05-23 22:19:26.000000 medviz-1.0.1/medviz/pkg2_local/example.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/plots/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      123 2023-05-23 23:18:05.000000 medviz-1.0.1/medviz/plots/__init__.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     1552 2023-05-18 02:42:18.000000 medviz-1.0.1/medviz/plots/_plot_image.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/plots/gif/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)    10203 2023-05-24 04:19:50.000000 medviz-1.0.1/medviz/plots/gif/gif.py
--rw-rw----   0 mohsen    (1000) mohsen    (1000)     2217 2023-05-25 02:41:16.000000 medviz-1.0.1/medviz/plots/helper_plot.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     3682 2023-05-24 04:19:50.000000 medviz-1.0.1/medviz/plots/layered_plot2D.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/plots/plot2d/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      238 2023-05-24 02:22:53.000000 medviz-1.0.1/medviz/plots/plot2d/__init__.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     2139 2023-06-08 02:13:51.000000 medviz-1.0.1/medviz/plots/plot2d/image_mask_annotated.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     2332 2023-06-08 02:13:23.000000 medviz-1.0.1/medviz/plots/plot2d/image_masks.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     2359 2023-06-08 04:45:40.000000 medviz-1.0.1/medviz/plots/plot2d/images.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     2593 2023-06-08 04:46:15.000000 medviz-1.0.1/medviz/plots/plot2d/masks.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/plots/plot3d/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      205 2023-06-08 07:01:03.000000 medviz-1.0.1/medviz/plots/plot3d/__init__.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     1890 2023-06-08 07:01:51.000000 medviz-1.0.1/medviz/plots/plot3d/image_mask_annotated.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2339 2023-07-18 18:20:40.000000 medviz-1.0.1/medviz/plots/plot3d/image_masks.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     3113 2023-06-08 04:47:31.000000 medviz-1.0.1/medviz/plots/plot3d/images.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     2060 2023-05-31 20:21:55.000000 medviz-1.0.1/medviz/plots/plot3d/layered_plot.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     3577 2023-06-08 06:34:09.000000 medviz-1.0.1/medviz/plots/plot3d/masks.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/preprocess/
--rw-rw----   0 mohsen    (1000) mohsen    (1000)      120 2023-07-21 18:32:38.000000 medviz-1.0.1/medviz/preprocess/__init__.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     2071 2023-07-16 03:13:55.000000 medviz-1.0.1/medviz/preprocess/mask.py
--rw-rw----   0 mohsen    (1000) mohsen    (1000)     2764 2023-06-03 02:10:07.000000 medviz-1.0.1/medviz/preprocess/match_image_mask.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2086 2023-07-21 17:52:29.000000 medviz-1.0.1/medviz/preprocess/resampling.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2521 2023-07-18 18:47:42.000000 medviz-1.0.1/medviz/preprocess/resampling_local.py
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)     2996 2023-07-21 17:12:55.000000 medviz-1.0.1/medviz/preprocess/resampling_local_new.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz/utils/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      614 2023-06-08 00:57:20.000000 medviz-1.0.1/medviz/utils/__init__.py
--rw-rw----   0 mohsen    (1000) mohsen    (1000)     2175 2023-05-13 17:59:38.000000 medviz-1.0.1/medviz/utils/array_profile.py
--rw-rw----   0 mohsen    (1000) mohsen    (1000)      662 2023-05-13 18:05:32.000000 medviz-1.0.1/medviz/utils/array_threshold.py
--rwxr-x---   0 mohsen    (1000) mohsen    (1000)     1069 2023-06-08 00:57:03.000000 medviz-1.0.1/medviz/utils/custom_type.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     4587 2023-05-23 23:25:32.000000 medviz-1.0.1/medviz/utils/helper_mask.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     2583 2023-07-18 18:20:40.000000 medviz-1.0.1/medviz/utils/helper_path.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      689 2023-01-02 16:26:25.000000 medviz-1.0.1/medviz/utils/log.py
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      859 2023-05-24 05:07:22.000000 medviz-1.0.1/medviz/utils/reader.py
--rwxr-x---   0 mohsen    (1000) mohsen    (1000)       80 2023-05-17 19:24:17.000000 medviz-1.0.1/medviz/utils/utility.py
-drwxr-xr-x   0 mohsen    (1000) mohsen    (1000)        0 2023-07-21 18:42:09.764025 medviz-1.0.1/medviz.egg-info/
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     2274 2023-07-21 18:42:09.000000 medviz-1.0.1/medviz.egg-info/PKG-INFO
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     1444 2023-07-21 18:42:09.000000 medviz-1.0.1/medviz.egg-info/SOURCES.txt
--rw-r-----   0 mohsen    (1000) mohsen    (1000)        1 2023-07-21 18:42:09.000000 medviz-1.0.1/medviz.egg-info/dependency_links.txt
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      190 2023-07-21 18:42:09.000000 medviz-1.0.1/medviz.egg-info/requires.txt
--rw-r-----   0 mohsen    (1000) mohsen    (1000)        7 2023-07-21 18:42:09.000000 medviz-1.0.1/medviz.egg-info/top_level.txt
--rw-r-----   0 mohsen    (1000) mohsen    (1000)     1359 2023-06-01 05:50:19.000000 medviz-1.0.1/pyproject.toml
--rw-r--r--   0 mohsen    (1000) mohsen    (1000)       38 2023-07-21 18:42:09.764025 medviz-1.0.1/setup.cfg
--rw-r-----   0 mohsen    (1000) mohsen    (1000)      170 2023-04-02 14:20:15.000000 medviz-1.0.1/setup.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.943623 medviz-1.0.2/
+-rw-r-----   0 fes       (1000) fes       (1000)    36861 2023-05-31 20:04:32.000000 medviz-1.0.2/LICENSE
+-rw-r-----   0 fes       (1000) fes       (1000)      180 2023-06-01 05:23:25.000000 medviz-1.0.2/MANIFEST.in
+-rw-rw-r--   0 fes       (1000) fes       (1000)     2274 2023-07-26 04:21:19.943623 medviz-1.0.2/PKG-INFO
+-rw-r-----   0 fes       (1000) fes       (1000)     1803 2023-04-27 15:46:29.000000 medviz-1.0.2/README.rst
+-rw-r-----   0 fes       (1000) fes       (1000)        5 2023-07-26 04:21:05.000000 medviz-1.0.2/VERSION
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.931624 medviz-1.0.2/medviz/
+-rw-r-----   0 fes       (1000) fes       (1000)     2375 2023-07-26 04:21:03.000000 medviz-1.0.2/medviz/__init__.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.931624 medviz-1.0.2/medviz/collage/
+-rw-r-----   0 fes       (1000) fes       (1000)       41 2023-06-01 02:13:13.000000 medviz-1.0.2/medviz/collage/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     1982 2023-06-01 02:40:53.000000 medviz-1.0.2/medviz/collage/compute_collage.py
+-rw-r-----   0 fes       (1000) fes       (1000)    24895 2023-05-31 20:21:55.000000 medviz-1.0.2/medviz/collage/main.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2122 2023-06-01 02:47:15.000000 medviz-1.0.2/medviz/collage/stats.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.931624 medviz-1.0.2/medviz/multimodal/
+-rw-r-----   0 fes       (1000) fes       (1000)       85 2023-05-22 16:27:34.000000 medviz-1.0.2/medviz/multimodal/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     1065 2023-05-24 22:21:17.000000 medviz-1.0.2/medviz/multimodal/save_dicom_metadata.py
+-rw-r-----   0 fes       (1000) fes       (1000)      509 2023-05-22 16:27:37.000000 medviz-1.0.2/medviz/multimodal/stats.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.931624 medviz-1.0.2/medviz/nifti/
+-rw-rw-r--   0 fes       (1000) fes       (1000)       30 2023-07-26 03:32:59.000000 medviz-1.0.2/medviz/nifti/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     4377 2023-07-26 03:23:51.000000 medviz-1.0.2/medviz/nifti/helper.py
+-rw-rw-r--   0 fes       (1000) fes       (1000)     1505 2023-07-26 04:17:29.000000 medviz-1.0.2/medviz/nifti/metadata.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.931624 medviz-1.0.2/medviz/pkg2_local/
+-rw-r-----   0 fes       (1000) fes       (1000)      134 2023-05-23 22:19:26.000000 medviz-1.0.2/medviz/pkg2_local/example.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.935624 medviz-1.0.2/medviz/plots/
+-rw-r-----   0 fes       (1000) fes       (1000)      123 2023-05-23 23:18:05.000000 medviz-1.0.2/medviz/plots/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     1552 2023-05-18 02:42:18.000000 medviz-1.0.2/medviz/plots/_plot_image.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.935624 medviz-1.0.2/medviz/plots/gif/
+-rw-r-----   0 fes       (1000) fes       (1000)    10203 2023-05-24 04:19:50.000000 medviz-1.0.2/medviz/plots/gif/gif.py
+-rw-rw----   0 fes       (1000) fes       (1000)     2217 2023-05-25 02:41:16.000000 medviz-1.0.2/medviz/plots/helper_plot.py
+-rw-r-----   0 fes       (1000) fes       (1000)     3682 2023-05-24 04:19:50.000000 medviz-1.0.2/medviz/plots/layered_plot2D.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.935624 medviz-1.0.2/medviz/plots/plot2d/
+-rw-r-----   0 fes       (1000) fes       (1000)      238 2023-05-24 02:22:53.000000 medviz-1.0.2/medviz/plots/plot2d/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2139 2023-06-08 02:13:51.000000 medviz-1.0.2/medviz/plots/plot2d/image_mask_annotated.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2332 2023-06-08 02:13:23.000000 medviz-1.0.2/medviz/plots/plot2d/image_masks.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2359 2023-06-08 04:45:40.000000 medviz-1.0.2/medviz/plots/plot2d/images.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2593 2023-06-08 04:46:15.000000 medviz-1.0.2/medviz/plots/plot2d/masks.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.935624 medviz-1.0.2/medviz/plots/plot3d/
+-rw-r-----   0 fes       (1000) fes       (1000)      205 2023-06-08 07:01:03.000000 medviz-1.0.2/medviz/plots/plot3d/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     1890 2023-06-08 07:01:51.000000 medviz-1.0.2/medviz/plots/plot3d/image_mask_annotated.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     2339 2023-07-18 18:20:40.000000 medviz-1.0.2/medviz/plots/plot3d/image_masks.py
+-rw-r-----   0 fes       (1000) fes       (1000)     3113 2023-06-08 04:47:31.000000 medviz-1.0.2/medviz/plots/plot3d/images.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2060 2023-05-31 20:21:55.000000 medviz-1.0.2/medviz/plots/plot3d/layered_plot.py
+-rw-r-----   0 fes       (1000) fes       (1000)     3577 2023-06-08 06:34:09.000000 medviz-1.0.2/medviz/plots/plot3d/masks.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.939623 medviz-1.0.2/medviz/preprocess/
+-rw-rw----   0 fes       (1000) fes       (1000)      161 2023-07-21 19:23:55.000000 medviz-1.0.2/medviz/preprocess/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2071 2023-07-16 03:13:55.000000 medviz-1.0.2/medviz/preprocess/mask.py
+-rw-rw----   0 fes       (1000) fes       (1000)     2764 2023-06-03 02:10:07.000000 medviz-1.0.2/medviz/preprocess/match_image_mask.py
+-rw-r--r--   0 fes       (1000) fes       (1000)      983 2023-07-21 19:29:56.000000 medviz-1.0.2/medviz/preprocess/read_mha.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     2092 2023-07-21 18:48:10.000000 medviz-1.0.2/medviz/preprocess/resampling.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     2521 2023-07-18 18:47:42.000000 medviz-1.0.2/medviz/preprocess/resampling_local.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     2996 2023-07-21 17:12:55.000000 medviz-1.0.2/medviz/preprocess/resampling_local_new.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     1320 2023-07-21 19:26:45.000000 medviz-1.0.2/medviz/preprocess/resampling_mha.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.939623 medviz-1.0.2/medviz/utils/
+-rw-r-----   0 fes       (1000) fes       (1000)      614 2023-06-08 00:57:20.000000 medviz-1.0.2/medviz/utils/__init__.py
+-rw-rw----   0 fes       (1000) fes       (1000)     2175 2023-05-13 17:59:38.000000 medviz-1.0.2/medviz/utils/array_profile.py
+-rw-rw----   0 fes       (1000) fes       (1000)      662 2023-05-13 18:05:32.000000 medviz-1.0.2/medviz/utils/array_threshold.py
+-rwxr-x---   0 fes       (1000) fes       (1000)     1069 2023-06-08 00:57:03.000000 medviz-1.0.2/medviz/utils/custom_type.py
+-rw-r-----   0 fes       (1000) fes       (1000)     4587 2023-05-23 23:25:32.000000 medviz-1.0.2/medviz/utils/helper_mask.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2583 2023-07-18 18:20:40.000000 medviz-1.0.2/medviz/utils/helper_path.py
+-rw-r-----   0 fes       (1000) fes       (1000)      689 2023-01-02 16:26:25.000000 medviz-1.0.2/medviz/utils/log.py
+-rw-r-----   0 fes       (1000) fes       (1000)      859 2023-05-24 05:07:22.000000 medviz-1.0.2/medviz/utils/reader.py
+-rwxr-x---   0 fes       (1000) fes       (1000)       80 2023-05-17 19:24:17.000000 medviz-1.0.2/medviz/utils/utility.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 04:21:19.931624 medviz-1.0.2/medviz.egg-info/
+-rw-r-----   0 fes       (1000) fes       (1000)     2274 2023-07-26 04:21:19.000000 medviz-1.0.2/medviz.egg-info/PKG-INFO
+-rw-r-----   0 fes       (1000) fes       (1000)     1560 2023-07-26 04:21:19.000000 medviz-1.0.2/medviz.egg-info/SOURCES.txt
+-rw-r-----   0 fes       (1000) fes       (1000)        1 2023-07-26 04:21:19.000000 medviz-1.0.2/medviz.egg-info/dependency_links.txt
+-rw-r-----   0 fes       (1000) fes       (1000)      207 2023-07-26 04:21:19.000000 medviz-1.0.2/medviz.egg-info/requires.txt
+-rw-r-----   0 fes       (1000) fes       (1000)        7 2023-07-26 04:21:19.000000 medviz-1.0.2/medviz.egg-info/top_level.txt
+-rw-r-----   0 fes       (1000) fes       (1000)     1383 2023-07-21 19:19:01.000000 medviz-1.0.2/pyproject.toml
+-rw-rw-r--   0 fes       (1000) fes       (1000)       38 2023-07-26 04:21:19.943623 medviz-1.0.2/setup.cfg
+-rw-r-----   0 fes       (1000) fes       (1000)      170 2023-04-02 14:20:15.000000 medviz-1.0.2/setup.py
```

### Comparing `medviz-1.0.1/LICENSE` & `medviz-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/PKG-INFO` & `medviz-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 1.0.1
+Version: 1.0.2
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-1.0.1/README.rst` & `medviz-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/__init__.py` & `medviz-1.0.2/medviz/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,17 +77,19 @@
 
 from .preprocess import *
 from .preprocess import resample
 
 from .collage import compute_stats_collage
 
 from .nifti.helper import nii3d_to_annotated2d, nii_mask3d_to_2d
+from .nifti.metadata import metadata as metadata
 
 # def version():
 #     with open("VERSION", "r") as f:
 #         version = f.read().strip()
 #     return version
 
 # __version__ = version()
 
-__version__ = "1.0.1"
 
+
+__version__ = "1.0.2"
```

### Comparing `medviz-1.0.1/medviz/collage/compute_collage.py` & `medviz-1.0.2/medviz/collage/compute_collage.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/collage/main.py` & `medviz-1.0.2/medviz/collage/main.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/collage/stats.py` & `medviz-1.0.2/medviz/collage/stats.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/multimodal/save_dicom_metadata.py` & `medviz-1.0.2/medviz/multimodal/save_dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/nifti/helper.py` & `medviz-1.0.2/medviz/nifti/helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,19 +60,19 @@
     mask_data[mask_data_bool == False] = 0
 
     mask_img = nib.Nifti1Image(mask_data, affine)
     nib.save(mask_img, output_path)
     print("Mask saved at", output_path)
 
 
-if __name__ == "__main__":
-    mask_data_bool = np.array([[True, False, True], [False, True, False]])
-    affine = np.eye(4)
-    output_path = "mask.nii.gz"
-    mask(mask_data_bool, affine, output_path)
+# if __name__ == "__main__":
+#     mask_data_bool = np.array([[True, False, True], [False, True, False]])
+#     affine = np.eye(4)
+#     output_path = "mask.nii.gz"
+#     mask(mask_data_bool, affine, output_path)
 
 
 def arr_to_nifti(arr: np.ndarray, affine: np.ndarray, output_path: str):
     """
     Save numpy array as nii.gz file
     :param arr: numpy array
     :param affine: affine matrix
```

### Comparing `medviz-1.0.1/medviz/plots/_plot_image.py` & `medviz-1.0.2/medviz/plots/_plot_image.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/gif/gif.py` & `medviz-1.0.2/medviz/plots/gif/gif.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/helper_plot.py` & `medviz-1.0.2/medviz/plots/helper_plot.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/layered_plot2D.py` & `medviz-1.0.2/medviz/plots/layered_plot2D.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/plot2d/image_mask_annotated.py` & `medviz-1.0.2/medviz/plots/plot2d/image_mask_annotated.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/plot2d/image_masks.py` & `medviz-1.0.2/medviz/plots/plot2d/image_masks.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/plot2d/images.py` & `medviz-1.0.2/medviz/plots/plot2d/images.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/plot2d/masks.py` & `medviz-1.0.2/medviz/plots/plot2d/masks.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/plot3d/image_mask_annotated.py` & `medviz-1.0.2/medviz/plots/plot3d/image_mask_annotated.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/plot3d/image_masks.py` & `medviz-1.0.2/medviz/plots/plot3d/image_masks.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/plot3d/images.py` & `medviz-1.0.2/medviz/plots/plot3d/images.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/plot3d/layered_plot.py` & `medviz-1.0.2/medviz/plots/plot3d/layered_plot.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/plots/plot3d/masks.py` & `medviz-1.0.2/medviz/plots/plot3d/masks.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/preprocess/mask.py` & `medviz-1.0.2/medviz/preprocess/mask.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/preprocess/match_image_mask.py` & `medviz-1.0.2/medviz/preprocess/match_image_mask.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/preprocess/resampling.py` & `medviz-1.0.2/medviz/preprocess/resampling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import nibabel as nib
 import numpy as np
-from ..utils import path_in, save_path_file
 from scipy.ndimage import zoom
 
+from ..utils import path_in, save_path_file
+
 
 def resample(input_path, output_path, new_voxel_size, method):
     input_path = path_in(input_path)
 
     # Load the input NIfTI image
     img = nib.load(input_path)
     data = img.get_fdata()
@@ -24,15 +25,15 @@
 
     # Compute the new shape after resampling
     print("Input shape", data.shape)
     new_shape = np.ceil(data.shape * scaling_factors).astype(int)
     print("Output shape", new_shape)
 
     if method == "trilinear":
-    # Use Trilinear interpolation to resample the data
+        # Use Trilinear interpolation to resample the data
         resampled_data = zoom(data, scaling_factors, order=1)
     elif method == "nearest":
         resampled_data = np.zeros(new_shape, dtype=data.dtype)
 
         # Iterate over each voxel in the resampled image
         for i in range(new_shape[0]):
             for j in range(new_shape[1]):
@@ -51,8 +52,8 @@
 
     # Create a new NIfTI image with resampled data and the same affine
     resampled_img = nib.Nifti1Image(resampled_data, affine)
 
     # Save the resampled image to the output path
     save_path = save_path_file(output_path, suffix=".nii")
 
-    nib.save(resampled_img, save_path)
+    nib.save(resampled_img, save_path)
```

### Comparing `medviz-1.0.1/medviz/preprocess/resampling_local.py` & `medviz-1.0.2/medviz/preprocess/resampling_local.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/preprocess/resampling_local_new.py` & `medviz-1.0.2/medviz/preprocess/resampling_local_new.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/utils/__init__.py` & `medviz-1.0.2/medviz/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/utils/array_profile.py` & `medviz-1.0.2/medviz/utils/array_profile.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/utils/array_threshold.py` & `medviz-1.0.2/medviz/utils/array_threshold.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/utils/custom_type.py` & `medviz-1.0.2/medviz/utils/custom_type.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/utils/helper_mask.py` & `medviz-1.0.2/medviz/utils/helper_mask.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/utils/helper_path.py` & `medviz-1.0.2/medviz/utils/helper_path.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/utils/log.py` & `medviz-1.0.2/medviz/utils/log.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz/utils/reader.py` & `medviz-1.0.2/medviz/utils/reader.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.1/medviz.egg-info/PKG-INFO` & `medviz-1.0.2/medviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 1.0.1
+Version: 1.0.2
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-1.0.1/medviz.egg-info/SOURCES.txt` & `medviz-1.0.2/medviz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 medviz/collage/__init__.py
 medviz/collage/compute_collage.py
 medviz/collage/main.py
 medviz/collage/stats.py
 medviz/multimodal/__init__.py
 medviz/multimodal/save_dicom_metadata.py
 medviz/multimodal/stats.py
+medviz/nifti/__init__.py
 medviz/nifti/helper.py
+medviz/nifti/metadata.py
 medviz/pkg2_local/example.py
 medviz/plots/__init__.py
 medviz/plots/_plot_image.py
 medviz/plots/helper_plot.py
 medviz/plots/layered_plot2D.py
 medviz/plots/gif/gif.py
 medviz/plots/plot2d/__init__.py
@@ -34,17 +36,19 @@
 medviz/plots/plot3d/image_masks.py
 medviz/plots/plot3d/images.py
 medviz/plots/plot3d/layered_plot.py
 medviz/plots/plot3d/masks.py
 medviz/preprocess/__init__.py
 medviz/preprocess/mask.py
 medviz/preprocess/match_image_mask.py
+medviz/preprocess/read_mha.py
 medviz/preprocess/resampling.py
 medviz/preprocess/resampling_local.py
 medviz/preprocess/resampling_local_new.py
+medviz/preprocess/resampling_mha.py
 medviz/utils/__init__.py
 medviz/utils/array_profile.py
 medviz/utils/array_threshold.py
 medviz/utils/custom_type.py
 medviz/utils/helper_mask.py
 medviz/utils/helper_path.py
 medviz/utils/log.py
```

### Comparing `medviz-1.0.1/pyproject.toml` & `medviz-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   "matplotlib >= 3.3.4",
   "nibabel >= 3.2.1",
   "imageio >= 2.9.0",
   "scikit-image >= 0.18.3",
   "tabulate >= 0.8.9",
   "pydicom >= 2.1.2",
   "mahotas >= 1.4.11",
+  "SimpleITK >= 2.1.1",
 ]
 
 [tool.setuptools]
 packages = ["medviz", "medviz.multimodal", "medviz.preprocess"]
 
 
 [tool.setuptools.dynamic]
```

