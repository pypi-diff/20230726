# Comparing `tmp/talan-0.1.4.4.tar.gz` & `tmp/talan-0.1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talan-0.1.4.4.tar", last modified: Tue Jul 18 19:12:46 2023, max compression
+gzip compressed data, was "talan-0.1.4.5.tar", last modified: Wed Jul 26 21:09:11 2023, max compression
```

## Comparing `talan-0.1.4.4.tar` & `talan-0.1.4.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2023-07-18 19:12:46.446617 talan-0.1.4.4/
--rw-r--r--   0 rstudio   (1001) users      (100)      688 2023-07-18 19:12:46.446617 talan-0.1.4.4/PKG-INFO
--rw-r--r--   0 rstudio   (1001) users      (100)      314 2021-10-14 21:05:42.000000 talan-0.1.4.4/README.md
--rw-r--r--   0 rstudio   (1001) users      (100)       38 2023-07-18 19:12:46.446617 talan-0.1.4.4/setup.cfg
--rw-r--r--   0 rstudio   (1001) users      (100)      975 2023-07-18 19:12:39.000000 talan-0.1.4.4/setup.py
-drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2023-07-18 19:12:46.446617 talan-0.1.4.4/talan/
--rwxr-xr-x   0 rstudio   (1001) users      (100)      240 2023-07-05 19:22:10.000000 talan-0.1.4.4/talan/__init__.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    39966 2023-07-04 04:09:16.000000 talan-0.1.4.4/talan/_alan_calc.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    13742 2023-07-03 20:21:58.000000 talan-0.1.4.4/talan/_alan_date.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    14990 2022-05-09 20:38:57.000000 talan-0.1.4.4/talan/_alan_mp4.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    11723 2022-11-22 22:19:42.000000 talan-0.1.4.4/talan/_alan_ohlc_fcs.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     4265 2019-08-01 04:14:12.000000 talan-0.1.4.4/talan/_alan_optparse.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    14976 2021-10-29 01:15:39.000000 talan-0.1.4.4/talan/_alan_pppscf.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    29498 2023-01-23 14:30:39.000000 talan-0.1.4.4/talan/_alan_rmc.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    65801 2023-07-04 02:53:11.000000 talan-0.1.4.4/talan/_alan_str.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    47116 2023-02-09 16:29:37.000000 talan-0.1.4.4/talan/alanapi.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     7501 2023-02-16 02:31:23.000000 talan-0.1.4.4/talan/chatgptAPI.py
--rw-r--r--   0 rstudio   (1001) users      (100)    31949 2022-12-30 20:32:22.000000 talan-0.1.4.4/talan/csv2plotj2ts.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     7100 2021-09-19 20:39:01.000000 talan-0.1.4.4/talan/find_recent_eps.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     3518 2022-10-12 19:28:21.000000 talan-0.1.4.4/talan/fredReader.py
--rw-r--r--   0 rstudio   (1001) users      (100)     2185 2023-07-18 18:27:13.000000 talan-0.1.4.4/talan/get_rq.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     6262 2023-01-31 19:25:24.000000 talan-0.1.4.4/talan/headline_calc.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     9876 2020-05-08 19:29:00.000000 talan-0.1.4.4/talan/headline_sts.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     6261 2020-05-19 00:26:02.000000 talan-0.1.4.4/talan/iex_peers.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    34234 2022-03-30 17:55:59.000000 talan-0.1.4.4/talan/lsi_daily.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     9822 2021-09-29 19:06:55.000000 talan-0.1.4.4/talan/macro_event_yh.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    41692 2022-12-23 21:01:13.000000 talan-0.1.4.4/talan/plot_templates.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     7703 2023-07-04 20:28:27.000000 talan-0.1.4.4/talan/prc_temp_DN.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    11503 2023-01-31 19:15:38.000000 talan-0.1.4.4/talan/record_hilo.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     1027 2023-07-18 15:56:52.000000 talan-0.1.4.4/talan/talan_wrap.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    14131 2023-01-06 22:09:49.000000 talan-0.1.4.4/talan/theme_list.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     6113 2023-02-02 21:45:43.000000 talan-0.1.4.4/talan/ticker2label.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     6613 2022-11-07 00:19:24.000000 talan-0.1.4.4/talan/ticker_mapping.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     4825 2021-10-11 19:44:03.000000 talan-0.1.4.4/talan/upd_mapping_ticker.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     8716 2023-07-05 03:31:50.000000 talan-0.1.4.4/talan/webReader.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    42404 2023-07-04 04:49:24.000000 talan-0.1.4.4/talan/yh_chart.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)    15454 2022-11-14 21:58:33.000000 talan-0.1.4.4/talan/yh_hist_batch.py
--rwxr-xr-x   0 rstudio   (1001) users      (100)     5521 2023-01-31 21:38:37.000000 talan-0.1.4.4/talan/yh_predefined.py
-drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2023-07-18 19:12:46.446617 talan-0.1.4.4/talan.egg-info/
--rw-r--r--   0 rstudio   (1001) users      (100)      688 2023-07-18 19:12:46.000000 talan-0.1.4.4/talan.egg-info/PKG-INFO
--rw-r--r--   0 rstudio   (1001) users      (100)      837 2023-07-18 19:12:46.000000 talan-0.1.4.4/talan.egg-info/SOURCES.txt
--rw-r--r--   0 rstudio   (1001) users      (100)        1 2023-07-18 19:12:46.000000 talan-0.1.4.4/talan.egg-info/dependency_links.txt
--rw-r--r--   0 rstudio   (1001) users      (100)       38 2023-07-18 19:12:46.000000 talan-0.1.4.4/talan.egg-info/requires.txt
--rw-r--r--   0 rstudio   (1001) users      (100)        6 2023-07-18 19:12:46.000000 talan-0.1.4.4/talan.egg-info/top_level.txt
+drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2023-07-26 21:09:11.212836 talan-0.1.4.5/
+-rw-r--r--   0 rstudio   (1001) users      (100)      688 2023-07-26 21:09:11.208836 talan-0.1.4.5/PKG-INFO
+-rw-r--r--   0 rstudio   (1001) users      (100)      314 2021-10-14 21:05:42.000000 talan-0.1.4.5/README.md
+-rw-r--r--   0 rstudio   (1001) users      (100)       38 2023-07-26 21:09:11.212836 talan-0.1.4.5/setup.cfg
+-rw-r--r--   0 rstudio   (1001) users      (100)      975 2023-07-26 21:07:48.000000 talan-0.1.4.5/setup.py
+drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2023-07-26 21:09:11.208836 talan-0.1.4.5/talan/
+-rwxr-xr-x   0 rstudio   (1001) users      (100)      240 2023-07-26 21:08:00.000000 talan-0.1.4.5/talan/__init__.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    39966 2023-07-04 04:09:16.000000 talan-0.1.4.5/talan/_alan_calc.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    13742 2023-07-03 20:21:58.000000 talan-0.1.4.5/talan/_alan_date.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    14990 2022-05-09 20:38:57.000000 talan-0.1.4.5/talan/_alan_mp4.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    11723 2022-11-22 22:19:42.000000 talan-0.1.4.5/talan/_alan_ohlc_fcs.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     4265 2019-08-01 04:14:12.000000 talan-0.1.4.5/talan/_alan_optparse.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    14976 2021-10-29 01:15:39.000000 talan-0.1.4.5/talan/_alan_pppscf.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    29498 2023-01-23 14:30:39.000000 talan-0.1.4.5/talan/_alan_rmc.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    65801 2023-07-04 02:53:11.000000 talan-0.1.4.5/talan/_alan_str.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    47116 2023-02-09 16:29:37.000000 talan-0.1.4.5/talan/alanapi.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     7501 2023-02-16 02:31:23.000000 talan-0.1.4.5/talan/chatgptAPI.py
+-rw-r--r--   0 rstudio   (1001) users      (100)    31949 2022-12-30 20:32:22.000000 talan-0.1.4.5/talan/csv2plotj2ts.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     7100 2021-09-19 20:39:01.000000 talan-0.1.4.5/talan/find_recent_eps.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     3518 2022-10-12 19:28:21.000000 talan-0.1.4.5/talan/fredReader.py
+-rw-r--r--   0 rstudio   (1001) users      (100)     2185 2023-07-18 18:27:13.000000 talan-0.1.4.5/talan/get_rq.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     6262 2023-01-31 19:25:24.000000 talan-0.1.4.5/talan/headline_calc.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     9876 2020-05-08 19:29:00.000000 talan-0.1.4.5/talan/headline_sts.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     6261 2020-05-19 00:26:02.000000 talan-0.1.4.5/talan/iex_peers.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    34234 2022-03-30 17:55:59.000000 talan-0.1.4.5/talan/lsi_daily.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     9822 2021-09-29 19:06:55.000000 talan-0.1.4.5/talan/macro_event_yh.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    41692 2022-12-23 21:01:13.000000 talan-0.1.4.5/talan/plot_templates.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     7703 2023-07-04 20:28:27.000000 talan-0.1.4.5/talan/prc_temp_DN.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    11503 2023-01-31 19:15:38.000000 talan-0.1.4.5/talan/record_hilo.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     1027 2023-07-18 15:56:52.000000 talan-0.1.4.5/talan/talan_wrap.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    14131 2023-01-06 22:09:49.000000 talan-0.1.4.5/talan/theme_list.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     6113 2023-02-02 21:45:43.000000 talan-0.1.4.5/talan/ticker2label.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     6613 2022-11-07 00:19:24.000000 talan-0.1.4.5/talan/ticker_mapping.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     4825 2021-10-11 19:44:03.000000 talan-0.1.4.5/talan/upd_mapping_ticker.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     8716 2023-07-05 03:31:50.000000 talan-0.1.4.5/talan/webReader.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    42362 2023-07-26 21:05:51.000000 talan-0.1.4.5/talan/yh_chart.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)    15454 2022-11-14 21:58:33.000000 talan-0.1.4.5/talan/yh_hist_batch.py
+-rwxr-xr-x   0 rstudio   (1001) users      (100)     5521 2023-01-31 21:38:37.000000 talan-0.1.4.5/talan/yh_predefined.py
+drwxr-xr-x   0 rstudio   (1001) users      (100)        0 2023-07-26 21:09:11.208836 talan-0.1.4.5/talan.egg-info/
+-rw-r--r--   0 rstudio   (1001) users      (100)      688 2023-07-26 21:09:11.000000 talan-0.1.4.5/talan.egg-info/PKG-INFO
+-rw-r--r--   0 rstudio   (1001) users      (100)      837 2023-07-26 21:09:11.000000 talan-0.1.4.5/talan.egg-info/SOURCES.txt
+-rw-r--r--   0 rstudio   (1001) users      (100)        1 2023-07-26 21:09:11.000000 talan-0.1.4.5/talan.egg-info/dependency_links.txt
+-rw-r--r--   0 rstudio   (1001) users      (100)       38 2023-07-26 21:09:11.000000 talan-0.1.4.5/talan.egg-info/requires.txt
+-rw-r--r--   0 rstudio   (1001) users      (100)        6 2023-07-26 21:09:11.000000 talan-0.1.4.5/talan.egg-info/top_level.txt
```

### Comparing `talan-0.1.4.4/PKG-INFO` & `talan-0.1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talan
-Version: 0.1.4.4
+Version: 0.1.4.5
 Summary: ('Technical ALgorithmic ANalytics',)
 Home-page: https://github.com/beyondbond/talan
 Author: Ted Hong
 Author-email: ted@beyondbond.com
 License: BSD 2-clause
 Description: Utility funcitions for financial analysis
 Platform: UNKNOWN
