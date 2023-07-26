# Comparing `tmp/sdypy_io_tdms-0.0.1.tar.gz` & `tmp/sdypy_io_tdms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdypy_io_tdms-0.0.1.tar", last modified: Wed Jul 26 13:36:38 2023, max compression
+gzip compressed data, was "sdypy_io_tdms-0.0.2.tar", last modified: Wed Jul 26 14:24:49 2023, max compression
```

## Comparing `sdypy_io_tdms-0.0.1.tar` & `sdypy_io_tdms-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:36:38.755792 sdypy_io_tdms-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-26 13:36:38.755792 sdypy_io_tdms-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-26 13:36:28.000000 sdypy_io_tdms-0.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:36:38.751792 sdypy_io_tdms-0.0.1/sdypy_io_tdms/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 13:36:28.000000 sdypy_io_tdms-0.0.1/sdypy_io_tdms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-26 13:36:28.000000 sdypy_io_tdms-0.0.1/sdypy_io_tdms/tdms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:36:38.755792 sdypy_io_tdms-0.0.1/sdypy_io_tdms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-26 13:36:38.000000 sdypy_io_tdms-0.0.1/sdypy_io_tdms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 13:36:38.000000 sdypy_io_tdms-0.0.1/sdypy_io_tdms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:36:38.000000 sdypy_io_tdms-0.0.1/sdypy_io_tdms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 13:36:38.000000 sdypy_io_tdms-0.0.1/sdypy_io_tdms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 13:36:38.755792 sdypy_io_tdms-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-26 13:36:28.000000 sdypy_io_tdms-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:36:38.755792 sdypy_io_tdms-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-26 13:36:28.000000 sdypy_io_tdms-0.0.1/tests/test_tdms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:24:49.170850 sdypy_io_tdms-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-26 14:24:49.170850 sdypy_io_tdms-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-26 14:24:35.000000 sdypy_io_tdms-0.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:24:49.166850 sdypy_io_tdms-0.0.2/sdypy_io_tdms/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-26 14:24:35.000000 sdypy_io_tdms-0.0.2/sdypy_io_tdms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-26 14:24:35.000000 sdypy_io_tdms-0.0.2/sdypy_io_tdms/tdms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:24:49.166850 sdypy_io_tdms-0.0.2/sdypy_io_tdms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-26 14:24:49.000000 sdypy_io_tdms-0.0.2/sdypy_io_tdms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-26 14:24:49.000000 sdypy_io_tdms-0.0.2/sdypy_io_tdms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:24:49.000000 sdypy_io_tdms-0.0.2/sdypy_io_tdms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 14:24:49.000000 sdypy_io_tdms-0.0.2/sdypy_io_tdms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:24:49.170850 sdypy_io_tdms-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-26 14:24:35.000000 sdypy_io_tdms-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:24:49.170850 sdypy_io_tdms-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-26 14:24:35.000000 sdypy_io_tdms-0.0.2/tests/test_tdms.py
```

### Comparing `sdypy_io_tdms-0.0.1/PKG-INFO` & `sdypy_io_tdms-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdypy_io_tdms
-Version: 0.0.1
+Version: 0.0.2
 Summary: TDMS file read and write functions compliant with SDyPy SEP5
 Home-page: https://github.com/sdypy
 Author: Wout Weijtjens
 Author-email: wout.weijtjens@vub.be
 Maintainer: Wout Weijtjens
 Maintainer-email: wout.weijtjens@vub.be
 License: MIT license
```

### Comparing `sdypy_io_tdms-0.0.1/sdypy_io_tdms/tdms.py` & `sdypy_io_tdms-0.0.2/sdypy_io_tdms/tdms.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,42 +19,46 @@
     if not os.path.isfile(path):
         warnings.warn("FAILED IMPORT: No TDMS file at: " + path, UserWarning)
         signals = []
         return signals
 
     try:
         tdms_file = TdmsFile(path)
-    except FileNotFoundError as fnf_error:
+    except FileNotFoundError:
         warnings.warn(
             f"FAILED IMPORT: No TDMS file at: {path}",
             UserWarning
         )
         signals = []
         return signals
-    except ValueError as val_error:
+    except ValueError:
         warnings.warn(
             f"FAILED IMPORT: TDMS file at: {path} seems corrupted. Failed to import.",
             UserWarning
         )
         signals = []
         return signals
 
     signals = []
     groups = tdms_file.groups()
 
     for group in groups:
         channels = tdms_file[group.name].channels()
         for channel in channels:
             signal = {}
-            signal['group'] = group
+            signal['group'] = group.name
             signal['name'] = str(channel).split("/")[2][1:-2]
             if "unit_string" in channel.properties:
                 unit_str = channel.properties["unit_string"]
             else:
                 unit_str = ""
             signal['unit_str'] = unit_str
             signal['data'] = tdms_file[group.name][channel.name].data
             signal['fs'] = 1 / channel.properties["wf_increment"]
-            signal['start_timestamp'] = np.datetime_as_string(channel.properties["wf_start_time"], unit='s')
+            if 'wf_start_time' in channel.properties:
+                signal['start_timestamp'] = np.datetime_as_string(
+                    channel.properties["wf_start_time"],
+                    unit='s'
+                )
             signals.append(signal)
 
-    return signals
+    return signals
```

### Comparing `sdypy_io_tdms-0.0.1/sdypy_io_tdms.egg-info/PKG-INFO` & `sdypy_io_tdms-0.0.2/sdypy_io_tdms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdypy-io-tdms
-Version: 0.0.1
+Version: 0.0.2
 Summary: TDMS file read and write functions compliant with SDyPy SEP5
 Home-page: https://github.com/sdypy
 Author: Wout Weijtjens
 Author-email: wout.weijtjens@vub.be
 Maintainer: Wout Weijtjens
 Maintainer-email: wout.weijtjens@vub.be
 License: MIT license
```

### Comparing `sdypy_io_tdms-0.0.1/setup.py` & `sdypy_io_tdms-0.0.2/setup.py`

 * *Files identical despite different names*

