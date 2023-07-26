# Comparing `tmp/aotpy-0.8.1.tar.gz` & `tmp/aotpy-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aotpy-0.8.1.tar", last modified: Mon Jul 24 13:09:45 2023, max compression
+gzip compressed data, was "aotpy-0.8.2.tar", last modified: Wed Jul 26 16:34:13 2023, max compression
```

## Comparing `aotpy-0.8.1.tar` & `aotpy-0.8.2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:45.002474 aotpy-0.8.1/
--rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.8.1/LICENSE
--rw-rw-rw-   0        0        0     2997 2023-07-24 13:09:45.002474 aotpy-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2023-05-02 22:45:22.000000 aotpy-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.938486 aotpy-0.8.1/aotpy/
--rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.8.1/aotpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.958016 aotpy-0.8.1/aotpy/core/
--rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.8.1/aotpy/core/__init__.py
--rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.8.1/aotpy/core/aberration.py
--rw-rw-rw-   0        0        0     5304 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/core/ao_system.py
--rw-rw-rw-   0        0        0     3050 2023-07-17 15:15:05.000000 aotpy-0.8.1/aotpy/core/atmosphere.py
--rw-rw-rw-   0        0        0     1162 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/core/base.py
--rw-rw-rw-   0        0        0     1338 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/core/image.py
--rw-rw-rw-   0        0        0     5293 2023-07-17 15:13:26.000000 aotpy-0.8.1/aotpy/core/loop.py
--rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.8.1/aotpy/core/optical_sensor.py
--rw-rw-rw-   0        0        0     2863 2023-05-22 10:44:57.000000 aotpy-0.8.1/aotpy/core/source.py
--rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-0.8.1/aotpy/core/telescope.py
--rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-0.8.1/aotpy/core/time.py
--rw-rw-rw-   0        0        0     3552 2023-07-17 10:39:59.000000 aotpy-0.8.1/aotpy/core/wavefront_corrector.py
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.958994 aotpy-0.8.1/aotpy/data/
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.961924 aotpy-0.8.1/aotpy/data/ERIS/
--rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.8.1/aotpy/data/ERIS/ho_subap.fits
--rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-0.8.1/aotpy/data/ERIS/lo_subap.fits
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.963876 aotpy-0.8.1/aotpy/data/GALACSI/
--rw-rw-rw-   0        0        0    11520 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/data/GALACSI/subap.fits
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.964852 aotpy-0.8.1/aotpy/data/NAOMI/
--rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-0.8.1/aotpy/data/NAOMI/zernike_control_modes.fits
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.980988 aotpy-0.8.1/aotpy/data/PAPYRUS/
--rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-0.8.1/aotpy/data/PAPYRUS/T152_pupil.fits
--rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.8.1/aotpy/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.984893 aotpy-0.8.1/aotpy/io/
--rw-rw-rw-   0        0        0      436 2023-06-19 16:50:12.000000 aotpy-0.8.1/aotpy/io/__init__.py
--rw-rw-rw-   0        0        0     2789 2023-06-19 16:50:12.000000 aotpy-0.8.1/aotpy/io/base.py
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.991728 aotpy-0.8.1/aotpy/io/fits/
--rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.8.1/aotpy/io/fits/__init__.py
--rw-rw-rw-   0        0        0    26755 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/io/fits/_keywords.py
--rw-rw-rw-   0        0        0    41933 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/io/fits/reader.py
--rw-rw-rw-   0        0        0     9313 2023-07-24 13:06:09.000000 aotpy-0.8.1/aotpy/io/fits/utils.py
--rw-rw-rw-   0        0        0    31367 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/io/fits/writer.py
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:45.000517 aotpy-0.8.1/aotpy/translators/
--rw-rw-rw-   0        0        0      440 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/__init__.py
--rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-0.8.1/aotpy/translators/base.py
--rw-rw-rw-   0        0        0     7087 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/ciao.py
--rw-rw-rw-   0        0        0    18377 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/eris.py
--rw-rw-rw-   0        0        0    10376 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/eso.py
--rw-rw-rw-   0        0        0    11408 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/galacsi.py
--rw-rw-rw-   0        0        0     7494 2023-07-24 12:45:59.000000 aotpy-0.8.1/aotpy/translators/naomi.py
--rw-rw-rw-   0        0        0    12582 2023-07-24 13:05:57.000000 aotpy-0.8.1/aotpy/translators/papyrus.py
-drwxrwxrwx   0        0        0        0 2023-07-24 13:09:44.944345 aotpy-0.8.1/aotpy.egg-info/
--rw-rw-rw-   0        0        0     2997 2023-07-24 13:09:44.000000 aotpy-0.8.1/aotpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2023-07-24 13:09:44.000000 aotpy-0.8.1/aotpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 13:09:44.000000 aotpy-0.8.1/aotpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      138 2023-07-24 13:09:44.000000 aotpy-0.8.1/aotpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-24 13:09:44.000000 aotpy-0.8.1/aotpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0     1029 2023-07-24 13:09:45.003452 aotpy-0.8.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.174644 aotpy-0.8.2/
+-rw-rw-rw-   0        0        0     1592 2022-07-17 01:57:35.000000 aotpy-0.8.2/LICENSE
+-rw-rw-rw-   0        0        0     3108 2023-07-26 16:34:13.174644 aotpy-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2309 2023-07-26 16:33:12.000000 aotpy-0.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.122675 aotpy-0.8.2/aotpy/
+-rw-rw-rw-   0        0        0      521 2023-05-03 10:25:00.000000 aotpy-0.8.2/aotpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.138676 aotpy-0.8.2/aotpy/core/
+-rw-rw-rw-   0        0        0      555 2023-05-08 11:52:45.000000 aotpy-0.8.2/aotpy/core/__init__.py
+-rw-rw-rw-   0        0        0     1073 2023-05-02 09:36:00.000000 aotpy-0.8.2/aotpy/core/aberration.py
+-rw-rw-rw-   0        0        0     5304 2023-07-17 15:33:42.000000 aotpy-0.8.2/aotpy/core/ao_system.py
+-rw-rw-rw-   0        0        0     3050 2023-07-17 15:15:05.000000 aotpy-0.8.2/aotpy/core/atmosphere.py
+-rw-rw-rw-   0        0        0     1162 2023-07-17 10:40:27.000000 aotpy-0.8.2/aotpy/core/base.py
+-rw-rw-rw-   0        0        0     1338 2023-07-17 12:24:43.000000 aotpy-0.8.2/aotpy/core/image.py
+-rw-rw-rw-   0        0        0     5293 2023-07-17 15:13:26.000000 aotpy-0.8.2/aotpy/core/loop.py
+-rw-rw-rw-   0        0        0    11452 2023-05-08 11:39:26.000000 aotpy-0.8.2/aotpy/core/optical_sensor.py
+-rw-rw-rw-   0        0        0     2863 2023-05-22 10:44:57.000000 aotpy-0.8.2/aotpy/core/source.py
+-rw-rw-rw-   0        0        0     4887 2023-06-19 16:50:55.000000 aotpy-0.8.2/aotpy/core/telescope.py
+-rw-rw-rw-   0        0        0      706 2023-06-19 16:50:55.000000 aotpy-0.8.2/aotpy/core/time.py
+-rw-rw-rw-   0        0        0     3552 2023-07-17 10:39:59.000000 aotpy-0.8.2/aotpy/core/wavefront_corrector.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.142674 aotpy-0.8.2/aotpy/data/
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.142674 aotpy-0.8.2/aotpy/data/ERIS/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.8.2/aotpy/data/ERIS/ho_subap.fits
+-rw-rw-rw-   0        0        0     5760 2023-06-19 12:38:42.000000 aotpy-0.8.2/aotpy/data/ERIS/lo_subap.fits
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.142674 aotpy-0.8.2/aotpy/data/GALACSI/
+-rw-rw-rw-   0        0        0    11520 2023-04-03 16:42:38.000000 aotpy-0.8.2/aotpy/data/GALACSI/subap.fits
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.146679 aotpy-0.8.2/aotpy/data/NAOMI/
+-rw-rw-rw-   0        0        0  7344000 2023-05-03 14:12:48.000000 aotpy-0.8.2/aotpy/data/NAOMI/zernike_control_modes.fits
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.154652 aotpy-0.8.2/aotpy/data/PAPYRUS/
+-rw-rw-rw-   0        0        0  1013760 2023-06-19 15:05:10.000000 aotpy-0.8.2/aotpy/data/PAPYRUS/T152_pupil.fits
+-rw-rw-rw-   0        0        0      105 2023-05-02 18:50:46.000000 aotpy-0.8.2/aotpy/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.158644 aotpy-0.8.2/aotpy/io/
+-rw-rw-rw-   0        0        0      436 2023-06-19 16:50:12.000000 aotpy-0.8.2/aotpy/io/__init__.py
+-rw-rw-rw-   0        0        0     2789 2023-06-19 16:50:12.000000 aotpy-0.8.2/aotpy/io/base.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.162644 aotpy-0.8.2/aotpy/io/fits/
+-rw-rw-rw-   0        0        0      200 2023-05-02 13:23:11.000000 aotpy-0.8.2/aotpy/io/fits/__init__.py
+-rw-rw-rw-   0        0        0    26722 2023-07-25 11:24:17.000000 aotpy-0.8.2/aotpy/io/fits/_keywords.py
+-rw-rw-rw-   0        0        0    40528 2023-07-25 15:30:54.000000 aotpy-0.8.2/aotpy/io/fits/reader.py
+-rw-rw-rw-   0        0        0     9313 2023-07-24 13:06:09.000000 aotpy-0.8.2/aotpy/io/fits/utils.py
+-rw-rw-rw-   0        0        0    31347 2023-07-26 14:41:33.000000 aotpy-0.8.2/aotpy/io/fits/writer.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.174644 aotpy-0.8.2/aotpy/translators/
+-rw-rw-rw-   0        0        0      440 2023-06-28 16:02:08.000000 aotpy-0.8.2/aotpy/translators/__init__.py
+-rw-rw-rw-   0        0        0      981 2023-06-19 16:46:11.000000 aotpy-0.8.2/aotpy/translators/base.py
+-rw-rw-rw-   0        0        0     7166 2023-07-25 17:10:27.000000 aotpy-0.8.2/aotpy/translators/ciao.py
+-rw-rw-rw-   0        0        0    18440 2023-07-26 15:13:13.000000 aotpy-0.8.2/aotpy/translators/eris.py
+-rw-rw-rw-   0        0        0    10740 2023-07-26 16:13:22.000000 aotpy-0.8.2/aotpy/translators/eso.py
+-rw-rw-rw-   0        0        0    11473 2023-07-25 17:13:23.000000 aotpy-0.8.2/aotpy/translators/galacsi.py
+-rw-rw-rw-   0        0        0     7574 2023-07-25 17:10:28.000000 aotpy-0.8.2/aotpy/translators/naomi.py
+-rw-rw-rw-   0        0        0    12588 2023-07-26 10:27:29.000000 aotpy-0.8.2/aotpy/translators/papyrus.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:34:13.126675 aotpy-0.8.2/aotpy.egg-info/
+-rw-rw-rw-   0        0        0     3108 2023-07-26 16:34:13.000000 aotpy-0.8.2/aotpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2023-07-26 16:34:13.000000 aotpy-0.8.2/aotpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 16:34:13.000000 aotpy-0.8.2/aotpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      138 2023-07-26 16:34:13.000000 aotpy-0.8.2/aotpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 16:34:13.000000 aotpy-0.8.2/aotpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-11-05 13:42:41.000000 aotpy-0.8.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1029 2023-07-26 16:34:13.174644 aotpy-0.8.2/setup.cfg
```

### Comparing `aotpy-0.8.1/LICENSE` & `aotpy-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/PKG-INFO` & `aotpy-0.8.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.8.1
+Version: 0.8.2
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/STAR-PORT/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/STAR-PORT/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -16,14 +16,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: esoarchive
 Provides-Extra: savfiles
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8187230.svg)](https://doi.org/10.5281/zenodo.8187230)
+
+
 # aotpy
 Helper Python package for handling Adaptive Optics Telemetry (AOT) standard files.
 Basic [documentation available](https://aotpy.readthedocs.io/en/latest/).
 
 ## How to install
 Support is offered for Python 3.10 or later.
```

### Comparing `aotpy-0.8.1/README.md` & `aotpy-0.8.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8187230.svg)](https://doi.org/10.5281/zenodo.8187230)
+
+
 # aotpy
 Helper Python package for handling Adaptive Optics Telemetry (AOT) standard files.
 Basic [documentation available](https://aotpy.readthedocs.io/en/latest/).
 
 ## How to install
 Support is offered for Python 3.10 or later.
```

### Comparing `aotpy-0.8.1/aotpy/__init__.py` & `aotpy-0.8.2/aotpy/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/__init__.py` & `aotpy-0.8.2/aotpy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/aberration.py` & `aotpy-0.8.2/aotpy/core/aberration.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/ao_system.py` & `aotpy-0.8.2/aotpy/core/ao_system.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/atmosphere.py` & `aotpy-0.8.2/aotpy/core/atmosphere.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/base.py` & `aotpy-0.8.2/aotpy/core/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/image.py` & `aotpy-0.8.2/aotpy/core/image.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/loop.py` & `aotpy-0.8.2/aotpy/core/loop.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/optical_sensor.py` & `aotpy-0.8.2/aotpy/core/optical_sensor.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/source.py` & `aotpy-0.8.2/aotpy/core/source.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/telescope.py` & `aotpy-0.8.2/aotpy/core/telescope.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/time.py` & `aotpy-0.8.2/aotpy/core/time.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/core/wavefront_corrector.py` & `aotpy-0.8.2/aotpy/core/wavefront_corrector.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/data/ERIS/ho_subap.fits` & `aotpy-0.8.2/aotpy/data/ERIS/ho_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/data/ERIS/lo_subap.fits` & `aotpy-0.8.2/aotpy/data/ERIS/lo_subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/data/GALACSI/subap.fits` & `aotpy-0.8.2/aotpy/data/GALACSI/subap.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/data/NAOMI/zernike_control_modes.fits` & `aotpy-0.8.2/aotpy/data/NAOMI/zernike_control_modes.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/data/PAPYRUS/T152_pupil.fits` & `aotpy-0.8.2/aotpy/data/PAPYRUS/T152_pupil.fits`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/io/base.py` & `aotpy-0.8.2/aotpy/io/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/io/fits/_keywords.py` & `aotpy-0.8.2/aotpy/io/fits/_keywords.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         return FLOAT_FORMAT
     if fits_type in ['B', 'I', 'J', 'K']:
         return INTEGER_FORMAT
     if re.fullmatch(r'\d*A', fits_type):
         return STRING_FORMAT
     if re.fullmatch(r'[QP][DE]\(\d*\)', fits_type):
         return LIST_FORMAT
-    raise ValueError('Format not in AOT FITS')
+    return ''
 
 
 STRING_FORMAT = 'str'  # e.g. 64A
 INTEGER_FORMAT = 'int'  # e.g. K
 FLOAT_FORMAT = 'flt'  # e.g. D
 LIST_FORMAT = 'lst'  # e.g. QD
```

### Comparing `aotpy-0.8.1/aotpy/io/fits/reader.py` & `aotpy-0.8.2/aotpy/io/fits/reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,55 +12,14 @@
 import aotpy
 from . import _keywords as kw
 from .utils import FITSURLImage, FITSFileImage, image_from_hdu, keyword_is_relevant, metadatum_from_card
 from ..base import SystemReader
 
 _reference_pattern = re.compile(r'([^<]+)<(.+)>(\d+)?')
 
-
-def _type_matches(aot_format: str, fits_type: str) -> bool:
-    try:
-        return aot_format == kw.fits_type_to_aot(fits_type)
-    except ValueError:
-        return False
-
-
-def _convert_row(columns: fits.ColDefs, row: fits.FITS_record, fields: kw.AOTFieldDict) -> dict:
-    res = {}
-    for name, field in fields.items():
-        try:
-            value = row[name]
-        except KeyError:
-            value = None
-
-        match field.format:
-            case kw.STRING_FORMAT:
-                if value == '':
-                    value = None
-            case kw.LIST_FORMAT:
-                if value is None:
-                    value = []
-                value = [None if np.isnan(v) else v for v in value]
-            case kw.FLOAT_FORMAT:
-                if np.isnan(value):
-                    value = None
-            case kw.INTEGER_FORMAT:
-                if value is not None:
-                    col = columns[name]
-                    if col.null and value == col.null:
-                        value = None
-            case _:
-                raise RuntimeError  # This should never happen
-        if value is None and field.mandatory:
-            # This will never trigger in list fields, but it's ok because we don't have mandatory list fields
-            raise ValueError(f"Found null value in mandatory field '{name}'")
-        res[name] = value
-    return res
-
-
 def read_system_from_fits(filename: str, extra_data: bool = False, **kwargs) -> aotpy.AOSystem:
     """
     Get `AOSystem` from FITS file specified by `filename`.
 
     Parameters
     ----------
     filename
@@ -231,51 +190,98 @@
         for card in self._primary_header.cards:
             if card.keyword not in kw.AOT_HEADER_SET and keyword_is_relevant(card.keyword):
                 metadata.append(metadatum_from_card(card))
 
         return aotpy.AOSystem(ao_mode=ao_mode, date_beginning=beg, date_end=end, name=name, strehl_ratio=strehl_ratio,
                               temporal_error=temporal_error, config=config, metadata=metadata)
 
-    def _check_bintable(self, hdus: fits.HDUList, table_name: str):
-        fields = kw.TABLE_FIELDS[table_name]
-        table = hdus[table_name]
-        if not isinstance(table, fits.BinTableHDU):
-            raise ValueError(f"HDU '{table.name}' must be a binary table")
+    def _check_and_convert_rows(self, table: fits.BinTableHDU) -> list[dict]:
+        fields = kw.TABLE_FIELDS[table.name]
 
-        field_count = {field: 0 for field in fields}
+        converted_rows = [{} for _ in range(len(table.data))]
+        field_found = {field: False for field in fields}
         for col in table.columns.columns:
-            if col.name in field_count:
-                field_count[col.name] += 1
+            if col.name in field_found:
+                if field_found[col.name]:
+                    warnings.warn(f"Column '{col.name}' appears repeated in table '{table.name}'. "
+                                  f"Ignoring repeated instance.")
+                    continue
+                field_found[col.name] = True
                 field = fields[col.name]
-                if not _type_matches(field.format, col.format):
-                    raise ValueError(f"Column '{col.name}' in table '{table_name}' must be a '{field.format}'"
-                                     f" field (found '{col.format}')")
+
+                for row, d in zip(table.data, converted_rows, strict=True):
+                    value = row[col.name]
+                    match kw.fits_type_to_aot(col.format):
+                        case kw.STRING_FORMAT:
+                            if value == '':
+                                value = None
+                        case kw.LIST_FORMAT:
+                            if value is None:
+                                value = []
+                            value = [None if np.isnan(v) else v for v in value]
+                        case kw.FLOAT_FORMAT:
+                            if np.isnan(value):
+                                value = None
+                        case kw.INTEGER_FORMAT:
+                            if col.null and value == col.null:
+                                value = None
+                        case _:
+                            value = None
+                    if value is None and field.mandatory:
+                        # Never triggers in list fields, but it's ok because we don't have mandatory list fields
+                        raise ValueError(f"Found null value in mandatory field '{col.name}'")
+                    d[col.name] = value
+                if field.format != kw.fits_type_to_aot(col.format):
+                    # Column does not have the expected format
+                    if field.mandatory:
+                        # If it is mandatory we cannot accept a wrong format even if it is filled
+                        raise ValueError(f"Mandatory column '{col.name}' in table '{table.name}' must be a "
+                                         f"'{field.format}' field (found '{col.format}')")
+                    else:
+                        # If the column has any data in it, we need to throw a warning
+                        for d in converted_rows:
+                            value = d[col.name]
+                            if (value is not None) and (value != []):
+                                warnings.warn(f"Ignored column '{col.name}' in table '{table.name}' due to unexpected "
+                                              f"format: (got '{field.format}', expected '{col.format}').")
+                                break
+
                 if col.unit != field.unit:
-                    warnings.warn(f"Column '{col.name}' in table '{table_name}' does not have a standard unit. "
+                    warnings.warn(f"Column '{col.name}' in table '{table.name}' does not have a standard unit. "
                                   f"Found '{col.unit}', expected '{field.unit}'")
                 if field.unique:
                     u = table.data[col.name]
                     if len(np.unique(u)) != len(u):
                         raise ValueError(
-                            f"Column '{col.name}' in table '{table_name}' must have unique values.")
+                            f"Column '{col.name}' in table '{table.name}' must have unique values.")
             else:
-                self._extra_columns.setdefault(table_name, []).append(col)
-        if table_name in self._extra_columns and not self._extra_data_flag:
-            warnings.warn(f"""Table '{table_name}' contains non-AOT columns that were ignored: """
-                          f"""{', '.join([f"'{x.name}'" for x in self._extra_columns[table_name]])}""")
-
-        for name, count in field_count.items():
-            if count < 1:
-                warnings.warn(f"Column '{name}' missing in table '{table_name}'.")
-            if count > 1:
-                raise ValueError(f"Column '{name}' cannot appear repeated in table '{table_name}'.")
+                self._extra_columns.setdefault(table.name, []).append(col)
+        if table.name in self._extra_columns and not self._extra_data_flag:
+            warnings.warn(f"""Table '{table.name}' contains non-AOT columns that were ignored: """
+                          f"""{', '.join([f"'{x.name}'" for x in self._extra_columns[table.name]])}""")
+
+        for name, found in field_found.items():
+            if not found:
+                field = fields[name]
+                if field.mandatory:
+                    raise ValueError(f"Mandatory column '{name}' in table '{table.name}' is missing.")
+                warnings.warn(f"Column '{name}' missing in table '{table.name}'. Assuming null data.")
+                # If the column does not exist, we create it but empty
+                if field.format == kw.LIST_FORMAT:
+                    value = []
+                else:
+                    value = None
+                for d in converted_rows:
+                    d[name] = value
 
-        seq = [field_name for field_name, count in field_count.items() if count > 0]
+        seq = [field_name for field_name, found in field_found.items() if found]
         if seq != [col.name for col, _ in zip(table.columns.columns, seq)]:
-            warnings.warn(f"Non-AOT column sequence in table '{table_name}'.")
+            warnings.warn(f"Non-AOT column sequence in table '{table.name}'.")
+
+        return converted_rows
 
     def _handle_image(self, ref: str):
         if ref is None:
             return None
         fullmatch = _reference_pattern.fullmatch(ref)
         if fullmatch is None:
             warnings.warn(f"Image reference '{ref}' was ignored: not properly formatted.")
@@ -345,368 +351,312 @@
             if unused:
                 self._extra_objects.extend(unused.values())
                 if not self._extra_data_flag:
                     warnings.warn(f"""File contains some {name} were ignored for never being referenced: """
                                   f"""{', '.join([f"'{x}'" for x in unused])}""")
 
     def _handle_time(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.TIME_TABLE)
-
-        table = hdus[kw.TIME_TABLE]
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.TIME_FIELDS)
-
-            self._time[data[kw.REFERENCE_UID]] = [aotpy.Time(
-                uid=data[kw.REFERENCE_UID],
-                timestamps=data[kw.TIME_TIMESTAMPS],
-                frame_numbers=data[kw.TIME_FRAME_NUMBERS]
+        for row in self._check_and_convert_rows(hdus[kw.TIME_TABLE]):
+            self._time[row[kw.REFERENCE_UID]] = [aotpy.Time(
+                uid=row[kw.REFERENCE_UID],
+                timestamps=row[kw.TIME_TIMESTAMPS],
+                frame_numbers=row[kw.TIME_FRAME_NUMBERS]
             ), False]
 
     def _handle_atmosphere(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.ATMOSPHERIC_PARAMETERS_TABLE)
-
-        table = hdus[kw.ATMOSPHERIC_PARAMETERS_TABLE]
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.ATMOSPHERIC_PARAMETERS_FIELDS)
-
+        for row in self._check_and_convert_rows(hdus[kw.ATMOSPHERIC_PARAMETERS_TABLE]):
             self._system.atmosphere_params.append(
                 aotpy.AtmosphericParameters(
-                    uid=data[kw.REFERENCE_UID],
-                    wavelength=data[kw.ATMOSPHERIC_PARAMETERS_WAVELENGTH],
-                    time=self._handle_reference(data[kw.TIME_REFERENCE], kw.TIME_TABLE),
-                    r0=data[kw.ATMOSPHERIC_PARAMETERS_R0],
-                    fwhm=data[kw.ATMOSPHERIC_PARAMETERS_FWHM],
-                    tau0=data[kw.ATMOSPHERIC_PARAMETERS_TAU0],
-                    theta0=data[kw.ATMOSPHERIC_PARAMETERS_THETA0],
-                    layers_weight=self._handle_image(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WEIGHT]),
-                    layers_height=self._handle_image(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_HEIGHT]),
-                    layers_l0=self._handle_image(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_L0]),
-                    layers_wind_speed=self._handle_image(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WIND_SPEED]),
-                    layers_wind_direction=self._handle_image(data[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WIND_DIRECTION]),
-                    transformation_matrix=self._handle_image(data[kw.TRANSFORMATION_MATRIX])
+                    uid=row[kw.REFERENCE_UID],
+                    wavelength=row[kw.ATMOSPHERIC_PARAMETERS_WAVELENGTH],
+                    time=self._handle_reference(row[kw.TIME_REFERENCE], kw.TIME_TABLE),
+                    r0=row[kw.ATMOSPHERIC_PARAMETERS_R0],
+                    fwhm=row[kw.ATMOSPHERIC_PARAMETERS_FWHM],
+                    tau0=row[kw.ATMOSPHERIC_PARAMETERS_TAU0],
+                    theta0=row[kw.ATMOSPHERIC_PARAMETERS_THETA0],
+                    layers_weight=self._handle_image(row[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WEIGHT]),
+                    layers_height=self._handle_image(row[kw.ATMOSPHERIC_PARAMETERS_LAYERS_HEIGHT]),
+                    layers_l0=self._handle_image(row[kw.ATMOSPHERIC_PARAMETERS_LAYERS_L0]),
+                    layers_wind_speed=self._handle_image(row[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WIND_SPEED]),
+                    layers_wind_direction=self._handle_image(row[kw.ATMOSPHERIC_PARAMETERS_LAYERS_WIND_DIRECTION]),
+                    transformation_matrix=self._handle_image(row[kw.TRANSFORMATION_MATRIX])
                 )
             )
 
     def _handle_aberrations(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.ABERRATIONS_TABLE)
-
-        table = hdus[kw.ABERRATIONS_TABLE]
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.ABERRATION_FIELDS)
-
-            self._aberrations[data[kw.REFERENCE_UID]] = [aotpy.Aberration(
-                uid=data[kw.REFERENCE_UID],
-                modes=self._handle_image(data[kw.ABERRATION_MODES]),
-                coefficients=self._handle_image(data[kw.ABERRATION_COEFFICIENTS]),
+        for row in self._check_and_convert_rows(hdus[kw.ABERRATIONS_TABLE]):
+            self._aberrations[row[kw.REFERENCE_UID]] = [aotpy.Aberration(
+                uid=row[kw.REFERENCE_UID],
+                modes=self._handle_image(row[kw.ABERRATION_MODES]),
+                coefficients=self._handle_image(row[kw.ABERRATION_COEFFICIENTS]),
                 offsets=[aotpy.Coordinates(x, y)
-                         for x, y in zip(data[kw.ABERRATION_X_OFFSETS], data[kw.ABERRATION_Y_OFFSETS])],
+                         for x, y in zip(row[kw.ABERRATION_X_OFFSETS], row[kw.ABERRATION_Y_OFFSETS])],
             ), False]
 
     def _handle_telescopes(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.TELESCOPES_TABLE)
-
-        table = hdus[kw.TELESCOPES_TABLE]
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.TELESCOPE_FIELDS)
-
-            uid = data[kw.REFERENCE_UID]
-            t = data[kw.TELESCOPE_TYPE]
+        for row in self._check_and_convert_rows(hdus[kw.TELESCOPES_TABLE]):
+            uid = row[kw.REFERENCE_UID]
+            t = row[kw.TELESCOPE_TYPE]
             if t == kw.TELESCOPE_TYPE_MAIN:
                 if self._system.main_telescope is not None:
                     raise ValueError(f"There must only be one telescope of type '{kw.TELESCOPE_TYPE_MAIN}'.")
                 tel = aotpy.MainTelescope(uid)
                 self._system.main_telescope = tel
                 self._telescopes[uid] = [tel, True]  # The main telescope is always referenced by the AOSystem
             elif t == kw.TELESCOPE_TYPE_LLT:
                 tel = aotpy.LaserLaunchTelescope(uid)
                 self._telescopes[uid] = [tel, False]
             else:
                 warnings.warn(f"Skipped telescope {uid}: unknown type '{t}'.")
                 continue
 
-            tel.latitude = data[kw.TELESCOPE_LATITUDE]
-            tel.longitude = data[kw.TELESCOPE_LONGITUDE]
-            tel.elevation = data[kw.TELESCOPE_ELEVATION]
-            tel.azimuth = data[kw.TELESCOPE_AZIMUTH]
-            tel.parallactic = data[kw.TELESCOPE_PARALLACTIC]
-            tel.pupil_mask = self._handle_image(data[kw.TELESCOPE_PUPIL_MASK])
-            tel.pupil_angle = data[kw.TELESCOPE_PUPIL_ANGLE]
-            tel.enclosing_diameter = data[kw.TELESCOPE_ENCLOSING_D]
-            tel.inscribed_diameter = data[kw.TELESCOPE_INSCRIBED_D]
-            tel.obstruction_diameter = data[kw.TELESCOPE_OBSTRUCTION_D]
+            tel.latitude = row[kw.TELESCOPE_LATITUDE]
+            tel.longitude = row[kw.TELESCOPE_LONGITUDE]
+            tel.elevation = row[kw.TELESCOPE_ELEVATION]
+            tel.azimuth = row[kw.TELESCOPE_AZIMUTH]
+            tel.parallactic = row[kw.TELESCOPE_PARALLACTIC]
+            tel.pupil_mask = self._handle_image(row[kw.TELESCOPE_PUPIL_MASK])
+            tel.pupil_angle = row[kw.TELESCOPE_PUPIL_ANGLE]
+            tel.enclosing_diameter = row[kw.TELESCOPE_ENCLOSING_D]
+            tel.inscribed_diameter = row[kw.TELESCOPE_INSCRIBED_D]
+            tel.obstruction_diameter = row[kw.TELESCOPE_OBSTRUCTION_D]
 
-            t = data[kw.TELESCOPE_SEGMENTS_TYPE]
+            t = row[kw.TELESCOPE_SEGMENTS_TYPE]
             if t == kw.TELESCOPE_SEGMENT_TYPE_MONOLITHIC:
                 seg = aotpy.Monolithic()
             else:
                 if t == kw.TELESCOPE_SEGMENT_TYPE_CIRCLE:
                     seg = aotpy.CircularSegments()
                 elif t == kw.TELESCOPE_SEGMENT_TYPE_HEXAGON:
                     seg = aotpy.HexagonalSegments()
                 else:
                     warnings.warn(f"Ignored unknown segment type '{t}'.")
                     seg = aotpy.Monolithic()
-                seg.size = data[kw.TELESCOPE_SEGMENTS_SIZE]
+                seg.size = row[kw.TELESCOPE_SEGMENTS_SIZE]
                 seg.coordinates = [aotpy.Coordinates(x, y)
-                                   for x, y in zip(data[kw.TELESCOPE_SEGMENTS_X], data[kw.TELESCOPE_SEGMENTS_Y])]
+                                   for x, y in zip(row[kw.TELESCOPE_SEGMENTS_X], row[kw.TELESCOPE_SEGMENTS_Y])]
 
             tel.segments = seg
-            tel.transformation_matrix = self._handle_image(data[kw.TRANSFORMATION_MATRIX])
-            tel.aberration = self._handle_reference(data[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE)
+            tel.transformation_matrix = self._handle_image(row[kw.TRANSFORMATION_MATRIX])
+            tel.aberration = self._handle_reference(row[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE)
 
     def _handle_sources(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.SOURCES_TABLE)
-
         table = hdus[kw.SOURCES_TABLE]
+        source_rows = self._check_and_convert_rows(table)
+
         existing_types = table.data['TYPE']
         if kw.SOURCE_TYPE_SODIUM_LASER_GUIDE_STAR in existing_types:
             if kw.SOURCES_SODIUM_LGS_TABLE in hdus:
-                self._check_bintable(hdus, kw.SOURCES_SODIUM_LGS_TABLE)
+                sodium_rows = self._check_and_convert_rows(hdus[kw.SOURCES_SODIUM_LGS_TABLE])
             else:
                 raise ValueError(f"Missing table '{kw.SOURCES_SODIUM_LGS_TABLE}' must exist when "
                                  f"'{kw.SOURCE_TYPE_SODIUM_LASER_GUIDE_STAR}' type sources exist")
         if kw.SOURCE_TYPE_RAYLEIGH_LASER_GUIDE_STAR in existing_types:
             if kw.SOURCES_RAYLEIGH_LGS_TABLE in hdus:
-                self._check_bintable(hdus, kw.SOURCES_RAYLEIGH_LGS_TABLE)
+                rayleigh_rows = self._check_and_convert_rows(hdus[kw.SOURCES_RAYLEIGH_LGS_TABLE])
             else:
                 raise ValueError(f"Missing table '{kw.SOURCES_SODIUM_LGS_TABLE}' must exist when "
                                  f"'{kw.SOURCE_TYPE_RAYLEIGH_LASER_GUIDE_STAR}' type sources exist")
 
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.SOURCE_FIELDS)
-
-            uid = data[kw.REFERENCE_UID]
-            t = data[kw.SOURCE_TYPE]
+        for row in source_rows:
+            uid = row[kw.REFERENCE_UID]
+            t = row[kw.SOURCE_TYPE]
             if t == kw.SOURCE_TYPE_SCIENCE_STAR:
                 src = aotpy.ScienceStar(uid)
             elif t == kw.SOURCE_TYPE_NATURAL_GUIDE_STAR:
                 src = aotpy.NaturalGuideStar(uid)
             elif t == kw.SOURCE_TYPE_SODIUM_LASER_GUIDE_STAR:
                 # Try to find uid in secondary table
-                f = next((x for x in hdus[kw.SOURCES_SODIUM_LGS_TABLE].data if x[kw.REFERENCE_UID] == uid), None)
-                if f is None:
+                other_data = next((x for x in sodium_rows if x[kw.REFERENCE_UID] == uid), None)
+                if other_data is None:
                     raise ValueError(f"Source '{uid}' not found in table '{kw.SOURCES_SODIUM_LGS_TABLE}' even"
                                      f" though it is of type '{t}'")
 
-                other_data = _convert_row(hdus[kw.SOURCES_SODIUM_LGS_TABLE].columns, f, kw.SOURCE_SODIUM_LGS_FIELDS)
                 src = aotpy.SodiumLaserGuideStar(
                     uid=uid,
                     height=other_data[kw.SOURCE_SODIUM_LGS_HEIGHT],
                     profile=self._handle_image(other_data[kw.SOURCE_SODIUM_LGS_PROFILE]),
                     altitudes=other_data[kw.SOURCE_SODIUM_LGS_ALTITUDES],
                     laser_launch_telescope=self._handle_reference(other_data[kw.LASER_LAUNCH_TELESCOPE_REFERENCE],
                                                                   kw.TELESCOPES_TABLE)
                 )
             elif t == kw.SOURCE_TYPE_RAYLEIGH_LASER_GUIDE_STAR:
                 # Try to find uid in secondary table
-                f = next((x for x in hdus[kw.SOURCES_RAYLEIGH_LGS_TABLE].data if x[kw.REFERENCE_UID] == uid), None)
-                if f is None:
+                other_data = next((x for x in rayleigh_rows if x[kw.REFERENCE_UID] == uid), None)
+                if other_data is None:
                     raise ValueError(f"Source '{uid}' not found in table '{kw.SOURCES_RAYLEIGH_LGS_TABLE}' even"
                                      f" though it is of type '{t}'")
 
-                other_data = _convert_row(hdus[kw.SOURCES_RAYLEIGH_LGS_TABLE].columns, f, kw.SOURCE_RAYLEIGH_LGS_FIELDS)
                 src = aotpy.RayleighLaserGuideStar(
                     uid=uid,
                     distance=other_data[kw.SOURCE_RAYLEIGH_LGS_DISTANCE],
                     depth=other_data[kw.SOURCE_RAYLEIGH_LGS_DEPTH],
                     laser_launch_telescope=self._handle_reference(other_data[kw.LASER_LAUNCH_TELESCOPE_REFERENCE],
                                                                   kw.TELESCOPES_TABLE)
                 )
             else:
                 warnings.warn(f"Skipped source '{uid}': unknown type '{t}'.")
                 continue
 
-            src.right_ascension = data[kw.SOURCE_RIGHT_ASCENSION]
-            src.declination = data[kw.SOURCE_DECLINATION]
-            src.elevation_offset = data[kw.SOURCE_ELEVATION_OFFSET]
-            src.azimuth_offset = data[kw.SOURCE_AZIMUTH_OFFSET]
-            src.width = data[kw.SOURCE_WIDTH]
+            src.right_ascension = row[kw.SOURCE_RIGHT_ASCENSION]
+            src.declination = row[kw.SOURCE_DECLINATION]
+            src.elevation_offset = row[kw.SOURCE_ELEVATION_OFFSET]
+            src.azimuth_offset = row[kw.SOURCE_AZIMUTH_OFFSET]
+            src.width = row[kw.SOURCE_WIDTH]
 
             self._sources[uid] = [src, True]  # sources are always referenced by AOSystem
             self._system.sources.append(src)
 
     def _handle_detectors(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.DETECTORS_TABLE)
-
-        table = hdus[kw.DETECTORS_TABLE]
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.DETECTOR_FIELDS)
-
-            self._detectors[data[kw.REFERENCE_UID]] = [aotpy.Detector(
-                uid=data[kw.REFERENCE_UID],
-                type=data[kw.DETECTOR_TYPE],
-                sampling_technique=data[kw.DETECTOR_SAMPLING_TECHNIQUE],
-                shutter_type=data[kw.DETECTOR_SHUTTER_TYPE],
-                flat_field=self._handle_image(data[kw.DETECTOR_FLAT_FIELD]),
-                readout_noise=data[kw.DETECTOR_READOUT_NOISE],
-                pixel_intensities=self._handle_image(data[kw.DETECTOR_PIXEL_INTENSITIES]),
-                integration_time=data[kw.DETECTOR_INTEGRATION_TIME],
-                coadds=data[kw.DETECTOR_COADDS],
-                dark=self._handle_image(data[kw.DETECTOR_DARK]),
-                weight_map=self._handle_image(data[kw.DETECTOR_WEIGHT_MAP]),
-                quantum_efficiency=data[kw.DETECTOR_QUANTUM_EFFICIENCY],
-                pixel_scale=data[kw.DETECTOR_PIXEL_SCALE],
-                binning=data[kw.DETECTOR_BINNING],
-                bandwidth=data[kw.DETECTOR_BANDWIDTH],
-                transmission_wavelength=data[kw.DETECTOR_TRANSMISSION_WAVELENGTH],
-                transmission=data[kw.DETECTOR_TRANSMISSION],
-                sky_background=self._handle_image(data[kw.DETECTOR_SKY_BACKGROUND]),
-                gain=data[kw.DETECTOR_GAIN],
-                excess_noise=data[kw.DETECTOR_EXCESS_NOISE],
-                filter=data[kw.DETECTOR_FILTER],
-                bad_pixel_map=self._handle_image(data[kw.DETECTOR_BAD_PIXEL_MAP]),
-                dynamic_range=data[kw.DETECTOR_DYNAMIC_RANGE],
-                readout_rate=data[kw.DETECTOR_READOUT_RATE],
-                frame_rate=data[kw.DETECTOR_FRAME_RATE],
-                transformation_matrix=self._handle_image(data[kw.TRANSFORMATION_MATRIX])
+        for row in self._check_and_convert_rows(hdus[kw.DETECTORS_TABLE]):
+            self._detectors[row[kw.REFERENCE_UID]] = [aotpy.Detector(
+                uid=row[kw.REFERENCE_UID],
+                type=row[kw.DETECTOR_TYPE],
+                sampling_technique=row[kw.DETECTOR_SAMPLING_TECHNIQUE],
+                shutter_type=row[kw.DETECTOR_SHUTTER_TYPE],
+                flat_field=self._handle_image(row[kw.DETECTOR_FLAT_FIELD]),
+                readout_noise=row[kw.DETECTOR_READOUT_NOISE],
+                pixel_intensities=self._handle_image(row[kw.DETECTOR_PIXEL_INTENSITIES]),
+                integration_time=row[kw.DETECTOR_INTEGRATION_TIME],
+                coadds=row[kw.DETECTOR_COADDS],
+                dark=self._handle_image(row[kw.DETECTOR_DARK]),
+                weight_map=self._handle_image(row[kw.DETECTOR_WEIGHT_MAP]),
+                quantum_efficiency=row[kw.DETECTOR_QUANTUM_EFFICIENCY],
+                pixel_scale=row[kw.DETECTOR_PIXEL_SCALE],
+                binning=row[kw.DETECTOR_BINNING],
+                bandwidth=row[kw.DETECTOR_BANDWIDTH],
+                transmission_wavelength=row[kw.DETECTOR_TRANSMISSION_WAVELENGTH],
+                transmission=row[kw.DETECTOR_TRANSMISSION],
+                sky_background=self._handle_image(row[kw.DETECTOR_SKY_BACKGROUND]),
+                gain=row[kw.DETECTOR_GAIN],
+                excess_noise=row[kw.DETECTOR_EXCESS_NOISE],
+                filter=row[kw.DETECTOR_FILTER],
+                bad_pixel_map=self._handle_image(row[kw.DETECTOR_BAD_PIXEL_MAP]),
+                dynamic_range=row[kw.DETECTOR_DYNAMIC_RANGE],
+                readout_rate=row[kw.DETECTOR_READOUT_RATE],
+                frame_rate=row[kw.DETECTOR_FRAME_RATE],
+                transformation_matrix=self._handle_image(row[kw.TRANSFORMATION_MATRIX])
             ), False]
 
     def _handle_scoring_cameras(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.SCORING_CAMERAS_TABLE)
-
-        table = hdus[kw.SCORING_CAMERAS_TABLE]
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.SCORING_CAMERA_FIELDS)
-
+        for row in self._check_and_convert_rows(hdus[kw.SCORING_CAMERAS_TABLE]):
             self._system.scoring_cameras.append(aotpy.ScoringCamera(
-                uid=data[kw.REFERENCE_UID],
-                pupil_mask=self._handle_image(data[kw.SCORING_CAMERA_PUPIL_MASK]),
-                wavelength=data[kw.SCORING_CAMERA_WAVELENGTH],
-                transformation_matrix=self._handle_image(data[kw.TRANSFORMATION_MATRIX]),
-                detector=self._handle_reference(data[kw.DETECTOR_REFERENCE], kw.DETECTORS_TABLE),
-                aberration=self._handle_reference(data[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE),
+                uid=row[kw.REFERENCE_UID],
+                pupil_mask=self._handle_image(row[kw.SCORING_CAMERA_PUPIL_MASK]),
+                wavelength=row[kw.SCORING_CAMERA_WAVELENGTH],
+                transformation_matrix=self._handle_image(row[kw.TRANSFORMATION_MATRIX]),
+                detector=self._handle_reference(row[kw.DETECTOR_REFERENCE], kw.DETECTORS_TABLE),
+                aberration=self._handle_reference(row[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE),
             ))
 
     def _handle_wavefront_sensors(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.WAVEFRONT_SENSORS_TABLE)
-
         table = hdus[kw.WAVEFRONT_SENSORS_TABLE]
+        wfs_rows = self._check_and_convert_rows(table)
+
         existing_types = table.data['TYPE']
         if kw.WAVEFRONT_SENSOR_TYPE_SHACK_HARTMANN in existing_types:
             if kw.WAVEFRONT_SENSORS_SHACK_HARTMANN_TABLE in hdus:
-                self._check_bintable(hdus, kw.WAVEFRONT_SENSORS_SHACK_HARTMANN_TABLE)
+                sh_rows = self._check_and_convert_rows(hdus[kw.WAVEFRONT_SENSORS_SHACK_HARTMANN_TABLE])
             else:
                 raise ValueError(f"Missing table '{kw.WAVEFRONT_SENSORS_SHACK_HARTMANN_TABLE}' must exist when "
                                  f"'{kw.WAVEFRONT_SENSOR_TYPE_SHACK_HARTMANN}' type wavefront sensors exist")
         if kw.WAVEFRONT_SENSOR_TYPE_PYRAMID in existing_types:
             if kw.WAVEFRONT_SENSORS_PYRAMID_TABLE in hdus:
-                self._check_bintable(hdus, kw.WAVEFRONT_SENSORS_PYRAMID_TABLE)
+                pyr_rows = self._check_and_convert_rows(hdus[kw.WAVEFRONT_SENSORS_PYRAMID_TABLE])
             else:
                 raise ValueError(f"Missing table '{kw.WAVEFRONT_SENSORS_PYRAMID_TABLE}' must exist when "
                                  f"'{kw.WAVEFRONT_SENSOR_TYPE_PYRAMID}' type wavefront sensors exist")
 
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.WAVEFRONT_SENSOR_FIELDS)
-
-            uid = data[kw.REFERENCE_UID]
-            t = data[kw.WAVEFRONT_SENSOR_TYPE]
-            source = self._handle_reference(data[kw.SOURCE_REFERENCE], kw.SOURCES_TABLE)
-            dimensions = data[kw.WAVEFRONT_SENSOR_DIMENSIONS]
-            n_valid_subapertures = data[kw.WAVEFRONT_SENSOR_N_VALID_SUBAPERTURES]
+        for row in wfs_rows:
+            uid = row[kw.REFERENCE_UID]
+            t = row[kw.WAVEFRONT_SENSOR_TYPE]
+            source = self._handle_reference(row[kw.SOURCE_REFERENCE], kw.SOURCES_TABLE)
+            dimensions = row[kw.WAVEFRONT_SENSOR_DIMENSIONS]
+            n_valid_subapertures = row[kw.WAVEFRONT_SENSOR_N_VALID_SUBAPERTURES]
             if t == kw.WAVEFRONT_SENSOR_TYPE_SHACK_HARTMANN:
                 # Try to find uid in secondary table
-                f = next(
-                    (x for x in hdus[kw.WAVEFRONT_SENSORS_SHACK_HARTMANN_TABLE].data if x[kw.REFERENCE_UID] == uid),
-                    None)
-                if f is None:
+                other_data = next((x for x in sh_rows if x[kw.REFERENCE_UID] == uid), None)
+                if other_data is None:
                     raise ValueError(f"Wavefront sensor '{uid}' not found in table "
                                      f"'{kw.WAVEFRONT_SENSORS_SHACK_HARTMANN_TABLE}' even though it is of type '{t}'")
-
-                other_data = _convert_row(hdus[kw.WAVEFRONT_SENSORS_SHACK_HARTMANN_TABLE].columns, f,
-                                          kw.WAVEFRONT_SENSOR_SHACK_HARTMANN_FIELDS)
                 if dimensions != 2:
                     warnings.warn(f"Unexpected value for '{kw.WAVEFRONT_SENSOR_DIMENSIONS}' in wavefront sensor '{uid}'"
                                   f" of type '{t}'. Expected 2, got {dimensions}.")
                 wfs = aotpy.ShackHartmann(
                     uid=uid,
                     source=source,
                     n_valid_subapertures=n_valid_subapertures,
                     centroiding_algorithm=other_data[kw.WAVEFRONT_SENSOR_SHACK_HARTMANN_CENTROIDING_ALGORITHM],
                     centroid_gains=self._handle_image(other_data[kw.WAVEFRONT_SENSOR_SHACK_HARTMANN_CENTROID_GAINS]),
                     spot_fwhm=self._handle_image(other_data[kw.WAVEFRONT_SENSOR_SHACK_HARTMANN_SPOT_FWHM])
                 )
             elif t == kw.WAVEFRONT_SENSOR_TYPE_PYRAMID:
                 # Try to find uid in secondary table
-                f = next((x for x in hdus[kw.WAVEFRONT_SENSORS_PYRAMID_TABLE].data if x[kw.REFERENCE_UID] == uid), None)
-                if f is None:
+                other_data = next((x for x in pyr_rows if x[kw.REFERENCE_UID] == uid), None)
+                if other_data is None:
                     raise ValueError(f"Wavefront sensor '{uid}' not found in table "
                                      f"'{kw.WAVEFRONT_SENSORS_PYRAMID_TABLE}' even though it is of type '{t}'")
 
-                other_data = _convert_row(hdus[kw.WAVEFRONT_SENSORS_PYRAMID_TABLE].columns, f,
-                                          kw.WAVEFRONT_SENSOR_PYRAMID_FIELDS)
                 wfs = aotpy.Pyramid(
                     uid=uid,
                     source=source,
                     dimensions=dimensions,
                     n_valid_subapertures=n_valid_subapertures,
                     n_sides=other_data[kw.WAVEFRONT_SENSOR_PYRAMID_N_SIDES],
                     modulation=other_data[kw.WAVEFRONT_SENSOR_PYRAMID_MODULATION]
                 )
             else:
                 warnings.warn(f"Skipped wavefront sensor '{uid}': unknown type '{t}'.")
                 continue
 
-            wfs.measurements = self._handle_image(data[kw.WAVEFRONT_SENSOR_MEASUREMENTS])
-            wfs.ref_measurements = self._handle_image(data[kw.WAVEFRONT_SENSOR_REF_MEASUREMENTS])
-            wfs.subaperture_mask = self._handle_image(data[kw.WAVEFRONT_SENSOR_SUBAPERTURE_MASK])
-            wfs.mask_offsets = [aotpy.Coordinates(x, y) for x, y in zip(data[kw.WAVEFRONT_SENSOR_MASK_X_OFFSETS],
-                                                                        data[kw.WAVEFRONT_SENSOR_MASK_Y_OFFSETS])]
-            wfs.subaperture_size = data[kw.WAVEFRONT_SENSOR_SUBAPERTURE_SIZE]
-            wfs.subaperture_intensities = self._handle_image(data[kw.WAVEFRONT_SENSOR_SUBAPERTURE_INTENSITIES])
-            wfs.wavelength = data[kw.WAVEFRONT_SENSOR_WAVELENGTH]
-            wfs.optical_gain = self._handle_image(data[kw.WAVEFRONT_SENSOR_OPTICAL_GAIN])
-            wfs.transformation_matrix = self._handle_image(data[kw.TRANSFORMATION_MATRIX])
-            wfs.detector = self._handle_reference(data[kw.DETECTOR_REFERENCE], kw.DETECTORS_TABLE)
-            wfs.aberration = self._handle_reference(data[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE)
-            wfs.non_common_path_aberration = self._handle_reference(data[kw.NCPA_REFERENCE], kw.ABERRATIONS_TABLE)
+            wfs.measurements = self._handle_image(row[kw.WAVEFRONT_SENSOR_MEASUREMENTS])
+            wfs.ref_measurements = self._handle_image(row[kw.WAVEFRONT_SENSOR_REF_MEASUREMENTS])
+            wfs.subaperture_mask = self._handle_image(row[kw.WAVEFRONT_SENSOR_SUBAPERTURE_MASK])
+            wfs.mask_offsets = [aotpy.Coordinates(x, y) for x, y in zip(row[kw.WAVEFRONT_SENSOR_MASK_X_OFFSETS],
+                                                                        row[kw.WAVEFRONT_SENSOR_MASK_Y_OFFSETS])]
+            wfs.subaperture_size = row[kw.WAVEFRONT_SENSOR_SUBAPERTURE_SIZE]
+            wfs.subaperture_intensities = self._handle_image(row[kw.WAVEFRONT_SENSOR_SUBAPERTURE_INTENSITIES])
+            wfs.wavelength = row[kw.WAVEFRONT_SENSOR_WAVELENGTH]
+            wfs.optical_gain = self._handle_image(row[kw.WAVEFRONT_SENSOR_OPTICAL_GAIN])
+            wfs.transformation_matrix = self._handle_image(row[kw.TRANSFORMATION_MATRIX])
+            wfs.detector = self._handle_reference(row[kw.DETECTOR_REFERENCE], kw.DETECTORS_TABLE)
+            wfs.aberration = self._handle_reference(row[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE)
+            wfs.non_common_path_aberration = self._handle_reference(row[kw.NCPA_REFERENCE], kw.ABERRATIONS_TABLE)
 
             self._wfss[uid] = [wfs, True]  # wavefront sensors are always referenced by AOSystem
             self._system.wavefront_sensors.append(wfs)
 
     def _handle_wavefront_correctors(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.WAVEFRONT_CORRECTORS_TABLE)
-
         table = hdus[kw.WAVEFRONT_CORRECTORS_TABLE]
+        rows = self._check_and_convert_rows(table)
+
         existing_types = table.data['TYPE']
         if kw.WAVEFRONT_CORRECTOR_TYPE_DM in existing_types:
             if kw.WAVEFRONT_CORRECTORS_DM_TABLE in hdus:
-                self._check_bintable(hdus, kw.WAVEFRONT_CORRECTORS_DM_TABLE)
+                dm_rows = self._check_and_convert_rows(hdus[kw.WAVEFRONT_CORRECTORS_DM_TABLE])
             else:
                 raise ValueError(f"Missing table '{kw.WAVEFRONT_CORRECTORS_DM_TABLE}' must exist when "
                                  f"'{kw.WAVEFRONT_CORRECTOR_TYPE_DM}' type wavefront correctors exist")
 
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.WAVEFRONT_CORRECTOR_FIELDS)
-
-            uid = data[kw.REFERENCE_UID]
-            t = data[kw.WAVEFRONT_CORRECTOR_TYPE]
-            telescope = self._handle_reference(data[kw.TELESCOPE_REFERENCE], kw.TELESCOPES_TABLE)
+        for row in rows:
+            uid = row[kw.REFERENCE_UID]
+            t = row[kw.WAVEFRONT_CORRECTOR_TYPE]
+            telescope = self._handle_reference(row[kw.TELESCOPE_REFERENCE], kw.TELESCOPES_TABLE)
 
             if t == kw.WAVEFRONT_CORRECTOR_TYPE_DM:
                 # Try to find uid in secondary table
-                f = next((x for x in hdus[kw.WAVEFRONT_CORRECTORS_DM_TABLE].data if x[kw.REFERENCE_UID] == uid), None)
-                if f is None:
+                other_data = next((x for x in dm_rows if x[kw.REFERENCE_UID] == uid), None)
+                if other_data is None:
                     raise ValueError(f"Wavefront corrector '{uid}' not found in table "
                                      f"'{kw.WAVEFRONT_CORRECTORS_DM_TABLE}' even though it is of type '{t}'")
 
-                other_data = _convert_row(hdus[kw.WAVEFRONT_CORRECTORS_DM_TABLE].columns, f,
-                                          kw.WAVEFRONT_CORRECTOR_DM_FIELDS)
                 cor = aotpy.DeformableMirror(
                     uid=uid,
                     telescope=telescope,
-                    n_valid_actuators=data[kw.WAVEFRONT_CORRECTOR_N_VALID_ACTUATORS],
+                    n_valid_actuators=row[kw.WAVEFRONT_CORRECTOR_N_VALID_ACTUATORS],
                     actuator_coordinates=[aotpy.Coordinates(x, y) for x, y in
                                           zip(other_data[kw.WAVEFRONT_CORRECTOR_DM_ACTUATORS_X],
                                               other_data[kw.WAVEFRONT_CORRECTOR_DM_ACTUATORS_Y])],
                     influence_function=self._handle_image(other_data[kw.WAVEFRONT_CORRECTOR_DM_INFLUENCE_FUNCTION]),
                     stroke=other_data[kw.WAVEFRONT_CORRECTOR_DM_STROKE]
                 )
             elif t == kw.WAVEFRONT_CORRECTOR_TYPE_TTM:
@@ -719,57 +669,53 @@
                     uid=uid,
                     telescope=telescope
                 )
             else:
                 warnings.warn(f"Skipped wavefront corrector '{uid}': unknown type '{t}'.")
                 continue
 
-            cor.pupil_mask = self._handle_image(data[kw.WAVEFRONT_CORRECTOR_PUPIL_MASK])
-            cor.tfz_num = data[kw.WAVEFRONT_CORRECTOR_TFZ_NUM]
-            cor.tfz_den = data[kw.WAVEFRONT_CORRECTOR_TFZ_DEN]
-            cor.transformation_matrix = self._handle_image(data[kw.TRANSFORMATION_MATRIX])
-            cor.aberration = self._handle_reference(data[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE)
+            cor.pupil_mask = self._handle_image(row[kw.WAVEFRONT_CORRECTOR_PUPIL_MASK])
+            cor.tfz_num = row[kw.WAVEFRONT_CORRECTOR_TFZ_NUM]
+            cor.tfz_den = row[kw.WAVEFRONT_CORRECTOR_TFZ_DEN]
+            cor.transformation_matrix = self._handle_image(row[kw.TRANSFORMATION_MATRIX])
+            cor.aberration = self._handle_reference(row[kw.ABERRATION_REFERENCE], kw.ABERRATIONS_TABLE)
 
             self._wfcs[uid] = [cor, True]  # wavefront corectors are always referenced by AOSystem
             self._system.wavefront_correctors.append(cor)
 
     def _handle_loops(self, hdus: fits.HDUList):
-        self._check_bintable(hdus, kw.LOOPS_TABLE)
-
         table = hdus[kw.LOOPS_TABLE]
+        rows = self._check_and_convert_rows(table)
+
         existing_types = table.data['TYPE']
         if kw.LOOPS_TYPE_CONTROL in existing_types:
             if kw.LOOPS_CONTROL_TABLE in hdus:
-                self._check_bintable(hdus, kw.LOOPS_CONTROL_TABLE)
+                control_rows = self._check_and_convert_rows(hdus[kw.LOOPS_CONTROL_TABLE])
             else:
                 raise ValueError(f"Missing table '{kw.LOOPS_CONTROL_TABLE}' must exist when "
                                  f"'{kw.LOOPS_TYPE_CONTROL}' type loops exist")
         if kw.LOOPS_TYPE_OFFLOAD in existing_types:
             if kw.LOOPS_OFFLOAD_TABLE in hdus:
-                self._check_bintable(hdus, kw.LOOPS_OFFLOAD_TABLE)
+                offload_rows = self._check_and_convert_rows(hdus[kw.LOOPS_OFFLOAD_TABLE])
             else:
                 raise ValueError(f"Missing table '{kw.LOOPS_OFFLOAD_TABLE}' must exist when "
                                  f"'{kw.LOOPS_TYPE_OFFLOAD}' type loops exist")
 
-        columns = table.columns
-        for row in table.data:
-            data = _convert_row(columns, row, kw.LOOPS_FIELDS)
-
-            uid = data[kw.REFERENCE_UID]
-            t = data[kw.WAVEFRONT_SENSOR_TYPE]
-            commanded = self._handle_reference(data[kw.LOOPS_COMMANDED], kw.WAVEFRONT_CORRECTORS_TABLE)
+        for row in rows:
+            uid = row[kw.REFERENCE_UID]
+            t = row[kw.WAVEFRONT_SENSOR_TYPE]
+            commanded = self._handle_reference(row[kw.LOOPS_COMMANDED], kw.WAVEFRONT_CORRECTORS_TABLE)
 
             if t == kw.LOOPS_TYPE_CONTROL:
                 # Try to find uid in secondary table
-                f = next((x for x in hdus[kw.LOOPS_CONTROL_TABLE].data if x[kw.REFERENCE_UID] == uid), None)
-                if f is None:
+                other_data = next((x for x in control_rows if x[kw.REFERENCE_UID] == uid), None)
+                if other_data is None:
                     raise ValueError(f"Loop '{uid}' not found in table "
                                      f"'{kw.LOOPS_CONTROL_TABLE}' even though it is of type '{t}'")
 
-                other_data = _convert_row(hdus[kw.LOOPS_CONTROL_TABLE].columns, f, kw.LOOPS_CONTROL_FIELDS)
                 loop = aotpy.ControlLoop(
                     uid=uid,
                     commanded_corrector=commanded,
                     input_sensor=self._handle_reference(other_data[kw.LOOPS_CONTROL_INPUT_SENSOR],
                                                         kw.WAVEFRONT_SENSORS_TABLE),
                     modes=self._handle_image(other_data[kw.LOOPS_CONTROL_MODES]),
                     modal_coefficients=self._handle_image(other_data[kw.LOOPS_CONTROL_MODAL_COEFFICIENTS]),
@@ -779,42 +725,41 @@
                     interaction_matrix=self._handle_image(other_data[kw.LOOPS_CONTROL_INTERACTION_MATRIX]),
                     commands_to_modes=self._handle_image(other_data[kw.LOOPS_CONTROL_COMMANDS_TO_MODES]),
                     modes_to_measurements=self._handle_image(other_data[kw.LOOPS_CONTROL_MODES_TO_MEASUREMENTS]),
                     residual_commands=self._handle_image(other_data[kw.LOOPS_CONTROL_RESIDUAL_COMMANDS])
                 )
             elif t == kw.LOOPS_TYPE_OFFLOAD:
                 # Try to find uid in secondary table
-                f = next((x for x in hdus[kw.LOOPS_OFFLOAD_TABLE].data if x[kw.REFERENCE_UID] == uid), None)
-                if f is None:
+                other_data = next((x for x in offload_rows if x[kw.REFERENCE_UID] == uid), None)
+                if other_data is None:
                     raise ValueError(f"Loop '{uid}' not found in table "
                                      f"'{kw.LOOPS_OFFLOAD_TABLE}' even though it is of type '{t}'")
 
-                other_data = _convert_row(hdus[kw.LOOPS_OFFLOAD_TABLE].columns, f, kw.LOOPS_OFFLOAD_FIELDS)
                 loop = aotpy.OffloadLoop(
                     uid=uid,
                     commanded_corrector=commanded,
                     input_corrector=self._handle_reference(other_data[kw.LOOPS_OFFLOAD_INPUT_CORRECTOR],
                                                            kw.WAVEFRONT_CORRECTORS_TABLE),
                     offload_matrix=self._handle_image(other_data[kw.LOOPS_OFFLOAD_OFFLOAD_MATRIX])
                 )
             else:
                 warnings.warn(f"Skipped loop '{uid}': unknown type '{t}'.")
                 continue
 
-            loop.time = self._handle_reference(data[kw.TIME_REFERENCE], kw.TIME_TABLE)
-            if (status := data[kw.LOOPS_STATUS]) is None:
+            loop.time = self._handle_reference(row[kw.TIME_REFERENCE], kw.TIME_TABLE)
+            if (status := row[kw.LOOPS_STATUS]) is None:
                 loop.closed = None
             elif status == kw.LOOPS_STATUS_CLOSED:
                 loop.closed = True
             elif status == kw.LOOPS_STATUS_OPEN:
                 loop.closed = False
             else:
                 warnings.warn(f"Ignored unknown loop status '{status}'.")
                 loop.closed = None
-            loop.commands = self._handle_image(data[kw.LOOPS_COMMANDS])
-            loop.ref_commands = self._handle_image(data[kw.LOOPS_REF_COMMANDS])
-            loop.framerate = data[kw.LOOPS_FRAMERATE]
-            loop.delay = data[kw.LOOPS_DELAY]
-            loop.time_filter_num = self._handle_image(data[kw.LOOPS_TIME_FILTER_NUM])
-            loop.time_filter_den = self._handle_image(data[kw.LOOPS_TIME_FILTER_DEN])
+            loop.commands = self._handle_image(row[kw.LOOPS_COMMANDS])
+            loop.ref_commands = self._handle_image(row[kw.LOOPS_REF_COMMANDS])
+            loop.framerate = row[kw.LOOPS_FRAMERATE]
+            loop.delay = row[kw.LOOPS_DELAY]
+            loop.time_filter_num = self._handle_image(row[kw.LOOPS_TIME_FILTER_NUM])
+            loop.time_filter_den = self._handle_image(row[kw.LOOPS_TIME_FILTER_DEN])
 
             self._system.loops.append(loop)
```

### Comparing `aotpy-0.8.1/aotpy/io/fits/utils.py` & `aotpy-0.8.2/aotpy/io/fits/utils.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/io/fits/writer.py` & `aotpy-0.8.2/aotpy/io/fits/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,17 +152,16 @@
     @staticmethod
     def _create_row_reference(uid: str) -> str:
         return f'{kw.ROW_REFERENCE}<{uid}>'
 
     def _handle_time(self, time: aotpy.Time) -> str | None:
         if time is None:
             return None
-        if time.timestamps is not None and time.frame_numbers is not None \
-                and len(time.timestamps) != len(time.frame_numbers):
-            raise ValueError(f"Error in Time '{time.uid}': If both 'timestamps' and 'frame_numbers' are non-null, they"
+        if time.timestamps and time.frame_numbers and len(time.timestamps) != len(time.frame_numbers):
+            raise ValueError(f"Error in Time '{time.uid}': If both 'timestamps' and 'frame_numbers' are non-null, they "
                              f"must have the same length.")
         row = {
             kw.REFERENCE_UID: time.uid,
             kw.TIME_TIMESTAMPS: time.timestamps,
             kw.TIME_FRAME_NUMBERS: time.frame_numbers
         }
         self._add_to_table(kw.TIME_TABLE, time, row)
@@ -514,17 +513,15 @@
             kw.LOOPS_DELAY: loop.delay,
             kw.LOOPS_TIME_FILTER_NUM: self._handle_image(loop.time_filter_num),
             kw.LOOPS_TIME_FILTER_DEN: self._handle_image(loop.time_filter_den)
         }
         self._add_to_table(kw.LOOPS_TABLE, loop, row)
 
     def _create_primary_hdu(self) -> fits.PrimaryHDU:
-        hdr = fits.Header([(f'HIERARCH {md.key}' if len(md.key) > 8 else md.key,
-                            md.value,
-                            md.comment) for md in self._system.metadata])
+        hdr = fits.Header()
         hdr[kw.AOT_VERSION] = kw.CURRENT_AOT_VERSION
         hdr[kw.AOT_TIMESYS] = kw.AOT_TIMESYS_UTC
 
         if self._system.ao_mode not in kw.AOT_AO_MODE_SET:
             raise ValueError(f"'AOSystem.ao_mode' must be one of: {str(kw.AOT_AO_MODE_SET)[1:-1]}")
         hdr[kw.AOT_AO_MODE] = self._system.ao_mode
 
@@ -536,14 +533,17 @@
         if self._system.strehl_ratio is not None:
             hdr[kw.AOT_STREHL_RATIO] = self._system.strehl_ratio
         if self._system.temporal_error is not None:
             hdr[kw.AOT_TEMPORAL_ERROR] = self._system.temporal_error
         if self._system.config is not None:
             hdr[kw.AOT_CONFIG] = self._system.config
 
+        hdr.extend([(f'HIERARCH {md.key}' if len(md.key) > 8 else md.key,
+                            md.value,
+                            md.comment) for md in self._system.metadata])
         return fits.PrimaryHDU(header=hdr)
 
     def _create_bintable_hdus(self) -> list[fits.BinTableHDU]:
         hdus = []
         for table_name in kw.TABLE_SEQUENCE:
             try:
                 table = self._tables[table_name]
```

### Comparing `aotpy-0.8.1/aotpy/translators/base.py` & `aotpy-0.8.2/aotpy/translators/base.py`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/aotpy/translators/ciao.py` & `aotpy-0.8.2/aotpy/translators/ciao.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,7 +158,10 @@
         return f"ESO-VLTI-%A%{self._at_number}%"
 
     def _get_eso_ao_name(self) -> str:
         return 'CIAO'
 
     def _get_run_id(self) -> str:
         return '60.A-9278(C)'
+
+    def _get_chip_id(self) -> str:
+        return f'CIAO{self._at_number}'
```

### Comparing `aotpy-0.8.1/aotpy/translators/eris.py` & `aotpy-0.8.2/aotpy/translators/eris.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,15 +304,15 @@
                              frame_numbers=ho_frame_numbers.tolist())
 
         ngs = aotpy.NaturalGuideStar('NGS')
         self.system.sources.append(ngs)
 
         eris_data_path = importlib.resources.files('aotpy.data') / 'ERIS'
         with importlib.resources.as_file(eris_data_path / 'ho_subap.fits') as p:
-            subaperture_mask = image_from_file(p, name='LO WFS SUBAPERTURE MASK')
+            subaperture_mask = image_from_file(p, name='HO WFS SUBAPERTURE MASK')
         n_valid_subapertures = np.count_nonzero(subaperture_mask.data != -1)
 
         reference = self._stack_slopes(fits.getdata(self._path / 'HOAcq.DET1.REFSLP_WITH_OFFSETS.fits'),
                                        slope_axis=1)[0]
         ho_wfs = aotpy.ShackHartmann(
             uid='HO WFS',
             source=ngs,
@@ -362,7 +362,10 @@
         return 'ESO-VLT-U4'
 
     def _get_eso_ao_name(self) -> str:
         return 'ERIAO'
 
     def _get_run_id(self) -> str:
         return '60.A-9278(E)'
+
+    def _get_chip_id(self) -> str:
+        return f'ERIAO'
```

### Comparing `aotpy-0.8.1/aotpy/translators/eso.py` & `aotpy-0.8.2/aotpy/translators/eso.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from astropy.time import Time
 
 try:
     from pyvo.dal import tap
 except (ImportError, ModuleNotFoundError):
     tap = None
 
-from ..core.base import Metadatum
+import aotpy
 from .base import BaseTranslator
 
 ESO_TAP_OBS = "https://archive.eso.org/tap_obs"
 
 
 class ESOTranslator(BaseTranslator):
     """Abstract class for translators for ESO systems.
@@ -91,30 +91,39 @@
     @abstractmethod
     def _get_run_id(self) -> str:
         """
         Get the run ID (prog ID) that refers to the data, as defined by ESO.
         """
         pass
 
+    @abstractmethod
+    def _get_chip_id(self) -> str:
+        """
+        Get HIERARCH ESO DET CHIP1 ID for the specific data. This is an ESO archive requirement to ensure compatibility
+        when there are simultaneous recordings of the same instrument on different telescopes.
+        """
+        pass
+
     def add_archive_metadata(self, query_archive: bool = False) -> None:
         """
         Adds necessary metadata for ESO Archive to AOSystem.
 
         Parameters
         ----------
         query_archive : default = False
             Whether the ESO archive should be queried to find relevant metadata already in the archive. Requires pyvo.
         """
         telescope = self._get_eso_telescope_name()
         metadata = {
             'ORIGIN': 'ESO-PARANAL',
+            'DATE': datetime.now().isoformat(timespec='milliseconds'),
+            'TELESCOP': telescope.replace('%', ''),
             'INSTRUME': self._get_eso_ao_name(),
+            'HIERARCH ESO DET CHIP1 ID': self._get_chip_id(),
             'HIERARCH ESO OBS PROG ID': self._get_run_id(),
-            'TELESCOP': telescope.replace('%', ''),
-            'DATE': datetime.now().isoformat(timespec='milliseconds'),
             'OBJECT': 'AO-TELEM',
             'OBSERVER': 'I, Condor',
             'DATE-OBS': self.system.date_beginning.astimezone(timezone.utc).replace(tzinfo=None).isoformat(
                 timespec='milliseconds'),
             'MJD-OBS': Time(self.system.date_beginning, scale='utc').mjd,
             'MJD-END': Time(self.system.date_end, scale='utc').mjd,
             'EXPTIME': (self.system.date_end - self.system.date_beginning).total_seconds(),
@@ -162,15 +171,15 @@
                 if 'HIERARCH ESO TEL AZ' not in metadata:
                     metadata['HIERARCH ESO TEL AZ'] = res['tel_az']
                 if 'HIERARCH ESO TEL ALT' not in metadata:
                     metadata['HIERARCH ESO TEL ALT'] = res['tel_alt']
             else:
                 warnings.warn(f"Could not find data from telescope '{telescope}' near mjd_obs {beg.mjd} at the "
                               f"ESO Archive")
-        self.system.metadata.extend([Metadatum(k, v) for k, v in metadata.items()])
+        self.system.metadata.extend([aotpy.Metadatum(k, v) for k, v in metadata.items()])
 
     def get_atmospheric_parameters_from_archive(self) -> astropy.table.Table:
         """
         Get atmospheric data from ESO's Science Archive within the recording period.
 
         Requires pyvo.
         """
```

### Comparing `aotpy-0.8.1/aotpy/translators/galacsi.py` & `aotpy-0.8.2/aotpy/translators/galacsi.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,7 +230,10 @@
         return 'ESO-VLT-U4'
 
     def _get_eso_ao_name(self) -> str:
         return 'GALACSI'
 
     def _get_run_id(self) -> str:
         return '60.A-9278(B)'
+
+    def _get_chip_id(self) -> str:
+        return f'GALACSI'
```

### Comparing `aotpy-0.8.1/aotpy/translators/naomi.py` & `aotpy-0.8.2/aotpy/translators/naomi.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,7 +157,10 @@
         return f"ESO-VLTI-%A%{self._at_number}%"
 
     def _get_eso_ao_name(self) -> str:
         return 'NAOMI'
 
     def _get_run_id(self) -> str:
         return '60.A-9278(D)'
+
+    def _get_chip_id(self) -> str:
+        return f'NAOMI{self._at_number}'
```

### Comparing `aotpy-0.8.1/aotpy/translators/papyrus.py` & `aotpy-0.8.2/aotpy/translators/papyrus.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,16 @@
         time_stamp_measurements = (np.array(data['wfsSlopesMetaData']['timestamp'], dtype=float) / 1e9).tolist()
         frame_number_pixel_intensities = np.array(data['wfsImagesMetaData']['frameid'], dtype=float).tolist()
         time_stamp_pixel_intensities = (np.array(data['wfsImagesMetaData']['timestamp'], dtype=float) / 1e9).tolist()
         frame_number_commands = np.array(data['wfcCommandMetaData']['frameid'], dtype=float).tolist()
         time_stamp_commands = (np.array(data['wfcCommandMetaData']['timestamp'], dtype=float) / 1e9).tolist()
 
         # extract acquisition date from time stamps
-        self.system.date_beginning = datetime.datetime.fromtimestamp(time_stamp_commands[0])
-        self.system.date_end = datetime.datetime.fromtimestamp(time_stamp_commands[-1])
+        self.system.date_beginning = datetime.datetime.utcfromtimestamp(time_stamp_commands[0])
+        self.system.date_end = datetime.datetime.utcfromtimestamp(time_stamp_commands[-1])
 
         time_measurements = aotpy.Time(uid='Measurements time',
                                        timestamps=time_stamp_measurements,
                                        frame_numbers=frame_number_measurements)
 
         time_pixel_intensities = aotpy.Time(uid='WFS detector frames time',
                                             timestamps=time_stamp_pixel_intensities,
```

### Comparing `aotpy-0.8.1/aotpy.egg-info/PKG-INFO` & `aotpy-0.8.2/aotpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aotpy
-Version: 0.8.1
+Version: 0.8.2
 Summary: Helper package for handling Adaptive Optics Telemetry (AOT) standard files
 Home-page: https://github.com/STAR-PORT/aotpy
 Author: Tiago Gomes
 Author-email: tiagogomes@fe.up.pt
 Project-URL: Bug Tracker, https://github.com/STAR-PORT/aotpy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -16,14 +16,17 @@
 Description-Content-Type: text/markdown
 Provides-Extra: esoarchive
 Provides-Extra: savfiles
 Provides-Extra: docs
 Provides-Extra: all
 License-File: LICENSE
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8187230.svg)](https://doi.org/10.5281/zenodo.8187230)
+
+
 # aotpy
 Helper Python package for handling Adaptive Optics Telemetry (AOT) standard files.
 Basic [documentation available](https://aotpy.readthedocs.io/en/latest/).
 
 ## How to install
 Support is offered for Python 3.10 or later.
```

### Comparing `aotpy-0.8.1/aotpy.egg-info/SOURCES.txt` & `aotpy-0.8.2/aotpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aotpy-0.8.1/setup.cfg` & `aotpy-0.8.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6f74 7079 0d0a 7665 7273 696f   = aotpy..versio
-00000020: 6e20 3d20 302e 382e 310d 0a61 7574 686f  n = 0.8.1..autho
+00000020: 6e20 3d20 302e 382e 320d 0a61 7574 686f  n = 0.8.2..autho
 00000030: 7220 3d20 5469 6167 6f20 476f 6d65 730d  r = Tiago Gomes.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7469 6167 6f67 6f6d 6573 4066 652e 7570  tiagogomes@fe.up
 00000060: 2e70 740d 0a64 6573 6372 6970 7469 6f6e  .pt..description
 00000070: 203d 2048 656c 7065 7220 7061 636b 6167   = Helper packag
 00000080: 6520 666f 7220 6861 6e64 6c69 6e67 2041  e for handling A
 00000090: 6461 7074 6976 6520 4f70 7469 6373 2054  daptive Optics T
```

