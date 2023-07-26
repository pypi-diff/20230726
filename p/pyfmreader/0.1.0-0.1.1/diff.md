# Comparing `tmp/pyfmreader-0.1.0.tar.gz` & `tmp/pyfmreader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmreader-0.1.0.tar", last modified: Wed Jul 26 10:35:58 2023, max compression
+gzip compressed data, was "pyfmreader-0.1.1.tar", last modified: Wed Jul 26 10:57:57 2023, max compression
```

## Comparing `pyfmreader-0.1.0.tar` & `pyfmreader-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 10:35:58.600928 pyfmreader-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-07-26 08:55:15.000000 pyfmreader-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2331 2023-07-26 10:35:58.600928 pyfmreader-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      620 2023-07-26 10:31:22.000000 pyfmreader-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 10:35:58.415042 pyfmreader-0.1.0/pyfmreader/
-drwxrwxrwx   0        0        0        0 2023-07-26 10:35:58.496920 pyfmreader-0.1.0/pyfmreader/jpk/
--rw-rw-rw-   0        0        0      113 2023-03-10 20:18:56.000000 pyfmreader-0.1.0/pyfmreader/jpk/__init__.py
--rw-rw-rw-   0        0        0     6279 2023-04-26 09:25:11.000000 pyfmreader-0.1.0/pyfmreader/jpk/loadjpkcurve.py
--rw-rw-rw-   0        0        0     4593 2023-04-13 09:37:32.000000 pyfmreader-0.1.0/pyfmreader/jpk/loadjpkfile.py
--rw-rw-rw-   0        0        0     6672 2023-07-26 10:32:30.000000 pyfmreader-0.1.0/pyfmreader/jpk/loadjpkimg.py
--rw-rw-rw-   0        0        0     2809 2023-03-10 20:18:56.000000 pyfmreader-0.1.0/pyfmreader/jpk/loadjpkthermalfile.py
--rw-rw-rw-   0        0        0    16785 2023-04-13 09:04:54.000000 pyfmreader-0.1.0/pyfmreader/jpk/parsejpkheader.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:35:58.528917 pyfmreader-0.1.0/pyfmreader/nanosc/
--rw-rw-rw-   0        0        0      125 2023-03-10 20:18:56.000000 pyfmreader-0.1.0/pyfmreader/nanosc/__init__.py
--rw-rw-rw-   0        0        0     5946 2023-03-10 20:18:56.000000 pyfmreader-0.1.0/pyfmreader/nanosc/loadnanosccurve.py
--rw-rw-rw-   0        0        0      676 2023-03-10 20:18:56.000000 pyfmreader-0.1.0/pyfmreader/nanosc/loadnanoscfile.py
--rw-rw-rw-   0        0        0     1577 2023-03-10 20:18:56.000000 pyfmreader-0.1.0/pyfmreader/nanosc/loadnanoscimg.py
--rw-rw-rw-   0        0        0    10626 2023-03-10 20:18:56.000000 pyfmreader-0.1.0/pyfmreader/nanosc/parsenanoscheader.py
-drwxrwxrwx   0        0        0        0 2023-07-26 10:35:58.568923 pyfmreader-0.1.0/pyfmreader/pyfmreader.egg-info/
--rw-rw-rw-   0        0        0     2331 2023-07-26 10:35:58.000000 pyfmreader-0.1.0/pyfmreader/pyfmreader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      704 2023-07-26 10:35:58.000000 pyfmreader-0.1.0/pyfmreader/pyfmreader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 10:35:58.000000 pyfmreader-0.1.0/pyfmreader/pyfmreader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 10:35:58.000000 pyfmreader-0.1.0/pyfmreader/pyfmreader.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 10:35:58.584924 pyfmreader-0.1.0/pyfmreader/utils/
--rw-rw-rw-   0        0        0        0 2023-03-10 20:18:56.000000 pyfmreader-0.1.0/pyfmreader/utils/__init__.py
--rw-rw-rw-   0        0        0     4073 2023-03-10 20:18:56.000000 pyfmreader-0.1.0/pyfmreader/utils/forcecurve.py
--rw-rw-rw-   0        0        0     5959 2023-03-10 20:18:56.000000 pyfmreader-0.1.0/pyfmreader/utils/segment.py
--rw-rw-rw-   0        0        0      250 2023-07-26 10:34:49.000000 pyfmreader-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      774 2023-07-26 10:35:58.608926 pyfmreader-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 10:35:58.592925 pyfmreader-0.1.0/tests/
--rw-rw-rw-   0        0        0    11278 2023-07-26 10:32:52.000000 pyfmreader-0.1.0/tests/test_pyafmreader.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:57.849693 pyfmreader-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-07-26 08:55:15.000000 pyfmreader-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2331 2023-07-26 10:57:57.849693 pyfmreader-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      620 2023-07-26 10:31:22.000000 pyfmreader-0.1.1/README.md
+-rw-rw-rw-   0        0        0      243 2023-07-26 10:56:28.000000 pyfmreader-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      760 2023-07-26 10:57:57.857706 pyfmreader-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:57.659116 pyfmreader-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:57.729681 pyfmreader-0.1.1/src/pyfmreader/
+-rw-rw-rw-   0        0        0      121 2023-07-26 10:55:40.000000 pyfmreader-0.1.1/src/pyfmreader/__init__.py
+-rw-rw-rw-   0        0        0     1508 2023-07-26 10:09:41.000000 pyfmreader-0.1.1/src/pyfmreader/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:57.793691 pyfmreader-0.1.1/src/pyfmreader/jpk/
+-rw-rw-rw-   0        0        0      113 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/jpk/__init__.py
+-rw-rw-rw-   0        0        0     6279 2023-04-26 09:25:11.000000 pyfmreader-0.1.1/src/pyfmreader/jpk/loadjpkcurve.py
+-rw-rw-rw-   0        0        0     4593 2023-04-13 09:37:32.000000 pyfmreader-0.1.1/src/pyfmreader/jpk/loadjpkfile.py
+-rw-rw-rw-   0        0        0     6672 2023-07-26 10:32:30.000000 pyfmreader-0.1.1/src/pyfmreader/jpk/loadjpkimg.py
+-rw-rw-rw-   0        0        0     2809 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/jpk/loadjpkthermalfile.py
+-rw-rw-rw-   0        0        0    16785 2023-04-13 09:04:54.000000 pyfmreader-0.1.1/src/pyfmreader/jpk/parsejpkheader.py
+-rw-rw-rw-   0        0        0     3974 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/load_uff.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:57.817703 pyfmreader-0.1.1/src/pyfmreader/nanosc/
+-rw-rw-rw-   0        0        0      125 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/nanosc/__init__.py
+-rw-rw-rw-   0        0        0     5946 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/nanosc/loadnanosccurve.py
+-rw-rw-rw-   0        0        0      676 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/nanosc/loadnanoscfile.py
+-rw-rw-rw-   0        0        0     1577 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/nanosc/loadnanoscimg.py
+-rw-rw-rw-   0        0        0    10626 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/nanosc/parsenanoscheader.py
+-rw-rw-rw-   0        0        0     1839 2023-07-26 10:05:01.000000 pyfmreader-0.1.1/src/pyfmreader/pyfmreader.py
+-rw-rw-rw-   0        0        0     8251 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/save_uff.py
+-rw-rw-rw-   0        0        0     4893 2023-04-13 09:36:10.000000 pyfmreader-0.1.1/src/pyfmreader/uff.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:57.833692 pyfmreader-0.1.1/src/pyfmreader/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/utils/__init__.py
+-rw-rw-rw-   0        0        0     4073 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/utils/forcecurve.py
+-rw-rw-rw-   0        0        0     5959 2023-03-10 20:18:56.000000 pyfmreader-0.1.1/src/pyfmreader/utils/segment.py
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:57.753695 pyfmreader-0.1.1/src/pyfmreader.egg-info/
+-rw-rw-rw-   0        0        0     2331 2023-07-26 10:57:57.000000 pyfmreader-0.1.1/src/pyfmreader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      892 2023-07-26 10:57:57.000000 pyfmreader-0.1.1/src/pyfmreader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 10:57:57.000000 pyfmreader-0.1.1/src/pyfmreader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 10:57:57.000000 pyfmreader-0.1.1/src/pyfmreader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 10:57:57.841704 pyfmreader-0.1.1/tests/
+-rw-rw-rw-   0        0        0    11278 2023-07-26 10:32:52.000000 pyfmreader-0.1.1/tests/test_pyafmreader.py
```

### Comparing `pyfmreader-0.1.0/LICENSE.txt` & `pyfmreader-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/PKG-INFO` & `pyfmreader-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmreader
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package to read Nanoscope and JPK AFM files.
 Home-page: https://github.com/jlopezalo/PyFMReader
 Author: Javier Lopez Alonso
 Author-email: jla.lopez.18@gmail.com
 Project-URL: Bug Tracker, https://github.com/jlopezalo/PyFMReader/issues
 Project-URL: repository, https://github.com/jlopezalo/PyFMReader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfmreader-0.1.0/README.md` & `pyfmreader-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/jpk/loadjpkcurve.py` & `pyfmreader-0.1.1/src/pyfmreader/jpk/loadjpkcurve.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/jpk/loadjpkfile.py` & `pyfmreader-0.1.1/src/pyfmreader/jpk/loadjpkfile.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/jpk/loadjpkimg.py` & `pyfmreader-0.1.1/src/pyfmreader/jpk/loadjpkimg.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/jpk/loadjpkthermalfile.py` & `pyfmreader-0.1.1/src/pyfmreader/jpk/loadjpkthermalfile.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/jpk/parsejpkheader.py` & `pyfmreader-0.1.1/src/pyfmreader/jpk/parsejpkheader.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/nanosc/loadnanosccurve.py` & `pyfmreader-0.1.1/src/pyfmreader/nanosc/loadnanosccurve.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/nanosc/loadnanoscfile.py` & `pyfmreader-0.1.1/src/pyfmreader/nanosc/loadnanoscfile.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/nanosc/loadnanoscimg.py` & `pyfmreader-0.1.1/src/pyfmreader/nanosc/loadnanoscimg.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/nanosc/parsenanoscheader.py` & `pyfmreader-0.1.1/src/pyfmreader/nanosc/parsenanoscheader.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/pyfmreader.egg-info/PKG-INFO` & `pyfmreader-0.1.1/src/pyfmreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmreader
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python package to read Nanoscope and JPK AFM files.
 Home-page: https://github.com/jlopezalo/PyFMReader
 Author: Javier Lopez Alonso
 Author-email: jla.lopez.18@gmail.com
 Project-URL: Bug Tracker, https://github.com/jlopezalo/PyFMReader/issues
 Project-URL: repository, https://github.com/jlopezalo/PyFMReader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfmreader-0.1.0/pyfmreader/pyfmreader.egg-info/SOURCES.txt` & `pyfmreader-0.1.1/src/pyfmreader.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
