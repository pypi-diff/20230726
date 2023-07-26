# Comparing `tmp/gpcal-0.9.5.1.tar.gz` & `tmp/gpcal-0.9.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gpcal-0.9.5.1.tar", last modified: Wed Jul 26 07:03:34 2023, max compression
+gzip compressed data, was "dist/gpcal-0.9.5.2.tar", last modified: Wed Jul 26 07:06:06 2023, max compression
```

## Comparing `gpcal-0.9.5.1.tar` & `gpcal-0.9.5.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 07:03:34.000000 gpcal-0.9.5.1/
--rw-rw-r--   0 jpark     (1000) jpark     (1000)      701 2023-07-26 07:03:34.000000 gpcal-0.9.5.1/PKG-INFO
--rw-r--r--   0 jpark     (1000) jpark     (1000)       62 2023-03-20 13:01:37.000000 gpcal-0.9.5.1/setup.cfg
--rw-r--r--   0 jpark     (1000) jpark     (1000)     1653 2023-07-26 07:03:28.000000 gpcal-0.9.5.1/setup.py
-drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 07:03:34.000000 gpcal-0.9.5.1/gpcal/
--rw-r--r--   0 jpark     (1000) jpark     (1000)      209 2023-07-26 06:46:08.000000 gpcal-0.9.5.1/gpcal/__init__.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    25255 2023-07-26 07:02:43.000000 gpcal-0.9.5.1/gpcal/synthetic.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)     1256 2023-07-26 06:24:04.000000 gpcal-0.9.5.1/gpcal/cleanhelpers.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    36452 2023-07-26 07:02:38.000000 gpcal-0.9.5.1/gpcal/polsolver.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    67724 2023-07-26 07:02:48.000000 gpcal-0.9.5.1/gpcal/timecal.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)    15099 2023-07-26 06:24:04.000000 gpcal-0.9.5.1/gpcal/aipsutil.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)    27028 2023-07-26 07:02:26.000000 gpcal-0.9.5.1/gpcal/obshelpers.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    66454 2023-07-26 07:02:11.000000 gpcal-0.9.5.1/gpcal/channelcal.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)   193550 2023-07-26 06:24:04.000000 gpcal-0.9.5.1/gpcal/gpcal.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    19950 2023-07-26 07:02:32.000000 gpcal-0.9.5.1/gpcal/plothelpers.py
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 07:06:06.000000 gpcal-0.9.5.2/
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)      701 2023-07-26 07:06:06.000000 gpcal-0.9.5.2/PKG-INFO
+-rw-r--r--   0 jpark     (1000) jpark     (1000)       62 2023-03-20 13:01:37.000000 gpcal-0.9.5.2/setup.cfg
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     1653 2023-07-26 07:05:40.000000 gpcal-0.9.5.2/setup.py
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 07:06:06.000000 gpcal-0.9.5.2/gpcal/
+-rw-r--r--   0 jpark     (1000) jpark     (1000)      209 2023-07-26 06:46:08.000000 gpcal-0.9.5.2/gpcal/__init__.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    25255 2023-07-26 07:02:43.000000 gpcal-0.9.5.2/gpcal/synthetic.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     1256 2023-07-26 06:24:04.000000 gpcal-0.9.5.2/gpcal/cleanhelpers.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    36452 2023-07-26 07:02:38.000000 gpcal-0.9.5.2/gpcal/polsolver.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    67724 2023-07-26 07:02:48.000000 gpcal-0.9.5.2/gpcal/timecal.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)    15099 2023-07-26 06:24:04.000000 gpcal-0.9.5.2/gpcal/aipsutil.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)    27028 2023-07-26 07:02:26.000000 gpcal-0.9.5.2/gpcal/obshelpers.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    66454 2023-07-26 07:02:11.000000 gpcal-0.9.5.2/gpcal/channelcal.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)   193530 2023-07-26 07:05:20.000000 gpcal-0.9.5.2/gpcal/gpcal.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    19950 2023-07-26 07:02:32.000000 gpcal-0.9.5.2/gpcal/plothelpers.py
```

### Comparing `gpcal-0.9.5.1/PKG-INFO` & `gpcal-0.9.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gpcal
-Version: 0.9.5.1
+Version: 0.9.5.2
 Summary: A generalized instrumental polarization calibration pipeline for VLBI data
 Home-page: https://github.com/jhparkastro/gpcal
 Author: Jongho Park
 Author-email: jpark@asiaa.sinica.edu.tw
 License: gpl-2.0
 Download-URL: https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz
 Description: UNKNOWN
```

### Comparing `gpcal-0.9.5.1/setup.py` & `gpcal-0.9.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'gpcal',         # How you named your package folder (MyLib)
   packages = ['gpcal'],   # Chose the same as "name"
-  version = '0.9.5.1',      # Start with a small number and increase it with every change you make
+  version = '0.9.5.2',      # Start with a small number and increase it with every change you make
   license='gpl-2.0',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A generalized instrumental polarization calibration pipeline for VLBI data',   # Give a short description about your library
   author = 'Jongho Park',                   # Type in your name
   author_email = 'jpark@asiaa.sinica.edu.tw',      # Type in your E-Mail
   url = 'https://github.com/jhparkastro/gpcal',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz',    # I explain this later on
   keywords = ['VLBI', 'polarimetry', 'astronomy', 'calibration'],   # Keywords that define your package best
```

### Comparing `gpcal-0.9.5.1/gpcal/synthetic.py` & `gpcal-0.9.5.2/gpcal/synthetic.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.1/gpcal/cleanhelpers.py` & `gpcal-0.9.5.2/gpcal/cleanhelpers.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.1/gpcal/polsolver.py` & `gpcal-0.9.5.2/gpcal/polsolver.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.1/gpcal/timecal.py` & `gpcal-0.9.5.2/gpcal/timecal.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.1/gpcal/aipsutil.py` & `gpcal-0.9.5.2/gpcal/aipsutil.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.1/gpcal/obshelpers.py` & `gpcal-0.9.5.2/gpcal/obshelpers.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.1/gpcal/channelcal.py` & `gpcal-0.9.5.2/gpcal/channelcal.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.1/gpcal/gpcal.py` & `gpcal-0.9.5.2/gpcal/gpcal.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
 from scipy.optimize import curve_fit
 
 import matplotlib
 matplotlib.use('Agg')
 import matplotlib.pyplot as plt
 
-import gpcaltest.aipsutil as au
-import gpcaltest.obshelpers as oh
-import gpcaltest.cleanhelpers as ch
-import gpcaltest.plothelpers as ph
-import gpcaltest.polsolver as ps
+import gpcal.aipsutil as au
+import gpcal.obshelpers as oh
+import gpcal.cleanhelpers as ch
+import gpcal.plothelpers as ph
+import gpcal.polsolver as ps
 
 import gc
 import psutil
 
 from astropy.io import fits
 
 from multiprocessing import cpu_count, Pool
```

### Comparing `gpcal-0.9.5.1/gpcal/plothelpers.py` & `gpcal-0.9.5.2/gpcal/plothelpers.py`

 * *Files identical despite different names*

