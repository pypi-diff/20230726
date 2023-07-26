# Comparing `tmp/svo_api-0.1.0.tar.gz` & `tmp/svo_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svo_api-0.1.0.tar", last modified: Mon May 22 14:54:38 2023, max compression
+gzip compressed data, was "svo_api-0.1.1.tar", last modified: Wed Jul 26 07:52:11 2023, max compression
```

## Comparing `svo_api-0.1.0.tar` & `svo_api-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-22 14:54:38.023557 svo_api-0.1.0/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-05-22 14:38:11.000000 svo_api-0.1.0/LICENSE
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       25 2023-05-22 14:54:14.000000 svo_api-0.1.0/MANIFEST.in
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1976 2023-05-22 14:54:38.023557 svo_api-0.1.0/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1516 2023-05-22 14:50:25.000000 svo_api-0.1.0/README.md
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2023-05-22 14:38:58.000000 svo_api-0.1.0/requirements.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-05-22 14:54:38.023557 svo_api-0.1.0/setup.cfg
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1105 2023-05-22 14:51:15.000000 svo_api-0.1.0/setup.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-22 14:54:38.019557 svo_api-0.1.0/svo_api/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       78 2023-05-22 14:40:26.000000 svo_api-0.1.0/svo_api/__init__.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-05-22 14:40:03.000000 svo_api-0.1.0/svo_api/_version.py
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     4731 2023-05-22 14:51:15.000000 svo_api-0.1.0/svo_api/svo.py
-drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-05-22 14:54:38.019557 svo_api-0.1.0/svo_api.egg-info/
--rw-rw-r--   0 tomas     (1000) tomas     (1000)     1976 2023-05-22 14:54:38.000000 svo_api-0.1.0/svo_api.egg-info/PKG-INFO
--rw-rw-r--   0 tomas     (1000) tomas     (1000)      264 2023-05-22 14:54:38.000000 svo_api-0.1.0/svo_api.egg-info/SOURCES.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-05-22 14:54:38.000000 svo_api-0.1.0/svo_api.egg-info/dependency_links.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2023-05-22 14:54:38.000000 svo_api-0.1.0/svo_api.egg-info/requires.txt
--rw-rw-r--   0 tomas     (1000) tomas     (1000)        8 2023-05-22 14:54:38.000000 svo_api-0.1.0/svo_api.egg-info/top_level.txt
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-26 07:52:11.707971 svo_api-0.1.1/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1080 2023-07-26 07:30:56.000000 svo_api-0.1.1/LICENSE
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       25 2023-07-26 07:30:56.000000 svo_api-0.1.1/MANIFEST.in
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2421 2023-07-26 07:52:11.707971 svo_api-0.1.1/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1961 2023-07-26 07:30:56.000000 svo_api-0.1.1/README.md
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2023-07-26 07:30:56.000000 svo_api-0.1.1/requirements.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       38 2023-07-26 07:52:11.707971 svo_api-0.1.1/setup.cfg
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     1105 2023-07-26 07:30:56.000000 svo_api-0.1.1/setup.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-26 07:52:11.707971 svo_api-0.1.1/svo_api/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       78 2023-07-26 07:30:56.000000 svo_api-0.1.1/svo_api/__init__.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       46 2023-07-26 07:51:50.000000 svo_api-0.1.1/svo_api/_version.py
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     5137 2023-07-26 07:50:37.000000 svo_api-0.1.1/svo_api/svo.py
+drwxrwxr-x   0 tomas     (1000) tomas     (1000)        0 2023-07-26 07:52:11.707971 svo_api-0.1.1/svo_api.egg-info/
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)     2421 2023-07-26 07:52:11.000000 svo_api-0.1.1/svo_api.egg-info/PKG-INFO
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)      264 2023-07-26 07:52:11.000000 svo_api-0.1.1/svo_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        1 2023-07-26 07:52:11.000000 svo_api-0.1.1/svo_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)       15 2023-07-26 07:52:11.000000 svo_api-0.1.1/svo_api.egg-info/requires.txt
+-rw-rw-r--   0 tomas     (1000) tomas     (1000)        8 2023-07-26 07:52:11.000000 svo_api-0.1.1/svo_api.egg-info/top_level.txt
```

### Comparing `svo_api-0.1.0/LICENSE` & `svo_api-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `svo_api-0.1.0/PKG-INFO` & `svo_api-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svo_api
-Version: 0.1.0
+Version: 0.1.1
 Summary: API to download SVO filters
 Home-page: https://github.com/temuller/svo_api
 Author: Tomás Enrique Müller-Bravo
 Author-email: t.e.muller-bravo@ice.csic.es
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -15,15 +15,17 @@
 
 # SVO API
 API to download [Spanish Virtual Observatory](http://svo2.cab.inta-csic.es/theory/fps/index.php?mode=browse) filters.
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fsvo_api-blue.svg?style=flat)](https://github.com/temuller/svo_api)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/svo_api/blob/master/LICENSE)
 ![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue)
-[![PyPI](https://img.shields.io/pypi/v/wiserep_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/svo_api/)
+[![PyPI](https://img.shields.io/pypi/v/svo_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/svo_api/)
+[![DOI](https://zenodo.org/badge/643973679.svg)](https://zenodo.org/badge/latestdoi/643973679)
+
 
 ## Installation
 
 It is recommended to install ``svo_api`` from pip:
 
 ```python
 pip install svo_api
