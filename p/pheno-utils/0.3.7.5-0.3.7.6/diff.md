# Comparing `tmp/pheno-utils-0.3.7.5.tar.gz` & `tmp/pheno-utils-0.3.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.7.5.tar", last modified: Wed Jul 26 07:09:04 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.7.6.tar", last modified: Wed Jul 26 08:40:52 2023, max compression
```

## Comparing `pheno-utils-0.3.7.5.tar` & `pheno-utils-0.3.7.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 07:09:04.493284 pheno-utils-0.3.7.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2361 2023-07-26 07:09:04.492230 pheno-utils-0.3.7.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.7.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 07:09:04.440484 pheno-utils-0.3.7.5/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      344 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18932 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16402 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)    11559 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/config.py
--rw-r--r--   0 root         (0) root         (0)     2825 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    20116 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-07-26 07:08:44.000000 pheno-utils-0.3.7.5/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 07:09:04.486333 pheno-utils-0.3.7.5/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2361 2023-07-26 07:09:04.000000 pheno-utils-0.3.7.5/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      684 2023-07-26 07:09:04.000000 pheno-utils-0.3.7.5/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 07:09:04.000000 pheno-utils-0.3.7.5/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-26 07:09:04.000000 pheno-utils-0.3.7.5/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.7.5/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-07-26 07:09:04.000000 pheno-utils-0.3.7.5/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 07:09:04.000000 pheno-utils-0.3.7.5/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      944 2023-07-26 07:08:19.000000 pheno-utils-0.3.7.5/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 07:09:04.493805 pheno-utils-0.3.7.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3840 2023-07-26 07:06:28.000000 pheno-utils-0.3.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:40:52.841837 pheno-utils-0.3.7.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-21 16:13:16.000000 pheno-utils-0.3.7.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-07-26 08:40:52.840707 pheno-utils-0.3.7.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.7.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:40:52.787822 pheno-utils-0.3.7.6/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19064 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    11559 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     4638 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20116 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-07-26 08:40:31.000000 pheno-utils-0.3.7.6/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 08:40:52.831999 pheno-utils-0.3.7.6/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      684 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 08:40:52.000000 pheno-utils-0.3.7.6/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      944 2023-07-26 08:40:26.000000 pheno-utils-0.3.7.6/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 08:40:52.842455 pheno-utils-0.3.7.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3842 2023-07-26 08:31:51.000000 pheno-utils-0.3.7.6/setup.py
```

### Comparing `pheno-utils-0.3.7.5/LICENSE` & `pheno-utils-0.3.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/PKG-INFO` & `pheno-utils-0.3.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.7.5
+Version: 0.3.7.6
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.7.5/README.md` & `pheno-utils-0.3.7.6/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils/_modidx.py` & `pheno-utils-0.3.7.6/pheno_utils/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,16 @@
                                                                                     'pheno_utils/cgm_plots.py')},
             'pheno_utils.cohort_selector': { 'pheno_utils.cohort_selector.CohortSelector': ( 'cohort_selector.html#cohortselector',
                                                                                              'pheno_utils/cohort_selector.py'),
                                              'pheno_utils.cohort_selector.CohortSelector.__init__': ( 'cohort_selector.html#cohortselector.__init__',
                                                                                                       'pheno_utils/cohort_selector.py'),
                                              'pheno_utils.cohort_selector.CohortSelector.select': ( 'cohort_selector.html#cohortselector.select',
                                                                                                     'pheno_utils/cohort_selector.py')},
