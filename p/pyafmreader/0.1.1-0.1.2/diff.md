# Comparing `tmp/pyafmreader-0.1.1.tar.gz` & `tmp/pyafmreader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyafmreader-0.1.1.tar", last modified: Wed Jul 26 09:46:40 2023, max compression
+gzip compressed data, was "pyafmreader-0.1.2.tar", last modified: Wed Jul 26 10:07:35 2023, max compression
```

## Comparing `pyafmreader-0.1.1.tar` & `pyafmreader-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:40.660405 pyafmreader-0.1.1/
--rw-rw-rw-   0        0        0     1084 2023-07-26 08:55:15.000000 pyafmreader-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2335 2023-07-26 09:46:40.660405 pyafmreader-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      623 2023-07-26 09:46:08.000000 pyafmreader-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:40.538377 pyafmreader-0.1.1/pyafmreader/
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:40.594389 pyafmreader-0.1.1/pyafmreader/jpk/
--rw-rw-rw-   0        0        0      113 2023-03-10 20:18:56.000000 pyafmreader-0.1.1/pyafmreader/jpk/__init__.py
--rw-rw-rw-   0        0        0     6279 2023-04-26 09:25:11.000000 pyafmreader-0.1.1/pyafmreader/jpk/loadjpkcurve.py
--rw-rw-rw-   0        0        0     4593 2023-04-13 09:37:32.000000 pyafmreader-0.1.1/pyafmreader/jpk/loadjpkfile.py
--rw-rw-rw-   0        0        0     6673 2023-04-14 07:46:03.000000 pyafmreader-0.1.1/pyafmreader/jpk/loadjpkimg.py
--rw-rw-rw-   0        0        0     2809 2023-03-10 20:18:56.000000 pyafmreader-0.1.1/pyafmreader/jpk/loadjpkthermalfile.py
--rw-rw-rw-   0        0        0    16785 2023-04-13 09:04:54.000000 pyafmreader-0.1.1/pyafmreader/jpk/parsejpkheader.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:40.618396 pyafmreader-0.1.1/pyafmreader/nanosc/
--rw-rw-rw-   0        0        0      125 2023-03-10 20:18:56.000000 pyafmreader-0.1.1/pyafmreader/nanosc/__init__.py
--rw-rw-rw-   0        0        0     5946 2023-03-10 20:18:56.000000 pyafmreader-0.1.1/pyafmreader/nanosc/loadnanosccurve.py
--rw-rw-rw-   0        0        0      676 2023-03-10 20:18:56.000000 pyafmreader-0.1.1/pyafmreader/nanosc/loadnanoscfile.py
--rw-rw-rw-   0        0        0     1577 2023-03-10 20:18:56.000000 pyafmreader-0.1.1/pyafmreader/nanosc/loadnanoscimg.py
--rw-rw-rw-   0        0        0    10626 2023-03-10 20:18:56.000000 pyafmreader-0.1.1/pyafmreader/nanosc/parsenanoscheader.py
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:40.640399 pyafmreader-0.1.1/pyafmreader/pyafmreader.egg-info/
--rw-rw-rw-   0        0        0     2335 2023-07-26 09:46:40.000000 pyafmreader-0.1.1/pyafmreader/pyafmreader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-07-26 09:46:40.000000 pyafmreader-0.1.1/pyafmreader/pyafmreader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 09:46:40.000000 pyafmreader-0.1.1/pyafmreader/pyafmreader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 09:46:40.000000 pyafmreader-0.1.1/pyafmreader/pyafmreader.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:40.650401 pyafmreader-0.1.1/pyafmreader/utils/
--rw-rw-rw-   0        0        0        0 2023-03-10 20:18:56.000000 pyafmreader-0.1.1/pyafmreader/utils/__init__.py
--rw-rw-rw-   0        0        0     4073 2023-03-10 20:18:56.000000 pyafmreader-0.1.1/pyafmreader/utils/forcecurve.py
--rw-rw-rw-   0        0        0     5959 2023-03-10 20:18:56.000000 pyafmreader-0.1.1/pyafmreader/utils/segment.py
--rw-rw-rw-   0        0        0      113 2023-07-26 09:46:03.000000 pyafmreader-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      777 2023-07-26 09:46:40.670406 pyafmreader-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 09:46:40.655404 pyafmreader-0.1.1/tests/
--rw-rw-rw-   0        0        0    11279 2023-07-26 07:43:48.000000 pyafmreader-0.1.1/tests/test_pyafmreader.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:07:35.647467 pyafmreader-0.1.2/
+-rw-rw-rw-   0        0        0     1084 2023-07-26 08:55:15.000000 pyafmreader-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2335 2023-07-26 10:07:35.647467 pyafmreader-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      623 2023-07-26 10:06:35.000000 pyafmreader-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 10:07:35.533441 pyafmreader-0.1.2/pyafmreader/
+drwxrwxrwx   0        0        0        0 2023-07-26 10:07:35.587454 pyafmreader-0.1.2/pyafmreader/jpk/
+-rw-rw-rw-   0        0        0      113 2023-03-10 20:18:56.000000 pyafmreader-0.1.2/pyafmreader/jpk/__init__.py
+-rw-rw-rw-   0        0        0     6279 2023-04-26 09:25:11.000000 pyafmreader-0.1.2/pyafmreader/jpk/loadjpkcurve.py
+-rw-rw-rw-   0        0        0     4593 2023-04-13 09:37:32.000000 pyafmreader-0.1.2/pyafmreader/jpk/loadjpkfile.py
+-rw-rw-rw-   0        0        0     6673 2023-04-14 07:46:03.000000 pyafmreader-0.1.2/pyafmreader/jpk/loadjpkimg.py
+-rw-rw-rw-   0        0        0     2809 2023-03-10 20:18:56.000000 pyafmreader-0.1.2/pyafmreader/jpk/loadjpkthermalfile.py
+-rw-rw-rw-   0        0        0    16785 2023-04-13 09:04:54.000000 pyafmreader-0.1.2/pyafmreader/jpk/parsejpkheader.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:07:35.609458 pyafmreader-0.1.2/pyafmreader/nanosc/
+-rw-rw-rw-   0        0        0      125 2023-03-10 20:18:56.000000 pyafmreader-0.1.2/pyafmreader/nanosc/__init__.py
+-rw-rw-rw-   0        0        0     5946 2023-03-10 20:18:56.000000 pyafmreader-0.1.2/pyafmreader/nanosc/loadnanosccurve.py
+-rw-rw-rw-   0        0        0      676 2023-03-10 20:18:56.000000 pyafmreader-0.1.2/pyafmreader/nanosc/loadnanoscfile.py
+-rw-rw-rw-   0        0        0     1577 2023-03-10 20:18:56.000000 pyafmreader-0.1.2/pyafmreader/nanosc/loadnanoscimg.py
+-rw-rw-rw-   0        0        0    10626 2023-03-10 20:18:56.000000 pyafmreader-0.1.2/pyafmreader/nanosc/parsenanoscheader.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:07:35.629463 pyafmreader-0.1.2/pyafmreader/pyafmreader.egg-info/
+-rw-rw-rw-   0        0        0     2335 2023-07-26 10:07:35.000000 pyafmreader-0.1.2/pyafmreader/pyafmreader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-07-26 10:07:35.000000 pyafmreader-0.1.2/pyafmreader/pyafmreader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 10:07:35.000000 pyafmreader-0.1.2/pyafmreader/pyafmreader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 10:07:35.000000 pyafmreader-0.1.2/pyafmreader/pyafmreader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 10:07:35.637465 pyafmreader-0.1.2/pyafmreader/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-10 20:18:56.000000 pyafmreader-0.1.2/pyafmreader/utils/__init__.py
+-rw-rw-rw-   0        0        0     4073 2023-03-10 20:18:56.000000 pyafmreader-0.1.2/pyafmreader/utils/forcecurve.py
+-rw-rw-rw-   0        0        0     5959 2023-03-10 20:18:56.000000 pyafmreader-0.1.2/pyafmreader/utils/segment.py
+-rw-rw-rw-   0        0        0      113 2023-07-26 09:46:03.000000 pyafmreader-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      777 2023-07-26 10:07:35.654469 pyafmreader-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 10:07:35.642466 pyafmreader-0.1.2/tests/
+-rw-rw-rw-   0        0        0    11279 2023-07-26 07:43:48.000000 pyafmreader-0.1.2/tests/test_pyafmreader.py
```

### Comparing `pyafmreader-0.1.1/LICENSE.txt` & `pyafmreader-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/PKG-INFO` & `pyafmreader-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyafmreader
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package to read Nanoscope and JPK AFM files.
 Home-page: https://github.com/jlopezalo/PyFMReader
 Author: Javier Lopez Alonso
 Author-email: jla.lopez.18@gmail.com
 Project-URL: Bug Tracker, https://github.com/jlopezalo/PyFMReader/issues
 Project-URL: repository, https://github.com/jlopezalo/PyFMReader
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Pyafmreader V.0.1.1
+# Pyafmreader V.0.1.2
 
 In development, not fully stable.
 If you find any issues please open an issue at:
 https://github.com/jlopezalo/PyFMReader/issues
 
 If you have any questions, contact:
 jla.lopez.18@gmail.com
