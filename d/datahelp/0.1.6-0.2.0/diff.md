# Comparing `tmp/datahelp-0.1.6.tar.gz` & `tmp/datahelp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datahelp-0.1.6.tar", max compression
+gzip compressed data, was "datahelp-0.2.0.tar", last modified: Wed Jul 26 09:23:30 2023, max compression
```

## Comparing `datahelp-0.1.6.tar` & `datahelp-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,22 @@
--rw-r--r--   0        0        0     1067 2023-07-19 21:51:44.526819 datahelp-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0     3277 2023-07-23 15:57:07.399162 datahelp-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-04-26 07:38:28.009704 datahelp-0.1.6/datahelp/.editorconfig
--rw-r--r--   0        0        0       22 2023-07-23 19:01:46.446493 datahelp-0.1.6/datahelp/__init__.py
--rw-r--r--   0        0        0     4634 2023-07-23 15:41:42.769384 datahelp-0.1.6/datahelp/create_project.py
--rw-r--r--   0        0        0     7813 2023-07-23 00:03:38.918086 datahelp-0.1.6/datahelp/eda.py
--rw-r--r--   0        0        0     8215 2023-07-23 18:22:48.157069 datahelp-0.1.6/datahelp/examples/.ipynb_checkpoints/ex3-checkpoint.ipynb
--rw-r--r--   0        0        0     3858 2023-05-01 16:01:21.804048 datahelp-0.1.6/datahelp/examples/data/iris.csv
--rw-r--r--   0        0        0     1755 2023-07-22 21:56:39.608845 datahelp-0.1.6/datahelp/examples/ex1.py
--rw-r--r--   0        0        0    17425 2023-07-23 18:52:53.576632 datahelp-0.1.6/datahelp/examples/ex3.ipynb
--rw-r--r--   0        0        0     5003 2023-07-22 22:04:55.078795 datahelp-0.1.6/datahelp/feature_engineering.py
--rw-r--r--   0        0        0     4231 2023-07-22 22:00:28.688823 datahelp-0.1.6/datahelp/modelling.py
--rw-r--r--   0        0        0     1042 2023-07-22 23:17:03.308364 datahelp-0.1.6/datahelp/utils.py
--rw-r--r--   0        0        0      745 2023-07-19 21:38:45.626915 datahelp-0.1.6/datahelp/visualize.py
--rw-r--r--   0        0        0      941 2023-07-23 19:01:41.196494 datahelp-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4626 1970-01-01 00:00:00.000000 datahelp-0.1.6/PKG-INFO
+drwxr-xr-x   0 shak      (1000) shak      (1000)        0 2023-07-26 09:23:30.513308 datahelp-0.2.0/
+-rw-r--r--   0 shak      (1000) shak      (1000)     1067 2023-07-19 21:51:44.000000 datahelp-0.2.0/LICENSE.txt
+-rw-r--r--   0 shak      (1000) shak      (1000)     3772 2023-07-26 09:23:30.513308 datahelp-0.2.0/PKG-INFO
+-rw-r--r--   0 shak      (1000) shak      (1000)     3327 2023-07-23 19:35:11.000000 datahelp-0.2.0/README.md
+drwxr-xr-x   0 shak      (1000) shak      (1000)        0 2023-07-26 09:23:30.513308 datahelp-0.2.0/datahelp/
+-rw-r--r--   0 shak      (1000) shak      (1000)       22 2023-07-23 19:01:46.000000 datahelp-0.2.0/datahelp/__init__.py
+-rw-r--r--   0 shak      (1000) shak      (1000)     4634 2023-07-23 15:41:42.000000 datahelp-0.2.0/datahelp/create_project.py
+-rw-r--r--   0 shak      (1000) shak      (1000)    11106 2023-07-23 19:56:09.000000 datahelp-0.2.0/datahelp/eda.py
+-rw-r--r--   0 shak      (1000) shak      (1000)     5003 2023-07-22 22:04:55.000000 datahelp-0.2.0/datahelp/feature_engineering.py
+-rw-r--r--   0 shak      (1000) shak      (1000)     4231 2023-07-22 22:00:28.000000 datahelp-0.2.0/datahelp/modelling.py
+-rw-r--r--   0 shak      (1000) shak      (1000)     7248 2023-07-23 19:55:05.000000 datahelp-0.2.0/datahelp/timeseries.py
+-rw-r--r--   0 shak      (1000) shak      (1000)     1042 2023-07-22 23:17:03.000000 datahelp-0.2.0/datahelp/utils.py
+-rw-r--r--   0 shak      (1000) shak      (1000)      745 2023-07-19 21:38:45.000000 datahelp-0.2.0/datahelp/visualize.py
+drwxr-xr-x   0 shak      (1000) shak      (1000)        0 2023-07-26 09:23:30.513308 datahelp-0.2.0/datahelp.egg-info/
+-rw-r--r--   0 shak      (1000) shak      (1000)     3772 2023-07-26 09:23:30.000000 datahelp-0.2.0/datahelp.egg-info/PKG-INFO
+-rw-r--r--   0 shak      (1000) shak      (1000)      395 2023-07-26 09:23:30.000000 datahelp-0.2.0/datahelp.egg-info/SOURCES.txt
+-rw-r--r--   0 shak      (1000) shak      (1000)        1 2023-07-26 09:23:30.000000 datahelp-0.2.0/datahelp.egg-info/dependency_links.txt
+-rw-r--r--   0 shak      (1000) shak      (1000)       65 2023-07-26 09:23:30.000000 datahelp-0.2.0/datahelp.egg-info/requires.txt
+-rw-r--r--   0 shak      (1000) shak      (1000)        9 2023-07-26 09:23:30.000000 datahelp-0.2.0/datahelp.egg-info/top_level.txt
+-rw-r--r--   0 shak      (1000) shak      (1000)      941 2023-07-26 09:20:48.000000 datahelp-0.2.0/pyproject.toml
+-rw-r--r--   0 shak      (1000) shak      (1000)       79 2023-07-26 09:23:30.513308 datahelp-0.2.0/setup.cfg
+-rw-r--r--   0 shak      (1000) shak      (1000)     1039 2023-07-26 09:22:49.000000 datahelp-0.2.0/setup.py
```

### Comparing `datahelp-0.1.6/LICENSE.txt` & `datahelp-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datahelp-0.1.6/README.md` & `datahelp-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 ```bash
 pip install datahelp
 ```
 
 Once installed, you can import the library and explore its functionality:
 
 ```python
-import datahelp as dh
+import datahelp as dh # import the datahelp library
 
-df = pd.read_csv("data/iris.csv")
+df = pd.read_csv("data/iris.csv") # load iris dataset
 
 df.head()
 
 cats = dh.eda.get_cat_vars(df)
 print(cats)
 
 num_var = dh.eda.get_num_vars(df)
```

### Comparing `datahelp-0.1.6/datahelp/create_project.py` & `datahelp-0.2.0/datahelp/create_project.py`

 * *Files identical despite different names*

### Comparing `datahelp-0.1.6/datahelp/feature_engineering.py` & `datahelp-0.2.0/datahelp/feature_engineering.py`

 * *Files identical despite different names*

### Comparing `datahelp-0.1.6/datahelp/modelling.py` & `datahelp-0.2.0/datahelp/modelling.py`

 * *Files identical despite different names*

### Comparing `datahelp-0.1.6/datahelp/utils.py` & `datahelp-0.2.0/datahelp/utils.py`

 * *Files identical despite different names*

### Comparing `datahelp-0.1.6/datahelp/visualize.py` & `datahelp-0.2.0/datahelp/visualize.py`

 * *Files identical despite different names*

### Comparing `datahelp-0.1.6/pyproject.toml` & `datahelp-0.2.0/pyproject.toml`

 * *Files identical despite different names*

