# Comparing `tmp/actipy-2.1.0.tar.gz` & `tmp/actipy-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actipy-2.1.0.tar", last modified: Tue Jun 27 17:25:16 2023, max compression
+gzip compressed data, was "actipy-2.1.1.tar", last modified: Tue Jul 25 22:05:17 2023, max compression
```

## Comparing `actipy-2.1.0.tar` & `actipy-2.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:25:16.191441 actipy-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-06-27 17:25:01.000000 actipy-2.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-27 17:25:01.000000 actipy-2.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-27 17:25:16.191441 actipy-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-27 17:25:01.000000 actipy-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-27 17:25:01.000000 actipy-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:25:16.191441 actipy-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-27 17:25:01.000000 actipy-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:25:16.183441 actipy-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:25:16.191441 actipy-2.1.0/src/actipy/
--rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-06-27 17:25:06.000000 actipy-2.1.0/src/actipy/ActigraphReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/ActigraphReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-06-27 17:25:06.000000 actipy-2.1.0/src/actipy/AxivityReader.class
--rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/AxivityReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-27 17:25:06.000000 actipy-2.1.0/src/actipy/GENEActivReader.class
--rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/GENEActivReader.java
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-06-27 17:25:06.000000 actipy-2.1.0/src/actipy/NpyWriter.class
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/NpyWriter.java
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-27 17:25:16.191441 actipy-2.1.0/src/actipy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-06-27 17:25:01.000000 actipy-2.1.0/src/actipy/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:25:16.191441 actipy-2.1.0/src/actipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-27 17:25:16.000000 actipy-2.1.0/src/actipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-27 17:25:16.000000 actipy-2.1.0/src/actipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:25:16.000000 actipy-2.1.0/src/actipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-27 17:25:16.000000 actipy-2.1.0/src/actipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 17:25:16.000000 actipy-2.1.0/src/actipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-27 17:25:01.000000 actipy-2.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:05:17.366103 actipy-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-07-25 22:04:58.000000 actipy-2.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 22:04:58.000000 actipy-2.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-25 22:05:17.366103 actipy-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-25 22:04:58.000000 actipy-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-07-25 22:04:58.000000 actipy-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 22:05:17.366103 actipy-2.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-25 22:04:58.000000 actipy-2.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:05:17.362103 actipy-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:05:17.366103 actipy-2.1.1/src/actipy/
+-rw-r--r--   0 runner    (1001) docker     (123)    11517 2023-07-25 22:05:03.000000 actipy-2.1.1/src/actipy/ActigraphReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    30928 2023-07-25 22:04:58.000000 actipy-2.1.1/src/actipy/ActigraphReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-07-25 22:05:03.000000 actipy-2.1.1/src/actipy/AxivityReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-07-25 22:04:58.000000 actipy-2.1.1/src/actipy/AxivityReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-07-25 22:05:03.000000 actipy-2.1.1/src/actipy/GENEActivReader.class
+-rw-r--r--   0 runner    (1001) docker     (123)     9656 2023-07-25 22:04:58.000000 actipy-2.1.1/src/actipy/GENEActivReader.java
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-25 22:05:03.000000 actipy-2.1.1/src/actipy/NpyWriter.class
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-07-25 22:04:58.000000 actipy-2.1.1/src/actipy/NpyWriter.java
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-25 22:04:58.000000 actipy-2.1.1/src/actipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-25 22:05:17.366103 actipy-2.1.1/src/actipy/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14795 2023-07-25 22:04:58.000000 actipy-2.1.1/src/actipy/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-07-25 22:04:58.000000 actipy-2.1.1/src/actipy/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 22:05:17.366103 actipy-2.1.1/src/actipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-25 22:05:17.000000 actipy-2.1.1/src/actipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-25 22:05:17.000000 actipy-2.1.1/src/actipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 22:05:17.000000 actipy-2.1.1/src/actipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-25 22:05:17.000000 actipy-2.1.1/src/actipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 22:05:17.000000 actipy-2.1.1/src/actipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-25 22:04:58.000000 actipy-2.1.1/versioneer.py
```

### Comparing `actipy-2.1.0/LICENSE.md` & `actipy-2.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/PKG-INFO` & `actipy-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actipy
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python package to process wearable accelerometer data
 Home-page: https://github.com/OxWearables/actipy
 Download-URL: https://github.com/OxWearables/actipy
 Author: Shing Chan, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
