# Comparing `tmp/swatmf-0.2.4.tar.gz` & `tmp/swatmf-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swatmf-0.2.4.tar", last modified: Wed Sep 21 21:21:55 2022, max compression
+gzip compressed data, was "swatmf-0.3.0.tar", last modified: Wed Jul 26 19:46:04 2023, max compression
```

## Comparing `swatmf-0.2.4.tar` & `swatmf-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxrwxrwx   0        0        0        0 2022-09-21 21:21:55.207306 swatmf-0.2.4/
--rw-rw-rw-   0        0        0     1549 2022-02-07 21:13:22.000000 swatmf-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       26 2022-02-04 16:08:00.000000 swatmf-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2249 2022-09-21 21:21:55.205275 swatmf-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     1213 2022-06-17 05:15:57.000000 swatmf-0.2.4/README.rst
--rw-rw-rw-   0        0        0       42 2022-09-21 21:21:55.209313 swatmf-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1839 2022-09-21 21:21:10.000000 swatmf-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-21 21:21:54.998682 swatmf-0.2.4/swatmf/
--rw-rw-rw-   0        0        0      410 2022-06-19 04:02:57.000000 swatmf-0.2.4/swatmf/__init__.py
--rw-rw-rw-   0        0        0        0 2022-09-19 20:46:24.000000 swatmf-0.2.4/swatmf/cvt_gcm_pcp.py
--rw-rw-rw-   0        0        0     3896 2022-06-22 01:42:51.000000 swatmf-0.2.4/swatmf/forward_run.py
--rw-rw-rw-   0        0        0        0 2022-09-19 20:46:14.000000 swatmf-0.2.4/swatmf/gcm_analysis.py
--rw-rw-rw-   0        0        0     6531 2022-05-31 21:15:54.000000 swatmf-0.2.4/swatmf/gumu_pst_utils.py
-drwxrwxrwx   0        0        0        0 2022-09-21 21:21:55.065592 swatmf-0.2.4/swatmf/hg/
--rw-rw-rw-   0        0        0      479 2022-06-20 21:36:01.000000 swatmf-0.2.4/swatmf/hg/__init__.py
--rw-rw-rw-   0        0        0    12791 2022-09-19 22:19:15.000000 swatmf-0.2.4/swatmf/hg/hg_handler.py
--rw-rw-rw-   0        0        0     4357 2022-06-21 16:07:42.000000 swatmf-0.2.4/swatmf/hg/viz.py
-drwxrwxrwx   0        0        0        0 2022-09-21 21:21:55.186272 swatmf-0.2.4/swatmf/opt_files/
--rw-rw-rw-   0        0        0    56149 2020-06-05 14:31:21.000000 swatmf-0.2.4/swatmf/opt_files/Absolute_SWAT_Values.txt
--rwxrwxrwx   0        0        0   538085 2015-05-12 21:22:20.000000 swatmf-0.2.4/swatmf/opt_files/SUFI2_LH_sample.exe
--rwxrwxrwx   0        0        0   203776 2014-09-23 20:29:02.000000 swatmf-0.2.4/swatmf/opt_files/Swat_Edit.exe
--rwxrwxrwx   0        0        0  2826752 2019-05-12 16:54:36.000000 swatmf-0.2.4/swatmf/opt_files/beopest64.exe
--rwxrwxrwx   0        0        0  2470400 2017-04-27 22:26:52.000000 swatmf-0.2.4/swatmf/opt_files/i64pest.exe
--rwxrwxrwx   0        0        0   844288 2019-11-21 19:44:00.000000 swatmf-0.2.4/swatmf/opt_files/i64pwtadj1.exe
--rw-rw-rw-   0        0        0       57 2022-02-03 23:26:08.000000 swatmf-0.2.4/swatmf/opt_files/model.in
--rw-rw-rw-   0        0        0     1159 2020-06-02 21:21:54.000000 swatmf-0.2.4/swatmf/swatmf_par_chg_run.py
--rw-rw-rw-   0        0        0    15291 2022-07-05 02:24:09.000000 swatmf-0.2.4/swatmf/swatmf_pst_par.py
--rw-rw-rw-   0        0        0     3076 2022-06-16 05:35:37.000000 swatmf-0.2.4/swatmf/swatmf_pst_stats.py
--rw-rw-rw-   0        0        0    30015 2022-08-08 16:32:23.000000 swatmf-0.2.4/swatmf/swatmf_pst_utils.py
--rw-rw-rw-   0        0        0    12353 2022-02-14 16:15:02.000000 swatmf-0.2.4/swatmf/swatmf_scenario_utils.py
--rw-rw-rw-   0        0        0    26793 2022-02-09 05:07:37.000000 swatmf-0.2.4/swatmf/swatmf_viz.py
-drwxrwxrwx   0        0        0        0 2022-09-21 21:21:55.198273 swatmf-0.2.4/swatmf/utils/
--rw-rw-rw-   0        0        0      490 2022-09-19 21:01:09.000000 swatmf-0.2.4/swatmf/utils/__init__.py
--rw-rw-rw-   0        0        0     9114 2022-09-21 18:43:47.000000 swatmf-0.2.4/swatmf/utils/swat_utils.py
--rw-rw-rw-   0        0        0    17885 2022-06-21 15:05:50.000000 swatmf-0.2.4/swatmf/utils.py
--rw-rw-rw-   0        0        0       23 2022-09-21 21:20:59.000000 swatmf-0.2.4/swatmf/version.py
-drwxrwxrwx   0        0        0        0 2022-09-21 21:21:55.038724 swatmf-0.2.4/swatmf.egg-info/
--rw-rw-rw-   0        0        0     2249 2022-09-21 21:21:54.000000 swatmf-0.2.4/swatmf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      837 2022-09-21 21:21:54.000000 swatmf-0.2.4/swatmf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-21 21:21:54.000000 swatmf-0.2.4/swatmf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2022-09-21 21:21:54.000000 swatmf-0.2.4/swatmf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-21 21:21:54.000000 swatmf-0.2.4/swatmf.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.555612 swatmf-0.3.0/
+-rw-rw-rw-   0        0        0     1549 2022-02-07 21:13:22.000000 swatmf-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       26 2022-02-04 16:08:00.000000 swatmf-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5147 2023-07-26 19:46:04.552611 swatmf-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4058 2023-07-26 19:45:51.000000 swatmf-0.3.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-26 19:46:04.557613 swatmf-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1868 2023-07-26 19:44:06.000000 swatmf-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.274531 swatmf-0.3.0/swatmf/
+-rw-rw-rw-   0        0        0      410 2022-06-19 04:02:57.000000 swatmf-0.3.0/swatmf/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-09-19 20:46:24.000000 swatmf-0.3.0/swatmf/cvt_gcm_pcp.py
+-rw-rw-rw-   0        0        0     4059 2023-07-26 16:30:38.000000 swatmf-0.3.0/swatmf/forward_run.py
+-rw-rw-rw-   0        0        0        0 2022-09-19 20:46:14.000000 swatmf-0.3.0/swatmf/gcm_analysis.py
+-rw-rw-rw-   0        0        0     6531 2022-05-31 21:15:54.000000 swatmf-0.3.0/swatmf/gumu_pst_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.343551 swatmf-0.3.0/swatmf/hg/
+-rw-rw-rw-   0        0        0      479 2022-06-20 21:36:01.000000 swatmf-0.3.0/swatmf/hg/__init__.py
+-rw-rw-rw-   0        0        0    12791 2022-09-19 22:19:15.000000 swatmf-0.3.0/swatmf/hg/hg_handler.py
+-rw-rw-rw-   0        0        0     4357 2022-06-21 16:07:42.000000 swatmf-0.3.0/swatmf/hg/viz.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.506599 swatmf-0.3.0/swatmf/opt_files/
+-rw-rw-rw-   0        0        0    56149 2020-06-05 14:31:21.000000 swatmf-0.3.0/swatmf/opt_files/Absolute_SWAT_Values.txt
+-rwxrwxrwx   0        0        0   538085 2015-05-12 21:22:20.000000 swatmf-0.3.0/swatmf/opt_files/SUFI2_LH_sample.exe
+-rwxrwxrwx   0        0        0   203776 2014-09-23 20:29:02.000000 swatmf-0.3.0/swatmf/opt_files/Swat_Edit.exe
+-rwxrwxrwx   0        0        0   844288 2019-11-21 19:44:00.000000 swatmf-0.3.0/swatmf/opt_files/i64pwtadj1.exe
+-rw-rw-rw-   0        0        0       57 2022-02-03 23:26:08.000000 swatmf-0.3.0/swatmf/opt_files/model.in
+-rwxrwxrwx   0        0        0  3742208 2023-04-25 07:17:33.000000 swatmf-0.3.0/swatmf/opt_files/pestpp-glm.exe
+-rwxrwxrwx   0        0        0  4294656 2023-04-25 07:17:31.000000 swatmf-0.3.0/swatmf/opt_files/pestpp-ies.exe
+-rwxrwxrwx   0        0        0  4382720 2023-04-25 07:17:32.000000 swatmf-0.3.0/swatmf/opt_files/pestpp-opt.exe
+-rwxrwxrwx   0        0        0  2186752 2023-04-25 07:17:32.000000 swatmf-0.3.0/swatmf/opt_files/pestpp-sen.exe
+-rw-rw-rw-   0        0        0     1159 2020-06-02 21:21:54.000000 swatmf-0.3.0/swatmf/swatmf_par_chg_run.py
+-rw-rw-rw-   0        0        0    15291 2022-07-05 02:24:09.000000 swatmf-0.3.0/swatmf/swatmf_pst_par.py
+-rw-rw-rw-   0        0        0     3076 2022-06-16 05:35:37.000000 swatmf-0.3.0/swatmf/swatmf_pst_stats.py
+-rw-rw-rw-   0        0        0    30439 2023-07-25 17:41:32.000000 swatmf-0.3.0/swatmf/swatmf_pst_utils.py
+-rw-rw-rw-   0        0        0    12353 2022-02-14 16:15:02.000000 swatmf-0.3.0/swatmf/swatmf_scenario_utils.py
+-rw-rw-rw-   0        0        0    30561 2023-07-26 16:30:38.000000 swatmf-0.3.0/swatmf/swatmf_viz.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.543610 swatmf-0.3.0/swatmf/utils/
+-rw-rw-rw-   0        0        0      490 2022-09-19 21:01:09.000000 swatmf-0.3.0/swatmf/utils/__init__.py
+-rw-rw-rw-   0        0        0      547 2022-11-22 22:19:38.000000 swatmf-0.3.0/swatmf/utils/etc.py
+-rw-rw-rw-   0        0        0     9114 2022-10-04 13:58:18.000000 swatmf-0.3.0/swatmf/utils/swat_utils.py
+-rw-rw-rw-   0        0        0    17877 2023-07-25 17:43:32.000000 swatmf-0.3.0/swatmf/utils.py
+-rw-rw-rw-   0        0        0       23 2023-07-26 19:23:40.000000 swatmf-0.3.0/swatmf/version.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:46:04.321544 swatmf-0.3.0/swatmf.egg-info/
+-rw-rw-rw-   0        0        0     5147 2023-07-26 19:46:03.000000 swatmf-0.3.0/swatmf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      925 2023-07-26 19:46:03.000000 swatmf-0.3.0/swatmf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 19:46:03.000000 swatmf-0.3.0/swatmf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2023-07-26 19:46:03.000000 swatmf-0.3.0/swatmf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 19:46:03.000000 swatmf-0.3.0/swatmf.egg-info/top_level.txt
```

### Comparing `swatmf-0.2.4/LICENSE` & `swatmf-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/setup.py` & `swatmf-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from setuptools import setup, find_packages
+from setuptools import setup, find_packages, Extension
 import codecs
 import os
 
