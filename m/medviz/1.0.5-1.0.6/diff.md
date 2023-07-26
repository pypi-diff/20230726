# Comparing `tmp/medviz-1.0.5.tar.gz` & `tmp/medviz-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medviz-1.0.5.tar", last modified: Wed Jul 26 18:48:02 2023, max compression
+gzip compressed data, was "medviz-1.0.6.tar", last modified: Wed Jul 26 18:55:59 2023, max compression
```

## Comparing `medviz-1.0.5.tar` & `medviz-1.0.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.756736 medviz-1.0.5/
--rw-r-----   0 fes       (1000) fes       (1000)    36861 2023-05-31 20:04:32.000000 medviz-1.0.5/LICENSE
--rw-r-----   0 fes       (1000) fes       (1000)      180 2023-06-01 05:23:25.000000 medviz-1.0.5/MANIFEST.in
--rw-rw-r--   0 fes       (1000) fes       (1000)     2274 2023-07-26 18:48:02.756736 medviz-1.0.5/PKG-INFO
--rw-r-----   0 fes       (1000) fes       (1000)     1803 2023-04-27 15:46:29.000000 medviz-1.0.5/README.rst
--rw-r-----   0 fes       (1000) fes       (1000)        5 2023-07-26 18:47:40.000000 medviz-1.0.5/VERSION
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.744736 medviz-1.0.5/medviz/
--rw-r-----   0 fes       (1000) fes       (1000)     2462 2023-07-26 18:47:47.000000 medviz-1.0.5/medviz/__init__.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.748736 medviz-1.0.5/medviz/collage/
--rw-r-----   0 fes       (1000) fes       (1000)       41 2023-06-01 02:13:13.000000 medviz-1.0.5/medviz/collage/__init__.py
--rw-r-----   0 fes       (1000) fes       (1000)     1982 2023-06-01 02:40:53.000000 medviz-1.0.5/medviz/collage/compute_collage.py
--rw-r-----   0 fes       (1000) fes       (1000)    24895 2023-05-31 20:21:55.000000 medviz-1.0.5/medviz/collage/main.py
--rw-r-----   0 fes       (1000) fes       (1000)     2122 2023-06-01 02:47:15.000000 medviz-1.0.5/medviz/collage/stats.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.748736 medviz-1.0.5/medviz/multimodal/
--rw-r-----   0 fes       (1000) fes       (1000)       85 2023-05-22 16:27:34.000000 medviz-1.0.5/medviz/multimodal/__init__.py
--rw-r-----   0 fes       (1000) fes       (1000)     1065 2023-05-24 22:21:17.000000 medviz-1.0.5/medviz/multimodal/save_dicom_metadata.py
--rw-r-----   0 fes       (1000) fes       (1000)      509 2023-05-22 16:27:37.000000 medviz-1.0.5/medviz/multimodal/stats.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.748736 medviz-1.0.5/medviz/nifti/
--rw-rw-r--   0 fes       (1000) fes       (1000)       30 2023-07-26 03:32:59.000000 medviz-1.0.5/medviz/nifti/__init__.py
--rw-r-----   0 fes       (1000) fes       (1000)     4377 2023-07-26 03:23:51.000000 medviz-1.0.5/medviz/nifti/helper.py
--rw-rw-r--   0 fes       (1000) fes       (1000)     1664 2023-07-26 15:18:23.000000 medviz-1.0.5/medviz/nifti/metadata.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.748736 medviz-1.0.5/medviz/pkg2_local/
--rw-r-----   0 fes       (1000) fes       (1000)      134 2023-05-23 22:19:26.000000 medviz-1.0.5/medviz/pkg2_local/example.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.748736 medviz-1.0.5/medviz/plots/
--rw-r-----   0 fes       (1000) fes       (1000)      123 2023-05-23 23:18:05.000000 medviz-1.0.5/medviz/plots/__init__.py
--rw-r-----   0 fes       (1000) fes       (1000)     1552 2023-05-18 02:42:18.000000 medviz-1.0.5/medviz/plots/_plot_image.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.748736 medviz-1.0.5/medviz/plots/gif/
--rw-r-----   0 fes       (1000) fes       (1000)    10203 2023-05-24 04:19:50.000000 medviz-1.0.5/medviz/plots/gif/gif.py
--rw-rw----   0 fes       (1000) fes       (1000)     2217 2023-05-25 02:41:16.000000 medviz-1.0.5/medviz/plots/helper_plot.py
--rw-r-----   0 fes       (1000) fes       (1000)     3682 2023-05-24 04:19:50.000000 medviz-1.0.5/medviz/plots/layered_plot2D.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.752736 medviz-1.0.5/medviz/plots/plot2d/
--rw-r-----   0 fes       (1000) fes       (1000)      238 2023-05-24 02:22:53.000000 medviz-1.0.5/medviz/plots/plot2d/__init__.py
--rw-r-----   0 fes       (1000) fes       (1000)     2139 2023-06-08 02:13:51.000000 medviz-1.0.5/medviz/plots/plot2d/image_mask_annotated.py
--rw-r-----   0 fes       (1000) fes       (1000)     2332 2023-06-08 02:13:23.000000 medviz-1.0.5/medviz/plots/plot2d/image_masks.py
--rw-r-----   0 fes       (1000) fes       (1000)     2359 2023-06-08 04:45:40.000000 medviz-1.0.5/medviz/plots/plot2d/images.py
--rw-r-----   0 fes       (1000) fes       (1000)     2593 2023-06-08 04:46:15.000000 medviz-1.0.5/medviz/plots/plot2d/masks.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.752736 medviz-1.0.5/medviz/plots/plot3d/
--rw-r-----   0 fes       (1000) fes       (1000)      205 2023-06-08 07:01:03.000000 medviz-1.0.5/medviz/plots/plot3d/__init__.py
--rw-r-----   0 fes       (1000) fes       (1000)     1890 2023-06-08 07:01:51.000000 medviz-1.0.5/medviz/plots/plot3d/image_mask_annotated.py
--rw-r--r--   0 fes       (1000) fes       (1000)     2339 2023-07-18 18:20:40.000000 medviz-1.0.5/medviz/plots/plot3d/image_masks.py
--rw-r-----   0 fes       (1000) fes       (1000)     3113 2023-06-08 04:47:31.000000 medviz-1.0.5/medviz/plots/plot3d/images.py
--rw-r-----   0 fes       (1000) fes       (1000)     2060 2023-05-31 20:21:55.000000 medviz-1.0.5/medviz/plots/plot3d/layered_plot.py
--rw-r-----   0 fes       (1000) fes       (1000)     3577 2023-06-08 06:34:09.000000 medviz-1.0.5/medviz/plots/plot3d/masks.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.756736 medviz-1.0.5/medviz/preprocess/
--rw-rw----   0 fes       (1000) fes       (1000)      258 2023-07-26 18:46:13.000000 medviz-1.0.5/medviz/preprocess/__init__.py
--rw-r-----   0 fes       (1000) fes       (1000)     2071 2023-07-16 03:13:55.000000 medviz-1.0.5/medviz/preprocess/mask.py
--rw-rw----   0 fes       (1000) fes       (1000)     2764 2023-06-03 02:10:07.000000 medviz-1.0.5/medviz/preprocess/match_image_mask.py
--rw-rw-r--   0 fes       (1000) fes       (1000)      423 2023-07-26 18:28:23.000000 medviz-1.0.5/medviz/preprocess/mha_resampling.py
--rw-r--r--   0 fes       (1000) fes       (1000)     1128 2023-07-26 18:42:33.000000 medviz-1.0.5/medviz/preprocess/read_mha.py
--rw-r--r--   0 fes       (1000) fes       (1000)     2226 2023-07-26 18:25:53.000000 medviz-1.0.5/medviz/preprocess/resampling.py
--rw-r--r--   0 fes       (1000) fes       (1000)     2521 2023-07-18 18:47:42.000000 medviz-1.0.5/medviz/preprocess/resampling_local.py
--rw-r--r--   0 fes       (1000) fes       (1000)     3132 2023-07-26 06:57:23.000000 medviz-1.0.5/medviz/preprocess/resampling_local_new.py
--rw-r--r--   0 fes       (1000) fes       (1000)     1320 2023-07-21 19:26:45.000000 medviz-1.0.5/medviz/preprocess/resampling_mha.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.756736 medviz-1.0.5/medviz/utils/
--rw-r-----   0 fes       (1000) fes       (1000)      614 2023-06-08 00:57:20.000000 medviz-1.0.5/medviz/utils/__init__.py
--rw-rw----   0 fes       (1000) fes       (1000)     2175 2023-05-13 17:59:38.000000 medviz-1.0.5/medviz/utils/array_profile.py
--rw-rw----   0 fes       (1000) fes       (1000)      662 2023-05-13 18:05:32.000000 medviz-1.0.5/medviz/utils/array_threshold.py
--rwxr-x---   0 fes       (1000) fes       (1000)     1069 2023-06-08 00:57:03.000000 medviz-1.0.5/medviz/utils/custom_type.py
--rw-r-----   0 fes       (1000) fes       (1000)     4587 2023-05-23 23:25:32.000000 medviz-1.0.5/medviz/utils/helper_mask.py
--rw-r-----   0 fes       (1000) fes       (1000)     2583 2023-07-18 18:20:40.000000 medviz-1.0.5/medviz/utils/helper_path.py
--rw-r-----   0 fes       (1000) fes       (1000)      689 2023-01-02 16:26:25.000000 medviz-1.0.5/medviz/utils/log.py
--rw-r-----   0 fes       (1000) fes       (1000)      859 2023-05-24 05:07:22.000000 medviz-1.0.5/medviz/utils/reader.py
--rwxr-x---   0 fes       (1000) fes       (1000)       80 2023-05-17 19:24:17.000000 medviz-1.0.5/medviz/utils/utility.py
-drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:48:02.744736 medviz-1.0.5/medviz.egg-info/
--rw-r-----   0 fes       (1000) fes       (1000)     2274 2023-07-26 18:48:02.000000 medviz-1.0.5/medviz.egg-info/PKG-INFO
--rw-r-----   0 fes       (1000) fes       (1000)     1596 2023-07-26 18:48:02.000000 medviz-1.0.5/medviz.egg-info/SOURCES.txt
--rw-r-----   0 fes       (1000) fes       (1000)        1 2023-07-26 18:48:02.000000 medviz-1.0.5/medviz.egg-info/dependency_links.txt
--rw-r-----   0 fes       (1000) fes       (1000)      222 2023-07-26 18:48:02.000000 medviz-1.0.5/medviz.egg-info/requires.txt
--rw-r-----   0 fes       (1000) fes       (1000)        7 2023-07-26 18:48:02.000000 medviz-1.0.5/medviz.egg-info/top_level.txt
--rw-r-----   0 fes       (1000) fes       (1000)     1405 2023-07-26 18:37:00.000000 medviz-1.0.5/pyproject.toml
--rw-rw-r--   0 fes       (1000) fes       (1000)       38 2023-07-26 18:48:02.756736 medviz-1.0.5/setup.cfg
--rw-r-----   0 fes       (1000) fes       (1000)      170 2023-04-02 14:20:15.000000 medviz-1.0.5/setup.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.266834 medviz-1.0.6/
+-rw-r-----   0 fes       (1000) fes       (1000)    36861 2023-05-31 20:04:32.000000 medviz-1.0.6/LICENSE
+-rw-r-----   0 fes       (1000) fes       (1000)      180 2023-06-01 05:23:25.000000 medviz-1.0.6/MANIFEST.in
+-rw-rw-r--   0 fes       (1000) fes       (1000)     2274 2023-07-26 18:55:59.266834 medviz-1.0.6/PKG-INFO
+-rw-r-----   0 fes       (1000) fes       (1000)     1803 2023-04-27 15:46:29.000000 medviz-1.0.6/README.rst
+-rw-r-----   0 fes       (1000) fes       (1000)        5 2023-07-26 18:55:41.000000 medviz-1.0.6/VERSION
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.254834 medviz-1.0.6/medviz/
+-rw-r-----   0 fes       (1000) fes       (1000)     2462 2023-07-26 18:55:49.000000 medviz-1.0.6/medviz/__init__.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.258834 medviz-1.0.6/medviz/collage/
+-rw-r-----   0 fes       (1000) fes       (1000)       41 2023-06-01 02:13:13.000000 medviz-1.0.6/medviz/collage/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     1982 2023-06-01 02:40:53.000000 medviz-1.0.6/medviz/collage/compute_collage.py
+-rw-r-----   0 fes       (1000) fes       (1000)    24895 2023-05-31 20:21:55.000000 medviz-1.0.6/medviz/collage/main.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2122 2023-06-01 02:47:15.000000 medviz-1.0.6/medviz/collage/stats.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.258834 medviz-1.0.6/medviz/multimodal/
+-rw-r-----   0 fes       (1000) fes       (1000)       85 2023-05-22 16:27:34.000000 medviz-1.0.6/medviz/multimodal/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     1065 2023-05-24 22:21:17.000000 medviz-1.0.6/medviz/multimodal/save_dicom_metadata.py
+-rw-r-----   0 fes       (1000) fes       (1000)      509 2023-05-22 16:27:37.000000 medviz-1.0.6/medviz/multimodal/stats.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.258834 medviz-1.0.6/medviz/nifti/
+-rw-rw-r--   0 fes       (1000) fes       (1000)       30 2023-07-26 03:32:59.000000 medviz-1.0.6/medviz/nifti/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     4377 2023-07-26 03:23:51.000000 medviz-1.0.6/medviz/nifti/helper.py
+-rw-rw-r--   0 fes       (1000) fes       (1000)     1664 2023-07-26 15:18:23.000000 medviz-1.0.6/medviz/nifti/metadata.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.258834 medviz-1.0.6/medviz/pkg2_local/
+-rw-r-----   0 fes       (1000) fes       (1000)      134 2023-05-23 22:19:26.000000 medviz-1.0.6/medviz/pkg2_local/example.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.258834 medviz-1.0.6/medviz/plots/
+-rw-r-----   0 fes       (1000) fes       (1000)      123 2023-05-23 23:18:05.000000 medviz-1.0.6/medviz/plots/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     1552 2023-05-18 02:42:18.000000 medviz-1.0.6/medviz/plots/_plot_image.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.258834 medviz-1.0.6/medviz/plots/gif/
+-rw-r-----   0 fes       (1000) fes       (1000)    10203 2023-05-24 04:19:50.000000 medviz-1.0.6/medviz/plots/gif/gif.py
+-rw-rw----   0 fes       (1000) fes       (1000)     2217 2023-05-25 02:41:16.000000 medviz-1.0.6/medviz/plots/helper_plot.py
+-rw-r-----   0 fes       (1000) fes       (1000)     3682 2023-05-24 04:19:50.000000 medviz-1.0.6/medviz/plots/layered_plot2D.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.262834 medviz-1.0.6/medviz/plots/plot2d/
+-rw-r-----   0 fes       (1000) fes       (1000)      238 2023-05-24 02:22:53.000000 medviz-1.0.6/medviz/plots/plot2d/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2139 2023-06-08 02:13:51.000000 medviz-1.0.6/medviz/plots/plot2d/image_mask_annotated.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2332 2023-06-08 02:13:23.000000 medviz-1.0.6/medviz/plots/plot2d/image_masks.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2359 2023-06-08 04:45:40.000000 medviz-1.0.6/medviz/plots/plot2d/images.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2593 2023-06-08 04:46:15.000000 medviz-1.0.6/medviz/plots/plot2d/masks.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.262834 medviz-1.0.6/medviz/plots/plot3d/
+-rw-r-----   0 fes       (1000) fes       (1000)      205 2023-06-08 07:01:03.000000 medviz-1.0.6/medviz/plots/plot3d/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     1890 2023-06-08 07:01:51.000000 medviz-1.0.6/medviz/plots/plot3d/image_mask_annotated.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     2339 2023-07-18 18:20:40.000000 medviz-1.0.6/medviz/plots/plot3d/image_masks.py
+-rw-r-----   0 fes       (1000) fes       (1000)     3113 2023-06-08 04:47:31.000000 medviz-1.0.6/medviz/plots/plot3d/images.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2060 2023-05-31 20:21:55.000000 medviz-1.0.6/medviz/plots/plot3d/layered_plot.py
+-rw-r-----   0 fes       (1000) fes       (1000)     3577 2023-06-08 06:34:09.000000 medviz-1.0.6/medviz/plots/plot3d/masks.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.262834 medviz-1.0.6/medviz/preprocess/
+-rw-rw----   0 fes       (1000) fes       (1000)      258 2023-07-26 18:46:13.000000 medviz-1.0.6/medviz/preprocess/__init__.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2071 2023-07-16 03:13:55.000000 medviz-1.0.6/medviz/preprocess/mask.py
+-rw-rw----   0 fes       (1000) fes       (1000)     2764 2023-06-03 02:10:07.000000 medviz-1.0.6/medviz/preprocess/match_image_mask.py
+-rw-rw-r--   0 fes       (1000) fes       (1000)      423 2023-07-26 18:28:23.000000 medviz-1.0.6/medviz/preprocess/mha_resampling.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     1128 2023-07-26 18:42:33.000000 medviz-1.0.6/medviz/preprocess/read_mha.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     2226 2023-07-26 18:25:53.000000 medviz-1.0.6/medviz/preprocess/resampling.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     2521 2023-07-18 18:47:42.000000 medviz-1.0.6/medviz/preprocess/resampling_local.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     3132 2023-07-26 06:57:23.000000 medviz-1.0.6/medviz/preprocess/resampling_local_new.py
+-rw-r--r--   0 fes       (1000) fes       (1000)     1320 2023-07-21 19:26:45.000000 medviz-1.0.6/medviz/preprocess/resampling_mha.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.266834 medviz-1.0.6/medviz/utils/
+-rw-r-----   0 fes       (1000) fes       (1000)      614 2023-06-08 00:57:20.000000 medviz-1.0.6/medviz/utils/__init__.py
+-rw-rw----   0 fes       (1000) fes       (1000)     2175 2023-05-13 17:59:38.000000 medviz-1.0.6/medviz/utils/array_profile.py
+-rw-rw----   0 fes       (1000) fes       (1000)      662 2023-05-13 18:05:32.000000 medviz-1.0.6/medviz/utils/array_threshold.py
+-rwxr-x---   0 fes       (1000) fes       (1000)     1069 2023-06-08 00:57:03.000000 medviz-1.0.6/medviz/utils/custom_type.py
+-rw-r-----   0 fes       (1000) fes       (1000)     4587 2023-05-23 23:25:32.000000 medviz-1.0.6/medviz/utils/helper_mask.py
+-rw-r-----   0 fes       (1000) fes       (1000)     2583 2023-07-18 18:20:40.000000 medviz-1.0.6/medviz/utils/helper_path.py
+-rw-r-----   0 fes       (1000) fes       (1000)      689 2023-01-02 16:26:25.000000 medviz-1.0.6/medviz/utils/log.py
+-rw-r-----   0 fes       (1000) fes       (1000)      859 2023-05-24 05:07:22.000000 medviz-1.0.6/medviz/utils/reader.py
+-rwxr-x---   0 fes       (1000) fes       (1000)       80 2023-05-17 19:24:17.000000 medviz-1.0.6/medviz/utils/utility.py
+drwxrwxr-x   0 fes       (1000) fes       (1000)        0 2023-07-26 18:55:59.254834 medviz-1.0.6/medviz.egg-info/
+-rw-r-----   0 fes       (1000) fes       (1000)     2274 2023-07-26 18:55:59.000000 medviz-1.0.6/medviz.egg-info/PKG-INFO
+-rw-r-----   0 fes       (1000) fes       (1000)     1596 2023-07-26 18:55:59.000000 medviz-1.0.6/medviz.egg-info/SOURCES.txt
+-rw-r-----   0 fes       (1000) fes       (1000)        1 2023-07-26 18:55:59.000000 medviz-1.0.6/medviz.egg-info/dependency_links.txt
+-rw-r-----   0 fes       (1000) fes       (1000)      223 2023-07-26 18:55:59.000000 medviz-1.0.6/medviz.egg-info/requires.txt
+-rw-r-----   0 fes       (1000) fes       (1000)        7 2023-07-26 18:55:59.000000 medviz-1.0.6/medviz.egg-info/top_level.txt
+-rw-r-----   0 fes       (1000) fes       (1000)     1406 2023-07-26 18:55:37.000000 medviz-1.0.6/pyproject.toml
+-rw-rw-r--   0 fes       (1000) fes       (1000)       38 2023-07-26 18:55:59.266834 medviz-1.0.6/setup.cfg
+-rw-r-----   0 fes       (1000) fes       (1000)      170 2023-04-02 14:20:15.000000 medviz-1.0.6/setup.py
```

### Comparing `medviz-1.0.5/LICENSE` & `medviz-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/PKG-INFO` & `medviz-1.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 1.0.5
+Version: 1.0.6
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-1.0.5/README.rst` & `medviz-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/__init__.py` & `medviz-1.0.6/medviz/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,8 +91,8 @@
 #         version = f.read().strip()
 #     return version
 
 # __version__ = version()
 
 
 
