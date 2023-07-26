# Comparing `tmp/anesthetic-2.1.0.tar.gz` & `tmp/anesthetic-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anesthetic-2.1.0.tar", last modified: Wed Jul 19 23:39:36 2023, max compression
+gzip compressed data, was "anesthetic-2.1.1.tar", last modified: Wed Jul 26 17:16:59 2023, max compression
```

## Comparing `anesthetic-2.1.0.tar` & `anesthetic-2.1.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:39:36.109542 anesthetic-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-19 23:39:24.000000 anesthetic-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-19 23:39:36.109542 anesthetic-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-19 23:39:24.000000 anesthetic-2.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:39:36.097542 anesthetic-2.1.0/anesthetic/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/_code_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/_format.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/boundary.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:39:36.101542 anesthetic-2.1.0/anesthetic/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/examples/_matplotlib_agg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/examples/perfect_ns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:39:36.101542 anesthetic-2.1.0/anesthetic/gui/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/gui/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/gui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/kde.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    54567 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:39:36.101542 anesthetic-2.1.0/anesthetic/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/plotting/_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:39:36.105542 anesthetic-2.1.0/anesthetic/plotting/_matplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/plotting/_matplotlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/plotting/_matplotlib/boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/plotting/_matplotlib/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/plotting/_matplotlib/hist.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/plotting/_matplotlib/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:39:36.105542 anesthetic-2.1.0/anesthetic/read/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/read/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/read/cobaya.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/read/getdist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/read/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/read/multinest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/read/polychord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/read/ultranest.py
--rw-r--r--   0 runner    (1001) docker     (123)    50714 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25506 2023-07-19 23:39:24.000000 anesthetic-2.1.0/anesthetic/weighted_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:39:36.101542 anesthetic-2.1.0/anesthetic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-19 23:39:36.000000 anesthetic-2.1.0/anesthetic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-19 23:39:36.000000 anesthetic-2.1.0/anesthetic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 23:39:36.000000 anesthetic-2.1.0/anesthetic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-19 23:39:36.000000 anesthetic-2.1.0/anesthetic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-19 23:39:36.000000 anesthetic-2.1.0/anesthetic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 23:39:36.000000 anesthetic-2.1.0/anesthetic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-19 23:39:24.000000 anesthetic-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-19 23:39:36.109542 anesthetic-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 23:39:36.109542 anesthetic-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-19 23:39:24.000000 anesthetic-2.1.0/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-19 23:39:24.000000 anesthetic-2.1.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-19 23:39:24.000000 anesthetic-2.1.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-19 23:39:24.000000 anesthetic-2.1.0/tests/test_labelled_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)    27808 2023-07-19 23:39:24.000000 anesthetic-2.1.0/tests/test_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-07-19 23:39:24.000000 anesthetic-2.1.0/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    62635 2023-07-19 23:39:24.000000 anesthetic-2.1.0/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-19 23:39:24.000000 anesthetic-2.1.0/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-19 23:39:24.000000 anesthetic-2.1.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34191 2023-07-19 23:39:24.000000 anesthetic-2.1.0/tests/test_weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:16:59.600386 anesthetic-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-26 17:16:49.000000 anesthetic-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 17:16:59.600386 anesthetic-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-07-26 17:16:49.000000 anesthetic-2.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:16:59.596386 anesthetic-2.1.1/anesthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/_code_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/boundary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:16:59.596386 anesthetic-2.1.1/anesthetic/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/examples/_matplotlib_agg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/examples/perfect_ns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:16:59.596386 anesthetic-2.1.1/anesthetic/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/gui/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/gui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54624 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:16:59.596386 anesthetic-2.1.1/anesthetic/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/plotting/_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:16:59.596386 anesthetic-2.1.1/anesthetic/plotting/_matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/plotting/_matplotlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/plotting/_matplotlib/boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/plotting/_matplotlib/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/plotting/_matplotlib/hist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/plotting/_matplotlib/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:16:59.600386 anesthetic-2.1.1/anesthetic/read/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/read/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/read/cobaya.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/read/getdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/read/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/read/multinest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/read/polychord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/read/ultranest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50714 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18707 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25506 2023-07-26 17:16:49.000000 anesthetic-2.1.1/anesthetic/weighted_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:16:59.596386 anesthetic-2.1.1/anesthetic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-07-26 17:16:59.000000 anesthetic-2.1.1/anesthetic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-26 17:16:59.000000 anesthetic-2.1.1/anesthetic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:16:59.000000 anesthetic-2.1.1/anesthetic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 17:16:59.000000 anesthetic-2.1.1/anesthetic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-26 17:16:59.000000 anesthetic-2.1.1/anesthetic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 17:16:59.000000 anesthetic-2.1.1/anesthetic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-26 17:16:49.000000 anesthetic-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-26 17:16:59.600386 anesthetic-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:16:59.600386 anesthetic-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-26 17:16:50.000000 anesthetic-2.1.1/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-26 17:16:50.000000 anesthetic-2.1.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-26 17:16:50.000000 anesthetic-2.1.1/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18564 2023-07-26 17:16:50.000000 anesthetic-2.1.1/tests/test_labelled_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28539 2023-07-26 17:16:50.000000 anesthetic-2.1.1/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-07-26 17:16:50.000000 anesthetic-2.1.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62635 2023-07-26 17:16:50.000000 anesthetic-2.1.1/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-26 17:16:50.000000 anesthetic-2.1.1/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-07-26 17:16:50.000000 anesthetic-2.1.1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34191 2023-07-26 17:16:50.000000 anesthetic-2.1.1/tests/test_weighted_pandas.py
```

### Comparing `anesthetic-2.1.0/LICENSE` & `anesthetic-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/PKG-INFO` & `anesthetic-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.1.0
+Version: 2.1.1
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -55,15 +55,15 @@
 Provides-Extra: all
 License-File: LICENSE
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.1.0
+:Version: 2.1.1
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.1.0/README.rst` & `anesthetic-2.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.1.0
+:Version: 2.1.1
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.1.0/anesthetic/__init__.py` & `anesthetic-2.1.1/anesthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/_code_utils.py` & `anesthetic-2.1.1/anesthetic/_code_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/_format.py` & `anesthetic-2.1.1/anesthetic/_format.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/boundary.py` & `anesthetic-2.1.1/anesthetic/boundary.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/convert.py` & `anesthetic-2.1.1/anesthetic/convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/examples/perfect_ns.py` & `anesthetic-2.1.1/anesthetic/examples/perfect_ns.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/examples/utils.py` & `anesthetic-2.1.1/anesthetic/examples/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/gui/plot.py` & `anesthetic-2.1.1/anesthetic/gui/plot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/gui/widgets.py` & `anesthetic-2.1.1/anesthetic/gui/widgets.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/kde.py` & `anesthetic-2.1.1/anesthetic/kde.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/labelled_pandas.py` & `anesthetic-2.1.1/anesthetic/labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/plot.py` & `anesthetic-2.1.1/anesthetic/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,22 +401,22 @@
                                           **kwargs)
                         else:
                             a.tick_params('y', left=True, labelleft=True,
                                           **kwargs)
                     elif a.position == 'diagonal':  # not first column
                         a.tick_params('y', direction='out', length=tl/2,
                                       left=True, labelleft=False, **kwargs)
