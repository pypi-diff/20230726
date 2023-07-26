# Comparing `tmp/hyperopt_prophet-0.1.1.tar.gz` & `tmp/hyperopt_prophet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperopt_prophet-0.1.1.tar", max compression
+gzip compressed data, was "hyperopt_prophet-0.1.2.tar", max compression
```

## Comparing `hyperopt_prophet-0.1.1.tar` & `hyperopt_prophet-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1083 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/LICENSE
--rw-r--r--   0        0        0      980 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/README.md
--rw-r--r--   0        0        0      113 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/__init__.py
--rw-r--r--   0        0        0      204 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/hyperopt_prophet.py
--rw-r--r--   0        0        0     5047 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/inference.py
--rw-r--r--   0        0        0    21410 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/model.py
--rw-r--r--   0        0        0      198 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/training.env
--rw-r--r--   0        0        0    10032 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/training.py
--rw-r--r--   0        0        0     4714 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/hyperopt_prophet/utils.py
--rw-r--r--   0        0        0       85 2023-07-26 01:16:38.925116 hyperopt_prophet-0.1.1/main.py
--rw-r--r--   0        0        0      843 2023-07-26 01:16:38.929116 hyperopt_prophet-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-26 03:08:56.622334 hyperopt_prophet-0.1.2/LICENSE
+-rw-r--r--   0        0        0      980 2023-07-26 03:08:56.622334 hyperopt_prophet-0.1.2/README.md
+-rw-r--r--   0        0        0      113 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/__init__.py
+-rw-r--r--   0        0        0      204 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/hyperopt_prophet.py
+-rw-r--r--   0        0        0     5047 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/inference.py
+-rw-r--r--   0        0        0    21410 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/model.py
+-rw-r--r--   0        0        0    10032 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/training.py
+-rw-r--r--   0        0        0     4714 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/hyperopt_prophet/utils.py
+-rw-r--r--   0        0        0       85 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/main.py
+-rw-r--r--   0        0        0      843 2023-07-26 03:08:56.626334 hyperopt_prophet-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.2/PKG-INFO
```

### Comparing `hyperopt_prophet-0.1.1/LICENSE` & `hyperopt_prophet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.1/README.md` & `hyperopt_prophet-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.1/hyperopt_prophet/inference.py` & `hyperopt_prophet-0.1.2/hyperopt_prophet/inference.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.1/hyperopt_prophet/model.py` & `hyperopt_prophet-0.1.2/hyperopt_prophet/model.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.1/hyperopt_prophet/training.py` & `hyperopt_prophet-0.1.2/hyperopt_prophet/training.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.1/hyperopt_prophet/utils.py` & `hyperopt_prophet-0.1.2/hyperopt_prophet/utils.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.1/pyproject.toml` & `hyperopt_prophet-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperopt-prophet"
-version = "0.1.1"
+version = "0.1.2"
 description = "Integration of prophet forecasting with hyperopt, mlflow"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "hyperopt_prophet"},
     {include = "main.py"}
```

### Comparing `hyperopt_prophet-0.1.1/PKG-INFO` & `hyperopt_prophet-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperopt-prophet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Integration of prophet forecasting with hyperopt, mlflow
 License: MIT
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