-__version__ = "1.0.5"
+__version__ = "1.0.6"
```

### Comparing `medviz-1.0.5/medviz/collage/compute_collage.py` & `medviz-1.0.6/medviz/collage/compute_collage.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/collage/main.py` & `medviz-1.0.6/medviz/collage/main.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/collage/stats.py` & `medviz-1.0.6/medviz/collage/stats.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/multimodal/save_dicom_metadata.py` & `medviz-1.0.6/medviz/multimodal/save_dicom_metadata.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/nifti/helper.py` & `medviz-1.0.6/medviz/nifti/helper.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/nifti/metadata.py` & `medviz-1.0.6/medviz/nifti/metadata.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/_plot_image.py` & `medviz-1.0.6/medviz/plots/_plot_image.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/gif/gif.py` & `medviz-1.0.6/medviz/plots/gif/gif.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/helper_plot.py` & `medviz-1.0.6/medviz/plots/helper_plot.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/layered_plot2D.py` & `medviz-1.0.6/medviz/plots/layered_plot2D.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/plot2d/image_mask_annotated.py` & `medviz-1.0.6/medviz/plots/plot2d/image_mask_annotated.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/plot2d/image_masks.py` & `medviz-1.0.6/medviz/plots/plot2d/image_masks.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/plot2d/images.py` & `medviz-1.0.6/medviz/plots/plot2d/images.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/plot2d/masks.py` & `medviz-1.0.6/medviz/plots/plot2d/masks.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/plot3d/image_mask_annotated.py` & `medviz-1.0.6/medviz/plots/plot3d/image_mask_annotated.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/plot3d/image_masks.py` & `medviz-1.0.6/medviz/plots/plot3d/image_masks.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/plot3d/images.py` & `medviz-1.0.6/medviz/plots/plot3d/images.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/plot3d/layered_plot.py` & `medviz-1.0.6/medviz/plots/plot3d/layered_plot.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/plots/plot3d/masks.py` & `medviz-1.0.6/medviz/plots/plot3d/masks.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/preprocess/mask.py` & `medviz-1.0.6/medviz/preprocess/mask.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/preprocess/match_image_mask.py` & `medviz-1.0.6/medviz/preprocess/match_image_mask.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/preprocess/read_mha.py` & `medviz-1.0.6/medviz/preprocess/read_mha.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/preprocess/resampling.py` & `medviz-1.0.6/medviz/preprocess/resampling.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/preprocess/resampling_local.py` & `medviz-1.0.6/medviz/preprocess/resampling_local.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/preprocess/resampling_local_new.py` & `medviz-1.0.6/medviz/preprocess/resampling_local_new.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/preprocess/resampling_mha.py` & `medviz-1.0.6/medviz/preprocess/resampling_mha.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/utils/__init__.py` & `medviz-1.0.6/medviz/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/utils/array_profile.py` & `medviz-1.0.6/medviz/utils/array_profile.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/utils/array_threshold.py` & `medviz-1.0.6/medviz/utils/array_threshold.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/utils/custom_type.py` & `medviz-1.0.6/medviz/utils/custom_type.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/utils/helper_mask.py` & `medviz-1.0.6/medviz/utils/helper_mask.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/utils/helper_path.py` & `medviz-1.0.6/medviz/utils/helper_path.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/utils/log.py` & `medviz-1.0.6/medviz/utils/log.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz/utils/reader.py` & `medviz-1.0.6/medviz/utils/reader.py`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/medviz.egg-info/PKG-INFO` & `medviz-1.0.6/medviz.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medviz
-Version: 1.0.5
+Version: 1.0.6
 Summary: Medical Image Visualization Tool 🐍🚀🎉🦕
 Author-email: Mohsen Hariri <mohsen.hariri@case.eud>
 License: GPL-3.0 License
 Keywords: MRI,CT
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `medviz-1.0.5/medviz.egg-info/SOURCES.txt` & `medviz-1.0.6/medviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medviz-1.0.5/pyproject.toml` & `medviz-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   "nibabel >= 3.2.1",
   "imageio >= 2.9.0",
   "scikit-image >= 0.18.3",
   "tabulate >= 0.8.9",
   "pydicom >= 2.1.2",
   "mahotas >= 1.4.11",
   "SimpleITK >= 2.1.1",
-  "torchie >= 0.1.2",
+  "torchio >= 0.19.0",
 ]
 
 [tool.setuptools]
 packages = ["medviz", "medviz.multimodal", "medviz.preprocess"]
 
 
 [tool.setuptools.dynamic]
```

