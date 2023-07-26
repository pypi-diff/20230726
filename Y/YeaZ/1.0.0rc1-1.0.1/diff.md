# Comparing `tmp/YeaZ-1.0.0rc1.tar.gz` & `tmp/YeaZ-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "YeaZ-1.0.0rc1.tar", last modified: Tue Jul 25 19:25:37 2023, max compression
+gzip compressed data, was "YeaZ-1.0.1.tar", last modified: Wed Jul 26 13:52:50 2023, max compression
```

## Comparing `YeaZ-1.0.0rc1.tar` & `YeaZ-1.0.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 19:25:37.824975 YeaZ-1.0.0rc1/
--rw-rw-rw-   0        0        0   573440 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/.coverage
--rw-rw-rw-   0        0        0     2236 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/.gitignore
--rw-rw-rw-   0        0        0     1095 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/LICENSE
--rw-rw-rw-   0        0        0    17083 2023-07-25 19:25:37.825972 YeaZ-1.0.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0    15662 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 19:25:37.761145 YeaZ-1.0.0rc1/YeaZ.egg-info/
--rw-rw-rw-   0        0        0    17083 2023-07-25 19:25:37.000000 YeaZ-1.0.0rc1/YeaZ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1188 2023-07-25 19:25:37.000000 YeaZ-1.0.0rc1/YeaZ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 19:25:37.000000 YeaZ-1.0.0rc1/YeaZ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-25 19:25:37.000000 YeaZ-1.0.0rc1/YeaZ.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      274 2023-07-25 19:25:37.000000 YeaZ-1.0.0rc1/YeaZ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-25 19:25:37.000000 YeaZ-1.0.0rc1/YeaZ.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-25 19:25:37.767130 YeaZ-1.0.0rc1/example_data/
--rw-rw-rw-   0        0        0  1490384 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/example_data/2020_3_19_frame_100_cropped.tif
--rw-rw-rw-   0        0        0       71 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/example_data/readme.md
--rw-rw-rw-   0        0        0      328 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/pyproject.toml
--rw-rw-rw-   0        0        0      255 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/requirements.txt
--rw-rw-rw-   0        0        0     1712 2023-07-25 19:25:37.826969 YeaZ-1.0.0rc1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 19:25:37.777130 YeaZ-1.0.0rc1/yeaz/
--rw-rw-rw-   0        0        0    77932 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/GUI_main.py
--rw-rw-rw-   0        0        0     5645 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/Launch_NN_command_line.py
--rw-rw-rw-   0        0        0        0 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/__init__.py
--rw-rw-rw-   0        0        0     2422 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/__main__.py
--rw-rw-rw-   0        0        0      167 2023-07-25 19:25:37.000000 YeaZ-1.0.0rc1/yeaz/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:25:37.783115 YeaZ-1.0.0rc1/yeaz/disk/
--rw-rw-rw-   0        0        0     5626 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/disk/DialogFileBrowser.py
--rw-rw-rw-   0        0        0    16603 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/disk/Reader.py
--rw-rw-rw-   0        0        0        0 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/disk/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/disk/image_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:25:37.796052 YeaZ-1.0.0rc1/yeaz/icons/
--rw-rw-rw-   0        0        0     3988 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/icons/HomeIcon.png
--rw-rw-rw-   0        0        0      403 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/icons/LeftArrowIcon.png
--rw-rw-rw-   0        0        0      533 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/icons/MoveArrowsIcon.png
--rw-rw-rw-   0        0        0      399 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/icons/RightArrowIcon.png
--rw-rw-rw-   0        0        0      418 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/icons/ZoomIcon.png
--rw-rw-rw-   0        0        0        0 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/icons/__init__.py
--rw-rw-rw-   0        0        0     1201 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/icons/brush2.png
--rw-rw-rw-   0        0        0      884 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/icons/eraser.png
-drwxrwxrwx   0        0        0        0 2023-07-25 19:25:37.802037 YeaZ-1.0.0rc1/yeaz/init/
--rw-rw-rw-   0        0        0    11461 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/init/InitButtons.py
--rw-rw-rw-   0        0        0     2571 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/init/InitLayout.py
--rw-rw-rw-   0        0        0        0 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/init/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:25:37.812009 YeaZ-1.0.0rc1/yeaz/misc/
--rw-rw-rw-   0        0        0     1449 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/misc/BatchRetrack.py
--rw-rw-rw-   0        0        0     1699 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/misc/ChangeOneCellValue.py
--rw-rw-rw-   0        0        0     1693 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/misc/ExchangeCellValues.py
--rw-rw-rw-   0        0        0    15906 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/misc/Extract.py
--rw-rw-rw-   0        0        0    23716 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/misc/PlotCanvas.py
--rw-rw-rw-   0        0        0     1278 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/misc/ProgressBar.py
--rw-rw-rw-   0        0        0        0 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/misc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:25:37.823977 YeaZ-1.0.0rc1/yeaz/unet/
--rw-rw-rw-   0        0        0     3068 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/unet/LaunchBatchPrediction.py
--rw-rw-rw-   0        0        0        0 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/unet/__init__.py
--rw-rw-rw-   0        0        0     4251 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/unet/hungarian.py
--rw-rw-rw-   0        0        0     4706 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/unet/model_pytorch.py
--rw-rw-rw-   0        0        0     3881 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/unet/model_tensorflow.py
--rw-rw-rw-   0        0        0     4214 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/unet/neural_network.py
--rw-rw-rw-   0        0        0     6331 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/unet/segment.py
--rw-rw-rw-   0        0        0     1576 2023-07-25 19:25:19.000000 YeaZ-1.0.0rc1/yeaz/unet/utils.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.722675 YeaZ-1.0.1/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)   573440 2023-07-26 13:51:44.000000 YeaZ-1.0.1/.coverage
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     2091 2023-07-26 13:51:44.000000 YeaZ-1.0.1/.gitignore
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1074 2023-07-26 13:51:44.000000 YeaZ-1.0.1/LICENSE
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    16986 2023-07-26 13:52:50.722850 YeaZ-1.0.1/PKG-INFO
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    15602 2023-07-26 13:51:44.000000 YeaZ-1.0.1/README.md
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.712077 YeaZ-1.0.1/YeaZ.egg-info/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    16986 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/PKG-INFO
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1188 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/SOURCES.txt
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        1 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/dependency_links.txt
+-rw-r--r--   0 farzanehwork   (502) staff       (20)       43 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/entry_points.txt
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      274 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/requires.txt
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        5 2023-07-26 13:52:50.000000 YeaZ-1.0.1/YeaZ.egg-info/top_level.txt
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.714470 YeaZ-1.0.1/example_data/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)  1490384 2023-07-26 13:51:44.000000 YeaZ-1.0.1/example_data/2020_3_19_frame_100_cropped.tif
+-rw-r--r--   0 farzanehwork   (502) staff       (20)       67 2023-07-26 13:51:44.000000 YeaZ-1.0.1/example_data/readme.md
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      311 2023-07-26 13:51:44.000000 YeaZ-1.0.1/pyproject.toml
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      253 2023-07-26 13:51:44.000000 YeaZ-1.0.1/requirements.txt
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1641 2023-07-26 13:52:50.723527 YeaZ-1.0.1/setup.cfg
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.715845 YeaZ-1.0.1/yeaz/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    76187 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/GUI_main.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     5521 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/Launch_NN_command_line.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/__init__.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     2354 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/__main__.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      160 2023-07-26 13:52:50.000000 YeaZ-1.0.1/yeaz/_version.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.716702 YeaZ-1.0.1/yeaz/disk/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     5495 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/disk/DialogFileBrowser.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    17565 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/disk/Reader.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/disk/__init__.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1623 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/disk/image_loader.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.718222 YeaZ-1.0.1/yeaz/icons/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     3988 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/HomeIcon.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      403 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/LeftArrowIcon.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      533 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/MoveArrowsIcon.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      399 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/RightArrowIcon.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      418 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/ZoomIcon.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/__init__.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1201 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/brush2.png
+-rw-r--r--   0 farzanehwork   (502) staff       (20)      884 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/icons/eraser.png
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.718778 YeaZ-1.0.1/yeaz/init/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    11215 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/init/InitButtons.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     2505 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/init/InitLayout.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/init/__init__.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.720524 YeaZ-1.0.1/yeaz/misc/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1418 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/BatchRetrack.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1655 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/ChangeOneCellValue.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1650 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/ExchangeCellValues.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    15475 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/Extract.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)    23157 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/PlotCanvas.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1239 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/ProgressBar.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/misc/__init__.py
+drwxr-xr-x   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:52:50.722483 YeaZ-1.0.1/yeaz/unet/
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     2991 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/LaunchBatchPrediction.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)        0 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/__init__.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     4114 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/hungarian.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     4586 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/model_pytorch.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     3819 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/model_tensorflow.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     4088 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/neural_network.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     6163 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/segment.py
+-rw-r--r--   0 farzanehwork   (502) staff       (20)     1537 2023-07-26 13:51:44.000000 YeaZ-1.0.1/yeaz/unet/utils.py
```

### Comparing `YeaZ-1.0.0rc1/.coverage` & `YeaZ-1.0.1/.coverage`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.0rc1/PKG-INFO` & `YeaZ-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,201 +1,170 @@
-Metadata-Version: 2.1
-Name: YeaZ
-Version: 1.0.0rc1
-Summary: Deep-learning based yeast cell segmentation
-Home-page: https://github.com/rahi-lab/YeaZ-GUI
-Author: Sahand Jamal Rahi
-Author-email: sahand.rahi@epfl.ch
-Project-URL: Rahi lab, https://www.epfl.ch/labs/lpbs/
-Keywords: live-cell imaging,cell segmentation,cell tracking,image analysis
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: gui
-Provides-Extra: tensorflow
-Provides-Extra: torch
-License-File: LICENSE
-
-# YeaZ
-
-This is the user manual for the graphical interface for segmenting yeast images using the YeaZ convolutional neural network. You can find the training set with the segmented training images here: https://www.quantsysbio.com/data-and-software/. 
-
-Want to try out the neural network without installing any software? Check out our online segmentation tool at https://lpbs-nn.epfl.ch/.
-
-## Latest updates
-
-18.04.2023:
-
-1. Update all dependencies to the latest versions
-2. Update PyQt to PyQt6, enabling the application to run on machines with m1 or m2 processors
-3. Add the ability to retrack multiple frames together
-4. Replace the old TensorFlow model with a PyTorch model
-5. Optimize the application's speed when showing cell numbers
-6. Improve the overall speed and performance of the application
-7. Add the ability to segment fission images
-8. Fix minor bugs and improve overall stability
-9. enable the option to run on GPU (windows and linux only)
-
-
-## Installation
-
-### System requirements
-
-The software requires a standard computer with enough RAM to apply the neural network. 8 GB RAM is enough to predict the 700 x 500 px image provided as the test data. The RAM requirements scales linearly with the number of image pixels.
-
-It was tested on OS X High Sierra (10.13.6), Windows 10 Education, and Ubuntu 18.04.4.
-
-Package dependencies: The convolutional neural network relies on Keras with TensorFlow. The Hungarian algorithm is implemented in the munkres package. In addition, standard image processing and scientific computing libraries are used. 
-
-Installation time is less than 5 minutes. 
-
-### Installation Steps
-
-1. Download the parameters for the neural network:
-    2.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b. Put the file in the folder `/unet`.  
-    2.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0. Put the file in the folder `/unet`.  
-    2.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/15Egg0zXSAFHD34a0urbthStIxlb4Q_G%5f. Put the file in the folder `/unet`.  
-
-### Install from PyPi
-
-1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
-2. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`. 
-3. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
-    3.1. for more information visit https://pytorch.org/get-started/locally/
-4. Install YeaZ with the command `pip install yeaz`.
-
-### Install from source
-
-1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
-2. Clone this repository (`git clone https://github.com/rahi-lab/YeaZ-GUI`).
-3. In the command line, navigate to the folder where you cloned YeaZ-GUI (command `cd YeaZ-GUI`).
-4. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`.   
-5. Activate the environment using `conda activate YeaZ`. 
-6. Install with the command `pip install -e .`.
-7. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
-    7.1. for more information visit https://pytorch.org/get-started/locally/
-
-## Runnig the GUI
-
-1. Open a terminal and activate the environment using `conda activate YeaZ`. 
-2. Run the program with the command `yeaz`.
-
-## Troubleshooting / FAQ 
-
-### Memory error when running on GPU (cuda). Also might happen on CPU.
-
-Unlike CPU, GPU memory is very limited. If you get a memory error when running on GPU, try the following steps:
-1. Crop the images to smaller sizes. Memory usage depends on number of pixels in your images. You may try cropping your images into several smaller images or removing empty space around cells.
-2. Another application might be using the GPU memory. Try to close all other applications and run the program again. You can also check applications that use GPU memory using the task manager (windows) or `nvidia-smi` command (linux).
-3. Try running on CPU or on a cluster with more GPU memory.
-
-### The application is running on CPU instead of GPU
-
-if you have specified running on GPU and the application is running on CPU instead, this might be due to the following reasons:
-1. you don't have a cuda compatible gpu. check the list of cuda-compatible gpus here: https://developer.nvidia.com/cuda-gpus
-2. you are using mac os with m1 or m2 processors. Unfortunately, the current version of PyTorch implementation does not fully support Mac M1 or M2 GPUs. In the meantime, you can still run your program on Mac M1 or M2 CPUs, which are quite powerful and can provide significant performance gains over traditional CPUs.
-3. you have not installed cuda. please follow the installation steps above to install cuda (run `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`).
-
-### Small buds are not recognized as cells
-
-If small buds aren't recognized as cells in your image, this is likely linked to a segmentation parameter that is too high. Relaunching the CNN with a smaller parameter will likely yield better results.
-
-### I just want the CNN, but not the GUI
-
-In case you only want to use the functionalities of the convolutional neural network and the segmentation, but not the full GUI, you only need the files `unet/model_pytorch.py`, `unet/neural_network.py` (for making predictions), `unet/segment.py` (for doing watershed segmentation) and `unet/hungarian.py` (for tracking), as well as the weights for the neural network which have to be in the same folder. You can create predictions using the `prediction` function in `neural_network.py` (note that before making predictions, you have to use the function `equalize_adapthist` from `skimage.exposure` on the image). The segmentations can be obtained with the `segment` function in `segment.py`, and tracking between two frames is done using the `correspondence` function in `hungarian.py`.
-You can also run `Launch_NN_comand_Line.py` and give input arguments to run the whole pipeline and save final mask. Here is an example for running the CNN on a phase contrast image:
-`python Launch_NN_command_line.py -i "example_data/2020_3_19_frame_100_cropped.tif" -m "newmaskfile.h5" --image_type  "pc" --device "cuda" --range_of_frames 0 0 --`
-
-### CNN performs less well on bright-field images
-
-Our CNN was trained on fewer cells with the bright-field technique (3841 unique cells imaged with 6 different exposure levels versus >8000 for phase contrast).
-
-### Graphical user interface not working on Mac OS Big Sur
-
-Jordan Xiao of Stanford University pointed out that one of the python modules (Pyqt) has some issues on Mac OS Big Sur. Check out https://stackoverflow.com/questions/64833558/apps-not-popping-up-on-macos-big-sur-11-0-1 and https://stackoverflow.com/questions/64818879/is-there-any-solution-regarding-to-pyqt-library-doesnt-work-in-mac-os-big-sur/64856281 for more information and possible fixes.
-
-## User Guide
-
-### Launching the Program
-
-Upon starting the program, it prompts you to select your images and your (new) mask file. There are two ways to select images: One can directly select a single image file using the button `Open image file`. Currently, we support Nikon `.nd2` files and multi-stack `.tif` files in addition to all standard formats such as `.png`, `.jpg`, or `.tif`. One can also select a folder of image files using the button `Open image folder`. This takes every single image in the folder to be a frame in a timelapse recording of yeast cells. The folder must contain images that all have the same size. 
-
-The program will save segmentation masks in `.h5` files. You can either create a new file by specifying its name in the text box or if you already have an h5 file for a specific set of images, you can select it using `Open mask file`. Note that when using an existing `.h5` file, you also have to use the same images as you did at its creation.
-
-### The Interface
-
-After clicking OK in the launcher, the main program will open. It consists of an image display of three images, the current image in the middle, the previous one to the left and the next image to the right. This display was chosen to easily be able to check whether the cell numbers and the segmentations are consistent throughout time.
-
-On the very bottom of the program, there is a status bar which displays the state of the program. In addition, when hovering over a button, it gives detailed information about what the button does and how to use it.
-
-On the top left of the three images, there are multiple buttons that allow the user to use pan and zoom to navigate through the image. The home button to the very left allows to reset zoom and pan, while the arrows allow to go to the next and previous pan/zoom positions. 
-
-On the bottom of the images, there are three rows of buttons. The first row of buttons allows the user to select the field of view, color channel, and time frame. Note that support for multiple fields of view and color channels is currently only available when opening .nd2 files. The second row contains tools to make edits to the mask, in order to correct the mistakes of the CNN. Moreover, it allows to show or hide the segmentation mask and the cell numbers. On the bottom right, the buttons allow to launch the CNN, to recalculate the tracking, and to extract the fluorescence or segmentation masks.
-
-### Launching the CNN
-
-After opening a new image file, the next step is typically to launch the convolutional neural network with the `Launch CNN` button. Note that if you are using a file with multiple color channels, this has to be done with the brightfield channel visible. This will open a dialog box, in which you can specify the time frames that you want to launch the CNN on as well as the field of view you want to use and type of your images. 
-
-Moreover, it lets you specify two parameters: The **threshold value** specifies the predicted value above which a pixel is considered to belong to a cell. This value is set at 0.5 per default and doesn't have to be changed in our experience. Increasing this value will decrease the sizes of the cells and can come in handy if the cells tend to exceed their borders. The **segmentation parameter** tells the program how far away two cell centers have to be at least, in order for two cells to be considered as separate entities. It has to be adjusted depending on how large the image resolution is: For small resolutions, a value of 2 seems to work well, whereas 5 is good for higher resolutions.
-
-### Making edits to the mask
-
-After the CNN has run, it is possible to correct the mistakes it has made. This can be done in the following ways:
-
-`Add region`: Add a region to an existing cell, by defining a polygon. First left-click on the cell to which you want to add a region, then continue clicking to draw a polygon to add. Finally click on the button again to confirm.
-
-`New cell`: This works similar to `Add region` but defines a new cell. Draw a polygon using left-clicks and re-click the button to confirm.
-
-`Brush`: This is an alternative way to add to a cell. The user right-clicks to select the cell to draw. Then the user can click and drag to draw the cell. The brush size can be controlled using the spin-box to the right.
-
-`Eraser`: This can be used to remove a region from a cell. The use is the same as for `Brush`.
-
-`Exchange cell IDs`: This allows correction of cell ID values by switching two cells. 
-
-`Change cell ID`: This allows changing the ID number of a cell. **Important: **If you change the number to the number of another cell, those two cells will from now on be considered as one single cell. This is useful for fusing cells that were oversegmented but has to be used with care.
-
-`Retrack`: Having made edits to a frame, the cell numbers may no longer correspond in the next frame. This can be automatically fixed by navigating to the next frame and clicking the retrack button.
-
-### Extracting the results
-
-After the masks are satisfactory for a given field of view, you can click on the `Extract` button to export the results. There are two ways the results can be exported: Firstly, the masks that were found can be exported as multistack TIFF files. Secondly, the fluorescence together with several statistics giving information about every individual cell can be extracted and saved as a `.csv` file. 
-
-Moreover, you may only be interested in a subset of the cells visible in the image, which is why this second window allows you to select the cells which you are interested in. You can select or deselect multiple cells by drawing a polygon around them and confirming with a right-click, or select and deselect single cells by just left-clicking them. Note that the image that is displayed corresponds to the last frame for which you have a mask. Cells which disappeared throughout the timelapse video - and thus are not part of the mask - will be exported as well but indicated with a flag in the exported fluorescence csv. 
-
-When you want to extract fluorescence, you can add files from which to extract fluorescence by clicking the `Add` button. There you can either add a single image file, a multistack TIFF file, or a folder containing image files. Note that if multiple files or frames are used, the fluorescence file or folder must have the same amount of images as the image given to the program at startup.
-
-The output csv contains one line for every combination of cells, timeframe, and channel. This allows the file easily to be read into pandas, and avoids a varying amount of columns depending on how many fluorescence channels are used. The following statistics are exported: The *area* of the cell, the *mean* intensity, the intensity *variance*, the *total intensity*, and the x and y coordinates of the *center of mass*. Moreover, the major and minor axes of the cells are found using principal component analysis. In particular, the *angle* of the major axis to the x axis is given, together with the *length* of the major and minor axis, thus, fully specifying an ellipsoid approximating the cell. Finally, we report whether the cell disappears, i.e., whether or not it is present in the last frame. 
-
-### Running the demo
-
-We guide you step-by-step through the demo:
-
-1. In the startup dialog, click `Open image file` and select the file in the `example_data` folder from within the file dialog.
-2. Give a name to the h5 mask file, such as example_data.h5. Press `OK` to confirm.
-3. We want to predict the segmentation. Click `Launch CNN`. In the pop-up dialog. Enter 0 and 0 as the time bounds. Select the Field of View 1 by clicking on it. Press `OK`. 
-4. Wait for the neural network to predict. This takes about 1 min on a standard computer. 
-5. Now go through the image to verify the predictions and correct mistakes as needed. Instructions about how to use every tool is shown in the status bar at the bottom when you hover over the tool button. 
-6. Click `Extract` if you are satisfied. Extract the mask or the cell statistics, specify a file name, and you're done! In case you wanted additional fluorescence channels or only extract a subset of cells, you could also do this here using the corresponding buttons.
-
-
-
-
-
-`
-
+# YeaZ
+
+This is the user manual for the graphical interface for segmenting yeast images using the YeaZ convolutional neural network. You can find the training set with the segmented training images here: https://www.quantsysbio.com/data-and-software/. 
+
+Want to try out the neural network without installing any software? Check out our online segmentation tool at https://lpbs-nn.epfl.ch/.
+
+## Latest updates
+26.07.2023:
+1. Updata the installation structure
+2. Packaging and upload on Pypi.
+
+18.04.2023:
+
+1. Update all dependencies to the latest versions
+2. Update PyQt to PyQt6, enabling the application to run on machines with m1 or m2 processors
+3. Add the ability to retrack multiple frames together
+4. Replace the old TensorFlow model with a PyTorch model
+5. Optimize the application's speed when showing cell numbers
+6. Improve the overall speed and performance of the application
+7. Add the ability to segment fission images
+8. Fix minor bugs and improve overall stability
+9. enable the option to run on GPU (windows and linux only)
+
+
+## Installation
+
+### System requirements
+
+The software requires a standard computer with enough RAM to apply the neural network. 8 GB RAM is enough to predict the 700 x 500 px image provided as the test data. The RAM requirements scale linearly with the number of image pixels.
+
+It was tested on macOS Ventura (13.4.1), Windows 10 Education, and Ubuntu 20.04.4.
+
+Package dependencies: The convolutional neural network relies on Pytorch. The Hungarian algorithm is implemented in the munkres package. In addition, standard image processing and scientific computing libraries are used. 
+
+Installation time is less than 5 minutes. 
+
+### Download weight files for neural network
+
+1. Download the parameters for the neural network:<br>
+    1.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b. Put the file in the folder `yeaz/unet`.  <br>
+    1.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0. Put the file in the folder `yeaz/unet`.  <br>
+    1.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS. Put the file in the folder `yeaz/unet`.  
+
+### Install from PyPi
+
+1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
+2. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`. 
+3. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    3.1. for more information visit https://pytorch.org/get-started/locally/
+4. Install YeaZ with the command `pip install yeaz`.
+
+### Install from source
+
+1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
+2. Clone this repository (`git clone https://github.com/rahi-lab/YeaZ-GUI`).
+3. In the command line, navigate to the folder where you cloned YeaZ-GUI (command `cd YeaZ-GUI`).
+4. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`.   
+5. Activate the environment using `conda activate YeaZ`. 
+6. Install with the command `pip install -e .`.
+7. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    7.1. for more information visit https://pytorch.org/get-started/locally/
+
+## Runnig the GUI
+
+1. Open a terminal and activate the environment using `conda activate YeaZ`. 
+2. Run the program with the command `yeaz`.
+
+## Troubleshooting / FAQ 
+
+### Memory error when running on GPU (cuda). Also might happen on CPU.
+
+Unlike CPU, GPU memory is very limited. If you get a memory error when running on GPU, try the following steps:
+1. Crop the images to smaller sizes. Memory usage depends on number of pixels in your images. You may try cropping your images into several smaller images or removing empty space around cells.
+2. Another application might be using the GPU memory. Try to close all other applications and run the program again. You can also check applications that use GPU memory using the task manager (windows) or `nvidia-smi` command (linux).
+3. Try running on CPU or on a cluster with more GPU memory.
+
+### The application is running on CPU instead of GPU
+
+if you have specified running on GPU and the application is running on CPU instead, this might be due to the following reasons:
+1. you don't have a cuda compatible gpu. check the list of cuda-compatible gpus here: https://developer.nvidia.com/cuda-gpus
+2. you are using mac os with m1 or m2 processors. Unfortunately, the current version of PyTorch implementation does not fully support Mac M1 or M2 GPUs. In the meantime, you can still run your program on Mac M1 or M2 CPUs, which are quite powerful and can provide significant performance gains over traditional CPUs.
+3. you have not installed cuda. please follow the installation steps above to install cuda (run `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`).
+
+### Small buds are not recognized as cells
+
+If small buds aren't recognized as cells in your image, this is likely linked to a segmentation parameter that is too high. Relaunching the CNN with a smaller parameter will likely yield better results.
+
+### I just want the CNN, but not the GUI
+
+In case you only want to use the functionalities of the convolutional neural network and the segmentation, but not the full GUI, you only need the files `unet/model_pytorch.py`, `unet/neural_network.py` (for making predictions), `unet/segment.py` (for doing watershed segmentation) and `unet/hungarian.py` (for tracking), as well as the weights for the neural network which have to be in the same folder. You can create predictions using the `prediction` function in `neural_network.py` (note that before making predictions, you have to use the function `equalize_adapthist` from `skimage.exposure` on the image). The segmentations can be obtained with the `segment` function in `segment.py`, and tracking between two frames is done using the `correspondence` function in `hungarian.py`.
+You can also run `Launch_NN_comand_Line.py` and give input arguments to run the whole pipeline and save final mask. Here is an example for running the CNN on a phase contrast image:
+`python Launch_NN_command_line.py -i "example_data/2020_3_19_frame_100_cropped.tif" -m "newmaskfile.h5" --image_type  "pc" --device "cuda" --range_of_frames 0 0 --`
+
+### CNN performs less well on bright-field images
+
+Our CNN was trained on fewer cells with the bright-field technique (3841 unique cells imaged with 6 different exposure levels versus >8000 for phase contrast).
+
+### Graphical user interface not working on Mac OS Big Sur
+
+Jordan Xiao of Stanford University pointed out that one of the python modules (Pyqt) has some issues on Mac OS Big Sur. Check out https://stackoverflow.com/questions/64833558/apps-not-popping-up-on-macos-big-sur-11-0-1 and https://stackoverflow.com/questions/64818879/is-there-any-solution-regarding-to-pyqt-library-doesnt-work-in-mac-os-big-sur/64856281 for more information and possible fixes.
+
+## User Guide
+
+### Launching the Program
+
+Upon starting the program, it prompts you to select your images and your (new) mask file. There are two ways to select images: One can directly select a single image file using the button `Open image file`. Currently, we support Nikon `.nd2` files and multi-stack `.tif` files in addition to all standard formats such as `.png`, `.jpg`, or `.tif`. One can also select a folder of image files using the button `Open image folder`. This takes every single image in the folder to be a frame in a timelapse recording of yeast cells. The folder must contain images that all have the same size. 
+
+The program will save segmentation masks in `.h5` files. You can either create a new file by specifying its name in the text box or if you already have an h5 file for a specific set of images, you can select it using `Open mask file`. Note that when using an existing `.h5` file, you also have to use the same images as you did at its creation.
+
+### The Interface
+
+After clicking OK in the launcher, the main program will open. It consists of an image display of three images, the current image in the middle, the previous one to the left and the next image to the right. This display was chosen to easily be able to check whether the cell numbers and the segmentations are consistent throughout time.
+
+On the very bottom of the program, there is a status bar which displays the state of the program. In addition, when hovering over a button, it gives detailed information about what the button does and how to use it.
+
+On the top left of the three images, there are multiple buttons that allow the user to use pan and zoom to navigate through the image. The home button to the very left allows to reset zoom and pan, while the arrows allow to go to the next and previous pan/zoom positions. 
+
+On the bottom of the images, there are three rows of buttons. The first row of buttons allows the user to select the field of view, color channel, and time frame. Note that support for multiple fields of view and color channels is currently only available when opening .nd2 files. The second row contains tools to make edits to the mask, in order to correct the mistakes of the CNN. Moreover, it allows to show or hide the segmentation mask and the cell numbers. On the bottom right, the buttons allow to launch the CNN, to recalculate the tracking, and to extract the fluorescence or segmentation masks.
+
+### Launching the CNN
+
+After opening a new image file, the next step is typically to launch the convolutional neural network with the `Launch CNN` button. Note that if you are using a file with multiple color channels, this has to be done with the brightfield channel visible. This will open a dialog box, in which you can specify the time frames that you want to launch the CNN on as well as the field of view you want to use and type of your images. 
+
+Moreover, it lets you specify two parameters: The **threshold value** specifies the predicted value above which a pixel is considered to belong to a cell. This value is set at 0.5 per default and doesn't have to be changed in our experience. Increasing this value will decrease the sizes of the cells and can come in handy if the cells tend to exceed their borders. The **segmentation parameter** tells the program how far away two cell centers have to be at least, in order for two cells to be considered as separate entities. It has to be adjusted depending on how large the image resolution is: For small resolutions, a value of 2 seems to work well, whereas 5 is good for higher resolutions.
+
+### Making edits to the mask
+
+After the CNN has run, it is possible to correct the mistakes it has made. This can be done in the following ways:
+
+`Add region`: Add a region to an existing cell, by defining a polygon. First left-click on the cell to which you want to add a region, then continue clicking to draw a polygon to add. Finally click on the button again to confirm.
+
+`New cell`: This works similar to `Add region` but defines a new cell. Draw a polygon using left-clicks and re-click the button to confirm.
+
+`Brush`: This is an alternative way to add to a cell. The user right-clicks to select the cell to draw. Then the user can click and drag to draw the cell. The brush size can be controlled using the spin-box to the right.
+
+`Eraser`: This can be used to remove a region from a cell. The use is the same as for `Brush`.
+
+`Exchange cell IDs`: This allows correction of cell ID values by switching two cells. 
+
+`Change cell ID`: This allows changing the ID number of a cell. **Important: **If you change the number to the number of another cell, those two cells will from now on be considered as one single cell. This is useful for fusing cells that were oversegmented but has to be used with care.
+
+`Retrack`: Having made edits to a frame, the cell numbers may no longer correspond in the next frame. This can be automatically fixed by navigating to the next frame and clicking the retrack button.
+
+### Extracting the results
+
+After the masks are satisfactory for a given field of view, you can click on the `Extract` button to export the results. There are two ways the results can be exported: Firstly, the masks that were found can be exported as multistack TIFF files. Secondly, the fluorescence together with several statistics giving information about every individual cell can be extracted and saved as a `.csv` file. 
+
+Moreover, you may only be interested in a subset of the cells visible in the image, which is why this second window allows you to select the cells which you are interested in. You can select or deselect multiple cells by drawing a polygon around them and confirming with a right-click, or select and deselect single cells by just left-clicking them. Note that the image that is displayed corresponds to the last frame for which you have a mask. Cells which disappeared throughout the timelapse video - and thus are not part of the mask - will be exported as well but indicated with a flag in the exported fluorescence csv. 
+
+When you want to extract fluorescence, you can add files from which to extract fluorescence by clicking the `Add` button. There you can either add a single image file, a multistack TIFF file, or a folder containing image files. Note that if multiple files or frames are used, the fluorescence file or folder must have the same amount of images as the image given to the program at startup.
+
+The output csv contains one line for every combination of cells, timeframe, and channel. This allows the file easily to be read into pandas, and avoids a varying amount of columns depending on how many fluorescence channels are used. The following statistics are exported: The *area* of the cell, the *mean* intensity, the intensity *variance*, the *total intensity*, and the x and y coordinates of the *center of mass*. Moreover, the major and minor axes of the cells are found using principal component analysis. In particular, the *angle* of the major axis to the x axis is given, together with the *length* of the major and minor axis, thus, fully specifying an ellipsoid approximating the cell. Finally, we report whether the cell disappears, i.e., whether or not it is present in the last frame. 
+
+### Running the demo
+
+We guide you step-by-step through the demo:
+
+1. In the startup dialog, click `Open image file` and select the file in the `example_data` folder from within the file dialog.
+2. Give a name to the h5 mask file, such as example_data.h5. Press `OK` to confirm.
+3. We want to predict the segmentation. Click `Launch CNN`. In the pop-up dialog. Enter 0 and 0 as the time bounds. Select the Field of View 1 by clicking on it. Press `OK`. 
+4. Wait for the neural network to predict. This takes about 1 min on a standard computer. 
+5. Now go through the image to verify the predictions and correct mistakes as needed. Instructions about how to use every tool is shown in the status bar at the bottom when you hover over the tool button. 
+6. Click `Extract` if you are satisfied. Extract the mask or the cell statistics, specify a file name, and you're done! In case you wanted additional fluorescence channels or only extract a subset of cells, you could also do this here using the corresponding buttons.
+
+
+
+
+
+`
+
```

### Comparing `YeaZ-1.0.0rc1/README.md` & `YeaZ-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,167 +1,204 @@
-# YeaZ
-
-This is the user manual for the graphical interface for segmenting yeast images using the YeaZ convolutional neural network. You can find the training set with the segmented training images here: https://www.quantsysbio.com/data-and-software/. 
-
-Want to try out the neural network without installing any software? Check out our online segmentation tool at https://lpbs-nn.epfl.ch/.
-
-## Latest updates
-
-18.04.2023:
-
-1. Update all dependencies to the latest versions
-2. Update PyQt to PyQt6, enabling the application to run on machines with m1 or m2 processors
-3. Add the ability to retrack multiple frames together
-4. Replace the old TensorFlow model with a PyTorch model
-5. Optimize the application's speed when showing cell numbers
-6. Improve the overall speed and performance of the application
-7. Add the ability to segment fission images
-8. Fix minor bugs and improve overall stability
-9. enable the option to run on GPU (windows and linux only)
-
-
-## Installation
-
-### System requirements
-
-The software requires a standard computer with enough RAM to apply the neural network. 8 GB RAM is enough to predict the 700 x 500 px image provided as the test data. The RAM requirements scales linearly with the number of image pixels.
-
-It was tested on OS X High Sierra (10.13.6), Windows 10 Education, and Ubuntu 18.04.4.
-
-Package dependencies: The convolutional neural network relies on Keras with TensorFlow. The Hungarian algorithm is implemented in the munkres package. In addition, standard image processing and scientific computing libraries are used. 
-
-Installation time is less than 5 minutes. 
-
-### Installation Steps
-
-1. Download the parameters for the neural network:
-    2.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b. Put the file in the folder `/unet`.  
-    2.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0. Put the file in the folder `/unet`.  
-    2.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/15Egg0zXSAFHD34a0urbthStIxlb4Q_G%5f. Put the file in the folder `/unet`.  
-
-### Install from PyPi
-
-1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
-2. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`. 
-3. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
-    3.1. for more information visit https://pytorch.org/get-started/locally/
-4. Install YeaZ with the command `pip install yeaz`.
-
-### Install from source
-
-1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
-2. Clone this repository (`git clone https://github.com/rahi-lab/YeaZ-GUI`).
-3. In the command line, navigate to the folder where you cloned YeaZ-GUI (command `cd YeaZ-GUI`).
-4. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`.   
-5. Activate the environment using `conda activate YeaZ`. 
-6. Install with the command `pip install -e .`.
-7. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
-    7.1. for more information visit https://pytorch.org/get-started/locally/
-
-## Runnig the GUI
-
-1. Open a terminal and activate the environment using `conda activate YeaZ`. 
-2. Run the program with the command `yeaz`.
-
-## Troubleshooting / FAQ 
-
-### Memory error when running on GPU (cuda). Also might happen on CPU.
-
-Unlike CPU, GPU memory is very limited. If you get a memory error when running on GPU, try the following steps:
-1. Crop the images to smaller sizes. Memory usage depends on number of pixels in your images. You may try cropping your images into several smaller images or removing empty space around cells.
-2. Another application might be using the GPU memory. Try to close all other applications and run the program again. You can also check applications that use GPU memory using the task manager (windows) or `nvidia-smi` command (linux).
-3. Try running on CPU or on a cluster with more GPU memory.
-
-### The application is running on CPU instead of GPU
-
-if you have specified running on GPU and the application is running on CPU instead, this might be due to the following reasons:
-1. you don't have a cuda compatible gpu. check the list of cuda-compatible gpus here: https://developer.nvidia.com/cuda-gpus
-2. you are using mac os with m1 or m2 processors. Unfortunately, the current version of PyTorch implementation does not fully support Mac M1 or M2 GPUs. In the meantime, you can still run your program on Mac M1 or M2 CPUs, which are quite powerful and can provide significant performance gains over traditional CPUs.
-3. you have not installed cuda. please follow the installation steps above to install cuda (run `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`).
-
-### Small buds are not recognized as cells
-
-If small buds aren't recognized as cells in your image, this is likely linked to a segmentation parameter that is too high. Relaunching the CNN with a smaller parameter will likely yield better results.
-
-### I just want the CNN, but not the GUI
-
-In case you only want to use the functionalities of the convolutional neural network and the segmentation, but not the full GUI, you only need the files `unet/model_pytorch.py`, `unet/neural_network.py` (for making predictions), `unet/segment.py` (for doing watershed segmentation) and `unet/hungarian.py` (for tracking), as well as the weights for the neural network which have to be in the same folder. You can create predictions using the `prediction` function in `neural_network.py` (note that before making predictions, you have to use the function `equalize_adapthist` from `skimage.exposure` on the image). The segmentations can be obtained with the `segment` function in `segment.py`, and tracking between two frames is done using the `correspondence` function in `hungarian.py`.
-You can also run `Launch_NN_comand_Line.py` and give input arguments to run the whole pipeline and save final mask. Here is an example for running the CNN on a phase contrast image:
-`python Launch_NN_command_line.py -i "example_data/2020_3_19_frame_100_cropped.tif" -m "newmaskfile.h5" --image_type  "pc" --device "cuda" --range_of_frames 0 0 --`
-
-### CNN performs less well on bright-field images
-
-Our CNN was trained on fewer cells with the bright-field technique (3841 unique cells imaged with 6 different exposure levels versus >8000 for phase contrast).
-
-### Graphical user interface not working on Mac OS Big Sur
-
-Jordan Xiao of Stanford University pointed out that one of the python modules (Pyqt) has some issues on Mac OS Big Sur. Check out https://stackoverflow.com/questions/64833558/apps-not-popping-up-on-macos-big-sur-11-0-1 and https://stackoverflow.com/questions/64818879/is-there-any-solution-regarding-to-pyqt-library-doesnt-work-in-mac-os-big-sur/64856281 for more information and possible fixes.
-
-## User Guide
-
-### Launching the Program
-
-Upon starting the program, it prompts you to select your images and your (new) mask file. There are two ways to select images: One can directly select a single image file using the button `Open image file`. Currently, we support Nikon `.nd2` files and multi-stack `.tif` files in addition to all standard formats such as `.png`, `.jpg`, or `.tif`. One can also select a folder of image files using the button `Open image folder`. This takes every single image in the folder to be a frame in a timelapse recording of yeast cells. The folder must contain images that all have the same size. 
-
-The program will save segmentation masks in `.h5` files. You can either create a new file by specifying its name in the text box or if you already have an h5 file for a specific set of images, you can select it using `Open mask file`. Note that when using an existing `.h5` file, you also have to use the same images as you did at its creation.
-
-### The Interface
-
-After clicking OK in the launcher, the main program will open. It consists of an image display of three images, the current image in the middle, the previous one to the left and the next image to the right. This display was chosen to easily be able to check whether the cell numbers and the segmentations are consistent throughout time.
-
-On the very bottom of the program, there is a status bar which displays the state of the program. In addition, when hovering over a button, it gives detailed information about what the button does and how to use it.
-
-On the top left of the three images, there are multiple buttons that allow the user to use pan and zoom to navigate through the image. The home button to the very left allows to reset zoom and pan, while the arrows allow to go to the next and previous pan/zoom positions. 
-
-On the bottom of the images, there are three rows of buttons. The first row of buttons allows the user to select the field of view, color channel, and time frame. Note that support for multiple fields of view and color channels is currently only available when opening .nd2 files. The second row contains tools to make edits to the mask, in order to correct the mistakes of the CNN. Moreover, it allows to show or hide the segmentation mask and the cell numbers. On the bottom right, the buttons allow to launch the CNN, to recalculate the tracking, and to extract the fluorescence or segmentation masks.
-
-### Launching the CNN
-
-After opening a new image file, the next step is typically to launch the convolutional neural network with the `Launch CNN` button. Note that if you are using a file with multiple color channels, this has to be done with the brightfield channel visible. This will open a dialog box, in which you can specify the time frames that you want to launch the CNN on as well as the field of view you want to use and type of your images. 
-
-Moreover, it lets you specify two parameters: The **threshold value** specifies the predicted value above which a pixel is considered to belong to a cell. This value is set at 0.5 per default and doesn't have to be changed in our experience. Increasing this value will decrease the sizes of the cells and can come in handy if the cells tend to exceed their borders. The **segmentation parameter** tells the program how far away two cell centers have to be at least, in order for two cells to be considered as separate entities. It has to be adjusted depending on how large the image resolution is: For small resolutions, a value of 2 seems to work well, whereas 5 is good for higher resolutions.
-
-### Making edits to the mask
-
-After the CNN has run, it is possible to correct the mistakes it has made. This can be done in the following ways:
-
-`Add region`: Add a region to an existing cell, by defining a polygon. First left-click on the cell to which you want to add a region, then continue clicking to draw a polygon to add. Finally click on the button again to confirm.
-
-`New cell`: This works similar to `Add region` but defines a new cell. Draw a polygon using left-clicks and re-click the button to confirm.
-
-`Brush`: This is an alternative way to add to a cell. The user right-clicks to select the cell to draw. Then the user can click and drag to draw the cell. The brush size can be controlled using the spin-box to the right.
-
-`Eraser`: This can be used to remove a region from a cell. The use is the same as for `Brush`.
-
-`Exchange cell IDs`: This allows correction of cell ID values by switching two cells. 
-
-`Change cell ID`: This allows changing the ID number of a cell. **Important: **If you change the number to the number of another cell, those two cells will from now on be considered as one single cell. This is useful for fusing cells that were oversegmented but has to be used with care.
-
-`Retrack`: Having made edits to a frame, the cell numbers may no longer correspond in the next frame. This can be automatically fixed by navigating to the next frame and clicking the retrack button.
-
-### Extracting the results
-
-After the masks are satisfactory for a given field of view, you can click on the `Extract` button to export the results. There are two ways the results can be exported: Firstly, the masks that were found can be exported as multistack TIFF files. Secondly, the fluorescence together with several statistics giving information about every individual cell can be extracted and saved as a `.csv` file. 
-
-Moreover, you may only be interested in a subset of the cells visible in the image, which is why this second window allows you to select the cells which you are interested in. You can select or deselect multiple cells by drawing a polygon around them and confirming with a right-click, or select and deselect single cells by just left-clicking them. Note that the image that is displayed corresponds to the last frame for which you have a mask. Cells which disappeared throughout the timelapse video - and thus are not part of the mask - will be exported as well but indicated with a flag in the exported fluorescence csv. 
-
-When you want to extract fluorescence, you can add files from which to extract fluorescence by clicking the `Add` button. There you can either add a single image file, a multistack TIFF file, or a folder containing image files. Note that if multiple files or frames are used, the fluorescence file or folder must have the same amount of images as the image given to the program at startup.
-
-The output csv contains one line for every combination of cells, timeframe, and channel. This allows the file easily to be read into pandas, and avoids a varying amount of columns depending on how many fluorescence channels are used. The following statistics are exported: The *area* of the cell, the *mean* intensity, the intensity *variance*, the *total intensity*, and the x and y coordinates of the *center of mass*. Moreover, the major and minor axes of the cells are found using principal component analysis. In particular, the *angle* of the major axis to the x axis is given, together with the *length* of the major and minor axis, thus, fully specifying an ellipsoid approximating the cell. Finally, we report whether the cell disappears, i.e., whether or not it is present in the last frame. 
-
-### Running the demo
-
-We guide you step-by-step through the demo:
-
-1. In the startup dialog, click `Open image file` and select the file in the `example_data` folder from within the file dialog.
-2. Give a name to the h5 mask file, such as example_data.h5. Press `OK` to confirm.
-3. We want to predict the segmentation. Click `Launch CNN`. In the pop-up dialog. Enter 0 and 0 as the time bounds. Select the Field of View 1 by clicking on it. Press `OK`. 
-4. Wait for the neural network to predict. This takes about 1 min on a standard computer. 
-5. Now go through the image to verify the predictions and correct mistakes as needed. Instructions about how to use every tool is shown in the status bar at the bottom when you hover over the tool button. 
-6. Click `Extract` if you are satisfied. Extract the mask or the cell statistics, specify a file name, and you're done! In case you wanted additional fluorescence channels or only extract a subset of cells, you could also do this here using the corresponding buttons.
-
-
-
-
-
-`
-
+Metadata-Version: 2.1
+Name: YeaZ
+Version: 1.0.1
+Summary: Deep-learning based yeast cell segmentation
+Home-page: https://github.com/rahi-lab/YeaZ-GUI
+Author: Sahand Jamal Rahi
+Author-email: sahand.rahi@epfl.ch
+Project-URL: Rahi lab, https://www.epfl.ch/labs/lpbs/
+Keywords: live-cell imaging,cell segmentation,cell tracking,image analysis
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Utilities
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: gui
+Provides-Extra: tensorflow
+Provides-Extra: torch
+License-File: LICENSE
+
+# YeaZ
+
+This is the user manual for the graphical interface for segmenting yeast images using the YeaZ convolutional neural network. You can find the training set with the segmented training images here: https://www.quantsysbio.com/data-and-software/. 
+
+Want to try out the neural network without installing any software? Check out our online segmentation tool at https://lpbs-nn.epfl.ch/.
+
+## Latest updates
+26.07.2023:
+1. Updata the installation structure
+2. Packaging and upload on Pypi.
+
+18.04.2023:
+
+1. Update all dependencies to the latest versions
+2. Update PyQt to PyQt6, enabling the application to run on machines with m1 or m2 processors
+3. Add the ability to retrack multiple frames together
+4. Replace the old TensorFlow model with a PyTorch model
+5. Optimize the application's speed when showing cell numbers
+6. Improve the overall speed and performance of the application
+7. Add the ability to segment fission images
+8. Fix minor bugs and improve overall stability
+9. enable the option to run on GPU (windows and linux only)
+
+
+## Installation
+
+### System requirements
+
+The software requires a standard computer with enough RAM to apply the neural network. 8 GB RAM is enough to predict the 700 x 500 px image provided as the test data. The RAM requirements scale linearly with the number of image pixels.
+
+It was tested on macOS Ventura (13.4.1), Windows 10 Education, and Ubuntu 20.04.4.
+
+Package dependencies: The convolutional neural network relies on Pytorch. The Hungarian algorithm is implemented in the munkres package. In addition, standard image processing and scientific computing libraries are used. 
+
+Installation time is less than 5 minutes. 
+
+### Download weight files for neural network
+
+1. Download the parameters for the neural network:<br>
+    1.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b. Put the file in the folder `yeaz/unet`.  <br>
+    1.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0. Put the file in the folder `yeaz/unet`.  <br>
+    1.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS. Put the file in the folder `yeaz/unet`.  
+
+### Install from PyPi
+
+1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
+2. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`. 
+3. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    3.1. for more information visit https://pytorch.org/get-started/locally/
+4. Install YeaZ with the command `pip install yeaz`.
+
+### Install from source
+
+1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
+2. Clone this repository (`git clone https://github.com/rahi-lab/YeaZ-GUI`).
+3. In the command line, navigate to the folder where you cloned YeaZ-GUI (command `cd YeaZ-GUI`).
+4. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`.   
+5. Activate the environment using `conda activate YeaZ`. 
+6. Install with the command `pip install -e .`.
+7. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    7.1. for more information visit https://pytorch.org/get-started/locally/
+
+## Runnig the GUI
+
+1. Open a terminal and activate the environment using `conda activate YeaZ`. 
+2. Run the program with the command `yeaz`.
+
+## Troubleshooting / FAQ 
+
+### Memory error when running on GPU (cuda). Also might happen on CPU.
+
+Unlike CPU, GPU memory is very limited. If you get a memory error when running on GPU, try the following steps:
+1. Crop the images to smaller sizes. Memory usage depends on number of pixels in your images. You may try cropping your images into several smaller images or removing empty space around cells.
+2. Another application might be using the GPU memory. Try to close all other applications and run the program again. You can also check applications that use GPU memory using the task manager (windows) or `nvidia-smi` command (linux).
+3. Try running on CPU or on a cluster with more GPU memory.
+
+### The application is running on CPU instead of GPU
+
+if you have specified running on GPU and the application is running on CPU instead, this might be due to the following reasons:
+1. you don't have a cuda compatible gpu. check the list of cuda-compatible gpus here: https://developer.nvidia.com/cuda-gpus
+2. you are using mac os with m1 or m2 processors. Unfortunately, the current version of PyTorch implementation does not fully support Mac M1 or M2 GPUs. In the meantime, you can still run your program on Mac M1 or M2 CPUs, which are quite powerful and can provide significant performance gains over traditional CPUs.
+3. you have not installed cuda. please follow the installation steps above to install cuda (run `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`).
+
+### Small buds are not recognized as cells
+
+If small buds aren't recognized as cells in your image, this is likely linked to a segmentation parameter that is too high. Relaunching the CNN with a smaller parameter will likely yield better results.
+
+### I just want the CNN, but not the GUI
+
+In case you only want to use the functionalities of the convolutional neural network and the segmentation, but not the full GUI, you only need the files `unet/model_pytorch.py`, `unet/neural_network.py` (for making predictions), `unet/segment.py` (for doing watershed segmentation) and `unet/hungarian.py` (for tracking), as well as the weights for the neural network which have to be in the same folder. You can create predictions using the `prediction` function in `neural_network.py` (note that before making predictions, you have to use the function `equalize_adapthist` from `skimage.exposure` on the image). The segmentations can be obtained with the `segment` function in `segment.py`, and tracking between two frames is done using the `correspondence` function in `hungarian.py`.
+You can also run `Launch_NN_comand_Line.py` and give input arguments to run the whole pipeline and save final mask. Here is an example for running the CNN on a phase contrast image:
+`python Launch_NN_command_line.py -i "example_data/2020_3_19_frame_100_cropped.tif" -m "newmaskfile.h5" --image_type  "pc" --device "cuda" --range_of_frames 0 0 --`
+
+### CNN performs less well on bright-field images
+
+Our CNN was trained on fewer cells with the bright-field technique (3841 unique cells imaged with 6 different exposure levels versus >8000 for phase contrast).
+
+### Graphical user interface not working on Mac OS Big Sur
+
+Jordan Xiao of Stanford University pointed out that one of the python modules (Pyqt) has some issues on Mac OS Big Sur. Check out https://stackoverflow.com/questions/64833558/apps-not-popping-up-on-macos-big-sur-11-0-1 and https://stackoverflow.com/questions/64818879/is-there-any-solution-regarding-to-pyqt-library-doesnt-work-in-mac-os-big-sur/64856281 for more information and possible fixes.
+
+## User Guide
+
+### Launching the Program
+
+Upon starting the program, it prompts you to select your images and your (new) mask file. There are two ways to select images: One can directly select a single image file using the button `Open image file`. Currently, we support Nikon `.nd2` files and multi-stack `.tif` files in addition to all standard formats such as `.png`, `.jpg`, or `.tif`. One can also select a folder of image files using the button `Open image folder`. This takes every single image in the folder to be a frame in a timelapse recording of yeast cells. The folder must contain images that all have the same size. 
+
+The program will save segmentation masks in `.h5` files. You can either create a new file by specifying its name in the text box or if you already have an h5 file for a specific set of images, you can select it using `Open mask file`. Note that when using an existing `.h5` file, you also have to use the same images as you did at its creation.
+
+### The Interface
+
+After clicking OK in the launcher, the main program will open. It consists of an image display of three images, the current image in the middle, the previous one to the left and the next image to the right. This display was chosen to easily be able to check whether the cell numbers and the segmentations are consistent throughout time.
+
+On the very bottom of the program, there is a status bar which displays the state of the program. In addition, when hovering over a button, it gives detailed information about what the button does and how to use it.
+
+On the top left of the three images, there are multiple buttons that allow the user to use pan and zoom to navigate through the image. The home button to the very left allows to reset zoom and pan, while the arrows allow to go to the next and previous pan/zoom positions. 
+
+On the bottom of the images, there are three rows of buttons. The first row of buttons allows the user to select the field of view, color channel, and time frame. Note that support for multiple fields of view and color channels is currently only available when opening .nd2 files. The second row contains tools to make edits to the mask, in order to correct the mistakes of the CNN. Moreover, it allows to show or hide the segmentation mask and the cell numbers. On the bottom right, the buttons allow to launch the CNN, to recalculate the tracking, and to extract the fluorescence or segmentation masks.
+
+### Launching the CNN
+
+After opening a new image file, the next step is typically to launch the convolutional neural network with the `Launch CNN` button. Note that if you are using a file with multiple color channels, this has to be done with the brightfield channel visible. This will open a dialog box, in which you can specify the time frames that you want to launch the CNN on as well as the field of view you want to use and type of your images. 
+
+Moreover, it lets you specify two parameters: The **threshold value** specifies the predicted value above which a pixel is considered to belong to a cell. This value is set at 0.5 per default and doesn't have to be changed in our experience. Increasing this value will decrease the sizes of the cells and can come in handy if the cells tend to exceed their borders. The **segmentation parameter** tells the program how far away two cell centers have to be at least, in order for two cells to be considered as separate entities. It has to be adjusted depending on how large the image resolution is: For small resolutions, a value of 2 seems to work well, whereas 5 is good for higher resolutions.
+
+### Making edits to the mask
+
+After the CNN has run, it is possible to correct the mistakes it has made. This can be done in the following ways:
+
+`Add region`: Add a region to an existing cell, by defining a polygon. First left-click on the cell to which you want to add a region, then continue clicking to draw a polygon to add. Finally click on the button again to confirm.
+
+`New cell`: This works similar to `Add region` but defines a new cell. Draw a polygon using left-clicks and re-click the button to confirm.
+
+`Brush`: This is an alternative way to add to a cell. The user right-clicks to select the cell to draw. Then the user can click and drag to draw the cell. The brush size can be controlled using the spin-box to the right.
+
+`Eraser`: This can be used to remove a region from a cell. The use is the same as for `Brush`.
+
+`Exchange cell IDs`: This allows correction of cell ID values by switching two cells. 
+
+`Change cell ID`: This allows changing the ID number of a cell. **Important: **If you change the number to the number of another cell, those two cells will from now on be considered as one single cell. This is useful for fusing cells that were oversegmented but has to be used with care.
+
+`Retrack`: Having made edits to a frame, the cell numbers may no longer correspond in the next frame. This can be automatically fixed by navigating to the next frame and clicking the retrack button.
+
+### Extracting the results
+
+After the masks are satisfactory for a given field of view, you can click on the `Extract` button to export the results. There are two ways the results can be exported: Firstly, the masks that were found can be exported as multistack TIFF files. Secondly, the fluorescence together with several statistics giving information about every individual cell can be extracted and saved as a `.csv` file. 
+
+Moreover, you may only be interested in a subset of the cells visible in the image, which is why this second window allows you to select the cells which you are interested in. You can select or deselect multiple cells by drawing a polygon around them and confirming with a right-click, or select and deselect single cells by just left-clicking them. Note that the image that is displayed corresponds to the last frame for which you have a mask. Cells which disappeared throughout the timelapse video - and thus are not part of the mask - will be exported as well but indicated with a flag in the exported fluorescence csv. 
+
+When you want to extract fluorescence, you can add files from which to extract fluorescence by clicking the `Add` button. There you can either add a single image file, a multistack TIFF file, or a folder containing image files. Note that if multiple files or frames are used, the fluorescence file or folder must have the same amount of images as the image given to the program at startup.
+
+The output csv contains one line for every combination of cells, timeframe, and channel. This allows the file easily to be read into pandas, and avoids a varying amount of columns depending on how many fluorescence channels are used. The following statistics are exported: The *area* of the cell, the *mean* intensity, the intensity *variance*, the *total intensity*, and the x and y coordinates of the *center of mass*. Moreover, the major and minor axes of the cells are found using principal component analysis. In particular, the *angle* of the major axis to the x axis is given, together with the *length* of the major and minor axis, thus, fully specifying an ellipsoid approximating the cell. Finally, we report whether the cell disappears, i.e., whether or not it is present in the last frame. 
+
+### Running the demo
+
+We guide you step-by-step through the demo:
+
+1. In the startup dialog, click `Open image file` and select the file in the `example_data` folder from within the file dialog.
+2. Give a name to the h5 mask file, such as example_data.h5. Press `OK` to confirm.
+3. We want to predict the segmentation. Click `Launch CNN`. In the pop-up dialog. Enter 0 and 0 as the time bounds. Select the Field of View 1 by clicking on it. Press `OK`. 
+4. Wait for the neural network to predict. This takes about 1 min on a standard computer. 
+5. Now go through the image to verify the predictions and correct mistakes as needed. Instructions about how to use every tool is shown in the status bar at the bottom when you hover over the tool button. 
+6. Click `Extract` if you are satisfied. Extract the mask or the cell statistics, specify a file name, and you're done! In case you wanted additional fluorescence channels or only extract a subset of cells, you could also do this here using the corresponding buttons.
+
+
+
+
+
+`
+
```

### Comparing `YeaZ-1.0.0rc1/YeaZ.egg-info/PKG-INFO` & `YeaZ-1.0.1/YeaZ.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,201 +1,204 @@
-Metadata-Version: 2.1
-Name: YeaZ
-Version: 1.0.0rc1
-Summary: Deep-learning based yeast cell segmentation
-Home-page: https://github.com/rahi-lab/YeaZ-GUI
-Author: Sahand Jamal Rahi
-Author-email: sahand.rahi@epfl.ch
-Project-URL: Rahi lab, https://www.epfl.ch/labs/lpbs/
-Keywords: live-cell imaging,cell segmentation,cell tracking,image analysis
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: gui
-Provides-Extra: tensorflow
-Provides-Extra: torch
-License-File: LICENSE
-
-# YeaZ
-
-This is the user manual for the graphical interface for segmenting yeast images using the YeaZ convolutional neural network. You can find the training set with the segmented training images here: https://www.quantsysbio.com/data-and-software/. 
-
-Want to try out the neural network without installing any software? Check out our online segmentation tool at https://lpbs-nn.epfl.ch/.
-
-## Latest updates
-
-18.04.2023:
-
-1. Update all dependencies to the latest versions
-2. Update PyQt to PyQt6, enabling the application to run on machines with m1 or m2 processors
-3. Add the ability to retrack multiple frames together
-4. Replace the old TensorFlow model with a PyTorch model
-5. Optimize the application's speed when showing cell numbers
-6. Improve the overall speed and performance of the application
-7. Add the ability to segment fission images
-8. Fix minor bugs and improve overall stability
-9. enable the option to run on GPU (windows and linux only)
-
-
-## Installation
-
-### System requirements
-
-The software requires a standard computer with enough RAM to apply the neural network. 8 GB RAM is enough to predict the 700 x 500 px image provided as the test data. The RAM requirements scales linearly with the number of image pixels.
-
-It was tested on OS X High Sierra (10.13.6), Windows 10 Education, and Ubuntu 18.04.4.
-
-Package dependencies: The convolutional neural network relies on Keras with TensorFlow. The Hungarian algorithm is implemented in the munkres package. In addition, standard image processing and scientific computing libraries are used. 
-
-Installation time is less than 5 minutes. 
-
-### Installation Steps
-
-1. Download the parameters for the neural network:
-    2.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b. Put the file in the folder `/unet`.  
-    2.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0. Put the file in the folder `/unet`.  
-    2.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/15Egg0zXSAFHD34a0urbthStIxlb4Q_G%5f. Put the file in the folder `/unet`.  
-
-### Install from PyPi
-
-1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
-2. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`. 
-3. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
-    3.1. for more information visit https://pytorch.org/get-started/locally/
-4. Install YeaZ with the command `pip install yeaz`.
-
-### Install from source
-
-1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
-2. Clone this repository (`git clone https://github.com/rahi-lab/YeaZ-GUI`).
-3. In the command line, navigate to the folder where you cloned YeaZ-GUI (command `cd YeaZ-GUI`).
-4. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`.   
-5. Activate the environment using `conda activate YeaZ`. 
-6. Install with the command `pip install -e .`.
-7. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
-    7.1. for more information visit https://pytorch.org/get-started/locally/
-
-## Runnig the GUI
-
-1. Open a terminal and activate the environment using `conda activate YeaZ`. 
-2. Run the program with the command `yeaz`.
-
-## Troubleshooting / FAQ 
-
-### Memory error when running on GPU (cuda). Also might happen on CPU.
-
-Unlike CPU, GPU memory is very limited. If you get a memory error when running on GPU, try the following steps:
-1. Crop the images to smaller sizes. Memory usage depends on number of pixels in your images. You may try cropping your images into several smaller images or removing empty space around cells.
-2. Another application might be using the GPU memory. Try to close all other applications and run the program again. You can also check applications that use GPU memory using the task manager (windows) or `nvidia-smi` command (linux).
-3. Try running on CPU or on a cluster with more GPU memory.
-
-### The application is running on CPU instead of GPU
-
-if you have specified running on GPU and the application is running on CPU instead, this might be due to the following reasons:
-1. you don't have a cuda compatible gpu. check the list of cuda-compatible gpus here: https://developer.nvidia.com/cuda-gpus
-2. you are using mac os with m1 or m2 processors. Unfortunately, the current version of PyTorch implementation does not fully support Mac M1 or M2 GPUs. In the meantime, you can still run your program on Mac M1 or M2 CPUs, which are quite powerful and can provide significant performance gains over traditional CPUs.
-3. you have not installed cuda. please follow the installation steps above to install cuda (run `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`).
-
-### Small buds are not recognized as cells
-
-If small buds aren't recognized as cells in your image, this is likely linked to a segmentation parameter that is too high. Relaunching the CNN with a smaller parameter will likely yield better results.
-
-### I just want the CNN, but not the GUI
-
-In case you only want to use the functionalities of the convolutional neural network and the segmentation, but not the full GUI, you only need the files `unet/model_pytorch.py`, `unet/neural_network.py` (for making predictions), `unet/segment.py` (for doing watershed segmentation) and `unet/hungarian.py` (for tracking), as well as the weights for the neural network which have to be in the same folder. You can create predictions using the `prediction` function in `neural_network.py` (note that before making predictions, you have to use the function `equalize_adapthist` from `skimage.exposure` on the image). The segmentations can be obtained with the `segment` function in `segment.py`, and tracking between two frames is done using the `correspondence` function in `hungarian.py`.
-You can also run `Launch_NN_comand_Line.py` and give input arguments to run the whole pipeline and save final mask. Here is an example for running the CNN on a phase contrast image:
-`python Launch_NN_command_line.py -i "example_data/2020_3_19_frame_100_cropped.tif" -m "newmaskfile.h5" --image_type  "pc" --device "cuda" --range_of_frames 0 0 --`
-
-### CNN performs less well on bright-field images
-
-Our CNN was trained on fewer cells with the bright-field technique (3841 unique cells imaged with 6 different exposure levels versus >8000 for phase contrast).
-
-### Graphical user interface not working on Mac OS Big Sur
-
-Jordan Xiao of Stanford University pointed out that one of the python modules (Pyqt) has some issues on Mac OS Big Sur. Check out https://stackoverflow.com/questions/64833558/apps-not-popping-up-on-macos-big-sur-11-0-1 and https://stackoverflow.com/questions/64818879/is-there-any-solution-regarding-to-pyqt-library-doesnt-work-in-mac-os-big-sur/64856281 for more information and possible fixes.
-
-## User Guide
-
-### Launching the Program
-
-Upon starting the program, it prompts you to select your images and your (new) mask file. There are two ways to select images: One can directly select a single image file using the button `Open image file`. Currently, we support Nikon `.nd2` files and multi-stack `.tif` files in addition to all standard formats such as `.png`, `.jpg`, or `.tif`. One can also select a folder of image files using the button `Open image folder`. This takes every single image in the folder to be a frame in a timelapse recording of yeast cells. The folder must contain images that all have the same size. 
-
-The program will save segmentation masks in `.h5` files. You can either create a new file by specifying its name in the text box or if you already have an h5 file for a specific set of images, you can select it using `Open mask file`. Note that when using an existing `.h5` file, you also have to use the same images as you did at its creation.
-
-### The Interface
-
-After clicking OK in the launcher, the main program will open. It consists of an image display of three images, the current image in the middle, the previous one to the left and the next image to the right. This display was chosen to easily be able to check whether the cell numbers and the segmentations are consistent throughout time.
-
-On the very bottom of the program, there is a status bar which displays the state of the program. In addition, when hovering over a button, it gives detailed information about what the button does and how to use it.
-
-On the top left of the three images, there are multiple buttons that allow the user to use pan and zoom to navigate through the image. The home button to the very left allows to reset zoom and pan, while the arrows allow to go to the next and previous pan/zoom positions. 
-
-On the bottom of the images, there are three rows of buttons. The first row of buttons allows the user to select the field of view, color channel, and time frame. Note that support for multiple fields of view and color channels is currently only available when opening .nd2 files. The second row contains tools to make edits to the mask, in order to correct the mistakes of the CNN. Moreover, it allows to show or hide the segmentation mask and the cell numbers. On the bottom right, the buttons allow to launch the CNN, to recalculate the tracking, and to extract the fluorescence or segmentation masks.
-
-### Launching the CNN
-
-After opening a new image file, the next step is typically to launch the convolutional neural network with the `Launch CNN` button. Note that if you are using a file with multiple color channels, this has to be done with the brightfield channel visible. This will open a dialog box, in which you can specify the time frames that you want to launch the CNN on as well as the field of view you want to use and type of your images. 
-
-Moreover, it lets you specify two parameters: The **threshold value** specifies the predicted value above which a pixel is considered to belong to a cell. This value is set at 0.5 per default and doesn't have to be changed in our experience. Increasing this value will decrease the sizes of the cells and can come in handy if the cells tend to exceed their borders. The **segmentation parameter** tells the program how far away two cell centers have to be at least, in order for two cells to be considered as separate entities. It has to be adjusted depending on how large the image resolution is: For small resolutions, a value of 2 seems to work well, whereas 5 is good for higher resolutions.
-
-### Making edits to the mask
-
-After the CNN has run, it is possible to correct the mistakes it has made. This can be done in the following ways:
-
-`Add region`: Add a region to an existing cell, by defining a polygon. First left-click on the cell to which you want to add a region, then continue clicking to draw a polygon to add. Finally click on the button again to confirm.
-
-`New cell`: This works similar to `Add region` but defines a new cell. Draw a polygon using left-clicks and re-click the button to confirm.
-
-`Brush`: This is an alternative way to add to a cell. The user right-clicks to select the cell to draw. Then the user can click and drag to draw the cell. The brush size can be controlled using the spin-box to the right.
-
-`Eraser`: This can be used to remove a region from a cell. The use is the same as for `Brush`.
-
-`Exchange cell IDs`: This allows correction of cell ID values by switching two cells. 
-
-`Change cell ID`: This allows changing the ID number of a cell. **Important: **If you change the number to the number of another cell, those two cells will from now on be considered as one single cell. This is useful for fusing cells that were oversegmented but has to be used with care.
-
-`Retrack`: Having made edits to a frame, the cell numbers may no longer correspond in the next frame. This can be automatically fixed by navigating to the next frame and clicking the retrack button.
-
-### Extracting the results
-
-After the masks are satisfactory for a given field of view, you can click on the `Extract` button to export the results. There are two ways the results can be exported: Firstly, the masks that were found can be exported as multistack TIFF files. Secondly, the fluorescence together with several statistics giving information about every individual cell can be extracted and saved as a `.csv` file. 
-
-Moreover, you may only be interested in a subset of the cells visible in the image, which is why this second window allows you to select the cells which you are interested in. You can select or deselect multiple cells by drawing a polygon around them and confirming with a right-click, or select and deselect single cells by just left-clicking them. Note that the image that is displayed corresponds to the last frame for which you have a mask. Cells which disappeared throughout the timelapse video - and thus are not part of the mask - will be exported as well but indicated with a flag in the exported fluorescence csv. 
-
-When you want to extract fluorescence, you can add files from which to extract fluorescence by clicking the `Add` button. There you can either add a single image file, a multistack TIFF file, or a folder containing image files. Note that if multiple files or frames are used, the fluorescence file or folder must have the same amount of images as the image given to the program at startup.
-
-The output csv contains one line for every combination of cells, timeframe, and channel. This allows the file easily to be read into pandas, and avoids a varying amount of columns depending on how many fluorescence channels are used. The following statistics are exported: The *area* of the cell, the *mean* intensity, the intensity *variance*, the *total intensity*, and the x and y coordinates of the *center of mass*. Moreover, the major and minor axes of the cells are found using principal component analysis. In particular, the *angle* of the major axis to the x axis is given, together with the *length* of the major and minor axis, thus, fully specifying an ellipsoid approximating the cell. Finally, we report whether the cell disappears, i.e., whether or not it is present in the last frame. 
-
-### Running the demo
-
-We guide you step-by-step through the demo:
-
-1. In the startup dialog, click `Open image file` and select the file in the `example_data` folder from within the file dialog.
-2. Give a name to the h5 mask file, such as example_data.h5. Press `OK` to confirm.
-3. We want to predict the segmentation. Click `Launch CNN`. In the pop-up dialog. Enter 0 and 0 as the time bounds. Select the Field of View 1 by clicking on it. Press `OK`. 
-4. Wait for the neural network to predict. This takes about 1 min on a standard computer. 
-5. Now go through the image to verify the predictions and correct mistakes as needed. Instructions about how to use every tool is shown in the status bar at the bottom when you hover over the tool button. 
-6. Click `Extract` if you are satisfied. Extract the mask or the cell statistics, specify a file name, and you're done! In case you wanted additional fluorescence channels or only extract a subset of cells, you could also do this here using the corresponding buttons.
-
-
-
-
-
-`
-
+Metadata-Version: 2.1
+Name: YeaZ
+Version: 1.0.1
+Summary: Deep-learning based yeast cell segmentation
+Home-page: https://github.com/rahi-lab/YeaZ-GUI
+Author: Sahand Jamal Rahi
+Author-email: sahand.rahi@epfl.ch
+Project-URL: Rahi lab, https://www.epfl.ch/labs/lpbs/
+Keywords: live-cell imaging,cell segmentation,cell tracking,image analysis
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Image Processing
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Utilities
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: gui
+Provides-Extra: tensorflow
+Provides-Extra: torch
+License-File: LICENSE
+
+# YeaZ
+
+This is the user manual for the graphical interface for segmenting yeast images using the YeaZ convolutional neural network. You can find the training set with the segmented training images here: https://www.quantsysbio.com/data-and-software/. 
+
+Want to try out the neural network without installing any software? Check out our online segmentation tool at https://lpbs-nn.epfl.ch/.
+
+## Latest updates
+26.07.2023:
+1. Updata the installation structure
+2. Packaging and upload on Pypi.
+
+18.04.2023:
+
+1. Update all dependencies to the latest versions
+2. Update PyQt to PyQt6, enabling the application to run on machines with m1 or m2 processors
+3. Add the ability to retrack multiple frames together
+4. Replace the old TensorFlow model with a PyTorch model
+5. Optimize the application's speed when showing cell numbers
+6. Improve the overall speed and performance of the application
+7. Add the ability to segment fission images
+8. Fix minor bugs and improve overall stability
+9. enable the option to run on GPU (windows and linux only)
+
+
+## Installation
+
+### System requirements
+
+The software requires a standard computer with enough RAM to apply the neural network. 8 GB RAM is enough to predict the 700 x 500 px image provided as the test data. The RAM requirements scale linearly with the number of image pixels.
+
+It was tested on macOS Ventura (13.4.1), Windows 10 Education, and Ubuntu 20.04.4.
+
+Package dependencies: The convolutional neural network relies on Pytorch. The Hungarian algorithm is implemented in the munkres package. In addition, standard image processing and scientific computing libraries are used. 
+
+Installation time is less than 5 minutes. 
+
+### Download weight files for neural network
+
+1. Download the parameters for the neural network:<br>
+    1.1. Download the parameters for segmenting phase contrast images from: https://drive.google.com/file/d/1tcdl34Aq11mrPVlyu0Qd4rUigw_6948b. Put the file in the folder `yeaz/unet`.  <br>
+    1.2. Download the parameters for segmenting bright-field images from: https://drive.google.com/file/d/1vnhkp54McM836yczh4F-YYJwPahbTsY0. Put the file in the folder `yeaz/unet`.  <br>
+    1.3. Download the parameters for segmenting fission images form: https://drive.google.com/file/d/1h_Wz2d3UY0jkGtMrhl32iEqbOQVXsmKS. Put the file in the folder `yeaz/unet`.  
+
+### Install from PyPi
+
+1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
+2. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`. 
+3. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    3.1. for more information visit https://pytorch.org/get-started/locally/
+4. Install YeaZ with the command `pip install yeaz`.
+
+### Install from source
+
+1. If you don't have conda or miniconda installed, download it from https://docs.conda.io/en/latest/miniconda.html.
+2. Clone this repository (`git clone https://github.com/rahi-lab/YeaZ-GUI`).
+3. In the command line, navigate to the folder where you cloned YeaZ-GUI (command `cd YeaZ-GUI`).
+4. In the command line, create a virtual environment with python 3.9 with the command `conda create -n YeaZ python=3.9`.   
+5. Activate the environment using `conda activate YeaZ`. 
+6. Install with the command `pip install -e .`.
+7. Install pytorch and cuda using `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`
+    7.1. for more information visit https://pytorch.org/get-started/locally/
+
+## Runnig the GUI
+
+1. Open a terminal and activate the environment using `conda activate YeaZ`. 
+2. Run the program with the command `yeaz`.
+
+## Troubleshooting / FAQ 
+
+### Memory error when running on GPU (cuda). Also might happen on CPU.
+
+Unlike CPU, GPU memory is very limited. If you get a memory error when running on GPU, try the following steps:
+1. Crop the images to smaller sizes. Memory usage depends on number of pixels in your images. You may try cropping your images into several smaller images or removing empty space around cells.
+2. Another application might be using the GPU memory. Try to close all other applications and run the program again. You can also check applications that use GPU memory using the task manager (windows) or `nvidia-smi` command (linux).
+3. Try running on CPU or on a cluster with more GPU memory.
+
+### The application is running on CPU instead of GPU
+
+if you have specified running on GPU and the application is running on CPU instead, this might be due to the following reasons:
+1. you don't have a cuda compatible gpu. check the list of cuda-compatible gpus here: https://developer.nvidia.com/cuda-gpus
+2. you are using mac os with m1 or m2 processors. Unfortunately, the current version of PyTorch implementation does not fully support Mac M1 or M2 GPUs. In the meantime, you can still run your program on Mac M1 or M2 CPUs, which are quite powerful and can provide significant performance gains over traditional CPUs.
+3. you have not installed cuda. please follow the installation steps above to install cuda (run `conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia`).
+
+### Small buds are not recognized as cells
+
+If small buds aren't recognized as cells in your image, this is likely linked to a segmentation parameter that is too high. Relaunching the CNN with a smaller parameter will likely yield better results.
+
+### I just want the CNN, but not the GUI
+
+In case you only want to use the functionalities of the convolutional neural network and the segmentation, but not the full GUI, you only need the files `unet/model_pytorch.py`, `unet/neural_network.py` (for making predictions), `unet/segment.py` (for doing watershed segmentation) and `unet/hungarian.py` (for tracking), as well as the weights for the neural network which have to be in the same folder. You can create predictions using the `prediction` function in `neural_network.py` (note that before making predictions, you have to use the function `equalize_adapthist` from `skimage.exposure` on the image). The segmentations can be obtained with the `segment` function in `segment.py`, and tracking between two frames is done using the `correspondence` function in `hungarian.py`.
+You can also run `Launch_NN_comand_Line.py` and give input arguments to run the whole pipeline and save final mask. Here is an example for running the CNN on a phase contrast image:
+`python Launch_NN_command_line.py -i "example_data/2020_3_19_frame_100_cropped.tif" -m "newmaskfile.h5" --image_type  "pc" --device "cuda" --range_of_frames 0 0 --`
+
+### CNN performs less well on bright-field images
+
+Our CNN was trained on fewer cells with the bright-field technique (3841 unique cells imaged with 6 different exposure levels versus >8000 for phase contrast).
+
+### Graphical user interface not working on Mac OS Big Sur
+
+Jordan Xiao of Stanford University pointed out that one of the python modules (Pyqt) has some issues on Mac OS Big Sur. Check out https://stackoverflow.com/questions/64833558/apps-not-popping-up-on-macos-big-sur-11-0-1 and https://stackoverflow.com/questions/64818879/is-there-any-solution-regarding-to-pyqt-library-doesnt-work-in-mac-os-big-sur/64856281 for more information and possible fixes.
+
+## User Guide
+
+### Launching the Program
+
+Upon starting the program, it prompts you to select your images and your (new) mask file. There are two ways to select images: One can directly select a single image file using the button `Open image file`. Currently, we support Nikon `.nd2` files and multi-stack `.tif` files in addition to all standard formats such as `.png`, `.jpg`, or `.tif`. One can also select a folder of image files using the button `Open image folder`. This takes every single image in the folder to be a frame in a timelapse recording of yeast cells. The folder must contain images that all have the same size. 
+
+The program will save segmentation masks in `.h5` files. You can either create a new file by specifying its name in the text box or if you already have an h5 file for a specific set of images, you can select it using `Open mask file`. Note that when using an existing `.h5` file, you also have to use the same images as you did at its creation.
+
+### The Interface
+
+After clicking OK in the launcher, the main program will open. It consists of an image display of three images, the current image in the middle, the previous one to the left and the next image to the right. This display was chosen to easily be able to check whether the cell numbers and the segmentations are consistent throughout time.
+
+On the very bottom of the program, there is a status bar which displays the state of the program. In addition, when hovering over a button, it gives detailed information about what the button does and how to use it.
+
+On the top left of the three images, there are multiple buttons that allow the user to use pan and zoom to navigate through the image. The home button to the very left allows to reset zoom and pan, while the arrows allow to go to the next and previous pan/zoom positions. 
+
+On the bottom of the images, there are three rows of buttons. The first row of buttons allows the user to select the field of view, color channel, and time frame. Note that support for multiple fields of view and color channels is currently only available when opening .nd2 files. The second row contains tools to make edits to the mask, in order to correct the mistakes of the CNN. Moreover, it allows to show or hide the segmentation mask and the cell numbers. On the bottom right, the buttons allow to launch the CNN, to recalculate the tracking, and to extract the fluorescence or segmentation masks.
+
+### Launching the CNN
+
+After opening a new image file, the next step is typically to launch the convolutional neural network with the `Launch CNN` button. Note that if you are using a file with multiple color channels, this has to be done with the brightfield channel visible. This will open a dialog box, in which you can specify the time frames that you want to launch the CNN on as well as the field of view you want to use and type of your images. 
+
+Moreover, it lets you specify two parameters: The **threshold value** specifies the predicted value above which a pixel is considered to belong to a cell. This value is set at 0.5 per default and doesn't have to be changed in our experience. Increasing this value will decrease the sizes of the cells and can come in handy if the cells tend to exceed their borders. The **segmentation parameter** tells the program how far away two cell centers have to be at least, in order for two cells to be considered as separate entities. It has to be adjusted depending on how large the image resolution is: For small resolutions, a value of 2 seems to work well, whereas 5 is good for higher resolutions.
+
+### Making edits to the mask
+
+After the CNN has run, it is possible to correct the mistakes it has made. This can be done in the following ways:
+
+`Add region`: Add a region to an existing cell, by defining a polygon. First left-click on the cell to which you want to add a region, then continue clicking to draw a polygon to add. Finally click on the button again to confirm.
+
+`New cell`: This works similar to `Add region` but defines a new cell. Draw a polygon using left-clicks and re-click the button to confirm.
+
+`Brush`: This is an alternative way to add to a cell. The user right-clicks to select the cell to draw. Then the user can click and drag to draw the cell. The brush size can be controlled using the spin-box to the right.
+
+`Eraser`: This can be used to remove a region from a cell. The use is the same as for `Brush`.
+
+`Exchange cell IDs`: This allows correction of cell ID values by switching two cells. 
+
+`Change cell ID`: This allows changing the ID number of a cell. **Important: **If you change the number to the number of another cell, those two cells will from now on be considered as one single cell. This is useful for fusing cells that were oversegmented but has to be used with care.
+
+`Retrack`: Having made edits to a frame, the cell numbers may no longer correspond in the next frame. This can be automatically fixed by navigating to the next frame and clicking the retrack button.
+
+### Extracting the results
+
+After the masks are satisfactory for a given field of view, you can click on the `Extract` button to export the results. There are two ways the results can be exported: Firstly, the masks that were found can be exported as multistack TIFF files. Secondly, the fluorescence together with several statistics giving information about every individual cell can be extracted and saved as a `.csv` file. 
+
+Moreover, you may only be interested in a subset of the cells visible in the image, which is why this second window allows you to select the cells which you are interested in. You can select or deselect multiple cells by drawing a polygon around them and confirming with a right-click, or select and deselect single cells by just left-clicking them. Note that the image that is displayed corresponds to the last frame for which you have a mask. Cells which disappeared throughout the timelapse video - and thus are not part of the mask - will be exported as well but indicated with a flag in the exported fluorescence csv. 
+
+When you want to extract fluorescence, you can add files from which to extract fluorescence by clicking the `Add` button. There you can either add a single image file, a multistack TIFF file, or a folder containing image files. Note that if multiple files or frames are used, the fluorescence file or folder must have the same amount of images as the image given to the program at startup.
+
+The output csv contains one line for every combination of cells, timeframe, and channel. This allows the file easily to be read into pandas, and avoids a varying amount of columns depending on how many fluorescence channels are used. The following statistics are exported: The *area* of the cell, the *mean* intensity, the intensity *variance*, the *total intensity*, and the x and y coordinates of the *center of mass*. Moreover, the major and minor axes of the cells are found using principal component analysis. In particular, the *angle* of the major axis to the x axis is given, together with the *length* of the major and minor axis, thus, fully specifying an ellipsoid approximating the cell. Finally, we report whether the cell disappears, i.e., whether or not it is present in the last frame. 
+
+### Running the demo
+
+We guide you step-by-step through the demo:
+
+1. In the startup dialog, click `Open image file` and select the file in the `example_data` folder from within the file dialog.
+2. Give a name to the h5 mask file, such as example_data.h5. Press `OK` to confirm.
+3. We want to predict the segmentation. Click `Launch CNN`. In the pop-up dialog. Enter 0 and 0 as the time bounds. Select the Field of View 1 by clicking on it. Press `OK`. 
+4. Wait for the neural network to predict. This takes about 1 min on a standard computer. 
+5. Now go through the image to verify the predictions and correct mistakes as needed. Instructions about how to use every tool is shown in the status bar at the bottom when you hover over the tool button. 
+6. Click `Extract` if you are satisfied. Extract the mask or the cell statistics, specify a file name, and you're done! In case you wanted additional fluorescence channels or only extract a subset of cells, you could also do this here using the corresponding buttons.
+
+
+
+
+
+`
+
```

### Comparing `YeaZ-1.0.0rc1/YeaZ.egg-info/SOURCES.txt` & `YeaZ-1.0.1/YeaZ.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.0rc1/example_data/2020_3_19_frame_100_cropped.tif` & `YeaZ-1.0.1/example_data/2020_3_19_frame_100_cropped.tif`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.0rc1/setup.cfg` & `YeaZ-1.0.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,103 @@
-00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2059 6561 5a0d 0a61 7574 686f 7220   = YeaZ..author 
-00000020: 3d20 5361 6861 6e64 204a 616d 616c 2052  = Sahand Jamal R
-00000030: 6168 690d 0a61 7574 686f 725f 656d 6169  ahi..author_emai
-00000040: 6c20 3d20 7361 6861 6e64 2e72 6168 6940  l = sahand.rahi@
-00000050: 6570 666c 2e63 680d 0a64 6573 6372 6970  epfl.ch..descrip
-00000060: 7469 6f6e 203d 2044 6565 702d 6c65 6172  tion = Deep-lear
-00000070: 6e69 6e67 2062 6173 6564 2079 6561 7374  ning based yeast
-00000080: 2063 656c 6c20 7365 676d 656e 7461 7469   cell segmentati
-00000090: 6f6e 0d0a 6b65 7977 6f72 6473 203d 200d  on..keywords = .
-000000a0: 0a09 6c69 7665 2d63 656c 6c20 696d 6167  ..live-cell imag
-000000b0: 696e 670d 0a09 6365 6c6c 2073 6567 6d65  ing...cell segme
-000000c0: 6e74 6174 696f 6e0d 0a09 6365 6c6c 2074  ntation...cell t
-000000d0: 7261 636b 696e 670d 0a09 696d 6167 6520  racking...image 
-000000e0: 616e 616c 7973 6973 0d0a 6c6f 6e67 5f64  analysis..long_d
-000000f0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-00000100: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-00000110: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-00000120: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-00000130: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
-00000140: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000150: 622e 636f 6d2f 7261 6869 2d6c 6162 2f59  b.com/rahi-lab/Y
-00000160: 6561 5a2d 4755 490d 0a70 726f 6a65 6374  eaZ-GUI..project
-00000170: 5f75 726c 7320 3d20 0d0a 0952 6168 6920  _urls = ...Rahi 
-00000180: 6c61 6220 3d20 6874 7470 733a 2f2f 7777  lab = https://ww
-00000190: 772e 6570 666c 2e63 682f 6c61 6273 2f6c  w.epfl.ch/labs/l
-000001a0: 7062 732f 0d0a 636c 6173 7369 6669 6572  pbs/..classifier
-000001b0: 7320 3d20 0d0a 0944 6576 656c 6f70 6d65  s = ...Developme
-000001c0: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
-000001d0: 2042 6574 610d 0a09 5072 6f67 7261 6d6d   Beta...Programm
-000001e0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001f0: 5079 7468 6f6e 203a 3a20 3320 3a3a 204f  Python :: 3 :: O
-00000200: 6e6c 790d 0a09 5072 6f67 7261 6d6d 696e  nly...Programmin
-00000210: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000220: 7468 6f6e 203a 3a20 332e 380d 0a09 5072  thon :: 3.8...Pr
-00000230: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000240: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000250: 332e 390d 0a09 5072 6f67 7261 6d6d 696e  3.9...Programmin
-00000260: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000270: 7468 6f6e 203a 3a20 332e 3130 0d0a 094c  thon :: 3.10...L
-00000280: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-00000290: 7072 6f76 6564 203a 3a20 4253 4420 4c69  proved :: BSD Li
-000002a0: 6365 6e73 650d 0a09 496e 7465 6e64 6564  cense...Intended
-000002b0: 2041 7564 6965 6e63 6520 3a3a 2045 6475   Audience :: Edu
-000002c0: 6361 7469 6f6e 0d0a 0949 6e74 656e 6465  cation...Intende
-000002d0: 6420 4175 6469 656e 6365 203a 3a20 5363  d Audience :: Sc
-000002e0: 6965 6e63 652f 5265 7365 6172 6368 0d0a  ience/Research..
-000002f0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
-00000300: 6d20 3a3a 204d 6963 726f 736f 6674 203a  m :: Microsoft :
-00000310: 3a20 5769 6e64 6f77 730d 0a09 4f70 6572  : Windows...Oper
-00000320: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-00000330: 504f 5349 580d 0a09 4f70 6572 6174 696e  POSIX...Operatin
-00000340: 6720 5379 7374 656d 203a 3a20 556e 6978  g System :: Unix
-00000350: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-00000360: 7465 6d20 3a3a 204d 6163 4f53 0d0a 0954  tem :: MacOS...T
-00000370: 6f70 6963 203a 3a20 5363 6965 6e74 6966  opic :: Scientif
-00000380: 6963 2f45 6e67 696e 6565 7269 6e67 0d0a  ic/Engineering..
-00000390: 0954 6f70 6963 203a 3a20 5363 6965 6e74  .Topic :: Scient
-000003a0: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
-000003b0: 203a 3a20 4269 6f2d 496e 666f 726d 6174   :: Bio-Informat
-000003c0: 6963 730d 0a09 546f 7069 6320 3a3a 2053  ics...Topic :: S
-000003d0: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-000003e0: 6572 696e 6720 3a3a 2049 6e66 6f72 6d61  ering :: Informa
-000003f0: 7469 6f6e 2041 6e61 6c79 7369 730d 0a09  tion Analysis...
-00000400: 546f 7069 6320 3a3a 2053 6369 656e 7469  Topic :: Scienti
-00000410: 6669 632f 456e 6769 6e65 6572 696e 6720  fic/Engineering 
-00000420: 3a3a 2049 6d61 6765 2050 726f 6365 7373  :: Image Process
-00000430: 696e 670d 0a09 546f 7069 6320 3a3a 2053  ing...Topic :: S
-00000440: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
-00000450: 6572 696e 6720 3a3a 2056 6973 7561 6c69  ering :: Visuali
-00000460: 7a61 7469 6f6e 0d0a 0954 6f70 6963 203a  zation...Topic :
-00000470: 3a20 5574 696c 6974 6965 730d 0a0d 0a5b  : Utilities....[
-00000480: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
-00000490: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
-000004a0: 6f6e 5f72 6571 7569 7265 7320 3d20 0d0a  on_requires = ..
-000004b0: 093e 3d33 2e39 0d0a 696e 636c 7564 655f  .>=3.9..include_
-000004c0: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
-000004d0: 7275 650d 0a69 6e73 7461 6c6c 5f72 6571  rue..install_req
-000004e0: 7569 7265 7320 3d20 0d0a 096e 756d 7079  uires = ...numpy
-000004f0: 3e3d 312e 3137 2e34 0d0a 096d 6174 706c  >=1.17.4...matpl
-00000500: 6f74 6c69 623e 3d33 2e31 2e31 0d0a 096e  otlib>=3.1.1...n
-00000510: 6432 7265 6164 6572 3e3d 332e 332e 300d  d2reader>=3.3.0.
-00000520: 0a09 6835 7079 3e3d 332e 382e 300d 0a09  ..h5py>=3.8.0...
-00000530: 7363 696b 6974 2d69 6d61 6765 3e3d 302e  scikit-image>=0.
-00000540: 3135 2e30 0d0a 096f 7065 6e70 7978 6c3e  15.0...openpyxl>
-00000550: 3d33 2e31 2e32 0d0a 096f 7065 6e63 762d  =3.1.2...opencv-
-00000560: 7079 7468 6f6e 2d68 6561 646c 6573 733e  python-headless>
-00000570: 3d34 2e37 2e30 2e37 320d 0a09 7061 6e64  =4.7.0.72...pand
-00000580: 6173 3e3d 302e 3235 2e33 0d0a 096d 756e  as>=0.25.3...mun
-00000590: 6b72 6573 0d0a 0973 6369 6b69 742d 6c65  kres...scikit-le
-000005a0: 6172 6e3e 3d30 2e30 0d0a 0969 6d61 6765  arn>=0.0...image
-000005b0: 696f 3e3d 322e 362e 310d 0a09 5069 6c6c  io>=2.6.1...Pill
-000005c0: 6f77 3e3d 362e 322e 310d 0a09 7471 646d  ow>=6.2.1...tqdm
-000005d0: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 7874  ....[options.ext
-000005e0: 7261 735f 7265 7175 6972 655d 0d0a 6775  ras_require]..gu
-000005f0: 6920 3d20 0d0a 0950 7951 7436 0d0a 7465  i = ...PyQt6..te
-00000600: 6e73 6f72 666c 6f77 203d 200d 0a09 7465  nsorflow = ...te
-00000610: 6e73 6f72 666c 6f77 3e3d 322e 3131 2e30  nsorflow>=2.11.0
-00000620: 0d0a 746f 7263 6820 3d20 0d0a 0974 6f72  ..torch = ...tor
-00000630: 6368 3e3d 322e 302e 300d 0a0d 0a5b 6f70  ch>=2.0.0....[op
-00000640: 7469 6f6e 732e 656e 7472 795f 706f 696e  tions.entry_poin
-00000650: 7473 5d0d 0a63 6f6e 736f 6c65 5f73 6372  ts]..console_scr
-00000660: 6970 7473 203d 200d 0a09 7965 617a 203d  ipts = ...yeaz =
-00000670: 2079 6561 7a2e 5f5f 6d61 696e 5f5f 3a72   yeaz.__main__:r
-00000680: 756e 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  un....[egg_info]
-00000690: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000006a0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
+00000010: 3d20 5965 615a 0a61 7574 686f 7220 3d20  = YeaZ.author = 
+00000020: 5361 6861 6e64 204a 616d 616c 2052 6168  Sahand Jamal Rah
+00000030: 690a 6175 7468 6f72 5f65 6d61 696c 203d  i.author_email =
+00000040: 2073 6168 616e 642e 7261 6869 4065 7066   sahand.rahi@epf
+00000050: 6c2e 6368 0a64 6573 6372 6970 7469 6f6e  l.ch.description
+00000060: 203d 2044 6565 702d 6c65 6172 6e69 6e67   = Deep-learning
+00000070: 2062 6173 6564 2079 6561 7374 2063 656c   based yeast cel
+00000080: 6c20 7365 676d 656e 7461 7469 6f6e 0a6b  l segmentation.k
+00000090: 6579 776f 7264 7320 3d20 0a09 6c69 7665  eywords = ..live
+000000a0: 2d63 656c 6c20 696d 6167 696e 670a 0963  -cell imaging..c
+000000b0: 656c 6c20 7365 676d 656e 7461 7469 6f6e  ell segmentation
+000000c0: 0a09 6365 6c6c 2074 7261 636b 696e 670a  ..cell tracking.
+000000d0: 0969 6d61 6765 2061 6e61 6c79 7369 730a  .image analysis.
+000000e0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000f0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+00000100: 6d64 0a6c 6f6e 675f 6465 7363 7269 7074  md.long_descript
+00000110: 696f 6e5f 636f 6e74 656e 745f 7479 7065  ion_content_type
+00000120: 203d 2074 6578 742f 6d61 726b 646f 776e   = text/markdown
+00000130: 0a75 726c 203d 2068 7474 7073 3a2f 2f67  .url = https://g
+00000140: 6974 6875 622e 636f 6d2f 7261 6869 2d6c  ithub.com/rahi-l
+00000150: 6162 2f59 6561 5a2d 4755 490a 7072 6f6a  ab/YeaZ-GUI.proj
+00000160: 6563 745f 7572 6c73 203d 200a 0952 6168  ect_urls = ..Rah
+00000170: 6920 6c61 6220 3d20 6874 7470 733a 2f2f  i lab = https://
+00000180: 7777 772e 6570 666c 2e63 682f 6c61 6273  www.epfl.ch/labs
+00000190: 2f6c 7062 732f 0a63 6c61 7373 6966 6965  /lpbs/.classifie
+000001a0: 7273 203d 200a 0944 6576 656c 6f70 6d65  rs = ..Developme
+000001b0: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
+000001c0: 2042 6574 610a 0950 726f 6772 616d 6d69   Beta..Programmi
+000001d0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001e0: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
+000001f0: 6c79 0a09 5072 6f67 7261 6d6d 696e 6720  ly..Programming 
+00000200: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+00000210: 6f6e 203a 3a20 332e 380a 0950 726f 6772  on :: 3.8..Progr
+00000220: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+00000230: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e39  :: Python :: 3.9
+00000240: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+00000250: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000260: 203a 3a20 332e 3130 0a09 4c69 6365 6e73   :: 3.10..Licens
+00000270: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000280: 6420 3a3a 2042 5344 204c 6963 656e 7365  d :: BSD License
+00000290: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+000002a0: 6e63 6520 3a3a 2045 6475 6361 7469 6f6e  nce :: Education
+000002b0: 0a09 496e 7465 6e64 6564 2041 7564 6965  ..Intended Audie
+000002c0: 6e63 6520 3a3a 2053 6369 656e 6365 2f52  nce :: Science/R
+000002d0: 6573 6561 7263 680a 094f 7065 7261 7469  esearch..Operati
+000002e0: 6e67 2053 7973 7465 6d20 3a3a 204d 6963  ng System :: Mic
+000002f0: 726f 736f 6674 203a 3a20 5769 6e64 6f77  rosoft :: Window
+00000300: 730a 094f 7065 7261 7469 6e67 2053 7973  s..Operating Sys
+00000310: 7465 6d20 3a3a 2050 4f53 4958 0a09 4f70  tem :: POSIX..Op
+00000320: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
+00000330: 3a20 556e 6978 0a09 4f70 6572 6174 696e  : Unix..Operatin
+00000340: 6720 5379 7374 656d 203a 3a20 4d61 634f  g System :: MacO
+00000350: 530a 0954 6f70 6963 203a 3a20 5363 6965  S..Topic :: Scie
+00000360: 6e74 6966 6963 2f45 6e67 696e 6565 7269  ntific/Engineeri
+00000370: 6e67 0a09 546f 7069 6320 3a3a 2053 6369  ng..Topic :: Sci
+00000380: 656e 7469 6669 632f 456e 6769 6e65 6572  entific/Engineer
+00000390: 696e 6720 3a3a 2042 696f 2d49 6e66 6f72  ing :: Bio-Infor
+000003a0: 6d61 7469 6373 0a09 546f 7069 6320 3a3a  matics..Topic ::
+000003b0: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+000003c0: 6e65 6572 696e 6720 3a3a 2049 6e66 6f72  neering :: Infor
+000003d0: 6d61 7469 6f6e 2041 6e61 6c79 7369 730a  mation Analysis.
+000003e0: 0954 6f70 6963 203a 3a20 5363 6965 6e74  .Topic :: Scient
+000003f0: 6966 6963 2f45 6e67 696e 6565 7269 6e67  ific/Engineering
+00000400: 203a 3a20 496d 6167 6520 5072 6f63 6573   :: Image Proces
+00000410: 7369 6e67 0a09 546f 7069 6320 3a3a 2053  sing..Topic :: S
+00000420: 6369 656e 7469 6669 632f 456e 6769 6e65  cientific/Engine
+00000430: 6572 696e 6720 3a3a 2056 6973 7561 6c69  ering :: Visuali
+00000440: 7a61 7469 6f6e 0a09 546f 7069 6320 3a3a  zation..Topic ::
+00000450: 2055 7469 6c69 7469 6573 0a0a 5b6f 7074   Utilities..[opt
+00000460: 696f 6e73 5d0a 7061 636b 6167 6573 203d  ions].packages =
+00000470: 2066 696e 643a 0a70 7974 686f 6e5f 7265   find:.python_re
+00000480: 7175 6972 6573 203d 200a 093e 3d33 2e39  quires = ..>=3.9
+00000490: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
+000004a0: 5f64 6174 6120 3d20 5472 7565 0a69 6e73  _data = True.ins
+000004b0: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
+000004c0: 0a09 6e75 6d70 793e 3d31 2e31 372e 340a  ..numpy>=1.17.4.
+000004d0: 096d 6174 706c 6f74 6c69 623e 3d33 2e31  .matplotlib>=3.1
+000004e0: 2e31 0a09 6e64 3272 6561 6465 723e 3d33  .1..nd2reader>=3
+000004f0: 2e33 2e30 0a09 6835 7079 3e3d 332e 382e  .3.0..h5py>=3.8.
+00000500: 300a 0973 6369 6b69 742d 696d 6167 653e  0..scikit-image>
+00000510: 3d30 2e31 352e 300a 096f 7065 6e70 7978  =0.15.0..openpyx
+00000520: 6c3e 3d33 2e31 2e32 0a09 6f70 656e 6376  l>=3.1.2..opencv
+00000530: 2d70 7974 686f 6e2d 6865 6164 6c65 7373  -python-headless
+00000540: 3e3d 342e 372e 302e 3732 0a09 7061 6e64  >=4.7.0.72..pand
+00000550: 6173 3e3d 302e 3235 2e33 0a09 6d75 6e6b  as>=0.25.3..munk
+00000560: 7265 730a 0973 6369 6b69 742d 6c65 6172  res..scikit-lear
+00000570: 6e3e 3d30 2e30 0a09 696d 6167 6569 6f3e  n>=0.0..imageio>
+00000580: 3d32 2e36 2e31 0a09 5069 6c6c 6f77 3e3d  =2.6.1..Pillow>=
+00000590: 362e 322e 310a 0974 7164 6d0a 0a5b 6f70  6.2.1..tqdm..[op
+000005a0: 7469 6f6e 732e 6578 7472 6173 5f72 6571  tions.extras_req
+000005b0: 7569 7265 5d0a 6775 6920 3d20 0a09 5079  uire].gui = ..Py
+000005c0: 5174 360a 7465 6e73 6f72 666c 6f77 203d  Qt6.tensorflow =
+000005d0: 200a 0974 656e 736f 7266 6c6f 773e 3d32   ..tensorflow>=2
+000005e0: 2e31 312e 300a 746f 7263 6820 3d20 0a09  .11.0.torch = ..
+000005f0: 746f 7263 683e 3d32 2e30 2e30 0a0a 5b6f  torch>=2.0.0..[o
+00000600: 7074 696f 6e73 2e65 6e74 7279 5f70 6f69  ptions.entry_poi
+00000610: 6e74 735d 0a63 6f6e 736f 6c65 5f73 6372  nts].console_scr
+00000620: 6970 7473 203d 200a 0979 6561 7a20 3d20  ipts = ..yeaz = 
+00000630: 7965 617a 2e5f 5f6d 6169 6e5f 5f3a 7275  yeaz.__main__:ru
+00000640: 6e0a 0a5b 6567 675f 696e 666f 5d0a 7461  n..[egg_info].ta
+00000650: 675f 6275 696c 6420 3d20 0a74 6167 5f64  g_build = .tag_d
+00000660: 6174 6520 3d20 300a 0a                   ate = 0..
```

### Comparing `YeaZ-1.0.0rc1/yeaz/GUI_main.py` & `YeaZ-1.0.1/yeaz/GUI_main.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1745 +1,1745 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-This script is the main script used to produce a GUI which should help for
-cell segmentation. This script can only read .nd2 files containing the 
-images of cells, especially it displays for each recorded positions (field
-of view) the pictures in the time axis.
-
-The script opens first a window which allows you to load an nd2 file and
-to load or create an hdf file. The hdf file contains all the masks, so if
-it is the first the user segments an nd2 file, a new one should be created.
-And it can be then loaded for later use.  Along with new hdf file, created
-by the name entered by the user (say filename), it creates three other hdf 
-files (filename_predicted.h5, filename_thresholded.h5 and 
-filename_segmented.h5) these contain all the steps of the NN to get to the 
-segmented picture. 
-
-After the first window is finished a second one opens, where at each time 
-index, three pictures 
-are displayed the t-1 picture, the t picture (current frame which can be
-edited) and the t+1 picture. Using the arrows one can navigate through time.
-On top of the picture, there is always a mask which is displayed, if no cells
-are present in the mask then the mask is blank and the user does not see it. 
-If one wants to hand anmotate the pictures, one can just start to draw on the
-picture using the different functions (New Cell, Add Region, Brush, Eraser,
-Save Mask, ...) and the informations will be saved in the mask overlayed on 
-top of the pictures. 
-
-If one wants to segment using a neural network, one can press the
-corresponding button (Launch CNN) and select the time range and 
-the field of views on which the neural network is applied.
-
-Once the neural network has finished predicting, there are still no visible
-masks, but on the field of views and time indices where the NN has been
-applied, the threshold and segment buttons are enabled. By checking these
-two buttons one can either display the thresholded image of the prediction or
-display the segmentation of the thresholded prediction.
-
-At this stage, one can correct the segmentation of the prediction using
-the functions (New Cell, Add Region, etc..) by selecting the Segment
-checkbox and then save them using the Save Seg button.
-If the user is happy with the segmentation, the Cell Correspondence button 
-can be clicked. Until then, the cells get random numbers attributed by
-the segmentation algorithm. In order to keep track of the cell through time,
-the same cells should have the same number between two different time pictures.
-This can be (with some errors) achieved by the Cell Correspondence button,
-which tries to attribute the same number to corresponding cells in time.
-After that, the final mask is saved and it is always visible when you go on
-the corresponding picture. This mask can also be corrected using the 
-usual buttons (because the Cell Correspondence makes also mistakes). 
-
-"""
-import sys
-import numpy as np
-import pandas as pd
-import h5py
-import skimage
-
-# For writing excel files
-#from openpyxl import load_workbook
-#from openpyxl import Workbook
-
-#Import from matplotlib to use it to display the pictures and masks.
-from matplotlib.backends.qt_compat import QtWidgets
-from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
-
-from sklearn.decomposition import PCA
-import imageio
-from PIL import Image, ImageDraw
-
-# tqdm for progress bar
-import tqdm
-import time
-
-# Import everything for the Graphical User Interface from the PyQt6 library.
-from PyQt6.QtWidgets import (QApplication, QMainWindow, QDialog, QSpinBox,
-    QMessageBox, QPushButton, QCheckBox, QStatusBar, QLabel)
-from PyQt6 import QtGui
-from PyQt6.QtGui import QAction
-from PyQt6.QtCore import Qt
-from PyQt6.QtGui import QPalette, QColor
-
-#Import all the other python files
-#this file handles the interaction with the disk, so loading/saving images
-#and masks and it also runs the neural network.
-from .disk import Reader as nd
-
-#this file contains a dialog window that takes two integers as entry to swap
-#two cell values
-from .misc import ExchangeCellValues as ecv
-
-#this file contains a window that opens to change the value of one cell. It 
-#is opened as soon as the user presses with the left click on a specific cell.
-from .misc import ChangeOneCellValue as cocv
-
-#this file contains a dialog window where a time range and the field of views
-#can be selected to then launch a prediction of the neural network on
-#a specific range of pictures.
-from .unet import LaunchBatchPrediction as lbp
-
-#this file contains a dialog window where a time range can be selected to retrack
-from .misc import BatchRetrack as br
-
-#this file initializes all the buttons present in the gui, sets the shortcuts
-#to these buttons and also connect the buttons to the function that are 
-#triggered when the buttons are pressed.
-from .init import InitButtons
-
-#this file contains the layout of the main window so it justs puts the buttons
-#and the pictures at the desired position in the main window.
-from .init import InitLayout
-
-# PlotCanvas for fast plotting
-from .misc.PlotCanvas import PlotCanvas
-
-from .misc import Extract as extr
-
-from .disk.image_loader import load_image
-from .unet.segment import segment
-from .unet import neural_network as nn
-from .misc.ProgressBar import ProgressBar
-
-import warnings
-# warnings.filterwarnings('ignore')
-
-import logging
-import os
-
-# Configure the root logger
-logging.basicConfig(
-    format='%(asctime)s %(levelname)s %(funcName)s: %(message)s',
-    level=os.environ.get("LOGLEVEL", "WARNING"),
-    filename='yeaz_GUI.log'
-)
-log = logging.getLogger(__name__)
-
-
-if getattr(sys, 'frozen', False):
-    path_icons = os.path.join(sys._MEIPASS, "icons/")
-    path_weights  = os.path.join(sys._MEIPASS, 'unet/')
-    
-else:
-    path_icons = './icons/'
-    path_weights = './unet/'
-
-
-class NavigationToolbar(NavigationToolbar):
-    """This is the standard matplotlib toolbar but only the buttons
-    that are of interest for this gui are loaded. These buttons allow 
-    to zoom into the pictures/masks and to navigate in the zoomed picture. 
-    A Home button can be used to set the view back to the original view.
-    """
-    toolitems = [t for t in NavigationToolbar.toolitems if
-                 t[0] in ('Home', 'Pan', 'Zoom','Back', 'Forward')]
-      
-class App(QMainWindow):
-    """This class creates the main window.
-    """
-
-    def __init__(self, nd2pathstr, hdfpathstr, newhdfstr):
-        super().__init__()
-        self.setWindowTitle('YeaZ')
-        log.info('initiating application')
-
-        # all these ids are integers which are used to set a connection between
-        # the button and the function that this button calls.
-        # There are three of them because it happens that one can trigger three 
-        # different functions with one button.        
-        self.id = 0
-        self.id2 = 0
-        self.id3 = 0 
-
-        self.reader = nd.Reader(hdfpathstr, newhdfstr, nd2pathstr)
-        
-        # these variables are used to create/read/load the excel file used
-        # to write the fluorescence values extracted. For each field of view,
-        # the user will be asked each time to create a new xls file for the 
-        # field of view or to load an existing field of view (this is the role
-        # of the boolean variable)
-        self.xlsfilename = ''
-        self.nd2path = nd2pathstr
-        
-        # Set the indices for the time axis and the field of view index. These
-        # indices represent everywhere the current picture (the one that can be
-        # edited, i.e. the time t frame)
-        self.Tindex = 0
-        self.FOVindex = 0
-        
-        # loading the first images of the cells from the nd2 file
-        self.currentframe = self.reader.LoadOneImage(self.Tindex,self.FOVindex)
-        
-        # check if the t+1 time frame exists, avoid failure if there is only
-        # one picture in the folder/nd2 file
-        if self.Tindex+1 < self.reader.sizet:
-            self.nextframe = self.reader.LoadOneImage(self.Tindex+1, self.FOVindex)
-        else:
-            self.nextframe = np.zeros([self.reader.sizey, self.reader.sizex])
-        
-        self.previousframe = np.zeros([self.reader.sizey, self.reader.sizex])
-
-        # loading the first masks from the hdf5 file
-        self.mask_curr = self.reader.LoadMask(self.Tindex, self.FOVindex)
-        self.mask_previous = np.zeros([self.reader.sizey, self.reader.sizex])
-        
-        # check if the t+1 mask exists, avoid failure if there is only
-        # one mask in the hdf file
-        if self.Tindex+1 < self.reader.sizet:
-            self.mask_next = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
-        else:
-            self.mask_next = np.zeros([self.reader.sizey, self.reader.sizex])
-        
-        # creates a list of all the buttons, which will then be used in order
-        # to disable all the other buttons at once when one button/function
-        # is pressed/used in the gui.
-        self.buttonlist = []
-        
-        # setting buttons as attributes
-        # the shortcuts for the buttons, the functions to which they are
-        # connected to,... are all set up in the ButtonInit file which is called
-        # in the self.initUI() method below.
-        self.button_newcell = QPushButton("New cell")
-        self.buttonlist.append(self.button_newcell)
-        
-        self.button_add_region = QPushButton("Add region")
-        self.buttonlist.append(self.button_add_region)
-        
-        self.button_drawmouse = QPushButton('Brush')
-        self.buttonlist.append(self.button_drawmouse)
-        
-        self.button_eraser = QPushButton('Eraser')
-        self.buttonlist.append(self.button_eraser)
-        
-        self.label_brushsize = QLabel('Brush/Eraser radius:')
-        self.spinbox_brushsize = QSpinBox()
-        self.buttonlist.append(self.spinbox_brushsize)
-        
-        self.button_exval = QPushButton('Exchange cell IDs')
-        self.buttonlist.append(self.button_exval)
-        
-        self.button_showval = QCheckBox('Show cell IDs')
-        self.buttonlist.append(self.button_showval)
-        
-        self.button_hidemask = QCheckBox('Hide mask')
-        self.buttonlist.append(self.button_hidemask)
-        
-        self.button_split = QPushButton('Split cell')
-        self.buttonlist.append(self.button_split)
-        
-        self.button_mergewithneighbors = QPushButton('Merge cells')
-        self.buttonlist.append(self.button_mergewithneighbors)
-        
-        self.button_nextframe = QPushButton("Next time frame")
-        self.buttonlist.append(self.button_nextframe)
-        
-        self.button_previousframe = QPushButton("Previous time frame")
-        self.buttonlist.append(self.button_previousframe)
-        
-        self.button_cnn = QPushButton('Launch CNN')
-        self.buttonlist.append(self.button_cnn)
-        
-        self.button_cellcorrespondence = QPushButton('Retrack')
-        self.buttonlist.append(self.button_cellcorrespondence)
-        
-        self.button_changecellvalue = QPushButton('Change cell ID')
-        self.buttonlist.append(self.button_changecellvalue)        
-        
-        self.button_extractfluorescence = QPushButton('Extract')
-        self.buttonlist.append(self.button_extractfluorescence)
-        
-        self.button_hide_show = QPushButton('CNN')
-        self.buttonlist.append(self.button_hide_show)
-        
-        self.initUI()
-
-
-    def initUI(self):
-        """Initializing the widgets contained in the window. 
-        Especially, it creates the widget to plot the 
-        pictures/masks by creating an object of the PlotCanvas class self.m. 
-        Every interaction with the masks or the pictures (loading new
-        frames/editing the frames/masks) occurs through this class.
-        
-        This method initializes all the buttons with the InitButtons file.
-        It connects the buttons to the functions that they should trigger,
-        it sets the shortcuts to the buttons, a tool tip, 
-        eventually a message on the status bar when the user hovers 
-        over the button, etc..
-        
-        This function also sets all the layout in the InitLayout file. It 
-        takes and places the widgets (buttons, canvas, toolbar).
-
-        The function initializes a Menu Bar to have a menu which can be 
-        improved later on.
-        It sets a toolbar of the matplotlib library and hides it. But it allows
-        to connect to the functions of this toolbar through "homemade" 
-        QPushButtons instead of the ones provided by matplotlib.
-        Finally, it sets a StatusBar which displays some text to describe
-        the use of some buttons, or to show that the program is working on 
-        something (running the neural network, loading frames, etc...)
-        
-        After all this has been initialized, the program is ready to be used.
-        """
-        log.info('initiate UI')
-        self._main = QtWidgets.QWidget()
-        self.setCentralWidget(self._main)
-
-        # Here our canvas is created where using matplotlib, 
-        # one can plot data to display the pictures and masks.
-        self.m = PlotCanvas(self)
-        
-        # Initialize all the buttons that are needed and the functions that are 
-        # connected when the buttons are triggered.
-        InitButtons.Init(self)
-        InitLayout.Init(self)
-        
-        # MENU, TOOLBAR AND STATUS BAR
-        # creates a menu just in case, some other functions can be added later
-        # in this menu.
-#        menubar = self.menuBar()
-#        self.fileMenu = menubar.addMenu('File')   
-#        self.saveactionmenu = QAction('Save')
-#        self.fileMenu.addAction(self.saveactionmenu)
-#        self.saveactionmenu.triggered.connect(self.SaveMask)
-        
-        # hide the toolbar and instead of the original buttons of matplotlib,
-        # QPushbuttons are used and are connected to the functions of the toolbar
-        # it is than easier to interact with these buttons (for example to 
-        # to disable them and so on..)
-        self.Nvgtlbar = NavigationToolbar(self.m, self)
-        self.addToolBar(self.Nvgtlbar)
-        self.Nvgtlbar.hide()
-        
-        # creates a status bar with user instructions
-        self.statusBar = QStatusBar()
-        self.setStatusBar(self.statusBar)
-        self.statusBarText = QLabel()
-        self.statusBar.addWidget(self.statusBarText)
-                
-        self.show()
-                
-        
-# -----------------------------------------------------------------------------
-# FUNCTIONS LINKED TO NAVIGATION
-# connect the functions of the toolbar to our custom QPushbuttons.
-    def ZoomTlbar(self):
-        """The button_zoom is connected to the zoom function of the toolbar 
-        already present in the matplotlib library.
-        
-        Depending on the buttons that are active or checked, when the zoom 
-        function is used, it does not disable all the buttons.
-        
-        If the segment and threshold button are not checked or used
-        when the zoom button is clicked, it disables all the button
-        using self.Disable which disables everything except the button passed
-        in argument (in this case button_zoom).
-        
-        If the zoom button is used while the segment button is checked,
-        it disables all the buttons (1st elif) except the segment button
-        but once it is finished (so the zoom button becomes unchecked) 
-        then it enables only the editing buttons (as long as the segment
-        button is still checked) such as New Cell, Add Region, Eraser, 
-        Brush,etc.. and the other toolbar buttons (3rd elif)
-        
-        
-        If the zoom button is clicked while the threshold button is checked,
-        it disables all the button except the threshold button (2nd elif).
-        Once the zoom button is unchecked, it enables the toolbar buttons
-        (4th elif)
-        In any other case, it just enables all the buttons again.
-        """
-        self.Nvgtlbar.zoom()
-        
-        if (self.button_zoom.isChecked()):
-            self.Disable(self.button_zoom)
-            
-        else:
-            self.Enable(self.button_zoom)
-        
-        
-    def HomeTlbar(self):
-        """
-        connects the home button to the home function of the matplotlib
-        toolbar. It sets the view to the original view (no zoom)
-        """
-        self.Nvgtlbar.home()
-
-            
-    def BackTlbar(self):
-        """
-        It calls the back function of the matplotlib toolbar which sets the 
-        view to the previous one (if the user does several zooms/pans, 
-        this button allows to go back in the "history of views")
-        """
-        self.Nvgtlbar.back()
-
-        
-    def ForwardTlbar(self):
-        """
-        It calls the forward function of the matplotlib toolbar which sets the 
-        view to the next one (if the user does several zooms/pans, 
-        this button allows to go forward in the "history of views"
-        """
-        self.Nvgtlbar.forward()
-
-    
-    def PanTlbar(self):
-        """The button_pan is connected to the pan function of the toolbar 
-        already present in the matplotlib library.
-        
-        Depending on the buttons that are active or checked, when the pan 
-        function is used, it does not disable all the buttons.
-        
-        If the segment and threshold button are not checked or used
-        when the pan button is clicked, it disables all the button
-        using self.Disable which disables everything except the button passed
-        in argument (in this case button_pan).
-        
-        If the pan button is used while the segment button is checked,
-        it disables all the buttons (1st elif) except the segment button
-        but once it is finished (so the zoom button becomes unchecked) 
-        then it enables only the editing buttons (as long as the segment
-        button is still checked) such as New Cell, Add Region, Eraser, 
-        Brush,etc.. and the other toolbar buttons (3rd elif)
-        
-        
-        If the pan button is clicked while the threshold button is checked,
-        it disables all the button except the threshold button (2nd elif).
-        Once the pan button is unchecked, it enables the toolbar buttons
-        (4th elif)
-        In any other case, it just enables all the buttons again.
-        """
-
-        self.Nvgtlbar.pan()
-
-        if (self.button_pan.isChecked()):
-            self.Disable(self.button_pan)
-        else:
-            self.Enable(self.button_pan)
-
-            
-    def ButtonFluo(self):
-        """This function is called everytime the Extract Fluorescence button is 
-        clicked (self.button_extractfluorescence). 
-        """        
-        self.Disable(self.button_extractfluorescence)
-        self.WriteStatusBar('Extracting ...')
-        
-        # Get last image with mask
-        for time_index in range(self.reader.sizet-1, -1, -1):            
-            # Test if time has a mask
-            file = h5py.File(self.reader.hdfpath, 'r+')
-            time_exist = self.reader.TestTimeExist(time_index, self.FOVindex, file)
-            file.close()
-            
-            if not time_exist:
-                continue
-            
-            # load picture and sheet
-            image = self.reader.LoadImageChannel(time_index, self.FOVindex, 
-                                                 self.reader.default_channel)
-            mask = self.reader.LoadMask(time_index, self.FOVindex)
-            
-            # Break if mask is non-empty
-            if mask.sum()>0:
-                break
-            
-            if time_index==0:
-                msg_box = QMessageBox(QMessageBox.Icon.Critical, 'Error', 'No mask found', parent=self)
-                msg_box.exec()
-                self.Enable(self.button_extractfluorescence)
-                self.ClearStatusBar()
-        
-        # Launch dialog with last image
-        dlg = extr.Extract(image, mask, self.reader.channel_names)
-        dlg.exec()
-        if dlg.exit_code == 1: # Fluorescence
-            self.ExtractFluo(dlg.cells, dlg.desel_cells, dlg.outfile, dlg.file_list)
-        elif dlg.exit_code == 2: # Mask
-            self.ExtractMask(dlg.desel_cells, dlg.outfile)
-            
-        self.Enable(self.button_extractfluorescence)
-        self.ClearStatusBar()
-
-
-    def ExtractMask(self, desel_cells, outfile):
-        """Extract the mask to the specified tiff file. Only take cells 
-        specified by the cell_list"""
-        
-        mask_list = []
-        for time_index in range(0, self.reader.sizet):
-            
-            # Test if time has a mask
-            file = h5py.File(self.reader.hdfpath, 'r+')
-            time_exist = self.reader.TestTimeExist(time_index, self.FOVindex, file)
-            file.close()
-            
-            if not time_exist:
-                continue
-            
-            mask = self.reader.LoadMask(time_index, self.FOVindex)
-            for cell in desel_cells:
-                mask[mask==cell] = 0
-            mask_list.append(mask)
-            
-        imageio.mimwrite(outfile, np.array(mask_list, dtype=np.uint16))
-                        
-
-    def ExtractFluo(self, sel_cells, desel_cells, csv_filename, channel_list):
-        """This is the function that takes as argument the filepath to the xls
-        file and writes in the file.
-        It iterates over the different channels (or the sheets of the file,
-        each channel has one sheet.), and reads the image corresponding
-        to the time, field of view and channel index. It reads the already
-        existing file and makes a copy in which the data will be written in it.
-        
-        The first step of calculating the data is to iterate through each
-        cell/segment of the mask (so each cell is a submatrix of one value
-        in the matrix of the mask).
-        For each of these value /cell, the area is extracted as being
-        the number of pixels corresponding to this cell/value. 
-        (it is known from the microscope settings how to convert
-        the pixel in area).
-        The total intensity is just the value of the pixel and it is added over
-        all the pixels corresonding to the cell/value.
-        The mean is then calculated as being the total intensity divided by
-        the number of pixels (which here is equal to the area also).
-        With the mean it is then possible to calculate the variance of the 
-        signal for one cell/value.
-        
-        Then, it is checked if the value of the cell (cell number) already
-        exists in the first column, if it already exists it continues to
-        find the column corresponding to the time index where the values
-        should be written. It sets the flag to True such that it does not
-        write the cell as new one and adds it at the end of the column
-        
-        If the value is not found in the cell number column (new cell or
-        first time writing in the file), the flag is False, thus it adds the 
-        cell number at the end of the column.
-        It then saves the xls file.
-        
-        """
-        # List of cell properties
-        cell_list = []
-
-        for time_index in range(0, self.reader.sizet):
-            # Test if time has a mask
-            file = h5py.File(self.reader.hdfpath, 'r+')
-            time_exist = self.reader.TestTimeExist(time_index, self.FOVindex, file)
-            file.close()
-            
-            if not time_exist:
-                continue
-            
-            mask = self.reader.LoadMask(time_index, self.FOVindex)
-            
-            for channel in channel_list:
-                # check if channel is in list of nd2 channels
-                try:
-                    channel_ix = self.reader.channel_names.index(channel)
-                    image = self.reader.LoadImageChannel(time_index, self.FOVindex, channel_ix)
-                
-                # channel is a file
-                except ValueError:
-                    image = load_image(channel, ix=time_index)
-                    
-                for val in np.unique(mask):
-                    # bg is not cell
-                    if val == 0:
-                        continue
-                    # disregard cells not in cell_list
-                    if (val in desel_cells):
-                        continue
-                    
-                    # Calculate stats
-                    stats = {'Cell': val,
-                             'Time': time_index,
-                             'Channel': channel}
-                    
-                    stats = {**stats,
-                             **self.cell_statistics(image, mask == val)}
-                    stats['Disappeared in video'] = not (val in sel_cells)
-                    cell_list.append(stats)
-                    
-        
-        # Use Pandas to write csv
-        df = pd.DataFrame(cell_list)
-        df = df.sort_values(['Cell', 'Time'])
-        df.to_csv(csv_filename, index=False)
-                    
-        self.Enable(self.button_extractfluorescence)
-        self.ClearStatusBar()
-
-
-    def cell_statistics(self, image, mask):
-        """Calculate statistics about cells. Passing None to image will
-        create dictionary to zeros, which allows to extract dictionary keys"""
-        if image is not None:
-            cell_vals = image[mask]
-            area = mask.sum()
-            tot_intensity = cell_vals.sum()
-            mean = tot_intensity/area if area > 0 else 0
-            var = np.var(cell_vals)
-            
-            # Center of mass
-            y,x = mask.nonzero()
-            com_x = np.mean(x)
-            com_y = np.mean(y)
-            
-            # PCA only works for multiple points
-            if area > 1:
-                pca = PCA().fit(np.array([x,y]).T)
-                pc1_x, pc1_y = pca.components_[0,:]
-                angle = np.arctan(pc1_y / pc1_x) / (2*np.pi) * 360
-                v1, v2 = pca.explained_variance_
-                
-                len_maj = 4*np.sqrt(v1)
-                len_min = 4*np.sqrt(v2)
-            else:
-                angle = 0
-                len_maj = 1
-                len_min = 1
-            
-        else:
-            mean = 0
-            var = np.nan
-            tot_intensity = 0
-            com_x = np.nan
-            com_y = np.nan
-            angle = np.nan
-            len_maj = np.nan
-            len_min = np.nan
-        
-        return {'Area': area,
-                'Mean': mean,
-                'Variance': var,
-                'Total Intensity': tot_intensity,
-                'Center of Mass X': com_x,
-                'Center of Mass Y': com_y,
-                'Angle of Major Axis': angle,
-                'Length Major Axis': len_maj,
-                'Length Minor Axis': len_min}
-
-# -----------------------------------------------------------------------------
-# NEURAL NETWORK
-    def ShowHideCNNbuttons(self):
-        """hide and show the buttons corresponding to the neural network.
-            this function is called by the button CNN which is hidden. But
-            if activated in the InitLayout.py then you can have a button
-            which hides the CNN buttons (which are now on the normal also
-            hidden...).
-        """
-        if self.button_hide_show.isChecked():
-            self.button_cnn.setVisible(True)
-
-        else:
-            self.button_cnn.setVisible(False)
-            
-
-    def LaunchBatchPrediction(self):
-        """This function is called whenever the button Launch CNN is pressed.
-        It allows to run the neural network over a time range and selected
-        field of views.
-            
-        It creates a dialog window with two entries, that define the time range
-        and a list where the user can select the desired fields of view.
-        
-        Once it reads all the value, it calls the neural network function
-        inside of self.PredThreshSeg and it does the prediction of the neural
-        network, thresholds this prediction and then segments it.
-        """
-        def reset():
-            self.m.UpdatePlots()
-            self.ClearStatusBar()
-            self.Enable(self.button_cnn)
-            self.EnableCNNButtons()
-        
-        
-        self.WriteStatusBar('Running the neural network...')
-        self.Disable(self.button_cnn)
-
-        # creates a dialog window from the LaunchBatchPrediction.py file
-        dlg = lbp.CustomDialog(self)
-        
-        # this if tests if the user pressed 'ok' in the dialog window
-        result = dlg.exec()
-        if result == QDialog.DialogCode.Accepted:
-            # it tests if the user has entered some values
-            # if not it ignores and returns.
-            if not (dlg.entry1.text()!= '' and dlg.entry2.text() != ''):
-                msg_box = QMessageBox(QMessageBox.Icon.Critical, 'Error', "No Time Specified", parent=self)
-                msg_box.exec()
-                reset()
-                return 
-            
-            # reads out the entry given by the user and converts the index
-            # to integers
-            time_value1 = int(dlg.entry1.text())
-            time_value2 = int(dlg.entry2.text())
-    
-            # it tests if the first value is smaller or equal such that
-            # time_value1 is the lower range of the time range
-            # and time_value2 the upper boundary of the range.
-            if time_value1 > time_value2 :
-                msg_box = QMessageBox(QMessageBox.Icon.Critical, 'Error', 'Invalid Time Constraints', parent=self)
-                msg_box.exec()
-                reset()
-                return
-            
-            # displays that the neural network is running
-            self.WriteStatusBar('Running the neural network...')
-    
-            #it iterates in the list of the user-selected fields 
-            #of view, to return the corresponding index, the function
-            #dlg.listfov.row(item) is used which gives an integer
-            if len(dlg.listfov.selectedItems())==0:
-                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", "No FOV Selected", parent=self)
-                msg_box.exec()
-            # Check if the user have selected a mic type
-            
-            mic_type = dlg.mic_type.currentData()
-            if dlg.mic_type.currentData() is not None:
-                # User has selected an option, do something with it
-                log.debug(msg='Mic type selected: {}'.format(mic_type))
-            else:
-                # User has not selected any option, show error message
-                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", "No Image Type Selected", parent=self)
-                msg_box.exec()
-                reset()
-                return 
-            
-            # decide between cuda or cpu for running neural network
-            device = None
-            import torch
-            if (dlg.device_selection.currentData() == 'cuda') and (torch.cuda.is_available()):
-                device = 'cuda'
-            else:
-                device = 'cpu'
-            
-            for item in tqdm.tqdm(dlg.listfov.selectedItems(), desc='FOV', position=0, leave=True):
-                #iterates over the time indices in the range
-                for t in tqdm.tqdm(range(time_value1, time_value2+1), desc='Time', position=1, leave=False):                    
-                    #calls the neural network for time t and selected
-                    #fov
-                    if dlg.entry_threshold.text() !=  '':
-                        thr_val = float(dlg.entry_threshold.text())
-                    else:
-                        thr_val = None
-                    if dlg.entry_segmentation.text() != '':
-                        seg_val = int(dlg.entry_segmentation.text())
-                    else:
-                        seg_val = 10
-                    
-                    self.PredThreshSeg(t, dlg.listfov.row(item), thr_val, seg_val,
-                                       mic_type, device=device)
-                    
-                    # apply tracker if wanted and if not at first time
-                    temp_mask = self.reader.CellCorrespondence(t, dlg.listfov.row(item))
-                    self.reader.SaveMask(t,dlg.listfov.row(item), temp_mask)
-            
-            self.ReloadThreeMasks()
-        reset()
-
-    
-    def PredThreshSeg(self, timeindex, fovindex, thr_val, seg_val, 
-                      mic_type, device=None):
-        """
-        This function is called in the LaunchBatchPrediction function.
-        This function calls the neural network function in the
-        InteractionDisk.py file and then thresholds the result
-        of the prediction, saves this thresholded prediction.
-        Then it segments the thresholded prediction and saves the
-        segmentation. 
-        """
-        log.debug('--------- Segmenting field of view:',fovindex,'Time point:',timeindex)
-        im = self.reader.LoadOneImage(timeindex, fovindex)
-        try:
-            pred = self.LaunchPrediction(im, mic_type, device=device)
-        except ValueError:
-            msg_box = QMessageBox(QMessageBox.Icon.Critical,'Error',
-                                 'The neural network weight files could not '
-                                 'be found. Make sure to download them from '
-                                 'the link in the readme and put them into '
-                                 'the folder unet', parent=self)
-            msg_box.exec()
-            
-            return
-
-        thresh = self.ThresholdPred(thr_val, pred)
-        seg = segment(thresh, pred, seg_val)
-        self.reader.SaveMask(timeindex, fovindex, seg)
-        log.debug('--------- Finished segmenting.')
-          
-          
-    @staticmethod
-    def LaunchPrediction(im, mic_type, pretrained_weights=None, device=None):
-        """It launches the neural neutwork on the current image and creates 
-        an hdf file with the prediction for the time T and corresponding FOV. 
-        """
-        im = skimage.exposure.equalize_adapthist(im)
-        im = im*1.0;	
-        pred = nn.prediction(im, mic_type, pretrained_weights, device=device)
-        return pred
-
-
-    @staticmethod
-    def ThresholdPred(thvalue, pred):
-        """Thresholds prediction with value"""
-        if thvalue == None:
-            thresholdedmask = nn.threshold(pred)
-        else:
-            thresholdedmask = nn.threshold(pred, thvalue)
-        return thresholdedmask
-
-    
-    def SelectChannel(self, index):
-        """This function is called when the button to select different channels
-        is used. From the displayed list in the button, the chosen index
-        corresponnds to the same index in the list of channels from the reader.
-        So, it sets the default channel with the new index (called index below)
-        """
-        self.reader.default_channel = index
-        # update the pictures using the same function as the one used to 
-        # change the fields of view.
-        self.ChangeFOV()
-        
-
-    def SelectFov(self, index):
-        """This function is called when the button containing the list of 
-        fields od view is used.
-        The index correspondds to the field of view selected in the list.
-        """
-        # mask is automatically saved.
-        self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
-        self.FOVindex = index    
-        
-        # it updates the fov in the plot with the new index.
-        self.ChangeFOV()
-                
-        
-    def ChangeFOV(self):
-        """
-        it changes the fov or channel according to the choice of the user
-        and it updates the plot shown and it initializes the new fov/channel
-        at t=0 by default.
-        """
-        
-        self.Tindex = 0
-        
-        # load the image and mask for the current plot
-        self.m.currpicture = self.reader.LoadOneImage(self.Tindex,self.FOVindex)
-        self.m.plotmask = self.reader.LoadMask(self.Tindex,self.FOVindex)
-        
-        # sets the image and the mask to 0 for the previous plot
-        self.m.prevpicture = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
-        self.m.prevplotmask = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
-        
-        # load the image and the mask for the next plot, check if it exists
-        if self.Tindex+1 < self.reader.sizet:
-            self.m.nextpicture = self.reader.LoadOneImage(self.Tindex+1, self.FOVindex)
-            self.m.nextplotmask = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
-            
-            # enables the next frame button in case it was disabled when the 
-            # fov/channel was changed
-            self.button_nextframe.setEnabled(True)
-        else:
-            self.m.nextpicture = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
-            self.m.nextplotmask =  np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
-            
-            # disables the next frame button if the mask or the picture
-            # does not exist.
-            self.button_nextframe.setEnabled(False)
-            
-        # once the images and masks are loaded into the variables, they are 
-        # displaye in the gui.
-        self.m.UpdatePlots()
-        
-        # disables the previous frame button in case it was active before 
-        # changing fov/channel.
-        self.button_previousframe.setEnabled(False)
-        
-        # updates the title of the plots to display the right time indices
-        # aboves the plots.
-        self.UpdateTitleSubplots()
-            
-        # if the button to hide the mask was checked before changing fov/channel,
-        # it hides the mask again.
-        if self.button_hidemask.isChecked():
-            self.m.HideMask()
-        
-        # the button to set the time index is also set to 0/default again.
-        self.button_timeindex.setText('')
-        # enables the neural network buttons if there is already an 
-        # existing prediction for the current image.
-        self.EnableCNNButtons()
-        
-        
-    def ReloadThreeMasks(self):
-        """
-        A function which replots all the masks at the current time and fov 
-        indices. Needed after the batch prediction is completed to display
-        the result of the NN.
-        """
-        log.debug("reload three mask for frame {}".format(self.Tindex))
-        
-        if self.Tindex >= 0 and self.Tindex <= self.reader.sizet-1:
-            if self.Tindex == 0:
-                self.button_nextframe.setEnabled(True)
-                
-                if self.Tindex < self.reader.sizet-1:
-                    self.m.nextplotmask = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
-                else:
-                    np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
-                
-                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)
-                self.m.prevplotmask = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
-                self.m.UpdatePlots()
-                self.button_previousframe.setEnabled(False)
-                
-                
-            elif self.Tindex == self.reader.sizet-1:
-                self.button_previousframe.setEnabled(True)
-                self.m.prevplotmask = self.reader.LoadMask(self.Tindex-1, self.FOVindex)
-                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)
-                self.m.nextplotmask =  np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
-                self.m.UpdatePlots()
-                self.button_nextframe.setEnabled(False)
-                
-            else:
-                self.button_nextframe.setEnabled(True)
-                self.button_previousframe.setEnabled(True)
-                self.m.prevplotmask = self.reader.LoadMask(self.Tindex-1, self.FOVindex)
-                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)              
-                self.m.nextplotmask = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
-                self.m.UpdatePlots()
-            
-            self.UpdateTitleSubplots()
-                        
-            if self.button_hidemask.isChecked():
-                self.m.HideMask()
-            self.EnableCNNButtons()
-        
-        else:
-            return
-        
-    
-    def ChangeTimeFrame(self):
-        """This funcion is called whenever the user gives a new time index, 
-        to jump to the new given index, once "enter" button is pressed.
-        """
-        
-        # it reads out the text in the button and converts it to an int.
-        newtimeindex = int(self.button_timeindex.text())
-        if newtimeindex >= 0 and newtimeindex <= self.reader.sizet-1:
-            self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
-            
-            self.Tindex = newtimeindex
-            
-            if self.Tindex == 0:
-                self.button_nextframe.setEnabled(True)
-                self.m.nextpicture = self.reader.LoadOneImage(self.Tindex+1,self.FOVindex)
-                self.m.nextplotmask = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
-                
-                self.m.currpicture = self.reader.LoadOneImage(self.Tindex, self.FOVindex)
-                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)
-                
-                self.m.prevpicture = np.zeros([self.reader.sizey, self.reader.sizex], 
-                                              dtype = np.uint16)
-                self.m.prevplotmask = np.zeros([self.reader.sizey, self.reader.sizex], 
-                                               dtype = np.uint16)
-    
-                self.m.UpdatePlots()
-                self.button_previousframe.setEnabled(False)
-                
-            elif self.Tindex == self.reader.sizet-1:
-                self.button_previousframe.setEnabled(True)
-                self.m.prevpicture = self.reader.LoadOneImage(self.Tindex-1, self.FOVindex)
-                self.m.prevplotmask = self.reader.LoadMask(self.Tindex-1, self.FOVindex)
-                   
-                self.m.currpicture = self.reader.LoadOneImage(self.Tindex, self.FOVindex)
-                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)
-                  
-                self.m.nextpicture =  np.zeros([self.reader.sizey, self.reader.sizex], 
-                                               dtype = np.uint16)
-                self.m.nextplotmask =  np.zeros([self.reader.sizey, self.reader.sizex], 
-                                                dtype = np.uint16)
-                
-                self.m.UpdatePlots()
-                self.button_nextframe.setEnabled(False)
-                
-            else:
-                self.button_nextframe.setEnabled(True)
-                self.button_previousframe.setEnabled(True)
-                self.m.prevpicture = self.reader.LoadOneImage(self.Tindex-1, self.FOVindex)
-                self.m.prevplotmask = self.reader.LoadMask(self.Tindex-1, self.FOVindex)
-                   
-                self.m.currpicture = self.reader.LoadOneImage(self.Tindex, self.FOVindex)
-                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)              
-                  
-                self.m.nextpicture = self.reader.LoadOneImage(self.Tindex+1,self.FOVindex)
-                self.m.nextplotmask = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
-                self.m.UpdatePlots()
-            
-            self.UpdateTitleSubplots()
-            self.button_timeindex.clearFocus()
-            self.button_timeindex.setText(str(self.Tindex)+'/'+str(self.reader.sizet-1))
-            
-            if self.button_hidemask.isChecked():
-                self.m.HideMask()
-            self.EnableCNNButtons()
-        
-        else:
-            self.button_timeindex.clearFocus()
-            return
-        
-    def BatchCellCorresp(self):
-        def reset():
-            self.ClearStatusBar()
-            self.Enable(self.button_cellcorrespondence)
-            self.button_cellcorrespondence.setChecked(False)
-        
-        self.Disable(self.button_cellcorrespondence)
-        self.WriteStatusBar('retracking... ')
-
-        if(self.Tindex==self.reader.sizet-1):
-            msg_box = QMessageBox(QMessageBox.Icon.Critical, 'Error',"This is the last frame. Nothing to retrack after this", parent=self)
-            msg_box.exec()
-            reset()
-            return 
-
-
-        # creates a dialog window from the BatchRetrack.py file
-        dlg = br.CustomDialog(self)
-        
-        # this if tests if the user pressed 'ok' in the dialog window
-        result = dlg.exec()
-        if result == QDialog.DialogCode.Accepted:
-            # it tests if the user has entered some values
-            if not (dlg.entry1.text()!= ''):
-                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", "No Time Specified", parent=self)
-                msg_box.exec()
-                reset()
-                return 
-            
-            # reads out the entry given by the user and converts the index
-            # to integers
-            time_value1 = int(dlg.entry1.text())
-    
-            # it tests if the value is bigger than current frame
-            if (time_value1 <  self.Tindex or time_value1 > self.reader.sizet-1):
-                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", 'Invalid Time Constraints', parent=self)
-                msg_box.exec()
-                reset()
-                return
-            # if everything was okay, start a progress bar to show progress:
-            progress = ProgressBar(self)
-            progress_value = 0
-            ratio = 100/(time_value1 - self.Tindex)
-            for t in range(self.Tindex+1, time_value1+1):
-                log.debug('start correspondance for frame {}'.format(t))                    
-                #calls the cell correspondance for current time, t, and t+1
-                temp_mask = self.reader.CellCorrespondence(t, self.FOVindex)
-                progress_value += ratio
-                progress.update_progress(progress_value)
-                # update the progress status label
-                progress.status.setText("Processing frame {}... ".format(t+1))
-                self.reader.SaveMask(t, self.FOVindex, temp_mask)
-                QApplication.processEvents()  # Process events to allow GUI to update               
-                log.debug('finish correspondance and savemask for frame {}'.format(t))                    
-            # close the progress bar dialog
-            progress.close()
-            self.ReloadThreeMasks()
-
-            log.info('reload three frames')
-        reset()
-
-    def CellCorrespActivation(self):
-        log.debug('An outdated function is called')
-        self.Disable(self.button_cellcorrespondence)
-        self.WriteStatusBar('Doing the cell correspondence')
-        if self.Tindex > 0:
-            self.m.plotmask = self.reader.CellCorrespondence(self.Tindex, self.FOVindex)
-            self.m.updatedata()
-        else:
-            pass
-            #self.m.plotmask = self.reader.LoadSeg(self.Tindex, self.FOVindex)
-            #self.m.updatedata()
-
-        self.Enable(self.button_cellcorrespondence)
-        self.button_cellcorrespondence.setChecked(False)
-        self.ClearStatusBar()
-        self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
-    
-    def ButtonSaveSegMask(self):
-        """saves the segmented mask
-        """
-        self.reader.SaveSegMask(self.Tindex, self.FOVindex, self.m.plotmask)
-
-        
-    def ChangePreviousFrame(self):
-         """This function is called when the previous frame buttons is pressed 
-         and it tests if the buttons is enabled and if so it calls the
-         BackwardTime() function. It should avoid the let the user do multiple 
-         clicks and that the function is then called afterwards several times,
-         once the frames and masks of the current time index have been loaded.
-         """
-         if self.button_previousframe.isEnabled():
-            self.button_previousframe.setEnabled(False)
-            self.BackwardTime()
-            if self.Tindex >0:
-                self.button_previousframe.setEnabled(True)
-         else:
-             return
-             
-             
-    def ChangeNextFrame(self):
-        """This function is called when the next frame buttons is pressed 
-        and it tests if the buttons is enabled and if so it calls the
-        ForwardTime() function. It should avoid the let the user do multiple 
-        clicks and that the function is then called afterwards several times,
-        once the frames and masks of the current time index have been loaded.
-        """
-        if self.button_nextframe.isEnabled():
-            self.button_nextframe.setEnabled(False)
-            self.ForwardTime()
-            if self.Tindex + 1 < self.reader.sizet:
-                self.button_nextframe.setEnabled(True)
-                
-        else:
-            return
-
-        
-    def ForwardTime(self):
-        """This function switches the frame in forward time index. And it tests
-        several conditions if t == lastTimeIndex-1, because then the next frame
-        button has to be disabled. It also tests if the show value of cells
-        button and hidemask are active in order to hide/show the mask or to 
-        show the cell values.
-        """
-        # the t frame is defined as the currently shown frame on the display.
-        # If the button "Next time frame" is pressed, this function is called
-        self.WriteStatusBar('Loading the next frame...')
-        self.Disable(self.button_nextframe)
-
-        if self.Tindex + 1 < self.reader.sizet - 1 :
-            self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
-            
-            self.m.prevpicture = self.m.currpicture.copy()
-            self.m.prevplotmask = self.m.plotmask.copy()
-            
-            self.m.currpicture = self.m.nextpicture.copy()
-            self.m.plotmask = self.m.nextplotmask.copy()
-            
-            self.m.nextpicture = self.reader.LoadOneImage(self.Tindex+2, self.FOVindex)
-            self.m.nextplotmask = self.reader.LoadMask(self.Tindex+2, self.FOVindex)
-
-            if self.Tindex + 1 == 1:
-                self.button_previousframe.setEnabled(True)
-                
-        else:
-            self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
-        
-            self.m.prevpicture = self.m.currpicture.copy()
-            self.m.prevplotmask = self.m.plotmask.copy()
-            self.m.currpicture = self.m.nextpicture.copy()
-            self.m.plotmask = self.m.nextplotmask.copy()
-            self.m.nextpicture = np.zeros([self.reader.sizey, self.reader.sizex], 
-                                          dtype = np.uint16)
-            self.m.nextplotmask = np.zeros([self.reader.sizey,self.reader.sizex], 
-                                           dtype = np.uint16)
-
-            self.button_nextframe.setEnabled(False)
-
-        self.Tindex = self.Tindex+1
-        self.m.UpdatePlots()
-        self.UpdateTitleSubplots()
-        
-        if self.button_hidemask.isChecked():
-            self.m.HideMask()
-
-        self.Enable(self.button_nextframe)
-        self.ClearStatusBar()
-        self.button_timeindex.setText(str(self.Tindex)+'/'+str(self.reader.sizet-1))
-
-    
-    def BackwardTime(self):
-        """This function switches the frame in backward time index. And it 
-        several conditions if t == 1, because then the button previous frame has to
-        be disabled. It also tests if the show value of cells button and 
-        hidemask are active in order to hide/show the mask or to show the cell
-        values.
-        """
-        # the t frame is defined as the currently shown frame on the display.
-        # If the button "Previous time frame" is pressed, this function is called
-        self.WriteStatusBar('Loading the previous frame...')
-        self.Disable(self.button_previousframe)
-        
-        self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
-
-        self.m.nextpicture = self.m.currpicture.copy()
-        self.m.nextplotmask = self.m.plotmask.copy()
-        self.m.currpicture = self.m.prevpicture.copy()
-        self.m.plotmask = self.m.prevplotmask.copy()
-            
-        if self.Tindex == 1:
-            self.m.prevpicture = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
-            self.m.prevplotmask = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
-            self.button_previousframe.setEnabled(False)
-            
-        else:
-            self.m.prevpicture = self.reader.LoadOneImage(self.Tindex-2, self.FOVindex)
-            self.m.prevplotmask = self.reader.LoadMask(self.Tindex-2, self.FOVindex)
-
-        
-        if self.Tindex-1 == self.reader.sizet-2:
-            self.button_nextframe.setEnabled(True)            
-        
-        if self.button_hidemask.isChecked():
-            self.m.HideMask()
-        
-        self.Tindex -= 1
-        self.m.UpdatePlots()
-        self.UpdateTitleSubplots()
-            
-        self.Enable(self.button_previousframe)
-        
-        if self.Tindex > 0:
-            self.button_previousframe.setEnabled(True)          
-            
-        self.ClearStatusBar()
-        self.button_timeindex.setText(str(self.Tindex)+'/' + str(self.reader.sizet-1))
-
-
-# -----------------------------------------------------------------------------
-# MANUAL MASK CORRECTIONS
-            
-    def ChangeOneValue(self):
-        """This function is called when the button Change cell value is
-        clicked. It displays the instructions on the status bar.
-        And if the user clicks in the graph where the current mask is displayed
-        it connects the event of the click (meaning that user has clicked on
-        one cell) to the function self.DialogBoxChangeOneValue. 
-        This function will then replaces the cell selected by the user with
-        the click with a new value entered by the user.
-        """
-        
-        # displaying the instructions on the statusbar
-        self.WriteStatusBar((
-            'Left-click to select cell, right-click to abort.'))
-
-        # disables all the buttons
-        self.Disable(self.button_changecellvalue)
-        
-        # connects the event "press mouse button" in the matplotlib plot 
-        # (picture) to the function self.DialogBoxChangeOneValue
-        self.id = self.m.mpl_connect('button_press_event', self.DialogBoxChangeOneValue)
-        
-        
-    def DialogBoxChangeOneValue(self, event):
-        """This function is called when the user after the user has selected
-        the button Change cell value and clicked in the picture to select
-        the desired cell to change.
-        
-        It first deconnects the mouse click event in matplotlib with this 
-        function to not generate any other dialog window.
-        
-        It then tests if the click is inside the matplotlib plot (if it is
-        outside it equals to None) and if it is the current and editable plot
-        (the one in the middle of the gui, self.m.ax)
-        
-        If is true, then it sets the coordinates to int. and creates a dialog
-        window where the user is asked to type a value to set it to the cell.
-        
-        If the user presses ok, it tests if the entry is valid (>0 and not 
-        empty) and looks for the old cell value and replaces it. And then
-        it updates the plot such that the result of the change can be seen.
-        """
-        # the function is disconnected from the matplotlib event.
-        self.m.mpl_disconnect(self.id)
-        
-        # test if the button is a left click and if the coordinates
-        # chosen by the user click is inside of the current matplotlib plot
-        # which is given by self.m.ax
-        if (event.button == 1 
-            and (event.xdata != None and event.ydata != None) 
-            and self.m.ax == event.inaxes):
-            newx = int(event.xdata)
-            newy = int(event.ydata)
-            
-            # creates a dialog window
-            dlg = cocv.CustomDialog(self)
-            
-            #if the user presses 'ok' in the dialog window it executes the code
-            #else it does nothing
-            result = dlg.exec()
-            if result == QDialog.DialogCode.Accepted:
-                #it tests that the user has entered some value, that it is not
-                #empty and that it is equal or bigger to 0.
-                if dlg.entry1.text() != '' and int(dlg.entry1.text()) >= 0:
-                    #reads the new value to set and converts it from str to int
-                    value = int(dlg.entry1.text())
-                    
-                    # gives the coordinates where it is equal to the value
-                    # selected by the user. And it replaces it with the new
-                    # value.
-                    self.m.plotmask[self.m.plotmask == self.m.plotmask[newy,newx]] = value
-                    
-                    # updates the plot to see the modification.
-                    self.m.updatedata()
-                    
-        self.Enable(self.button_changecellvalue)
-        self.button_changecellvalue.setChecked(False)
-        self.m.ShowCellNumbers(type='current')
-        self.SaveMask()
-        self.ClearStatusBar()
-        
-        
-    def DialogBoxECV(self, s):
-        """This functions creates from the ExchangeCellValues.py file a 
-        window which takes two integer entries and then swaps the cells having
-        the given integer values.
-        """
-        # creates a dialog window from the ExchangeCellValues.py file
-        dlg = ecv.CustomDialog(self)
-        
-        # if the user presses 'ok', it executes the code
-        result = dlg.exec()
-        if result == QDialog.DialogCode.Accepted:
-            # it tests if both value to be swapped are not empty.
-            if dlg.entry1.text()!= '' and dlg.entry2.text() != '':
-                
-                # reads out the values and converts it into integers.
-                value1 = int(dlg.entry1.text())
-                value2 = int(dlg.entry2.text())
-                
-                # calls the function which does the swap
-                try:
-                    self.m.ExchangeCellValue(value1,value2)
-                except ValueError as e:
-                    msg_box = QMessageBox(QMessageBox.Icon.Critical, 'Error', str(e), parent=self)
-                    msg_box.exec()
-                self.m.ShowCellNumbers(type='current')
-                self.SaveMask()
-        else:
-            return
-
-
-    def MouseDraw(self):
-        """
-        This function is called whenever the brush or the eraser button is
-        pressed. On the first press event it calls the self.m.OneClick, which
-        tests whether it is a right click or a left click. If it a right click
-        it assigns the value of the pixel which has been right clicked
-        to self.cellval, meaning that the next drawn pixels will be set to this
-        value.
-        If it is left clicked, then it draws a 3x3 square with the current
-        value of self.cellval.
-        If after left clicking you drag the mouse, then you start drawing 
-        using the mouse and it stops once you release the left click.
-        
-        Same for the eraser button, it sets directly the value of self.cellval
-        to 0.
-        """
-        do_draw = self.button_drawmouse.isChecked()
-        do_erase = self.button_eraser.isChecked()
-        
-        if do_draw or do_erase:
-            self.m.tempmask = self.m.plotmask.copy()
-            
-            #save status of the showval check box, then turn off (slows brush/eraser down too much)
-            self.showval_was_checked = self.button_showval.isChecked()
-            self.button_showval.setChecked(False)
-            
-            if do_draw:
-                self.WriteStatusBar(('Draw using the brush, right click to select '
-                                     'the cell to draw.'))
-                self.Disable(self.button_drawmouse)
-                
-            elif do_erase:
-                self.WriteStatusBar('Erasing by setting the values to 0.')
-                self.Disable(self.button_eraser)
-                self.m.cellval = 0
-                
-            radius = self.spinbox_brushsize.value()
-            self.id2 = self.m.mpl_connect('button_press_event', 
-                                          lambda e: self.m.OneClick(e, radius))
-            self.id = self.m.mpl_connect('motion_notify_event', 
-                                          lambda e: self.m.PaintBrush(e, radius))
-            self.id3 = self.m.mpl_connect('button_release_event', self.m.ReleaseClick)
-                
-                        
-        else:
-            self.m.mpl_disconnect(self.id3)
-            self.m.mpl_disconnect(self.id2)
-            self.m.mpl_disconnect(self.id)
-            QApplication.restoreOverrideCursor()
-            self.Enable(self.button_drawmouse)
-            self.Enable(self.button_eraser)
-            self.button_showval.setChecked(self.showval_was_checked)
-            self.SaveMask()
-            self.ClearStatusBar()
-            
-            
-    
-    def SelectSplitCell(self):
-        """Function called upon clicking Split Cell button"""
-      
-        if self.button_split.isChecked():
-            self.cell_to_split=-1
-            self.Disable(self.button_split)
-            self.WriteStatusBar('First, select the cell to be split with a left click. '
-                                'Then, left-click the corners of a polygon to be split off from the '
-                                'selected cell. Right click to confirm.')
-            
-            def sel_cell(e):
-                if e.button != 1:
-                    self.cell_to_split=-1
-                    self.Enable(self.button_split)
-                else:
-                    x = int(e.xdata)
-                    y = int(e.ydata)
-                    self.cell_to_split = self.m.plotmask[y,x]
-                    self.m.mpl_disconnect(self.id)
-                    self.ClickSplitCell()
-    
-            self.id = self.m.mpl_connect('button_press_event', sel_cell)
-            
-        else:
-            self.DoSplitCell()
-
-
-    def ClickSplitCell(self):
-        self.WriteStatusBar('Click to define the corners of a polygon which'
-                            'will be split off the selected cell. Right click '
-                            'or reclick the button to confirm.')
-        if self.cell_to_split == -1:
-            return
-        
-        self.m.tempmask = self.m.plotmask.copy()
-        self.m.storemouseclicks = [] 
-        self.id = self.m.mpl_connect('button_press_event', 
-                                     lambda e: self.m.multiple_click(e, self.DoSplitCell))
-
-        
-    def DoSplitCell(self):
-        self.m.mpl_disconnect(self.id)
-        if len(self.m.storemouseclicks) > 2:
-            nx, ny = self.m.plotmask.shape
-            img = Image.new('L', (ny, nx), 0)
-            ImageDraw.Draw(img).polygon(self.m.storemouseclicks, outline=1, fill=1)
-            polygon = np.array(img).astype(bool)
-            selected_mask = self.m.plotmask==self.cell_to_split
-            replace_cell = self.m.plotmask.max() + 1
-            self.m.plotmask[selected_mask & polygon] = replace_cell
-        self.Enable(self.button_split)
-        self.m.UpdatePlots(type='current')
-        self.ClearStatusBar()
-        self.SaveMask()
-        self.m.storemouseclicks = []
-        self.button_split.setChecked(False)
-        
-        
-    def UpdateTitleSubplots(self):
-        """This function updates the title of the plots according to the 
-        current time index. So it called whenever a frame or a fov is changed.
-        """
-        if self.Tindex == 0:
-            self.m.titlecurr.set_text('Time index {}'.format(self.Tindex))
-            self.m.titleprev.set_text('No frame {}'.format(''))
-            self.m.titlenext.set_text('Next time index {}'.format(self.Tindex+1))
-            self.m.draw()
-            
-        elif self.Tindex == self.reader.sizet-1:
-            self.m.titlecurr.set_text('Time index {}'.format(self.Tindex))
-            self.m.titleprev.set_text('Previous time index {}'.format(self.Tindex-1))
-            self.m.titlenext.set_text('No frame {}'.format(''))            
-            self.m.draw()
-            
-        else:
-            self.m.titlecurr.set_text('Time index {}'.format(self.Tindex))
-            self.m.titleprev.set_text('Previous time index {}'.format(self.Tindex-1))
-            self.m.titlenext.set_text('Next time index {}'.format(self.Tindex+1))
-            self.m.draw()
-        
-        
-    def ClickNewCell(self):
-        """ 
-        this method is called when the button New Cell is clicked. If the button
-        state corresponds to True (if is activated) then it connects the mouse 
-        clicks on the pyqt window to the canvas (so to the matplolib figure).
-        The connection has an "id" which is given by the integer self.id
-        After the connections is made, it calls the Disable function with argument 0
-        which turns off the other button(s).
-        
-        If the button is clicked but it is deactivated then it disconnects the 
-        connection between the canvas and the window (the user can not interact
-        with the plot anymore). 
-        Storemouseclicks is a list corresponding to the coordinates of all mouse
-        clicks between the activation and the deactivation of the button.
-        So if it is empty, it does not draw anything because no clicks
-        were registered. 
-        But if it has some coordinates, it will draw a polygon where the vertices
-        are the coordinates of all the mouseclicks.
-        Once the figure has been updated with a new polygon, the other button(s)
-        are again enabled. 
-        
-        """
-        if self.button_newcell.isChecked():
-            self.WriteStatusBar(('Draw a new cell. Use the left click to '
-                                 'produce a polygon with a new cell value. '
-                                 'Click the button again to confirm.'))
-            self.m.tempmask = self.m.plotmask.copy()
-            self.id = self.m.mpl_connect('button_press_event', self.m.MouseClick)
-            self.Disable(self.button_newcell)
-            
-        else:
-            self.m.mpl_disconnect(self.id)
-            if  self.m.storemouseclicks and self.TestSelectedPoints():
-                self.m.DrawRegion(True)
-            else:
-                self.m.updatedata()
-            self.Enable(self.button_newcell)
-            self.m.ShowCellNumbers(type='current')
-            self.ClearStatusBar()
-            self.SaveMask()
-            
-            
-    def TestSelectedPoints(self):
-        """This function is just used to catch an exception, when the new cell
-        or the add region function is called. If all the dots drawn by the user
-        are located on one line (horizontal or vertical) the DrawRegion 
-        function calls a method to create a polygon and 
-        it can not make a polygon out of straight line so it gives an error.
-        In order to prevent this error, this function avoids to attempt to draw
-        by returning False if the square are all on one line.
-        """
-                
-        allx = list(np.array(self.m.storemouseclicks)[:,0])
-        ally = list(np.array(self.m.storemouseclicks)[:,1])
-        
-        resultx = all(elem == allx[0] for elem in allx)
-        resulty = all(elem == ally[0] for elem in ally)
-        
-        if resultx or resulty:
-            return False
-        else:
-            return True
-                    
-        
-    def clickmethod(self):
-        """ 
-        this method is called when the button Add region is clicked. If the button
-        state corresponds to True (if is activated) then it connects the mouse 
-        clicks on the pyqt window to the canvas (so to the matplolib figure).
-        The connection has an "id" which is given by the integer self.id
-        After the connections is made, it calls the Disable function with argument 1
-        which turns off the other button(s).
-        
-        If the button is clicked and it is deactivated then it disconnects the 
-        connection between the canvas and the window (the user can not interact
-        with the plot anymore). 
-        Storemouseclicks is a list corresponding to the coordinates of all mouse
-        clicks between the activation and the deactivation of the button.
-        So if it is empty, it does not draw anything because no clicks
-        were registered. 
-        But if it has some coordinates, it will draw a polygon where the vertices
-        are the coordinates of all the mouseclicks.
-        Once the figure has been updated with a new polygon, the other button(s)
-        are again enabled. 
-        
-        """
-        if self.button_add_region.isChecked():
-            self.WriteStatusBar(('Select the cell with the first click, '
-                                 'then draw polygon with subsequent '
-                                 'clicks. Reclick the button to confirm.'))
-            self.m.tempmask = self.m.plotmask.copy()
-            self.id = self.m.mpl_connect('button_press_event', self.m.MouseClick)           
-            self.Disable(self.button_add_region) 
-            
-        else:
-            self.m.mpl_disconnect(self.id)
-            
-            # test if the list is not empty and if the dots are not all in the same line
-            if self.m.storemouseclicks and self.TestSelectedPoints():
-                self.m.DrawRegion(False)
-
-            else:
-                self.m.updatedata()
-                
-            self.Enable(self.button_add_region)
-            self.m.ShowCellNumbers(type='current')
-            self.ClearStatusBar()
-            self.SaveMask()
-            
-            
-    def MergeWithNeighbors(self):
-        """This function is called when the button Merge With Neighbors is
-        clicked. It displays the instructions on the status bar.
-        And if the user clicks in the graph where the current mask is displayed
-        it connects the event of the click (meaning that user has clicked on
-        one cell) to the function self.PerformMergeWithNeighbors. 
-        This function will then merge the cell selected by the user with
-        the click with all (touching) neighbors.
-        """
-        
-        # displaying the instructions on the statusbar
-        self.WriteStatusBar((
-            'Left-click to select cell, right-click to abort.'))
-
-        # disables all the buttons
-        self.Disable(self.button_mergewithneighbors)
-        
-        # connects the event "press mouse button" in the matplotlib plot 
-        # (picture) to the function self.PerformMergeWithNeighbors
-        self.id = self.m.mpl_connect('button_press_event', self.PerformMergeWithNeighbors)
-        
-        
-    def PerformMergeWithNeighbors(self, event):
-        """This function is called after the user has selected
-        the button Merge With Neighbors and clicked in the picture to select
-        the desired cell to start the merger.
-        
-        It first deconnects the mouse click event in matplotlib with this 
-        function to not generate any other dialog window.
-        
-        It then tests if the click is inside the matplotlib plot (if it is
-        outside it equals to None) and if it is the current and editable plot
-        (the one in the middle of the gui, self.m.ax)
-        
-        If is true, then it sets the coordinates to int. and creates a dialog
-        window where the user is asked to type a value to set it to the cell.
-        
-        If the user presses ok, it tests if the entry is valid (>0 and not 
-        empty) and looks for the old cell value and replaces it. And then
-        it updates the plot such that the result of the change can be seen.
-        """
-        # the function is disconnected from the matplotlib event.
-        self.m.mpl_disconnect(self.id)
-        
-        # test if the button is a left click and if the coordinates
-        # chosen by the user click is inside of the current matplotlib plot
-        # which is given by self.m.ax
-        if (event.button == 1 
-            and (event.xdata != None and event.ydata != None) 
-            and self.m.ax == event.inaxes):
-            newx = int(event.xdata)
-            newy = int(event.ydata)
-            # get the ID of the selected cell
-            selectedcell_ID = self.m.plotmask[newy,newx]
-            # binarize the existing mask and number ("label") each component
-            labeled_binarized_mask = skimage.measure.label(self.m.plotmask > 0)
-            # select the component pixels that corresponds to the selected point
-            flood_indices=(labeled_binarized_mask==labeled_binarized_mask[newy,newx])
-            # set the mask pixels that correspond to the component to the cell ID
-            self.m.plotmask[flood_indices] = selectedcell_ID
-                    
-            # updates the plot to see the modification.
-            self.m.updatedata()
-                    
-        self.Enable(self.button_mergewithneighbors)
-        self.button_mergewithneighbors.setChecked(False)
-        self.m.ShowCellNumbers(type='current')
-        self.SaveMask()
-        self.ClearStatusBar()
-        
-        
-# -----------------------------------------------------------------------------
-# BUTTON ENABLE / DISABLE
-    
-    def Enable(self, button):
-        """
-        this functions turns on buttons all the buttons, depending on the time
-        index. (next and previous buttons should not be turned on if t = 0 
-        or t = lasttimeindex)
-        """
-        for k in range(0, len(self.buttonlist)):
-            if button != self.buttonlist[k]:
-                self.buttonlist[k].setEnabled(True)
-                
-        if self.Tindex == 0:
-            self.button_previousframe.setEnabled(False)
-            
-        if self.Tindex == self.reader.sizet-1:
-            self.button_nextframe.setEnabled(False)
-            
-        self.EnableCNNButtons()
-         
-     
-    def Disable(self, button):
-        """
-        this functions turns off all the buttons except the one given in 
-        argument.
-        """
-
-        for k in range(0,len(self.buttonlist)):
-            if button != self.buttonlist[k]:
-                self.buttonlist[k].setEnabled(False)
-
-
-    def EnableCNNButtons(self):
-        if self.reader.TestTimeExist(self.Tindex, self.FOVindex):
-            self.button_cellcorrespondence.setEnabled(True)
-            self.button_extractfluorescence.setEnabled(True)
-        else:
-            self.button_cellcorrespondence.setEnabled(False)
-            self.button_extractfluorescence.setEnabled(False)
-    
-    
-    def EnableCorrectionsButtons(self):
-        self.button_newcell.setEnabled(True)
-        self.button_add_region.setEnabled(True)
-        self.button_drawmouse.setEnabled(True)
-        self.button_eraser.setEnabled(True)
-        self.button_exval.setEnabled(True)
-        self.button_changecellvalue.setEnabled(True)
-        self.button_showval.setEnabled(True)
-        self.button_split.setEnabled(True)
-        
-        
-    def DisableCorrectionsButtons(self):
-        self.button_newcell.setEnabled(False)
-        self.button_add_region.setEnabled(False)
-        self.button_drawmouse.setEnabled(False)
-        self.button_eraser.setEnabled(False)
-        self.button_exval.setEnabled(False)
-        self.button_changecellvalue.setEnabled(False)
-        self.button_showval.setEnabled(False)
-        self.button_split.setEnabled(False)
-        
-    
-    def SaveMask(self):
-        """
-        When this function is called, it saves the current mask
-        (self.m.plotmask)
-        """
-        self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
-        
-        
-    def WriteStatusBar(self, text):
-        """Writes text to status bar"""
-        self.statusBarText.setText(text)
-        
-        
-    def ClearStatusBar(self):
-        """Removes text from status bar"""
-        self.statusBarText.setText('')
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+This script is the main script used to produce a GUI which should help for
+cell segmentation. This script can only read .nd2 files containing the 
+images of cells, especially it displays for each recorded positions (field
+of view) the pictures in the time axis.
+
+The script opens first a window which allows you to load an nd2 file and
+to load or create an hdf file. The hdf file contains all the masks, so if
+it is the first the user segments an nd2 file, a new one should be created.
+And it can be then loaded for later use.  Along with new hdf file, created
+by the name entered by the user (say filename), it creates three other hdf 
+files (filename_predicted.h5, filename_thresholded.h5 and 
+filename_segmented.h5) these contain all the steps of the NN to get to the 
+segmented picture. 
+
+After the first window is finished a second one opens, where at each time 
+index, three pictures 
+are displayed the t-1 picture, the t picture (current frame which can be
+edited) and the t+1 picture. Using the arrows one can navigate through time.
+On top of the picture, there is always a mask which is displayed, if no cells
+are present in the mask then the mask is blank and the user does not see it. 
+If one wants to hand anmotate the pictures, one can just start to draw on the
+picture using the different functions (New Cell, Add Region, Brush, Eraser,
+Save Mask, ...) and the informations will be saved in the mask overlayed on 
+top of the pictures. 
+
+If one wants to segment using a neural network, one can press the
+corresponding button (Launch CNN) and select the time range and 
+the field of views on which the neural network is applied.
+
+Once the neural network has finished predicting, there are still no visible
+masks, but on the field of views and time indices where the NN has been
+applied, the threshold and segment buttons are enabled. By checking these
+two buttons one can either display the thresholded image of the prediction or
+display the segmentation of the thresholded prediction.
+
+At this stage, one can correct the segmentation of the prediction using
+the functions (New Cell, Add Region, etc..) by selecting the Segment
+checkbox and then save them using the Save Seg button.
+If the user is happy with the segmentation, the Cell Correspondence button 
+can be clicked. Until then, the cells get random numbers attributed by
+the segmentation algorithm. In order to keep track of the cell through time,
+the same cells should have the same number between two different time pictures.
+This can be (with some errors) achieved by the Cell Correspondence button,
+which tries to attribute the same number to corresponding cells in time.
+After that, the final mask is saved and it is always visible when you go on
+the corresponding picture. This mask can also be corrected using the 
+usual buttons (because the Cell Correspondence makes also mistakes). 
+
+"""
+import sys
+import numpy as np
+import pandas as pd
+import h5py
+import skimage
+
+# For writing excel files
+#from openpyxl import load_workbook
+#from openpyxl import Workbook
+
+#Import from matplotlib to use it to display the pictures and masks.
+from matplotlib.backends.qt_compat import QtWidgets
+from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
+
+from sklearn.decomposition import PCA
+import imageio
+from PIL import Image, ImageDraw
+
+# tqdm for progress bar
+import tqdm
+import time
+
+# Import everything for the Graphical User Interface from the PyQt6 library.
+from PyQt6.QtWidgets import (QApplication, QMainWindow, QDialog, QSpinBox,
+    QMessageBox, QPushButton, QCheckBox, QStatusBar, QLabel)
+from PyQt6 import QtGui
+from PyQt6.QtGui import QAction
+from PyQt6.QtCore import Qt
+from PyQt6.QtGui import QPalette, QColor
+
+#Import all the other python files
+#this file handles the interaction with the disk, so loading/saving images
+#and masks and it also runs the neural network.
+from .disk import Reader as nd
+
+#this file contains a dialog window that takes two integers as entry to swap
+#two cell values
+from .misc import ExchangeCellValues as ecv
+
+#this file contains a window that opens to change the value of one cell. It 
+#is opened as soon as the user presses with the left click on a specific cell.
+from .misc import ChangeOneCellValue as cocv
+
+#this file contains a dialog window where a time range and the field of views
+#can be selected to then launch a prediction of the neural network on
+#a specific range of pictures.
+from .unet import LaunchBatchPrediction as lbp
+
+#this file contains a dialog window where a time range can be selected to retrack
+from .misc import BatchRetrack as br
+
+#this file initializes all the buttons present in the gui, sets the shortcuts
+#to these buttons and also connect the buttons to the function that are 
+#triggered when the buttons are pressed.
+from .init import InitButtons
+
+#this file contains the layout of the main window so it justs puts the buttons
+#and the pictures at the desired position in the main window.
+from .init import InitLayout
+
+# PlotCanvas for fast plotting
+from .misc.PlotCanvas import PlotCanvas
+
+from .misc import Extract as extr
+
+from .disk.image_loader import load_image
+from .unet.segment import segment
+from .unet import neural_network as nn
+from .misc.ProgressBar import ProgressBar
+
+import warnings
+# warnings.filterwarnings('ignore')
+
+import logging
+import os
+
+# Configure the root logger
+logging.basicConfig(
+    format='%(asctime)s %(levelname)s %(funcName)s: %(message)s',
+    level=os.environ.get("LOGLEVEL", "WARNING"),
+    filename='yeaz_GUI.log'
+)
+log = logging.getLogger(__name__)
+
+
+if getattr(sys, 'frozen', False):
+    path_icons = os.path.join(sys._MEIPASS, "icons/")
+    path_weights  = os.path.join(sys._MEIPASS, 'unet/')
+    
+else:
+    path_icons = './icons/'
+    path_weights = './unet/'
+
+
+class NavigationToolbar(NavigationToolbar):
+    """This is the standard matplotlib toolbar but only the buttons
+    that are of interest for this gui are loaded. These buttons allow 
+    to zoom into the pictures/masks and to navigate in the zoomed picture. 
+    A Home button can be used to set the view back to the original view.
+    """
+    toolitems = [t for t in NavigationToolbar.toolitems if
+                 t[0] in ('Home', 'Pan', 'Zoom','Back', 'Forward')]
+      
+class App(QMainWindow):
+    """This class creates the main window.
+    """
+
+    def __init__(self, nd2pathstr, hdfpathstr, newhdfstr):
+        super().__init__()
+        self.setWindowTitle('YeaZ')
+        log.info('initiating application')
+
+        # all these ids are integers which are used to set a connection between
+        # the button and the function that this button calls.
+        # There are three of them because it happens that one can trigger three 
+        # different functions with one button.        
+        self.id = 0
+        self.id2 = 0
+        self.id3 = 0 
+
+        self.reader = nd.Reader(hdfpathstr, newhdfstr, nd2pathstr)
+        
+        # these variables are used to create/read/load the excel file used
+        # to write the fluorescence values extracted. For each field of view,
+        # the user will be asked each time to create a new xls file for the 
+        # field of view or to load an existing field of view (this is the role
+        # of the boolean variable)
+        self.xlsfilename = ''
+        self.nd2path = nd2pathstr
+        
+        # Set the indices for the time axis and the field of view index. These
+        # indices represent everywhere the current picture (the one that can be
+        # edited, i.e. the time t frame)
+        self.Tindex = 0
+        self.FOVindex = 0
+        
+        # loading the first images of the cells from the nd2 file
+        self.currentframe = self.reader.LoadOneImage(self.Tindex,self.FOVindex)
+        
+        # check if the t+1 time frame exists, avoid failure if there is only
+        # one picture in the folder/nd2 file
+        if self.Tindex+1 < self.reader.sizet:
+            self.nextframe = self.reader.LoadOneImage(self.Tindex+1, self.FOVindex)
+        else:
+            self.nextframe = np.zeros([self.reader.sizey, self.reader.sizex])
+        
+        self.previousframe = np.zeros([self.reader.sizey, self.reader.sizex])
+
+        # loading the first masks from the hdf5 file
+        self.mask_curr = self.reader.LoadMask(self.Tindex, self.FOVindex)
+        self.mask_previous = np.zeros([self.reader.sizey, self.reader.sizex])
+        
+        # check if the t+1 mask exists, avoid failure if there is only
+        # one mask in the hdf file
+        if self.Tindex+1 < self.reader.sizet:
+            self.mask_next = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
+        else:
+            self.mask_next = np.zeros([self.reader.sizey, self.reader.sizex])
+        
+        # creates a list of all the buttons, which will then be used in order
+        # to disable all the other buttons at once when one button/function
+        # is pressed/used in the gui.
+        self.buttonlist = []
+        
+        # setting buttons as attributes
+        # the shortcuts for the buttons, the functions to which they are
+        # connected to,... are all set up in the ButtonInit file which is called
+        # in the self.initUI() method below.
+        self.button_newcell = QPushButton("New cell")
+        self.buttonlist.append(self.button_newcell)
+        
+        self.button_add_region = QPushButton("Add region")
+        self.buttonlist.append(self.button_add_region)
+        
+        self.button_drawmouse = QPushButton('Brush')
+        self.buttonlist.append(self.button_drawmouse)
+        
+        self.button_eraser = QPushButton('Eraser')
+        self.buttonlist.append(self.button_eraser)
+        
+        self.label_brushsize = QLabel('Brush/Eraser radius:')
+        self.spinbox_brushsize = QSpinBox()
+        self.buttonlist.append(self.spinbox_brushsize)
+        
+        self.button_exval = QPushButton('Exchange cell IDs')
+        self.buttonlist.append(self.button_exval)
+        
+        self.button_showval = QCheckBox('Show cell IDs')
+        self.buttonlist.append(self.button_showval)
+        
+        self.button_hidemask = QCheckBox('Hide mask')
+        self.buttonlist.append(self.button_hidemask)
+        
+        self.button_split = QPushButton('Split cell')
+        self.buttonlist.append(self.button_split)
+        
+        self.button_mergewithneighbors = QPushButton('Merge cells')
+        self.buttonlist.append(self.button_mergewithneighbors)
+        
+        self.button_nextframe = QPushButton("Next time frame")
+        self.buttonlist.append(self.button_nextframe)
+        
+        self.button_previousframe = QPushButton("Previous time frame")
+        self.buttonlist.append(self.button_previousframe)
+        
+        self.button_cnn = QPushButton('Launch CNN')
+        self.buttonlist.append(self.button_cnn)
+        
+        self.button_cellcorrespondence = QPushButton('Retrack')
+        self.buttonlist.append(self.button_cellcorrespondence)
+        
+        self.button_changecellvalue = QPushButton('Change cell ID')
+        self.buttonlist.append(self.button_changecellvalue)        
+        
+        self.button_extractfluorescence = QPushButton('Extract')
+        self.buttonlist.append(self.button_extractfluorescence)
+        
+        self.button_hide_show = QPushButton('CNN')
+        self.buttonlist.append(self.button_hide_show)
+        
+        self.initUI()
+
+
+    def initUI(self):
+        """Initializing the widgets contained in the window. 
+        Especially, it creates the widget to plot the 
+        pictures/masks by creating an object of the PlotCanvas class self.m. 
+        Every interaction with the masks or the pictures (loading new
+        frames/editing the frames/masks) occurs through this class.
+        
+        This method initializes all the buttons with the InitButtons file.
+        It connects the buttons to the functions that they should trigger,
+        it sets the shortcuts to the buttons, a tool tip, 
+        eventually a message on the status bar when the user hovers 
+        over the button, etc..
+        
+        This function also sets all the layout in the InitLayout file. It 
+        takes and places the widgets (buttons, canvas, toolbar).
+
+        The function initializes a Menu Bar to have a menu which can be 
+        improved later on.
+        It sets a toolbar of the matplotlib library and hides it. But it allows
+        to connect to the functions of this toolbar through "homemade" 
+        QPushButtons instead of the ones provided by matplotlib.
+        Finally, it sets a StatusBar which displays some text to describe
+        the use of some buttons, or to show that the program is working on 
+        something (running the neural network, loading frames, etc...)
+        
+        After all this has been initialized, the program is ready to be used.
+        """
+        log.info('initiate UI')
+        self._main = QtWidgets.QWidget()
+        self.setCentralWidget(self._main)
+
+        # Here our canvas is created where using matplotlib, 
+        # one can plot data to display the pictures and masks.
+        self.m = PlotCanvas(self)
+        
+        # Initialize all the buttons that are needed and the functions that are 
+        # connected when the buttons are triggered.
+        InitButtons.Init(self)
+        InitLayout.Init(self)
+        
+        # MENU, TOOLBAR AND STATUS BAR
+        # creates a menu just in case, some other functions can be added later
+        # in this menu.
+#        menubar = self.menuBar()
+#        self.fileMenu = menubar.addMenu('File')   
+#        self.saveactionmenu = QAction('Save')
+#        self.fileMenu.addAction(self.saveactionmenu)
+#        self.saveactionmenu.triggered.connect(self.SaveMask)
+        
+        # hide the toolbar and instead of the original buttons of matplotlib,
+        # QPushbuttons are used and are connected to the functions of the toolbar
+        # it is than easier to interact with these buttons (for example to 
+        # to disable them and so on..)
+        self.Nvgtlbar = NavigationToolbar(self.m, self)
+        self.addToolBar(self.Nvgtlbar)
+        self.Nvgtlbar.hide()
+        
+        # creates a status bar with user instructions
+        self.statusBar = QStatusBar()
+        self.setStatusBar(self.statusBar)
+        self.statusBarText = QLabel()
+        self.statusBar.addWidget(self.statusBarText)
+                
+        self.show()
+                
+        
+# -----------------------------------------------------------------------------
+# FUNCTIONS LINKED TO NAVIGATION
+# connect the functions of the toolbar to our custom QPushbuttons.
+    def ZoomTlbar(self):
+        """The button_zoom is connected to the zoom function of the toolbar 
+        already present in the matplotlib library.
+        
+        Depending on the buttons that are active or checked, when the zoom 
+        function is used, it does not disable all the buttons.
+        
+        If the segment and threshold button are not checked or used
+        when the zoom button is clicked, it disables all the button
+        using self.Disable which disables everything except the button passed
+        in argument (in this case button_zoom).
+        
+        If the zoom button is used while the segment button is checked,
+        it disables all the buttons (1st elif) except the segment button
+        but once it is finished (so the zoom button becomes unchecked) 
+        then it enables only the editing buttons (as long as the segment
+        button is still checked) such as New Cell, Add Region, Eraser, 
+        Brush,etc.. and the other toolbar buttons (3rd elif)
+        
+        
+        If the zoom button is clicked while the threshold button is checked,
+        it disables all the button except the threshold button (2nd elif).
+        Once the zoom button is unchecked, it enables the toolbar buttons
+        (4th elif)
+        In any other case, it just enables all the buttons again.
+        """
+        self.Nvgtlbar.zoom()
+        
+        if (self.button_zoom.isChecked()):
+            self.Disable(self.button_zoom)
+            
+        else:
+            self.Enable(self.button_zoom)
+        
+        
+    def HomeTlbar(self):
+        """
+        connects the home button to the home function of the matplotlib
+        toolbar. It sets the view to the original view (no zoom)
+        """
+        self.Nvgtlbar.home()
+
+            
+    def BackTlbar(self):
+        """
+        It calls the back function of the matplotlib toolbar which sets the 
+        view to the previous one (if the user does several zooms/pans, 
+        this button allows to go back in the "history of views")
+        """
+        self.Nvgtlbar.back()
+
+        
+    def ForwardTlbar(self):
+        """
+        It calls the forward function of the matplotlib toolbar which sets the 
+        view to the next one (if the user does several zooms/pans, 
+        this button allows to go forward in the "history of views"
+        """
+        self.Nvgtlbar.forward()
+
+    
+    def PanTlbar(self):
+        """The button_pan is connected to the pan function of the toolbar 
+        already present in the matplotlib library.
+        
+        Depending on the buttons that are active or checked, when the pan 
+        function is used, it does not disable all the buttons.
+        
+        If the segment and threshold button are not checked or used
+        when the pan button is clicked, it disables all the button
+        using self.Disable which disables everything except the button passed
+        in argument (in this case button_pan).
+        
+        If the pan button is used while the segment button is checked,
+        it disables all the buttons (1st elif) except the segment button
+        but once it is finished (so the zoom button becomes unchecked) 
+        then it enables only the editing buttons (as long as the segment
+        button is still checked) such as New Cell, Add Region, Eraser, 
+        Brush,etc.. and the other toolbar buttons (3rd elif)
+        
+        
+        If the pan button is clicked while the threshold button is checked,
+        it disables all the button except the threshold button (2nd elif).
+        Once the pan button is unchecked, it enables the toolbar buttons
+        (4th elif)
+        In any other case, it just enables all the buttons again.
+        """
+
+        self.Nvgtlbar.pan()
+
+        if (self.button_pan.isChecked()):
+            self.Disable(self.button_pan)
+        else:
+            self.Enable(self.button_pan)
+
+            
+    def ButtonFluo(self):
+        """This function is called everytime the Extract Fluorescence button is 
+        clicked (self.button_extractfluorescence). 
+        """        
+        self.Disable(self.button_extractfluorescence)
+        self.WriteStatusBar('Extracting ...')
+        
+        # Get last image with mask
+        for time_index in range(self.reader.sizet-1, -1, -1):            
+            # Test if time has a mask
+            file = h5py.File(self.reader.hdfpath, 'r+')
+            time_exist = self.reader.TestTimeExist(time_index, self.FOVindex, file)
+            file.close()
+            
+            if not time_exist:
+                continue
+            
+            # load picture and sheet
+            image = self.reader.LoadImageChannel(time_index, self.FOVindex, 
+                                                 self.reader.default_channel)
+            mask = self.reader.LoadMask(time_index, self.FOVindex)
+            
+            # Break if mask is non-empty
+            if mask.sum()>0:
+                break
+            
+            if time_index==0:
+                msg_box = QMessageBox(QMessageBox.Icon.Critical, 'Error', 'No mask found', parent=self)
+                msg_box.exec()
+                self.Enable(self.button_extractfluorescence)
+                self.ClearStatusBar()
+        
+        # Launch dialog with last image
+        dlg = extr.Extract(image, mask, self.reader.channel_names)
+        dlg.exec()
+        if dlg.exit_code == 1: # Fluorescence
+            self.ExtractFluo(dlg.cells, dlg.desel_cells, dlg.outfile, dlg.file_list)
+        elif dlg.exit_code == 2: # Mask
+            self.ExtractMask(dlg.desel_cells, dlg.outfile)
+            
+        self.Enable(self.button_extractfluorescence)
+        self.ClearStatusBar()
+
+
+    def ExtractMask(self, desel_cells, outfile):
+        """Extract the mask to the specified tiff file. Only take cells 
+        specified by the cell_list"""
+        
+        mask_list = []
+        for time_index in range(0, self.reader.sizet):
+            
+            # Test if time has a mask
+            file = h5py.File(self.reader.hdfpath, 'r+')
+            time_exist = self.reader.TestTimeExist(time_index, self.FOVindex, file)
+            file.close()
+            
+            if not time_exist:
+                continue
+            
+            mask = self.reader.LoadMask(time_index, self.FOVindex)
+            for cell in desel_cells:
+                mask[mask==cell] = 0
+            mask_list.append(mask)
+            
+        imageio.mimwrite(outfile, np.array(mask_list, dtype=np.uint16))
+                        
+
+    def ExtractFluo(self, sel_cells, desel_cells, csv_filename, channel_list):
+        """This is the function that takes as argument the filepath to the xls
+        file and writes in the file.
+        It iterates over the different channels (or the sheets of the file,
+        each channel has one sheet.), and reads the image corresponding
+        to the time, field of view and channel index. It reads the already
+        existing file and makes a copy in which the data will be written in it.
+        
+        The first step of calculating the data is to iterate through each
+        cell/segment of the mask (so each cell is a submatrix of one value
+        in the matrix of the mask).
+        For each of these value /cell, the area is extracted as being
+        the number of pixels corresponding to this cell/value. 
+        (it is known from the microscope settings how to convert
+        the pixel in area).
+        The total intensity is just the value of the pixel and it is added over
+        all the pixels corresonding to the cell/value.
+        The mean is then calculated as being the total intensity divided by
+        the number of pixels (which here is equal to the area also).
+        With the mean it is then possible to calculate the variance of the 
+        signal for one cell/value.
+        
+        Then, it is checked if the value of the cell (cell number) already
+        exists in the first column, if it already exists it continues to
+        find the column corresponding to the time index where the values
+        should be written. It sets the flag to True such that it does not
+        write the cell as new one and adds it at the end of the column
+        
+        If the value is not found in the cell number column (new cell or
+        first time writing in the file), the flag is False, thus it adds the 
+        cell number at the end of the column.
+        It then saves the xls file.
+        
+        """
+        # List of cell properties
+        cell_list = []
+
+        for time_index in range(0, self.reader.sizet):
+            # Test if time has a mask
+            file = h5py.File(self.reader.hdfpath, 'r+')
+            time_exist = self.reader.TestTimeExist(time_index, self.FOVindex, file)
+            file.close()
+            
+            if not time_exist:
+                continue
+            
+            mask = self.reader.LoadMask(time_index, self.FOVindex)
+            
+            for channel in channel_list:
+                # check if channel is in list of nd2 channels
+                try:
+                    channel_ix = self.reader.channel_names.index(channel)
+                    image = self.reader.LoadImageChannel(time_index, self.FOVindex, channel_ix)
+                
+                # channel is a file
+                except ValueError:
+                    image = load_image(channel, ix=time_index)
+                    
+                for val in np.unique(mask):
+                    # bg is not cell
+                    if val == 0:
+                        continue
+                    # disregard cells not in cell_list
+                    if (val in desel_cells):
+                        continue
+                    
+                    # Calculate stats
+                    stats = {'Cell': val,
+                             'Time': time_index,
+                             'Channel': channel}
+                    
+                    stats = {**stats,
+                             **self.cell_statistics(image, mask == val)}
+                    stats['Disappeared in video'] = not (val in sel_cells)
+                    cell_list.append(stats)
+                    
+        
+        # Use Pandas to write csv
+        df = pd.DataFrame(cell_list)
+        df = df.sort_values(['Cell', 'Time'])
+        df.to_csv(csv_filename, index=False)
+                    
+        self.Enable(self.button_extractfluorescence)
+        self.ClearStatusBar()
+
+
+    def cell_statistics(self, image, mask):
+        """Calculate statistics about cells. Passing None to image will
+        create dictionary to zeros, which allows to extract dictionary keys"""
+        if image is not None:
+            cell_vals = image[mask]
+            area = mask.sum()
+            tot_intensity = cell_vals.sum()
+            mean = tot_intensity/area if area > 0 else 0
+            var = np.var(cell_vals)
+            
+            # Center of mass
+            y,x = mask.nonzero()
+            com_x = np.mean(x)
+            com_y = np.mean(y)
+            
+            # PCA only works for multiple points
+            if area > 1:
+                pca = PCA().fit(np.array([x,y]).T)
+                pc1_x, pc1_y = pca.components_[0,:]
+                angle = np.arctan(pc1_y / pc1_x) / (2*np.pi) * 360
+                v1, v2 = pca.explained_variance_
+                
+                len_maj = 4*np.sqrt(v1)
+                len_min = 4*np.sqrt(v2)
+            else:
+                angle = 0
+                len_maj = 1
+                len_min = 1
+            
+        else:
+            mean = 0
+            var = np.nan
+            tot_intensity = 0
+            com_x = np.nan
+            com_y = np.nan
+            angle = np.nan
+            len_maj = np.nan
+            len_min = np.nan
+        
+        return {'Area': area,
+                'Mean': mean,
+                'Variance': var,
+                'Total Intensity': tot_intensity,
+                'Center of Mass X': com_x,
+                'Center of Mass Y': com_y,
+                'Angle of Major Axis': angle,
+                'Length Major Axis': len_maj,
+                'Length Minor Axis': len_min}
+
+# -----------------------------------------------------------------------------
+# NEURAL NETWORK
+    def ShowHideCNNbuttons(self):
+        """hide and show the buttons corresponding to the neural network.
+            this function is called by the button CNN which is hidden. But
+            if activated in the InitLayout.py then you can have a button
+            which hides the CNN buttons (which are now on the normal also
+            hidden...).
+        """
+        if self.button_hide_show.isChecked():
+            self.button_cnn.setVisible(True)
+
+        else:
+            self.button_cnn.setVisible(False)
+            
+
+    def LaunchBatchPrediction(self):
+        """This function is called whenever the button Launch CNN is pressed.
+        It allows to run the neural network over a time range and selected
+        field of views.
+            
+        It creates a dialog window with two entries, that define the time range
+        and a list where the user can select the desired fields of view.
+        
+        Once it reads all the value, it calls the neural network function
+        inside of self.PredThreshSeg and it does the prediction of the neural
+        network, thresholds this prediction and then segments it.
+        """
+        def reset():
+            self.m.UpdatePlots()
+            self.ClearStatusBar()
+            self.Enable(self.button_cnn)
+            self.EnableCNNButtons()
+        
+        
+        self.WriteStatusBar('Running the neural network...')
+        self.Disable(self.button_cnn)
+
+        # creates a dialog window from the LaunchBatchPrediction.py file
+        dlg = lbp.CustomDialog(self)
+        
+        # this if tests if the user pressed 'ok' in the dialog window
+        result = dlg.exec()
+        if result == QDialog.DialogCode.Accepted:
+            # it tests if the user has entered some values
+            # if not it ignores and returns.
+            if not (dlg.entry1.text()!= '' and dlg.entry2.text() != ''):
+                msg_box = QMessageBox(QMessageBox.Icon.Critical, 'Error', "No Time Specified", parent=self)
+                msg_box.exec()
+                reset()
+                return 
+            
+            # reads out the entry given by the user and converts the index
+            # to integers
+            time_value1 = int(dlg.entry1.text())
+            time_value2 = int(dlg.entry2.text())
+    
+            # it tests if the first value is smaller or equal such that
+            # time_value1 is the lower range of the time range
+            # and time_value2 the upper boundary of the range.
+            if time_value1 > time_value2 :
+                msg_box = QMessageBox(QMessageBox.Icon.Critical, 'Error', 'Invalid Time Constraints', parent=self)
+                msg_box.exec()
+                reset()
+                return
+            
+            # displays that the neural network is running
+            self.WriteStatusBar('Running the neural network...')
+    
+            #it iterates in the list of the user-selected fields 
+            #of view, to return the corresponding index, the function
+            #dlg.listfov.row(item) is used which gives an integer
+            if len(dlg.listfov.selectedItems())==0:
+                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", "No FOV Selected", parent=self)
+                msg_box.exec()
+            # Check if the user have selected a mic type
+            
+            mic_type = dlg.mic_type.currentData()
+            if dlg.mic_type.currentData() is not None:
+                # User has selected an option, do something with it
+                log.debug(msg='Mic type selected: {}'.format(mic_type))
+            else:
+                # User has not selected any option, show error message
+                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", "No Image Type Selected", parent=self)
+                msg_box.exec()
+                reset()
+                return 
+            
+            # decide between cuda or cpu for running neural network
+            device = None
+            import torch
+            if (dlg.device_selection.currentData() == 'cuda') and (torch.cuda.is_available()):
+                device = 'cuda'
+            else:
+                device = 'cpu'
+            
+            for item in tqdm.tqdm(dlg.listfov.selectedItems(), desc='FOV', position=0, leave=True):
+                #iterates over the time indices in the range
+                for t in tqdm.tqdm(range(time_value1, time_value2+1), desc='Time', position=1, leave=False):                    
+                    #calls the neural network for time t and selected
+                    #fov
+                    if dlg.entry_threshold.text() !=  '':
+                        thr_val = float(dlg.entry_threshold.text())
+                    else:
+                        thr_val = None
+                    if dlg.entry_segmentation.text() != '':
+                        seg_val = int(dlg.entry_segmentation.text())
+                    else:
+                        seg_val = 10
+                    
+                    self.PredThreshSeg(t, dlg.listfov.row(item), thr_val, seg_val,
+                                       mic_type, device=device)
+                    
+                    # apply tracker if wanted and if not at first time
+                    temp_mask = self.reader.CellCorrespondence(t, dlg.listfov.row(item))
+                    self.reader.SaveMask(t,dlg.listfov.row(item), temp_mask)
+            
+            self.ReloadThreeMasks()
+        reset()
+
+    
+    def PredThreshSeg(self, timeindex, fovindex, thr_val, seg_val, 
+                      mic_type, device=None):
+        """
+        This function is called in the LaunchBatchPrediction function.
+        This function calls the neural network function in the
+        InteractionDisk.py file and then thresholds the result
+        of the prediction, saves this thresholded prediction.
+        Then it segments the thresholded prediction and saves the
+        segmentation. 
+        """
+        log.debug('--------- Segmenting field of view:',fovindex,'Time point:',timeindex)
+        im = self.reader.LoadOneImage(timeindex, fovindex)
+        try:
+            pred = self.LaunchPrediction(im, mic_type, device=device)
+        except ValueError:
+            msg_box = QMessageBox(QMessageBox.Icon.Critical,'Error',
+                                 'The neural network weight files could not '
+                                 'be found. Make sure to download them from '
+                                 'the link in the readme and put them into '
+                                 'the folder unet', parent=self)
+            msg_box.exec()
+            
+            return
+
+        thresh = self.ThresholdPred(thr_val, pred)
+        seg = segment(thresh, pred, seg_val)
+        self.reader.SaveMask(timeindex, fovindex, seg)
+        log.debug('--------- Finished segmenting.')
+          
+          
+    @staticmethod
+    def LaunchPrediction(im, mic_type, pretrained_weights=None, device=None):
+        """It launches the neural neutwork on the current image and creates 
+        an hdf file with the prediction for the time T and corresponding FOV. 
+        """
+        im = skimage.exposure.equalize_adapthist(im)
+        im = im*1.0;	
+        pred = nn.prediction(im, mic_type, pretrained_weights, device=device)
+        return pred
+
+
+    @staticmethod
+    def ThresholdPred(thvalue, pred):
+        """Thresholds prediction with value"""
+        if thvalue == None:
+            thresholdedmask = nn.threshold(pred)
+        else:
+            thresholdedmask = nn.threshold(pred, thvalue)
+        return thresholdedmask
+
+    
+    def SelectChannel(self, index):
+        """This function is called when the button to select different channels
+        is used. From the displayed list in the button, the chosen index
+        corresponnds to the same index in the list of channels from the reader.
+        So, it sets the default channel with the new index (called index below)
+        """
+        self.reader.default_channel = index
+        # update the pictures using the same function as the one used to 
+        # change the fields of view.
+        self.ChangeFOV()
+        
+
+    def SelectFov(self, index):
+        """This function is called when the button containing the list of 
+        fields od view is used.
+        The index correspondds to the field of view selected in the list.
+        """
+        # mask is automatically saved.
+        self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
+        self.FOVindex = index    
+        
+        # it updates the fov in the plot with the new index.
+        self.ChangeFOV()
+                
+        
+    def ChangeFOV(self):
+        """
+        it changes the fov or channel according to the choice of the user
+        and it updates the plot shown and it initializes the new fov/channel
+        at t=0 by default.
+        """
+        
+        self.Tindex = 0
+        
+        # load the image and mask for the current plot
+        self.m.currpicture = self.reader.LoadOneImage(self.Tindex,self.FOVindex)
+        self.m.plotmask = self.reader.LoadMask(self.Tindex,self.FOVindex)
+        
+        # sets the image and the mask to 0 for the previous plot
+        self.m.prevpicture = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
+        self.m.prevplotmask = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
+        
+        # load the image and the mask for the next plot, check if it exists
+        if self.Tindex+1 < self.reader.sizet:
+            self.m.nextpicture = self.reader.LoadOneImage(self.Tindex+1, self.FOVindex)
+            self.m.nextplotmask = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
+            
+            # enables the next frame button in case it was disabled when the 
+            # fov/channel was changed
+            self.button_nextframe.setEnabled(True)
+        else:
+            self.m.nextpicture = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
+            self.m.nextplotmask =  np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
+            
+            # disables the next frame button if the mask or the picture
+            # does not exist.
+            self.button_nextframe.setEnabled(False)
+            
+        # once the images and masks are loaded into the variables, they are 
+        # displaye in the gui.
+        self.m.UpdatePlots()
+        
+        # disables the previous frame button in case it was active before 
+        # changing fov/channel.
+        self.button_previousframe.setEnabled(False)
+        
+        # updates the title of the plots to display the right time indices
+        # aboves the plots.
+        self.UpdateTitleSubplots()
+            
+        # if the button to hide the mask was checked before changing fov/channel,
+        # it hides the mask again.
+        if self.button_hidemask.isChecked():
+            self.m.HideMask()
+        
+        # the button to set the time index is also set to 0/default again.
+        self.button_timeindex.setText('')
+        # enables the neural network buttons if there is already an 
+        # existing prediction for the current image.
+        self.EnableCNNButtons()
+        
+        
+    def ReloadThreeMasks(self):
+        """
+        A function which replots all the masks at the current time and fov 
+        indices. Needed after the batch prediction is completed to display
+        the result of the NN.
+        """
+        log.debug("reload three mask for frame {}".format(self.Tindex))
+        
+        if self.Tindex >= 0 and self.Tindex <= self.reader.sizet-1:
+            if self.Tindex == 0:
+                self.button_nextframe.setEnabled(True)
+                
+                if self.Tindex < self.reader.sizet-1:
+                    self.m.nextplotmask = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
+                else:
+                    np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
+                
+                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)
+                self.m.prevplotmask = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
+                self.m.UpdatePlots()
+                self.button_previousframe.setEnabled(False)
+                
+                
+            elif self.Tindex == self.reader.sizet-1:
+                self.button_previousframe.setEnabled(True)
+                self.m.prevplotmask = self.reader.LoadMask(self.Tindex-1, self.FOVindex)
+                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)
+                self.m.nextplotmask =  np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
+                self.m.UpdatePlots()
+                self.button_nextframe.setEnabled(False)
+                
+            else:
+                self.button_nextframe.setEnabled(True)
+                self.button_previousframe.setEnabled(True)
+                self.m.prevplotmask = self.reader.LoadMask(self.Tindex-1, self.FOVindex)
+                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)              
+                self.m.nextplotmask = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
+                self.m.UpdatePlots()
+            
+            self.UpdateTitleSubplots()
+                        
+            if self.button_hidemask.isChecked():
+                self.m.HideMask()
+            self.EnableCNNButtons()
+        
+        else:
+            return
+        
+    
+    def ChangeTimeFrame(self):
+        """This funcion is called whenever the user gives a new time index, 
+        to jump to the new given index, once "enter" button is pressed.
+        """
+        
+        # it reads out the text in the button and converts it to an int.
+        newtimeindex = int(self.button_timeindex.text())
+        if newtimeindex >= 0 and newtimeindex <= self.reader.sizet-1:
+            self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
+            
+            self.Tindex = newtimeindex
+            
+            if self.Tindex == 0:
+                self.button_nextframe.setEnabled(True)
+                self.m.nextpicture = self.reader.LoadOneImage(self.Tindex+1,self.FOVindex)
+                self.m.nextplotmask = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
+                
+                self.m.currpicture = self.reader.LoadOneImage(self.Tindex, self.FOVindex)
+                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)
+                
+                self.m.prevpicture = np.zeros([self.reader.sizey, self.reader.sizex], 
+                                              dtype = np.uint16)
+                self.m.prevplotmask = np.zeros([self.reader.sizey, self.reader.sizex], 
+                                               dtype = np.uint16)
+    
+                self.m.UpdatePlots()
+                self.button_previousframe.setEnabled(False)
+                
+            elif self.Tindex == self.reader.sizet-1:
+                self.button_previousframe.setEnabled(True)
+                self.m.prevpicture = self.reader.LoadOneImage(self.Tindex-1, self.FOVindex)
+                self.m.prevplotmask = self.reader.LoadMask(self.Tindex-1, self.FOVindex)
+                   
+                self.m.currpicture = self.reader.LoadOneImage(self.Tindex, self.FOVindex)
+                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)
+                  
+                self.m.nextpicture =  np.zeros([self.reader.sizey, self.reader.sizex], 
+                                               dtype = np.uint16)
+                self.m.nextplotmask =  np.zeros([self.reader.sizey, self.reader.sizex], 
+                                                dtype = np.uint16)
+                
+                self.m.UpdatePlots()
+                self.button_nextframe.setEnabled(False)
+                
+            else:
+                self.button_nextframe.setEnabled(True)
+                self.button_previousframe.setEnabled(True)
+                self.m.prevpicture = self.reader.LoadOneImage(self.Tindex-1, self.FOVindex)
+                self.m.prevplotmask = self.reader.LoadMask(self.Tindex-1, self.FOVindex)
+                   
+                self.m.currpicture = self.reader.LoadOneImage(self.Tindex, self.FOVindex)
+                self.m.plotmask = self.reader.LoadMask(self.Tindex, self.FOVindex)              
+                  
+                self.m.nextpicture = self.reader.LoadOneImage(self.Tindex+1,self.FOVindex)
+                self.m.nextplotmask = self.reader.LoadMask(self.Tindex+1, self.FOVindex)
+                self.m.UpdatePlots()
+            
+            self.UpdateTitleSubplots()
+            self.button_timeindex.clearFocus()
+            self.button_timeindex.setText(str(self.Tindex)+'/'+str(self.reader.sizet-1))
+            
+            if self.button_hidemask.isChecked():
+                self.m.HideMask()
+            self.EnableCNNButtons()
+        
+        else:
+            self.button_timeindex.clearFocus()
+            return
+        
+    def BatchCellCorresp(self):
+        def reset():
+            self.ClearStatusBar()
+            self.Enable(self.button_cellcorrespondence)
+            self.button_cellcorrespondence.setChecked(False)
+        
+        self.Disable(self.button_cellcorrespondence)
+        self.WriteStatusBar('retracking... ')
+
+        if(self.Tindex==self.reader.sizet-1):
+            msg_box = QMessageBox(QMessageBox.Icon.Critical, 'Error',"This is the last frame. Nothing to retrack after this", parent=self)
+            msg_box.exec()
+            reset()
+            return 
+
+
+        # creates a dialog window from the BatchRetrack.py file
+        dlg = br.CustomDialog(self)
+        
+        # this if tests if the user pressed 'ok' in the dialog window
+        result = dlg.exec()
+        if result == QDialog.DialogCode.Accepted:
+            # it tests if the user has entered some values
+            if not (dlg.entry1.text()!= ''):
+                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", "No Time Specified", parent=self)
+                msg_box.exec()
+                reset()
+                return 
+            
+            # reads out the entry given by the user and converts the index
+            # to integers
+            time_value1 = int(dlg.entry1.text())
+    
+            # it tests if the value is bigger than current frame
+            if (time_value1 <  self.Tindex or time_value1 > self.reader.sizet-1):
+                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", 'Invalid Time Constraints', parent=self)
+                msg_box.exec()
+                reset()
+                return
+            # if everything was okay, start a progress bar to show progress:
+            progress = ProgressBar(self)
+            progress_value = 0
+            ratio = 100/(time_value1 - self.Tindex)
+            for t in range(self.Tindex+1, time_value1+1):
+                log.debug('start correspondance for frame {}'.format(t))                    
+                #calls the cell correspondance for current time, t, and t+1
+                temp_mask = self.reader.CellCorrespondence(t, self.FOVindex)
+                progress_value += ratio
+                progress.update_progress(progress_value)
+                # update the progress status label
+                progress.status.setText("Processing frame {}... ".format(t+1))
+                self.reader.SaveMask(t, self.FOVindex, temp_mask)
+                QApplication.processEvents()  # Process events to allow GUI to update               
+                log.debug('finish correspondance and savemask for frame {}'.format(t))                    
+            # close the progress bar dialog
+            progress.close()
+            self.ReloadThreeMasks()
+
+            log.info('reload three frames')
+        reset()
+
+    def CellCorrespActivation(self):
+        log.debug('An outdated function is called')
+        self.Disable(self.button_cellcorrespondence)
+        self.WriteStatusBar('Doing the cell correspondence')
+        if self.Tindex > 0:
+            self.m.plotmask = self.reader.CellCorrespondence(self.Tindex, self.FOVindex)
+            self.m.updatedata()
+        else:
+            pass
+            #self.m.plotmask = self.reader.LoadSeg(self.Tindex, self.FOVindex)
+            #self.m.updatedata()
+
+        self.Enable(self.button_cellcorrespondence)
+        self.button_cellcorrespondence.setChecked(False)
+        self.ClearStatusBar()
+        self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
+    
+    def ButtonSaveSegMask(self):
+        """saves the segmented mask
+        """
+        self.reader.SaveSegMask(self.Tindex, self.FOVindex, self.m.plotmask)
+
+        
+    def ChangePreviousFrame(self):
+         """This function is called when the previous frame buttons is pressed 
+         and it tests if the buttons is enabled and if so it calls the
+         BackwardTime() function. It should avoid the let the user do multiple 
+         clicks and that the function is then called afterwards several times,
+         once the frames and masks of the current time index have been loaded.
+         """
+         if self.button_previousframe.isEnabled():
+            self.button_previousframe.setEnabled(False)
+            self.BackwardTime()
+            if self.Tindex >0:
+                self.button_previousframe.setEnabled(True)
+         else:
+             return
+             
+             
+    def ChangeNextFrame(self):
+        """This function is called when the next frame buttons is pressed 
+        and it tests if the buttons is enabled and if so it calls the
+        ForwardTime() function. It should avoid the let the user do multiple 
+        clicks and that the function is then called afterwards several times,
+        once the frames and masks of the current time index have been loaded.
+        """
+        if self.button_nextframe.isEnabled():
+            self.button_nextframe.setEnabled(False)
+            self.ForwardTime()
+            if self.Tindex + 1 < self.reader.sizet:
+                self.button_nextframe.setEnabled(True)
+                
+        else:
+            return
+
+        
+    def ForwardTime(self):
+        """This function switches the frame in forward time index. And it tests
+        several conditions if t == lastTimeIndex-1, because then the next frame
+        button has to be disabled. It also tests if the show value of cells
+        button and hidemask are active in order to hide/show the mask or to 
+        show the cell values.
+        """
+        # the t frame is defined as the currently shown frame on the display.
+        # If the button "Next time frame" is pressed, this function is called
+        self.WriteStatusBar('Loading the next frame...')
+        self.Disable(self.button_nextframe)
+
+        if self.Tindex + 1 < self.reader.sizet - 1 :
+            self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
+            
+            self.m.prevpicture = self.m.currpicture.copy()
+            self.m.prevplotmask = self.m.plotmask.copy()
+            
+            self.m.currpicture = self.m.nextpicture.copy()
+            self.m.plotmask = self.m.nextplotmask.copy()
+            
+            self.m.nextpicture = self.reader.LoadOneImage(self.Tindex+2, self.FOVindex)
+            self.m.nextplotmask = self.reader.LoadMask(self.Tindex+2, self.FOVindex)
+
+            if self.Tindex + 1 == 1:
+                self.button_previousframe.setEnabled(True)
+                
+        else:
+            self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
+        
+            self.m.prevpicture = self.m.currpicture.copy()
+            self.m.prevplotmask = self.m.plotmask.copy()
+            self.m.currpicture = self.m.nextpicture.copy()
+            self.m.plotmask = self.m.nextplotmask.copy()
+            self.m.nextpicture = np.zeros([self.reader.sizey, self.reader.sizex], 
+                                          dtype = np.uint16)
+            self.m.nextplotmask = np.zeros([self.reader.sizey,self.reader.sizex], 
+                                           dtype = np.uint16)
+
+            self.button_nextframe.setEnabled(False)
+
+        self.Tindex = self.Tindex+1
+        self.m.UpdatePlots()
+        self.UpdateTitleSubplots()
+        
+        if self.button_hidemask.isChecked():
+            self.m.HideMask()
+
+        self.Enable(self.button_nextframe)
+        self.ClearStatusBar()
+        self.button_timeindex.setText(str(self.Tindex)+'/'+str(self.reader.sizet-1))
+
+    
+    def BackwardTime(self):
+        """This function switches the frame in backward time index. And it 
+        several conditions if t == 1, because then the button previous frame has to
+        be disabled. It also tests if the show value of cells button and 
+        hidemask are active in order to hide/show the mask or to show the cell
+        values.
+        """
+        # the t frame is defined as the currently shown frame on the display.
+        # If the button "Previous time frame" is pressed, this function is called
+        self.WriteStatusBar('Loading the previous frame...')
+        self.Disable(self.button_previousframe)
+        
+        self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
+
+        self.m.nextpicture = self.m.currpicture.copy()
+        self.m.nextplotmask = self.m.plotmask.copy()
+        self.m.currpicture = self.m.prevpicture.copy()
+        self.m.plotmask = self.m.prevplotmask.copy()
+            
+        if self.Tindex == 1:
+            self.m.prevpicture = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
+            self.m.prevplotmask = np.zeros([self.reader.sizey, self.reader.sizex], dtype = np.uint16)
+            self.button_previousframe.setEnabled(False)
+            
+        else:
+            self.m.prevpicture = self.reader.LoadOneImage(self.Tindex-2, self.FOVindex)
+            self.m.prevplotmask = self.reader.LoadMask(self.Tindex-2, self.FOVindex)
+
+        
+        if self.Tindex-1 == self.reader.sizet-2:
+            self.button_nextframe.setEnabled(True)            
+        
+        if self.button_hidemask.isChecked():
+            self.m.HideMask()
+        
+        self.Tindex -= 1
+        self.m.UpdatePlots()
+        self.UpdateTitleSubplots()
+            
+        self.Enable(self.button_previousframe)
+        
+        if self.Tindex > 0:
+            self.button_previousframe.setEnabled(True)          
+            
+        self.ClearStatusBar()
+        self.button_timeindex.setText(str(self.Tindex)+'/' + str(self.reader.sizet-1))
+
+
+# -----------------------------------------------------------------------------
+# MANUAL MASK CORRECTIONS
+            
+    def ChangeOneValue(self):
+        """This function is called when the button Change cell value is
+        clicked. It displays the instructions on the status bar.
+        And if the user clicks in the graph where the current mask is displayed
+        it connects the event of the click (meaning that user has clicked on
+        one cell) to the function self.DialogBoxChangeOneValue. 
+        This function will then replaces the cell selected by the user with
+        the click with a new value entered by the user.
+        """
+        
+        # displaying the instructions on the statusbar
+        self.WriteStatusBar((
+            'Left-click to select cell, right-click to abort.'))
+
+        # disables all the buttons
+        self.Disable(self.button_changecellvalue)
+        
+        # connects the event "press mouse button" in the matplotlib plot 
+        # (picture) to the function self.DialogBoxChangeOneValue
+        self.id = self.m.mpl_connect('button_press_event', self.DialogBoxChangeOneValue)
+        
+        
+    def DialogBoxChangeOneValue(self, event):
+        """This function is called when the user after the user has selected
+        the button Change cell value and clicked in the picture to select
+        the desired cell to change.
+        
+        It first deconnects the mouse click event in matplotlib with this 
+        function to not generate any other dialog window.
+        
+        It then tests if the click is inside the matplotlib plot (if it is
+        outside it equals to None) and if it is the current and editable plot
+        (the one in the middle of the gui, self.m.ax)
+        
+        If is true, then it sets the coordinates to int. and creates a dialog
+        window where the user is asked to type a value to set it to the cell.
+        
+        If the user presses ok, it tests if the entry is valid (>0 and not 
+        empty) and looks for the old cell value and replaces it. And then
+        it updates the plot such that the result of the change can be seen.
+        """
+        # the function is disconnected from the matplotlib event.
+        self.m.mpl_disconnect(self.id)
+        
+        # test if the button is a left click and if the coordinates
+        # chosen by the user click is inside of the current matplotlib plot
+        # which is given by self.m.ax
+        if (event.button == 1 
+            and (event.xdata != None and event.ydata != None) 
+            and self.m.ax == event.inaxes):
+            newx = int(event.xdata)
+            newy = int(event.ydata)
+            
+            # creates a dialog window
+            dlg = cocv.CustomDialog(self)
+            
+            #if the user presses 'ok' in the dialog window it executes the code
+            #else it does nothing
+            result = dlg.exec()
+            if result == QDialog.DialogCode.Accepted:
+                #it tests that the user has entered some value, that it is not
+                #empty and that it is equal or bigger to 0.
+                if dlg.entry1.text() != '' and int(dlg.entry1.text()) >= 0:
+                    #reads the new value to set and converts it from str to int
+                    value = int(dlg.entry1.text())
+                    
+                    # gives the coordinates where it is equal to the value
+                    # selected by the user. And it replaces it with the new
+                    # value.
+                    self.m.plotmask[self.m.plotmask == self.m.plotmask[newy,newx]] = value
+                    
+                    # updates the plot to see the modification.
+                    self.m.updatedata()
+                    
+        self.Enable(self.button_changecellvalue)
+        self.button_changecellvalue.setChecked(False)
+        self.m.ShowCellNumbers(type='current')
+        self.SaveMask()
+        self.ClearStatusBar()
+        
+        
+    def DialogBoxECV(self, s):
+        """This functions creates from the ExchangeCellValues.py file a 
+        window which takes two integer entries and then swaps the cells having
+        the given integer values.
+        """
+        # creates a dialog window from the ExchangeCellValues.py file
+        dlg = ecv.CustomDialog(self)
+        
+        # if the user presses 'ok', it executes the code
+        result = dlg.exec()
+        if result == QDialog.DialogCode.Accepted:
+            # it tests if both value to be swapped are not empty.
+            if dlg.entry1.text()!= '' and dlg.entry2.text() != '':
+                
+                # reads out the values and converts it into integers.
+                value1 = int(dlg.entry1.text())
+                value2 = int(dlg.entry2.text())
+                
+                # calls the function which does the swap
+                try:
+                    self.m.ExchangeCellValue(value1,value2)
+                except ValueError as e:
+                    msg_box = QMessageBox(QMessageBox.Icon.Critical, 'Error', str(e), parent=self)
+                    msg_box.exec()
+                self.m.ShowCellNumbers(type='current')
+                self.SaveMask()
+        else:
+            return
+
+
+    def MouseDraw(self):
+        """
+        This function is called whenever the brush or the eraser button is
+        pressed. On the first press event it calls the self.m.OneClick, which
+        tests whether it is a right click or a left click. If it a right click
+        it assigns the value of the pixel which has been right clicked
+        to self.cellval, meaning that the next drawn pixels will be set to this
+        value.
+        If it is left clicked, then it draws a 3x3 square with the current
+        value of self.cellval.
+        If after left clicking you drag the mouse, then you start drawing 
+        using the mouse and it stops once you release the left click.
+        
+        Same for the eraser button, it sets directly the value of self.cellval
+        to 0.
+        """
+        do_draw = self.button_drawmouse.isChecked()
+        do_erase = self.button_eraser.isChecked()
+        
+        if do_draw or do_erase:
+            self.m.tempmask = self.m.plotmask.copy()
+            
+            #save status of the showval check box, then turn off (slows brush/eraser down too much)
+            self.showval_was_checked = self.button_showval.isChecked()
+            self.button_showval.setChecked(False)
+            
+            if do_draw:
+                self.WriteStatusBar(('Draw using the brush, right click to select '
+                                     'the cell to draw.'))
+                self.Disable(self.button_drawmouse)
+                
+            elif do_erase:
+                self.WriteStatusBar('Erasing by setting the values to 0.')
+                self.Disable(self.button_eraser)
+                self.m.cellval = 0
+                
+            radius = self.spinbox_brushsize.value()
+            self.id2 = self.m.mpl_connect('button_press_event', 
+                                          lambda e: self.m.OneClick(e, radius))
+            self.id = self.m.mpl_connect('motion_notify_event', 
+                                          lambda e: self.m.PaintBrush(e, radius))
+            self.id3 = self.m.mpl_connect('button_release_event', self.m.ReleaseClick)
+                
+                        
+        else:
+            self.m.mpl_disconnect(self.id3)
+            self.m.mpl_disconnect(self.id2)
+            self.m.mpl_disconnect(self.id)
+            QApplication.restoreOverrideCursor()
+            self.Enable(self.button_drawmouse)
+            self.Enable(self.button_eraser)
+            self.button_showval.setChecked(self.showval_was_checked)
+            self.SaveMask()
+            self.ClearStatusBar()
+            
+            
+    
+    def SelectSplitCell(self):
+        """Function called upon clicking Split Cell button"""
+      
+        if self.button_split.isChecked():
+            self.cell_to_split=-1
+            self.Disable(self.button_split)
+            self.WriteStatusBar('First, select the cell to be split with a left click. '
+                                'Then, left-click the corners of a polygon to be split off from the '
+                                'selected cell. Right click to confirm.')
+            
+            def sel_cell(e):
+                if e.button != 1:
+                    self.cell_to_split=-1
+                    self.Enable(self.button_split)
+                else:
+                    x = int(e.xdata)
+                    y = int(e.ydata)
+                    self.cell_to_split = self.m.plotmask[y,x]
+                    self.m.mpl_disconnect(self.id)
+                    self.ClickSplitCell()
+    
+            self.id = self.m.mpl_connect('button_press_event', sel_cell)
+            
+        else:
+            self.DoSplitCell()
+
+
+    def ClickSplitCell(self):
+        self.WriteStatusBar('Click to define the corners of a polygon which'
+                            'will be split off the selected cell. Right click '
+                            'or reclick the button to confirm.')
+        if self.cell_to_split == -1:
+            return
+        
+        self.m.tempmask = self.m.plotmask.copy()
+        self.m.storemouseclicks = [] 
+        self.id = self.m.mpl_connect('button_press_event', 
+                                     lambda e: self.m.multiple_click(e, self.DoSplitCell))
+
+        
+    def DoSplitCell(self):
+        self.m.mpl_disconnect(self.id)
+        if len(self.m.storemouseclicks) > 2:
+            nx, ny = self.m.plotmask.shape
+            img = Image.new('L', (ny, nx), 0)
+            ImageDraw.Draw(img).polygon(self.m.storemouseclicks, outline=1, fill=1)
+            polygon = np.array(img).astype(bool)
+            selected_mask = self.m.plotmask==self.cell_to_split
+            replace_cell = self.m.plotmask.max() + 1
+            self.m.plotmask[selected_mask & polygon] = replace_cell
+        self.Enable(self.button_split)
+        self.m.UpdatePlots(type='current')
+        self.ClearStatusBar()
+        self.SaveMask()
+        self.m.storemouseclicks = []
+        self.button_split.setChecked(False)
+        
+        
+    def UpdateTitleSubplots(self):
+        """This function updates the title of the plots according to the 
+        current time index. So it called whenever a frame or a fov is changed.
+        """
+        if self.Tindex == 0:
+            self.m.titlecurr.set_text('Time index {}'.format(self.Tindex))
+            self.m.titleprev.set_text('No frame {}'.format(''))
+            self.m.titlenext.set_text('Next time index {}'.format(self.Tindex+1))
+            self.m.draw()
+            
+        elif self.Tindex == self.reader.sizet-1:
+            self.m.titlecurr.set_text('Time index {}'.format(self.Tindex))
+            self.m.titleprev.set_text('Previous time index {}'.format(self.Tindex-1))
+            self.m.titlenext.set_text('No frame {}'.format(''))            
+            self.m.draw()
+            
+        else:
+            self.m.titlecurr.set_text('Time index {}'.format(self.Tindex))
+            self.m.titleprev.set_text('Previous time index {}'.format(self.Tindex-1))
+            self.m.titlenext.set_text('Next time index {}'.format(self.Tindex+1))
+            self.m.draw()
+        
+        
+    def ClickNewCell(self):
+        """ 
+        this method is called when the button New Cell is clicked. If the button
+        state corresponds to True (if is activated) then it connects the mouse 
+        clicks on the pyqt window to the canvas (so to the matplolib figure).
+        The connection has an "id" which is given by the integer self.id
+        After the connections is made, it calls the Disable function with argument 0
+        which turns off the other button(s).
+        
+        If the button is clicked but it is deactivated then it disconnects the 
+        connection between the canvas and the window (the user can not interact
+        with the plot anymore). 
+        Storemouseclicks is a list corresponding to the coordinates of all mouse
+        clicks between the activation and the deactivation of the button.
+        So if it is empty, it does not draw anything because no clicks
+        were registered. 
+        But if it has some coordinates, it will draw a polygon where the vertices
+        are the coordinates of all the mouseclicks.
+        Once the figure has been updated with a new polygon, the other button(s)
+        are again enabled. 
+        
+        """
+        if self.button_newcell.isChecked():
+            self.WriteStatusBar(('Draw a new cell. Use the left click to '
+                                 'produce a polygon with a new cell value. '
+                                 'Click the button again to confirm.'))
+            self.m.tempmask = self.m.plotmask.copy()
+            self.id = self.m.mpl_connect('button_press_event', self.m.MouseClick)
+            self.Disable(self.button_newcell)
+            
+        else:
+            self.m.mpl_disconnect(self.id)
+            if  self.m.storemouseclicks and self.TestSelectedPoints():
+                self.m.DrawRegion(True)
+            else:
+                self.m.updatedata()
+            self.Enable(self.button_newcell)
+            self.m.ShowCellNumbers(type='current')
+            self.ClearStatusBar()
+            self.SaveMask()
+            
+            
+    def TestSelectedPoints(self):
+        """This function is just used to catch an exception, when the new cell
+        or the add region function is called. If all the dots drawn by the user
+        are located on one line (horizontal or vertical) the DrawRegion 
+        function calls a method to create a polygon and 
+        it can not make a polygon out of straight line so it gives an error.
+        In order to prevent this error, this function avoids to attempt to draw
+        by returning False if the square are all on one line.
+        """
+                
+        allx = list(np.array(self.m.storemouseclicks)[:,0])
+        ally = list(np.array(self.m.storemouseclicks)[:,1])
+        
+        resultx = all(elem == allx[0] for elem in allx)
+        resulty = all(elem == ally[0] for elem in ally)
+        
+        if resultx or resulty:
+            return False
+        else:
+            return True
+                    
+        
+    def clickmethod(self):
+        """ 
+        this method is called when the button Add region is clicked. If the button
+        state corresponds to True (if is activated) then it connects the mouse 
+        clicks on the pyqt window to the canvas (so to the matplolib figure).
+        The connection has an "id" which is given by the integer self.id
+        After the connections is made, it calls the Disable function with argument 1
+        which turns off the other button(s).
+        
+        If the button is clicked and it is deactivated then it disconnects the 
+        connection between the canvas and the window (the user can not interact
+        with the plot anymore). 
+        Storemouseclicks is a list corresponding to the coordinates of all mouse
+        clicks between the activation and the deactivation of the button.
+        So if it is empty, it does not draw anything because no clicks
+        were registered. 
+        But if it has some coordinates, it will draw a polygon where the vertices
+        are the coordinates of all the mouseclicks.
+        Once the figure has been updated with a new polygon, the other button(s)
+        are again enabled. 
+        
+        """
+        if self.button_add_region.isChecked():
+            self.WriteStatusBar(('Select the cell with the first click, '
+                                 'then draw polygon with subsequent '
+                                 'clicks. Reclick the button to confirm.'))
+            self.m.tempmask = self.m.plotmask.copy()
+            self.id = self.m.mpl_connect('button_press_event', self.m.MouseClick)           
+            self.Disable(self.button_add_region) 
+            
+        else:
+            self.m.mpl_disconnect(self.id)
+            
+            # test if the list is not empty and if the dots are not all in the same line
+            if self.m.storemouseclicks and self.TestSelectedPoints():
+                self.m.DrawRegion(False)
+
+            else:
+                self.m.updatedata()
+                
+            self.Enable(self.button_add_region)
+            self.m.ShowCellNumbers(type='current')
+            self.ClearStatusBar()
+            self.SaveMask()
+            
+            
+    def MergeWithNeighbors(self):
+        """This function is called when the button Merge With Neighbors is
+        clicked. It displays the instructions on the status bar.
+        And if the user clicks in the graph where the current mask is displayed
+        it connects the event of the click (meaning that user has clicked on
+        one cell) to the function self.PerformMergeWithNeighbors. 
+        This function will then merge the cell selected by the user with
+        the click with all (touching) neighbors.
+        """
+        
+        # displaying the instructions on the statusbar
+        self.WriteStatusBar((
+            'Left-click to select cell, right-click to abort.'))
+
+        # disables all the buttons
+        self.Disable(self.button_mergewithneighbors)
+        
+        # connects the event "press mouse button" in the matplotlib plot 
+        # (picture) to the function self.PerformMergeWithNeighbors
+        self.id = self.m.mpl_connect('button_press_event', self.PerformMergeWithNeighbors)
+        
+        
+    def PerformMergeWithNeighbors(self, event):
+        """This function is called after the user has selected
+        the button Merge With Neighbors and clicked in the picture to select
+        the desired cell to start the merger.
+        
+        It first deconnects the mouse click event in matplotlib with this 
+        function to not generate any other dialog window.
+        
+        It then tests if the click is inside the matplotlib plot (if it is
+        outside it equals to None) and if it is the current and editable plot
+        (the one in the middle of the gui, self.m.ax)
+        
+        If is true, then it sets the coordinates to int. and creates a dialog
+        window where the user is asked to type a value to set it to the cell.
+        
+        If the user presses ok, it tests if the entry is valid (>0 and not 
+        empty) and looks for the old cell value and replaces it. And then
+        it updates the plot such that the result of the change can be seen.
+        """
+        # the function is disconnected from the matplotlib event.
+        self.m.mpl_disconnect(self.id)
+        
+        # test if the button is a left click and if the coordinates
+        # chosen by the user click is inside of the current matplotlib plot
+        # which is given by self.m.ax
+        if (event.button == 1 
+            and (event.xdata != None and event.ydata != None) 
+            and self.m.ax == event.inaxes):
+            newx = int(event.xdata)
+            newy = int(event.ydata)
+            # get the ID of the selected cell
+            selectedcell_ID = self.m.plotmask[newy,newx]
+            # binarize the existing mask and number ("label") each component
+            labeled_binarized_mask = skimage.measure.label(self.m.plotmask > 0)
+            # select the component pixels that corresponds to the selected point
+            flood_indices=(labeled_binarized_mask==labeled_binarized_mask[newy,newx])
+            # set the mask pixels that correspond to the component to the cell ID
+            self.m.plotmask[flood_indices] = selectedcell_ID
+                    
+            # updates the plot to see the modification.
+            self.m.updatedata()
+                    
+        self.Enable(self.button_mergewithneighbors)
+        self.button_mergewithneighbors.setChecked(False)
+        self.m.ShowCellNumbers(type='current')
+        self.SaveMask()
+        self.ClearStatusBar()
+        
+        
+# -----------------------------------------------------------------------------
+# BUTTON ENABLE / DISABLE
+    
+    def Enable(self, button):
+        """
+        this functions turns on buttons all the buttons, depending on the time
+        index. (next and previous buttons should not be turned on if t = 0 
+        or t = lasttimeindex)
+        """
+        for k in range(0, len(self.buttonlist)):
+            if button != self.buttonlist[k]:
+                self.buttonlist[k].setEnabled(True)
+                
+        if self.Tindex == 0:
+            self.button_previousframe.setEnabled(False)
+            
+        if self.Tindex == self.reader.sizet-1:
+            self.button_nextframe.setEnabled(False)
+            
+        self.EnableCNNButtons()
+         
+     
+    def Disable(self, button):
+        """
+        this functions turns off all the buttons except the one given in 
+        argument.
+        """
+
+        for k in range(0,len(self.buttonlist)):
+            if button != self.buttonlist[k]:
+                self.buttonlist[k].setEnabled(False)
+
+
+    def EnableCNNButtons(self):
+        if self.reader.TestTimeExist(self.Tindex, self.FOVindex):
+            self.button_cellcorrespondence.setEnabled(True)
+            self.button_extractfluorescence.setEnabled(True)
+        else:
+            self.button_cellcorrespondence.setEnabled(False)
+            self.button_extractfluorescence.setEnabled(False)
+    
+    
+    def EnableCorrectionsButtons(self):
+        self.button_newcell.setEnabled(True)
+        self.button_add_region.setEnabled(True)
+        self.button_drawmouse.setEnabled(True)
+        self.button_eraser.setEnabled(True)
+        self.button_exval.setEnabled(True)
+        self.button_changecellvalue.setEnabled(True)
+        self.button_showval.setEnabled(True)
+        self.button_split.setEnabled(True)
+        
+        
+    def DisableCorrectionsButtons(self):
+        self.button_newcell.setEnabled(False)
+        self.button_add_region.setEnabled(False)
+        self.button_drawmouse.setEnabled(False)
+        self.button_eraser.setEnabled(False)
+        self.button_exval.setEnabled(False)
+        self.button_changecellvalue.setEnabled(False)
+        self.button_showval.setEnabled(False)
+        self.button_split.setEnabled(False)
+        
+    
+    def SaveMask(self):
+        """
+        When this function is called, it saves the current mask
+        (self.m.plotmask)
+        """
+        self.reader.SaveMask(self.Tindex, self.FOVindex, self.m.plotmask)
+        
+        
+    def WriteStatusBar(self, text):
+        """Writes text to status bar"""
+        self.statusBarText.setText(text)
+        
+        
+    def ClearStatusBar(self):
+        """Removes text from status bar"""
+        self.statusBarText.setText('')
```

### Comparing `YeaZ-1.0.0rc1/yeaz/Launch_NN_command_line.py` & `YeaZ-1.0.1/yeaz/Launch_NN_command_line.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-# Run:
-#
-# python Launch_NN_command_line.py -i DIRECTORY/IMAGE_FILE -m OUTPUT_MASK_FILE --path_to_weights PATH_TO_HDF5_FILE --fov N --range_of_frames n1 n2 --min_seed_dist 5 --threshold 0.5
-# 
-# or:
-#
-# python Launch_NN_command_line.py -i DIRECTORY/IMAGE_FILE -m OUTPUT_MASK_FILE --image_type pc_OR_bf               --fov N --range_of_frames n1 n2 --min_seed_dist 5 --threshold 0.5
-
-import time
-import tqdm
-
-import sys
-
-#Import all the other python files
-#this file handles the interaction with the disk, so loading/saving images
-#and masks and it also runs the neural network.
-
-
-from yeaz.unet.segment import segment
-from yeaz.disk import Reader as nd
-import argparse
-import skimage
-from yeaz.unet import neural_network as nn
-
-import torch
-
-def LaunchPrediction(im, mic_type, pretrained_weights=None, device='cpu'):
-    """It launches the neural neutwork on the current image and creates 
-    an hdf file with the prediction for the time T and corresponding FOV. 
-    """
-    im = skimage.exposure.equalize_adapthist(im)
-    im = im*1.0;	
-    pred = nn.prediction(im, mic_type, pretrained_weights, device=device)
-    return pred
-
-
-
-def ThresholdPred(thvalue, pred):
-    """Thresholds prediction with value"""
-    if thvalue == None:
-        thresholdedmask = nn.threshold(pred)
-    else:
-        thresholdedmask = nn.threshold(pred, thvalue)
-    return thresholdedmask
-
-def LaunchInstanceSegmentation(reader, image_type, fov_indices=[0], time_value1=0, time_value2=0, thr_val=None, min_seed_dist=5, path_to_weights=None, device='cpu'):
-    if (device == 'cuda') and torch.cuda.is_available():
-        f_device = 'cuda'
-    else:
-        f_device = 'cpu' 
-    # cannot have both path_to_weights and image_type supplied
-    if (image_type is not None) and (path_to_weights is not None):
-        print("image_type and path_to_weights cannot be both supplied.")
-        return
-    
-
-    # check if correct imaging value
-    if (image_type not in ['bf', 'pc']) and (path_to_weights is None):
-        print("Wrong imaging type value ('{}')!".format(image_type),
-              "imaging type must be either 'bf' or 'pc'")
-        return
-
-    # check range_of_frames constraint
-    if time_value1 > time_value2 :
-        print("Error", 'Invalid Time Constraints')
-        return
-    
-    # displays that the neural network is running
-    print('Running the neural network on {} ...'.format(f_device))
-    
-    for fov_ind in tqdm.tqdm(fov_indices, desc='FOV', position=0):
-
-        #iterates over the time indices in the range
-        for t in tqdm.tqdm(range(time_value1, time_value2+1), desc='Time', position=1, leave=False):         
-            # print('--------- Segmenting field of view:',fov_ind,'Time point:',t)
-
-            #calls the neural network for time t and selected fov
-            im = reader.LoadOneImage(t, fov_ind)
-
-            try:
-                pred = LaunchPrediction(im, image_type, pretrained_weights=path_to_weights, device=f_device)
-            except ValueError:
-                print('Error! ',
-                      'The neural network weight files could not '
-                      'be found. \nMake sure to download them from '
-                      'the link in the readme and put them into '
-                      'the folder unet, or specify a path to a custom weights file with -w argument.')
-                return
-
-            thresh = ThresholdPred(thr_val, pred)
-            seg = segment(thresh, pred, min_seed_dist)
-            reader.SaveMask(t, fov_ind, seg)
-            print('--------- Finished segmenting.')
-            
-            # apply tracker if wanted and if not at first time
-            temp_mask = reader.CellCorrespondence(t, fov_ind)
-            reader.SaveMask(t, fov_ind, temp_mask)
-
-def main(args):
-
-    if '.h5' in args.mask_path:
-        args.mask_path = args.mask_path.replace('.h5','')
-
-    reader = nd.Reader("", args.mask_path+'.h5', args.image_path)
-
-    LaunchInstanceSegmentation(reader, args.image_type, args.fov,
-                               args.range_of_frames[0],  args.range_of_frames[1], 
-                               args.threshold, args.min_seed_dist, 
-                               args.path_to_weights, device=args.device)
-
-if __name__ == '__main__':
-    
-    parser = argparse.ArgumentParser(description='', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-    parser.add_argument('-i', '--image_path', type=str, help="Specify the path to a single image or to a folder of images", required=True)
-    parser.add_argument('-m', '--mask_path', type=str, help="Specify where to save predicted masks", required=True)
-    parser.add_argument('--image_type', type=str, help="Specify the imaging type, possible types are 'bf', 'pc', and 'fission'. Supersedes path_to_weights.")
-    parser.add_argument('--path_to_weights', default=None, type=str, help="Specify weights path.")
-    parser.add_argument('--fov', default=[0], nargs='+', type=int, help="Specify field of view index (can specify more than one with space between them).")
-    parser.add_argument('--range_of_frames', nargs=2, default=[0,0], type=int, help="Specify start and end in range of frames. (e.g. 0 10)")
-    parser.add_argument('--threshold', default=None, type=float, help="Specify threshold value.")
-    parser.add_argument('--min_seed_dist', default=5, type=int, help="Specify minimum distance between seeds.")
-    parser.add_argument('--device', default='cpu', type=str, help="Specify device to run on (cpu or cuda).")
-    args = parser.parse_args()
-    main(args)
+# Run:
+#
+# python Launch_NN_command_line.py -i DIRECTORY/IMAGE_FILE -m OUTPUT_MASK_FILE --path_to_weights PATH_TO_HDF5_FILE --fov N --range_of_frames n1 n2 --min_seed_dist 5 --threshold 0.5
+# 
+# or:
+#
+# python Launch_NN_command_line.py -i DIRECTORY/IMAGE_FILE -m OUTPUT_MASK_FILE --image_type pc_OR_bf               --fov N --range_of_frames n1 n2 --min_seed_dist 5 --threshold 0.5
+
+import time
+import tqdm
+
+import sys
+
+#Import all the other python files
+#this file handles the interaction with the disk, so loading/saving images
+#and masks and it also runs the neural network.
+
+
+from yeaz.unet.segment import segment
+from yeaz.disk import Reader as nd
+import argparse
+import skimage
+from yeaz.unet import neural_network as nn
+
+import torch
+
+def LaunchPrediction(im, mic_type, pretrained_weights=None, device='cpu'):
+    """It launches the neural neutwork on the current image and creates 
+    an hdf file with the prediction for the time T and corresponding FOV. 
+    """
+    im = skimage.exposure.equalize_adapthist(im)
+    im = im*1.0;	
+    pred = nn.prediction(im, mic_type, pretrained_weights, device=device)
+    return pred
+
+
+
+def ThresholdPred(thvalue, pred):
+    """Thresholds prediction with value"""
+    if thvalue == None:
+        thresholdedmask = nn.threshold(pred)
+    else:
+        thresholdedmask = nn.threshold(pred, thvalue)
+    return thresholdedmask
+
+def LaunchInstanceSegmentation(reader, image_type, fov_indices=[0], time_value1=0, time_value2=0, thr_val=None, min_seed_dist=5, path_to_weights=None, device='cpu'):
+    if (device == 'cuda') and torch.cuda.is_available():
+        f_device = 'cuda'
+    else:
+        f_device = 'cpu' 
+    # cannot have both path_to_weights and image_type supplied
+    if (image_type is not None) and (path_to_weights is not None):
+        print("image_type and path_to_weights cannot be both supplied.")
+        return
+    
+
+    # check if correct imaging value
+    if (image_type not in ['bf', 'pc']) and (path_to_weights is None):
+        print("Wrong imaging type value ('{}')!".format(image_type),
+              "imaging type must be either 'bf' or 'pc'")
+        return
+
+    # check range_of_frames constraint
+    if time_value1 > time_value2 :
+        print("Error", 'Invalid Time Constraints')
+        return
+    
+    # displays that the neural network is running
+    print('Running the neural network on {} ...'.format(f_device))
+    
+    for fov_ind in tqdm.tqdm(fov_indices, desc='FOV', position=0):
+
+        #iterates over the time indices in the range
+        for t in tqdm.tqdm(range(time_value1, time_value2+1), desc='Time', position=1, leave=False):         
+            # print('--------- Segmenting field of view:',fov_ind,'Time point:',t)
+
+            #calls the neural network for time t and selected fov
+            im = reader.LoadOneImage(t, fov_ind)
+
+            try:
+                pred = LaunchPrediction(im, image_type, pretrained_weights=path_to_weights, device=f_device)
+            except ValueError:
+                print('Error! ',
+                      'The neural network weight files could not '
+                      'be found. \nMake sure to download them from '
+                      'the link in the readme and put them into '
+                      'the folder unet, or specify a path to a custom weights file with -w argument.')
+                return
+
+            thresh = ThresholdPred(thr_val, pred)
+            seg = segment(thresh, pred, min_seed_dist)
+            reader.SaveMask(t, fov_ind, seg)
+            print('--------- Finished segmenting.')
+            
+            # apply tracker if wanted and if not at first time
+            temp_mask = reader.CellCorrespondence(t, fov_ind)
+            reader.SaveMask(t, fov_ind, temp_mask)
+
+def main(args):
+
+    if '.h5' in args.mask_path:
+        args.mask_path = args.mask_path.replace('.h5','')
+
+    reader = nd.Reader("", args.mask_path+'.h5', args.image_path)
+
+    LaunchInstanceSegmentation(reader, args.image_type, args.fov,
+                               args.range_of_frames[0],  args.range_of_frames[1], 
+                               args.threshold, args.min_seed_dist, 
+                               args.path_to_weights, device=args.device)
+
+if __name__ == '__main__':
+    
+    parser = argparse.ArgumentParser(description='', formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('-i', '--image_path', type=str, help="Specify the path to a single image or to a folder of images", required=True)
+    parser.add_argument('-m', '--mask_path', type=str, help="Specify where to save predicted masks", required=True)
+    parser.add_argument('--image_type', type=str, help="Specify the imaging type, possible types are 'bf', 'pc', and 'fission'. Supersedes path_to_weights.")
+    parser.add_argument('--path_to_weights', default=None, type=str, help="Specify weights path.")
+    parser.add_argument('--fov', default=[0], nargs='+', type=int, help="Specify field of view index (can specify more than one with space between them).")
+    parser.add_argument('--range_of_frames', nargs=2, default=[0,0], type=int, help="Specify start and end in range of frames. (e.g. 0 10)")
+    parser.add_argument('--threshold', default=None, type=float, help="Specify threshold value.")
+    parser.add_argument('--min_seed_dist', default=5, type=int, help="Specify minimum distance between seeds.")
+    parser.add_argument('--device', default='cpu', type=str, help="Specify device to run on (cpu or cuda).")
+    args = parser.parse_args()
+    main(args)
```

### Comparing `YeaZ-1.0.0rc1/yeaz/__main__.py` & `YeaZ-1.0.1/yeaz/__main__.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-
-
-def _setup_gui():
-    try:
-        from PyQt6.QtCore import Qt
-    except Exception as e:
-        txt = (
-            'To run the GUI YeaZ needs to install a package called `PyQt6`.\n\n'
-            'You can let YeaZ install it now, or you can abort (press "n")\n'
-            'and install it manually with the following command:\n\n'
-            'pip install PyQt6\n'
-        )
-        print('-'*60)
-        print(txt)
-        while True:
-            answer = input('Do you want to install PyQt6 now ([y]/n)? ')
-            if answer.lower() == 'y' or not answer:
-                import subprocess
-                import sys
-                subprocess.check_call(
-                    [sys.executable, '-m', 'pip', 'install', '-U', 'PyQt6']
-                )
-                warn_restart = True
-                break
-            elif answer.lower() == 'n':
-                raise e
-            else:
-                print(
-                    f'"{answer}" is not a valid answer. '
-                    'Type "y" for "yes", or "n" for "no".'
-                )
-
-def run():
-    _setup_gui()
-    
-    print('Initializing application...')
-    
-    import sys
-    from PyQt6.QtWidgets import QApplication
-    
-    from .GUI_main import App
-    #this file contains a dialog window which is opened before the main program
-    #and allows to load the nd2 and hdf files by browsing through the computer.
-    from .disk import DialogFileBrowser as dfb
-    
-    app = QApplication(sys.argv)
-    
-    # If two arguments are given, make them nd2name and hdfname
-    if len(sys.argv)==3:
-        nd2name1 = sys.argv[1]
-        hdfname1 = sys.argv[2]
-        ex = App(nd2name1, hdfname1, '')
-        print('------------------------------------------------ Welcome to YeaZ-GUI -------------------------------------------------------')
-
-        sys.exit(app.exec())
-    
-    # Launch file browser otherwise
-    else:
-        wind = dfb.FileBrowser()
-        if wind.exec():
-            nd2name1 = wind.nd2name 
-            hdfname1 = wind.hdfname
-            hdfnewname = wind.newhdfname
-
-            ex = App(str(nd2name1), str(hdfname1), str(hdfnewname))
-            print('------------------------------------------------ Welcome to YeaZ-GUI -------------------------------------------------------')
-            sys.exit(app.exec())
-        else:
+
+
+def _setup_gui():
+    try:
+        from PyQt6.QtCore import Qt
+    except Exception as e:
+        txt = (
+            'To run the GUI YeaZ needs to install a package called `PyQt6`.\n\n'
+            'You can let YeaZ install it now, or you can abort (press "n")\n'
+            'and install it manually with the following command:\n\n'
+            'pip install PyQt6\n'
+        )
+        print('-'*60)
+        print(txt)
+        while True:
+            answer = input('Do you want to install PyQt6 now ([y]/n)? ')
+            if answer.lower() == 'y' or not answer:
+                import subprocess
+                import sys
+                subprocess.check_call(
+                    [sys.executable, '-m', 'pip', 'install', '-U', 'PyQt6']
+                )
+                warn_restart = True
+                break
+            elif answer.lower() == 'n':
+                raise e
+            else:
+                print(
+                    f'"{answer}" is not a valid answer. '
+                    'Type "y" for "yes", or "n" for "no".'
+                )
+
+def run():
+    _setup_gui()
+    
+    print('Initializing application...')
+    
+    import sys
+    from PyQt6.QtWidgets import QApplication
+    
+    from .GUI_main import App
+    #this file contains a dialog window which is opened before the main program
+    #and allows to load the nd2 and hdf files by browsing through the computer.
+    from .disk import DialogFileBrowser as dfb
+    
+    app = QApplication(sys.argv)
+    
+    # If two arguments are given, make them nd2name and hdfname
+    if len(sys.argv)==3:
+        nd2name1 = sys.argv[1]
+        hdfname1 = sys.argv[2]
+        ex = App(nd2name1, hdfname1, '')
+        print('------------------------------------------------ Welcome to YeaZ-GUI -------------------------------------------------------')
+
+        sys.exit(app.exec())
+    
+    # Launch file browser otherwise
+    else:
+        wind = dfb.FileBrowser()
+        if wind.exec():
+            nd2name1 = wind.nd2name 
+            hdfname1 = wind.hdfname
+            hdfnewname = wind.newhdfname
+
+            ex = App(str(nd2name1), str(hdfname1), str(hdfnewname))
+            print('------------------------------------------------ Welcome to YeaZ-GUI -------------------------------------------------------')
+            sys.exit(app.exec())
+        else:
             app.exit()
```

### Comparing `YeaZ-1.0.0rc1/yeaz/disk/Reader.py` & `YeaZ-1.0.1/yeaz/disk/Reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,389 +1,409 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Oct 15 15:00:29 2019
-
-This file handles all interactions with the hdf and image files, such as 
-loading or saving a particular image.
-"""
-from nd2reader import ND2Reader
-import numpy as np
-import re
-import h5py
-import os.path
-import skimage
-import skimage.io
-
-#import pytiff
-from ..unet import hungarian as hu
-
-import logging
-import os
-logging.basicConfig(
-    format='%(asctime)s %(levelname)s %(funcName)s: %(message)s',
-    level=os.environ.get("LOGLEVEL", "WARNING")
-)
-log = logging.getLogger(__name__)
-
-
-class Reader:
-    
-    
-    def __init__(self, hdfpathname, newhdfname, nd2pathname):
-        """
-        Initializes the data corresponding to the sizes of the pictures,
-        the number of different fields of views(Npos) taken in the experiment.
-        And it also sets the number of time frames per field of view.
-        """
-        # Identify filetype of image file
-        _, self.extension = os.path.splitext(nd2pathname)
-        self.isnd2 = self.extension == '.nd2'
-        self.isfolder = self.extension == ''
-        self.issingle = self.extension in ['.tif','.tiff',
-                                            '.jpg','.jpeg','.png','.bmp',
-                                           '.pbm','.pgm','.ppm','.pxm','.pnm','.jp2',
-                                           '.TIF','.TIFF',
-                                            '.JPG','.JPEG','.PNG','.BMP',
-                                           '.PBM','.PGM','.PPM','.PXM','.PNM','.JP2']
-        
-        self.nd2path = nd2pathname # path name is nd2path for legacy reasons
-        self.hdfpath = hdfpathname
-        self.newhdfpath = newhdfname
-        
-        if self.isnd2:
-            with ND2Reader(self.nd2path) as images:
-                self.sizex = images.sizes['x']
-                self.sizey = images.sizes['y']
-                self.sizet = images.sizes['t']
-                try:
-                    self.sizec = images.sizes['c']
-                except KeyError:
-                    self.sizec = 1
-                try:
-                    self.Npos  = images.sizes['v']
-                except KeyError:
-                    self.Npos  = 1
-                self.channel_names = images.metadata['channels']
-                
-        elif self.issingle:
-#            with pytiff.Tiff(self.nd2path) as handle:
-#                self.sizey, self.sizex = handle.shape #SJR: changed by me
-#                self.sizec = 1
-#                self.sizet = handle.number_of_pages
-#                self.Npos = 1
-#                self.channel_names = ['Channel1']
-            im = skimage.io.imread(self.nd2path)
-
-            if im.ndim==3:
-                # num pages should be smaller than x or y dimension, very unlikely not to be the case
-                if im.shape[2] < im.shape[0] and im.shape[2] < im.shape[1]:  
-                    im = np.moveaxis(im, -1, 0) # move last axis to first
-                self.sizet, self.sizey, self.sizex = im.shape
-            else:
-                self.sizey, self.sizex = im.shape
-                self.sizet = 1
-                
-            self.Npos = 1
-            self.channel_names = ['Channel1']
-                
-        elif self.isfolder:
-            filelist = sorted(os.listdir(self.nd2path))            
-            for f in filelist:
-                if f.startswith('.'):
-                    filelist.remove(f)
-            self.sizey = 0
-            self.sizex = 0
-            
-            # filter filelist for supported image files
-            filelist = [f for f in filelist if re.search(r".png|.tif|.jpg|.bmp|.jpeg|.pbm|.pgm|.ppm|.pxm|.pnm|.jp2"
-                                                         "|.PNG|.TIF|.JPG|.BMP|.JPEG|.PBM|.PGM|.PPM|.PXM|.PNM|.JP2", f)]
-            
-            for f in filelist:
-                im = skimage.io.imread(os.path.join(self.nd2path , f))
-                self.sizey = max(self.sizey, im.shape[0]) #SJR: changed by me
-                self.sizex = max(self.sizex, im.shape[1]) #SJR: changed by me
-            self.sizec = 1
-            self.Npos = 1
-            self.sizet = len(filelist)
-            self.channel_names = ['Channel1']
-                            
-        #create the labels which index the masks with respect to time and 
-        #fov indices in the hdf5 file
-        self.fovlabels = []
-        self.tlabels = []        
-        self.InitLabels()
-        
-        self.default_channel = 0
-        self.name = self.hdfpath
-                            
-        # create an new hfd5 file if no one existing already
-        self.Inithdf()
-
-        
-    def InitLabels(self):
-        """Create two lists containing all the possible fields of view and time
-        labels, in order to access the arrays in the hdf5 file.
-        """
-        for i in range(0, self.Npos):
-            self.fovlabels.append('FOV' + str(i))
-        
-        for j in range(0, self.sizet):
-            self.tlabels.append('T'+ str(j))
-    
-    
-    def Inithdf(self):
-        """If the file already exists then it is loaded else 
-        a new hdf5 file is created and for every fields of view
-        a new group is created in the createhdf method
-        """
-        newFileExists = os.path.isfile(self.newhdfpath)
-        if not self.hdfpath and not newFileExists:            
-            return self.Createhdf()
-             
-        else:
-            if not self.hdfpath:
-                self.hdfpath = self.newhdfpath
-            filenamewithpath, extension = os.path.splitext(self.hdfpath)
-                
-            # If mask file is a tiff file
-            if (extension == '.tiff' or extension == '.tif' or 
-               extension == '.TIFF' or extension == '.TIF'):
-                im = skimage.io.imread(self.hdfpath)
-                imdims = im.shape
-                
-                # num pages should be smaller than x or y dimension, very unlikely not to be the case
-                if len(imdims) == 3 and imdims[2] < imdims[0] and imdims[2] < imdims[1]:  
-                    im = np.moveaxis(im, -1, 0) # move last axis to first
-
-                with h5py.File(filenamewithpath + '.h5', 'w') as hf:
-                    hf.create_group('FOV0')  
-        
-                    if im.ndim==2:
-                        hf.create_dataset('/FOV0/T0', data = im, compression = 'gzip')
-                    elif im.ndim==3:
-                        nim = im.shape[0]
-                        for i in range(nim):
-                            hf.create_dataset('/FOV0/T{}'.format(i), 
-                                              data = im[i,:,:], compression = 'gzip')
-
-                self.hdfpath = filenamewithpath + '.h5'
-            
-            
-    def Createhdf(self):
-        """In this method, for each field of view one group is created. And 
-        in each one of these group, there will be for each time frame a 
-        corresponding dataset equivalent to a 2d array containing the 
-        corresponding masks data (segmented/thresholded/predicted).
-        """
-                    
-        self.hdfpath = self.newhdfpath
-        
-        hf = h5py.File(self.hdfpath, 'w')
-        for i in range(0, self.Npos):
-            grpname = self.fovlabels[i]
-            hf.create_group(grpname)
-        hf.close()
-
-
-    def LoadMask(self, currentT, currentFOV):
-        """this method is called when one mask should be loaded from the file 
-        on the disk to the user's buffer. If there is no mask corresponding
-        in the file, it creates the mask corresponding to the given time and 
-        field of view index and returns an array filled with zeros.
-        """
-        
-        file = h5py.File(self.hdfpath,'r+')
-        if self.TestTimeExist(currentT,currentFOV,file):
-            mask = np.array(file['/{}/{}'.format(self.fovlabels[currentFOV], self.tlabels[currentT])], dtype = np.uint16)
-            log.debug('load mask')
-            file.close()
-            
-            return mask
-        
-        else:
-            zeroarray = np.zeros([self.sizey, self.sizex],dtype = np.uint16)
-            file.create_dataset('/{}/{}'.format(self.fovlabels[currentFOV], self.tlabels[currentT]), 
-                                data = zeroarray, compression = 'gzip')
-            log.debug('create dataset with zeroarray')
-            file.close()
-            return zeroarray
-            
-            
-    def TestTimeExist(self, currentT, currentFOV, file=None):
-        """This method tests if the array which is requested by LoadMask
-        already exists or not in the hdf file.
-        
-        If file is None, then it opens the h5py File. Otherwise allows to pass
-        an already open file. 
-        """
-        def closefile(f):
-            if file is None:
-                f.close()
-                
-        def openfile(file):
-            if file is None:
-                return h5py.File(self.hdfpath, 'r+')
-            else:
-                return file
-                            
-        if currentT <= len(self.tlabels) - 1 and currentT >= 0:
-            f = openfile(file)
-            for t in f['/{}'.format(self.fovlabels[currentFOV])].keys():
-                # currentT is a number
-                # self.tlabels is some string that indexes the time point? E.g., T0?
-                if t == self.tlabels[currentT]:
-                    closefile(f)
-                    return True
-            closefile(f)
-            return False
-        else:
-            return False
-
-            
-    def SaveMask(self, currentT, currentFOV, mask):
-        """This function is called when the user wants to save the mask in the
-        hdf5 file on the disk. It overwrites the existing array with the new 
-        one given in argument. 
-        If it is a new mask, there should already
-        be an existing null array which has been created by the LoadMask method
-        when the new array has been loaded/created in the main before calling
-        this save method.
-        """
-        
-        file = h5py.File(self.hdfpath, 'r+')
-        
-        if self.TestTimeExist(currentT,currentFOV,file):
-            dataset= file['/{}/{}'.format(self.fovlabels[currentFOV], self.tlabels[currentT])]
-            dataset[:] = mask
-            log.debug('save mask for FOV {} and frame {} to file'.format(self.fovlabels[currentFOV], self.tlabels[currentT]))
-            file.close()
-            
-        else:
-            file.create_dataset('/{}/{}'.format(self.fovlabels[currentFOV], self.tlabels[currentT]), data = mask, compression = 'gzip')
-            log.debug('create dateset and save mask to file')
-            file.close()
-        
-        
-    def TestIndexRange(self,currentT, currentfov):
-        """this method receives the time and the fov index and checks
-        if it is present in the images data.
-        """
-        
-        if currentT < (self.sizet-1) and currentfov < self.Npos:
-            return True
-        if currentT == self.sizet - 1 and currentfov < self.Npos:
-            return False
-
-
-    def LoadOneImage(self,currentT, currentfov):
-        """This method returns from the nd2 file, the picture requested by the 
-        main program as an array. It fixes the fov index and iterates over the 
-        time index.
-        """
-        if not (currentT < self.sizet and currentfov < self.Npos):
-            return None
-        
-        if self.isnd2:
-            with ND2Reader(self.nd2path) as images:
-                try:
-                    images.default_coords['v'] = currentfov
-                except ValueError:
-                    pass
-                try:
-                    images.default_coords['c'] = self.default_channel
-                except ValueError:
-                    pass
-                images.iter_axes = 't'
-                im = images[currentT]
-                
-        elif self.issingle:
-#            with pytiff.Tiff(self.nd2path) as handle:
-#                handle.set_page(currentT)
-#                im = handle[:]
-            full = skimage.io.imread(self.nd2path)
-            if full.ndim==2:
-                im = full
-            elif full.ndim==3:
-                # num pages should be smaller than x or y dimension, very unlikely not to be the case
-                if full.shape[2] < full.shape[0] and full.shape[2] < full.shape[1]:  
-                    full = np.moveaxis(full, -1, 0) # move last axis to first
-                im = full[currentT]
-
-                                
-        elif self.isfolder:
-            filelist = sorted(os.listdir(self.nd2path))
-            for f in filelist:
-                if f.startswith('.'):
-                    filelist.remove(f)
-            im = skimage.io.imread(os.path.join(self.nd2path , filelist[currentT]))
-            im = np.pad(im,( (0, self.sizey - im.shape[0]) , (0, self.sizex -  im.shape[1] ) ),constant_values=0) # pad with zeros so all images in the same folder have same size
-            
-        outputarray = np.array(im, dtype = np.uint16)
-        return outputarray
-
-    
-    def LoadImageChannel(self,currentT, currentFOV, ch):
-        """Loads image at specified time, FOV and channel. Only for nd2 files"""
-        if self.isnd2:
-            with ND2Reader(self.nd2path) as images:
-                try:
-                    images.default_coords['v'] = currentFOV
-                except ValueError:
-                    pass
-                try:
-                    images.iter_axes = 'c'
-                except ValueError:
-                    pass
-                images.default_coords['t'] = currentT
-                im = images[ch]
-                return np.array(im)
-        
-        elif self.issingle:
-            return self.LoadOneImage(currentT, currentFOV)
-                
-        elif self.isfolder:
-            return self.LoadOneImage(currentT, currentFOV)
-
-
-    def CellCorrespondence(self, currentT, currentFOV):
-        """Performs tracking, handles loading of the images. If the image to 
-        track has no precedent, returns unaltered mask. If no mask exists
-        for the current timeframe, returns zero array."""
-        filemasks = h5py.File(self.hdfpath, 'r+')
-        log.debug('Reader.CellCorrespondence')
-        
-        if self.TestTimeExist(currentT-1, currentFOV, filemasks):
-            prevmask = np.array(filemasks['/{}/{}'.format(self.fovlabels[currentFOV], 
-                                                          self.tlabels[currentT-1])])
-            # A mask exists for both time frames
-            if self.TestTimeExist(currentT, currentFOV, filemasks):
-                nextmask = np.array(filemasks['/{}/{}'.format(self.fovlabels[currentFOV],
-                                                              self.tlabels[currentT])])             
-                newmask = hu.correspondence(prevmask, nextmask)
-                out = newmask
-                log.debug('make new mask')
-            # No mask exists for the current timeframe, return empty array
-            else:
-                null = np.zeros([self.sizey, self.sizex])
-                log.warn('No mask exists in FOV {} for the current timeframe {}, return empty array'.format(self.fovlabels[currentFOV],self.tlabels[currentT-1]))
-                out = null
-        
-        else:
-            # Current mask exists, but no previous - returns current mask unchanged
-            if self.TestTimeExist(currentT, currentFOV, filemasks):
-                nextmask = np.array(filemasks['/{}/{}'.format(self.fovlabels[currentFOV],
-                                                              self.tlabels[currentT])]) 
-                out = nextmask
-                log.warn('NCurrent mask exists, but no previous - returns current mask unchanged. FOV {} and Time {}'.format(self.fovlabels[currentFOV],self.tlabels[currentT-1]))
-            # Neither current nor previous mask exists - return empty array
-            else:
-                log.warn('Neither current nor previous mask exists - return empty array. FOV {} and Time {}'.format(self.fovlabels[currentFOV],self.tlabels[currentT-1]))
-                null = np.zeros([self.sizey, self.sizex])
-                out = null
-                    
-        filemasks.close()
-        return out
-                
-                
-                
-        
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Oct 15 15:00:29 2019
+
+This file handles all interactions with the hdf and image files, such as 
+loading or saving a particular image.
+"""
+from nd2reader import ND2Reader
+import numpy as np
+import re
+import h5py
+import os.path
+import skimage
+import skimage.io
+
+from ..unet import hungarian as hu
+import logging
+import os
+logging.basicConfig(
+    format='%(asctime)s %(levelname)s %(funcName)s: %(message)s',
+    level=os.environ.get("LOGLEVEL", "WARNING")
+)
+log = logging.getLogger(__name__)
+
+
+class Reader:
+    
+    
+    def __init__(self, hdfpathname, newhdfname, nd2pathname):
+        """
+        Initializes the data corresponding to the sizes of the pictures,
+        the number of different fields of views(Npos) taken in the experiment.
+        And it also sets the number of time frames per field of view.
+        """
+        # Identify filetype of image file
+        _, self.extension = os.path.splitext(nd2pathname)
+        self.isnd2 = self.extension == '.nd2'
+        self.isfolder = self.extension == ''
+        self.issingle = self.extension in ['.tif','.tiff',
+                                            '.jpg','.jpeg','.png','.bmp',
+                                           '.pbm','.pgm','.ppm','.pxm','.pnm','.jp2',
+                                           '.TIF','.TIFF',
+                                            '.JPG','.JPEG','.PNG','.BMP',
+                                           '.PBM','.PGM','.PPM','.PXM','.PNM','.JP2']
+        
+        self.nd2path = nd2pathname # path name is nd2path for legacy reasons
+        self.hdfpath = hdfpathname
+        self.newhdfpath = newhdfname
+        
+        if self.isnd2:
+            with ND2Reader(self.nd2path) as images:
+                self.sizex = images.sizes['x']
+                self.sizey = images.sizes['y']
+                self.sizet = images.sizes['t']
+                try:
+                    self.sizec = images.sizes['c']
+                except KeyError:
+                    self.sizec = 1
+                try:
+                    self.Npos  = images.sizes['v']
+                except KeyError:
+                    self.Npos  = 1
+                self.channel_names = images.metadata['channels']
+                
+        elif self.issingle:
+#            with pytiff.Tiff(self.nd2path) as handle:
+#                self.sizey, self.sizex = handle.shape #SJR: changed by me
+#                self.sizec = 1
+#                self.sizet = handle.number_of_pages
+#                self.Npos = 1
+#                self.channel_names = ['Channel1']
+            im = skimage.io.imread(self.nd2path)
+
+            if im.ndim==3:
+                # num pages should be smaller than x or y dimension, very unlikely not to be the case
+                if im.shape[2] < im.shape[0] and im.shape[2] < im.shape[1]:  
+                    im = np.moveaxis(im, -1, 0) # move last axis to first
+                self.sizet, self.sizey, self.sizex = im.shape
+            else:
+                self.sizey, self.sizex = im.shape
+                self.sizet = 1
+                
+            self.Npos = 1
+            self.channel_names = ['Channel1']
+                
+        elif self.isfolder:
+            filelist = sorted(os.listdir(self.nd2path))  
+            # filter filelist for supported image files
+            filelist = [f for f in filelist if re.search(r".png|.tif|.jpg|.bmp|.jpeg|.pbm|.pgm|.ppm|.pxm|.pnm|.jp2"
+                                                         "|.PNG|.TIF|.JPG|.BMP|.JPEG|.PBM|.PGM|.PPM|.PXM|.PNM|.JP2", f)]          
+            for f in filelist:
+                if f.startswith('.'):
+                    filelist.remove(f)
+            self.sizey = 0
+            self.sizex = 0
+            self.sizec = 1
+            self.Npos = 1
+            self.sizet = len(filelist)
+            
+            for f in filelist:
+                im = skimage.io.imread(os.path.join(self.nd2path , f))
+                if im.ndim==3:
+                    self.sizec = max(self.sizec, im.shape[0])
+                    self.sizey = max(self.sizey, im.shape[1]) #SJR: changed by me
+                    self.sizex = max(self.sizex, im.shape[2]) #SJR: changed by me
+                else:
+                    self.sizey = max(self.sizey, im.shape[0]) #SJR: changed by me
+                    self.sizex = max(self.sizex, im.shape[1]) #SJR: changed by me
+
+            self.channel_names = [f'Channel{i}' for i in range(1,self.sizec+1)]
+
+        #create the labels which index the masks with respect to time and 
+        #fov indices in the hdf5 file
+        self.fovlabels = []
+        self.tlabels = []        
+        self.InitLabels()
+        
+        self.default_channel = 0
+        self.name = self.hdfpath
+                            
+        # create an new hfd5 file if no one existing already
+        self.Inithdf()
+
+        
+    def InitLabels(self):
+        """Create two lists containing all the possible fields of view and time
+        labels, in order to access the arrays in the hdf5 file.
+        """
+        for i in range(0, self.Npos):
+            self.fovlabels.append('FOV' + str(i))
+        
+        for j in range(0, self.sizet):
+            self.tlabels.append('T'+ str(j))
+    
+    
+    def Inithdf(self):
+        """If the file already exists then it is loaded else 
+        a new hdf5 file is created and for every fields of view
+        a new group is created in the createhdf method
+        """
+        newFileExists = os.path.isfile(self.newhdfpath)
+        if not self.hdfpath and not newFileExists:            
+            return self.Createhdf()
+             
+        else:
+            if not self.hdfpath:
+                self.hdfpath = self.newhdfpath
+            filenamewithpath, extension = os.path.splitext(self.hdfpath)
+                
+            # If mask file is a tiff file
+            if (extension == '.tiff' or extension == '.tif' or 
+               extension == '.TIFF' or extension == '.TIF'):
+                im = skimage.io.imread(self.hdfpath)
+                imdims = im.shape
+                
+                # num pages should be smaller than x or y dimension, very unlikely not to be the case
+                if len(imdims) == 3 and imdims[2] < imdims[0] and imdims[2] < imdims[1]:  
+                    im = np.moveaxis(im, -1, 0) # move last axis to first
+
+                with h5py.File(filenamewithpath + '.h5', 'w') as hf:
+                    hf.create_group('FOV0')  
+        
+                    if im.ndim==2:
+                        hf.create_dataset('/FOV0/T0', data = im, compression = 'gzip')
+                    elif im.ndim==3:
+                        nim = im.shape[0]
+                        for i in range(nim):
+                            hf.create_dataset('/FOV0/T{}'.format(i), 
+                                              data = im[i,:,:], compression = 'gzip')
+
+                self.hdfpath = filenamewithpath + '.h5'
+            
+            
+    def Createhdf(self):
+        """In this method, for each field of view one group is created. And 
+        in each one of these group, there will be for each time frame a 
+        corresponding dataset equivalent to a 2d array containing the 
+        corresponding masks data (segmented/thresholded/predicted).
+        """
+                    
+        self.hdfpath = self.newhdfpath
+        
+        hf = h5py.File(self.hdfpath, 'w')
+        for i in range(0, self.Npos):
+            grpname = self.fovlabels[i]
+            hf.create_group(grpname)
+        hf.close()
+
+
+    def LoadMask(self, currentT, currentFOV):
+        """this method is called when one mask should be loaded from the file 
+        on the disk to the user's buffer. If there is no mask corresponding
+        in the file, it creates the mask corresponding to the given time and 
+        field of view index and returns an array filled with zeros.
+        """
+        
+        file = h5py.File(self.hdfpath,'r+')
+        if self.TestTimeExist(currentT,currentFOV,file):
+            mask = np.array(file['/{}/{}'.format(self.fovlabels[currentFOV], self.tlabels[currentT])], dtype = np.uint16)
+            log.debug('load mask')
+            file.close()
+            
+            return mask
+        
+        else:
+            zeroarray = np.zeros([self.sizey, self.sizex],dtype = np.uint16)
+            file.create_dataset('/{}/{}'.format(self.fovlabels[currentFOV], self.tlabels[currentT]), 
+                                data = zeroarray, compression = 'gzip')
+            log.debug('create dataset with zeroarray')
+            file.close()
+            return zeroarray
+            
+            
+    def TestTimeExist(self, currentT, currentFOV, file=None):
+        """This method tests if the array which is requested by LoadMask
+        already exists or not in the hdf file.
+        
+        If file is None, then it opens the h5py File. Otherwise allows to pass
+        an already open file. 
+        """
+        def closefile(f):
+            if file is None:
+                f.close()
+                
+        def openfile(file):
+            if file is None:
+                return h5py.File(self.hdfpath, 'r+')
+            else:
+                return file
+                            
+        if currentT <= len(self.tlabels) - 1 and currentT >= 0:
+            f = openfile(file)
+            for t in f['/{}'.format(self.fovlabels[currentFOV])].keys():
+                # currentT is a number
+                # self.tlabels is some string that indexes the time point? E.g., T0?
+                if t == self.tlabels[currentT]:
+                    closefile(f)
+                    return True
+            closefile(f)
+            return False
+        else:
+            return False
+
+            
+    def SaveMask(self, currentT, currentFOV, mask):
+        """This function is called when the user wants to save the mask in the
+        hdf5 file on the disk. It overwrites the existing array with the new 
+        one given in argument. 
+        If it is a new mask, there should already
+        be an existing null array which has been created by the LoadMask method
+        when the new array has been loaded/created in the main before calling
+        this save method.
+        """
+        
+        file = h5py.File(self.hdfpath, 'r+')
+        
+        if self.TestTimeExist(currentT,currentFOV,file):
+            dataset= file['/{}/{}'.format(self.fovlabels[currentFOV], self.tlabels[currentT])]
+            dataset[:] = mask
+            log.debug('save mask for FOV {} and frame {} to file'.format(self.fovlabels[currentFOV], self.tlabels[currentT]))
+            file.close()
+            
+        else:
+            file.create_dataset('/{}/{}'.format(self.fovlabels[currentFOV], self.tlabels[currentT]), data = mask, compression = 'gzip')
+            log.debug('create dateset and save mask to file')
+            file.close()
+        
+        
+    def TestIndexRange(self,currentT, currentfov):
+        """this method receives the time and the fov index and checks
+        if it is present in the images data.
+        """
+        
+        if currentT < (self.sizet-1) and currentfov < self.Npos:
+            return True
+        if currentT == self.sizet - 1 and currentfov < self.Npos:
+            return False
+
+
+    def LoadOneImage(self,currentT, currentfov):
+        """This method returns from the nd2 file, the picture requested by the 
+        main program as an array. It fixes the fov index and iterates over the 
+        time index.
+        """
+        if not (currentT < self.sizet and currentfov < self.Npos):
+            return None
+        
+        if self.isnd2:
+            with ND2Reader(self.nd2path) as images:
+                try:
+                    images.default_coords['v'] = currentfov
+                except ValueError:
+                    pass
+                try:
+                    images.default_coords['c'] = self.default_channel
+                except ValueError:
+                    pass
+                images.iter_axes = 't'
+                im = images[currentT]
+                outputarray = np.array(im, dtype = np.uint16)
+                return outputarray
+
+                
+        elif self.issingle:
+            full = skimage.io.imread(self.nd2path)
+            if full.ndim==2:
+                im = full
+            elif full.ndim==3:
+                # num pages should be smaller than x or y dimension, very unlikely not to be the case
+                if full.shape[2] < full.shape[0] and full.shape[2] < full.shape[1]:  
+                    full = np.moveaxis(full, -1, 0) # move last axis to first
+                im = full[currentT]
+
+            outputarray = np.array(im, dtype = np.uint16)
+            return outputarray
+
+                                
+        elif self.isfolder:
+            filelist = sorted(os.listdir(self.nd2path))
+            # filter filelist for supported image files
+            filelist = [f for f in filelist if re.search(r".png|.tif|.jpg|.bmp|.jpeg|.pbm|.pgm|.ppm|.pxm|.pnm|.jp2"
+                                                         "|.PNG|.TIF|.JPG|.BMP|.JPEG|.PBM|.PGM|.PPM|.PXM|.PNM|.JP2", f)]
+            for f in filelist:
+                if f.startswith('.'):
+                    filelist.remove(f)
+            
+            im = skimage.io.imread(os.path.join(self.nd2path , filelist[currentT]))
+            if im.ndim==2:
+                im = np.pad(im,( (0, self.sizey - im.shape[0]) , (0, self.sizex -  im.shape[1] ) ),constant_values=0) # pad with zeros so all images in the same folder have same size
+                outputarray = np.array(im, dtype = np.uint16)
+            elif im.ndim ==3:
+                im = np.pad(im,( (0, self.sizec - im.shape[0]) , (0, self.sizey - im.shape[1]) , (0, self.sizex -  im.shape[2] ) ),constant_values=0)
+                # number of channels should be smaller than x and y
+                if im.shape[2] < im.shape[0] and im.shape[2] < im.shape[1]:  
+                    im = np.moveaxis(im, -1, 0) # move last axis to first
+                im = im[self.default_channel]
+                outputarray = np.array(im, dtype = np.uint16)
+            else:
+                outputarray = np.zeros([self.sizey, self.sizex],dtype = np.uint16)
+                print("Error: image has wrong number of dimensions")
+            return outputarray              
+
+    
+    def LoadImageChannel(self,currentT, currentFOV, ch):
+        """Loads image at specified time, FOV and channel. Only for nd2 files"""
+        if self.isnd2:
+            with ND2Reader(self.nd2path) as images:
+                try:
+                    images.default_coords['v'] = currentFOV
+                except ValueError:
+                    pass
+                try:
+                    images.iter_axes = 'c'
+                except ValueError:
+                    pass
+                images.default_coords['t'] = currentT
+                im = images[ch]
+                return np.array(im)
+        
+        elif self.issingle:
+            return self.LoadOneImage(currentT, currentFOV)
+                
+        elif self.isfolder:
+            return self.LoadOneImage(currentT, currentFOV)
+
+
+    def CellCorrespondence(self, currentT, currentFOV):
+        """Performs tracking, handles loading of the images. If the image to 
+        track has no precedent, returns unaltered mask. If no mask exists
+        for the current timeframe, returns zero array."""
+        filemasks = h5py.File(self.hdfpath, 'r+')
+        log.debug('Reader.CellCorrespondence')
+        
+        if self.TestTimeExist(currentT-1, currentFOV, filemasks):
+            prevmask = np.array(filemasks['/{}/{}'.format(self.fovlabels[currentFOV], 
+                                                          self.tlabels[currentT-1])])
+            # A mask exists for both time frames
+            if self.TestTimeExist(currentT, currentFOV, filemasks):
+                nextmask = np.array(filemasks['/{}/{}'.format(self.fovlabels[currentFOV],
+                                                              self.tlabels[currentT])])             
+                newmask = hu.correspondence(prevmask, nextmask)
+                out = newmask
+                log.debug('make new mask')
+            # No mask exists for the current timeframe, return empty array
+            else:
+                null = np.zeros([self.sizey, self.sizex])
+                log.warn('No mask exists in FOV {} for the current timeframe {}, return empty array'.format(self.fovlabels[currentFOV],self.tlabels[currentT-1]))
+                out = null
+        
+        else:
+            # Current mask exists, but no previous - returns current mask unchanged
+            if self.TestTimeExist(currentT, currentFOV, filemasks):
+                nextmask = np.array(filemasks['/{}/{}'.format(self.fovlabels[currentFOV],
+                                                              self.tlabels[currentT])]) 
+                out = nextmask
+                log.warn('NCurrent mask exists, but no previous - returns current mask unchanged. FOV {} and Time {}'.format(self.fovlabels[currentFOV],self.tlabels[currentT-1]))
+            # Neither current nor previous mask exists - return empty array
+            else:
+                log.warn('Neither current nor previous mask exists - return empty array. FOV {} and Time {}'.format(self.fovlabels[currentFOV],self.tlabels[currentT-1]))
+                null = np.zeros([self.sizey, self.sizex])
+                out = null
+                    
+        filemasks.close()
+        return out
+                
+                
+                
+
```

### Comparing `YeaZ-1.0.0rc1/yeaz/icons/HomeIcon.png` & `YeaZ-1.0.1/yeaz/icons/HomeIcon.png`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.0rc1/yeaz/icons/MoveArrowsIcon.png` & `YeaZ-1.0.1/yeaz/icons/MoveArrowsIcon.png`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.0rc1/yeaz/icons/brush2.png` & `YeaZ-1.0.1/yeaz/icons/brush2.png`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.0rc1/yeaz/icons/eraser.png` & `YeaZ-1.0.1/yeaz/icons/eraser.png`

 * *Files identical despite different names*

### Comparing `YeaZ-1.0.0rc1/yeaz/init/InitButtons.py` & `YeaZ-1.0.1/yeaz/init/InitButtons.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,246 +1,246 @@
-# -*- coding: utf-8 -*-
-"""
-Initializing all the buttons in this file.
-"""
-from PyQt6.QtWidgets import QPushButton, QComboBox, QLineEdit
-from PyQt6 import QtGui
-from PyQt6.QtCore import Qt
-from PyQt6.QtGui import QKeySequence
-
-import numpy as np
-import os
-import sys
-#in case the app is frozen, the original path cannot find the icons.
-if getattr(sys, 'frozen', False):
-    path_icons = os.path.join(sys._MEIPASS, "icons/")
-    
-else:
-    path_icons = './icons/'
-
-
-def Init(parent):
-    """
-    configuration of all the buttons, some buttons just need to be toggled
-    meaning that they need just to be clicked and the function associated 
-    to the button is called and executed. Other buttons are checkable 
-    meaning that until the user has not finished to use the function
-    connected to the button, this button stays active (or Checked)
-    """
-
-    # hide / show cnn buttons
-    parent.button_hide_show.setCheckable(True)    
-    parent.button_hide_show.setMaximumWidth(150)
-    parent.button_hide_show.clicked.connect(parent.ShowHideCNNbuttons)
-    parent.button_hide_show.setStatusTip('Press to hide and show neural network buttons.')
-
-    # ADD REGION
-    parent.button_add_region.setCheckable(True)
-    parent.button_add_region.setMaximumWidth(150)
-    parent.button_add_region.clicked.connect(parent.clickmethod)
-    parent.button_add_region.setShortcut("R")
-    parent.button_add_region.setToolTip("Shortcut: R key")
-    parent.button_add_region.setStatusTip('First left click identifies the ID value for the cell (or background) to be extended, then left-click to specify a polygon.')
-    
-    # NEW CELL
-    parent.button_newcell.setCheckable(True)
-    parent.button_newcell.setMaximumWidth(150)
-    parent.button_newcell.setShortcut("N")
-    parent.button_newcell.setToolTip("Shortcut: N key")
-    parent.button_newcell.clicked.connect(parent.ClickNewCell)
-    parent.button_newcell.setStatusTip('Use left clicks to produce a polygon with a new cell ID value.')
-    
-    # NEXT FRAME (TIME AXIS)
-    parent.button_nextframe.toggle()
-    parent.button_nextframe.pressed.connect(parent.ChangeNextFrame)
-    parent.button_nextframe.setToolTip("Shortcut: right arrow (->)")
-    parent.button_nextframe.setMaximumWidth(150)
-    parent.button_nextframe.setShortcut(Qt.Key.Key_Right)
-
-
-    
-    # if there is only one picture than this button is disabled
-    if np.all(parent.nextframe == 0):
-        parent.button_nextframe.setEnabled(False)    
-    
-    # PREVIOUS FRAME (TIME AXIS)
-    parent.button_previousframe.setEnabled(False)
-    parent.button_previousframe.toggle()
-    parent.button_previousframe.pressed.connect(parent.ChangePreviousFrame)
-    parent.button_previousframe.setToolTip("Shortcut: left arrow (<-)")
-    parent.button_previousframe.setMaximumWidth(150)
-    parent.button_previousframe.setShortcut(Qt.Key.Key_Left)
-    parent.button_previousframe.move(100,100)
-        
-    # ZOOM
-    parent.button_zoom = QPushButton()
-    parent.button_zoom.clicked.connect(parent.ZoomTlbar)
-    parent.button_zoom.setIcon(QtGui.QIcon(path_icons+'ZoomIcon.png'))
-    parent.button_zoom.setMaximumWidth(30)
-    parent.button_zoom.setMaximumHeight(30)
-    parent.button_zoom.setStyleSheet("QPushButton:hover { background-color: blue }" )
-    parent.button_zoom.setCheckable(True)
-    parent.button_zoom.setShortcut("Z")
-    parent.button_zoom.setToolTip("Shortcut: Z")
-    parent.button_zoom.setStatusTip('Zoom (draw rectangle with right mouse button to zoom out)')
-    parent.buttonlist.append(parent.button_zoom)
-    
-    # HOME
-    parent.button_home = QPushButton()
-    parent.button_home.clicked.connect(parent.HomeTlbar)
-    parent.button_home.setIcon(QtGui.QIcon(path_icons+'HomeIcon.png'))
-    parent.button_home.setMaximumWidth(30)
-    parent.button_home.setMaximumHeight(30)
-    parent.button_home.setStyleSheet("QPushButton:hover { background-color: blue }" )
-    parent.button_home.setShortcut("H")
-    parent.button_home.setToolTip("Shortcut: H")
-    parent.button_home.setStatusTip('Reset zoom')
-    parent.buttonlist.append(parent.button_home)
-    
-    # PREVIOUS SCALE (ZOOM SCALE)
-    parent.button_back = QPushButton()
-    parent.button_back.clicked.connect(parent.BackTlbar)
-    parent.button_back.setIcon(QtGui.QIcon(path_icons+'LeftArrowIcon.png'))
-    parent.button_back.setMaximumWidth(30)
-    parent.button_back.setMaximumHeight(30)
-    parent.button_back.setStyleSheet("QPushButton:hover { background-color: blue }" )
-    parent.button_back.setStatusTip('Go back to previous view (undo).')
-    parent.buttonlist.append(parent.button_back)
-    
-    # NEXT SCALE (ZOOM SCALE)
-    parent.button_forward = QPushButton()
-    parent.button_forward.clicked.connect(parent.ForwardTlbar)
-    parent.button_forward.setIcon(QtGui.QIcon(path_icons+'RightArrowIcon.png'))
-    parent.button_forward.setMaximumWidth(30)
-    parent.button_forward.setMaximumHeight(30)
-    parent.button_forward.setStyleSheet("QPushButton:hover { background-color: blue }")
-    parent.button_forward.setStatusTip('Go to next view (redo).')
-    parent.buttonlist.append(parent.button_forward)
-    
-    # PAN 
-    parent.button_pan = QPushButton()
-    parent.button_pan.clicked.connect(parent.PanTlbar)
-    parent.button_pan.setIcon(QtGui.QIcon(path_icons+'MoveArrowsIcon.png'))
-    parent.button_pan.setMaximumWidth(30)
-    parent.button_pan.setMaximumHeight(30)
-    parent.button_pan.setStyleSheet("QPushButton:hover { background-color: blue }")
-    parent.button_pan.setCheckable(True)
-    parent.button_pan.setShortcut("P")
-    parent.button_pan.setToolTip("Shortcut: P")
-    parent.button_pan.setStatusTip('Pan')
-    parent.buttonlist.append(parent.button_pan)
-    
-    # BRUSH 
-    parent.button_drawmouse.setCheckable(True)
-    parent.button_drawmouse.clicked.connect(parent.MouseDraw)
-    parent.button_drawmouse.setToolTip("Shortcut: B")
-    parent.button_drawmouse.setShortcut("B")
-    parent.button_drawmouse.setMaximumWidth(150)
-    parent.button_drawmouse.setStatusTip('Right click to select a cell ID value, then draw with left mouse button.')
-    
-    # ERASER
-    parent.button_eraser.setCheckable(True)
-    parent.button_eraser.clicked.connect(parent.MouseDraw)
-    parent.button_eraser.setToolTip("Shortcut: E")
-    parent.button_eraser.setShortcut("E")
-    parent.button_eraser.setMaximumWidth(150)
-    parent.button_eraser.setStatusTip('Drag to set values to background (=0).')
-    
-    # BRUSHSIZE
-    parent.spinbox_brushsize.setMinimum(1)
-    parent.spinbox_brushsize.setMaximumWidth(100)
-    parent.spinbox_brushsize.setValue(3)
-    
-    # EXCHANGE CELL VALUES
-    parent.button_exval.toggle()
-    parent.button_exval.setEnabled(True)
-    parent.button_exval.clicked.connect(parent.DialogBoxECV)
-    parent.button_exval.setMaximumWidth(150)
-    parent.button_exval.setStatusTip('Start dialog box for exchanging ID values between two cells.')
-
-    # CHANGE CELL VALUE
-    parent.button_changecellvalue.setCheckable(True)
-    parent.button_changecellvalue.setEnabled(True)
-    parent.button_changecellvalue.clicked.connect(parent.ChangeOneValue)
-    parent.button_changecellvalue.setMaximumWidth(150)
-    parent.button_changecellvalue.setShortcut("C")
-    parent.button_changecellvalue.setToolTip("Shortcut: C")
-#    parent.button_changecellvalue.setStatusTip('')
-    parent.button_changecellvalue.setStatusTip('Change ID value of one cell. Use left click to select one cell and enter a new ID value.')
-
-    # SPLIT CELLS
-    parent.button_split.toggle()
-    parent.button_split.setCheckable(True)
-    parent.button_split.setEnabled(True)
-    parent.button_split.clicked.connect(parent.SelectSplitCell)
-    parent.button_split.setMaximumWidth(150)
-    parent.button_split.setShortcut("X")
-    parent.button_split.setToolTip("Shortcut: X")
-    parent.button_split.setStatusTip('Split a selected cell into two. First left-click to select the cell, then draw a polygon around an area to split it off.')
-
-    # MERGE CELLS
-    parent.button_mergewithneighbors.toggle()
-    parent.button_mergewithneighbors.setCheckable(True)
-    parent.button_mergewithneighbors.setEnabled(True)
-    parent.button_mergewithneighbors.clicked.connect(parent.MergeWithNeighbors)
-    parent.button_mergewithneighbors.setMaximumWidth(150)
-    parent.button_mergewithneighbors.setShortcut("F")
-    parent.button_mergewithneighbors.setToolTip("Shortcut: F")
-    parent.button_mergewithneighbors.setStatusTip('Merge a cell with its immediate neighbors. Left-click to select the cell or right-click to abort.')
-
-    # MAKE THE CELL Correspondence
-    parent.button_cellcorrespondence.setEnabled(False)
-    parent.button_cellcorrespondence.setCheckable(True)
-    parent.button_cellcorrespondence.clicked.connect(parent.BatchCellCorresp)
-    parent.button_cellcorrespondence.setMaximumWidth(150)
-    parent.button_cellcorrespondence.setStatusTip('Retrack cell ID numbers for next frame(s) or selected next frames based on this frame.')
-        
-    # EXTRACT FLUORESCENCE IN DIFFERENT CHANNELS    
-    parent.button_extractfluorescence.setEnabled(False)
-    parent.button_extractfluorescence.toggle()
-    parent.button_extractfluorescence.clicked.connect(parent.ButtonFluo)
-    parent.button_extractfluorescence.setMaximumWidth(150)
-    parent.button_extractfluorescence.setStatusTip('Start the dialog box for exporting cell geometries and fluorescence for different channels.')
-    
-    # SHOW THE VALUES OF THE CELLS
-    parent.button_showval.stateChanged.connect(parent.m.OnShowCellID)
-    parent.button_showval.setShortcut('S')
-    parent.button_showval.setToolTip("Shortcut: S")
-        
-    # HIDE/SHOW THE MASK
-    parent.button_hidemask.stateChanged.connect(parent.m.HideMask)    
-    parent.button_hidemask.setShortcut('M')
-    parent.button_hidemask.setToolTip("Shortcut: M")
-    
-    # CHANGE TIME INDEX
-    parent.button_timeindex = QLineEdit()
-    parent.button_timeindex.setPlaceholderText('Time index 0-{}'.format(parent.reader.sizet-1))
-    parent.button_timeindex.setValidator(QtGui.QIntValidator(0,int(parent.reader.sizet-1)))
-    parent.button_timeindex.returnPressed.connect(parent.ChangeTimeFrame)
-    parent.button_timeindex.setMaximumWidth(150)
-    parent.buttonlist.append(parent.button_timeindex)
-    
-    # FIELDS OF VIEW BUTTON
-    parent.button_fov = QComboBox()
-    list_fov = []
-    for i in range(0, parent.reader.Npos):
-        list_fov.append("Field of View " + str(i+1))
-    parent.button_fov.addItems(list_fov)
-    parent.button_fov.setMaximumWidth(150)
-    parent.buttonlist.append(parent.button_fov)
-    parent.button_fov.activated.connect(parent.SelectFov)
-            
-    # CHANGE CHANNEL BUTTON
-    parent.button_channel = QComboBox()
-    parent.button_channel.addItems(parent.reader.channel_names)
-    parent.button_channel.setMaximumWidth(150)
-    parent.buttonlist.append(parent.button_channel)
-    parent.button_channel.activated.connect(parent.SelectChannel)
-        
-    # NEURAL NETWORK BUTTON
-    parent.button_cnn.setCheckable(True)
-    parent.button_cnn.pressed.connect(parent.LaunchBatchPrediction)
-    parent.button_cnn.setStatusTip("Start the dialog box for segmenting images.")
-    parent.button_cnn.setMaximumWidth(150)
-    parent.EnableCNNButtons()
-        
-
+# -*- coding: utf-8 -*-
+"""
+Initializing all the buttons in this file.
+"""
+from PyQt6.QtWidgets import QPushButton, QComboBox, QLineEdit
+from PyQt6 import QtGui
+from PyQt6.QtCore import Qt
+from PyQt6.QtGui import QKeySequence
+
+import numpy as np
+import os
+import sys
+#in case the app is frozen, the original path cannot find the icons.
+if getattr(sys, 'frozen', False):
+    path_icons = os.path.join(sys._MEIPASS, "icons/")
+    
+else:
+    path_icons = './icons/'
+
+
+def Init(parent):
+    """
+    configuration of all the buttons, some buttons just need to be toggled
+    meaning that they need just to be clicked and the function associated 
+    to the button is called and executed. Other buttons are checkable 
+    meaning that until the user has not finished to use the function
+    connected to the button, this button stays active (or Checked)
+    """
+
+    # hide / show cnn buttons
+    parent.button_hide_show.setCheckable(True)    
+    parent.button_hide_show.setMaximumWidth(150)
+    parent.button_hide_show.clicked.connect(parent.ShowHideCNNbuttons)
+    parent.button_hide_show.setStatusTip('Press to hide and show neural network buttons.')
+
+    # ADD REGION
+    parent.button_add_region.setCheckable(True)
+    parent.button_add_region.setMaximumWidth(150)
+    parent.button_add_region.clicked.connect(parent.clickmethod)
+    parent.button_add_region.setShortcut("R")
+    parent.button_add_region.setToolTip("Shortcut: R key")
+    parent.button_add_region.setStatusTip('First left click identifies the ID value for the cell (or background) to be extended, then left-click to specify a polygon.')
+    
+    # NEW CELL
+    parent.button_newcell.setCheckable(True)
+    parent.button_newcell.setMaximumWidth(150)
+    parent.button_newcell.setShortcut("N")
+    parent.button_newcell.setToolTip("Shortcut: N key")
+    parent.button_newcell.clicked.connect(parent.ClickNewCell)
+    parent.button_newcell.setStatusTip('Use left clicks to produce a polygon with a new cell ID value.')
+    
+    # NEXT FRAME (TIME AXIS)
+    parent.button_nextframe.toggle()
+    parent.button_nextframe.pressed.connect(parent.ChangeNextFrame)
+    parent.button_nextframe.setToolTip("Shortcut: right arrow (->)")
+    parent.button_nextframe.setMaximumWidth(150)
+    parent.button_nextframe.setShortcut(Qt.Key.Key_Right)
+
+
+    
+    # if there is only one picture than this button is disabled
+    if np.all(parent.nextframe == 0):
+        parent.button_nextframe.setEnabled(False)    
+    
+    # PREVIOUS FRAME (TIME AXIS)
+    parent.button_previousframe.setEnabled(False)
+    parent.button_previousframe.toggle()
+    parent.button_previousframe.pressed.connect(parent.ChangePreviousFrame)
+    parent.button_previousframe.setToolTip("Shortcut: left arrow (<-)")
+    parent.button_previousframe.setMaximumWidth(150)
+    parent.button_previousframe.setShortcut(Qt.Key.Key_Left)
+    parent.button_previousframe.move(100,100)
+        
+    # ZOOM
+    parent.button_zoom = QPushButton()
+    parent.button_zoom.clicked.connect(parent.ZoomTlbar)
+    parent.button_zoom.setIcon(QtGui.QIcon(path_icons+'ZoomIcon.png'))
+    parent.button_zoom.setMaximumWidth(30)
+    parent.button_zoom.setMaximumHeight(30)
+    parent.button_zoom.setStyleSheet("QPushButton:hover { background-color: blue }" )
+    parent.button_zoom.setCheckable(True)
+    parent.button_zoom.setShortcut("Z")
+    parent.button_zoom.setToolTip("Shortcut: Z")
+    parent.button_zoom.setStatusTip('Zoom (draw rectangle with right mouse button to zoom out)')
+    parent.buttonlist.append(parent.button_zoom)
+    
+    # HOME
+    parent.button_home = QPushButton()
+    parent.button_home.clicked.connect(parent.HomeTlbar)
+    parent.button_home.setIcon(QtGui.QIcon(path_icons+'HomeIcon.png'))
+    parent.button_home.setMaximumWidth(30)
+    parent.button_home.setMaximumHeight(30)
+    parent.button_home.setStyleSheet("QPushButton:hover { background-color: blue }" )
+    parent.button_home.setShortcut("H")
+    parent.button_home.setToolTip("Shortcut: H")
+    parent.button_home.setStatusTip('Reset zoom')
+    parent.buttonlist.append(parent.button_home)
+    
+    # PREVIOUS SCALE (ZOOM SCALE)
+    parent.button_back = QPushButton()
+    parent.button_back.clicked.connect(parent.BackTlbar)
+    parent.button_back.setIcon(QtGui.QIcon(path_icons+'LeftArrowIcon.png'))
+    parent.button_back.setMaximumWidth(30)
+    parent.button_back.setMaximumHeight(30)
+    parent.button_back.setStyleSheet("QPushButton:hover { background-color: blue }" )
+    parent.button_back.setStatusTip('Go back to previous view (undo).')
+    parent.buttonlist.append(parent.button_back)
+    
+    # NEXT SCALE (ZOOM SCALE)
+    parent.button_forward = QPushButton()
+    parent.button_forward.clicked.connect(parent.ForwardTlbar)
+    parent.button_forward.setIcon(QtGui.QIcon(path_icons+'RightArrowIcon.png'))
+    parent.button_forward.setMaximumWidth(30)
+    parent.button_forward.setMaximumHeight(30)
+    parent.button_forward.setStyleSheet("QPushButton:hover { background-color: blue }")
+    parent.button_forward.setStatusTip('Go to next view (redo).')
+    parent.buttonlist.append(parent.button_forward)
+    
+    # PAN 
+    parent.button_pan = QPushButton()
+    parent.button_pan.clicked.connect(parent.PanTlbar)
+    parent.button_pan.setIcon(QtGui.QIcon(path_icons+'MoveArrowsIcon.png'))
+    parent.button_pan.setMaximumWidth(30)
+    parent.button_pan.setMaximumHeight(30)
+    parent.button_pan.setStyleSheet("QPushButton:hover { background-color: blue }")
+    parent.button_pan.setCheckable(True)
+    parent.button_pan.setShortcut("P")
+    parent.button_pan.setToolTip("Shortcut: P")
+    parent.button_pan.setStatusTip('Pan')
+    parent.buttonlist.append(parent.button_pan)
+    
+    # BRUSH 
+    parent.button_drawmouse.setCheckable(True)
+    parent.button_drawmouse.clicked.connect(parent.MouseDraw)
+    parent.button_drawmouse.setToolTip("Shortcut: B")
+    parent.button_drawmouse.setShortcut("B")
+    parent.button_drawmouse.setMaximumWidth(150)
+    parent.button_drawmouse.setStatusTip('Right click to select a cell ID value, then draw with left mouse button.')
+    
+    # ERASER
+    parent.button_eraser.setCheckable(True)
+    parent.button_eraser.clicked.connect(parent.MouseDraw)
+    parent.button_eraser.setToolTip("Shortcut: E")
+    parent.button_eraser.setShortcut("E")
+    parent.button_eraser.setMaximumWidth(150)
+    parent.button_eraser.setStatusTip('Drag to set values to background (=0).')
+    
+    # BRUSHSIZE
+    parent.spinbox_brushsize.setMinimum(1)
+    parent.spinbox_brushsize.setMaximumWidth(100)
+    parent.spinbox_brushsize.setValue(3)
+    
+    # EXCHANGE CELL VALUES
+    parent.button_exval.toggle()
+    parent.button_exval.setEnabled(True)
+    parent.button_exval.clicked.connect(parent.DialogBoxECV)
+    parent.button_exval.setMaximumWidth(150)
+    parent.button_exval.setStatusTip('Start dialog box for exchanging ID values between two cells.')
+
+    # CHANGE CELL VALUE
+    parent.button_changecellvalue.setCheckable(True)
+    parent.button_changecellvalue.setEnabled(True)
+    parent.button_changecellvalue.clicked.connect(parent.ChangeOneValue)
+    parent.button_changecellvalue.setMaximumWidth(150)
+    parent.button_changecellvalue.setShortcut("C")
+    parent.button_changecellvalue.setToolTip("Shortcut: C")
+#    parent.button_changecellvalue.setStatusTip('')
+    parent.button_changecellvalue.setStatusTip('Change ID value of one cell. Use left click to select one cell and enter a new ID value.')
+
+    # SPLIT CELLS
+    parent.button_split.toggle()
+    parent.button_split.setCheckable(True)
+    parent.button_split.setEnabled(True)
+    parent.button_split.clicked.connect(parent.SelectSplitCell)
+    parent.button_split.setMaximumWidth(150)
+    parent.button_split.setShortcut("X")
+    parent.button_split.setToolTip("Shortcut: X")
+    parent.button_split.setStatusTip('Split a selected cell into two. First left-click to select the cell, then draw a polygon around an area to split it off.')
+
+    # MERGE CELLS
+    parent.button_mergewithneighbors.toggle()
+    parent.button_mergewithneighbors.setCheckable(True)
+    parent.button_mergewithneighbors.setEnabled(True)
+    parent.button_mergewithneighbors.clicked.connect(parent.MergeWithNeighbors)
+    parent.button_mergewithneighbors.setMaximumWidth(150)
+    parent.button_mergewithneighbors.setShortcut("F")
+    parent.button_mergewithneighbors.setToolTip("Shortcut: F")
+    parent.button_mergewithneighbors.setStatusTip('Merge a cell with its immediate neighbors. Left-click to select the cell or right-click to abort.')
+
+    # MAKE THE CELL Correspondence
+    parent.button_cellcorrespondence.setEnabled(False)
+    parent.button_cellcorrespondence.setCheckable(True)
+    parent.button_cellcorrespondence.clicked.connect(parent.BatchCellCorresp)
+    parent.button_cellcorrespondence.setMaximumWidth(150)
+    parent.button_cellcorrespondence.setStatusTip('Retrack cell ID numbers for next frame(s) or selected next frames based on this frame.')
+        
+    # EXTRACT FLUORESCENCE IN DIFFERENT CHANNELS    
+    parent.button_extractfluorescence.setEnabled(False)
+    parent.button_extractfluorescence.toggle()
+    parent.button_extractfluorescence.clicked.connect(parent.ButtonFluo)
+    parent.button_extractfluorescence.setMaximumWidth(150)
+    parent.button_extractfluorescence.setStatusTip('Start the dialog box for exporting cell geometries and fluorescence for different channels.')
+    
+    # SHOW THE VALUES OF THE CELLS
+    parent.button_showval.stateChanged.connect(parent.m.OnShowCellID)
+    parent.button_showval.setShortcut('S')
+    parent.button_showval.setToolTip("Shortcut: S")
+        
+    # HIDE/SHOW THE MASK
+    parent.button_hidemask.stateChanged.connect(parent.m.HideMask)    
+    parent.button_hidemask.setShortcut('M')
+    parent.button_hidemask.setToolTip("Shortcut: M")
+    
+    # CHANGE TIME INDEX
+    parent.button_timeindex = QLineEdit()
+    parent.button_timeindex.setPlaceholderText('Time index 0-{}'.format(parent.reader.sizet-1))
+    parent.button_timeindex.setValidator(QtGui.QIntValidator(0,int(parent.reader.sizet-1)))
+    parent.button_timeindex.returnPressed.connect(parent.ChangeTimeFrame)
+    parent.button_timeindex.setMaximumWidth(150)
+    parent.buttonlist.append(parent.button_timeindex)
+    
+    # FIELDS OF VIEW BUTTON
+    parent.button_fov = QComboBox()
+    list_fov = []
+    for i in range(0, parent.reader.Npos):
+        list_fov.append("Field of View " + str(i+1))
+    parent.button_fov.addItems(list_fov)
+    parent.button_fov.setMaximumWidth(150)
+    parent.buttonlist.append(parent.button_fov)
+    parent.button_fov.activated.connect(parent.SelectFov)
+            
+    # CHANGE CHANNEL BUTTON
+    parent.button_channel = QComboBox()
+    parent.button_channel.addItems(parent.reader.channel_names)
+    parent.button_channel.setMaximumWidth(150)
+    parent.buttonlist.append(parent.button_channel)
+    parent.button_channel.activated.connect(parent.SelectChannel)
+        
+    # NEURAL NETWORK BUTTON
+    parent.button_cnn.setCheckable(True)
+    parent.button_cnn.pressed.connect(parent.LaunchBatchPrediction)
+    parent.button_cnn.setStatusTip("Start the dialog box for segmenting images.")
+    parent.button_cnn.setMaximumWidth(150)
+    parent.EnableCNNButtons()
+        
+
```

### Comparing `YeaZ-1.0.0rc1/yeaz/init/InitLayout.py` & `YeaZ-1.0.1/yeaz/init/InitLayout.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-# -*- coding: utf-8 -*-
-"""
-Initializing the layout of the main window. It places the buttons and the 
-pictures at the desired positions.
-"""
-from matplotlib.backends.qt_compat import QtWidgets
-
-
-def Init(parent):
-
-    
-    # LAYOUT OF THE MAIN WINDOW
-    layout = QtWidgets.QVBoxLayout(parent._main)
-    
-    # LAYOUT FOR THE TOOLBAR BUTTONS
-    hbox = QtWidgets.QHBoxLayout()
-    hbox.addWidget(parent.button_home) 
-    hbox.addWidget(parent.button_back)
-    hbox.addWidget(parent.button_forward)
-    hbox.addWidget(parent.button_pan)
-    hbox.addWidget(parent.button_zoom)
-    hbox.addStretch(1)
-    layout.addLayout(hbox)
-    
-    # TIME NAVIGATION
-    hboxtimeframes = QtWidgets.QHBoxLayout()
-    hboxtimeframes.addWidget(parent.button_fov)
-    hboxtimeframes.addWidget(parent.button_channel)
-    hboxtimeframes.addStretch()
-    hboxtimeframes.addWidget(parent.button_previousframe)
-    hboxtimeframes.addWidget(parent.button_timeindex)
-    hboxtimeframes.addWidget(parent.button_nextframe)
-    hboxtimeframes.addStretch()
-    
-    # IMAGE DISPLAY
-    hlayout = QtWidgets.QHBoxLayout()
-    hlayout.addWidget(parent.m)
-    hlayout.setContentsMargins(0, 0, 0, 0)
-    layout.addLayout(hlayout)        
-    layout.addLayout(hboxtimeframes)
-    
-    # CORRECTIONS/ IMAGE EDITS       
-    hboxcorrectionsbuttons = QtWidgets.QHBoxLayout()
-    hboxcorrectionsbuttons.addWidget(parent.button_add_region)
-    hboxcorrectionsbuttons.addWidget(parent.button_newcell)
-    hboxcorrectionsbuttons.addWidget(parent.button_split)
-    hboxcorrectionsbuttons.addWidget(parent.button_mergewithneighbors)
-    hboxcorrectionsbuttons.addWidget(parent.button_drawmouse)
-    hboxcorrectionsbuttons.addWidget(parent.button_eraser)
-    hboxcorrectionsbuttons.addWidget(parent.label_brushsize)
-    hboxcorrectionsbuttons.addWidget(parent.spinbox_brushsize)
-    hboxcorrectionsbuttons.addStretch(2)
-    hboxcorrectionsbuttons.addWidget(parent.button_showval)
-    hboxcorrectionsbuttons.addWidget(parent.button_hidemask)
-    layout.addLayout(hboxcorrectionsbuttons)
-    
-    # LAYOUT FOR EDITING CELL VALUES, SHOW CELL VALUES AND HIDE MASK, CNN BUTTONS
-    hboxcellval = QtWidgets.QHBoxLayout()
-    hboxcellval.addWidget(parent.button_exval)
-    hboxcellval.addWidget(parent.button_changecellvalue)
-    hboxcellval.addWidget(parent.button_cellcorrespondence)
-    hboxcellval.addStretch(1)
-    hboxcellval.addWidget(parent.button_cnn)
-    hboxcellval.addWidget(parent.button_extractfluorescence)
-    layout.addLayout(hboxcellval)
-
+# -*- coding: utf-8 -*-
+"""
+Initializing the layout of the main window. It places the buttons and the 
+pictures at the desired positions.
+"""
+from matplotlib.backends.qt_compat import QtWidgets
+
+
+def Init(parent):
+
+    
+    # LAYOUT OF THE MAIN WINDOW
+    layout = QtWidgets.QVBoxLayout(parent._main)
+    
+    # LAYOUT FOR THE TOOLBAR BUTTONS
+    hbox = QtWidgets.QHBoxLayout()
+    hbox.addWidget(parent.button_home) 
+    hbox.addWidget(parent.button_back)
+    hbox.addWidget(parent.button_forward)
+    hbox.addWidget(parent.button_pan)
+    hbox.addWidget(parent.button_zoom)
+    hbox.addStretch(1)
+    layout.addLayout(hbox)
+    
+    # TIME NAVIGATION
+    hboxtimeframes = QtWidgets.QHBoxLayout()
+    hboxtimeframes.addWidget(parent.button_fov)
+    hboxtimeframes.addWidget(parent.button_channel)
+    hboxtimeframes.addStretch()
+    hboxtimeframes.addWidget(parent.button_previousframe)
+    hboxtimeframes.addWidget(parent.button_timeindex)
+    hboxtimeframes.addWidget(parent.button_nextframe)
+    hboxtimeframes.addStretch()
+    
+    # IMAGE DISPLAY
+    hlayout = QtWidgets.QHBoxLayout()
+    hlayout.addWidget(parent.m)
+    hlayout.setContentsMargins(0, 0, 0, 0)
+    layout.addLayout(hlayout)        
+    layout.addLayout(hboxtimeframes)
+    
+    # CORRECTIONS/ IMAGE EDITS       
+    hboxcorrectionsbuttons = QtWidgets.QHBoxLayout()
+    hboxcorrectionsbuttons.addWidget(parent.button_add_region)
+    hboxcorrectionsbuttons.addWidget(parent.button_newcell)
+    hboxcorrectionsbuttons.addWidget(parent.button_split)
+    hboxcorrectionsbuttons.addWidget(parent.button_mergewithneighbors)
+    hboxcorrectionsbuttons.addWidget(parent.button_drawmouse)
+    hboxcorrectionsbuttons.addWidget(parent.button_eraser)
+    hboxcorrectionsbuttons.addWidget(parent.label_brushsize)
+    hboxcorrectionsbuttons.addWidget(parent.spinbox_brushsize)
+    hboxcorrectionsbuttons.addStretch(2)
+    hboxcorrectionsbuttons.addWidget(parent.button_showval)
+    hboxcorrectionsbuttons.addWidget(parent.button_hidemask)
+    layout.addLayout(hboxcorrectionsbuttons)
+    
+    # LAYOUT FOR EDITING CELL VALUES, SHOW CELL VALUES AND HIDE MASK, CNN BUTTONS
+    hboxcellval = QtWidgets.QHBoxLayout()
+    hboxcellval.addWidget(parent.button_exval)
+    hboxcellval.addWidget(parent.button_changecellvalue)
+    hboxcellval.addWidget(parent.button_cellcorrespondence)
+    hboxcellval.addStretch(1)
+    hboxcellval.addWidget(parent.button_cnn)
+    hboxcellval.addWidget(parent.button_extractfluorescence)
+    layout.addLayout(hboxcellval)
+
```

### Comparing `YeaZ-1.0.0rc1/yeaz/misc/BatchRetrack.py` & `YeaZ-1.0.1/yeaz/misc/BatchRetrack.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-
-from PyQt6.QtWidgets import QApplication, QMainWindow, QMenu, QVBoxLayout, QSizePolicy, QMessageBox, QWidget, QPushButton, QComboBox, QDialog, QDialogButtonBox, QInputDialog, QLineEdit, QFormLayout, QLabel
-from PyQt6 import QtGui
-from PyQt6.QtGui import QShortcut
-from PyQt6.QtCore import pyqtSignal, QObject, Qt
-#import PyQt package, allows for GUI interactions
-
-class CustomDialog(QDialog):
-
-    def __init__(self, *args, **kwargs):
-        super(CustomDialog, self).__init__(*args, **kwargs)
-        app, = args
-        self.setWindowTitle("Retrack")
-        self.setGeometry(100,100, 500,200)
-        
-        self.entry1 = QLineEdit()
-        self.entry1.setValidator(QtGui.QIntValidator())
-        self.entry1.setMaxLength(4)
-        self.entry1.setAlignment(Qt.AlignmentFlag.AlignRight)
-        self.labeltime = QLabel("Enter a frame number between {} to {}".format(app.Tindex+1, app.reader.sizet-1))
-        flo = QFormLayout()
-        flo.addWidget(self.labeltime)
-        flo.addRow('retracking frames from {} (next frame) to '.format(app.Tindex+1), self.entry1)       
-        
-        QBtn = QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
-        
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-        flo.addWidget(self.buttonBox)
-        self.setLayout(flo)
+
+from PyQt6.QtWidgets import QApplication, QMainWindow, QMenu, QVBoxLayout, QSizePolicy, QMessageBox, QWidget, QPushButton, QComboBox, QDialog, QDialogButtonBox, QInputDialog, QLineEdit, QFormLayout, QLabel
+from PyQt6 import QtGui
+from PyQt6.QtGui import QShortcut
+from PyQt6.QtCore import pyqtSignal, QObject, Qt
+#import PyQt package, allows for GUI interactions
+
+class CustomDialog(QDialog):
+
+    def __init__(self, *args, **kwargs):
+        super(CustomDialog, self).__init__(*args, **kwargs)
+        app, = args
+        self.setWindowTitle("Retrack")
+        self.setGeometry(100,100, 500,200)
+        
+        self.entry1 = QLineEdit()
+        self.entry1.setValidator(QtGui.QIntValidator())
+        self.entry1.setMaxLength(4)
+        self.entry1.setAlignment(Qt.AlignmentFlag.AlignRight)
+        self.labeltime = QLabel("Enter a frame number between {} to {}".format(app.Tindex+1, app.reader.sizet-1))
+        flo = QFormLayout()
+        flo.addWidget(self.labeltime)
+        flo.addRow('retracking frames from {} (next frame) to '.format(app.Tindex+1), self.entry1)       
+        
+        QBtn = QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
+        
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+        flo.addWidget(self.buttonBox)
+        self.setLayout(flo)
```

### Comparing `YeaZ-1.0.0rc1/yeaz/misc/ChangeOneCellValue.py` & `YeaZ-1.0.1/yeaz/misc/ChangeOneCellValue.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Nov 19 17:38:58 2019
-"""
-
-from PyQt6.QtWidgets import QApplication, QMainWindow, QMenu, QVBoxLayout, QSizePolicy, QMessageBox, QWidget, QPushButton, QComboBox, QDialog, QDialogButtonBox, QInputDialog, QLineEdit, QFormLayout
-from PyQt6 import QtGui
-from PyQt6.QtGui import QShortcut
-from PyQt6.QtCore import pyqtSignal, QObject, Qt
-#import PyQt package, allows for GUI interactions
-
-class CustomDialog(QDialog):
-
-    def __init__(self, *args, **kwargs):
-        super(CustomDialog, self).__init__(*args, **kwargs)
-        
-        self.setWindowTitle("Change Value one cell")
-        self.setGeometry(100,100, 500,200)
-        
-        self.entry1 = QLineEdit()
-        self.entry1.setValidator(QtGui.QIntValidator())
-        self.entry1.setMaxLength(4)
-        self.entry1.setAlignment(Qt.AlignmentFlag.AlignRight)
-
-        
-#        self.entry2 = QLineEdit()
-#        self.entry2.setValidator(QtGui.QIntValidator())
-#        self.entry2.setMaxLength(4)
-#        self.entry2.setAlignment(Qt.AlignmentFlag.AlignRight)
-        
-        flo = QFormLayout()
-        flo.addRow('Enter Cell value (integer):', self.entry1)
-#        flo.addRow('Enter Cell value 2 (integer):', self.entry2)        
-        
-        QBtn = QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
-        
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-#        self.layout = QVBoxLayout()
-#        self.layout.addWidget(self.buttonBox
-        flo.addWidget(self.buttonBox)
-        self.setLayout(flo)
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Nov 19 17:38:58 2019
+"""
+
+from PyQt6.QtWidgets import QApplication, QMainWindow, QMenu, QVBoxLayout, QSizePolicy, QMessageBox, QWidget, QPushButton, QComboBox, QDialog, QDialogButtonBox, QInputDialog, QLineEdit, QFormLayout
+from PyQt6 import QtGui
+from PyQt6.QtGui import QShortcut
+from PyQt6.QtCore import pyqtSignal, QObject, Qt
+#import PyQt package, allows for GUI interactions
+
+class CustomDialog(QDialog):
+
+    def __init__(self, *args, **kwargs):
+        super(CustomDialog, self).__init__(*args, **kwargs)
+        
+        self.setWindowTitle("Change Value one cell")
+        self.setGeometry(100,100, 500,200)
+        
+        self.entry1 = QLineEdit()
+        self.entry1.setValidator(QtGui.QIntValidator())
+        self.entry1.setMaxLength(4)
+        self.entry1.setAlignment(Qt.AlignmentFlag.AlignRight)
+
+        
+#        self.entry2 = QLineEdit()
+#        self.entry2.setValidator(QtGui.QIntValidator())
+#        self.entry2.setMaxLength(4)
+#        self.entry2.setAlignment(Qt.AlignmentFlag.AlignRight)
+        
+        flo = QFormLayout()
+        flo.addRow('Enter Cell value (integer):', self.entry1)
+#        flo.addRow('Enter Cell value 2 (integer):', self.entry2)        
+        
+        QBtn = QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
+        
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+#        self.layout = QVBoxLayout()
+#        self.layout.addWidget(self.buttonBox
+        flo.addWidget(self.buttonBox)
+        self.setLayout(flo)
```

### Comparing `YeaZ-1.0.0rc1/yeaz/misc/ExchangeCellValues.py` & `YeaZ-1.0.1/yeaz/misc/ExchangeCellValues.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Nov 19 17:38:58 2019
-"""
-
-from PyQt6.QtWidgets import QApplication, QMainWindow, QMenu, QVBoxLayout, QSizePolicy, QMessageBox, QWidget, QPushButton, QComboBox, QDialog, QDialogButtonBox, QInputDialog, QLineEdit, QFormLayout
-from PyQt6 import QtGui
-from PyQt6.QtGui import QShortcut
-from PyQt6.QtCore import pyqtSignal, QObject, Qt
-#import PyQt package, allows for GUI interactions
-
-class CustomDialog(QDialog):
-
-    def __init__(self, *args, **kwargs):
-        super(CustomDialog, self).__init__(*args, **kwargs)
-        
-        self.setWindowTitle("Exchange Cell Values")
-        self.setGeometry(100,100, 500,200)
-        
-        self.entry1 = QLineEdit()
-        self.entry1.setValidator(QtGui.QIntValidator())
-        self.entry1.setMaxLength(4)
-        self.entry1.setAlignment(Qt.AlignmentFlag.AlignRight)
-        
-        self.entry2 = QLineEdit()
-        self.entry2.setValidator(QtGui.QIntValidator())
-        self.entry2.setMaxLength(4)
-        self.entry2.setAlignment(Qt.AlignmentFlag.AlignRight)
-        
-        flo = QFormLayout()
-        flo.addRow('Enter Cell value 1 (integer):', self.entry1)
-        flo.addRow('Enter Cell value 2 (integer):', self.entry2)        
-        
-        QBtn = QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
-        
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-#        self.layout = QVBoxLayout()
-#        self.layout.addWidget(self.buttonBox
-        flo.addWidget(self.buttonBox)
-        self.setLayout(flo)
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Nov 19 17:38:58 2019
+"""
+
+from PyQt6.QtWidgets import QApplication, QMainWindow, QMenu, QVBoxLayout, QSizePolicy, QMessageBox, QWidget, QPushButton, QComboBox, QDialog, QDialogButtonBox, QInputDialog, QLineEdit, QFormLayout
+from PyQt6 import QtGui
+from PyQt6.QtGui import QShortcut
+from PyQt6.QtCore import pyqtSignal, QObject, Qt
+#import PyQt package, allows for GUI interactions
+
+class CustomDialog(QDialog):
+
+    def __init__(self, *args, **kwargs):
+        super(CustomDialog, self).__init__(*args, **kwargs)
+        
+        self.setWindowTitle("Exchange Cell Values")
+        self.setGeometry(100,100, 500,200)
+        
+        self.entry1 = QLineEdit()
+        self.entry1.setValidator(QtGui.QIntValidator())
+        self.entry1.setMaxLength(4)
+        self.entry1.setAlignment(Qt.AlignmentFlag.AlignRight)
+        
+        self.entry2 = QLineEdit()
+        self.entry2.setValidator(QtGui.QIntValidator())
+        self.entry2.setMaxLength(4)
+        self.entry2.setAlignment(Qt.AlignmentFlag.AlignRight)
+        
+        flo = QFormLayout()
+        flo.addRow('Enter Cell value 1 (integer):', self.entry1)
+        flo.addRow('Enter Cell value 2 (integer):', self.entry2)        
+        
+        QBtn = QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
+        
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+#        self.layout = QVBoxLayout()
+#        self.layout.addWidget(self.buttonBox
+        flo.addWidget(self.buttonBox)
+        self.setLayout(flo)
```

### Comparing `YeaZ-1.0.0rc1/yeaz/misc/Extract.py` & `YeaZ-1.0.1/yeaz/misc/Extract.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,431 +1,431 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-GUI to select and deselect cells at extraction time.
-"""
-
-import sys
-import os
-import numpy as np
-from PyQt6.QtWidgets import (QApplication, QPushButton, QLabel,
-                             QHBoxLayout, QVBoxLayout, QListWidget,
-                             QFileDialog, QMessageBox, QDialog)
-from PyQt6.QtCore import Qt
-
-
-from PIL import Image, ImageDraw
-
-#Import from matplotlib to use it to display the pictures and masks.
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
-
-from matplotlib import cm
-from matplotlib.colors import LinearSegmentedColormap
-from matplotlib.figure import Figure
-
-from ..disk.image_loader import load_image
-
-class Extract(QDialog):
-    
-    
-    def __init__(self, image, mask, channel_names=[]):
-        parent = None
-        super(Extract, self).__init__(parent)
-        self.setWindowFlags(Qt.WindowType.WindowStaysOnTopHint)
-#        image, mask = _test_data()
-        self.pc = PlotCanvas(image, mask)
-        self.file_list = channel_names
-        self.init_UI()
-        self.exit_code = 0 # 0: Cancel, 1: Fluorescence, 2: Mask
-
-    def init_UI(self):
-        # Extract Buttons
-        title_extr = QLabel('Extract:')
-        self.extr_mask = _create_button("Extract mask", self.do_extr_mask)
-        self.extr_fluo = _create_button("Extract values", self.do_extr_fluo)
-        self.done = _create_button("Cancel", self.do_cancel)
-        self.done.setDefault(True)  
-        
-        extr_box = QVBoxLayout()
-        extr_box.addWidget(title_extr)
-        extr_box.addWidget(self.extr_mask)
-        extr_box.addWidget(self.extr_fluo)
-        extr_box.addWidget(self.done)
-        extr_box.setAlignment(Qt.AlignmentFlag.AlignTop)
-        
-        # Select Button
-        title_select = QLabel('Select cells:')
-        self.sel_mult = _create_button("Select multiple cells", self.do_sel_mult,
-                                       "Left-click to define the corners of a polygon around cells, "
-                                       "right-click to confirm.")
-        self.sel_sngl = _create_button("Select single cell", self.do_sel_sngl,
-                                       "Left-click to select cell, right-click "
-                                       "to abort.")
-        self.desel_mult = _create_button("Deselect multiple cells", self.do_desel_mult,
-                                       "Left-click to define the corners of a polygon around cells, "
-                                       "right-click to confirm.")
-        self.desel_sngl = _create_button("Deselect single cell", self.do_desel_sngl,
-                                       "Left-click to deselect cell, right-click "
-                                       "to abort.")
-        
-        sel_box = QVBoxLayout()
-        sel_box.addWidget(title_select)
-        sel_box.addWidget(self.sel_mult)
-        sel_box.addWidget(self.sel_sngl)
-        sel_box.addWidget(self.desel_mult)
-        sel_box.addWidget(self.desel_sngl)
-        sel_box.setAlignment(Qt.AlignmentFlag.AlignTop)
-        
-        # Additional Fluorescence File
-        file_title = QLabel("Manage files and channels for extraction:")
-        self.list_channels = QListWidget()
-        self.add_file = _create_button('Add', self.do_add_file)
-        self.remove_file = _create_button('Remove', self.do_remove_file)
-        
-        add_remove = QHBoxLayout()
-        add_remove.addWidget(self.add_file)
-        add_remove.addWidget(self.remove_file)
-        
-        manage_box = QVBoxLayout()
-        manage_box.addWidget(file_title)
-        manage_box.addWidget(self.list_channels)
-        manage_box.addLayout(add_remove)
-        manage_box.setAlignment(Qt.AlignmentFlag.AlignTop)
-        
-        # Button list
-        self.buttons = [self.extr_mask,
-                        self.extr_fluo,
-                        self.done,
-                        self.sel_mult,
-                        self.sel_sngl,
-                        self.desel_mult,
-                        self.desel_sngl,
-                        self.add_file,
-                        self.remove_file,
-                        self.list_channels]
-        
-        # Buttons
-        buttons = QHBoxLayout()
-        buttons.addLayout(sel_box)
-        buttons.addLayout(manage_box)
-        buttons.addLayout(extr_box)
-        
-        # Plot Canvas
-        full = QVBoxLayout()
-        full.addWidget(self.pc)
-        full.addStretch(.5)
-        full.addLayout(buttons)
-        
-        # Add channel list
-        self.do_show_list()
-
-        self.setLayout(full)    
-        self.setGeometry(300, 300, 600, 600)
-        self.setWindowTitle('Extract geometries, fluorescence, masks')
-        self.show()
-
-    def do_extr_fluo(self):
-        self.outfile, _ = QFileDialog.getSaveFileName(
-            self,"Specify CSV file for exporting values",
-            "","All files (*);;Text files (*.csv)")
-        _, ext = os.path.splitext(self.outfile)
-        if ext == '':
-            self.outfile += '.csv'
-        elif ext != '.csv':
-            msg_box = QMessageBox(QMessageBox.Icon.Critical,'Error','Must specify .csv file', parent=self)
-            msg_box.exec()
-            return 
-        
-        self.exit_code = 1
-        self.cells = self.pc.sellist
-        self.desel_cells = set(np.unique(self.pc.mask)) - set(self.cells)
-        self.close()
-
-    def do_cancel(self):
-        self.close()
-    
-    def do_extr_mask(self):
-        self.outfile, _ = QFileDialog.getSaveFileName(
-            self,"Specify TIFF file for exporting mask",
-            "","All files (*);;Image file (*.tiff)")
-        _, ext = os.path.splitext(self.outfile)
-        if ext == '':
-            self.outfile += '.tif'
-        elif ext != '.tif' and ext!='.tiff' and ext!='.TIF' and ext!='.TIFF':
-            msg_box = QMessageBox(QMessageBox.Icon.Critical,'Error','Must specify .tif file', parent=self)
-            msg_box.exec()
-            return 
-
-        self.exit_code = 2
-        self.cells = self.pc.sellist
-        self.desel_cells = set(np.unique(self.pc.mask)) - set(self.cells)
-        self.close()
-                
-    def do_sel_mult(self):
-        """Callback for selecting multiple"""
-        self.pc.storemouseclicks = []        
-        def to_connect(e):
-            self.pc.multiple_click(e, self.do_sel_mult_process)
-        self.pc.connect_id = self.pc.mpl_connect(
-                'button_press_event', 
-                 to_connect)
-        self.deactivate_all()
-        
-    def do_sel_mult_process(self):
-        """Process selecting multiple"""
-        cells = self.cells_in_polygon()
-        self.pc.sellist = self.pc.sellist.union(cells)
-        self.disconnect()
-        
-    def do_desel_mult(self):
-        self.pc.storemouseclicks = []        
-        """Callback for deselecting multiple"""
-        def to_connect(e):
-            self.pc.multiple_click(e, self.do_desel_mult_process)
-        self.pc.connect_id = self.pc.mpl_connect(
-                'button_press_event', 
-                 to_connect)
-        self.deactivate_all()
-        
-    def do_desel_mult_process(self):
-        """Process deselect multiple"""
-        cells = self.cells_in_polygon()
-        self.pc.sellist = self.pc.sellist - cells
-        self.disconnect()
-        
-    def cells_in_polygon(self):
-        """Extracts cells inside of polygon specified by pc.storemouseclicks"""
-        nx, ny = self.pc.mask.shape
-        img = Image.new('L', (ny, nx), 0)
-        ImageDraw.Draw(img).polygon(self.pc.storemouseclicks, outline=1, fill=1)
-        polygon = np.array(img).astype(bool)
-        return set(np.unique(self.pc.mask[polygon]))
-    
-    def do_sel_sngl(self):
-        """Select single cell"""
-        def to_connect(e):
-            self.pc.single_click(e, self.do_sel_sngl_process)
-        self.pc.connect_id = self.pc.mpl_connect(
-                'button_press_event', 
-                 to_connect)
-        self.deactivate_all()
-    
-    def do_sel_sngl_process(self, x, y):
-        """Process selected cell"""
-        if x is not None:
-            cell = self.pc.mask[y,x]
-            self.pc.sellist.add(cell)
-        self.disconnect()
-    
-    def do_desel_sngl(self):
-        """Deselect single cell"""
-        def to_connect(e):
-            self.pc.single_click(e, self.do_desel_sngl_process)
-        self.pc.connect_id = self.pc.mpl_connect(
-                'button_press_event', 
-                 to_connect)
-        self.deactivate_all()
-        
-    def do_desel_sngl_process(self, x, y):
-        """Process deselected cell"""
-        if x is not None:
-            cell = self.pc.mask[y,x]
-            self.pc.sellist.remove(cell)
-        self.disconnect()
-            
-    def disconnect(self):
-        """Disconnects callback, updates plots, activates buttons"""
-        self.pc.update_plots()
-        self.pc.mpl_disconnect(self.pc.connect_id)
-        self.activate_all()
-        
-    def deactivate_all(self):
-        for b in self.buttons:
-            b.setEnabled(False)
-            
-    def activate_all(self):
-        for b in self.buttons:
-            b.setEnabled(True)
-            
-    def do_add_file(self):
-        dlg = QFileDialog()
-        dlg.setProxyModel(None)
-        if dlg.exec():
-            full_files = dlg.selectedFiles()
-            if self.test_file(full_files):
-                self.file_list = self.file_list + full_files
-                self.do_show_list()
-    
-    def do_remove_file(self):
-        item_to_remove = self.list_channels.currentItem()
-        remove_ix = self.list_channels.row(item_to_remove)
-        self.file_list.pop(remove_ix)
-        self.do_show_list()
-    
-    def do_show_list(self):
-        self.list_channels.clear()
-        for file in self.file_list:
-            _, name = os.path.split(file)
-            self.list_channels.addItem(name)
-            
-    def test_file(self, files):
-        """Tests if input image has appropriate size and contains data"""
-        for f in files:
-            try: 
-                im = load_image(f, 0)
-            except ValueError:
-                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", "Could not load file", parent=self)
-                msg_box.exec()
-                return False
-            if not im.shape == self.pc.mask.shape:
-                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", "Loaded image has wrong size", parent=self)
-                msg_box.exec()
-                return False
-        return True
-            
-    
-
-class PlotCanvas(FigureCanvas):
-    
-    
-    def __init__(self, image, mask, parent=None, figsize=(5,4)):
-        """this class defines the canvas. It initializes a figure, which is then
-        used to plot our data using imshow.
-        """
-        fig = Figure()
-        self.ax = fig.add_subplot(111)
-        super(PlotCanvas, self).__init__(fig)
-        self.setParent(parent)
-        
-        self.image = image
-        self.mask = mask
-        self.sellist = set(np.unique(mask)) # selected cells
-        self.vismask = mask.copy() # mask with only selected cells
-        
-        self.ax_image, self.ax_mask = self.initialize_plots(image, mask, self.ax)        
-        self.storemouseclicks = []
-        self.connect_id = None
-
-    def initialize_plots(self, picture, mask, ax):
-        """Creates plots at initialization"""
-        newcmp = _colormap(21)
-        ax.axis("off")
-        self.draw()
-        return (ax.imshow(picture, interpolation= 'None', 
-                          origin = 'upper', cmap = 'gray_r'), 
-                ax.imshow((mask%10+1)*(mask != 0), origin = 'upper', 
-                          interpolation = 'None', cmap = newcmp,
-                          vmin=0, vmax=11))
-            
-    def single_click(self, event, call_after):
-        """Function for single click, calls call_after afterwards with
-        the clicked points (or None, None) if abort click."""
-        if (event.button == 1
-            and (event.xdata != None and event.ydata != None) 
-            and self.ax == event.inaxes):
-            x = int(event.xdata)
-            y = int(event.ydata)
-            call_after(x, y)
-        else:
-            call_after(None, None)
-            
-    def multiple_click(self, event, call_after):
-        """Function to keep track of multiple left clicks, confirmed with 
-        a right click. After right click, the function call_after is called"""        
-        
-        if (event.button == 1  # left click
-            and (event.xdata != None and event.ydata != None) 
-            and self.ax == event.inaxes):
-            
-            newx = int(event.xdata)
-            newy = int(event.ydata)
-            self.storemouseclicks.append((newx, newy))
-            self.draw_click(newx, newy)
-        
-        elif (event.button == 3): # right click
-            self.mpl_disconnect(self.connect_id)
-            call_after()
-        
-    def draw_click(self, posx, posy):
-        """
-        it updates the plot once the user clicks on the plot and draws a 4x4 pixel dot
-        at the coordinate of the click 
-        """     
-        self.vismask[posy:posy+2, posx:posx+2] = 9
-        self.redraw_mask()
-
-    def redraw_mask(self):
-        """Redraw mask with current self.vismask"""
-        self.ax_mask.set_data((self.vismask%10+1)*(self.vismask!=0))
-        self.ax.draw_artist(self.ax_image)
-        self.ax.draw_artist(self.ax_mask)
-        self.update()
-        self.flush_events()
-
-    def recalculate_vismask(self):
-        """Recalculates vismask with current list of cells to show"""
-        tmp = self.mask.copy()
-        all_cells = set(np.unique(tmp))
-        to_remove = all_cells - self.sellist
-        for cell in to_remove:
-            tmp[tmp==cell] = 0
-        self.vismask = tmp
-
-    def update_plots(self):
-        """Shows plot with currently selected cells"""
-        self.recalculate_vismask()
-        self.redraw_mask()
-
-def _create_button(text, connect, tooltip=None):
-    """Initializes button, connects with callback connect"""
-    button = QPushButton(text)
-    button.clicked.connect(connect)
-    button.setMaximumWidth(150)
-    
-    if tooltip is not None:
-        button.setToolTip(tooltip)
-    
-    return button
-
-def _colormap(Ncolors=21):
-    """Creates colormap for segmentation mask"""
-    jet = cm.get_cmap('jet', Ncolors)
-    
-    cmaplist = [(0,0,0,0)]
-    for i in range(jet.N):
-        r,g,b,_ = jet(i)
-        cmaplist.append((r,g,b,.2))
-    cmap = LinearSegmentedColormap.from_list('Custom cmap', cmaplist, Ncolors)
-    return cmap  
-        
-def _poly_to_mask(polygon, shape):
-    """Converts polygon to mask"""
-    img = Image.new('L', shape, 0)
-    ImageDraw.Draw(img).polygon(polygon, outline=0, fill=1)
-    return np.array(img).astype(int)
-
-def _poly_to_line(polygon, shape):
-    """Converts polygon to line"""
-    img = Image.new('L', shape, 0)
-    ImageDraw.Draw(img).polygon(polygon, outline=1, fill=0)
-    return np.array(img).astype(int)
-
-def _test_data():
-    """Creates test data"""
-    im = np.zeros((100,100))
-    mask = np.zeros(im.shape)
-
-    poly1 = [(20,20),(30,30),(20,40),(10,30)]
-    poly2 = [(50,50),(60,60),(50,70),(40,60)]
-
-    mask += _poly_to_mask(poly1, im.shape)
-    mask += _poly_to_mask(poly2, im.shape)*2
-    im += _poly_to_line(poly1, im.shape)
-    im += _poly_to_line(poly2, im.shape)
-    
-    return im, mask
-        
-        
-if __name__ == '__main__':
-    app = QApplication(sys.argv)
-    ex = Extract(*_test_data())
-    sys.exit(app.exec_())
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+GUI to select and deselect cells at extraction time.
+"""
+
+import sys
+import os
+import numpy as np
+from PyQt6.QtWidgets import (QApplication, QPushButton, QLabel,
+                             QHBoxLayout, QVBoxLayout, QListWidget,
+                             QFileDialog, QMessageBox, QDialog)
+from PyQt6.QtCore import Qt
+
+
+from PIL import Image, ImageDraw
+
+#Import from matplotlib to use it to display the pictures and masks.
+from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+
+from matplotlib import cm
+from matplotlib.colors import LinearSegmentedColormap
+from matplotlib.figure import Figure
+
+from ..disk.image_loader import load_image
+
+class Extract(QDialog):
+    
+    
+    def __init__(self, image, mask, channel_names=[]):
+        parent = None
+        super(Extract, self).__init__(parent)
+        self.setWindowFlags(Qt.WindowType.WindowStaysOnTopHint)
+#        image, mask = _test_data()
+        self.pc = PlotCanvas(image, mask)
+        self.file_list = channel_names
+        self.init_UI()
+        self.exit_code = 0 # 0: Cancel, 1: Fluorescence, 2: Mask
+
+    def init_UI(self):
+        # Extract Buttons
+        title_extr = QLabel('Extract:')
+        self.extr_mask = _create_button("Extract mask", self.do_extr_mask)
+        self.extr_fluo = _create_button("Extract values", self.do_extr_fluo)
+        self.done = _create_button("Cancel", self.do_cancel)
+        self.done.setDefault(True)  
+        
+        extr_box = QVBoxLayout()
+        extr_box.addWidget(title_extr)
+        extr_box.addWidget(self.extr_mask)
+        extr_box.addWidget(self.extr_fluo)
+        extr_box.addWidget(self.done)
+        extr_box.setAlignment(Qt.AlignmentFlag.AlignTop)
+        
+        # Select Button
+        title_select = QLabel('Select cells:')
+        self.sel_mult = _create_button("Select multiple cells", self.do_sel_mult,
+                                       "Left-click to define the corners of a polygon around cells, "
+                                       "right-click to confirm.")
+        self.sel_sngl = _create_button("Select single cell", self.do_sel_sngl,
+                                       "Left-click to select cell, right-click "
+                                       "to abort.")
+        self.desel_mult = _create_button("Deselect multiple cells", self.do_desel_mult,
+                                       "Left-click to define the corners of a polygon around cells, "
+                                       "right-click to confirm.")
+        self.desel_sngl = _create_button("Deselect single cell", self.do_desel_sngl,
+                                       "Left-click to deselect cell, right-click "
+                                       "to abort.")
+        
+        sel_box = QVBoxLayout()
+        sel_box.addWidget(title_select)
+        sel_box.addWidget(self.sel_mult)
+        sel_box.addWidget(self.sel_sngl)
+        sel_box.addWidget(self.desel_mult)
+        sel_box.addWidget(self.desel_sngl)
+        sel_box.setAlignment(Qt.AlignmentFlag.AlignTop)
+        
+        # Additional Fluorescence File
+        file_title = QLabel("Manage files and channels for extraction:")
+        self.list_channels = QListWidget()
+        self.add_file = _create_button('Add', self.do_add_file)
+        self.remove_file = _create_button('Remove', self.do_remove_file)
+        
+        add_remove = QHBoxLayout()
+        add_remove.addWidget(self.add_file)
+        add_remove.addWidget(self.remove_file)
+        
+        manage_box = QVBoxLayout()
+        manage_box.addWidget(file_title)
+        manage_box.addWidget(self.list_channels)
+        manage_box.addLayout(add_remove)
+        manage_box.setAlignment(Qt.AlignmentFlag.AlignTop)
+        
+        # Button list
+        self.buttons = [self.extr_mask,
+                        self.extr_fluo,
+                        self.done,
+                        self.sel_mult,
+                        self.sel_sngl,
+                        self.desel_mult,
+                        self.desel_sngl,
+                        self.add_file,
+                        self.remove_file,
+                        self.list_channels]
+        
+        # Buttons
+        buttons = QHBoxLayout()
+        buttons.addLayout(sel_box)
+        buttons.addLayout(manage_box)
+        buttons.addLayout(extr_box)
+        
+        # Plot Canvas
+        full = QVBoxLayout()
+        full.addWidget(self.pc)
+        full.addStretch(.5)
+        full.addLayout(buttons)
+        
+        # Add channel list
+        self.do_show_list()
+
+        self.setLayout(full)    
+        self.setGeometry(300, 300, 600, 600)
+        self.setWindowTitle('Extract geometries, fluorescence, masks')
+        self.show()
+
+    def do_extr_fluo(self):
+        self.outfile, _ = QFileDialog.getSaveFileName(
+            self,"Specify CSV file for exporting values",
+            "","All files (*);;Text files (*.csv)")
+        _, ext = os.path.splitext(self.outfile)
+        if ext == '':
+            self.outfile += '.csv'
+        elif ext != '.csv':
+            msg_box = QMessageBox(QMessageBox.Icon.Critical,'Error','Must specify .csv file', parent=self)
+            msg_box.exec()
+            return 
+        
+        self.exit_code = 1
+        self.cells = self.pc.sellist
+        self.desel_cells = set(np.unique(self.pc.mask)) - set(self.cells)
+        self.close()
+
+    def do_cancel(self):
+        self.close()
+    
+    def do_extr_mask(self):
+        self.outfile, _ = QFileDialog.getSaveFileName(
+            self,"Specify TIFF file for exporting mask",
+            "","All files (*);;Image file (*.tiff)")
+        _, ext = os.path.splitext(self.outfile)
+        if ext == '':
+            self.outfile += '.tif'
+        elif ext != '.tif' and ext!='.tiff' and ext!='.TIF' and ext!='.TIFF':
+            msg_box = QMessageBox(QMessageBox.Icon.Critical,'Error','Must specify .tif file', parent=self)
+            msg_box.exec()
+            return 
+
+        self.exit_code = 2
+        self.cells = self.pc.sellist
+        self.desel_cells = set(np.unique(self.pc.mask)) - set(self.cells)
+        self.close()
+                
+    def do_sel_mult(self):
+        """Callback for selecting multiple"""
+        self.pc.storemouseclicks = []        
+        def to_connect(e):
+            self.pc.multiple_click(e, self.do_sel_mult_process)
+        self.pc.connect_id = self.pc.mpl_connect(
+                'button_press_event', 
+                 to_connect)
+        self.deactivate_all()
+        
+    def do_sel_mult_process(self):
+        """Process selecting multiple"""
+        cells = self.cells_in_polygon()
+        self.pc.sellist = self.pc.sellist.union(cells)
+        self.disconnect()
+        
+    def do_desel_mult(self):
+        self.pc.storemouseclicks = []        
+        """Callback for deselecting multiple"""
+        def to_connect(e):
+            self.pc.multiple_click(e, self.do_desel_mult_process)
+        self.pc.connect_id = self.pc.mpl_connect(
+                'button_press_event', 
+                 to_connect)
+        self.deactivate_all()
+        
+    def do_desel_mult_process(self):
+        """Process deselect multiple"""
+        cells = self.cells_in_polygon()
+        self.pc.sellist = self.pc.sellist - cells
+        self.disconnect()
+        
+    def cells_in_polygon(self):
+        """Extracts cells inside of polygon specified by pc.storemouseclicks"""
+        nx, ny = self.pc.mask.shape
+        img = Image.new('L', (ny, nx), 0)
+        ImageDraw.Draw(img).polygon(self.pc.storemouseclicks, outline=1, fill=1)
+        polygon = np.array(img).astype(bool)
+        return set(np.unique(self.pc.mask[polygon]))
+    
+    def do_sel_sngl(self):
+        """Select single cell"""
+        def to_connect(e):
+            self.pc.single_click(e, self.do_sel_sngl_process)
+        self.pc.connect_id = self.pc.mpl_connect(
+                'button_press_event', 
+                 to_connect)
+        self.deactivate_all()
+    
+    def do_sel_sngl_process(self, x, y):
+        """Process selected cell"""
+        if x is not None:
+            cell = self.pc.mask[y,x]
+            self.pc.sellist.add(cell)
+        self.disconnect()
+    
+    def do_desel_sngl(self):
+        """Deselect single cell"""
+        def to_connect(e):
+            self.pc.single_click(e, self.do_desel_sngl_process)
+        self.pc.connect_id = self.pc.mpl_connect(
+                'button_press_event', 
+                 to_connect)
+        self.deactivate_all()
+        
+    def do_desel_sngl_process(self, x, y):
+        """Process deselected cell"""
+        if x is not None:
+            cell = self.pc.mask[y,x]
+            self.pc.sellist.remove(cell)
+        self.disconnect()
+            
+    def disconnect(self):
+        """Disconnects callback, updates plots, activates buttons"""
+        self.pc.update_plots()
+        self.pc.mpl_disconnect(self.pc.connect_id)
+        self.activate_all()
+        
+    def deactivate_all(self):
+        for b in self.buttons:
+            b.setEnabled(False)
+            
+    def activate_all(self):
+        for b in self.buttons:
+            b.setEnabled(True)
+            
+    def do_add_file(self):
+        dlg = QFileDialog()
+        dlg.setProxyModel(None)
+        if dlg.exec():
+            full_files = dlg.selectedFiles()
+            if self.test_file(full_files):
+                self.file_list = self.file_list + full_files
+                self.do_show_list()
+    
+    def do_remove_file(self):
+        item_to_remove = self.list_channels.currentItem()
+        remove_ix = self.list_channels.row(item_to_remove)
+        self.file_list.pop(remove_ix)
+        self.do_show_list()
+    
+    def do_show_list(self):
+        self.list_channels.clear()
+        for file in self.file_list:
+            _, name = os.path.split(file)
+            self.list_channels.addItem(name)
+            
+    def test_file(self, files):
+        """Tests if input image has appropriate size and contains data"""
+        for f in files:
+            try: 
+                im = load_image(f, 0)
+            except ValueError:
+                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", "Could not load file", parent=self)
+                msg_box.exec()
+                return False
+            if not im.shape == self.pc.mask.shape:
+                msg_box = QMessageBox(QMessageBox.Icon.Critical, "Error", "Loaded image has wrong size", parent=self)
+                msg_box.exec()
+                return False
+        return True
+            
+    
+
+class PlotCanvas(FigureCanvas):
+    
+    
+    def __init__(self, image, mask, parent=None, figsize=(5,4)):
+        """this class defines the canvas. It initializes a figure, which is then
+        used to plot our data using imshow.
+        """
+        fig = Figure()
+        self.ax = fig.add_subplot(111)
+        super(PlotCanvas, self).__init__(fig)
+        self.setParent(parent)
+        
+        self.image = image
+        self.mask = mask
+        self.sellist = set(np.unique(mask)) # selected cells
+        self.vismask = mask.copy() # mask with only selected cells
+        
+        self.ax_image, self.ax_mask = self.initialize_plots(image, mask, self.ax)        
+        self.storemouseclicks = []
+        self.connect_id = None
+
+    def initialize_plots(self, picture, mask, ax):
+        """Creates plots at initialization"""
+        newcmp = _colormap(21)
+        ax.axis("off")
+        self.draw()
+        return (ax.imshow(picture, interpolation= 'None', 
+                          origin = 'upper', cmap = 'gray_r'), 
+                ax.imshow((mask%10+1)*(mask != 0), origin = 'upper', 
+                          interpolation = 'None', cmap = newcmp,
+                          vmin=0, vmax=11))
+            
+    def single_click(self, event, call_after):
+        """Function for single click, calls call_after afterwards with
+        the clicked points (or None, None) if abort click."""
+        if (event.button == 1
+            and (event.xdata != None and event.ydata != None) 
+            and self.ax == event.inaxes):
+            x = int(event.xdata)
+            y = int(event.ydata)
+            call_after(x, y)
+        else:
+            call_after(None, None)
+            
+    def multiple_click(self, event, call_after):
+        """Function to keep track of multiple left clicks, confirmed with 
+        a right click. After right click, the function call_after is called"""        
+        
+        if (event.button == 1  # left click
+            and (event.xdata != None and event.ydata != None) 
+            and self.ax == event.inaxes):
+            
+            newx = int(event.xdata)
+            newy = int(event.ydata)
+            self.storemouseclicks.append((newx, newy))
+            self.draw_click(newx, newy)
+        
+        elif (event.button == 3): # right click
+            self.mpl_disconnect(self.connect_id)
+            call_after()
+        
+    def draw_click(self, posx, posy):
+        """
+        it updates the plot once the user clicks on the plot and draws a 4x4 pixel dot
+        at the coordinate of the click 
+        """     
+        self.vismask[posy:posy+2, posx:posx+2] = 9
+        self.redraw_mask()
+
+    def redraw_mask(self):
+        """Redraw mask with current self.vismask"""
+        self.ax_mask.set_data((self.vismask%10+1)*(self.vismask!=0))
+        self.ax.draw_artist(self.ax_image)
+        self.ax.draw_artist(self.ax_mask)
+        self.update()
+        self.flush_events()
+
+    def recalculate_vismask(self):
+        """Recalculates vismask with current list of cells to show"""
+        tmp = self.mask.copy()
+        all_cells = set(np.unique(tmp))
+        to_remove = all_cells - self.sellist
+        for cell in to_remove:
+            tmp[tmp==cell] = 0
+        self.vismask = tmp
+
+    def update_plots(self):
+        """Shows plot with currently selected cells"""
+        self.recalculate_vismask()
+        self.redraw_mask()
+
+def _create_button(text, connect, tooltip=None):
+    """Initializes button, connects with callback connect"""
+    button = QPushButton(text)
+    button.clicked.connect(connect)
+    button.setMaximumWidth(150)
+    
+    if tooltip is not None:
+        button.setToolTip(tooltip)
+    
+    return button
+
+def _colormap(Ncolors=21):
+    """Creates colormap for segmentation mask"""
+    jet = cm.get_cmap('jet', Ncolors)
+    
+    cmaplist = [(0,0,0,0)]
+    for i in range(jet.N):
+        r,g,b,_ = jet(i)
+        cmaplist.append((r,g,b,.2))
+    cmap = LinearSegmentedColormap.from_list('Custom cmap', cmaplist, Ncolors)
+    return cmap  
+        
+def _poly_to_mask(polygon, shape):
+    """Converts polygon to mask"""
+    img = Image.new('L', shape, 0)
+    ImageDraw.Draw(img).polygon(polygon, outline=0, fill=1)
+    return np.array(img).astype(int)
+
+def _poly_to_line(polygon, shape):
+    """Converts polygon to line"""
+    img = Image.new('L', shape, 0)
+    ImageDraw.Draw(img).polygon(polygon, outline=1, fill=0)
+    return np.array(img).astype(int)
+
+def _test_data():
+    """Creates test data"""
+    im = np.zeros((100,100))
+    mask = np.zeros(im.shape)
+
+    poly1 = [(20,20),(30,30),(20,40),(10,30)]
+    poly2 = [(50,50),(60,60),(50,70),(40,60)]
+
+    mask += _poly_to_mask(poly1, im.shape)
+    mask += _poly_to_mask(poly2, im.shape)*2
+    im += _poly_to_line(poly1, im.shape)
+    im += _poly_to_line(poly2, im.shape)
+    
+    return im, mask
+        
+        
+if __name__ == '__main__':
+    app = QApplication(sys.argv)
+    ex = Extract(*_test_data())
+    sys.exit(app.exec_())
```

### Comparing `YeaZ-1.0.0rc1/yeaz/misc/PlotCanvas.py` & `YeaZ-1.0.1/yeaz/misc/PlotCanvas.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,560 +1,560 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-This file handles the PlotCanvas of the GUI - aka the area where the graphics 
-are shown. 
-"""
-import numpy as np
-from skimage import morphology as morph
-from skimage import draw
-import logging
-import os
-logging.basicConfig(
-    format='%(asctime)s %(levelname)s %(funcName)s: %(message)s',
-    level=os.environ.get("LOGLEVEL", "WARNING")
-)
-log = logging.getLogger(__name__)
-
-
-# Import everything for the Graphical User Interface from the PyQt6 library.
-from PyQt6.QtWidgets import QSizePolicy
-
-#Import from matplotlib to use it to display the pictures and masks.
-from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
-
-import matplotlib.pyplot as plt
-
-from matplotlib import cm
-from matplotlib.colors import ListedColormap
-#from matplotlib.path import Path
-
-from scipy import ndimage
-
-from PIL import Image, ImageDraw
-
-
-
-class PlotCanvas(FigureCanvas):
-    def __init__(self, parent=None):
-        """this class defines the canvas. It initializes a figure, which is then
-        used to plot our data using imshow.
-        """
-        # define three subplots corresponding to the previous, current and next
-        # time index.
-        fig, (self.ax2, self.ax, self.ax3) = plt.subplots(1,3, sharex = True, sharey = True)
-        
-        fig.subplots_adjust(bottom=0, top=1, left=0, right=1, wspace = 0.05, hspace = 0.05)
-        FigureCanvas.__init__(self, fig)
-        self.setParent(parent)
-        self.parent = parent
-        
-        # this is some mambo jambo.
-        FigureCanvas.setSizePolicy(self, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
-
-        FigureCanvas.updateGeometry(self)
-        
-        # the self.currpicture attribute takes the original data and will then 
-        # contain the updates drawn by the user.
-        self.currpicture = parent.currentframe
-        self.prevpicture = parent.previousframe
-        self.nextpicture = parent.nextframe
-        self.plotmask = parent.mask_curr
-        self.prevplotmask = parent.mask_previous
-        self.nextplotmask = parent.mask_next
-        self.tempmask = self.plotmask.copy()
-        self.tempplotmask = self.plotmask.copy()
-        
-        # this line is just here to not attribute a zero value to the plot
-        # because if so, then it does not update the plot and it stays blank.
-        self.prevpicture = self.currpicture.copy()
-        
-        # Initialize Plots
-        self.currplot, self.currmask = self.plot(self.currpicture, self.plotmask, self.ax)
-        
-        self.previousplot, self.previousmask = self.plot(self.prevpicture, self.prevplotmask, self.ax2)
-        self.prevpicture = np.zeros([parent.reader.sizey, parent.reader.sizex], dtype = np.uint16)
-        self.prevplotmask = np.zeros([parent.reader.sizey, parent.reader.sizex], dtype =np.uint16)
-        
-        self.nextplot, self.nextmask = self.plot(self.nextpicture, self.nextplotmask, self.ax3)
-        self.previousplot.set_data(self.prevpicture)
-        self.previousmask.set_data((self.prevplotmask%10+1)*(self.prevplotmask != 0))
-
-        self.ax2.draw_artist(self.previousplot)
-        self.ax2.draw_artist(self.previousmask)
-        self.update()
-        self.flush_events()
-        
-        # Set title labels
-        self.titlecurr = self.ax.set_title('Time index {}'.format(parent.Tindex))
-        self.titleprev = self.ax2.set_title('No frame {}'.format(''))
-        self.titlenext = self.ax3.set_title('Next time index {}'.format(parent.Tindex+1))
-        
-        # these variables are just set to test the states of the buttons
-        # (button turned on or  off, etc..) of the buttons in the methods 
-        # used in this class.
-        self.button_showval_check = parent.button_showval
-        self.button_newcell_check = parent.button_newcell
-        self.button_add_region_check = parent.button_add_region
-        self.button_drawmouse_check = parent.button_drawmouse
-        self.button_eraser_check = parent.button_eraser
-        self.button_hidemask_check = parent.button_hidemask
-        
-        # It will plot for the first time and return the imshow function
-        self.currmask.set_clim(0, 10)
-        self.previousmask.set_clim(0,10)
-        self.nextmask.set_clim(0,10)
-        
-        # This attribute is a list which stores all the clicks of the mouse.
-        self.storemouseclicks = []
-        
-        # This attribute is used to store the square where the mouse has been
-        # in order than to draw lines (Paintbrush function)
-        self.storebrushclicks = [False,False]
-        
-        # self.cellval is the variable which sets the value to the pixel
-        # whenever something is drawn.
-        self.cellval = 0
-        
-        # These are lists storing all the annotations which are used to
-        # show the values of the cells on the plots.
-        self.ann_list = []
-        self.ann_list_prev = []
-        self.ann_list_next = []
-
-        
-    def ExchangeCellValue(self, val1, val2):
-        """Swaps the values of the cell between two clusters each representing
-        one cell. This method is called after the user has entered 
-        values in the ExchangeCellValues window.
-        """
-        if (val1 in self.plotmask) and (val2 in self.plotmask):
-            indices = np.where(self.plotmask == val1)
-            self.plotmask[self.plotmask == val2] = val1
-            for i in range(0,len(indices[0])):
-                self.plotmask[indices[0][i], indices[1][i]] = val2
-            self.updatedata()
-        else:
-            raise ValueError('Cell value does not exist.') 
-        
-        
-    def ReleaseClick(self, event):
-        """This method is called from the brush button when the mouse is 
-        released such that the last coordinate saved when something is drawn
-        is set to zero. Because otherwise, if the user starts drawing somewhere
-        else, than a straight line is draw between the last point of the
-        previous mouse drawing/dragging and the new one which then starts.
-        """
-        if self.ax == event.inaxes:
-            self.storebrushclicks = [False, False]
-            self.ShowCellNumbers(type = 'current')
-
-        
-    def OneClick(self, event, radius=3):
-        """This method is called when the Brush button is activated. And
-        sets the value of self.cellval if the click is a right click, or draws
-        a square if the click is a left click. (so if the user does just left
-        click but does not drag, there will be only a square which is drawn )
-        """
-        selem = morph.disk(radius-1)
-        
-        # Right click selects cell
-        if (event.button == 3 
-            and (event.xdata != None and event.ydata != None) 
-            and (not self.button_eraser_check.isChecked()) 
-            and self.ax == event.inaxes):
-            tempx = int(event.xdata)
-            tempy = int(event.ydata)
-            self.cellval = self.plotmask[tempy, tempx]
-            self.storebrushclicks = [False, False]
-            
-        # Left click draws square
-        elif (event.button == 1 and 
-              (event.xdata != None and event.ydata != None) 
-              and self.ax == event.inaxes):
-            tempx = int(event.xdata)
-            tempy = int(event.ydata)
-            
-            to_change = np.zeros(self.plotmask.shape, dtype=bool)
-            to_change[tempy, tempx] = True
-            to_change = morph.dilation(to_change, selem)
-            
-            self.plotmask[to_change] = self.cellval
-            self.storebrushclicks = [tempx,tempy]
-            self.updatedata()
-            
-        else:
-            return
-        
-        
-    def multiple_click(self, event, call_after, radius=3):
-        """Function to keep track of multiple left clicks, confirmed with 
-        a right click. After right click, the function call_after is called"""        
-        
-        if (event.button == 1  # left click
-            and (event.xdata != None and event.ydata != None) 
-            and self.ax == event.inaxes):
-            
-            newx = int(event.xdata)
-            newy = int(event.ydata)
-            self.storemouseclicks.append((newx, newy))
-            
-            self.updateplot(newx, newy, False)
-        
-        elif (event.button == 3): # right click
-            call_after()
-
-            
-    
-    def PaintBrush(self, event, radius=3):
-        """PantBrush is the method to paint using a "brush" and it is based
-        on the mouse event in matplotlib "motion notify event". However it can 
-        not record every pixel that the mouse has hovered over (it is too fast).
-        So, in order to not only draw points (happens when the mouse is dragged
-        too quickly), these points are interpolated here with lines.
-        """
-        selem = morph.disk(radius-1)
-        if (event.button == 1 
-            and (event.xdata != None and event.ydata != None) 
-            and self.ax == event.inaxes):
-            newx = int(event.xdata)
-            newy = int(event.ydata)
-            # when a new cell value is set, there is no point to interpolate, to
-            # draw a line between the points. 
-            if self.storebrushclicks[0] == False :
-                self.storebrushclicks = [newx,newy]
-                
-            else:
-                oldx, oldy = self.storebrushclicks
-                
-                rr, cc, _ = draw.line_aa(newy, newx, oldy, oldx)
-                to_change = np.zeros(self.plotmask.shape, dtype=bool)
-                to_change[rr,cc] = True
-                to_change = morph.dilation(to_change, selem)
-                self.plotmask[to_change] = self.cellval
-                
-            self.storebrushclicks = [newx, newy]
-            self.updatedata()
-            
-            
-    def MouseClick(self,event):
-        """This function is called whenever the add region or the new cell
-        buttons are active and the user clicks on the plot. For each 
-        click on the plot, it records the coordinate of the click and stores
-        it. When the user deactivate the new cell or add region button, 
-        all the coordinates are given to the DrawRegion function (if they 
-        do not all lie on the same line) and out of the coordinates, it makes
-        a polygon. And then draws inside of this polygon by setting the pixels
-        to the self.cellval value.
-        """
-        # button == 1 corresponds to the left click. 
-        if (event.button == 1 
-            and (event.xdata != None and event.ydata != None) 
-            and self.ax == event.inaxes):
-            
-            # extract the coordinate of the click inside of the matplotlib figure
-            # and then takes the integer part
-            newx = int(event.xdata)
-            newy = int(event.ydata)
-            
-            # stores the coordinates of the click
-            self.storemouseclicks.append((newx, newy))
-            
-            # draws in the figure a small square (4x4 pixels) to
-            # visualize where the user has clicked
-            self.updateplot(newx, newy)
-                
-
-    def DefineColormap(self, Ncolors):
-        """Define a new colormap by assigning 10 values of the jet colormap
-            such that there are only colors for the values 0-10 and the values >10
-            will be treated with a modulo operation (updatedata function)
-        """
-        jet = cm.get_cmap('jet', Ncolors)
-        colors = []
-        for i in range(0,Ncolors):
-            if i==0 : 
-                # set background transparency to 0
-                temp = list(jet(i))
-                temp[3]= 0.0
-                colors.append(tuple(temp))
-                
-            else:
-                colors.append(jet(i))
-                
-        colormap = ListedColormap(colors)
-        return colormap
-           
-    
-    def plot(self, picture, mask, ax):
-        """this function is called for the first time when all the subplots
-        are drawn.
-        """
-        # Define a new colormap with 20 colors.
-        newcmp = self.DefineColormap(21)
-        ax.axis("off")
-
-        self.draw()
-        return (ax.imshow(picture, interpolation= 'None', 
-                        origin = 'lower', cmap = 'gray_r'), 
-                ax.imshow((mask%10+1)*(mask != 0), origin = 'lower', 
-                        interpolation = 'None', alpha = 0.2, cmap = newcmp))
-   
-    
-    def UpdatePlots(self, type = "all"):
-        """
-        Updates plots, handles mask and cell numbers.
-        """
-        
-        # Plot images
-        log.debug('call UpdatePlot')
-        self.currplot.set_data(self.currpicture)
-        self.currplot.set_clim(np.amin(self.currpicture), np.amax(self.currpicture))
-        self.ax.draw_artist(self.currplot)
-        
-        self.previousplot.set_data(self.prevpicture)
-        self.previousplot.set_clim(np.amin(self.prevpicture), np.amax(self.prevpicture))
-        self.ax2.draw_artist(self.previousplot)
-            
-        self.nextplot.set_data(self.nextpicture)
-        self.nextplot.set_clim(np.amin(self.nextpicture), np.amax(self.nextpicture))
-        self.ax3.draw_artist(self.nextplot)
-        
-        # Plot masks
-        if not self.button_hidemask_check.isChecked():
-            self.currmask.set_data((self.plotmask%10+1)*(self.plotmask!=0))
-            self.previousmask.set_data((self.prevplotmask%10+1)*(self.prevplotmask != 0))
-            self.nextmask.set_data((self.nextplotmask % 10 +1 )*(self.nextplotmask != 0))
-            
-        else:
-            self.currmask.set_data(np.zeros(self.plotmask.shape))
-            self.previousmask.set_data(np.zeros(self.plotmask.shape))
-            self.nextmask.set_data(np.zeros(self.plotmask.shape))
-        
-        self.ShowCellNumbers(type=type)
-        self.draw()
-        self.update()
-        self.flush_events()
-                
-        
-    def updatedata(self, flag=True):
-        """
-        In order to just display the cells so regions with value > 0
-        and also to assign to each of the cell values one color,
-        the modulo 10 of the value is take and we add 1, to distinguish
-        the values of 10,20,30,... from the background (although the bckgrnd
-        gets with the addition the value 1) and the result of the 
-        modulo is multiplied with a matrix containing a False value for the 
-        background coordinates, setting the background to 0 again.
-        """
-        if flag:
-            self.currmask.set_data((self.plotmask%10+1)*(self.plotmask!=0))
-        else:
-            self.currmask.set_data((self.tempmask%10+1)*(self.tempmask!=0))
-        log.debug('updatedata with flag {}'.format(flag))
-        # show the updates by redrawing the array using draw_artist, it is faster 
-        # to use as it only redraws the array itself, and not everything else.
-        self.ax.draw_artist(self.currplot)
-        self.ax.draw_artist(self.currmask)
-        self.ShowCellNumbers(type='current' if flag else 'None')
-        self.update()
-        # self.flush_events()
-              
-        
-    def HideMask(self):
-        self.UpdatePlots()
-        
-                 
-    def _getCellCenters(self, plotmask):
-        """Get approximate locations for cell centers"""
-        log.debug('start')
-        vals = np.unique(plotmask).astype(int)
-        vals = np.delete(vals, np.where(vals == 0))
-        centers = np.array(ndimage.measurements.center_of_mass(plotmask, labels=plotmask, index=vals))
-        xtemp = np.round(centers[:, 1]).astype(int)
-        ytemp = np.round(centers[:, 0]).astype(int)
-        log.debug('finish')
-        return vals, xtemp, ytemp
-
-    def OnShowCellID(self):
-        """This function is only called when we activate the show cell IDs checkbox."""
-        self.UpdatePlots(type='all')
-
-    def ShowCellNumbers(self, type='all'):
-        """
-        Checks whether to show cell numbers, and does so if button is 
-        checked
-        This function can apply to current frame or to all frames
-        """
-        log.debug("show cell numbers called with type {}".format(type))
-        if self.button_showval_check.isChecked():
-            if(type == 'current'):
-                self.ShowCellNumbersCurr()
-            elif(type == 'all'):
-                self.ShowCellNumbersCurr()
-                self.ShowCellNumbersNext()
-                self.ShowCellNumbersPrev()
-            self.draw()
-        else:
-            self.clearAnnLists()
-        
-    
-    def ShowCellNumbersCurr(self):
-        """This function is called to display the cell values and computes the cebter of each cell and
-        gives the coordinate where the number will be 
-        displayed. The number to be displayed is just given by the value
-        in the mask of the cell.
-        This function is just used for the current time subplot.
-        """         
-        
-        for i,a in enumerate(self.ann_list):
-            a.remove()
-        self.ann_list[:] = []
-        # check if the mask is not empty
-        if np.sum(self.plotmask)==0 :
-            return
-            
-        vals, xtemp, ytemp = self._getCellCenters(self.plotmask)
-        if xtemp.any():
-            for i in range(0,len(xtemp)):
-                ann = self.ax.annotate(str(int(vals[i])), (xtemp[i], ytemp[i]),
-                                        ha='center', va='center')
-                self.ann_list.append(ann)
-    #  self.draw()
-                     
-             
-    def ShowCellNumbersPrev(self):
-        """This function is called to display the cell values and computes the cebter of each cell and
-        gives the coordinate where the number will be 
-        displayed. The number to be displayed is just given by the value
-        in the mask of the cell.
-        This function is just used for the previous time subplot and check if it is the first frame or not.
-        """
-        
-        for i,a in enumerate(self.ann_list_prev):
-            a.remove()
-        self.ann_list_prev[:] = []
-        
-        if(self.parent.Tindex != 0):
-            if np.sum(self.prevplotmask)==0 :
-                return
-            
-            vals, xtemp, ytemp = self._getCellCenters(self.prevplotmask)
-            if xtemp.any():
-                for i in range(0,len(xtemp)):
-                    ann = self.ax2.annotate(str(vals[i]), (xtemp[i], ytemp[i]),
-                                            ha='center', va='center')
-                    self.ann_list_prev.append(ann)
-        #  self.draw()
-        else:
-            self.ann_list_prev = []
-             
-             
-    def ShowCellNumbersNext(self):
-        """This function is called to display the cell values and computes the cebter of each cell and
-        gives the coordinate where the number will be 
-        displayed. The number to be displayed is just given by the value
-        in the mask of the cell.
-        This function is just used for the next time subplot and check if it is the first frame or not.
-        """
-        for i,a in enumerate(self.ann_list_next):
-            a.remove()
-        self.ann_list_next[:] = []
-        if(self.parent.Tindex != self.parent.reader.sizet-1):
-            if np.sum(self.nextplotmask)==0 :
-                return           
-            vals, xtemp, ytemp = self._getCellCenters(self.nextplotmask)
-                
-            if xtemp.any():
-                for i in range(0,len(xtemp)):
-                    ann = self.ax3.annotate(str(vals[i]), (xtemp[i], ytemp[i]),
-                                        ha='center', va='center')
-                    self.ann_list_next.append(ann)
-        #  self.draw()
-        else: 
-            self.ann_list_next = []
-        
-        
-    def clearAnnLists(self):
-        for ann in self.ann_list:
-            ann.remove()
-        self.ann_list = []
-        for ann in self.ann_list_prev:
-            ann.remove()
-        self.ann_list_prev = []
-        for ann in self.ann_list_next:
-            ann.remove()
-        self.ann_list_next = []
-        
-        
-    def updateplot(self, posx, posy, first_is_cell=True):
-        """
-        it updates the plot once the user clicks on the plot and draws a 4x4 pixel dot
-        at the coordinate of the click 
-        """        
-        if first_is_cell:
-            # remove the first coordinate as it should only coorespond 
-            # to the value that the user wants to attribute to the drawn region   
-            xtemp, ytemp = self.storemouseclicks[0]
-    
-            # here we initialize the value attributed to the pixels.
-            # it means that the first click selects the value that will be attributed to
-            # the pixels inside the polygon (drawn by the following mouse clicks of the user)
-            self.cellval = self.plotmask[ytemp, xtemp]
-            
-        else:
-            self.cellval=1
-          
-        # drawing the 2x2 square ot of the mouse click
-        if ((self.button_newcell_check.isChecked() or self.button_drawmouse_check.isChecked()) 
-            and self.cellval == 0):
-            self.tempmask[posy:posy+2, posx:posx+2] = 9
-        else:
-            self.tempmask[posy:posy+2,posx:posx+2] = self.cellval
-
-        # plot the mouseclick
-        self.updatedata(False)
-          
-
-    def DrawRegion(self, flag):
-        """
-        this method is used to draw either a new cell (flag = true) or to add a region to 
-        an existing cell (flag = false). The flag will just be used to set the
-        value of pixels (= self.cellval) in the drawn region. 
-        If flag = true, then the value will be the maximal value plus 1. Such 
-        that it attributes a new value to the new cell.
-        If flag = false, then it will use the value of the first click to set
-        the value of the pixels in the new added region. 
-        """
-        # here the values that have been changed to mark the mouse clicks are 
-        # restored such that they don't appear when the region/new cell is 
-        # drawn.        
-        if flag:
-            # if new cell is added, it sets the value of the drawn pixels to a new value
-            # corresponding to the new cell
-            self.cellval = np.amax(self.plotmask) + 1
-            
-        else:
-            # The first value is taken out as it is just used to set the value
-            # to the new region.
-            self.storemouseclicks.pop(0)
-        
-        if len(self.storemouseclicks) <= 2:
-            # if only two points or less have been click, it cannot make a area
-            # so it justs discards these values and returns. 
-            self.storemouseclicks = list(self.storemouseclicks)
-            self.storemouseclicks.clear()
-            self.updatedata(True)
-            return
-        
-        else:
-            # Draw polygon, fill it with cell values
-            nx, ny = self.plotmask.shape
-            img = Image.new('L', (ny, nx), 0)
-            ImageDraw.Draw(img).polygon(self.storemouseclicks, outline=1, fill=1)
-            polygon = np.array(img).astype(bool)
-            self.plotmask[polygon] = self.cellval
-            self.updatedata()
-            
-        # empty the lists ready for the next region to be drawn.
-        self.storemouseclicks = []
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+"""
+This file handles the PlotCanvas of the GUI - aka the area where the graphics 
+are shown. 
+"""
+import numpy as np
+from skimage import morphology as morph
+from skimage import draw
+import logging
+import os
+logging.basicConfig(
+    format='%(asctime)s %(levelname)s %(funcName)s: %(message)s',
+    level=os.environ.get("LOGLEVEL", "WARNING")
+)
+log = logging.getLogger(__name__)
+
+
+# Import everything for the Graphical User Interface from the PyQt6 library.
+from PyQt6.QtWidgets import QSizePolicy
+
+#Import from matplotlib to use it to display the pictures and masks.
+from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
+
+import matplotlib.pyplot as plt
+
+from matplotlib import cm
+from matplotlib.colors import ListedColormap
+#from matplotlib.path import Path
+
+from scipy import ndimage
+
+from PIL import Image, ImageDraw
+
+
+
+class PlotCanvas(FigureCanvas):
+    def __init__(self, parent=None):
+        """this class defines the canvas. It initializes a figure, which is then
+        used to plot our data using imshow.
+        """
+        # define three subplots corresponding to the previous, current and next
+        # time index.
+        fig, (self.ax2, self.ax, self.ax3) = plt.subplots(1,3, sharex = True, sharey = True)
+        
+        fig.subplots_adjust(bottom=0, top=1, left=0, right=1, wspace = 0.05, hspace = 0.05)
+        FigureCanvas.__init__(self, fig)
+        self.setParent(parent)
+        self.parent = parent
+        
+        # this is some mambo jambo.
+        FigureCanvas.setSizePolicy(self, QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Expanding)
+
+        FigureCanvas.updateGeometry(self)
+        
+        # the self.currpicture attribute takes the original data and will then 
+        # contain the updates drawn by the user.
+        self.currpicture = parent.currentframe
+        self.prevpicture = parent.previousframe
+        self.nextpicture = parent.nextframe
+        self.plotmask = parent.mask_curr
+        self.prevplotmask = parent.mask_previous
+        self.nextplotmask = parent.mask_next
+        self.tempmask = self.plotmask.copy()
+        self.tempplotmask = self.plotmask.copy()
+        
+        # this line is just here to not attribute a zero value to the plot
+        # because if so, then it does not update the plot and it stays blank.
+        self.prevpicture = self.currpicture.copy()
+        
+        # Initialize Plots
+        self.currplot, self.currmask = self.plot(self.currpicture, self.plotmask, self.ax)
+        
+        self.previousplot, self.previousmask = self.plot(self.prevpicture, self.prevplotmask, self.ax2)
+        self.prevpicture = np.zeros([parent.reader.sizey, parent.reader.sizex], dtype = np.uint16)
+        self.prevplotmask = np.zeros([parent.reader.sizey, parent.reader.sizex], dtype =np.uint16)
+        
+        self.nextplot, self.nextmask = self.plot(self.nextpicture, self.nextplotmask, self.ax3)
+        self.previousplot.set_data(self.prevpicture)
+        self.previousmask.set_data((self.prevplotmask%10+1)*(self.prevplotmask != 0))
+
+        self.ax2.draw_artist(self.previousplot)
+        self.ax2.draw_artist(self.previousmask)
+        self.update()
+        self.flush_events()
+        
+        # Set title labels
+        self.titlecurr = self.ax.set_title('Time index {}'.format(parent.Tindex))
+        self.titleprev = self.ax2.set_title('No frame {}'.format(''))
+        self.titlenext = self.ax3.set_title('Next time index {}'.format(parent.Tindex+1))
+        
+        # these variables are just set to test the states of the buttons
+        # (button turned on or  off, etc..) of the buttons in the methods 
+        # used in this class.
+        self.button_showval_check = parent.button_showval
+        self.button_newcell_check = parent.button_newcell
+        self.button_add_region_check = parent.button_add_region
+        self.button_drawmouse_check = parent.button_drawmouse
+        self.button_eraser_check = parent.button_eraser
+        self.button_hidemask_check = parent.button_hidemask
+        
+        # It will plot for the first time and return the imshow function
+        self.currmask.set_clim(0, 10)
+        self.previousmask.set_clim(0,10)
+        self.nextmask.set_clim(0,10)
+        
+        # This attribute is a list which stores all the clicks of the mouse.
+        self.storemouseclicks = []
+        
+        # This attribute is used to store the square where the mouse has been
+        # in order than to draw lines (Paintbrush function)
+        self.storebrushclicks = [False,False]
+        
+        # self.cellval is the variable which sets the value to the pixel
+        # whenever something is drawn.
+        self.cellval = 0
+        
+        # These are lists storing all the annotations which are used to
+        # show the values of the cells on the plots.
+        self.ann_list = []
+        self.ann_list_prev = []
+        self.ann_list_next = []
+
+        
+    def ExchangeCellValue(self, val1, val2):
+        """Swaps the values of the cell between two clusters each representing
+        one cell. This method is called after the user has entered 
+        values in the ExchangeCellValues window.
+        """
+        if (val1 in self.plotmask) and (val2 in self.plotmask):
+            indices = np.where(self.plotmask == val1)
+            self.plotmask[self.plotmask == val2] = val1
+            for i in range(0,len(indices[0])):
+                self.plotmask[indices[0][i], indices[1][i]] = val2
+            self.updatedata()
+        else:
+            raise ValueError('Cell value does not exist.') 
+        
+        
+    def ReleaseClick(self, event):
+        """This method is called from the brush button when the mouse is 
+        released such that the last coordinate saved when something is drawn
+        is set to zero. Because otherwise, if the user starts drawing somewhere
+        else, than a straight line is draw between the last point of the
+        previous mouse drawing/dragging and the new one which then starts.
+        """
+        if self.ax == event.inaxes:
+            self.storebrushclicks = [False, False]
+            self.ShowCellNumbers(type = 'current')
+
+        
+    def OneClick(self, event, radius=3):
+        """This method is called when the Brush button is activated. And
+        sets the value of self.cellval if the click is a right click, or draws
+        a square if the click is a left click. (so if the user does just left
+        click but does not drag, there will be only a square which is drawn )
+        """
+        selem = morph.disk(radius-1)
+        
+        # Right click selects cell
+        if (event.button == 3 
+            and (event.xdata != None and event.ydata != None) 
+            and (not self.button_eraser_check.isChecked()) 
+            and self.ax == event.inaxes):
+            tempx = int(event.xdata)
+            tempy = int(event.ydata)
+            self.cellval = self.plotmask[tempy, tempx]
+            self.storebrushclicks = [False, False]
+            
+        # Left click draws square
+        elif (event.button == 1 and 
+              (event.xdata != None and event.ydata != None) 
+              and self.ax == event.inaxes):
+            tempx = int(event.xdata)
+            tempy = int(event.ydata)
+            
+            to_change = np.zeros(self.plotmask.shape, dtype=bool)
+            to_change[tempy, tempx] = True
+            to_change = morph.dilation(to_change, selem)
+            
+            self.plotmask[to_change] = self.cellval
+            self.storebrushclicks = [tempx,tempy]
+            self.updatedata()
+            
+        else:
+            return
+        
+        
+    def multiple_click(self, event, call_after, radius=3):
+        """Function to keep track of multiple left clicks, confirmed with 
+        a right click. After right click, the function call_after is called"""        
+        
+        if (event.button == 1  # left click
+            and (event.xdata != None and event.ydata != None) 
+            and self.ax == event.inaxes):
+            
+            newx = int(event.xdata)
+            newy = int(event.ydata)
+            self.storemouseclicks.append((newx, newy))
+            
+            self.updateplot(newx, newy, False)
+        
+        elif (event.button == 3): # right click
+            call_after()
+
+            
+    
+    def PaintBrush(self, event, radius=3):
+        """PantBrush is the method to paint using a "brush" and it is based
+        on the mouse event in matplotlib "motion notify event". However it can 
+        not record every pixel that the mouse has hovered over (it is too fast).
+        So, in order to not only draw points (happens when the mouse is dragged
+        too quickly), these points are interpolated here with lines.
+        """
+        selem = morph.disk(radius-1)
+        if (event.button == 1 
+            and (event.xdata != None and event.ydata != None) 
+            and self.ax == event.inaxes):
+            newx = int(event.xdata)
+            newy = int(event.ydata)
+            # when a new cell value is set, there is no point to interpolate, to
+            # draw a line between the points. 
+            if self.storebrushclicks[0] == False :
+                self.storebrushclicks = [newx,newy]
+                
+            else:
+                oldx, oldy = self.storebrushclicks
+                
+                rr, cc, _ = draw.line_aa(newy, newx, oldy, oldx)
+                to_change = np.zeros(self.plotmask.shape, dtype=bool)
+                to_change[rr,cc] = True
+                to_change = morph.dilation(to_change, selem)
+                self.plotmask[to_change] = self.cellval
+                
+            self.storebrushclicks = [newx, newy]
+            self.updatedata()
+            
+            
+    def MouseClick(self,event):
+        """This function is called whenever the add region or the new cell
+        buttons are active and the user clicks on the plot. For each 
+        click on the plot, it records the coordinate of the click and stores
+        it. When the user deactivate the new cell or add region button, 
+        all the coordinates are given to the DrawRegion function (if they 
+        do not all lie on the same line) and out of the coordinates, it makes
+        a polygon. And then draws inside of this polygon by setting the pixels
+        to the self.cellval value.
+        """
+        # button == 1 corresponds to the left click. 
+        if (event.button == 1 
+            and (event.xdata != None and event.ydata != None) 
+            and self.ax == event.inaxes):
+            
+            # extract the coordinate of the click inside of the matplotlib figure
+            # and then takes the integer part
+            newx = int(event.xdata)
+            newy = int(event.ydata)
+            
+            # stores the coordinates of the click
+            self.storemouseclicks.append((newx, newy))
+            
+            # draws in the figure a small square (4x4 pixels) to
+            # visualize where the user has clicked
+            self.updateplot(newx, newy)
+                
+
+    def DefineColormap(self, Ncolors):
+        """Define a new colormap by assigning 10 values of the jet colormap
+            such that there are only colors for the values 0-10 and the values >10
+            will be treated with a modulo operation (updatedata function)
+        """
+        jet = cm.get_cmap('jet', Ncolors)
+        colors = []
+        for i in range(0,Ncolors):
+            if i==0 : 
+                # set background transparency to 0
+                temp = list(jet(i))
+                temp[3]= 0.0
+                colors.append(tuple(temp))
+                
+            else:
+                colors.append(jet(i))
+                
+        colormap = ListedColormap(colors)
+        return colormap
+           
+    
+    def plot(self, picture, mask, ax):
+        """this function is called for the first time when all the subplots
+        are drawn.
+        """
+        # Define a new colormap with 20 colors.
+        newcmp = self.DefineColormap(21)
+        ax.axis("off")
+
+        self.draw()
+        return (ax.imshow(picture, interpolation= 'None', 
+                        origin = 'lower', cmap = 'gray_r'), 
+                ax.imshow((mask%10+1)*(mask != 0), origin = 'lower', 
+                        interpolation = 'None', alpha = 0.2, cmap = newcmp))
+   
+    
+    def UpdatePlots(self, type = "all"):
+        """
+        Updates plots, handles mask and cell numbers.
+        """
+        
+        # Plot images
+        log.debug('call UpdatePlot')
+        self.currplot.set_data(self.currpicture)
+        self.currplot.set_clim(np.amin(self.currpicture), np.amax(self.currpicture))
+        self.ax.draw_artist(self.currplot)
+        
+        self.previousplot.set_data(self.prevpicture)
+        self.previousplot.set_clim(np.amin(self.prevpicture), np.amax(self.prevpicture))
+        self.ax2.draw_artist(self.previousplot)
+            
+        self.nextplot.set_data(self.nextpicture)
+        self.nextplot.set_clim(np.amin(self.nextpicture), np.amax(self.nextpicture))
+        self.ax3.draw_artist(self.nextplot)
+        
+        # Plot masks
+        if not self.button_hidemask_check.isChecked():
+            self.currmask.set_data((self.plotmask%10+1)*(self.plotmask!=0))
+            self.previousmask.set_data((self.prevplotmask%10+1)*(self.prevplotmask != 0))
+            self.nextmask.set_data((self.nextplotmask % 10 +1 )*(self.nextplotmask != 0))
+            
+        else:
+            self.currmask.set_data(np.zeros(self.plotmask.shape))
+            self.previousmask.set_data(np.zeros(self.plotmask.shape))
+            self.nextmask.set_data(np.zeros(self.plotmask.shape))
+        
+        self.ShowCellNumbers(type=type)
+        self.draw()
+        self.update()
+        self.flush_events()
+                
+        
+    def updatedata(self, flag=True):
+        """
+        In order to just display the cells so regions with value > 0
+        and also to assign to each of the cell values one color,
+        the modulo 10 of the value is take and we add 1, to distinguish
+        the values of 10,20,30,... from the background (although the bckgrnd
+        gets with the addition the value 1) and the result of the 
+        modulo is multiplied with a matrix containing a False value for the 
+        background coordinates, setting the background to 0 again.
+        """
+        if flag:
+            self.currmask.set_data((self.plotmask%10+1)*(self.plotmask!=0))
+        else:
+            self.currmask.set_data((self.tempmask%10+1)*(self.tempmask!=0))
+        log.debug('updatedata with flag {}'.format(flag))
+        # show the updates by redrawing the array using draw_artist, it is faster 
+        # to use as it only redraws the array itself, and not everything else.
+        self.ax.draw_artist(self.currplot)
+        self.ax.draw_artist(self.currmask)
+        self.ShowCellNumbers(type='current' if flag else 'None')
+        self.update()
+        # self.flush_events()
+              
+        
+    def HideMask(self):
+        self.UpdatePlots()
+        
+                 
+    def _getCellCenters(self, plotmask):
+        """Get approximate locations for cell centers"""
+        log.debug('start')
+        vals = np.unique(plotmask).astype(int)
+        vals = np.delete(vals, np.where(vals == 0))
+        centers = np.array(ndimage.measurements.center_of_mass(plotmask, labels=plotmask, index=vals))
+        xtemp = np.round(centers[:, 1]).astype(int)
+        ytemp = np.round(centers[:, 0]).astype(int)
+        log.debug('finish')
+        return vals, xtemp, ytemp
+
+    def OnShowCellID(self):
+        """This function is only called when we activate the show cell IDs checkbox."""
+        self.UpdatePlots(type='all')
+
+    def ShowCellNumbers(self, type='all'):
+        """
+        Checks whether to show cell numbers, and does so if button is 
+        checked
+        This function can apply to current frame or to all frames
+        """
+        log.debug("show cell numbers called with type {}".format(type))
+        if self.button_showval_check.isChecked():
+            if(type == 'current'):
+                self.ShowCellNumbersCurr()
+            elif(type == 'all'):
+                self.ShowCellNumbersCurr()
+                self.ShowCellNumbersNext()
+                self.ShowCellNumbersPrev()
+            self.draw()
+        else:
+            self.clearAnnLists()
+        
+    
+    def ShowCellNumbersCurr(self):
+        """This function is called to display the cell values and computes the cebter of each cell and
+        gives the coordinate where the number will be 
+        displayed. The number to be displayed is just given by the value
+        in the mask of the cell.
+        This function is just used for the current time subplot.
+        """         
+        
+        for i,a in enumerate(self.ann_list):
+            a.remove()
+        self.ann_list[:] = []
+        # check if the mask is not empty
+        if np.sum(self.plotmask)==0 :
+            return
+            
+        vals, xtemp, ytemp = self._getCellCenters(self.plotmask)
+        if xtemp.any():
+            for i in range(0,len(xtemp)):
+                ann = self.ax.annotate(str(int(vals[i])), (xtemp[i], ytemp[i]),
+                                        ha='center', va='center')
+                self.ann_list.append(ann)
+    #  self.draw()
+                     
+             
+    def ShowCellNumbersPrev(self):
+        """This function is called to display the cell values and computes the cebter of each cell and
+        gives the coordinate where the number will be 
+        displayed. The number to be displayed is just given by the value
+        in the mask of the cell.
+        This function is just used for the previous time subplot and check if it is the first frame or not.
+        """
+        
+        for i,a in enumerate(self.ann_list_prev):
+            a.remove()
+        self.ann_list_prev[:] = []
+        
+        if(self.parent.Tindex != 0):
+            if np.sum(self.prevplotmask)==0 :
+                return
+            
+            vals, xtemp, ytemp = self._getCellCenters(self.prevplotmask)
+            if xtemp.any():
+                for i in range(0,len(xtemp)):
+                    ann = self.ax2.annotate(str(vals[i]), (xtemp[i], ytemp[i]),
+                                            ha='center', va='center')
+                    self.ann_list_prev.append(ann)
+        #  self.draw()
+        else:
+            self.ann_list_prev = []
+             
+             
+    def ShowCellNumbersNext(self):
+        """This function is called to display the cell values and computes the cebter of each cell and
+        gives the coordinate where the number will be 
+        displayed. The number to be displayed is just given by the value
+        in the mask of the cell.
+        This function is just used for the next time subplot and check if it is the first frame or not.
+        """
+        for i,a in enumerate(self.ann_list_next):
+            a.remove()
+        self.ann_list_next[:] = []
+        if(self.parent.Tindex != self.parent.reader.sizet-1):
+            if np.sum(self.nextplotmask)==0 :
+                return           
+            vals, xtemp, ytemp = self._getCellCenters(self.nextplotmask)
+                
+            if xtemp.any():
+                for i in range(0,len(xtemp)):
+                    ann = self.ax3.annotate(str(vals[i]), (xtemp[i], ytemp[i]),
+                                        ha='center', va='center')
+                    self.ann_list_next.append(ann)
+        #  self.draw()
+        else: 
+            self.ann_list_next = []
+        
+        
+    def clearAnnLists(self):
+        for ann in self.ann_list:
+            ann.remove()
+        self.ann_list = []
+        for ann in self.ann_list_prev:
+            ann.remove()
+        self.ann_list_prev = []
+        for ann in self.ann_list_next:
+            ann.remove()
+        self.ann_list_next = []
+        
+        
+    def updateplot(self, posx, posy, first_is_cell=True):
+        """
+        it updates the plot once the user clicks on the plot and draws a 4x4 pixel dot
+        at the coordinate of the click 
+        """        
+        if first_is_cell:
+            # remove the first coordinate as it should only coorespond 
+            # to the value that the user wants to attribute to the drawn region   
+            xtemp, ytemp = self.storemouseclicks[0]
+    
+            # here we initialize the value attributed to the pixels.
+            # it means that the first click selects the value that will be attributed to
+            # the pixels inside the polygon (drawn by the following mouse clicks of the user)
+            self.cellval = self.plotmask[ytemp, xtemp]
+            
+        else:
+            self.cellval=1
+          
+        # drawing the 2x2 square ot of the mouse click
+        if ((self.button_newcell_check.isChecked() or self.button_drawmouse_check.isChecked()) 
+            and self.cellval == 0):
+            self.tempmask[posy:posy+2, posx:posx+2] = 9
+        else:
+            self.tempmask[posy:posy+2,posx:posx+2] = self.cellval
+
+        # plot the mouseclick
+        self.updatedata(False)
+          
+
+    def DrawRegion(self, flag):
+        """
+        this method is used to draw either a new cell (flag = true) or to add a region to 
+        an existing cell (flag = false). The flag will just be used to set the
+        value of pixels (= self.cellval) in the drawn region. 
+        If flag = true, then the value will be the maximal value plus 1. Such 
+        that it attributes a new value to the new cell.
+        If flag = false, then it will use the value of the first click to set
+        the value of the pixels in the new added region. 
+        """
+        # here the values that have been changed to mark the mouse clicks are 
+        # restored such that they don't appear when the region/new cell is 
+        # drawn.        
+        if flag:
+            # if new cell is added, it sets the value of the drawn pixels to a new value
+            # corresponding to the new cell
+            self.cellval = np.amax(self.plotmask) + 1
+            
+        else:
+            # The first value is taken out as it is just used to set the value
+            # to the new region.
+            self.storemouseclicks.pop(0)
+        
+        if len(self.storemouseclicks) <= 2:
+            # if only two points or less have been click, it cannot make a area
+            # so it justs discards these values and returns. 
+            self.storemouseclicks = list(self.storemouseclicks)
+            self.storemouseclicks.clear()
+            self.updatedata(True)
+            return
+        
+        else:
+            # Draw polygon, fill it with cell values
+            nx, ny = self.plotmask.shape
+            img = Image.new('L', (ny, nx), 0)
+            ImageDraw.Draw(img).polygon(self.storemouseclicks, outline=1, fill=1)
+            polygon = np.array(img).astype(bool)
+            self.plotmask[polygon] = self.cellval
+            self.updatedata()
+            
+        # empty the lists ready for the next region to be drawn.
+        self.storemouseclicks = []
```

### Comparing `YeaZ-1.0.0rc1/yeaz/misc/ProgressBar.py` & `YeaZ-1.0.1/yeaz/misc/ProgressBar.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-from PyQt6.QtWidgets import QApplication, QDialog, QProgressBar, QVBoxLayout, QPushButton, QLabel
-import time
-
-class ProgressBar(QDialog):
-    def __init__(self, parent):
-        super().__init__(parent)
-
-        # set the dialog to be a modal that blocks input to the main window
-        self.setModal(True)
-
-        # set the title of the dialog
-        self.setWindowTitle("Progress")
-
-        # create a progress bar widget
-        self.progress = QProgressBar(self)
-
-        # set the minimum and maximum values of the progress bar
-        self.progress.setMinimum(0)
-        self.progress.setMaximum(100)
-
-        # create a label widget to display the progress status
-        self.status = QLabel("Processing...", self)
-
-        # create a layout to add the widgets to
-        layout = QVBoxLayout(self)
-        layout.addWidget(self.status)
-        layout.addWidget(self.progress)
-        self.setLayout(layout)
-
-        # set initial value
-        self.progress.setValue(0)
-        self.status.setText("Processing...")
-
-        # show the dialog
-        self.show()
-
-    def update_progress(self, value):
-        self.progress.setValue(value)
-    def set_status(self, t):
+from PyQt6.QtWidgets import QApplication, QDialog, QProgressBar, QVBoxLayout, QPushButton, QLabel
+import time
+
+class ProgressBar(QDialog):
+    def __init__(self, parent):
+        super().__init__(parent)
+
+        # set the dialog to be a modal that blocks input to the main window
+        self.setModal(True)
+
+        # set the title of the dialog
+        self.setWindowTitle("Progress")
+
+        # create a progress bar widget
+        self.progress = QProgressBar(self)
+
+        # set the minimum and maximum values of the progress bar
+        self.progress.setMinimum(0)
+        self.progress.setMaximum(100)
+
+        # create a label widget to display the progress status
+        self.status = QLabel("Processing...", self)
+
+        # create a layout to add the widgets to
+        layout = QVBoxLayout(self)
+        layout.addWidget(self.status)
+        layout.addWidget(self.progress)
+        self.setLayout(layout)
+
+        # set initial value
+        self.progress.setValue(0)
+        self.status.setText("Processing...")
+
+        # show the dialog
+        self.show()
+
+    def update_progress(self, value):
+        self.progress.setValue(value)
+    def set_status(self, t):
         self.status.setText("Processing... {}%".format(t))
```

### Comparing `YeaZ-1.0.0rc1/yeaz/unet/LaunchBatchPrediction.py` & `YeaZ-1.0.1/yeaz/unet/LaunchBatchPrediction.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-# -*- coding: utf-8 -*-
-"""
-Created on Tue Nov 19 17:38:58 2019
-"""
-
-from PyQt6.QtWidgets import (QDialog, QDialogButtonBox, QLineEdit, QFormLayout, 
-                             QLabel, QListWidget, QAbstractItemView, QCheckBox,
-                             QButtonGroup, QRadioButton, QComboBox)
-from PyQt6 import QtGui
-
-
-class CustomDialog(QDialog):
-    def __init__(self, *args, **kwargs):
-        super(CustomDialog, self).__init__(*args, **kwargs)
-        
-        app, = args
-        maxtimeindex = app.reader.sizet
-        
-        self.setWindowTitle("Launch NN")
-        self.setGeometry(100,100, 500,200)
-        
-        self.entry1 = QLineEdit()
-        self.entry1.setValidator(QtGui.QIntValidator(0,int(maxtimeindex-1)))
-        self.entry2 = QLineEdit()
-        self.entry2.setValidator(QtGui.QIntValidator(0,int(maxtimeindex-1)))
-        
-        # FOV dialog
-        self.listfov = QListWidget()
-        self.listfov.setSelectionMode(QAbstractItemView.SelectionMode.MultiSelection)
-        for f in range(0, app.reader.Npos):
-            self.listfov.addItem('Field of View {}'.format(f+1))
-
-        self.labeltime = QLabel("Enter range of frames ({}-{}) to segment".format(0, app.reader.sizet-1))
-        
-        self.entry_threshold = QLineEdit()
-        self.entry_threshold.setValidator(QtGui.QDoubleValidator())
-        self.entry_threshold.setText('0.5')
-        
-        self.entry_segmentation = QLineEdit()
-        self.entry_segmentation.setValidator(QtGui.QIntValidator())
-        self.entry_segmentation.setText('5')
-                
-        flo = QFormLayout()
-        flo.addWidget(self.labeltime)
-        flo.addRow('Start from frame:', self.entry1)
-        flo.addRow('End at frame:', self.entry2)        
-        flo.addRow('Select field(s) of view:', self.listfov)
-        flo.addRow('Threshold value:', self.entry_threshold)
-        flo.addRow('Min. distance between seeds:', self.entry_segmentation)
-        
-        self.mic_type = QComboBox()
-        self.mic_type.addItem("Image type", None)
-        self.mic_type.addItem("Bright-field budding yeast", "bf")
-        self.mic_type.addItem("Phase contrast budding yeast", "pc")
-        self.mic_type.addItem("Bud phase contrast fission", "fission")
-
-        self.mic_type.setCurrentIndex(0)
-        flo.addRow("Select image type: ", self.mic_type)
-        
-        
-        self.device_selection = QComboBox()
-        self.device_selection.addItem("CPU", "cpu")
-        self.device_selection.addItem("GPU", "cuda")
-        self.device_selection.setCurrentIndex(0)
-        flo.addRow("Select device for running neural network: ", self.device_selection)
-        
-        QBtn = QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
-        
-        self.buttonBox = QDialogButtonBox(QBtn)
-        self.buttonBox.accepted.connect(self.accept)
-        self.buttonBox.rejected.connect(self.reject)
-
-        flo.addWidget(self.buttonBox)
-        self.setLayout(flo)
-        
-
-        
+# -*- coding: utf-8 -*-
+"""
+Created on Tue Nov 19 17:38:58 2019
+"""
+
+from PyQt6.QtWidgets import (QDialog, QDialogButtonBox, QLineEdit, QFormLayout, 
+                             QLabel, QListWidget, QAbstractItemView, QCheckBox,
+                             QButtonGroup, QRadioButton, QComboBox)
+from PyQt6 import QtGui
+
+
+class CustomDialog(QDialog):
+    def __init__(self, *args, **kwargs):
+        super(CustomDialog, self).__init__(*args, **kwargs)
+        
+        app, = args
+        maxtimeindex = app.reader.sizet
+        
+        self.setWindowTitle("Launch NN")
+        self.setGeometry(100,100, 500,200)
+        
+        self.entry1 = QLineEdit()
+        self.entry1.setValidator(QtGui.QIntValidator(0,int(maxtimeindex-1)))
+        self.entry2 = QLineEdit()
+        self.entry2.setValidator(QtGui.QIntValidator(0,int(maxtimeindex-1)))
+        
+        # FOV dialog
+        self.listfov = QListWidget()
+        self.listfov.setSelectionMode(QAbstractItemView.SelectionMode.MultiSelection)
+        for f in range(0, app.reader.Npos):
+            self.listfov.addItem('Field of View {}'.format(f+1))
+
+        self.labeltime = QLabel("Enter range of frames ({}-{}) to segment".format(0, app.reader.sizet-1))
+        
+        self.entry_threshold = QLineEdit()
+        self.entry_threshold.setValidator(QtGui.QDoubleValidator())
+        self.entry_threshold.setText('0.5')
+        
+        self.entry_segmentation = QLineEdit()
+        self.entry_segmentation.setValidator(QtGui.QIntValidator())
+        self.entry_segmentation.setText('5')
+                
+        flo = QFormLayout()
+        flo.addWidget(self.labeltime)
+        flo.addRow('Start from frame:', self.entry1)
+        flo.addRow('End at frame:', self.entry2)        
+        flo.addRow('Select field(s) of view:', self.listfov)
+        flo.addRow('Threshold value:', self.entry_threshold)
+        flo.addRow('Min. distance between seeds:', self.entry_segmentation)
+        
+        self.mic_type = QComboBox()
+        self.mic_type.addItem("Image type", None)
+        self.mic_type.addItem("Bright-field budding yeast", "bf")
+        self.mic_type.addItem("Phase contrast budding yeast", "pc")
+        self.mic_type.addItem("Bud phase contrast fission", "fission")
+
+        self.mic_type.setCurrentIndex(0)
+        flo.addRow("Select image type: ", self.mic_type)
+        
+        
+        self.device_selection = QComboBox()
+        self.device_selection.addItem("CPU", "cpu")
+        self.device_selection.addItem("GPU", "cuda")
+        self.device_selection.setCurrentIndex(0)
+        flo.addRow("Select device for running neural network: ", self.device_selection)
+        
+        QBtn = QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Cancel
+        
+        self.buttonBox = QDialogButtonBox(QBtn)
+        self.buttonBox.accepted.connect(self.accept)
+        self.buttonBox.rejected.connect(self.reject)
+
+        flo.addWidget(self.buttonBox)
+        self.setLayout(flo)
+        
+
+
```

### Comparing `YeaZ-1.0.0rc1/yeaz/unet/hungarian.py` & `YeaZ-1.0.1/yeaz/unet/hungarian.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import numpy as np
-import pandas as pd
-from munkres import Munkres
-from sklearn.preprocessing import scale
-from sklearn.metrics.pairwise import euclidean_distances
-
-
-def correspondence(prev, curr):
-    """
-    Corrects correspondence between previous and current mask, returns current
-    mask with corrected cell values. New cells are given the unique identifier
-    starting at max(prev)+1. 
-    
-    This is done by embedding every cell into a feature space consisting of
-    the center of mass and the area. The pairwise euclidean distance is 
-    calculated between the cells of the previous and current frame. This is 
-    then used as a cost for the bipartite matching problem which is in turn
-    solved by the Hungarian algorithm as implemented in the munkres package.
-    """
-    newcell = np.max(prev) + 1
-    
-    hu_dict = hungarian_align(prev, curr)
-    new = curr.copy()
-    for key, val in hu_dict.items():
-        # If new cell
-        if val == -1:
-            val = newcell
-            newcell += 1
-        
-        new[curr==key] = val
-        
-    return new
-
-
-def hungarian_align(m1, m2):
-    """
-    Aligns the cells using the hungarian algorithm using the euclidean distance as 
-    cost. 
-    Returns dictionary of cells in m2 to cells in m1. If a cell is new, the dictionary 
-    value is -1.
-    """
-    dist, ix1, ix2 = cell_distance(m1, m2)
-    
-    # If dist couldn't be calculated, return dictionary from cells to themselves 
-    if dist is None:
-        unique_m2 = np.unique(m2)
-        return dict(zip(unique_m2, unique_m2))
-    
-    solver = Munkres()
-    indexes = solver.compute(make_square(dist))
-    
-    # Create dictionary of cell indicies
-    d = dict([(ix2.get(i2, -1), ix1.get(i1, -1)) for i1, i2 in indexes])
-    d.pop(-1, None)  
-    return d
-
-
-def cell_to_features(im, c, nsamples=None, time=None):
-    """Embeds cell c in image im into feature space"""
-    coord = np.argwhere(im==c)
-    area = coord.shape[0]
-    
-    if nsamples is not None:
-        samples = np.random.choice(area, min(nsamples, area), replace=False)
-        sampled = coord[samples,:]
-    else:
-        sampled = coord
-    
-    com = sampled.mean(axis=0)
-    
-    return {'cell': c,
-            'time': time,
-            'sqrtarea': np.sqrt(area),
-            'area': area,
-            'com_x': com[0],
-            'com_y': com[1]}
-    
-    
-def cell_distance(m1, m2, weight_com=3):
-    """
-    Gives distance matrix between cells in first and second frame, by embedding
-    all cells into the feature space. Currently uses center of mass and area
-    as features, with center of mass weighted with factor weight_com (to 
-    make it more important).
-    """
-    # Modify to compute use more computed features
-    #cols = ['com_x', 'com_y', 'roundness', 'sqrtarea']
-    cols = ['com_x', 'com_y', 'area']
-
-    def get_features(m, t):
-        cells = list(np.unique(m))
-        if 0 in cells:
-            cells.remove(0)
-        features = [cell_to_features(m, c, time=t) for c in cells]
-        return pd.DataFrame(features), dict(enumerate(cells))
-    
-    # Create df, rescale
-    feat1, ix_to_cell1 = get_features(m1, 1)
-    feat2, ix_to_cell2 = get_features(m2, 2)
-    
-    # Check if one of matrices doesn't contain cells
-    if len(feat1)==0 or len(feat2)==0:
-        return None, None, None
-    
-    df = pd.concat((feat1, feat2))
-    df[cols] = scale(df[cols])
-    
-    # give more importance to center of mass
-    df[['com_x', 'com_y']] = df[['com_x', 'com_y']] * weight_com
-
-    # pairwise euclidean dist
-    dist = euclidean_distances(
-        df.loc[df['time']==1][cols],
-        df.loc[df['time']==2][cols]
-    )
-    return dist, ix_to_cell1, ix_to_cell2
-    
-    
-def zero_pad(m, shape):
-    """Pads matrix with zeros to be of desired shape"""
-    out = np.zeros(shape)
-    nrow, ncol = m.shape
-    out[0:nrow, 0:ncol] = m
-    return out
-
-
-def make_square(m):
-    """Turns matrix into square matrix, as required by Munkres algorithm"""
-    r,c = m.shape
-    if r==c:
-        return m
-    elif r>c:
-        return zero_pad(m, (r,r))
-    else:
-        return zero_pad(m, (c,c))
-
-    
+import numpy as np
+import pandas as pd
+from munkres import Munkres
+from sklearn.preprocessing import scale
+from sklearn.metrics.pairwise import euclidean_distances
+
+
+def correspondence(prev, curr):
+    """
+    Corrects correspondence between previous and current mask, returns current
+    mask with corrected cell values. New cells are given the unique identifier
+    starting at max(prev)+1. 
+    
+    This is done by embedding every cell into a feature space consisting of
+    the center of mass and the area. The pairwise euclidean distance is 
+    calculated between the cells of the previous and current frame. This is 
+    then used as a cost for the bipartite matching problem which is in turn
+    solved by the Hungarian algorithm as implemented in the munkres package.
+    """
+    newcell = np.max(prev) + 1
+    
+    hu_dict = hungarian_align(prev, curr)
+    new = curr.copy()
+    for key, val in hu_dict.items():
+        # If new cell
+        if val == -1:
+            val = newcell
+            newcell += 1
+        
+        new[curr==key] = val
+        
+    return new
+
+
+def hungarian_align(m1, m2):
+    """
+    Aligns the cells using the hungarian algorithm using the euclidean distance as 
+    cost. 
+    Returns dictionary of cells in m2 to cells in m1. If a cell is new, the dictionary 
+    value is -1.
+    """
+    dist, ix1, ix2 = cell_distance(m1, m2)
+    
+    # If dist couldn't be calculated, return dictionary from cells to themselves 
+    if dist is None:
+        unique_m2 = np.unique(m2)
+        return dict(zip(unique_m2, unique_m2))
+    
+    solver = Munkres()
+    indexes = solver.compute(make_square(dist))
+    
+    # Create dictionary of cell indicies
+    d = dict([(ix2.get(i2, -1), ix1.get(i1, -1)) for i1, i2 in indexes])
+    d.pop(-1, None)  
+    return d
+
+
+def cell_to_features(im, c, nsamples=None, time=None):
+    """Embeds cell c in image im into feature space"""
+    coord = np.argwhere(im==c)
+    area = coord.shape[0]
+    
+    if nsamples is not None:
+        samples = np.random.choice(area, min(nsamples, area), replace=False)
+        sampled = coord[samples,:]
+    else:
+        sampled = coord
+    
+    com = sampled.mean(axis=0)
+    
+    return {'cell': c,
+            'time': time,
+            'sqrtarea': np.sqrt(area),
+            'area': area,
+            'com_x': com[0],
+            'com_y': com[1]}
+    
+    
+def cell_distance(m1, m2, weight_com=3):
+    """
+    Gives distance matrix between cells in first and second frame, by embedding
+    all cells into the feature space. Currently uses center of mass and area
+    as features, with center of mass weighted with factor weight_com (to 
+    make it more important).
+    """
+    # Modify to compute use more computed features
+    #cols = ['com_x', 'com_y', 'roundness', 'sqrtarea']
+    cols = ['com_x', 'com_y', 'area']
+
+    def get_features(m, t):
+        cells = list(np.unique(m))
+        if 0 in cells:
+            cells.remove(0)
+        features = [cell_to_features(m, c, time=t) for c in cells]
+        return pd.DataFrame(features), dict(enumerate(cells))
+    
+    # Create df, rescale
+    feat1, ix_to_cell1 = get_features(m1, 1)
+    feat2, ix_to_cell2 = get_features(m2, 2)
+    
+    # Check if one of matrices doesn't contain cells
+    if len(feat1)==0 or len(feat2)==0:
+        return None, None, None
+    
+    df = pd.concat((feat1, feat2))
+    df[cols] = scale(df[cols])
+    
+    # give more importance to center of mass
+    df[['com_x', 'com_y']] = df[['com_x', 'com_y']] * weight_com
+
+    # pairwise euclidean dist
+    dist = euclidean_distances(
+        df.loc[df['time']==1][cols],
+        df.loc[df['time']==2][cols]
+    )
+    return dist, ix_to_cell1, ix_to_cell2
+    
+    
+def zero_pad(m, shape):
+    """Pads matrix with zeros to be of desired shape"""
+    out = np.zeros(shape)
+    nrow, ncol = m.shape
+    out[0:nrow, 0:ncol] = m
+    return out
+
+
+def make_square(m):
+    """Turns matrix into square matrix, as required by Munkres algorithm"""
+    r,c = m.shape
+    if r==c:
+        return m
+    elif r>c:
+        return zero_pad(m, (r,r))
+    else:
+        return zero_pad(m, (c,c))
+
+
```

### Comparing `YeaZ-1.0.0rc1/yeaz/unet/model_pytorch.py` & `YeaZ-1.0.1/yeaz/unet/model_pytorch.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-
-import torch
-import torch.nn as nn
-
-class UNet(nn.Module):
-    def __init__(self):
-        super().__init__()
-        self.conv2d = nn.Conv2d(1, 64, kernel_size=3, padding='same', padding_mode='zeros')
-        self.conv2d_1 = nn.Conv2d(64, 64, kernel_size=3, padding='same')
-        self.conv2d_2 = nn.Conv2d(64, 128, kernel_size=3, padding='same')
-        self.conv2d_3 = nn.Conv2d(128, 128, kernel_size=3, padding='same')
-        self.conv2d_4 = nn.Conv2d(128, 256, kernel_size=3, padding='same')
-        self.conv2d_5 = nn.Conv2d(256, 256, kernel_size=3, padding='same')
-        self.conv2d_6 = nn.Conv2d(256, 512, kernel_size=3, padding='same')
-        self.conv2d_7 = nn.Conv2d(512, 512, kernel_size=3, padding='same')
-        self.conv2d_8 = nn.Conv2d(512, 1024, kernel_size=3, padding='same')
-        self.conv2d_9 = nn.Conv2d(1024, 1024, kernel_size=3, padding='same')
-        self.conv2d_10 = nn.Conv2d(1024, 512, kernel_size=2, padding='same')
-        self.conv2d_11 = nn.Conv2d(1024, 512, kernel_size=3, padding='same')
-        self.conv2d_12 = nn.Conv2d(512, 512, kernel_size=3, padding='same')
-        self.conv2d_13 = nn.Conv2d(512, 256, kernel_size=2, padding='same')
-        self.conv2d_14 = nn.Conv2d(512, 256, kernel_size=3, padding='same')
-        self.conv2d_15 = nn.Conv2d(256, 256, kernel_size=3, padding='same')
-        self.conv2d_16 = nn.Conv2d(256, 128, kernel_size=2, padding='same')
-        self.conv2d_17 = nn.Conv2d(256, 128, kernel_size=3, padding='same')
-        self.conv2d_18 = nn.Conv2d(128, 128, kernel_size=3, padding='same')
-        self.conv2d_19 = nn.Conv2d(128, 64, kernel_size=2, padding='same')
-        self.conv2d_20 = nn.Conv2d(128, 64, kernel_size=3, padding='same')
-        self.conv2d_21 = nn.Conv2d(64, 64, kernel_size=3, padding='same')
-        self.conv2d_22 = nn.Conv2d(64, 2, kernel_size=3, padding='same')
-        self.conv2d_23 = nn.Conv2d(2, 1, kernel_size=1, padding='same')
-
-        # Other stuff
-        self.relu = nn.ReLU()
-        self.maxpool = nn.MaxPool2d((2,2), stride=(2,2))
-        self.dropout = nn.Dropout(0.5)
-        self.upsample =  nn.Upsample(scale_factor=2, mode='nearest')
-        self.sigmoid = nn.Sigmoid()
-
-    def forward(self, inputs):
-        """ Encoder """
-        conv1 = self.conv2d(inputs)
-        conv1 = self.relu(conv1)
-        conv1 = self.conv2d_1(conv1)
-        conv1 = self.relu(conv1)
-        pool1 = self.maxpool(conv1)
-
-        conv2 = self.conv2d_2(pool1)
-        conv2 = self.relu(conv2)
-        conv2 = self.conv2d_3(conv2)
-        conv2= self.relu(conv2)
-        pool2 = self.maxpool(conv2)
-
-        conv3 = self.conv2d_4(pool2)
-        conv3 = self.relu(conv3)
-        conv3 = self.conv2d_5(conv3)
-        conv3 = self.relu(conv3)
-        pool3 = self.maxpool(conv3)
-
-        conv4 = self.conv2d_6(pool3)
-        conv4 = self.relu(conv4)
-        conv4 = self.conv2d_7(conv4)
-        conv4 = self.relu(conv4)
-        drop4 = self.dropout(conv4)
-        pool4 = self.maxpool(drop4)
-
-        
-        """ Bottleneck """
-        conv5 = self.conv2d_8(pool4)
-        conv5 = self.relu(conv5)
-        conv5 = self.conv2d_9(conv5)
-        conv5 = self.relu(conv5)
-        drop5 = self.dropout(conv5)
-
-        """ Decoder """
-        up6 = self.upsample(drop5)
-        up6 = self.conv2d_10(up6)
-        up6 = self.relu(up6)
-        merg6 = torch.cat((drop4,up6), dim=1)
-        conv6 = self.conv2d_11(merg6)
-        conv6 = self.relu(conv6)
-        conv6 = self.conv2d_12(conv6)
-        conv6 = self.relu(conv6)
-
-        up7 = self.upsample(conv6)
-        up7 = self.conv2d_13(up7)
-        up7 = self.relu(up7)
-        merg7 = torch.cat((conv3,up7), dim=1)
-        conv7 = self.conv2d_14(merg7)
-        conv7 = self.relu(conv7)
-        conv7 = self.conv2d_15(conv7)
-        conv7 = self.relu(conv7)
-
-        up8 = self.upsample(conv7)
-        up8 = self.conv2d_16(up8)
-        up8 = self.relu(up8)
-        merg8 = torch.cat((conv2,up8), dim=1)
-        conv8 = self.conv2d_17(merg8)
-        conv8 = self.relu(conv8)
-        conv8 = self.conv2d_18(conv8)
-        conv8 = self.relu(conv8)
-
-        up9 = self.upsample(conv8)
-        up9 = self.conv2d_19(up9)
-        up9 = self.relu(up9)
-        merg9 = torch.cat((conv1,up9), dim=1)
-        conv9 = self.conv2d_20(merg9)
-        conv9 = self.relu(conv9)
-        conv9 = self.conv2d_21(conv9)
-        conv9 = self.relu(conv9)
-
-        """ Classifier """
-        conv9 = self.conv2d_22(conv9)
-        conv9 = self.relu(conv9)
-        conv10 = self.conv2d_23(conv9)
-        conv10 = self.sigmoid(conv10)
-        
-        
-        return conv10
-
+
+import torch
+import torch.nn as nn
+
+class UNet(nn.Module):
+    def __init__(self):
+        super().__init__()
+        self.conv2d = nn.Conv2d(1, 64, kernel_size=3, padding='same', padding_mode='zeros')
+        self.conv2d_1 = nn.Conv2d(64, 64, kernel_size=3, padding='same')
+        self.conv2d_2 = nn.Conv2d(64, 128, kernel_size=3, padding='same')
+        self.conv2d_3 = nn.Conv2d(128, 128, kernel_size=3, padding='same')
+        self.conv2d_4 = nn.Conv2d(128, 256, kernel_size=3, padding='same')
+        self.conv2d_5 = nn.Conv2d(256, 256, kernel_size=3, padding='same')
+        self.conv2d_6 = nn.Conv2d(256, 512, kernel_size=3, padding='same')
+        self.conv2d_7 = nn.Conv2d(512, 512, kernel_size=3, padding='same')
+        self.conv2d_8 = nn.Conv2d(512, 1024, kernel_size=3, padding='same')
+        self.conv2d_9 = nn.Conv2d(1024, 1024, kernel_size=3, padding='same')
+        self.conv2d_10 = nn.Conv2d(1024, 512, kernel_size=2, padding='same')
+        self.conv2d_11 = nn.Conv2d(1024, 512, kernel_size=3, padding='same')
+        self.conv2d_12 = nn.Conv2d(512, 512, kernel_size=3, padding='same')
+        self.conv2d_13 = nn.Conv2d(512, 256, kernel_size=2, padding='same')
+        self.conv2d_14 = nn.Conv2d(512, 256, kernel_size=3, padding='same')
+        self.conv2d_15 = nn.Conv2d(256, 256, kernel_size=3, padding='same')
+        self.conv2d_16 = nn.Conv2d(256, 128, kernel_size=2, padding='same')
+        self.conv2d_17 = nn.Conv2d(256, 128, kernel_size=3, padding='same')
+        self.conv2d_18 = nn.Conv2d(128, 128, kernel_size=3, padding='same')
+        self.conv2d_19 = nn.Conv2d(128, 64, kernel_size=2, padding='same')
+        self.conv2d_20 = nn.Conv2d(128, 64, kernel_size=3, padding='same')
+        self.conv2d_21 = nn.Conv2d(64, 64, kernel_size=3, padding='same')
+        self.conv2d_22 = nn.Conv2d(64, 2, kernel_size=3, padding='same')
+        self.conv2d_23 = nn.Conv2d(2, 1, kernel_size=1, padding='same')
+
+        # Other stuff
+        self.relu = nn.ReLU()
+        self.maxpool = nn.MaxPool2d((2,2), stride=(2,2))
+        self.dropout = nn.Dropout(0.5)
+        self.upsample =  nn.Upsample(scale_factor=2, mode='nearest')
+        self.sigmoid = nn.Sigmoid()
+
+    def forward(self, inputs):
+        """ Encoder """
+        conv1 = self.conv2d(inputs)
+        conv1 = self.relu(conv1)
+        conv1 = self.conv2d_1(conv1)
+        conv1 = self.relu(conv1)
+        pool1 = self.maxpool(conv1)
+
+        conv2 = self.conv2d_2(pool1)
+        conv2 = self.relu(conv2)
+        conv2 = self.conv2d_3(conv2)
+        conv2= self.relu(conv2)
+        pool2 = self.maxpool(conv2)
+
+        conv3 = self.conv2d_4(pool2)
+        conv3 = self.relu(conv3)
+        conv3 = self.conv2d_5(conv3)
+        conv3 = self.relu(conv3)
+        pool3 = self.maxpool(conv3)
+
+        conv4 = self.conv2d_6(pool3)
+        conv4 = self.relu(conv4)
+        conv4 = self.conv2d_7(conv4)
+        conv4 = self.relu(conv4)
+        drop4 = self.dropout(conv4)
+        pool4 = self.maxpool(drop4)
+
+        
+        """ Bottleneck """
+        conv5 = self.conv2d_8(pool4)
+        conv5 = self.relu(conv5)
+        conv5 = self.conv2d_9(conv5)
+        conv5 = self.relu(conv5)
+        drop5 = self.dropout(conv5)
+
+        """ Decoder """
+        up6 = self.upsample(drop5)
+        up6 = self.conv2d_10(up6)
+        up6 = self.relu(up6)
+        merg6 = torch.cat((drop4,up6), dim=1)
+        conv6 = self.conv2d_11(merg6)
+        conv6 = self.relu(conv6)
+        conv6 = self.conv2d_12(conv6)
+        conv6 = self.relu(conv6)
+
+        up7 = self.upsample(conv6)
+        up7 = self.conv2d_13(up7)
+        up7 = self.relu(up7)
+        merg7 = torch.cat((conv3,up7), dim=1)
+        conv7 = self.conv2d_14(merg7)
+        conv7 = self.relu(conv7)
+        conv7 = self.conv2d_15(conv7)
+        conv7 = self.relu(conv7)
+
+        up8 = self.upsample(conv7)
+        up8 = self.conv2d_16(up8)
+        up8 = self.relu(up8)
+        merg8 = torch.cat((conv2,up8), dim=1)
+        conv8 = self.conv2d_17(merg8)
+        conv8 = self.relu(conv8)
+        conv8 = self.conv2d_18(conv8)
+        conv8 = self.relu(conv8)
+
+        up9 = self.upsample(conv8)
+        up9 = self.conv2d_19(up9)
+        up9 = self.relu(up9)
+        merg9 = torch.cat((conv1,up9), dim=1)
+        conv9 = self.conv2d_20(merg9)
+        conv9 = self.relu(conv9)
+        conv9 = self.conv2d_21(conv9)
+        conv9 = self.relu(conv9)
+
+        """ Classifier """
+        conv9 = self.conv2d_22(conv9)
+        conv9 = self.relu(conv9)
+        conv10 = self.conv2d_23(conv9)
+        conv10 = self.sigmoid(conv10)
+        
+        
+        return conv10
+
```

### Comparing `YeaZ-1.0.0rc1/yeaz/unet/neural_network.py` & `YeaZ-1.0.1/yeaz/unet/neural_network.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-
-# -*- coding: utf-8 -*-
-"""
-Created on Sat Dec 21 18:54:10 2019
-
-"""
-import os
-import sys
-from .model_pytorch import UNet
-# from model_tensorflow import unet
-import numpy as np
-import skimage
-from skimage import io
-import skimage.transform as trans
-import torch
-
-if getattr(sys, 'frozen', False):
-    path_weights  = os.path.join(sys._MEIPASS, 'unet/')
-    
-else:
-    path_weights = './unet/'
-
-def create_directory_if_not_exists(path):
-    """
-    Create in the file system a new directory if it doesn't exist yet.
-    Param:
-        path: the path of the new directory
-    """
-    if not os.path.exists(path):
-        os.makedirs(path)
-
-
-def threshold(im,th = None):
-    """
-    Binarize an image with a threshold given by the user, or if the threshold is None, calculate the better threshold with isodata
-    Param:
-        im: a numpy array image (numpy array)
-        th: the value of the threshold (feature to select threshold was asked by the lab)
-    Return:
-        bi: threshold given by the user (numpy array)
-    """
-    im2 = im.copy()
-    if th == None:
-        th = skimage.filters.threshold_isodata(im2)
-    bi = im2
-    bi[bi > th] = 255
-    bi[bi <= th] = 0
-    return bi
-
-import gc
-def report_gpu():
-    gc.collect()
-    torch.cuda.empty_cache()
-    print('Memory allocated: ', torch.cuda.memory_allocated())
-
-def prediction(im, mic_type, pretrained_weights=None, model_type='pytorch', device=None):
-    """
-    Calculate the prediction of the label corresponding to image im
-    Param:
-        im: a numpy array image (numpy array), with max size 2048x2048
-    Return:
-        res: the predicted distribution of probability of the labels (numpy array)
-    """        
-    # pad with zeros such that is divisible by 16
-    (nrow, ncol) = im.shape
-    row_add = 16-nrow%16
-    col_add = 16-ncol%16
-    padded = np.pad(im, ((0, row_add), (0, col_add)))
-    
-    if pretrained_weights is None:
-        if mic_type == 'pc':
-            pretrained_weights = path_weights + 'weights_budding_PhC_multilab_0_1'
-        elif mic_type == 'bf':
-            pretrained_weights = path_weights + 'weights_budding_BF_multilab_0_1'
-        elif mic_type == 'fission':
-            pretrained_weights = path_weights + 'weights_fission_multilab_0_2'
-        if model_type == 'tensorflow':
-            pretrained_weights = pretrained_weights + '.hdf5'
-    
-    if not os.path.exists(pretrained_weights):
-        raise ValueError('Path does not exist')
-
-    # WHOLE CELL PREDICTION
-
-    if model_type == 'tensorflow':
-        tf_model = unet(pretrained_weights = pretrained_weights,
-                    input_size = (None,None,1))
-        input = padded[np.newaxis,:,:,np.newaxis]
-        tf_results = tf_model.predict(input, batch_size=1)
-        tf_res = tf_results[0,:,:,0]
-        
-        return tf_res
-
-    elif model_type == 'pytorch':
-        # Load saved weights in pytorch model and run the pytorch model
-        model = UNet()
-        model.load_state_dict(torch.load(pretrained_weights))
-        
-        if torch.cuda.is_available() and device == 'cuda':
-            device = torch.device('cuda')
-            model = model.to(device)
-            padded = torch.from_numpy(padded).to(device)
-            print('device: ', device)
-        else:
-            device = torch.device('cpu')
-            padded = torch.from_numpy(padded)
-            print('device: ', device)
-        model.eval()
-        with torch.no_grad():
-            # Convert input tensor to PyTorch tensor
-            input_tensor = padded.unsqueeze(0).unsqueeze(0).float()
-            # Pass input through the model
-            output_tensor = model.forward(input_tensor)
-            # Convert output tensor to NumPy array
-            output_array = output_tensor.cpu().detach().numpy()
-        pt_res = output_array[0, 0, :, :]
-        
-        # empty cache
-        if (device == 'cuda') and (torch.cuda.is_available()):
-            report_gpu()
-        
-        return pt_res[:nrow, :ncol]
-    
-    
-    else:
-        raise ValueError('model_type is not valid. should be either "pytorch" or "tensorflow".')
+
+# -*- coding: utf-8 -*-
+"""
+Created on Sat Dec 21 18:54:10 2019
+
+"""
+import os
+import sys
+from .model_pytorch import UNet
+# from model_tensorflow import unet
+import numpy as np
+import skimage
+from skimage import io
+import skimage.transform as trans
+import torch
+
+if getattr(sys, 'frozen', False):
+    path_weights  = os.path.join(sys._MEIPASS, 'unet/')
+    
+else:
+    path_weights = './unet/'
+
+def create_directory_if_not_exists(path):
+    """
+    Create in the file system a new directory if it doesn't exist yet.
+    Param:
+        path: the path of the new directory
+    """
+    if not os.path.exists(path):
+        os.makedirs(path)
+
+
+def threshold(im,th = None):
+    """
+    Binarize an image with a threshold given by the user, or if the threshold is None, calculate the better threshold with isodata
+    Param:
+        im: a numpy array image (numpy array)
+        th: the value of the threshold (feature to select threshold was asked by the lab)
+    Return:
+        bi: threshold given by the user (numpy array)
+    """
+    im2 = im.copy()
+    if th == None:
+        th = skimage.filters.threshold_isodata(im2)
+    bi = im2
+    bi[bi > th] = 255
+    bi[bi <= th] = 0
+    return bi
+
+import gc
+def report_gpu():
+    gc.collect()
+    torch.cuda.empty_cache()
+    print('Memory allocated: ', torch.cuda.memory_allocated())
+
+def prediction(im, mic_type, pretrained_weights=None, model_type='pytorch', device=None):
+    """
+    Calculate the prediction of the label corresponding to image im
+    Param:
+        im: a numpy array image (numpy array), with max size 2048x2048
+    Return:
+        res: the predicted distribution of probability of the labels (numpy array)
+    """        
+    # pad with zeros such that is divisible by 16
+    (nrow, ncol) = im.shape
+    row_add = 16-nrow%16
+    col_add = 16-ncol%16
+    padded = np.pad(im, ((0, row_add), (0, col_add)))
+    
+    if pretrained_weights is None:
+        if mic_type == 'pc':
+            pretrained_weights = path_weights + 'weights_budding_PhC_multilab_0_1'
+        elif mic_type == 'bf':
+            pretrained_weights = path_weights + 'weights_budding_BF_multilab_0_1'
+        elif mic_type == 'fission':
+            pretrained_weights = path_weights + 'weights_fission_multilab_0_2'
+        if model_type == 'tensorflow':
+            pretrained_weights = pretrained_weights + '.hdf5'
+    
+    if not os.path.exists(pretrained_weights):
+        raise ValueError('Path does not exist')
+
+    # WHOLE CELL PREDICTION
+
+    if model_type == 'tensorflow':
+        tf_model = unet(pretrained_weights = pretrained_weights,
+                    input_size = (None,None,1))
+        input = padded[np.newaxis,:,:,np.newaxis]
+        tf_results = tf_model.predict(input, batch_size=1)
+        tf_res = tf_results[0,:,:,0]
+        
+        return tf_res
+
+    elif model_type == 'pytorch':
+        # Load saved weights in pytorch model and run the pytorch model
+        model = UNet()
+        model.load_state_dict(torch.load(pretrained_weights))
+        
+        if torch.cuda.is_available() and device == 'cuda':
+            device = torch.device('cuda')
+            model = model.to(device)
+            padded = torch.from_numpy(padded).to(device)
+            print('device: ', device)
+        else:
+            device = torch.device('cpu')
+            padded = torch.from_numpy(padded)
+            print('device: ', device)
+        model.eval()
+        with torch.no_grad():
+            # Convert input tensor to PyTorch tensor
+            input_tensor = padded.unsqueeze(0).unsqueeze(0).float()
+            # Pass input through the model
+            output_tensor = model.forward(input_tensor)
+            # Convert output tensor to NumPy array
+            output_array = output_tensor.cpu().detach().numpy()
+        pt_res = output_array[0, 0, :, :]
+        
+        # empty cache
+        if (device == 'cuda') and (torch.cuda.is_available()):
+            report_gpu()
+        
+        return pt_res[:nrow, :ncol]
+    
+    
+    else:
+        raise ValueError('model_type is not valid. should be either "pytorch" or "tensorflow".')
```

### Comparing `YeaZ-1.0.0rc1/yeaz/unet/segment.py` & `YeaZ-1.0.1/yeaz/unet/segment.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,168 +1,168 @@
-from scipy import ndimage as ndi
-from skimage.feature import peak_local_max
-from skimage.morphology import dilation
-from skimage.segmentation import watershed
-from skimage.filters import gaussian
-from skimage.measure import label
-
-import numpy as np
-
-
-def segment(th, pred, min_distance=10, topology=None): 
-    """
-    Performs watershed segmentation on thresholded image. Seeds have to
-    have minimal distance of min_distance. topology defines the watershed
-    topology to be used, default is the negative distance transform. 
-    Can either be an array with the same size af th, or a function that will
-    be applied to the distance transform.
-    
-    After watershed, the borders found by watershed will be evaluated in terms
-    of their predicted value. If the borders are highly predicted to be cells,
-    the two cells are merged. 
-    """
-    dtr = ndi.morphology.distance_transform_edt(th)
-    if topology is None:
-        topology = -dtr
-    elif callable(topology):
-        topology = topology(dtr)
-
-    coords = peak_local_max(-topology, min_distance)
-    # to fix deprecation of indices in peak_local_max
-    mask = np.zeros(dtr.shape, dtype=bool)
-    mask[tuple(coords.T)] = True
-    
-    # Uncomment to start with cross for every pixel instead of single pixel
-    m_lab = label(mask) #comment this
-    #m_dil = dilation(m)
-    #m_lab = label(m_dil)
-    wsh = watershed(topology, m_lab, mask=th, connectivity=2)
-    merged = cell_merge(wsh, pred)
-    return correct_artefacts(merged)
-    
-    
-def correct_artefacts(wsh):
-    """
-    Sometimes artefacts arise with 3 or less pixels which are surrounded entirely
-    by another cell. Those are removed here.
-    """
-    unique, count = np.unique(wsh, return_counts=True)
-    to_remove = unique[count<=3]
-    for rem in to_remove:
-        rem_im = wsh==rem
-        rem_cont = dilation(rem_im) & ~rem_im
-        vals, val_counts = np.unique(wsh[rem_cont], return_counts=True)
-        replace_val = vals[np.argmax(val_counts)]
-        if replace_val != 0:
-            wsh[rem_im] = int(replace_val)
-    return wsh
-
-
-def cell_merge(wsh, pred):
-    """
-    Procedure that merges cells if the border between them is predicted to be
-    cell pixels.
-    """
-    wshshape=wsh.shape
-    
-    # masks for the original cells
-    objs = np.zeros((wsh.max()+1,wshshape[0],wshshape[1]), dtype=bool)	
-    
-    # masks for dilated cells
-    dil_objs = np.zeros((wsh.max()+1,wshshape[0],wshshape[1]), dtype=bool)
-    
-    # bounding box coordinates	
-    obj_coords = np.zeros((wsh.max()+1,4))
-    
-    # cleaned watershed, output of function	
-    wshclean = np.zeros((wshshape[0],wshshape[1]))
-    
-    # kernel to dilate objects
-    kernel = np.ones((3,3), dtype=bool)	
-    
-    for obj1 in range(wsh.max()):
-        # create masks and dilated masks for obj
-        objs[obj1,:,:] = wsh==(obj1+1)	
-        dil_objs[obj1,:,:] = dilation(objs[obj1,:,:], kernel)	
-        
-        # bounding box
-        obj_coords[obj1,:] = get_bounding_box(dil_objs[obj1,:,:])
-    
-    objcounter = 0	# counter for new watershed objects
-    
-    for obj1 in range(wsh.max()):	
-        dil1 = dil_objs[obj1,:,:]
-
-        # check if mask has been deleted
-        if np.sum(dil1) == 0:
-            continue
-        
-        objcounter = objcounter + 1
-        orig1 = objs[obj1,:,:]
-        
-        last_obj2_added_to_obj1 = -1
-
-        for obj2 in range(obj1+1,wsh.max()):
-            dil2 = dil_objs[obj2,:,:]
-            
-            # only check border if bounding box overlaps, and second mask 
-            # is not yet deleted
-            if (do_box_overlap(obj_coords[obj1,:], obj_coords[obj2,:])
-                and np.sum(dil2) > 0):
-                
-                border = dil1 * dil2	
-                border_pred = pred[border]
-                
-                # Border is too small to be considered
-                if len(border_pred) < 16:	#SJR: Changed on 18.04.2021 from previously 32. Not sure why 32. I remember 8.
-                    continue
-                
-                # Sum of top 25% of predicted border values
-                q75 = np.quantile(border_pred, .75)
-                top_border_pred = border_pred[border_pred >= q75]
-                top_border_height = top_border_pred.sum()
-                top_border_area = len(top_border_pred)
-                
-                # merge cells
-                if top_border_height / top_border_area > .99:
-                    orig1 = np.logical_or(orig1, objs[obj2,:,:])
-                    dil1 = np.logical_or(dil1, dil2)
-                    dil_objs[obj1,:,:] = dil1
-                    dil_objs[obj2,:,:] = np.zeros((wshshape[0], wshshape[1]))
-                    obj_coords[obj1,:] = get_bounding_box(dil_objs[obj1,:,:])
-#                    obj_coords[obj2,:] = get_bounding_box(dil_objs[obj2,:,:])
-                    last_obj2_added_to_obj1 = obj2
-        
-        # the last object that obj1 was merged with should be equal to obj1 so that additional cells could be merged with it
-        if last_obj2_added_to_obj1 > -1:
-            obj2 = last_obj2_added_to_obj1
-            dil_objs[obj2,:,:] = dil1
-            objs[obj2,:,:] = orig1
-            obj_coords[obj2,:] = get_bounding_box(dil_objs[obj2,:,:])
-            
-                    
-        wshclean = (1-orig1)*wshclean + orig1*objcounter
-        
-    # resort wshclean
-    u = np.unique(wshclean)[1:]	#ignore background
-    for obj1 in range(len(u)):
-        wshclean[wshclean==u[obj1]] = obj1 + 1
-            
-    return wshclean
-
-
-def do_box_overlap(coord1, coord2):
-    """Checks if boxes, determined by their coordinates, overlap. Safety
-    margin of 2 pixels"""
-    return (
-    (coord1[0] - 2 < coord2[0] and coord1[1] + 2 > coord2[0]
-        or coord2[0] - 2 < coord1[0] and coord2[1] + 2 > coord1[0]) 
-    and (coord1[2] - 2 < coord2[2] and coord1[3] + 2 > coord2[2]
-        or coord2[2] - 2 < coord1[2] and coord2[3] + 2 > coord1[2]))
-
-    
-def get_bounding_box(im):
-    """Returns bounding box of object in boolean image"""
-    coords = np.where(im)
-    
-    return np.array([np.min(coords[0]), np.max(coords[0]), 
-                     np.min(coords[1]), np.max(coords[1])])
+from scipy import ndimage as ndi
+from skimage.feature import peak_local_max
+from skimage.morphology import dilation
+from skimage.segmentation import watershed
+from skimage.filters import gaussian
+from skimage.measure import label
+
+import numpy as np
+
+
+def segment(th, pred, min_distance=10, topology=None): 
+    """
+    Performs watershed segmentation on thresholded image. Seeds have to
+    have minimal distance of min_distance. topology defines the watershed
+    topology to be used, default is the negative distance transform. 
+    Can either be an array with the same size af th, or a function that will
+    be applied to the distance transform.
+    
+    After watershed, the borders found by watershed will be evaluated in terms
+    of their predicted value. If the borders are highly predicted to be cells,
+    the two cells are merged. 
+    """
+    dtr = ndi.morphology.distance_transform_edt(th)
+    if topology is None:
+        topology = -dtr
+    elif callable(topology):
+        topology = topology(dtr)
+
+    coords = peak_local_max(-topology, min_distance)
+    # to fix deprecation of indices in peak_local_max
+    mask = np.zeros(dtr.shape, dtype=bool)
+    mask[tuple(coords.T)] = True
+    
+    # Uncomment to start with cross for every pixel instead of single pixel
+    m_lab = label(mask) #comment this
+    #m_dil = dilation(m)
+    #m_lab = label(m_dil)
+    wsh = watershed(topology, m_lab, mask=th, connectivity=2)
+    merged = cell_merge(wsh, pred)
+    return correct_artefacts(merged)
+    
+    
+def correct_artefacts(wsh):
+    """
+    Sometimes artefacts arise with 3 or less pixels which are surrounded entirely
+    by another cell. Those are removed here.
+    """
+    unique, count = np.unique(wsh, return_counts=True)
+    to_remove = unique[count<=3]
+    for rem in to_remove:
+        rem_im = wsh==rem
+        rem_cont = dilation(rem_im) & ~rem_im
+        vals, val_counts = np.unique(wsh[rem_cont], return_counts=True)
+        replace_val = vals[np.argmax(val_counts)]
+        if replace_val != 0:
+            wsh[rem_im] = int(replace_val)
+    return wsh
+
+
+def cell_merge(wsh, pred):
+    """
+    Procedure that merges cells if the border between them is predicted to be
+    cell pixels.
+    """
+    wshshape=wsh.shape
+    
+    # masks for the original cells
+    objs = np.zeros((wsh.max()+1,wshshape[0],wshshape[1]), dtype=bool)	
+    
+    # masks for dilated cells
+    dil_objs = np.zeros((wsh.max()+1,wshshape[0],wshshape[1]), dtype=bool)
+    
+    # bounding box coordinates	
+    obj_coords = np.zeros((wsh.max()+1,4))
+    
+    # cleaned watershed, output of function	
+    wshclean = np.zeros((wshshape[0],wshshape[1]))
+    
+    # kernel to dilate objects
+    kernel = np.ones((3,3), dtype=bool)	
+    
+    for obj1 in range(wsh.max()):
+        # create masks and dilated masks for obj
+        objs[obj1,:,:] = wsh==(obj1+1)	
+        dil_objs[obj1,:,:] = dilation(objs[obj1,:,:], kernel)	
+        
+        # bounding box
+        obj_coords[obj1,:] = get_bounding_box(dil_objs[obj1,:,:])
+    
+    objcounter = 0	# counter for new watershed objects
+    
+    for obj1 in range(wsh.max()):	
+        dil1 = dil_objs[obj1,:,:]
+
+        # check if mask has been deleted
+        if np.sum(dil1) == 0:
+            continue
+        
+        objcounter = objcounter + 1
+        orig1 = objs[obj1,:,:]
+        
+        last_obj2_added_to_obj1 = -1
+
+        for obj2 in range(obj1+1,wsh.max()):
+            dil2 = dil_objs[obj2,:,:]
+            
+            # only check border if bounding box overlaps, and second mask 
+            # is not yet deleted
+            if (do_box_overlap(obj_coords[obj1,:], obj_coords[obj2,:])
+                and np.sum(dil2) > 0):
+                
+                border = dil1 * dil2	
+                border_pred = pred[border]
+                
+                # Border is too small to be considered
+                if len(border_pred) < 16:	#SJR: Changed on 18.04.2021 from previously 32. Not sure why 32. I remember 8.
+                    continue
+                
+                # Sum of top 25% of predicted border values
+                q75 = np.quantile(border_pred, .75)
+                top_border_pred = border_pred[border_pred >= q75]
+                top_border_height = top_border_pred.sum()
+                top_border_area = len(top_border_pred)
+                
+                # merge cells
+                if top_border_height / top_border_area > .99:
+                    orig1 = np.logical_or(orig1, objs[obj2,:,:])
+                    dil1 = np.logical_or(dil1, dil2)
+                    dil_objs[obj1,:,:] = dil1
+                    dil_objs[obj2,:,:] = np.zeros((wshshape[0], wshshape[1]))
+                    obj_coords[obj1,:] = get_bounding_box(dil_objs[obj1,:,:])
+#                    obj_coords[obj2,:] = get_bounding_box(dil_objs[obj2,:,:])
+                    last_obj2_added_to_obj1 = obj2
+        
+        # the last object that obj1 was merged with should be equal to obj1 so that additional cells could be merged with it
+        if last_obj2_added_to_obj1 > -1:
+            obj2 = last_obj2_added_to_obj1
+            dil_objs[obj2,:,:] = dil1
+            objs[obj2,:,:] = orig1
+            obj_coords[obj2,:] = get_bounding_box(dil_objs[obj2,:,:])
+            
+                    
+        wshclean = (1-orig1)*wshclean + orig1*objcounter
+        
+    # resort wshclean
+    u = np.unique(wshclean)[1:]	#ignore background
+    for obj1 in range(len(u)):
+        wshclean[wshclean==u[obj1]] = obj1 + 1
+            
+    return wshclean
+
+
+def do_box_overlap(coord1, coord2):
+    """Checks if boxes, determined by their coordinates, overlap. Safety
+    margin of 2 pixels"""
+    return (
+    (coord1[0] - 2 < coord2[0] and coord1[1] + 2 > coord2[0]
+        or coord2[0] - 2 < coord1[0] and coord2[1] + 2 > coord1[0]) 
+    and (coord1[2] - 2 < coord2[2] and coord1[3] + 2 > coord2[2]
+        or coord2[2] - 2 < coord1[2] and coord2[3] + 2 > coord1[2]))
+
+    
+def get_bounding_box(im):
+    """Returns bounding box of object in boolean image"""
+    coords = np.where(im)
+    
+    return np.array([np.min(coords[0]), np.max(coords[0]), 
+                     np.min(coords[1]), np.max(coords[1])])
```

### Comparing `YeaZ-1.0.0rc1/yeaz/unet/utils.py` & `YeaZ-1.0.1/yeaz/unet/utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-
-from model_pytorch import UNet
-from model_tensorflow import unet
-import torch
-import tensorflow as tf
-
-def weight_loading(pretrained_weights):
-    # Load the weights
-    tf_model = tf.keras.models.load_model(pretrained_weights)
-    tf_weights = tf_model.get_weights()
-
-    # Load the PyTorch model
-    pt_model = UNet() #implemented based on the previous model (by myself)
-    initial_state_dict = pt_model.state_dict()
-    new_state_dict = {}
-    with torch.no_grad():
-        x = 0
-        for i, layer in enumerate(pt_model.modules()):
-            if isinstance(layer, torch.nn.Conv2d) or isinstance(layer, torch.nn.Linear):
-                # extract the weights and biases from the TensorFlow weights
-                weight_tf = tf_weights[x*2]
-                bias_tf = tf_weights[x*2+1]
-
-                # convert the weights and biases to PyTorch format
-                layer.weight.data = torch.tensor(weight_tf.transpose(3, 2, 0, 1), dtype=torch.float)
-                layer.bias.data = torch.tensor(bias_tf, dtype=torch.float)
-
-                x = x + 1
-
-            if isinstance(layer, torch.nn.ConvTranspose2d):
-                weight_tf = tf_weights[x*2]
-                bias_tf = tf_weights[x*2+1]
-                
-                # convert the weights and biases to PyTorch format
-                layer.weight.data = torch.tensor(weight_tf.transpose(2, 3, 0, 1), dtype=torch.float)
-                layer.bias.data = torch.tensor(bias_tf, dtype=torch.float)
-                
-                x = x + 1
-    return pt_model
+
+from model_pytorch import UNet
+from model_tensorflow import unet
+import torch
+import tensorflow as tf
+
+def weight_loading(pretrained_weights):
+    # Load the weights
+    tf_model = tf.keras.models.load_model(pretrained_weights)
+    tf_weights = tf_model.get_weights()
+
+    # Load the PyTorch model
+    pt_model = UNet() #implemented based on the previous model (by myself)
+    initial_state_dict = pt_model.state_dict()
+    new_state_dict = {}
+    with torch.no_grad():
+        x = 0
+        for i, layer in enumerate(pt_model.modules()):
+            if isinstance(layer, torch.nn.Conv2d) or isinstance(layer, torch.nn.Linear):
+                # extract the weights and biases from the TensorFlow weights
+                weight_tf = tf_weights[x*2]
+                bias_tf = tf_weights[x*2+1]
+
+                # convert the weights and biases to PyTorch format
+                layer.weight.data = torch.tensor(weight_tf.transpose(3, 2, 0, 1), dtype=torch.float)
+                layer.bias.data = torch.tensor(bias_tf, dtype=torch.float)
+
+                x = x + 1
+
+            if isinstance(layer, torch.nn.ConvTranspose2d):
+                weight_tf = tf_weights[x*2]
+                bias_tf = tf_weights[x*2+1]
+                
+                # convert the weights and biases to PyTorch format
+                layer.weight.data = torch.tensor(weight_tf.transpose(2, 3, 0, 1), dtype=torch.float)
+                layer.bias.data = torch.tensor(bias_tf, dtype=torch.float)
+                
+                x = x + 1
+    return pt_model
```

