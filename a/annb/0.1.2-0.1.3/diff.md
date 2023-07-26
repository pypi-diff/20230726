# Comparing `tmp/annb-0.1.2.tar.gz` & `tmp/annb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annb-0.1.2.tar", last modified: Wed Jul 26 03:42:07 2023, max compression
+gzip compressed data, was "annb-0.1.3.tar", last modified: Wed Jul 26 03:46:13 2023, max compression
```

## Comparing `annb-0.1.2.tar` & `annb-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.324287 annb-0.1.2/
--rw-r--r--   0 jibin      (501) staff       (20)    11357 2023-06-23 11:24:40.000000 annb-0.1.2/LICENSE
--rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-26 03:42:07.324397 annb-0.1.2/PKG-INFO
--rw-r--r--   0 jibin      (501) staff       (20)      297 2023-07-25 03:49:16.000000 annb-0.1.2/README.md
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.320634 annb-0.1.2/annb/
--rw-r--r--   0 jibin      (501) staff       (20)      385 2023-07-26 03:41:45.000000 annb-0.1.2/annb/__init__.py
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.318123 annb-0.1.2/annb/anns/
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.322253 annb-0.1.2/annb/anns/faiss/
--rw-r--r--   0 jibin      (501) staff       (20)      489 2023-06-23 14:28:30.000000 annb-0.1.2/annb/anns/faiss/deploy.py
--rw-r--r--   0 jibin      (501) staff       (20)     3595 2023-07-26 03:41:08.000000 annb-0.1.2/annb/anns/faiss/indexes.py
--rw-r--r--   0 jibin      (501) staff       (20)     9413 2023-07-26 03:19:49.000000 annb-0.1.2/annb/cli.py
--rw-r--r--   0 jibin      (501) staff       (20)     1853 2023-07-25 03:08:09.000000 annb-0.1.2/annb/config.py
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.324035 annb-0.1.2/annb/dataset/
--rw-r--r--   0 jibin      (501) staff       (20)      213 2023-07-25 03:44:19.000000 annb-0.1.2/annb/dataset/__init__.py
--rw-r--r--   0 jibin      (501) staff       (20)     1267 2023-07-25 03:08:09.000000 annb-0.1.2/annb/dataset/base_dataset.py
--rw-r--r--   0 jibin      (501) staff       (20)     6734 2023-07-25 03:08:09.000000 annb-0.1.2/annb/dataset/hdf5_dataset.py
--rw-r--r--   0 jibin      (501) staff       (20)     1946 2023-07-25 03:08:09.000000 annb-0.1.2/annb/dataset/random_dataset.py
--rw-r--r--   0 jibin      (501) staff       (20)     2416 2023-07-25 03:08:09.000000 annb-0.1.2/annb/dataset/utils.py
--rw-r--r--   0 jibin      (501) staff       (20)       75 2023-06-23 13:33:53.000000 annb-0.1.2/annb/envs.py
--rw-r--r--   0 jibin      (501) staff       (20)     7996 2023-07-26 03:37:36.000000 annb-0.1.2/annb/indexes.py
--rw-r--r--   0 jibin      (501) staff       (20)     1431 2023-07-25 03:07:57.000000 annb-0.1.2/annb/plot.py
--rw-r--r--   0 jibin      (501) staff       (20)     6405 2023-07-25 03:08:09.000000 annb-0.1.2/annb/result.py
--rw-r--r--   0 jibin      (501) staff       (20)     7718 2023-07-25 03:07:57.000000 annb-0.1.2/annb/runner.py
-drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:42:07.321696 annb-0.1.2/annb.egg-info/
--rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/PKG-INFO
--rw-r--r--   0 jibin      (501) staff       (20)      517 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/SOURCES.txt
--rw-r--r--   0 jibin      (501) staff       (20)        1 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/dependency_links.txt
--rw-r--r--   0 jibin      (501) staff       (20)       84 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/entry_points.txt
--rw-r--r--   0 jibin      (501) staff       (20)       49 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/requires.txt
--rw-r--r--   0 jibin      (501) staff       (20)        5 2023-07-26 03:42:07.000000 annb-0.1.2/annb.egg-info/top_level.txt
--rw-r--r--   0 jibin      (501) staff       (20)       99 2023-07-25 03:07:57.000000 annb-0.1.2/pyproject.toml
--rw-r--r--   0 jibin      (501) staff       (20)      668 2023-07-26 03:42:07.324710 annb-0.1.2/setup.cfg
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.727983 annb-0.1.3/
+-rw-r--r--   0 jibin      (501) staff       (20)    11357 2023-06-23 11:24:40.000000 annb-0.1.3/LICENSE
+-rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-26 03:46:13.728068 annb-0.1.3/PKG-INFO
+-rw-r--r--   0 jibin      (501) staff       (20)      297 2023-07-25 03:49:16.000000 annb-0.1.3/README.md
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.724796 annb-0.1.3/annb/
+-rw-r--r--   0 jibin      (501) staff       (20)      385 2023-07-26 03:45:48.000000 annb-0.1.3/annb/__init__.py
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.722423 annb-0.1.3/annb/anns/
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.726479 annb-0.1.3/annb/anns/faiss/
+-rw-r--r--   0 jibin      (501) staff       (20)      489 2023-06-23 14:28:30.000000 annb-0.1.3/annb/anns/faiss/deploy.py
+-rw-r--r--   0 jibin      (501) staff       (20)     3595 2023-07-26 03:41:08.000000 annb-0.1.3/annb/anns/faiss/indexes.py
+-rw-r--r--   0 jibin      (501) staff       (20)     9433 2023-07-26 03:45:30.000000 annb-0.1.3/annb/cli.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1853 2023-07-25 03:08:09.000000 annb-0.1.3/annb/config.py
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.727729 annb-0.1.3/annb/dataset/
+-rw-r--r--   0 jibin      (501) staff       (20)      213 2023-07-25 03:44:19.000000 annb-0.1.3/annb/dataset/__init__.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1267 2023-07-25 03:08:09.000000 annb-0.1.3/annb/dataset/base_dataset.py
+-rw-r--r--   0 jibin      (501) staff       (20)     6734 2023-07-25 03:08:09.000000 annb-0.1.3/annb/dataset/hdf5_dataset.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1946 2023-07-25 03:08:09.000000 annb-0.1.3/annb/dataset/random_dataset.py
+-rw-r--r--   0 jibin      (501) staff       (20)     2416 2023-07-25 03:08:09.000000 annb-0.1.3/annb/dataset/utils.py
+-rw-r--r--   0 jibin      (501) staff       (20)       75 2023-06-23 13:33:53.000000 annb-0.1.3/annb/envs.py
+-rw-r--r--   0 jibin      (501) staff       (20)     7996 2023-07-26 03:37:36.000000 annb-0.1.3/annb/indexes.py
+-rw-r--r--   0 jibin      (501) staff       (20)     1431 2023-07-25 03:07:57.000000 annb-0.1.3/annb/plot.py
+-rw-r--r--   0 jibin      (501) staff       (20)     6405 2023-07-25 03:08:09.000000 annb-0.1.3/annb/result.py
+-rw-r--r--   0 jibin      (501) staff       (20)     7718 2023-07-25 03:07:57.000000 annb-0.1.3/annb/runner.py
+drwxr-xr-x   0 jibin      (501) staff       (20)        0 2023-07-26 03:46:13.726091 annb-0.1.3/annb.egg-info/
+-rw-r--r--   0 jibin      (501) staff       (20)      615 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/PKG-INFO
+-rw-r--r--   0 jibin      (501) staff       (20)      517 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/SOURCES.txt
+-rw-r--r--   0 jibin      (501) staff       (20)        1 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/dependency_links.txt
+-rw-r--r--   0 jibin      (501) staff       (20)       84 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/entry_points.txt
+-rw-r--r--   0 jibin      (501) staff       (20)       49 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/requires.txt
+-rw-r--r--   0 jibin      (501) staff       (20)        5 2023-07-26 03:46:13.000000 annb-0.1.3/annb.egg-info/top_level.txt
+-rw-r--r--   0 jibin      (501) staff       (20)       99 2023-07-25 03:07:57.000000 annb-0.1.3/pyproject.toml
+-rw-r--r--   0 jibin      (501) staff       (20)      668 2023-07-26 03:46:13.728399 annb-0.1.3/setup.cfg
```

### Comparing `annb-0.1.2/LICENSE` & `annb-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/PKG-INFO` & `annb-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annb
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple ANN benchmark tools
 Home-page: https://github.com/matrixji/annb
 Author: Ji Bin
 Author-email: matrixji@live.com
 License: Apache-2.0
 Keywords: ANN benchmark,Test tools
 Requires-Python: >=3.6
