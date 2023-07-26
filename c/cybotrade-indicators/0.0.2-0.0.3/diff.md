# Comparing `tmp/cybotrade-indicators-0.0.2.tar.gz` & `tmp/cybotrade_indicators-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybotrade-indicators-0.0.2.tar", last modified: Wed Jul 26 02:49:01 2023, max compression
+gzip compressed data, was "cybotrade-indicators-0.0.3.tar", last modified: Wed Jul 26 03:01:12 2023, max compression
```

## Comparing `cybotrade-indicators-0.0.2.tar` & `cybotrade_indicators-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 02:49:01.811987 cybotrade-indicators-0.0.2/
--rw-r--r--   0 marcus     (501) staff       (20)      433 2023-07-25 20:08:51.000000 cybotrade-indicators-0.0.2/AUTHORS
--rw-r--r--   0 marcus     (501) staff       (20)     7650 2023-07-25 20:08:38.000000 cybotrade-indicators-0.0.2/LICENSE
--rw-r--r--   0 marcus     (501) staff       (20)      198 2023-07-25 20:25:04.000000 cybotrade-indicators-0.0.2/MANIFEST.in
--rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-07-26 02:49:01.811850 cybotrade-indicators-0.0.2/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)     2818 2023-07-25 20:06:26.000000 cybotrade-indicators-0.0.2/README.md
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 02:49:01.802148 cybotrade-indicators-0.0.2/external/
--rw-r--r--   0 marcus     (501) staff       (20)    53547 2023-07-25 10:32:29.000000 cybotrade-indicators-0.0.2/external/indicators.h
--rw-r--r--   0 marcus     (501) staff       (20)   419800 2023-07-25 10:32:24.000000 cybotrade-indicators-0.0.2/external/tiamalgamation.c
--rw-r--r--   0 marcus     (501) staff       (20)      920 2023-07-26 02:48:19.000000 cybotrade-indicators-0.0.2/pyproject.toml
--rw-r--r--   0 marcus     (501) staff       (20)       38 2023-07-26 02:49:01.812030 cybotrade-indicators-0.0.2/setup.cfg
--rw-r--r--   0 marcus     (501) staff       (20)      370 2023-07-25 19:18:28.000000 cybotrade-indicators-0.0.2/setup.py
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 02:49:01.800063 cybotrade-indicators-0.0.2/src/
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 02:49:01.810109 cybotrade-indicators-0.0.2/src/cybotrade_indicators/
--rw-r--r--   0 marcus     (501) staff       (20)  4146314 2023-07-26 02:34:36.000000 cybotrade-indicators-0.0.2/src/cybotrade_indicators/__init__.c
--rw-r--r--   0 marcus     (501) staff       (20)    24376 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.2/src/cybotrade_indicators/__init__.pyi
--rw-r--r--   0 marcus     (501) staff       (20)     1817 2023-07-25 19:17:58.000000 cybotrade-indicators-0.0.2/src/cybotrade_indicators/indicators.pxd
--rw-r--r--   0 marcus     (501) staff       (20)        0 2023-07-25 20:15:15.000000 cybotrade-indicators-0.0.2/src/cybotrade_indicators/py.typed
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 02:49:01.810714 cybotrade-indicators-0.0.2/src/cybotrade_indicators.egg-info/
--rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-07-26 02:49:01.000000 cybotrade-indicators-0.0.2/src/cybotrade_indicators.egg-info/PKG-INFO
--rw-r--r--   0 marcus     (501) staff       (20)      510 2023-07-26 02:49:01.000000 cybotrade-indicators-0.0.2/src/cybotrade_indicators.egg-info/SOURCES.txt
--rw-r--r--   0 marcus     (501) staff       (20)        1 2023-07-26 02:49:01.000000 cybotrade-indicators-0.0.2/src/cybotrade_indicators.egg-info/dependency_links.txt
--rw-r--r--   0 marcus     (501) staff       (20)       30 2023-07-26 02:49:01.000000 cybotrade-indicators-0.0.2/src/cybotrade_indicators.egg-info/requires.txt
--rw-r--r--   0 marcus     (501) staff       (20)       21 2023-07-26 02:49:01.000000 cybotrade-indicators-0.0.2/src/cybotrade_indicators.egg-info/top_level.txt
-drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 02:49:01.810840 cybotrade-indicators-0.0.2/tests/
--rw-r--r--   0 marcus     (501) staff       (20)     2219 2023-07-25 19:35:10.000000 cybotrade-indicators-0.0.2/tests/test.py
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.230521 cybotrade-indicators-0.0.3/
+-rw-r--r--   0 marcus     (501) staff       (20)      433 2023-07-25 20:08:51.000000 cybotrade-indicators-0.0.3/AUTHORS
+-rw-r--r--   0 marcus     (501) staff       (20)     7650 2023-07-25 20:08:38.000000 cybotrade-indicators-0.0.3/LICENSE
+-rw-r--r--   0 marcus     (501) staff       (20)      238 2023-07-26 03:00:01.000000 cybotrade-indicators-0.0.3/MANIFEST.in
+-rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-07-26 03:01:12.230386 cybotrade-indicators-0.0.3/PKG-INFO
+-rw-r--r--   0 marcus     (501) staff       (20)     2818 2023-07-25 20:06:26.000000 cybotrade-indicators-0.0.3/README.md
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.221196 cybotrade-indicators-0.0.3/external/
+-rw-r--r--   0 marcus     (501) staff       (20)    53547 2023-07-25 10:32:29.000000 cybotrade-indicators-0.0.3/external/indicators.h
+-rw-r--r--   0 marcus     (501) staff       (20)   419800 2023-07-25 10:32:24.000000 cybotrade-indicators-0.0.3/external/tiamalgamation.c
+-rw-r--r--   0 marcus     (501) staff       (20)      920 2023-07-26 03:01:07.000000 cybotrade-indicators-0.0.3/pyproject.toml
+-rw-r--r--   0 marcus     (501) staff       (20)       38 2023-07-26 03:01:12.230574 cybotrade-indicators-0.0.3/setup.cfg
+-rw-r--r--   0 marcus     (501) staff       (20)      370 2023-07-25 19:18:28.000000 cybotrade-indicators-0.0.3/setup.py
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.219386 cybotrade-indicators-0.0.3/src/
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.228563 cybotrade-indicators-0.0.3/src/cybotrade_indicators/
+-rw-r--r--   0 marcus     (501) staff       (20)  4146314 2023-07-26 02:34:36.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.c
+-rw-r--r--   0 marcus     (501) staff       (20)    24376 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.pyi
+-rw-r--r--   0 marcus     (501) staff       (20)    56715 2023-07-25 19:55:33.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.pyx
+-rw-r--r--   0 marcus     (501) staff       (20)     1817 2023-07-25 19:17:58.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators/indicators.pxd
+-rw-r--r--   0 marcus     (501) staff       (20)        0 2023-07-25 20:15:15.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators/py.typed
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.229211 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/
+-rw-r--r--   0 marcus     (501) staff       (20)     3493 2023-07-26 03:01:12.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/PKG-INFO
+-rw-r--r--   0 marcus     (501) staff       (20)      548 2023-07-26 03:01:12.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/SOURCES.txt
+-rw-r--r--   0 marcus     (501) staff       (20)        1 2023-07-26 03:01:12.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/dependency_links.txt
+-rw-r--r--   0 marcus     (501) staff       (20)       30 2023-07-26 03:01:12.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/requires.txt
+-rw-r--r--   0 marcus     (501) staff       (20)       21 2023-07-26 03:01:12.000000 cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/top_level.txt
+drwxr-xr-x   0 marcus     (501) staff       (20)        0 2023-07-26 03:01:12.229343 cybotrade-indicators-0.0.3/tests/
+-rw-r--r--   0 marcus     (501) staff       (20)     2219 2023-07-25 19:35:10.000000 cybotrade-indicators-0.0.3/tests/test.py
```

### Comparing `cybotrade-indicators-0.0.2/LICENSE` & `cybotrade-indicators-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.2/PKG-INFO` & `cybotrade-indicators-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybotrade-indicators
-Version: 0.0.2
+Version: 0.0.3
 Summary: This library provides a set of technical analysis indicators that can be used to craft trading strategies.
 Author-email: Marcus Lee <marcuslee@balaenaquant.com>, Lee Ze Lim <zelim@balaenaquant.com>
 Project-URL: Homepage, https://app.cybotrade.rs
 Project-URL: Documentation, https://docs.cybotrade.rs
 Project-URL: Repository, https://github.com/cybotrade/cybotrade-indicators
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cybotrade-indicators-0.0.2/README.md` & `cybotrade-indicators-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.2/external/indicators.h` & `cybotrade-indicators-0.0.3/external/indicators.h`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.2/external/tiamalgamation.c` & `cybotrade-indicators-0.0.3/external/tiamalgamation.c`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.2/pyproject.toml` & `cybotrade-indicators-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [project]
 name = "cybotrade-indicators"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Marcus Lee", email = "marcuslee@balaenaquant.com" },
     { name = "Lee Ze Lim", email = "zelim@balaenaquant.com" },
 ]
 description = "This library provides a set of technical analysis indicators that can be used to craft trading strategies."
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `cybotrade-indicators-0.0.2/src/cybotrade_indicators/__init__.c` & `cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.c`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.2/src/cybotrade_indicators/__init__.pyi` & `cybotrade-indicators-0.0.3/src/cybotrade_indicators/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.2/src/cybotrade_indicators/indicators.pxd` & `cybotrade-indicators-0.0.3/src/cybotrade_indicators/indicators.pxd`

 * *Files identical despite different names*

### Comparing `cybotrade-indicators-0.0.2/src/cybotrade_indicators.egg-info/PKG-INFO` & `cybotrade-indicators-0.0.3/src/cybotrade_indicators.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybotrade-indicators
-Version: 0.0.2
+Version: 0.0.3
 Summary: This library provides a set of technical analysis indicators that can be used to craft trading strategies.
 Author-email: Marcus Lee <marcuslee@balaenaquant.com>, Lee Ze Lim <zelim@balaenaquant.com>
 Project-URL: Homepage, https://app.cybotrade.rs
 Project-URL: Documentation, https://docs.cybotrade.rs
 Project-URL: Repository, https://github.com/cybotrade/cybotrade-indicators
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cybotrade-indicators-0.0.2/tests/test.py` & `cybotrade-indicators-0.0.3/tests/test.py`

 * *Files identical despite different names*