```

### Comparing `pyafmreader-0.1.1/README.md` & `pyafmreader-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Pyafmreader V.0.1.1
+# Pyafmreader V.0.1.2
 
 In development, not fully stable.
 If you find any issues please open an issue at:
 https://github.com/jlopezalo/PyFMReader/issues
 
 If you have any questions, contact:
 jla.lopez.18@gmail.com
```

### Comparing `pyafmreader-0.1.1/pyafmreader/jpk/loadjpkcurve.py` & `pyafmreader-0.1.2/pyafmreader/jpk/loadjpkcurve.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/jpk/loadjpkfile.py` & `pyafmreader-0.1.2/pyafmreader/jpk/loadjpkfile.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/jpk/loadjpkimg.py` & `pyafmreader-0.1.2/pyafmreader/jpk/loadjpkimg.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/jpk/loadjpkthermalfile.py` & `pyafmreader-0.1.2/pyafmreader/jpk/loadjpkthermalfile.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/jpk/parsejpkheader.py` & `pyafmreader-0.1.2/pyafmreader/jpk/parsejpkheader.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/nanosc/loadnanosccurve.py` & `pyafmreader-0.1.2/pyafmreader/nanosc/loadnanosccurve.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/nanosc/loadnanoscfile.py` & `pyafmreader-0.1.2/pyafmreader/nanosc/loadnanoscfile.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/nanosc/loadnanoscimg.py` & `pyafmreader-0.1.2/pyafmreader/nanosc/loadnanoscimg.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/nanosc/parsenanoscheader.py` & `pyafmreader-0.1.2/pyafmreader/nanosc/parsenanoscheader.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/pyafmreader.egg-info/PKG-INFO` & `pyafmreader-0.1.2/pyafmreader/pyafmreader.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pyafmreader
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package to read Nanoscope and JPK AFM files.
 Home-page: https://github.com/jlopezalo/PyFMReader
 Author: Javier Lopez Alonso
 Author-email: jla.lopez.18@gmail.com
 Project-URL: Bug Tracker, https://github.com/jlopezalo/PyFMReader/issues
 Project-URL: repository, https://github.com/jlopezalo/PyFMReader
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# Pyafmreader V.0.1.1
+# Pyafmreader V.0.1.2
 
 In development, not fully stable.
 If you find any issues please open an issue at:
 https://github.com/jlopezalo/PyFMReader/issues
 
 If you have any questions, contact:
 jla.lopez.18@gmail.com