```

### Comparing `talan-0.1.4.4/setup.py` & `talan-0.1.4.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup,find_packages
-VERSION = '0.1.4.4' 
+VERSION = '0.1.4.5' 
 DESCRIPTION = 'Technical ALgorithmic ANalytics',
 LONG_DESCRIPTION = 'Utility funcitions for financial analysis'
 
 # Setting up
 setup(
     name='talan',
     version=VERSION,
```

### Comparing `talan-0.1.4.4/talan/_alan_calc.py` & `talan-0.1.4.5/talan/_alan_calc.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/_alan_date.py` & `talan-0.1.4.5/talan/_alan_date.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/_alan_mp4.py` & `talan-0.1.4.5/talan/_alan_mp4.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/_alan_ohlc_fcs.py` & `talan-0.1.4.5/talan/_alan_ohlc_fcs.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/_alan_optparse.py` & `talan-0.1.4.5/talan/_alan_optparse.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/_alan_pppscf.py` & `talan-0.1.4.5/talan/_alan_pppscf.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/_alan_rmc.py` & `talan-0.1.4.5/talan/_alan_rmc.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/_alan_str.py` & `talan-0.1.4.5/talan/_alan_str.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/alanapi.py` & `talan-0.1.4.5/talan/alanapi.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/chatgptAPI.py` & `talan-0.1.4.5/talan/chatgptAPI.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/csv2plotj2ts.py` & `talan-0.1.4.5/talan/csv2plotj2ts.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/find_recent_eps.py` & `talan-0.1.4.5/talan/find_recent_eps.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/fredReader.py` & `talan-0.1.4.5/talan/fredReader.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/get_rq.py` & `talan-0.1.4.5/talan/get_rq.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/headline_calc.py` & `talan-0.1.4.5/talan/headline_calc.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/headline_sts.py` & `talan-0.1.4.5/talan/headline_sts.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/iex_peers.py` & `talan-0.1.4.5/talan/iex_peers.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/lsi_daily.py` & `talan-0.1.4.5/talan/lsi_daily.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/macro_event_yh.py` & `talan-0.1.4.5/talan/macro_event_yh.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/plot_templates.py` & `talan-0.1.4.5/talan/plot_templates.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/prc_temp_DN.py` & `talan-0.1.4.5/talan/prc_temp_DN.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/record_hilo.py` & `talan-0.1.4.5/talan/record_hilo.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/talan_wrap.py` & `talan-0.1.4.5/talan/talan_wrap.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/theme_list.py` & `talan-0.1.4.5/talan/theme_list.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/ticker2label.py` & `talan-0.1.4.5/talan/ticker2label.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/ticker_mapping.py` & `talan-0.1.4.5/talan/ticker_mapping.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/upd_mapping_ticker.py` & `talan-0.1.4.5/talan/upd_mapping_ticker.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/webReader.py` & `talan-0.1.4.5/talan/webReader.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/yh_chart.py` & `talan-0.1.4.5/talan/yh_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 ----------------------------------------------------------------------------------------
 '''
 __usage__='\n'.join(__doc__.split('\n')[:8])
 import sys, datetime, re
 import requests
 import numpy as np
 import pandas as pd
-from pandas.io.json import json_normalize
 from _alan_str import write2mdb,find_mdb,insert_mdb,upsert_mdb,get_arg2func
 from _alan_calc import getKeyVal,conn2pgdb,conn2mgdb,renameDict,subDict,subDF,saferun,safeRunArg
 
 headers={'Content-Type': 'text/html', 'Accept': 'application/json', 'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/59.0.3071.115 Safari/537.36'}
 credentials={}
 apiBase = 'https://query2.finance.yahoo.com'
```

### Comparing `talan-0.1.4.4/talan/yh_hist_batch.py` & `talan-0.1.4.5/talan/yh_hist_batch.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan/yh_predefined.py` & `talan-0.1.4.5/talan/yh_predefined.py`

 * *Files identical despite different names*

### Comparing `talan-0.1.4.4/talan.egg-info/PKG-INFO` & `talan-0.1.4.5/talan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talan
-Version: 0.1.4.4
+Version: 0.1.4.5
 Summary: ('Technical ALgorithmic ANalytics',)
 Home-page: https://github.com/beyondbond/talan
 Author: Ted Hong
 Author-email: ted@beyondbond.com
 License: BSD 2-clause
 Description: Utility funcitions for financial analysis
 Platform: UNKNOWN
```

### Comparing `talan-0.1.4.4/talan.egg-info/SOURCES.txt` & `talan-0.1.4.5/talan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