```

### Comparing `annb-0.1.2/annb/anns/faiss/indexes.py` & `annb-0.1.3/annb/anns/faiss/indexes.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/annb/cli.py` & `annb-0.1.3/annb/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
             v = int(v)
         except ValueError:
             v = str(v)
         try:
             v = float(v)
         except ValueError:
             v = str(v)
+        data[k] = v
     return data
 
 
 def load_index_factory(index_factory, index_factory_args) -> IndexUnderTestFactory:
     """
     >>> load_index_factory('annb.anns.faiss.indexes.index_under_test_factory')
     <annb.anns.faiss.indexes.FaissIndexUnderTestFactory object at 0x7f6b3d0b9e10>
```

### Comparing `annb-0.1.2/annb/config.py` & `annb-0.1.3/annb/config.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/annb/dataset/base_dataset.py` & `annb-0.1.3/annb/dataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/annb/dataset/hdf5_dataset.py` & `annb-0.1.3/annb/dataset/hdf5_dataset.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/annb/dataset/random_dataset.py` & `annb-0.1.3/annb/dataset/random_dataset.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/annb/dataset/utils.py` & `annb-0.1.3/annb/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/annb/indexes.py` & `annb-0.1.3/annb/indexes.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/annb/plot.py` & `annb-0.1.3/annb/plot.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/annb/result.py` & `annb-0.1.3/annb/result.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/annb/runner.py` & `annb-0.1.3/annb/runner.py`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/annb.egg-info/PKG-INFO` & `annb-0.1.3/annb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annb
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple ANN benchmark tools
 Home-page: https://github.com/matrixji/annb
 Author: Ji Bin
 Author-email: matrixji@live.com
 License: Apache-2.0
 Keywords: ANN benchmark,Test tools
 Requires-Python: >=3.6
```

### Comparing `annb-0.1.2/annb.egg-info/SOURCES.txt` & `annb-0.1.3/annb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `annb-0.1.2/setup.cfg` & `annb-0.1.3/setup.cfg`

 * *Files identical despite different names*