@@ -57,9 +59,18 @@
 To contribute, either open an issue or send a pull request (prefered option). You can also contact me directly (check my profile: https://github.com/temuller).
 
 ## Citing SVO API
 
 If you make use of this code, please cite it:
 
 ```code
-To be added
+@software{tomas_e_muller_bravo_2023_7957749,
+  author       = {Tomás E. Müller Bravo},
+  title        = {temuller/svo\_api: First Release (for zenodo)!},
+  month        = may,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v0.1.0-zenodo},
+  doi          = {10.5281/zenodo.7957749},
+  url          = {https://doi.org/10.5281/zenodo.7957749}
+}
 ```
```

### Comparing `svo_api-0.1.0/README.md` & `svo_api-0.1.1/svo_api.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,31 @@
+Metadata-Version: 2.1
+Name: svo-api
+Version: 0.1.1
+Summary: API to download SVO filters
+Home-page: https://github.com/temuller/svo_api
+Author: Tomás Enrique Müller-Bravo
+Author-email: t.e.muller-bravo@ice.csic.es
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # SVO API
 API to download [Spanish Virtual Observatory](http://svo2.cab.inta-csic.es/theory/fps/index.php?mode=browse) filters.
 
 [![repo](https://img.shields.io/badge/GitHub-temuller%2Fsvo_api-blue.svg?style=flat)](https://github.com/temuller/svo_api)
 [![license](http://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://github.com/temuller/svo_api/blob/master/LICENSE)
 ![Python Version](https://img.shields.io/badge/Python-3.9%2B-blue)
-[![PyPI](https://img.shields.io/pypi/v/wiserep_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/svo_api/)
+[![PyPI](https://img.shields.io/pypi/v/svo_api?label=PyPI&logo=pypi&logoColor=white)](https://pypi.org/project/svo_api/)
+[![DOI](https://zenodo.org/badge/643973679.svg)](https://zenodo.org/badge/latestdoi/643973679)
+
 
 ## Installation
 
 It is recommended to install ``svo_api`` from pip:
 
 ```python
 pip install svo_api
@@ -42,9 +59,18 @@
 To contribute, either open an issue or send a pull request (prefered option). You can also contact me directly (check my profile: https://github.com/temuller).
 
 ## Citing SVO API
 
 If you make use of this code, please cite it:
 
 ```code
-To be added
+@software{tomas_e_muller_bravo_2023_7957749,
+  author       = {Tomás E. Müller Bravo},
+  title        = {temuller/svo\_api: First Release (for zenodo)!},
+  month        = may,
+  year         = 2023,
+  publisher    = {Zenodo},
+  version      = {v0.1.0-zenodo},
+  doi          = {10.5281/zenodo.7957749},
+  url          = {https://doi.org/10.5281/zenodo.7957749}
+}
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `svo_api-0.1.0/setup.py` & `svo_api-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `svo_api-0.1.0/svo_api/svo.py` & `svo_api-0.1.1/svo_api/svo.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,18 +68,28 @@
     search_url = "http://svo2.cab.inta-csic.es/theory/fps/index.php?"
     facility_url = search_url + f"mode=browse&gname={facility}&asttype="
     response = get_response(facility_url)
 
     # get list of filters sets
     filters_sets = []
     filters_split = response.text.split(f"gname={facility}&gname2=")[1:]
+    # for facilities with multiple filter sets
     for line in filters_split:
         if len(line.split("&asttype=")) > 1:
             filter_set = line.split("&asttype=")[0]
-            filters_sets.append(filter_set)
+            if filter_set not in filters_sets:
+                filters_sets.append(filter_set)
+    
+    # for facilities with single filter sets
+    if len(filters_sets) == 0:
+        for line in filters_split:
+            if len(line.split("#")) > 1:
+                filter_set = line.split("#")[0]
+                if filter_set not in filters_sets:
+                    filters_sets.append(filter_set)
 
     if len(filters_sets) == 0:
         filters_sets = [facility]
 
     return filters_sets
```