-                    elif ax_[i-1].position == 'diagonal':  # next to diagonal
+                    elif ax_.iloc[i-1].position == 'diagonal':  # next to diag
                         a.tick_params('y', direction='in', length=tl/2,
                                       left=True, labelleft=False, **kwargs)
                     else:  # not diagonal and not first column
                         a.tick_params('y', direction='inout',
                                       left=True, labelleft=False, **kwargs)
             elif len(ax_) and direction == 'outer':  # no inner ticks
-                for a in ax_[1:]:
+                for a in ax_.iloc[1:]:
                     a.tick_params('y', left=False, labelleft=False, **kwargs)
             elif len(ax_) and direction is None:  # no ticks at all
                 for a in ax_:
                     a.tick_params('y', left=False, right=False,
                                   labelleft=False, labelright=False, **kwargs)
 
         # bottom and top ticks and labels
@@ -433,15 +433,15 @@
                                           bottom=True, labelbottom=False,
                                           **kwargs)
                             if a.position == 'diagonal':
                                 a.twin.tick_params('x', direction='inout',
                                                    bottom=True,
                                                    labelbottom=False, **kwargs)
                 elif direction == 'outer':  # no inner ticks
-                    for a in ax_[:-1]:
+                    for a in ax_.iloc[:-1]:
                         a.tick_params('x', bottom=False, labelbottom=False,
                                       **kwargs)
                 elif direction is None:  # no ticks at all
                     for a in ax_:
                         a.tick_params('x', bottom=False, top=False,
                                       labelbottom=False, labeltop=False,
                                       **kwargs)
