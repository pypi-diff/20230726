# Comparing `tmp/hyperopt_prophet-0.1.3.tar.gz` & `tmp/hyperopt_prophet-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperopt_prophet-0.1.3.tar", max compression
+gzip compressed data, was "hyperopt_prophet-0.1.4.tar", max compression
```

## Comparing `hyperopt_prophet-0.1.3.tar` & `hyperopt_prophet-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1083 2023-07-26 04:22:50.575338 hyperopt_prophet-0.1.3/LICENSE
--rw-r--r--   0        0        0      980 2023-07-26 04:22:50.575338 hyperopt_prophet-0.1.3/README.md
--rw-r--r--   0        0        0      150 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/hyperopt_prophet/__init__.py
--rw-r--r--   0        0        0     5047 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/hyperopt_prophet/inference.py
--rw-r--r--   0        0        0    21410 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/hyperopt_prophet/model.py
--rw-r--r--   0        0        0     9108 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/hyperopt_prophet/training.py
--rw-r--r--   0        0        0     4714 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/hyperopt_prophet/utils.py
--rw-r--r--   0        0        0       85 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/main.py
--rw-r--r--   0        0        0      818 2023-07-26 04:22:50.579338 hyperopt_prophet-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-07-26 04:48:12.823779 hyperopt_prophet-0.1.4/LICENSE
+-rw-r--r--   0        0        0      980 2023-07-26 04:48:12.823779 hyperopt_prophet-0.1.4/README.md
+-rw-r--r--   0        0        0      101 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/hyperopt_prophet/__init__.py
+-rw-r--r--   0        0        0     5047 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/hyperopt_prophet/inference.py
+-rw-r--r--   0        0        0    21410 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/hyperopt_prophet/model.py
+-rw-r--r--   0        0        0     9108 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/hyperopt_prophet/training.py
+-rw-r--r--   0        0        0     4714 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/hyperopt_prophet/utils.py
+-rw-r--r--   0        0        0       85 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/main.py
+-rw-r--r--   0        0        0      818 2023-07-26 04:48:12.827779 hyperopt_prophet-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 hyperopt_prophet-0.1.4/PKG-INFO
```

### Comparing `hyperopt_prophet-0.1.3/LICENSE` & `hyperopt_prophet-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.3/README.md` & `hyperopt_prophet-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.3/hyperopt_prophet/inference.py` & `hyperopt_prophet-0.1.4/hyperopt_prophet/inference.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.3/hyperopt_prophet/model.py` & `hyperopt_prophet-0.1.4/hyperopt_prophet/model.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.3/hyperopt_prophet/training.py` & `hyperopt_prophet-0.1.4/hyperopt_prophet/training.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.3/hyperopt_prophet/utils.py` & `hyperopt_prophet-0.1.4/hyperopt_prophet/utils.py`

 * *Files identical despite different names*

### Comparing `hyperopt_prophet-0.1.3/pyproject.toml` & `hyperopt_prophet-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyperopt-prophet"
-version = "0.1.3"
+version = "0.1.4"
 description = "Integration of prophet forecasting with hyperopt, mlflow"
 authors = ["Carlos D. Escobar-Valbuena <carlosdavidescobar@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "hyperopt_prophet"},
     {include = "main.py"}
```

### Comparing `hyperopt_prophet-0.1.3/PKG-INFO` & `hyperopt_prophet-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperopt-prophet
-Version: 0.1.3
+Version: 0.1.4
 Summary: Integration of prophet forecasting with hyperopt, mlflow
 License: MIT
 Author: Carlos D. Escobar-Valbuena
 Author-email: carlosdavidescobar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

