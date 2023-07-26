# Comparing `tmp/geosss-0.1.4.tar.gz` & `tmp/geosss-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geosss-0.1.4.tar", max compression
+gzip compressed data, was "geosss-0.1.5.tar", max compression
```

## Comparing `geosss-0.1.4.tar` & `geosss-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1474 2023-07-24 16:27:27.579099 geosss-0.1.4/LICENSE
--rw-r--r--   0        0        0     4520 2023-07-24 17:29:37.459846 geosss-0.1.4/README.md
--rw-r--r--   0        0        0      793 2023-07-25 18:15:32.875577 geosss-0.1.4/geosss/__init__.py
--rw-r--r--   0        0        0     1981 2023-07-25 18:12:02.547408 geosss-0.1.4/geosss/demo_vis.py
--rw-r--r--   0        0        0     5522 2023-07-25 18:15:09.487552 geosss-0.1.4/geosss/distributions.py
--rw-r--r--   0        0        0    10284 2023-07-25 18:15:13.175555 geosss-0.1.4/geosss/mcmc.py
--rw-r--r--   0        0        0     5091 2023-07-25 18:15:16.151557 geosss-0.1.4/geosss/rand.py
--rw-r--r--   0        0        0     3000 2023-07-25 18:15:18.371559 geosss-0.1.4/geosss/sphere.py
--rw-r--r--   0        0        0     7334 2023-07-25 18:16:16.463641 geosss-0.1.4/geosss/testing.py
--rw-r--r--   0        0        0     5156 2023-07-25 18:15:26.103567 geosss-0.1.4/geosss/utils.py
--rw-r--r--   0        0        0     9249 2023-07-25 18:15:30.843574 geosss-0.1.4/geosss/vMF_diagnostics.py
--rw-r--r--   0        0        0      890 2023-07-25 18:24:36.544259 geosss-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     5354 1970-01-01 00:00:00.000000 geosss-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1474 2023-07-24 16:27:27.579099 geosss-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4520 2023-07-24 17:29:37.459846 geosss-0.1.5/README.md
+-rw-r--r--   0        0        0      793 2023-07-25 18:35:32.784913 geosss-0.1.5/geosss/__init__.py
+-rw-r--r--   0        0        0     1981 2023-07-25 18:35:32.784913 geosss-0.1.5/geosss/demo_vis.py
+-rw-r--r--   0        0        0     5522 2023-07-25 18:35:32.784913 geosss-0.1.5/geosss/distributions.py
+-rw-r--r--   0        0        0    10284 2023-07-25 18:35:32.784913 geosss-0.1.5/geosss/mcmc.py
+-rw-r--r--   0        0        0     5091 2023-07-25 18:35:32.784913 geosss-0.1.5/geosss/rand.py
+-rw-r--r--   0        0        0     3000 2023-07-25 18:35:32.784913 geosss-0.1.5/geosss/sphere.py
+-rw-r--r--   0        0        0     7334 2023-07-25 18:35:32.784913 geosss-0.1.5/geosss/testing.py
+-rw-r--r--   0        0        0     5156 2023-07-25 18:35:32.784913 geosss-0.1.5/geosss/utils.py
+-rw-r--r--   0        0        0     9249 2023-07-25 18:35:32.784913 geosss-0.1.5/geosss/vMF_diagnostics.py
+-rw-r--r--   0        0        0      850 2023-07-26 10:36:25.614643 geosss-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5315 1970-01-01 00:00:00.000000 geosss-0.1.5/PKG-INFO
```

### Comparing `geosss-0.1.4/LICENSE` & `geosss-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/README.md` & `geosss-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/geosss/__init__.py` & `geosss-0.1.5/geosss/__init__.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/geosss/demo_vis.py` & `geosss-0.1.5/geosss/demo_vis.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/geosss/distributions.py` & `geosss-0.1.5/geosss/distributions.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/geosss/mcmc.py` & `geosss-0.1.5/geosss/mcmc.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/geosss/rand.py` & `geosss-0.1.5/geosss/rand.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/geosss/sphere.py` & `geosss-0.1.5/geosss/sphere.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/geosss/testing.py` & `geosss-0.1.5/geosss/testing.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/geosss/utils.py` & `geosss-0.1.5/geosss/utils.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/geosss/vMF_diagnostics.py` & `geosss-0.1.5/geosss/vMF_diagnostics.py`

 * *Files identical despite different names*

### Comparing `geosss-0.1.4/pyproject.toml` & `geosss-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geosss"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere."
 authors = ["Michael Habeck <michael.habeck@uni-jena.de>",
            "Shantanu Kodgirwar <shantanu.kodgirwar@uni-jena.de>", 
            "Mareike Hasenpflug <mareike.hasenpflug@uni-passau.de>",
            "Daniel Rudolf <daniel.rudolf@uni-passau.de>"]
 license = "BSD-3-Clause"
 readme = "README.md"
@@ -13,19 +13,17 @@
 [tool.poetry.dependencies]
 python = ">=3.9, <3.13"
 scipy = "^1.11.1"
 numpy = "^1.25.1"
 matplotlib = "^3.7.2"
 csb = "^1.2.5"
 arviz = "^0.15.1"
-pyqt5 = "^5.15.9"
 
 
 [tool.poetry.group.dev.dependencies]
-ipykernel = "^6.24.0"
 seaborn = "^0.12.2"
 black = "^23.7.0"
 tsp-solver = "^0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `geosss-0.1.4/PKG-INFO` & `geosss-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geosss
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python package implementing an ideal and shrinkage-based geodesic slice sampling on the sphere.
 Home-page: https://github.com/microscopic-image-analysis/geosss
 License: BSD-3-Clause
 Author: Michael Habeck
 Author-email: michael.habeck@uni-jena.de
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: BSD License
@@ -12,15 +12,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: arviz (>=0.15.1,<0.16.0)
 Requires-Dist: csb (>=1.2.5,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.2,<4.0.0)
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
-Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Project-URL: Repository, https://github.com/microscopic-image-analysis/geosss
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://raw.githubusercontent.com/microscopic-image-analysis/geosss/927ff8c8187b88a1a72725c4e450ae0f0523431b/assets/logo.svg" width="300">
 </p>
```

