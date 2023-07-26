# Comparing `tmp/gpcal-0.9.5.0.tar.gz` & `tmp/gpcal-0.9.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpcal-0.9.5.0.tar", last modified: Wed Jul 26 06:59:58 2023, max compression
+gzip compressed data, was "dist/gpcal-0.9.5.1.tar", last modified: Wed Jul 26 07:03:34 2023, max compression
```

## Comparing `gpcal-0.9.5.0.tar` & `gpcal-0.9.5.1.tar`

### file list

```diff
@@ -1,22 +1,15 @@
-drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 06:59:58.688346 gpcal-0.9.5.0/
--rw-rw-r--   0 jpark     (1000) jpark     (1000)      662 2023-07-26 06:59:58.688346 gpcal-0.9.5.0/PKG-INFO
--rw-r--r--   0 jpark     (1000) jpark     (1000)     2991 2023-03-20 13:01:37.000000 gpcal-0.9.5.0/README.rst
-drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 06:59:58.688346 gpcal-0.9.5.0/gpcal/
--rw-r--r--   0 jpark     (1000) jpark     (1000)      209 2023-07-26 06:46:08.000000 gpcal-0.9.5.0/gpcal/__init__.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)    15099 2023-07-26 06:24:04.000000 gpcal-0.9.5.0/gpcal/aipsutil.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    66474 2023-07-26 06:24:04.000000 gpcal-0.9.5.0/gpcal/channelcal.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)     1256 2023-07-26 06:24:04.000000 gpcal-0.9.5.0/gpcal/cleanhelpers.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)   193550 2023-07-26 06:24:04.000000 gpcal-0.9.5.0/gpcal/gpcal.py
--rw-r--r--   0 jpark     (1000) jpark     (1000)    27032 2023-07-26 06:24:04.000000 gpcal-0.9.5.0/gpcal/obshelpers.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    19954 2023-07-26 06:24:04.000000 gpcal-0.9.5.0/gpcal/plothelpers.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    36468 2023-07-26 06:24:04.000000 gpcal-0.9.5.0/gpcal/polsolver.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    25263 2023-07-26 06:24:04.000000 gpcal-0.9.5.0/gpcal/synthetic.py
--rw-rw-r--   0 jpark     (1000) jpark     (1000)    67744 2023-07-26 06:24:04.000000 gpcal-0.9.5.0/gpcal/timecal.py
-drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 06:59:58.688346 gpcal-0.9.5.0/gpcal.egg-info/
--rw-rw-r--   0 jpark     (1000) jpark     (1000)      662 2023-07-26 06:59:58.000000 gpcal-0.9.5.0/gpcal.egg-info/PKG-INFO
--rw-rw-r--   0 jpark     (1000) jpark     (1000)      362 2023-07-26 06:59:58.000000 gpcal-0.9.5.0/gpcal.egg-info/SOURCES.txt
--rw-rw-r--   0 jpark     (1000) jpark     (1000)        1 2023-07-26 06:59:58.000000 gpcal-0.9.5.0/gpcal.egg-info/dependency_links.txt
--rw-rw-r--   0 jpark     (1000) jpark     (1000)       38 2023-07-26 06:59:58.000000 gpcal-0.9.5.0/gpcal.egg-info/requires.txt
--rw-rw-r--   0 jpark     (1000) jpark     (1000)        6 2023-07-26 06:59:58.000000 gpcal-0.9.5.0/gpcal.egg-info/top_level.txt
--rw-r--r--   0 jpark     (1000) jpark     (1000)       79 2023-07-26 06:59:58.688346 gpcal-0.9.5.0/setup.cfg
--rw-r--r--   0 jpark     (1000) jpark     (1000)     1653 2023-07-26 06:59:53.000000 gpcal-0.9.5.0/setup.py
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 07:03:34.000000 gpcal-0.9.5.1/
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)      701 2023-07-26 07:03:34.000000 gpcal-0.9.5.1/PKG-INFO
+-rw-r--r--   0 jpark     (1000) jpark     (1000)       62 2023-03-20 13:01:37.000000 gpcal-0.9.5.1/setup.cfg
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     1653 2023-07-26 07:03:28.000000 gpcal-0.9.5.1/setup.py
+drwxrwxr-x   0 jpark     (1000) jpark     (1000)        0 2023-07-26 07:03:34.000000 gpcal-0.9.5.1/gpcal/
+-rw-r--r--   0 jpark     (1000) jpark     (1000)      209 2023-07-26 06:46:08.000000 gpcal-0.9.5.1/gpcal/__init__.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    25255 2023-07-26 07:02:43.000000 gpcal-0.9.5.1/gpcal/synthetic.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)     1256 2023-07-26 06:24:04.000000 gpcal-0.9.5.1/gpcal/cleanhelpers.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    36452 2023-07-26 07:02:38.000000 gpcal-0.9.5.1/gpcal/polsolver.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    67724 2023-07-26 07:02:48.000000 gpcal-0.9.5.1/gpcal/timecal.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)    15099 2023-07-26 06:24:04.000000 gpcal-0.9.5.1/gpcal/aipsutil.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)    27028 2023-07-26 07:02:26.000000 gpcal-0.9.5.1/gpcal/obshelpers.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    66454 2023-07-26 07:02:11.000000 gpcal-0.9.5.1/gpcal/channelcal.py
+-rw-r--r--   0 jpark     (1000) jpark     (1000)   193550 2023-07-26 06:24:04.000000 gpcal-0.9.5.1/gpcal/gpcal.py
+-rw-rw-r--   0 jpark     (1000) jpark     (1000)    19950 2023-07-26 07:02:32.000000 gpcal-0.9.5.1/gpcal/plothelpers.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `gpcal-0.9.5.0/PKG-INFO` & `gpcal-0.9.5.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: gpcal
-Version: 0.9.5.0
+Version: 0.9.5.1
 Summary: A generalized instrumental polarization calibration pipeline for VLBI data
 Home-page: https://github.com/jhparkastro/gpcal
-Download-URL: https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz
 Author: Jongho Park
 Author-email: jpark@asiaa.sinica.edu.tw
 License: gpl-2.0
+Download-URL: https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz
+Description: UNKNOWN
 Keywords: VLBI,polarimetry,astronomy,calibration
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `gpcal-0.9.5.0/gpcal/aipsutil.py` & `gpcal-0.9.5.1/gpcal/aipsutil.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.0/gpcal/channelcal.py` & `gpcal-0.9.5.1/gpcal/channelcal.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
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

