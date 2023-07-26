# Comparing `tmp/ptarcade-0.1.4.tar.gz` & `tmp/ptarcade-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptarcade-0.1.4.tar", max compression
+gzip compressed data, was "ptarcade-0.1.5.tar", max compression
```

## Comparing `ptarcade-0.1.4.tar` & `ptarcade-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1073 2023-07-02 18:28:45.209694 ptarcade-0.1.4/LICENSE
--rw-r--r--   0        0        0      673 2023-07-02 18:28:45.209694 ptarcade-0.1.4/README.md
--rw-r--r--   0        0        0     3313 2023-07-04 17:31:28.939748 ptarcade-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      555 2023-07-02 18:28:45.239694 ptarcade-0.1.4/src/ptarcade/__init__.py
--rw-r--r--   0        0        0    32466 2023-07-02 18:28:45.239694 ptarcade-0.1.4/src/ptarcade/chains_utils.py
--rw-r--r--   0        0        0       23 2023-07-02 18:28:45.239694 ptarcade-0.1.4/src/ptarcade/data/__init__.py
--rw-r--r--   0        0        0     1026 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/data/default_config.py
--rw-r--r--   0        0        0    29964 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/data/g_star.dat
--rw-r--r--   0        0        0     4994 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/fast_interpolate.py
--rw-r--r--   0        0        0    15036 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/input_handler.py
--rw-r--r--   0        0        0    17354 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/models_utils.py
--rw-r--r--   0        0        0    30151 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/plot_utils.py
--rw-r--r--   0        0        0     6885 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/pta_importer.py
--rw-r--r--   0        0        0    12031 2023-07-04 17:30:58.493116 ptarcade-0.1.4/src/ptarcade/sampler.py
--rw-r--r--   0        0        0    18088 2023-07-02 18:28:45.243028 ptarcade-0.1.4/src/ptarcade/signal_builder.py
--rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 ptarcade-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-26 03:41:09.403224 ptarcade-0.1.5/LICENSE
+-rw-r--r--   0        0        0      673 2023-07-26 03:41:09.403224 ptarcade-0.1.5/README.md
+-rw-r--r--   0        0        0     3314 2023-07-26 03:41:09.435224 ptarcade-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      555 2023-07-26 03:41:09.435224 ptarcade-0.1.5/src/ptarcade/__init__.py
+-rw-r--r--   0        0        0    32466 2023-07-26 03:41:09.435224 ptarcade-0.1.5/src/ptarcade/chains_utils.py
+-rw-r--r--   0        0        0       23 2023-07-26 03:41:09.435224 ptarcade-0.1.5/src/ptarcade/data/__init__.py
+-rw-r--r--   0        0        0     1026 2023-07-26 03:41:09.435224 ptarcade-0.1.5/src/ptarcade/data/default_config.py
+-rw-r--r--   0        0        0    29964 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/data/g_star.dat
+-rw-r--r--   0        0        0     4994 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/fast_interpolate.py
+-rw-r--r--   0        0        0    15036 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/input_handler.py
+-rw-r--r--   0        0        0    17354 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/models_utils.py
+-rw-r--r--   0        0        0    30151 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/plot_utils.py
+-rw-r--r--   0        0        0     6885 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/pta_importer.py
+-rw-r--r--   0        0        0    12031 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/sampler.py
+-rw-r--r--   0        0        0    18088 2023-07-26 03:41:09.439224 ptarcade-0.1.5/src/ptarcade/signal_builder.py
+-rw-r--r--   0        0        0     2646 1970-01-01 00:00:00.000000 ptarcade-0.1.5/PKG-INFO
```

### Comparing `ptarcade-0.1.4/LICENSE` & `ptarcade-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/README.md` & `ptarcade-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/pyproject.toml` & `ptarcade-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
   "doc/build/*.py",
   "doc/temp/*.py",
   ".eggs/*.py",
 ]
 
 [tool.poetry]
 name = "PTArcade"