-            'pheno_utils.config': { 'pheno_utils.config.generate_synthetic_data': ( 'config.html#generate_synthetic_data',
+            'pheno_utils.config': { 'pheno_utils.config.copy_tre_config': ('config.html#copy_tre_config', 'pheno_utils/config.py'),
+                                    'pheno_utils.config.generate_synthetic_data': ( 'config.html#generate_synthetic_data',
                                                                                     'pheno_utils/config.py'),
                                     'pheno_utils.config.generate_synthetic_data_like': ( 'config.html#generate_synthetic_data_like',
                                                                                          'pheno_utils/config.py')},
             'pheno_utils.dates_plots': { 'pheno_utils.dates_plots.dates_dist_plot': ( 'date_plots.html#dates_dist_plot',
                                                                                       'pheno_utils/dates_plots.py')},
             'pheno_utils.ecg_analysis': { 'pheno_utils.ecg_analysis.get_hrv_df': ( 'ecg_analysis.html#get_hrv_df',
                                                                                    'pheno_utils/ecg_analysis.py'),
```

### Comparing `pheno-utils-0.3.7.5/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.7.6/pheno_utils/age_reference_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_age_reference_plots.ipynb.
 
 # %% auto 0
 __all__ = ['get_gam_expectiles', 'AgeRefPlot', 'GenderAgeRefPlot']
 
 # %% ../nbs/03_age_reference_plots.ipynb 3
-from .config import *
+from pheno_utils.config import (
+    generate_synthetic_data, 
+    FEMALE_COLOR,
+    MALE_COLOR,
+    ALL_COLOR, 
+    REF_COLOR,
+    ERROR_ACTION, 
+    )
 
 from typing import Dict, List, Callable, Optional, Union, Tuple
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import importlib
 from scipy.stats import linregress
```

### Comparing `pheno-utils-0.3.7.5/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.7.6/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils/basic_plots.py` & `pheno-utils-0.3.7.6/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.7.6/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.7.6/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.7.6/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils/config.py` & `pheno-utils-0.3.7.6/pheno_utils/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_config.ipynb.
 
 # %% auto 0
 __all__ = ['REF_COLOR', 'FEMALE_COLOR', 'MALE_COLOR', 'ALL_COLOR', 'GLUC_COLOR', 'FOOD_COLOR', 'DATASETS_PATH', 'COHORT',
-           'EVENTS_DATASET', 'ERROR_ACTION', 'CONFIG_FILES', 'BULK_DATA_PATH', 'generate_synthetic_data',
-           'generate_synthetic_data_like']
+           'EVENTS_DATASET', 'ERROR_ACTION', 'CONFIG_FILES', 'BULK_DATA_PATH', 'config_found', 'copy_tre_config',
+           'generate_synthetic_data', 'generate_synthetic_data_like']
 
 # %% ../nbs/00_config.ipynb 3
 import os
 import json
 import numpy as np
 import pandas as pd
 
@@ -23,20 +23,47 @@
 DATASETS_PATH = '/home/ec2-user/studies/hpp/'
 COHORT = None
 EVENTS_DATASET = 'events'
 ERROR_ACTION = 'raise'
 CONFIG_FILES = ['.pheno/config.json', '~/.pheno/config.json', '/efs/.pheno/config.json']
 BULK_DATA_PATH = {}
 
+config_found = False
 
+
+
+# %% ../nbs/00_config.ipynb 5
+def copy_tre_config():
+    tre_mode = False
+    script_path = os.path.dirname(os.path.abspath(__file__))
+    absolute_config_path = os.path.join(script_path, '../config_setup/config_tre.json')
+    
+    with open(absolute_config_path, 'r') as openfile:
+        json_object = json.load(openfile)
+                
+    datasets_full_path = json_object['DATASETS_PATH']
+    if os.path.exists(datasets_full_path):
+        print("TRE Mode")
+        tre_mode = True
+        if not os.path.exists(os.path.expanduser('~/.pheno')):
+            os.makedirs(os.path.expanduser('~/.pheno'))
+        
+        shutil.copy2(absolute_config_path, os.path.expanduser('~/.pheno/config.json'))
+    
+    return tre_mode
+
+
+# %% ../nbs/00_config.ipynb 6
 for cf in CONFIG_FILES:
     cf = os.path.expanduser(cf)
     if not os.path.isfile(cf):
         continue
-
+    
+    config_found=True
+    
     f = open(cf)
     config = json.load(f)
     
     if 'DATASETS_PATH' in config:
         DATASETS_PATH = config['DATASETS_PATH']
     if 'BULK_DATA_PATH' in config:
         BULK_DATA_PATH = config['BULK_DATA_PATH']
@@ -45,16 +72,22 @@
     if 'COHORT' in config:
         if config['COHORT'] == 0 or config['COHORT']=='None' or config['COHORT']==None :
             COHORT = None
     if 'ERROR_ACTION' in config:
         ERROR_ACTION = config['ERROR_ACTION']
     break
 
+if not config_found: 
+    if not copy_tre_config():
+        raise ValueError(f'Missing Config file, please read the README file and run config_setup/create_default_config.py')
+        
+    
+    
 
-# %% ../nbs/00_config.ipynb 5
+# %% ../nbs/00_config.ipynb 7
 def generate_synthetic_data(n: int = 1000) -> pd.DataFrame:
     """
     Generates a sample DataFrame containing age, gender, and value data.
 
     Args:
         n: The number of rows in the generated DataFrame.
 
@@ -70,15 +103,15 @@
     genders = np.random.choice([0, 1], size=n)
     vals = np.random.normal(30 + 1 * ages + 40 * genders, 20, size=n)
     
     data = pd.DataFrame(data={"participant_id":pids,"date_of_research_stage": dates,"age_at_research_stage": ages, "sex": genders, "val1": vals}).set_index("participant_id")
     data["val2"] = data["val1"]*0.3 + 0.5*np.random.normal(0,50) + 0.2*10*data["sex"]
     return data
 
-# %% ../nbs/00_config.ipynb 6
+# %% ../nbs/00_config.ipynb 8
 def generate_synthetic_data_like(df: pd.DataFrame, n: int = 1000, random_seed: int = 42) -> pd.DataFrame:
     """
     Generate a sample DataFrame containing the same columns as `df`, but with random data.
 
     Args:
     
         df: The DataFrame whose columns should be used.
```

### Comparing `pheno-utils-0.3.7.5/pheno_utils/dates_plots.py` & `pheno-utils-0.3.7.6/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.7.6/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils/meta_loader.py` & `pheno-utils-0.3.7.6/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.7.6/pheno_utils/pheno_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.7.6/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.7.6/pheno_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.7.5
+Version: 0.3.7.6
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.7.5/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.7.6/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.7.5/settings.ini` & `pheno-utils-0.3.7.6/settings.ini`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pheno-utils
 lib_name = pheno-utils
-version = 0.3.7.5
+version = 0.3.7.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pheno_utils
 nbs_path = nbs
 recursive = True
```

### Comparing `pheno-utils-0.3.7.5/setup.py` & `pheno-utils-0.3.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             
         print(absolute_config_path)
         logging.info(absolute_config_path)
         
         shutil.copy2(absolute_config_path, os.path.expanduser('~/.pheno/config.json'))
 
         
-copy_tre_config()     
+# copy_tre_config()     
 
 # note: all settings are in settings.ini; edit there, not here
 config = ConfigParser(delimiters=['='])
 config.read('settings.ini')
 cfg = config['DEFAULT']
 
 cfg_keys = 'version description keywords author author_email'.split()
```