+# long description!!
+
 # here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 #
 
 with open("README.rst", "r") as fd:
     long_desc = fd.read()
 
 
-VERSION = '0.2.4'
+VERSION = '0.3.0'
 DESCRIPTION = 'swatmf is a set of python modules for SWAT-MODFLOW model evaluation and parameter estimation.'
 # LONG_DESCRIPTION = 'A package that allows to work with SWAT-MODFLOW model'
 
 license = "BSD-3-Clause"
 # Setting up
 setup(
     name="swatmf",
@@ -36,21 +38,21 @@
 
     include_package_data=True,
     package_data = {
         'opt_files': ['*'],
     },
     packages=find_packages(),
     install_requires=[
-        'pandas', 'numpy', 'pyemu', 'flopy<=3.3.4', 'scipy', 'matplotlib', 'openpyxl',
+        'pandas', 'numpy', 'pyemu', 'flopy', 'scipy', 'matplotlib', 'openpyxl',
         'hydroeval', 'tqdm', 'termcolor', 'pyshp'],
     keywords=['python', 'SWAT-MODFLOW', 'PEST'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         "Operating System :: Microsoft :: Windows",
         "License :: OSI Approved :: BSD License"
     ]
 )
```

### Comparing `swatmf-0.2.4/swatmf/forward_run.py` & `swatmf-0.3.0/swatmf/forward_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import os
 from datetime import datetime
 import pyemu
 import pandas as pd
