# Comparing `tmp/UNET_MDLE_CASE-0.1.tar.gz` & `tmp/UNET_MDLE_CASE-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UNET_MDLE_CASE-0.1.tar", last modified: Wed Jul 26 17:25:47 2023, max compression
+gzip compressed data, was "UNET_MDLE_CASE-0.2.tar", last modified: Wed Jul 26 17:56:56 2023, max compression
```

## Comparing `UNET_MDLE_CASE-0.1.tar` & `UNET_MDLE_CASE-0.2.tar`

### file list

```diff
@@ -1,10 +1,21 @@
-drwxr-xr-x   0 zxu4     (1123124) rxf131   (10097)        0 2023-07-26 17:25:47.036695 UNET_MDLE_CASE-0.1/
--rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      343 2023-07-26 17:25:47.036356 UNET_MDLE_CASE-0.1/PKG-INFO
-drwxr-xr-x   0 zxu4     (1123124) rxf131   (10097)        0 2023-07-26 17:25:47.027265 UNET_MDLE_CASE-0.1/UNET_MDLE_CASE.egg-info/
--rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      343 2023-07-26 17:25:46.000000 UNET_MDLE_CASE-0.1/UNET_MDLE_CASE.egg-info/PKG-INFO
--rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      197 2023-07-26 17:25:46.000000 UNET_MDLE_CASE-0.1/UNET_MDLE_CASE.egg-info/SOURCES.txt
--rw-r--r--   0 zxu4     (1123124) rxf131   (10097)        1 2023-07-26 17:25:46.000000 UNET_MDLE_CASE-0.1/UNET_MDLE_CASE.egg-info/dependency_links.txt
--rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      159 2023-07-26 17:25:46.000000 UNET_MDLE_CASE-0.1/UNET_MDLE_CASE.egg-info/requires.txt
--rw-r--r--   0 zxu4     (1123124) rxf131   (10097)        1 2023-07-26 17:25:46.000000 UNET_MDLE_CASE-0.1/UNET_MDLE_CASE.egg-info/top_level.txt
--rw-r--r--   0 zxu4     (1123124) rxf131   (10097)       38 2023-07-26 17:25:47.039938 UNET_MDLE_CASE-0.1/setup.cfg
--rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      603 2023-07-26 17:24:25.000000 UNET_MDLE_CASE-0.1/setup.py
+drwxr-xr-x   0 zxu4     (1123124) rxf131   (10097)        0 2023-07-26 17:56:56.783837 UNET_MDLE_CASE-0.2/
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      343 2023-07-26 17:56:56.782488 UNET_MDLE_CASE-0.2/PKG-INFO
+drwxr-xr-x   0 zxu4     (1123124) rxf131   (10097)        0 2023-07-26 17:56:55.817846 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)     3655 2023-07-26 16:35:05.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/XY.py
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      270 2023-07-26 15:13:41.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/__init__.py
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)     4737 2023-07-26 15:09:54.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/arc_unet.py
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)     2174 2023-07-26 15:10:46.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/gen_video.py
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)     3187 2023-07-26 15:17:06.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/pipeline.py
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)     1485 2023-07-26 15:11:36.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/plot_epochs.py
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)     1698 2023-07-26 15:11:59.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/pullcsv.py
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)     2848 2023-07-26 15:11:56.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/resizedim.py
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)     2018 2023-07-26 15:12:07.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/test_iou.py
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)     3339 2023-07-26 15:17:32.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE/train.py
+drwxr-xr-x   0 zxu4     (1123124) rxf131   (10097)        0 2023-07-26 17:56:56.629821 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE.egg-info/
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      343 2023-07-26 17:56:53.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE.egg-info/PKG-INFO
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      462 2023-07-26 17:56:54.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE.egg-info/SOURCES.txt
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)        1 2023-07-26 17:56:53.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE.egg-info/dependency_links.txt
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      159 2023-07-26 17:56:54.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE.egg-info/requires.txt
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)       15 2023-07-26 17:56:54.000000 UNET_MDLE_CASE-0.2/UNET_MDLE_CASE.egg-info/top_level.txt
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)       38 2023-07-26 17:56:56.807921 UNET_MDLE_CASE-0.2/setup.cfg
+-rw-r--r--   0 zxu4     (1123124) rxf131   (10097)      656 2023-07-26 17:56:37.000000 UNET_MDLE_CASE-0.2/setup.py
```

### Comparing `UNET_MDLE_CASE-0.1/setup.py` & `UNET_MDLE_CASE-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UNET_MDLE_CASE',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=['opencv-python>=4.7.0', 'numpy>=1.21.5', 'scikit-image>=0.20.0', 'pandas>=2.0.2', 'tqdm>=4.65.0', 'scikit-learn>=0.0.post1', 'matplotlib>=3.3.4', 'seaborn>=0.11.1', 'tensorflow>=2.0.0'],
     author='Zhuldyz Ualikhankyzy, Thomas Ciardi',
     author_email='zxu4@example.com, tgc17@case.edu',
     description='Package that helps to load data for, build, train, test, and visualize the results of UNET CNN',
     url='https://github.com/juldyzmurat/UNET',
+    package_data={'UNET_MDLE_CASE': ['examples/*']},
 )
```