```

### Comparing `pyafmreader-0.1.1/pyafmreader/pyafmreader.egg-info/SOURCES.txt` & `pyafmreader-0.1.2/pyafmreader/pyafmreader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/utils/forcecurve.py` & `pyafmreader-0.1.2/pyafmreader/utils/forcecurve.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/pyafmreader/utils/segment.py` & `pyafmreader-0.1.2/pyafmreader/utils/segment.py`

 * *Files identical despite different names*

### Comparing `pyafmreader-0.1.1/setup.cfg` & `pyafmreader-0.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7961 666d 7265 6164 6572 0d0a   = pyafmreader..
-00000020: 7665 7273 696f 6e20 3d20 302e 312e 310d  version = 0.1.1.
+00000020: 7665 7273 696f 6e20 3d20 302e 312e 320d  version = 0.1.2.
 00000030: 0a61 7574 686f 7220 3d20 4a61 7669 6572  .author = Javier
 00000040: 204c 6f70 657a 2041 6c6f 6e73 6f0d 0a61   Lopez Alonso..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 6a6c  uthor_email = jl
 00000060: 612e 6c6f 7065 7a2e 3138 4067 6d61 696c  a.lopez.18@gmail
 00000070: 2e63 6f6d 0d0a 6465 7363 7269 7074 696f  .com..descriptio
 00000080: 6e20 3d20 4120 7079 7468 6f6e 2070 6163  n = A python pac
 00000090: 6b61 6765 2074 6f20 7265 6164 204e 616e  kage to read Nan
```

### Comparing `pyafmreader-0.1.1/tests/test_pyafmreader.py` & `pyafmreader-0.1.2/tests/test_pyafmreader.py`

 * *Files identical despite different names*