+import sys
+import subprocess
+
+path = "D:/spark/gits/swatmf"
+sys.path.insert(1, path)
+
 from swatmf import swatmf_pst_par, utils
 from swatmf import swatmf_pst_utils
 
-
 wd = os.getcwd()
 os.chdir(wd)
 
 def time_stamp(des):
     time = datetime.now().strftime('[%m/%d/%y %H:%M:%S]')
     print('\n' + 35*'+ ')
     print(time + ' |  {} ...'.format(des))
@@ -26,16 +31,18 @@
     data_fac = pp_included
     for i in data_fac:
         outfile = i + '.ref'
         pyemu.utils.geostats.fac2real(i, factors_file=i+'.fac', out_file=outfile)
 
 def execute_swat_edit():
     des = "modifying SWAT parameters"
-    time_stamp(des)
-    pyemu.os_utils.run('Swat_Edit.exe', cwd='.')
+    # time_stamp(des)
+    # pyemu.os_utils.run('Swat_Edit.exe', cwd='.')
+    p = subprocess.Popen('Swat_Edit.exe' , cwd = '.')
+    p.wait()
 
 def execute_swatmf():
     des = "running model"
     time_stamp(des)
     # pyemu.os_utils.run('APEX-MODFLOW3.exe >_s+m.stdout', cwd='.')
     pyemu.os_utils.run('SWAT-MODFLOW3', cwd='.')