### Comparing `gpcal-0.9.5.0/gpcal/cleanhelpers.py` & `gpcal-0.9.5.1/gpcal/cleanhelpers.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.0/gpcal/gpcal.py` & `gpcal-0.9.5.1/gpcal/gpcal.py`

 * *Files identical despite different names*

### Comparing `gpcal-0.9.5.0/gpcal/obshelpers.py` & `gpcal-0.9.5.1/gpcal/obshelpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 from AIPS import AIPS
 from AIPSTask import AIPSTask
 from AIPSData import AIPSUVData, AIPSImage
 from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
 
-import gpcaltest.aipsutil as au
+import gpcal.aipsutil as au
 
 from os import path
 
 from IPython import embed
 
 
 def uvprt(data, select):
```

### Comparing `gpcal-0.9.5.0/gpcal/plothelpers.py` & `gpcal-0.9.5.1/gpcal/plothelpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 import numpy as np
 
 import matplotlib
 import matplotlib.pyplot as plt
 
-import gpcaltest.obshelpers as oh
+import gpcal.obshelpers as oh
 
 from multiprocessing import Pool
 
 from IPython import embed
 
 
 # Default matplotlib parameters
```

### Comparing `gpcal-0.9.5.0/gpcal/polsolver.py` & `gpcal-0.9.5.1/gpcal/polsolver.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import astropy.time as at
 
 from AIPS import AIPS
 from AIPSTask import AIPSTask
 from AIPSData import AIPSUVData, AIPSImage
 from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
 
-# import gpcaltest.gpcal as gp
-import gpcaltest.aipsutil as au
-import gpcaltest.obshelpers as oh
-import gpcaltest.plothelpers as ph
+# import gpcal.gpcal as gp
+import gpcal.aipsutil as au
+import gpcal.obshelpers as oh
+import gpcal.plothelpers as ph
 
 import os
 from os import path
 
 from IPython import embed
```

### Comparing `gpcal-0.9.5.0/gpcal/synthetic.py` & `gpcal-0.9.5.1/gpcal/synthetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import numpy as np
 import pandas as pd
 
 from AIPSData import AIPSUVData, AIPSImage
 from Wizardry.AIPSData import AIPSUVData as WAIPSUVData
 
-import gpcaltest.aipsutil as au
-import gpcaltest.obshelpers as oh
+import gpcal.aipsutil as au
+import gpcal.obshelpers as oh
 
 import os
 
 from IPython import embed
 
 
 def synthetic_deq(nant, pang1, pang2, ant1, ant2, llamp, llphas, rramp, rrphas, model_ireal, model_iimag, model_rlreal, model_rlimag, model_lrreal, model_lrimag, stokes, *p):
```

### Comparing `gpcal-0.9.5.0/gpcal/timecal.py` & `gpcal-0.9.5.1/gpcal/timecal.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 
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

### Comparing `gpcal-0.9.5.0/setup.py` & `gpcal-0.9.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'gpcal',         # How you named your package folder (MyLib)
   packages = ['gpcal'],   # Chose the same as "name"
-  version = '0.9.5.0',      # Start with a small number and increase it with every change you make
+  version = '0.9.5.1',      # Start with a small number and increase it with every change you make
   license='gpl-2.0',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'A generalized instrumental polarization calibration pipeline for VLBI data',   # Give a short description about your library
   author = 'Jongho Park',                   # Type in your name
   author_email = 'jpark@asiaa.sinica.edu.tw',      # Type in your E-Mail
   url = 'https://github.com/jhparkastro/gpcal',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/jhparkastro/gpcal/archive/v1.0.tar.gz',    # I explain this later on
   keywords = ['VLBI', 'polarimetry', 'astronomy', 'calibration'],   # Keywords that define your package best
```

