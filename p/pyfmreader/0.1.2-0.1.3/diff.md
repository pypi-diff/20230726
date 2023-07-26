# Comparing `tmp/pyfmreader-0.1.2.tar.gz` & `tmp/pyfmreader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmreader-0.1.2.tar", last modified: Wed Jul 26 11:06:22 2023, max compression
+gzip compressed data, was "pyfmreader-0.1.3.tar", last modified: Wed Jul 26 18:45:53 2023, max compression
```

## Comparing `pyfmreader-0.1.2.tar` & `pyfmreader-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:06:22.223764 pyfmreader-0.1.2/
--rw-rw-rw-   0        0        0     1084 2023-07-26 08:55:15.000000 pyfmreader-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0     2323 2023-07-26 11:06:22.223764 pyfmreader-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      612 2023-07-26 11:05:12.000000 pyfmreader-0.1.2/README.md
--rw-rw-rw-   0        0        0      243 2023-07-26 11:05:20.000000 pyfmreader-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      760 2023-07-26 11:06:22.231766 pyfmreader-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 11:06:21.987738 pyfmreader-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 11:06:22.079751 pyfmreader-0.1.2/src/pyfmreader/
--rw-rw-rw-   0        0        0      121 2023-07-26 10:55:40.000000 pyfmreader-0.1.2/src/pyfmreader/__init__.py
--rw-rw-rw-   0        0        0     1508 2023-07-26 10:09:41.000000 pyfmreader-0.1.2/src/pyfmreader/constants.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:06:22.175761 pyfmreader-0.1.2/src/pyfmreader/jpk/
--rw-rw-rw-   0        0        0      113 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/jpk/__init__.py
--rw-rw-rw-   0        0        0     6279 2023-04-26 09:25:11.000000 pyfmreader-0.1.2/src/pyfmreader/jpk/loadjpkcurve.py
--rw-rw-rw-   0        0        0     4593 2023-04-13 09:37:32.000000 pyfmreader-0.1.2/src/pyfmreader/jpk/loadjpkfile.py
--rw-rw-rw-   0        0        0     6672 2023-07-26 10:32:30.000000 pyfmreader-0.1.2/src/pyfmreader/jpk/loadjpkimg.py
--rw-rw-rw-   0        0        0     2809 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/jpk/loadjpkthermalfile.py
--rw-rw-rw-   0        0        0    16785 2023-04-13 09:04:54.000000 pyfmreader-0.1.2/src/pyfmreader/jpk/parsejpkheader.py
--rw-rw-rw-   0        0        0     3974 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/load_uff.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:06:22.199762 pyfmreader-0.1.2/src/pyfmreader/nanosc/
--rw-rw-rw-   0        0        0      125 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/nanosc/__init__.py
--rw-rw-rw-   0        0        0     5946 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/nanosc/loadnanosccurve.py
--rw-rw-rw-   0        0        0      676 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/nanosc/loadnanoscfile.py
--rw-rw-rw-   0        0        0     1579 2023-07-26 11:03:29.000000 pyfmreader-0.1.2/src/pyfmreader/nanosc/loadnanoscimg.py
--rw-rw-rw-   0        0        0    10626 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/nanosc/parsenanoscheader.py
--rw-rw-rw-   0        0        0     1839 2023-07-26 10:05:01.000000 pyfmreader-0.1.2/src/pyfmreader/pyfmreader.py
--rw-rw-rw-   0        0        0     8251 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/save_uff.py
--rw-rw-rw-   0        0        0     4893 2023-04-13 09:36:10.000000 pyfmreader-0.1.2/src/pyfmreader/uff.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:06:22.215764 pyfmreader-0.1.2/src/pyfmreader/utils/
--rw-rw-rw-   0        0        0        0 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/utils/__init__.py
--rw-rw-rw-   0        0        0     4073 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/utils/forcecurve.py
--rw-rw-rw-   0        0        0     5959 2023-03-10 20:18:56.000000 pyfmreader-0.1.2/src/pyfmreader/utils/segment.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:06:22.127755 pyfmreader-0.1.2/src/pyfmreader.egg-info/
--rw-rw-rw-   0        0        0     2323 2023-07-26 11:06:21.000000 pyfmreader-0.1.2/src/pyfmreader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      892 2023-07-26 11:06:21.000000 pyfmreader-0.1.2/src/pyfmreader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:06:21.000000 pyfmreader-0.1.2/src/pyfmreader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 11:06:21.000000 pyfmreader-0.1.2/src/pyfmreader.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 11:06:22.215764 pyfmreader-0.1.2/tests/
--rw-rw-rw-   0        0        0    11278 2023-07-26 10:32:52.000000 pyfmreader-0.1.2/tests/test_pyafmreader.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:45:53.372660 pyfmreader-0.1.3/
+-rw-rw-rw-   0        0        0     1084 2023-07-26 08:55:15.000000 pyfmreader-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2323 2023-07-26 18:45:53.372660 pyfmreader-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      612 2023-07-26 11:05:12.000000 pyfmreader-0.1.3/README.md
+-rw-rw-rw-   0        0        0      243 2023-07-26 18:44:36.000000 pyfmreader-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      809 2023-07-26 18:45:53.388676 pyfmreader-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 18:45:53.092566 pyfmreader-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 18:45:53.204640 pyfmreader-0.1.3/src/pyfmreader/
+-rw-rw-rw-   0        0        0      121 2023-07-26 10:55:40.000000 pyfmreader-0.1.3/src/pyfmreader/__init__.py
+-rw-rw-rw-   0        0        0     1508 2023-07-26 10:09:41.000000 pyfmreader-0.1.3/src/pyfmreader/constants.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:45:53.292647 pyfmreader-0.1.3/src/pyfmreader/jpk/
+-rw-rw-rw-   0        0        0      113 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/jpk/__init__.py
+-rw-rw-rw-   0        0        0     6279 2023-04-26 09:25:11.000000 pyfmreader-0.1.3/src/pyfmreader/jpk/loadjpkcurve.py
+-rw-rw-rw-   0        0        0     4593 2023-04-13 09:37:32.000000 pyfmreader-0.1.3/src/pyfmreader/jpk/loadjpkfile.py
+-rw-rw-rw-   0        0        0     6672 2023-07-26 10:32:30.000000 pyfmreader-0.1.3/src/pyfmreader/jpk/loadjpkimg.py
+-rw-rw-rw-   0        0        0     2809 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/jpk/loadjpkthermalfile.py
+-rw-rw-rw-   0        0        0    16785 2023-04-13 09:04:54.000000 pyfmreader-0.1.3/src/pyfmreader/jpk/parsejpkheader.py
+-rw-rw-rw-   0        0        0     3974 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/load_uff.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:45:53.332652 pyfmreader-0.1.3/src/pyfmreader/nanosc/
+-rw-rw-rw-   0        0        0      125 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/nanosc/__init__.py
+-rw-rw-rw-   0        0        0     5946 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/nanosc/loadnanosccurve.py
+-rw-rw-rw-   0        0        0      676 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/nanosc/loadnanoscfile.py
+-rw-rw-rw-   0        0        0     1579 2023-07-26 11:11:25.000000 pyfmreader-0.1.3/src/pyfmreader/nanosc/loadnanoscimg.py
+-rw-rw-rw-   0        0        0    10626 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/nanosc/parsenanoscheader.py
+-rw-rw-rw-   0        0        0     1839 2023-07-26 10:05:01.000000 pyfmreader-0.1.3/src/pyfmreader/pyfmreader.py
+-rw-rw-rw-   0        0        0     8251 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/save_uff.py
+-rw-rw-rw-   0        0        0     4893 2023-04-13 09:36:10.000000 pyfmreader-0.1.3/src/pyfmreader/uff.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:45:53.356655 pyfmreader-0.1.3/src/pyfmreader/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/utils/__init__.py
+-rw-rw-rw-   0        0        0     4073 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/utils/forcecurve.py
+-rw-rw-rw-   0        0        0     5959 2023-03-10 20:18:56.000000 pyfmreader-0.1.3/src/pyfmreader/utils/segment.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:45:53.244644 pyfmreader-0.1.3/src/pyfmreader.egg-info/
+-rw-rw-rw-   0        0        0     2323 2023-07-26 18:45:52.000000 pyfmreader-0.1.3/src/pyfmreader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      929 2023-07-26 18:45:53.000000 pyfmreader-0.1.3/src/pyfmreader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:45:53.000000 pyfmreader-0.1.3/src/pyfmreader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-26 18:45:53.000000 pyfmreader-0.1.3/src/pyfmreader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 18:45:53.000000 pyfmreader-0.1.3/src/pyfmreader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 18:45:53.364658 pyfmreader-0.1.3/tests/
+-rw-rw-rw-   0        0        0    11278 2023-07-26 10:32:52.000000 pyfmreader-0.1.3/tests/test_pyafmreader.py
```

### Comparing `pyfmreader-0.1.2/LICENSE.txt` & `pyfmreader-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/PKG-INFO` & `pyfmreader-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmreader
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package to read Nanoscope and JPK AFM files.
 Home-page: https://github.com/jlopezalo/PyFMReader
 Author: Javier Lopez Alonso
 Author-email: jla.lopez.18@gmail.com
 Project-URL: Bug Tracker, https://github.com/jlopezalo/PyFMReader/issues
 Project-URL: repository, https://github.com/jlopezalo/PyFMReader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfmreader-0.1.2/README.md` & `pyfmreader-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/setup.cfg` & `pyfmreader-0.1.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7966 6d72 6561 6465 720d 0a76   = pyfmreader..v