```

### Comparing `swatmf-0.2.4/swatmf/gumu_pst_utils.py` & `swatmf-0.3.0/swatmf/gumu_pst_utils.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/hg/hg_handler.py` & `swatmf-0.3.0/swatmf/hg/hg_handler.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/hg/viz.py` & `swatmf-0.3.0/swatmf/hg/viz.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/opt_files/Absolute_SWAT_Values.txt` & `swatmf-0.3.0/swatmf/opt_files/Absolute_SWAT_Values.txt`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/opt_files/SUFI2_LH_sample.exe` & `swatmf-0.3.0/swatmf/opt_files/SUFI2_LH_sample.exe`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/opt_files/Swat_Edit.exe` & `swatmf-0.3.0/swatmf/opt_files/Swat_Edit.exe`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/opt_files/i64pwtadj1.exe` & `swatmf-0.3.0/swatmf/opt_files/i64pwtadj1.exe`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/swatmf_par_chg_run.py` & `swatmf-0.3.0/swatmf/swatmf_par_chg_run.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/swatmf_pst_par.py` & `swatmf-0.3.0/swatmf/swatmf_pst_par.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/swatmf_pst_stats.py` & `swatmf-0.3.0/swatmf/swatmf_pst_stats.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/swatmf_pst_utils.py` & `swatmf-0.3.0/swatmf/swatmf_pst_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """ PEST support utilities: 12/4/2019 created by Seonggyu Park
-    last modified day: 09/14/2020 by Seonggyu Park
 """
 
 # from lib2to3.pgen2.token import NEWLINE
 import pandas as pd
 import numpy as np
 import time
 from pyemu.pst.pst_utils import SFMT,IFMT,FFMT
@@ -25,16 +24,17 @@
 
 
 
 def create_swatmf_con(
                 wd, sim_start, warmup, cal_start, cal_end,
                 subs=None, grids=None, riv_parm=None,
                 baseflow=None,
-                time_step=None, 
-                pp_included=None
+                time_step=None,
+                pp_included=None,
+                # depth_to_water=None, 
                 ):
     """create swatmf.con file containg SWAT-MODFLOW model PEST initial settings
 
     Args:
         wd (`str`): SWAT-MODFLOW working directory
         subs (`list`): reach numbers to be extracted
         grids (`list`): grid numbers to be extracted
@@ -58,58 +58,67 @@
         riv_parm = 'n'
     else:
         riv_parm = 'y'
     if time_step is None:
         time_step = 'day'
     if baseflow is None:
         baseflow = 'n'
-    if pp_included is None:
-        pp_included = 'n'
     else:
         baseflow = 'y'
+    if pp_included is None:
+        pp_included = 'n'
+    # if depth_to_water is None:
+    #     depth_to_water = 'n'
+
+
     col01 = [
         'wd', 'sim_start', 'warm-up', 'cal_start', 'cal_end',
         'subs', 'grids',
         'riv_parm', 'baseflow',
         'time_step',
-        'pp_included'
+        'pp_included',
         ]
     col02 = [
         wd, sim_start, warmup, cal_start, cal_end, 
         subs, grids,
         riv_parm, baseflow,
         time_step,
-        pp_included
+        pp_included,
         ]
     df = pd.DataFrame({'names': col01, 'vals': col02})
     with open(os.path.join(wd, 'swatmf.con'), 'w', newline='') as f:
         f.write("# swatmf.con created by swatmf\n")
         df.to_csv(
             f, sep='\t',
             encoding='utf-8', 
             index=False, header=False)
     return df
 
 def init_setup(wd, swatwd):
     filesToCopy = [
         "Absolute_SWAT_Values.txt",
-        "beopest64.exe",
-        "i64pest.exe",
         "i64pwtadj1.exe",
+        "pestpp-glm.exe",
+        "pestpp-ies.exe",
+        "pestpp-opt.exe",
+        "pestpp-sen.exe",
         "model.in",
         "SUFI2_LH_sample.exe",
         "Swat_Edit.exe",
         ]
-    
     suffix = ' passed'
     print(" Creating 'backup' folder ...",  end='\r', flush=True)
     if not os.path.isdir(os.path.join(wd, 'backup')):
         os.makedirs(os.path.join(wd, 'backup'))
-        filelist =  os.listdir(swatwd)
+        filelist = [f for f in os.listdir(swatwd) if os.path.isfile(os.path.join(swatwd, f))]
+        
+        # filelist =  os.listdir(swatwd)
         for i in tqdm(filelist):
+            # print(i)
+            # if os.path.getsize(os.path.join(swatwd, i)) != 0:
             shutil.copy2(os.path.join(swatwd, i), os.path.join(wd, 'backup'))
     print(" Creating 'backup' folder ..." + colored(suffix, 'green'))
     print(" Creating 'echo' folder ...",  end='\r', flush=True)
     if not os.path.isdir(os.path.join(wd, 'echo')):
         os.makedirs(os.path.join(wd, 'echo'))
     print(" Creating 'echo' folder ..." + colored(suffix, 'green'))
     print(" Creating 'sufi2.in' folder ...",  end='\r', flush=True)
@@ -244,15 +253,15 @@
             writer.writerow([(item[0]),
                 '{:.4f}'.format(float(item[1]))
                 ])
     print('Finished ...\n')
 
 
 def extract_depth_to_water(grid_ids, start_day, end_day):
-    """extract a simulated streamflow from the output.rch file,
+    """extract a simulated depth to water using modflow.obs and swatmf_out_MF_obs,
         store it in each channel file.
 
     Args:
         - rch_file (`str`): the path and name of the existing output file
         - channels (`list`): channel number in a list, e.g. [9, 60]
         - start_day ('str'): simulation start day after warmup period, e.g. '1/1/1985'
         - end_day ('str'): simulation end day e.g. '12/31/2000'
@@ -275,15 +284,15 @@
 
     # set index by modflow grid ids
     mf_obs_grid_ids = mf_obs_grid_ids.set_index([3])
 
     mf_sim = pd.read_csv(
                         'swatmf_out_MF_obs', skiprows=1, sep=r'\s+',
                         names=col_names,
-                        usecols=grid_ids,
+                        # usecols=grid_ids,
                         )
     mf_sim.index = pd.date_range(start_day, periods=len(mf_sim))
     mf_sim = mf_sim[start_day:end_day]
     for i in grid_ids:
         elev = mf_obs_grid_ids.loc[i].values  # use land surface elevation to get depth to water
         (mf_sim.loc[:, i] - elev).to_csv(
                         'dtw_{}.txt'.format(i), sep='\t', encoding='utf-8',
@@ -305,17 +314,17 @@
         - time_step (`str`): day, month, year
 
     Example:
         pest_utils.extract_month_stf('path', [9, 60], '1/1/1993', '12/31/2000')
     """ 
     if time_step is None:
         time_step = 'day'