-pyfmreader/jpk/__init__.py
-pyfmreader/jpk/loadjpkcurve.py
-pyfmreader/jpk/loadjpkfile.py
-pyfmreader/jpk/loadjpkimg.py
-pyfmreader/jpk/loadjpkthermalfile.py
-pyfmreader/jpk/parsejpkheader.py
-pyfmreader/nanosc/__init__.py
-pyfmreader/nanosc/loadnanosccurve.py
-pyfmreader/nanosc/loadnanoscfile.py
-pyfmreader/nanosc/loadnanoscimg.py
-pyfmreader/nanosc/parsenanoscheader.py
-pyfmreader/pyfmreader.egg-info/PKG-INFO
-pyfmreader/pyfmreader.egg-info/SOURCES.txt
-pyfmreader/pyfmreader.egg-info/dependency_links.txt
-pyfmreader/pyfmreader.egg-info/top_level.txt
-pyfmreader/utils/__init__.py
-pyfmreader/utils/forcecurve.py
-pyfmreader/utils/segment.py
+src/pyfmreader/__init__.py
+src/pyfmreader/constants.py
+src/pyfmreader/load_uff.py
+src/pyfmreader/pyfmreader.py
+src/pyfmreader/save_uff.py
+src/pyfmreader/uff.py
+src/pyfmreader.egg-info/PKG-INFO
+src/pyfmreader.egg-info/SOURCES.txt
+src/pyfmreader.egg-info/dependency_links.txt
+src/pyfmreader.egg-info/top_level.txt
+src/pyfmreader/jpk/__init__.py
+src/pyfmreader/jpk/loadjpkcurve.py
+src/pyfmreader/jpk/loadjpkfile.py
+src/pyfmreader/jpk/loadjpkimg.py
+src/pyfmreader/jpk/loadjpkthermalfile.py
+src/pyfmreader/jpk/parsejpkheader.py
+src/pyfmreader/nanosc/__init__.py
+src/pyfmreader/nanosc/loadnanosccurve.py
+src/pyfmreader/nanosc/loadnanoscfile.py
+src/pyfmreader/nanosc/loadnanoscimg.py
+src/pyfmreader/nanosc/parsenanoscheader.py
+src/pyfmreader/utils/__init__.py
+src/pyfmreader/utils/forcecurve.py
+src/pyfmreader/utils/segment.py
 tests/test_pyafmreader.py