-00000020: 6572 7369 6f6e 203d 2030 2e31 2e32 0d0a  ersion = 0.1.2..
+00000020: 6572 7369 6f6e 203d 2030 2e31 2e33 0d0a  ersion = 0.1.3..
 00000030: 6175 7468 6f72 203d 204a 6176 6965 7220  author = Javier 
 00000040: 4c6f 7065 7a20 416c 6f6e 736f 0d0a 6175  Lopez Alonso..au
 00000050: 7468 6f72 5f65 6d61 696c 203d 206a 6c61  thor_email = jla
 00000060: 2e6c 6f70 657a 2e31 3840 676d 6169 6c2e  .lopez.18@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2041 2070 7974 686f 6e20 7061 636b   = A python pack
 00000090: 6167 6520 746f 2072 6561 6420 4e61 6e6f  age to read Nano
@@ -32,17 +32,20 @@
 000001f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
 00000200: 3a3a 2033 0d0a 094c 6963 656e 7365 203a  :: 3...License :
 00000210: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
 00000220: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
 00000230: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
 00000240: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
 00000250: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
-00000260: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-00000270: 0a09 3d20 7372 630d 0a70 6163 6b61 6765  ..= src..package
-00000280: 7320 3d20 6669 6e64 3a0d 0a70 7974 686f  s = find:..pytho
-00000290: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-000002a0: 2e36 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .6....[options.p
-000002b0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-000002c0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
-000002d0: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-000002e0: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-000002f0: 203d 2030 0d0a 0d0a                       = 0....
+00000260: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+00000270: 7320 3d20 0d0a 096e 756d 7079 0d0a 0970  s = ...numpy...p
+00000280: 616e 6461 730d 0a09 7469 6666 6669 6c65  andas...tifffile
+00000290: 0d0a 7061 636b 6167 655f 6469 7220 3d20  ..package_dir = 
+000002a0: 0d0a 093d 2073 7263 0d0a 7061 636b 6167  ...= src..packag
+000002b0: 6573 203d 2066 696e 643a 0d0a 7079 7468  es = find:..pyth
+000002c0: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
+000002d0: 332e 360d 0a0d 0a5b 6f70 7469 6f6e 732e  3.6....[options.
+000002e0: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+000002f0: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+00000300: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000310: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000320: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `pyfmreader-0.1.2/src/pyfmreader/constants.py` & `pyfmreader-0.1.3/src/pyfmreader/constants.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/jpk/loadjpkcurve.py` & `pyfmreader-0.1.3/src/pyfmreader/jpk/loadjpkcurve.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/jpk/loadjpkfile.py` & `pyfmreader-0.1.3/src/pyfmreader/jpk/loadjpkfile.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/jpk/loadjpkimg.py` & `pyfmreader-0.1.3/src/pyfmreader/jpk/loadjpkimg.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/jpk/loadjpkthermalfile.py` & `pyfmreader-0.1.3/src/pyfmreader/jpk/loadjpkthermalfile.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/jpk/parsejpkheader.py` & `pyfmreader-0.1.3/src/pyfmreader/jpk/parsejpkheader.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/load_uff.py` & `pyfmreader-0.1.3/src/pyfmreader/load_uff.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/nanosc/loadnanosccurve.py` & `pyfmreader-0.1.3/src/pyfmreader/nanosc/loadnanosccurve.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/nanosc/loadnanoscfile.py` & `pyfmreader-0.1.3/src/pyfmreader/nanosc/loadnanoscfile.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/nanosc/loadnanoscimg.py` & `pyfmreader-0.1.3/src/pyfmreader/nanosc/loadnanoscimg.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/nanosc/parsenanoscheader.py` & `pyfmreader-0.1.3/src/pyfmreader/nanosc/parsenanoscheader.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/pyfmreader.py` & `pyfmreader-0.1.3/src/pyfmreader/pyfmreader.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/save_uff.py` & `pyfmreader-0.1.3/src/pyfmreader/save_uff.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/uff.py` & `pyfmreader-0.1.3/src/pyfmreader/uff.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/utils/forcecurve.py` & `pyfmreader-0.1.3/src/pyfmreader/utils/forcecurve.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader/utils/segment.py` & `pyfmreader-0.1.3/src/pyfmreader/utils/segment.py`

 * *Files identical despite different names*

### Comparing `pyfmreader-0.1.2/src/pyfmreader.egg-info/PKG-INFO` & `pyfmreader-0.1.3/src/pyfmreader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmreader
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python package to read Nanoscope and JPK AFM files.
 Home-page: https://github.com/jlopezalo/PyFMReader
 Author: Javier Lopez Alonso
 Author-email: jla.lopez.18@gmail.com
 Project-URL: Bug Tracker, https://github.com/jlopezalo/PyFMReader/issues
 Project-URL: repository, https://github.com/jlopezalo/PyFMReader
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfmreader-0.1.2/src/pyfmreader.egg-info/SOURCES.txt` & `pyfmreader-0.1.3/src/pyfmreader.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/pyfmreader/load_uff.py
 src/pyfmreader/pyfmreader.py
 src/pyfmreader/save_uff.py
 src/pyfmreader/uff.py
 src/pyfmreader.egg-info/PKG-INFO
 src/pyfmreader.egg-info/SOURCES.txt
 src/pyfmreader.egg-info/dependency_links.txt
+src/pyfmreader.egg-info/requires.txt
 src/pyfmreader.egg-info/top_level.txt
 src/pyfmreader/jpk/__init__.py
 src/pyfmreader/jpk/loadjpkcurve.py
 src/pyfmreader/jpk/loadjpkfile.py
 src/pyfmreader/jpk/loadjpkimg.py
 src/pyfmreader/jpk/loadjpkthermalfile.py
 src/pyfmreader/jpk/parsejpkheader.py
```

### Comparing `pyfmreader-0.1.2/tests/test_pyafmreader.py` & `pyfmreader-0.1.3/tests/test_pyafmreader.py`

 * *Files identical despite different names*