-version = "0.1.4"
+version = "0.1.5"
 description = "PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data."
 readme = "README.md"
 authors = ["Andrea Mitridate <andrea.mitridate@nanograv.org>",]
 keywords = ["ptarcade"]
 repository = "https://github.com/andrea-mitridate/PTArcade"
 documentation = "https://andrea-mitridate.github.io/PTArcade/"
 classifiers = [
@@ -124,15 +124,15 @@
 [tool.poetry.dependencies]
 python = ">=3.9, <3.11"
 ptmcmcsampler = "^2.1.1"
 mpi4py = "^3.1.4"
 h5py = "^3.8.0"
 enterprise-pulsar = "^3.3.3"
 enterprise-extensions = "^2.4.2"
-scikit-sparse = "^0.4.8"
+scikit-sparse = "^0.4.12"
 natpy = "^0.1.1"
 numpy = "^1.24.3"
 pandas = "^2.0.2"
 pyarrow = "^12.0.0"
 getdist = "^1.4.3"
 astroml = "^1.0.2.post1"
 scipy = "^1.10.1"
```

### Comparing `ptarcade-0.1.4/src/ptarcade/__init__.py` & `ptarcade-0.1.5/src/ptarcade/__init__.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/src/ptarcade/chains_utils.py` & `ptarcade-0.1.5/src/ptarcade/chains_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/src/ptarcade/data/default_config.py` & `ptarcade-0.1.5/src/ptarcade/data/default_config.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/src/ptarcade/data/g_star.dat` & `ptarcade-0.1.5/src/ptarcade/data/g_star.dat`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/src/ptarcade/fast_interpolate.py` & `ptarcade-0.1.5/src/ptarcade/fast_interpolate.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/src/ptarcade/input_handler.py` & `ptarcade-0.1.5/src/ptarcade/input_handler.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/src/ptarcade/models_utils.py` & `ptarcade-0.1.5/src/ptarcade/models_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/src/ptarcade/plot_utils.py` & `ptarcade-0.1.5/src/ptarcade/plot_utils.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/src/ptarcade/pta_importer.py` & `ptarcade-0.1.5/src/ptarcade/pta_importer.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/src/ptarcade/sampler.py` & `ptarcade-0.1.5/src/ptarcade/sampler.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/src/ptarcade/signal_builder.py` & `ptarcade-0.1.5/src/ptarcade/signal_builder.py`

 * *Files identical despite different names*

### Comparing `ptarcade-0.1.4/PKG-INFO` & `ptarcade-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptarcade
-Version: 0.1.4
+Version: 0.1.5
 Summary: PTArcade provides an interface to the ENTERPRISE analysis suite and allows for simple implementation of new-physics searches in PTA data.
 Home-page: https://github.com/andrea-mitridate/PTArcade
 Keywords: ptarcade
 Author: Andrea Mitridate
 Author-email: andrea.mitridate@nanograv.org
 Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Developers
@@ -29,15 +29,15 @@
 Requires-Dist: natpy (>=0.1.1,<0.2.0)
 Requires-Dist: numba (>=0.57.0,<0.58.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: ptmcmcsampler (>=2.1.1,<3.0.0)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: rich[jupyter] (>=13.4.2,<14.0.0)
-Requires-Dist: scikit-sparse (>=0.4.8,<0.5.0)
+Requires-Dist: scikit-sparse (>=0.4.12,<0.5.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: setuptools (>=67.8.0,<68.0.0)
 Requires-Dist: tables (>=3.8.0,<4.0.0)
 Project-URL: Bug Tracker, https://github.com/andrea-mitridate/PTArcade/issues
 Project-URL: Documentation, https://andrea-mitridate.github.io/PTArcade/
 Project-URL: Repository, https://github.com/andrea-mitridate/PTArcade
 Description-Content-Type: text/markdown
```