```

### Comparing `pyfmreader-0.1.0/pyfmreader/utils/forcecurve.py` & `pyfmreader-0.1.1/src/pyfmreader/utils/forcecurve.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/pyfmreader/utils/segment.py` & `pyfmreader-0.1.1/src/pyfmreader/utils/segment.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.0/setup.cfg` & `pyfmreader-0.1.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7966 6d72 6561 6465 720d 0a76   = pyfmreader..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e30 0d0a  ersion = 0.1.0..
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e31 0d0a  ersion = 0.1.1..
 00000030: 6175 7468 6f72 203d 204a 6176 6965 7220  author = Javier 
 00000040: 4c6f 7065 7a20 416c 6f6e 736f 0d0a 6175  Lopez Alonso..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 206a 6c61  thor_email = jla
 00000060: 2e6c 6f70 657a 2e31 3840 676d 6169 6c2e  .lopez.18@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2041 2070 7974 686f 6e20 7061 636b   = A python pack
 00000090: 6167 6520 746f 2072 6561 6420 4e61 6e6f  age to read Nano
@@ -33,17 +33,16 @@
 00000200: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
 00000210: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
 00000220: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
 00000230: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
 00000240: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
 00000250: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
 00000260: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-00000270: 0a09 3d20 7079 666d 7265 6164 6572 0d0a  ..= pyfmreader..
-00000280: 7061 636b 6167 6573 203d 2066 696e 643a  packages = find:
-00000290: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-000002a0: 7320 3d20 3e3d 332e 360d 0a0d 0a5b 6f70  s = >=3.6....[op
-000002b0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-000002c0: 696e 645d 0d0a 7768 6572 6520 3d20 7079  ind]..where = py
-000002d0: 666d 7265 6164 6572 0d0a 0d0a 5b65 6767  fmreader....[egg
-000002e0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-000002f0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000300: 2030 0d0a 0d0a                            0....
+00000270: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
+00000280: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
+00000290: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
+000002a0: 2e36 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .6....[options.p
+000002b0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+000002c0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
+000002d0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+000002e0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000002f0: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `pyfmreader-0.1.0/tests/test_pyafmreader.py` & `pyfmreader-0.1.1/tests/test_pyafmreader.py`

 * *Files identical despite different names*