@@ -609,15 +609,17 @@
     if 'tex' in fig_kw:
         raise NotImplementedError(
             "This is anesthetic 1.0 syntax. You need to update, e.g.\n"
             "make_1d_axes(..., tex=tex)     # anesthetic 1.0\n"
             "make_1d_axes(..., labels=tex)  # anesthetic 2.0"
             )
     fig = fig_kw.pop('fig') if 'fig' in fig_kw else plt.figure(**fig_kw)
-    axes = AxesSeries(index=np.atleast_1d(params),
+    if np.array(params).ndim == 0:
+        params = [params]
+    axes = AxesSeries(index=params,
                       fig=fig,
                       ncol=ncol,
                       labels=labels,
                       gridspec_kw=gridspec_kw,
                       subplot_spec=subplot_spec)
     if gridspec_kw is None:
         fig.tight_layout()
```

### Comparing `anesthetic-2.1.0/anesthetic/plotting/_core.py` & `anesthetic-2.1.1/anesthetic/plotting/_core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/plotting/_matplotlib/__init__.py` & `anesthetic-2.1.1/anesthetic/plotting/_matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/plotting/_matplotlib/boxplot.py` & `anesthetic-2.1.1/anesthetic/plotting/_matplotlib/boxplot.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/plotting/_matplotlib/core.py` & `anesthetic-2.1.1/anesthetic/plotting/_matplotlib/core.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/plotting/_matplotlib/hist.py` & `anesthetic-2.1.1/anesthetic/plotting/_matplotlib/hist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/read/chain.py` & `anesthetic-2.1.1/anesthetic/read/chain.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/read/cobaya.py` & `anesthetic-2.1.1/anesthetic/read/cobaya.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/read/getdist.py` & `anesthetic-2.1.1/anesthetic/read/getdist.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/read/hdf.py` & `anesthetic-2.1.1/anesthetic/read/hdf.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/read/multinest.py` & `anesthetic-2.1.1/anesthetic/read/multinest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/read/polychord.py` & `anesthetic-2.1.1/anesthetic/read/polychord.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/read/ultranest.py` & `anesthetic-2.1.1/anesthetic/read/ultranest.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/samples.py` & `anesthetic-2.1.1/anesthetic/samples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/scripts.py` & `anesthetic-2.1.1/anesthetic/scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/utils.py` & `anesthetic-2.1.1/anesthetic/utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic/weighted_pandas.py` & `anesthetic-2.1.1/anesthetic/weighted_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/anesthetic.egg-info/PKG-INFO` & `anesthetic-2.1.1/anesthetic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anesthetic
-Version: 2.1.0
+Version: 2.1.1
 Summary: nested sampling post-processing
 Author-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>, Adam Ormondroyd <ano23@cam.ac.uk>, Harry Bevins <htjb2@cam.ac.uk>, Johannes Buchner <jbuchner@mpe.mpg.de>, Ethan Carragher <ethan.carragher@adelaide.edu.au>, Andrew Fowlie <andrew.j.fowlie@googlemail.com>, Thomas Gessey-Jones <tg400@cam.ac.uk>, Stefan Heimersheim <sh2061@ast.cam.ac.uk>, Pablo Lemos <plemos91@gmail.com>, Toby Lovick <tcl44@cam.ac.uk>, Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>, Liangliang Su <liangliangsu@njnu.edu.cn>, David Yallup <david.yallup@gmail.com>
 Maintainer-email: Will Handley <williamjameshandley@gmail.com>, Lukas Hergt <lthergt@phas.ubc.ca>
 License: MIT License
         
         Copyright (c) 2019 Will Handley
         
@@ -55,15 +55,15 @@
 Provides-Extra: all
 License-File: LICENSE
 
 ===========================================
 anesthetic: nested sampling post-processing
 ===========================================
 :Authors: Will Handley and Lukas Hergt
-:Version: 2.1.0
+:Version: 2.1.1
 :Homepage: https://github.com/handley-lab/anesthetic
 :Documentation: http://anesthetic.readthedocs.io/
 
 .. image:: https://github.com/handley-lab/anesthetic/workflows/CI/badge.svg?branch=master
    :target: https://github.com/handley-lab/anesthetic/actions?query=workflow%3ACI+branch%3Amaster
    :alt: Build Status
 .. image:: https://codecov.io/gh/handley-lab/anesthetic/branch/master/graph/badge.svg
```

### Comparing `anesthetic-2.1.0/anesthetic.egg-info/SOURCES.txt` & `anesthetic-2.1.1/anesthetic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/pyproject.toml` & `anesthetic-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/tests/test_convert.py` & `anesthetic-2.1.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/tests/test_examples.py` & `anesthetic-2.1.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/tests/test_gui.py` & `anesthetic-2.1.1/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/tests/test_labelled_pandas.py` & `anesthetic-2.1.1/tests/test_labelled_pandas.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/tests/test_plot.py` & `anesthetic-2.1.1/tests/test_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,34 @@
     assert fig.get_figheight() == 5
 
     # Check unexpected kwargs
     with pytest.raises((AttributeError, TypeError)):
         make_1d_axes(paramnames, spam='ham')
 
 
+@pytest.mark.parametrize('params', [[0, 1, 2, 3],
+                                    [0, 2, 3],
+                                    [1, 2, 3],
+                                    ['x0', 'x1', 'x2'],
+                                    ['1', '2', '3'],
+                                    [0, 'x1', 'x2'],
+                                    ])
+def test_make_Nd_axes_integers(params):
+    fig, axes = make_1d_axes(params)
+    assert isinstance(fig, Figure)
+    assert isinstance(axes, AxesSeries)
+    assert list(axes.index) == params
+
+    fig, axes = make_2d_axes(params)
+    assert isinstance(fig, Figure)
+    assert isinstance(axes, AxesDataFrame)
+    assert list(axes.index) == params
+    assert list(axes.columns) == params
+
+
 def test_make_2d_axes_inputs_outputs():
     paramnames_x = ['A', 'B', 'C', 'D']
     paramnames_y = ['B', 'A', 'D', 'E']
 
     # 2D axes
     fig, axes = make_2d_axes([paramnames_x, paramnames_y])
     assert isinstance(fig, Figure)
```

### Comparing `anesthetic-2.1.0/tests/test_reader.py` & `anesthetic-2.1.1/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/tests/test_samples.py` & `anesthetic-2.1.1/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/tests/test_scripts.py` & `anesthetic-2.1.1/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/tests/test_utils.py` & `anesthetic-2.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `anesthetic-2.1.0/tests/test_weighted_pandas.py` & `anesthetic-2.1.1/tests/test_weighted_pandas.py`

 * *Files identical despite different names*