```

### Comparing `actipy-2.1.0/README.md` & `actipy-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/pyproject.toml` & `actipy-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/setup.py` & `actipy-2.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             "autopep8",
             "ipython",
             "ipdb",
             "memory-profiler",
             "twine",
             "tomli",
             "pytest",
+            "joblib",
         ],
         "docs": [
             "sphinx>=4.2",
             "sphinx_rtd_theme>=1.0",
             "readthedocs-sphinx-search>=0.1",
             "docutils<0.18",
         ]
```

### Comparing `actipy-2.1.0/src/actipy/ActigraphReader.class` & `actipy-2.1.1/src/actipy/ActigraphReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/src/actipy/ActigraphReader.java` & `actipy-2.1.1/src/actipy/ActigraphReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/src/actipy/AxivityReader.class` & `actipy-2.1.1/src/actipy/AxivityReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/src/actipy/AxivityReader.java` & `actipy-2.1.1/src/actipy/AxivityReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/src/actipy/GENEActivReader.class` & `actipy-2.1.1/src/actipy/GENEActivReader.class`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/src/actipy/GENEActivReader.java` & `actipy-2.1.1/src/actipy/GENEActivReader.java`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/src/actipy/NpyWriter.class` & `actipy-2.1.1/src/actipy/NpyWriter.class`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/src/actipy/NpyWriter.java` & `actipy-2.1.1/src/actipy/NpyWriter.java`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/src/actipy/processing.py` & `actipy-2.1.1/src/actipy/processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,32 +165,40 @@
     """
 
     info = {}
 
     if stationary_indicator is None:
         stationary_indicator = get_stationary_indicator(data)
 
-    # The paper uses 10sec averages instead of the raw ticks.
-    # This reduces computational cost. Also reduces influence of outliers.
-    stationary_data = (data[stationary_indicator]
-                       .resample('10s')
-                       .mean()
-                       .dropna())
+    xyz = (data.loc[stationary_indicator, ['x', 'y', 'z']]
+           .resample('10s')
+           .mean()
+           .to_numpy())
 
-    hasT = 'temperature' in stationary_data
-
-    xyz = stationary_data[['x', 'y', 'z']].to_numpy()
     # Remove any nonzero vectors as they cause nan issues
     nonzero = np.linalg.norm(xyz, axis=1) > 1e-8
     xyz = xyz[nonzero]
+
+    hasT = 'temperature' in data
     if hasT:
-        T = stationary_data['temperature'].to_numpy()
+        T = (data.loc[stationary_indicator, 'temperature']
+             .resample('10s')
+             .mean()
+             .to_numpy())
         T = T[nonzero]
-    del stationary_data
+
+    # Remove any nans
+    na = np.isnan(xyz).any(1)
+    if hasT:
+        na = na | np.isnan(T)
+        T = T[~na]
+    xyz = xyz[~na]
+
     del nonzero
+    del na
 
     if len(xyz) < calib_min_samples:
         info['CalibOK'] = 0
         info['CalibErrorBefore(mg)'] = np.nan
         info['CalibErrorAfter(mg)'] = np.nan
         warnings.warn(f"Skipping calibration: Insufficient stationary samples")
         return data, info
```

### Comparing `actipy-2.1.0/src/actipy/reader.py` & `actipy-2.1.1/src/actipy/reader.py`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/src/actipy.egg-info/PKG-INFO` & `actipy-2.1.1/src/actipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actipy
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python package to process wearable accelerometer data
 Home-page: https://github.com/OxWearables/actipy
 Download-URL: https://github.com/OxWearables/actipy
 Author: Shing Chan, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE.md
```

### Comparing `actipy-2.1.0/src/actipy.egg-info/SOURCES.txt` & `actipy-2.1.1/src/actipy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actipy-2.1.0/versioneer.py` & `actipy-2.1.1/versioneer.py`

 * *Files identical despite different names*