-        stfobd_file = 'stf_day.obd'
+        stfobd_file = 'swat_rch_day.obd'
     if time_step == 'month':
-        stfobd_file = 'stf_mon.obd'
+        stfobd_file = 'swat_rch_mon.obd'
 
 
     stf_obd = pd.read_csv(
                         stfobd_file,
                         sep='\t',
                         usecols=['date', col_name],
                         index_col=0,
@@ -353,30 +362,31 @@
     with open(srch_file+'.ins', "w", newline='') as f:
         f.write("pif ~" + "\n")
         result['{}_ins'.format(col_name)].to_csv(f, sep='\t', encoding='utf-8', index=False, header=False)
     print('{}.ins file has been created...'.format(srch_file))
     return result['{}_ins'.format(col_name)]
 
 
-def mf_obd_to_ins(wt_file, col_name, cal_start, cal_end):
+def mf_obd_to_ins(wt_file, col_name, cal_start, cal_end, mf_obd_file=None):
     """extract a simulated streamflow from the output.rch file,
         store it in each channel file.
 
     Args:
         - rch_file (`str`): the path and name of the existing output file
         - channels (`list`): channel number in a list, e.g. [9, 60]
         - start_day ('str'): simulation start day after warmup period, e.g. '1/1/1993'
         - end_day ('str'): simulation end day e.g. '12/31/2000'
 
     Example:
         pest_utils.extract_month_str('path', [9, 60], '1/1/1993', '12/31/2000')
     """ 
-
+    if mf_obd_file is None:
+        mf_obd_file = "modflow_day.obd"
     mf_obd = pd.read_csv(
-                        'modflow.obd',
+                        mf_obd_file,
                         sep='\t',
                         usecols=['date', col_name],
                         index_col=0,
                         na_values=[-999, ""],
                         parse_dates=True,
                         )
     mf_obd = mf_obd[cal_start:cal_end]
```

### Comparing `swatmf-0.2.4/swatmf/swatmf_scenario_utils.py` & `swatmf-0.3.0/swatmf/swatmf_scenario_utils.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/swatmf_viz.py` & `swatmf-0.3.0/swatmf/swatmf_viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 from hydroeval import evaluator, nse, rmse, pbias
 import numpy as np
+import math
 
 
 def get_all_scenario_lists(wd):
     os.chdir(wd)
     scn_nams = [name for name in os.listdir(".") if os.path.isdir(name)]
     full_paths = [os.path.abspath(name) for name in os.listdir(".") if os.path.isdir(name)]
     return scn_nams, full_paths    
 
 
 def all_strs(wd, sub_number, start_date, obd_nam, time_step=None):
     scn_nams, full_paths = get_all_scenario_lists(wd)
     if time_step is None:
         time_step = "D"
-        strobd_file = "streamflow.obd"
+        strobd_file = "swat_rch_day.obd"
     else:
         time_step = "M"
-        strobd_file = "streamflow_month.obd"
+        strobd_file = "swat_rch_mon.obd"
     tot_df = pd.DataFrame()
     for scn_nam, p in zip(scn_nams, full_paths):
         os.chdir(p)
         print("Folder changed to {}".format(p))
         df = pd.read_csv(
                     os.path.join("output.rch"),
                     delim_whitespace=True,
@@ -50,18 +51,18 @@
     return tot_df
 
 
 def all_seds(wd, sub_number, start_date, obd_nam, time_step=None):
     scn_nams, full_paths = get_all_scenario_lists(wd)
     if time_step is None:
         time_step = "D"
-        strobd_file = "streamflow.obd"
+        strobd_file = "swat_rch_day.obd"
     else:
         time_step = "M"
-        strobd_file = "streamflow_month.obd"
+        strobd_file = "swat_rch_mon.obd"
     tot_df = pd.DataFrame()
     for scn_nam, p in zip(scn_nams, full_paths):
         os.chdir(p)
         print("Folder changed to {}".format(p))
         df = pd.read_csv(
                     os.path.join("output.rch"),
                     delim_whitespace=True,
@@ -82,18 +83,18 @@
     print('Finished!')
     return tot_df
 
 
 def str_df(start_date, sub_number, time_step=None):
     if time_step is None:
         time_step = "D"
-        strobd_file = "streamflow.obd"
+        strobd_file = "swat_rch_day.obd"
     else:
         time_step = "M"
-        strobd_file = "streamflow_month.obd."
+        strobd_file = "swat_rch_mon.obd."
     df = pd.read_csv(
                 os.path.join("output.rch"),
                 delim_whitespace=True,
                 skiprows=9,
                 usecols=[1, 3, 6],
                 names=["date", "filter", "str_sim"],
                 index_col=0)
@@ -107,18 +108,18 @@
 
 
 
 def apex_str_df(rch_file, start_date, rch_num, obd_nam, time_step=None):
     
     if time_step is None:
         time_step = "D"
-        strobd_file = "streamflow.obd"
+        strobd_file = "swat_rch_day.obd"
     else:
         time_step = "M"
-        strobd_file = "streamflow_month.obd."
+        strobd_file = "swat_rch_mon.obd."
     output_rch = pd.read_csv(
                         rch_file, delim_whitespace=True, skiprows=9,
                         usecols=[0, 1, 8], names=["idx", "sub", "simulated"], index_col=0
                         )
     df = output_rch.loc["REACH"]
     str_obd = pd.read_csv(
                         strobd_file, sep=r'\s+', index_col=0, header=0,
@@ -342,31 +343,31 @@
                         na_values=[-999, ""]
                         )
     wt_obd = pd.read_csv(
                         'MODFLOW/' + wt_obd_file, sep=r'\s+', index_col=0, header=0,
                         parse_dates=True, delimiter="\t",
                         na_values=[-999, ""]
                         )
-    if strobd_file == 'streamflow_month.obd':
+    if strobd_file == 'swat_rch_mon.obd':
         str_obd = str_obd.resample('M').mean()
-    if wt_obd_file == 'modflow_month.obd':
+    if wt_obd_file == 'modflow_mon.obd':
         wt_obd = wt_obd.resample('M').mean()
 
     df = pd.concat([str_obd, wt_obd], axis=1)
     return df
     
 
 def wt_df(start_date, grid_id, obd_nam, time_step=None, prep_sub=None):
     
     if time_step is None:
         time_step = "D"
-        mfobd_file = "modflow.obd"
+        mfobd_file = "modflow_day.obd"
     else:
         time_step = "M"
-        mfobd_file = "modflow_month.obd."
+        mfobd_file = "modflow_mon.obd."
 
     mf_obs = pd.read_csv(
                         "MODFLOW/modflow.obs",
                         delim_whitespace=True,
                         skiprows = 2,
                         usecols = [3, 4],
                         index_col = 0,
@@ -484,18 +485,18 @@
         time_step (str, optional): simulation time step (day, month, annual). Defaults to None.
 
     Returns:
         dataframe: dataframe for all simulated depth to water and observed data
     """
     if time_step is None:
         time_step = "D"
-        mfobd_file = "modflow.obd"
+        mfobd_file = "modflow_day.obd"
     else:
         time_step = "M"
-        mfobd_file = "modflow_month.obd."
+        mfobd_file = "modflow_mon.obd."
     # read obs and obd files to get grid ids, elev, and observed values
     mf_obs = pd.read_csv(
                         "MODFLOW/modflow.obs",
                         delim_whitespace=True,
                         skiprows = 2,
                         usecols = [3, 4],
                         index_col = 0,
@@ -691,7 +692,87 @@
             if line.strip().startswith("Starting phi for this iteration"):
                 phis.append(float(line.replace('\n', '').split()[6]))
     
     df = pd.DataFrame({'Model Runs': model_calls, 'Phi': phis})
     df = df.set_index('Model Runs')
     df.plot(figsize=(5,5), grid=True)
 
+def plot_tseries_ensembles(
+                    pst, pr_oe, pt_oe, width=10, height=4, dot=True,
+#                     onames=["hds","sfr"]
+                    ):
+    # pst.try_parse_name_metadata()
+    # get the observation data from the control file and select 
+    obs = pst.observation_data.copy()
+    obs = obs.loc[obs.obgnme.apply(lambda x: x in pst.nnz_obs_groups),:]
+    time_col = []
+    for i in range(len(obs)):
+        time_col.append(obs.iloc[i, 0][-6:])
+    obs['time'] = time_col
+#     # onames provided in oname argument
+#     obs = obs.loc[obs.oname.apply(lambda x: x in onames)]
+    # only non-zero observations
+#     obs = obs.loc[obs.obgnme.apply(lambda x: x in pst.nnz_obs_groups),:]
+    # make a plot
+    ogs = obs.obgnme.unique()
+    fig,axes = plt.subplots(len(ogs),1,figsize=(width,height*len(ogs)))
+    ogs.sort()
+    # for each observation group (i.e. timeseries)
+    for ax,og in zip(axes,ogs):
+        # get values for x axis
+        oobs = obs.loc[obs.obgnme==og,:].copy()
+        oobs.loc[:,"time"] = oobs.loc[:,"time"].astype(str)
+#         oobs.sort_values(by="time",inplace=True)
+        tvals = oobs.time.values
+        onames = oobs.obsnme.values
+        if dot is True:
+            # plot prior
+            [ax.scatter(tvals,pr_oe.loc[i,onames].values,color="gray",s=30, alpha=0.5) for i in pr_oe.index]
+            # plot posterior
+            [ax.scatter(tvals,pt_oe.loc[i,onames].values,color='b',s=30,alpha=0.2) for i in pt_oe.index]
+            # plot measured+noise 
+            oobs = oobs.loc[oobs.weight>0,:]
+            tvals = oobs.time.values
+            onames = oobs.obsnme.values
+            ax.scatter(oobs.time,oobs.obsval,color='red',s=30).set_facecolor("none")
+        if dot is False:
+            # plot prior
+            [ax.plot(tvals,pr_oe.loc[i,onames].values,"0.5",lw=0.5,alpha=0.5) for i in pr_oe.index]
+            # plot posterior
+            [ax.plot(tvals,pt_oe.loc[i,onames].values,"b",lw=0.5,alpha=0.5) for i in pt_oe.index]
+            # plot measured+noise 
+            oobs = oobs.loc[oobs.weight>0,:]
+            tvals = oobs.time.values
+            onames = oobs.obsnme.values
+            ax.plot(oobs.time,oobs.obsval,"r-",lw=2)
+        ax.tick_params(axis='x', labelrotation=90)
+        ax.margins(x=0.01)
+        ax.set_title(og,loc="left")
+    # fig.tight_layout()
+    plt.show()
+
+
+def plot_prior_posterior_par_hist(prior_df, post_df, sel_pars, width=7, height=5, ncols=3):
+    nrows = math.ceil(len(sel_pars)/ncols)
+    fig, axes = plt.subplots(figsize=(width, height), nrows=nrows, ncols=ncols)
+    ax1 = fig.add_subplot(111, frameon=False)
+    ax1 = plt.tick_params(labelcolor='none', top=False, bottom=False, left=False, right=False)
+    for i, ax in enumerate(axes.flat):
+        if i<len(sel_pars):
+            colnam = sel_pars['parnme'].tolist()[i]
+            ax.hist(prior_df.loc[:, colnam].values,
+                    bins=np.linspace(
+                        sel_pars.loc[sel_pars["parnme"]==colnam, 'parlbnd'].values[0], 
+                        sel_pars.loc[sel_pars["parnme"]==colnam, 'parubnd'].values[0], 20),
+                    color = "gray", alpha=0.5, density=True,
+                    label="Prior"
+            )
+            y, x, _ = ax.hist(post_df.loc[:, colnam].values,
+                    bins=np.linspace(
+                        sel_pars.loc[sel_pars["parnme"]==colnam, 'parlbnd'].values[0], 
+                        sel_pars.loc[sel_pars["parnme"]==colnam, 'parubnd'].values[0], 20), 
+                     alpha=0.5, density=True, label="Posterior"
+            )
+            ax.set_ylabel(colnam)
+            ax.set_yticks([])
+    plt.xlabel("Parameter range")
+    plt.show()
```

### Comparing `swatmf-0.2.4/swatmf/utils/swat_utils.py` & `swatmf-0.3.0/swatmf/utils/swat_utils.py`

 * *Files identical despite different names*

### Comparing `swatmf-0.2.4/swatmf/utils.py` & `swatmf-0.3.0/swatmf/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,18 +72,18 @@
     return scn_nams, full_paths    
 
 
 def all_strs(wd, sub_number, start_date, obd_nam, time_step=None):
     scn_nams, full_paths = get_all_scenario_lists(wd)
     if time_step is None:
         time_step = "D"
-        strobd_file = "streamflow.obd"
+        strobd_file = "swat_rch_day.obd"
     else:
         time_step = "M"
-        strobd_file = "streamflow_month.obd"
+        strobd_file = "swat_rch_mon.obd"
     tot_df = pd.DataFrame()
     for scn_nam, p in zip(scn_nams, full_paths):
         os.chdir(p)
         print("Folder changed to {}".format(p))
         df = pd.read_csv(
                     os.path.join("output.rch"),
                     delim_whitespace=True,
@@ -105,18 +105,18 @@
     return tot_df
 
 
 def all_seds(wd, sub_number, start_date, obd_nam, time_step=None):
     scn_nams, full_paths = get_all_scenario_lists(wd)
     if time_step is None:
         time_step = "D"
-        strobd_file = "streamflow.obd"
+        strobd_file = "swat_rch_day.obd"
     else:
         time_step = "M"
-        strobd_file = "streamflow_month.obd"
+        strobd_file = "swat_rch_mon.obd"
     tot_df = pd.DataFrame()
     for scn_nam, p in zip(scn_nams, full_paths):
         os.chdir(p)
         print("Folder changed to {}".format(p))
         df = pd.read_csv(
                     os.path.join("output.rch"),
                     delim_whitespace=True,
@@ -138,18 +138,18 @@
     return tot_df
 
 
 def str_df(rch_file, start_date, rch_num, obd_nam, time_step=None):
     
     if time_step is None:
         time_step = "D"
-        strobd_file = "streamflow.obd"
+        strobd_file = "swat_rch_day.obd"
     else:
         time_step = "M"
-        strobd_file = "streamflow_month.obd."
+        strobd_file = "swat_rch_mon.obd."
     output_rch = pd.read_csv(
                         rch_file, delim_whitespace=True, skiprows=9,
                         usecols=[0, 1, 8], names=["idx", "sub", "simulated"], index_col=0
                         )
     df = output_rch.loc["REACH"]
     str_obd = pd.read_csv(
                         strobd_file, sep=r'\s+', index_col=0, header=0,
@@ -202,31 +202,31 @@
                         na_values=[-999, ""]
                         )
     wt_obd = pd.read_csv(
                         'MODFLOW/' + wt_obd_file, sep=r'\s+', index_col=0, header=0,
                         parse_dates=True, delimiter="\t",
                         na_values=[-999, ""]
                         )
-    if strobd_file == 'streamflow_month.obd':
+    if strobd_file == 'swat_rch_mon.obd':
         str_obd = str_obd.resample('M').mean()
-    if wt_obd_file == 'modflow_month.obd':
+    if wt_obd_file == 'modflow_mon.obd':
         wt_obd = wt_obd.resample('M').mean()
 
     df = pd.concat([str_obd, wt_obd], axis=1)
     return df
     
 
 def wt_df(start_date, grid_id, obd_nam, time_step=None, prep_sub=None):
     
     if time_step is None:
         time_step = "D"
-        mfobd_file = "modflow.obd"
+        mfobd_file = "modflow_day.obd"
     else:
         time_step = "M"
-        mfobd_file = "modflow_month.obd."
+        mfobd_file = "modflow_mon.obd."
 
     mf_obs = pd.read_csv(
                         "MODFLOW/modflow.obs",
                         delim_whitespace=True,
                         skiprows = 2,
                         usecols = [3, 4],
                         index_col = 0,
@@ -284,18 +284,18 @@
         time_step (str, optional): simulation time step (day, month, annual). Defaults to None.
 
     Returns:
         dataframe: dataframe for all simulated depth to water and observed data
     """
     if time_step is None:
         time_step = "D"
-        mfobd_file = "modflow.obd"
+        mfobd_file = "modflow_day.obd"
     else:
         time_step = "M"
-        mfobd_file = "modflow_month.obd."
+        mfobd_file = "modflow_mon.obd."
     # read obs and obd files to get grid ids, elev, and observed values
     mf_obs = pd.read_csv(
                         "MODFLOW/modflow.obs",
                         delim_whitespace=True,
                         skiprows = 2,
                         usecols = [3, 4],
                         index_col = 0,
```

### Comparing `swatmf-0.2.4/swatmf.egg-info/SOURCES.txt` & `swatmf-0.3.0/swatmf.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,13 +22,16 @@
 swatmf.egg-info/top_level.txt
 swatmf/hg/__init__.py
 swatmf/hg/hg_handler.py
 swatmf/hg/viz.py
 swatmf/opt_files/Absolute_SWAT_Values.txt
 swatmf/opt_files/SUFI2_LH_sample.exe
 swatmf/opt_files/Swat_Edit.exe
-swatmf/opt_files/beopest64.exe
-swatmf/opt_files/i64pest.exe
 swatmf/opt_files/i64pwtadj1.exe
 swatmf/opt_files/model.in
+swatmf/opt_files/pestpp-glm.exe
+swatmf/opt_files/pestpp-ies.exe
+swatmf/opt_files/pestpp-opt.exe
+swatmf/opt_files/pestpp-sen.exe
 swatmf/utils/__init__.py
+swatmf/utils/etc.py
 swatmf/utils/swat_utils.py
```

