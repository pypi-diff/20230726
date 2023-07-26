# Comparing `tmp/rapidpe_rift_pipe-0.5.4.dev20230725.tar.gz` & `tmp/rapidpe_rift_pipe-0.5.4.dev20230726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230725.tar", last modified: Tue Jul 25 05:17:32 2023, max compression
+gzip compressed data, was "rapidpe_rift_pipe-0.5.4.dev20230726.tar", last modified: Wed Jul 26 05:17:41 2023, max compression
```

## Comparing `rapidpe_rift_pipe-0.5.4.dev20230725.tar` & `rapidpe_rift_pipe-0.5.4.dev20230726.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.484939 rapidpe_rift_pipe-0.5.4.dev20230725/
--rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-25 05:17:32.485939 rapidpe_rift_pipe-0.5.4.dev20230725/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.479939 rapidpe_rift_pipe-0.5.4.dev20230725/bin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.481939 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/
--rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/compute_posterior.py
--rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/convert_result_to_txt.py
--rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/cprofile_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     6351 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/create_summarypage.py
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/plot_skymap.py
--rw-rw-rw-   0 root         (0) root         (0)     1419 2023-07-25 05:17:32.485939 rapidpe_rift_pipe-0.5.4.dev20230725/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.480939 rapidpe_rift_pipe-0.5.4.dev20230725/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.483939 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.484939 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.484939 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
--rwxrwxrwx   0 root         (0) root         (0)    31210 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/jacobians.py
--rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/pastro.py
--rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/postscript_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/profiling.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/search_bias_bounds.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.484939 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/static/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/static/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/static/stylesheet.css
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/test_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-25 05:17:21.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 05:17:32.484939 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1090 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1317 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      104 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 05:17:32.000000 rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:17:41.046542 rapidpe_rift_pipe-0.5.4.dev20230726/
+-rw-rw-rw-   0 root         (0) root         (0)    18046 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-26 05:17:41.046542 rapidpe_rift_pipe-0.5.4.dev20230726/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:17:41.028542 rapidpe_rift_pipe-0.5.4.dev20230726/bin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:17:41.034542 rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/compute_posterior.py
+-rwxrwxrwx   0 root         (0) root         (0)    12423 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/convert_result_to_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     6342 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/cprofile_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/create_summarypage.py
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/plot_skymap.py
+-rw-rw-rw-   0 root         (0) root         (0)     1419 2023-07-26 05:17:41.048542 rapidpe_rift_pipe-0.5.4.dev20230726/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:17:41.028542 rapidpe_rift_pipe-0.5.4.dev20230726/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:17:41.040542 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    47573 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    18705 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:17:41.044542 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/config_files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/config_files/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:17:41.045542 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/config_files/search_bias_bounds/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/config_files/search_bias_bounds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json
+-rwxrwxrwx   0 root         (0) root         (0)    31210 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/create_submit_dag_one_event.py
+-rw-rw-rw-   0 root         (0) root         (0)     2736 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/jacobians.py
+-rw-rw-rw-   0 root         (0) root         (0)     9701 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/pastro.py
+-rw-rw-rw-   0 root         (0) root         (0)    27677 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/postscript_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/profiling.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/search_bias_bounds.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:17:41.045542 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/static/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/static/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/static/stylesheet.css
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/test_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      375 2023-07-26 05:17:10.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 05:17:41.043542 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-07-26 05:17:40.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-07-26 05:17:41.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 05:17:40.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-26 05:17:40.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-26 05:17:40.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 05:17:40.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 05:17:40.000000 rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe.egg-info/zip-safe
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/COPYING` & `rapidpe_rift_pipe-0.5.4.dev20230726/COPYING`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/PKG-INFO` & `rapidpe_rift_pipe-0.5.4.dev20230726/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe_rift_pipe
-Version: 0.5.4.dev20230725
+Version: 0.5.4.dev20230726
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/compute_posterior.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/compute_posterior.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/convert_result_to_txt.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/convert_result_to_txt.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/cprofile_summary.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/cprofile_summary.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/create_summarypage.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/create_summarypage.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/bin/postscripts/plot_skymap.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/bin/postscripts/plot_skymap.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/setup.cfg` & `rapidpe_rift_pipe-0.5.4.dev20230726/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -49,10 +49,10 @@
 rapidpe_rift_pipe.config_files = *.ini, *.json
 
 [options.entry_points]
 console_scripts = 
 	rapidpe-rift-pipe = rapidpe_rift_pipe.cli:main
 
 [egg_info]
-tag_build = dev.20230725
+tag_build = dev.20230726
 tag_date = 0
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/cli.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/cli.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/config_files/search_bias_bounds/default.json`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/create_submit_dag_one_event.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/create_submit_dag_one_event.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/jacobians.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/jacobians.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/modules.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/modules.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/pastro.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/pastro.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/postscript_utils.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/postscript_utils.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/profiling.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/profiling.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/search_bias_bounds.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/search_bias_bounds.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/static/stylesheet.css` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/static/stylesheet.css`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe/test_config.py` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe/test_config.py`

 * *Files identical despite different names*

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/PKG-INFO` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidpe-rift-pipe
-Version: 0.5.4.dev20230725
+Version: 0.5.4.dev20230726
 Summary: Pipeline for running RapidPE and RIFT parameter estimation codes
 License: GPL-2+
 Keywords: parameter estimation,gravitational waves
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
```

### Comparing `rapidpe_rift_pipe-0.5.4.dev20230725/src/rapidpe_rift_pipe.egg-info/SOURCES.txt` & `rapidpe_rift_pipe-0.5.4.dev20230726/src/rapidpe_rift_pipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

