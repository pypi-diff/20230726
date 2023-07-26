# Comparing `tmp/pycrossva-0.93.tar.gz` & `tmp/pycrossva-0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrossva-0.93.tar", last modified: Fri Oct 28 18:33:23 2022, max compression
+gzip compressed data, was "pycrossva-0.94.tar", last modified: Wed Jul 26 19:05:14 2023, max compression
```

## Comparing `pycrossva-0.93.tar` & `pycrossva-0.94.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2022-10-28 18:33:23.257059 pycrossva-0.93/
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    35147 2022-07-12 21:13:08.000000 pycrossva-0.93/LICENSE
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      158 2022-07-12 21:13:08.000000 pycrossva-0.93/MANIFEST.in
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      677 2022-10-28 18:33:23.256542 pycrossva-0.93/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     7030 2022-10-28 17:10:24.000000 pycrossva-0.93/README.rst
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2022-10-28 18:33:23.208652 pycrossva-0.93/pycrossva/
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       19 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    25626 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/configuration.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    19825 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/mappings.py
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2022-10-28 18:33:23.198299 pycrossva-0.93/pycrossva/resources/
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2022-10-28 18:33:23.227625 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    32803 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    49398 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA5.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    42538 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    39105 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA5.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    42139 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    65280 2022-10-19 17:13:10.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA5.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    34196 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2021WHO_to_InSilicoVA.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    53080 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2021WHO_to_InterVA5.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    35344 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InSilicoVA.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    47073 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InterVA5.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     2608 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/example_config_1.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      575 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/mapping_configuration_files/example_config_2.csv
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2022-10-28 18:33:23.253906 pycrossva-0.93/pycrossva/resources/sample_data/
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     5059 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/sample_data/2012WHO_mock_data_1.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   470310 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/sample_data/2016WHO_bad_data_1.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   617783 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/sample_data/2016WHO_mock_data_1.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   915332 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/sample_data/2016WHO_mock_data_2.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     6760 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/sample_data/Mock_PHRMC_Data.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     6824 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/sample_data/PHRMC_mock_data_1.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   921756 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/sample_data/mock_data_2.csv
--rwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    36142 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/sample_data/mock_data_2016WHO151.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   193579 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/sample_data/test_data1.csv
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   136542 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/resources/sample_data/test_data2.csv
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2022-10-28 18:33:23.255523 pycrossva-0.93/pycrossva/scripts/
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     5170 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/scripts/pycrossva_transform.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    14592 2022-08-19 21:02:20.000000 pycrossva-0.93/pycrossva/transform.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     6327 2022-07-12 21:13:08.000000 pycrossva-0.93/pycrossva/utils.py
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    32987 2022-10-28 18:25:08.000000 pycrossva-0.93/pycrossva/validation.py
-drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2022-10-28 18:33:23.214617 pycrossva-0.93/pycrossva.egg-info/
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      677 2022-10-28 18:33:23.000000 pycrossva-0.93/pycrossva.egg-info/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     1867 2022-10-28 18:33:23.000000 pycrossva-0.93/pycrossva.egg-info/SOURCES.txt
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        1 2022-10-28 18:33:23.000000 pycrossva-0.93/pycrossva.egg-info/dependency_links.txt
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       83 2022-10-28 18:33:23.000000 pycrossva-0.93/pycrossva.egg-info/entry_points.txt
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        1 2022-07-13 00:34:30.000000 pycrossva-0.93/pycrossva.egg-info/not-zip-safe
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       19 2022-10-28 18:33:23.000000 pycrossva-0.93/pycrossva.egg-info/requires.txt
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       10 2022-10-28 18:33:23.000000 pycrossva-0.93/pycrossva.egg-info/top_level.txt
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       38 2022-10-28 18:33:23.257238 pycrossva-0.93/setup.cfg
--rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     1237 2022-10-28 18:29:45.000000 pycrossva-0.93/setup.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:05:14.288870 pycrossva-0.94/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    35147 2022-07-12 21:13:08.000000 pycrossva-0.94/LICENSE
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      158 2022-07-12 21:13:08.000000 pycrossva-0.94/MANIFEST.in
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      677 2023-07-26 19:05:14.288221 pycrossva-0.94/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     7030 2022-10-28 17:10:24.000000 pycrossva-0.94/README.rst
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:05:14.239354 pycrossva-0.94/pycrossva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       19 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    25626 2023-07-25 14:56:32.000000 pycrossva-0.94/pycrossva/configuration.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    19825 2023-07-25 14:56:39.000000 pycrossva-0.94/pycrossva/mappings.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:05:14.231834 pycrossva-0.94/pycrossva/resources/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:05:14.255932 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    32803 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    49398 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA5.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    42538 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    39105 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA5.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    42139 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    65280 2023-07-25 17:44:02.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA5.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    34196 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2021WHO_to_InSilicoVA.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    53080 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2021WHO_to_InterVA5.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    35344 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InSilicoVA.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    47073 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InterVA5.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088     2608 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/example_config_1.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      575 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/mapping_configuration_files/example_config_2.csv
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:05:14.281772 pycrossva-0.94/pycrossva/resources/sample_data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5059 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/sample_data/2012WHO_mock_data_1.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   470310 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/sample_data/2016WHO_bad_data_1.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   617783 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/sample_data/2016WHO_mock_data_1.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   915332 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/sample_data/2016WHO_mock_data_2.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     6760 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/sample_data/Mock_PHRMC_Data.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     6824 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/sample_data/PHRMC_mock_data_1.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   921756 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/sample_data/mock_data_2.csv
+-rwxr-xr-x   0 thomas.3912 (1583608718) 444659088    36142 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/sample_data/mock_data_2016WHO151.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   193579 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/sample_data/test_data1.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   136542 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/resources/sample_data/test_data2.csv
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:05:14.284250 pycrossva-0.94/pycrossva/scripts/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5170 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/scripts/pycrossva_transform.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    15203 2023-07-26 11:20:41.000000 pycrossva-0.94/pycrossva/transform.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     6327 2022-07-12 21:13:08.000000 pycrossva-0.94/pycrossva/utils.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    33042 2023-07-25 15:33:39.000000 pycrossva-0.94/pycrossva/validation.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:05:14.243542 pycrossva-0.94/pycrossva.egg-info/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      677 2023-07-26 19:05:14.000000 pycrossva-0.94/pycrossva.egg-info/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     1881 2023-07-26 19:05:14.000000 pycrossva-0.94/pycrossva.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        1 2023-07-26 19:05:14.000000 pycrossva-0.94/pycrossva.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       83 2023-07-26 19:05:14.000000 pycrossva-0.94/pycrossva.egg-info/entry_points.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        1 2022-07-13 00:34:30.000000 pycrossva-0.94/pycrossva.egg-info/not-zip-safe
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       19 2023-07-26 19:05:14.000000 pycrossva-0.94/pycrossva.egg-info/requires.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       10 2023-07-26 19:05:14.000000 pycrossva-0.94/pycrossva.egg-info/top_level.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       38 2023-07-26 19:05:14.289202 pycrossva-0.94/setup.cfg
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     1237 2023-07-25 14:56:52.000000 pycrossva-0.94/setup.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:05:14.286472 pycrossva-0.94/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      555 2023-07-25 14:58:56.000000 pycrossva-0.94/tests/test.py
```

### Comparing `pycrossva-0.93/LICENSE` & `pycrossva-0.94/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/PKG-INFO` & `pycrossva-0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrossva
-Version: 0.93
+Version: 0.94
 Summary: prepare data from WHO and PHRMC instruments for verbal autopsy algorithms
 Home-page: https://github.com/verbal-autopsy-software/pyCrossVA
 License: GNU General Public License v3.0
 Keywords: verbal autopsy data preparation
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pycrossva-0.93/README.rst` & `pycrossva-0.94/README.rst`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/configuration.py` & `pycrossva-0.94/pycrossva/configuration.py`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/mappings.py` & `pycrossva-0.94/pycrossva/mappings.py`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2012WHO_to_InSilicoVA.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA5.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2012WHO_to_InterVA5.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InSilicoVA.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA5.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2016WHOv141_to_InterVA5.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InSilicoVA.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA5.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2016WHOv151_to_InterVA5.csv`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 i022d, Was s(he) aged 5-14 years at death? 5-14 (adult or child),ageInYears,Calculated field: int(${ageInDays} div 365.25),between,5 to 14,,
 i022d, Was s(he) aged 5-14 years at death? 5-14 (adult or child),age_adult,Calculated field: int(${ageInDays} div 365.25),between,5 to 14,,
 i022e, Was s(he) aged 1 to 4 years at death? 1 to 4 (child),age_child_months,[Enter child's age in months:],between,12 to 48,,
 i022e, Was s(he) aged 1 to 4 years at death? 1 to 4 (child),age_child_years,[Enter child's age in years:],between,1 to 4,,
 i022e, Was s(he) aged 1 to 4 years at death? 1 to 4 (child),ageInYears,Calculated field: int(${ageInDays} div 365.25),between,1 to 4,,
 i022f, Was s(he) aged 1 to 11 months at death? 1-11 months (child or neonate?),age_child_years,[Enter child's age in months:],lt,1,,
 i022f, Was s(he) aged 1 to 11 months at death? 1-11 months (child or neonate?),age_child_months,[Enter child's age in months:],between,1 to 11,,
-i022f, Was s(he) aged 1 to 11 months at death? 1-11 months (child or neonate?),age_child_days,[Enter child's age in days:],between,28 to 364,,
-i022f, Was s(he) aged 1 to 11 months at death? 1-11 months (child or neonate?),ageInDays,Calculated field: int(${ageInYearsRemain} div 30.4),between,28 to 364,,
+i022f, Was s(he) aged 1 to 11 months at death? 1-11 months (child or neonate?),age_child_days,[Enter child's age in days:],between,28 to 365,,
+i022f, Was s(he) aged 1 to 11 months at death? 1-11 months (child or neonate?),ageInDays,Calculated field: int(${ageInYearsRemain} div 30.4),between,28 to 365,,
 i022g, Was s(he) aged < 1 month (28 days) at death? 0 - 27 days (neonate),ageInDays,"(${Id10023} - ${Id10021})",lt,28,,
 i022g, Was s(he) aged < 1 month (28 days) at death? 0 - 27 days (neonate),ageInDaysNeonate,"Calculated field: if(${ageInDays} = 'NaN' or string-length(${ageInDays}) = 0, ${age_neonate_days}, ${ageInDays})",lt,28,,
 i022h, Was s(he) a live baby who died within 24 hours of birth? day0 iv5Names[12],ageInDays,"(${Id10023} - ${Id10021})",lt,1,,
 i022h, Was s(he) a live baby who died within 24 hours of birth? day0 iv5Names[12],ageInDaysNeonate,"Calculated field: if(${ageInDays} = 'NaN' or string-length(${ageInDays}) = 0, ${age_neonate_days}, ${ageInDays})",lt,1,,
 i022i, Was s(he) a baby who died between 24 and 48 hours of birth? day1 iv5Names[13],ageInDays,"(${Id10023} - ${Id10021})",eq,1,,
 i022i, Was s(he) a baby who died between 24 and 48 hours of birth? day1 iv5Names[13],ageInDaysNeonate,"Calculated field: if(${ageInDays} = 'NaN' or string-length(${ageInDays}) = 0, ${age_neonate_days}, ${ageInDays})",eq,1,,
 i022j," Was s(he) a baby who died more than 48 hours from birth, but within the first week? day2-6 iv5Names[14]",ageInDays,"(${Id10023} - ${Id10021})",between,2 to 6,,
```

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2021WHO_to_InSilicoVA.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2021WHO_to_InSilicoVA.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/2021WHO_to_InterVA5.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/2021WHO_to_InterVA5.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InSilicoVA.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InSilicoVA.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InterVA5.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/PHRMCShort_to_InterVA5.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/example_config_1.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/example_config_1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/mapping_configuration_files/example_config_2.csv` & `pycrossva-0.94/pycrossva/resources/mapping_configuration_files/example_config_2.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/sample_data/2012WHO_mock_data_1.csv` & `pycrossva-0.94/pycrossva/resources/sample_data/2012WHO_mock_data_1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/sample_data/2016WHO_bad_data_1.csv` & `pycrossva-0.94/pycrossva/resources/sample_data/2016WHO_bad_data_1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/sample_data/2016WHO_mock_data_1.csv` & `pycrossva-0.94/pycrossva/resources/sample_data/2016WHO_mock_data_1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/sample_data/2016WHO_mock_data_2.csv` & `pycrossva-0.94/pycrossva/resources/sample_data/2016WHO_mock_data_2.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/sample_data/Mock_PHRMC_Data.csv` & `pycrossva-0.94/pycrossva/resources/sample_data/Mock_PHRMC_Data.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/sample_data/PHRMC_mock_data_1.csv` & `pycrossva-0.94/pycrossva/resources/sample_data/PHRMC_mock_data_1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/sample_data/mock_data_2.csv` & `pycrossva-0.94/pycrossva/resources/sample_data/mock_data_2.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/sample_data/mock_data_2016WHO151.csv` & `pycrossva-0.94/pycrossva/resources/sample_data/mock_data_2016WHO151.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/sample_data/test_data1.csv` & `pycrossva-0.94/pycrossva/resources/sample_data/test_data1.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/resources/sample_data/test_data2.csv` & `pycrossva-0.94/pycrossva/resources/sample_data/test_data2.csv`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/scripts/pycrossva_transform.py` & `pycrossva-0.94/pycrossva/scripts/pycrossva_transform.py`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/transform.py` & `pycrossva-0.94/pycrossva/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,29 @@
 from pycrossva.utils import flexible_read
 
 SUPPORTED_INPUTS = ["2016WHOv151", "2016WHOv141", "2012WHO",
                     "2021WHO", "PHRMCShort"]
 SUPPORTED_OUTPUTS = ["InterVA5", "InterVA4", "InSilicoVA"]
 
 
-def transform(mapping, raw_data, raw_data_id=None, verbose=2, preserve_na=True,
+def transform(mapping, raw_data, raw_data_id=None, lower=False,
+              verbose=2, preserve_na=True,
               result_values={"Present": "y", "Absent": "n", "NA": "."}):
     """transforms raw VA data (`raw_data`) into data suitable for use with a VA
     algorithm, according to the specified transformations given in `mapping`.
 
     Args:
         mapping (string, tuple or Pandas DataFrame): Should be either a tuple
             in form (input, output), a path to csv containing a configuration
             data file, or a Pandas DataFrame containing configuration data
         raw_data (string or Pandas DataFrame): raw verbal autopsy data to
             process
         raw_data_id (string): column name with record ID
+        lower (bool): whether the column names in the data should be
+            case-sensitive.
         verbose (int): integer from 0 to 5, controlling how much status detail
             is printed to console. Silent if 0. Defaults to 2, which will print
             only errors and warnings.
         preserve_na (bool): whether to preserve NAs in data, or to count them
             as FALSE. Overridden with True for InSilicoVA, False for InterVA4
             when mapping is given as a tuple. Defaults to TRUE, which allows
             NA values to perpetuate through the data.
@@ -230,24 +233,30 @@
                           " either a tuple in form (input, output), a path to csv"
                           " or a Pandas DataFrame."))
 
     # init configuration obj from given mapping data
     config = Configuration(config_data=mapping_data,
                            verbose=verbose,
                            process_strings=False)
+    if lower:
+        config.config_data["Source Column ID"] = config.config_data[
+            "Source Column ID"].str.lower()
+        config.source_columns = config.source_columns.str.lower()
 
     # if the configuration isn't valid, or if the data isn't valid for the
     # config file, then raise error
     if not config.validate(verbose=verbose):
         # Raise Error
         raise ValueError(("Configuration from mapping file must be valid "
                           "before transform."))
 
     # TODO adds args to init based on data type?
-    input_data = flexible_read(raw_data)
+    input_data = flexible_read(raw_data).copy()
+    if lower:
+        input_data.columns = input_data.columns.str.lower()
     cross_va = CrossVA(input_data, config)
     if not cross_va.validate(verbose=verbose):
         return
 #        raise ValueError(("Cannot transform if provided raw data is not valid "
 #                          "for configuration file."))
     final_data = cross_va.process()
     # if result values have been changed, then map as directed, otherwise
@@ -257,17 +266,22 @@
     defaults = {"Present": 1, "Absent": 0, "NA": np.nan}
     if result_values != defaults:
         actual_mapping = {value: result_values[key] for key,
                           value in defaults.items()}
         final_data = final_data.replace(actual_mapping)
     if raw_data_id is not None:
         try:
-            final_data.insert(loc=0,
-                              column="ID",
-                              value=input_data[raw_data_id])
+            if lower:
+                final_data.insert(loc=0,
+                                  column="ID",
+                                  value=input_data[raw_data_id.lower()])
+            else:
+                final_data.insert(loc=0,
+                                  column="ID",
+                                  value=input_data[raw_data_id])
         except KeyError:
             raise ValueError((f"Could not find column named {raw_data_id} "
                               "in raw_data."))
     else:
         final_data.reset_index(inplace=True)
         final_data.rename(columns={"index": "ID"}, inplace=True)
         final_data["ID"] = final_data["ID"] + 1
```

### Comparing `pycrossva-0.93/pycrossva/utils.py` & `pycrossva-0.94/pycrossva/utils.py`

 * *Files identical despite different names*

### Comparing `pycrossva-0.93/pycrossva/validation.py` & `pycrossva-0.94/pycrossva/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -826,15 +826,16 @@
 
     Examples:
         >>> report_row(pd.Series([True, True, False, True, False]))
         '#0, #1, and #3'
 
     """
     flagged = flag_where[flag_where.fillna(False)]
-    if flagged.index.is_numeric():
+    # if flagged.index.is_numeric():
+    if pd.api.types.is_numeric_dtype(flagged.index):
         unformatted_report = report_list(flagged.index.tolist(), paren=False)
         return re.sub(r"'(\d+)'", r"#\1", unformatted_report)
     return report_list(flagged.index.tolist(), paren=False)
 
 
 if __name__ == "__main__":
     import doctest
```

### Comparing `pycrossva-0.93/pycrossva.egg-info/PKG-INFO` & `pycrossva-0.94/pycrossva.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrossva
-Version: 0.93
+Version: 0.94
 Summary: prepare data from WHO and PHRMC instruments for verbal autopsy algorithms
 Home-page: https://github.com/verbal-autopsy-software/pyCrossVA
 License: GNU General Public License v3.0
 Keywords: verbal autopsy data preparation
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pycrossva-0.93/pycrossva.egg-info/SOURCES.txt` & `pycrossva-0.94/pycrossva.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,8 +33,9 @@
 pycrossva/resources/sample_data/2016WHO_mock_data_2.csv
 pycrossva/resources/sample_data/Mock_PHRMC_Data.csv
 pycrossva/resources/sample_data/PHRMC_mock_data_1.csv
 pycrossva/resources/sample_data/mock_data_2.csv
 pycrossva/resources/sample_data/mock_data_2016WHO151.csv
 pycrossva/resources/sample_data/test_data1.csv
 pycrossva/resources/sample_data/test_data2.csv
-pycrossva/scripts/pycrossva_transform.py
+pycrossva/scripts/pycrossva_transform.py
+tests/test.py
```

### Comparing `pycrossva-0.93/setup.py` & `pycrossva-0.94/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup(name='pycrossva',
-      version='0.93',
+      version='0.94',
       description='prepare data from WHO and PHRMC instruments for verbal autopsy algorithms',
       url='https://github.com/verbal-autopsy-software/pyCrossVA',
       license='GNU General Public License v3.0',
       packages=find_packages(),
       entry_points='''
                     [console_scripts]
                     pycrossva-transform=pycrossva.scripts.pycrossva_transform:main
```

