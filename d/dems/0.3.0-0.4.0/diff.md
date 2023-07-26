# Comparing `tmp/dems-0.3.0.tar.gz` & `tmp/dems-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dems-0.3.0.tar", max compression
+gzip compressed data, was "dems-0.4.0.tar", max compression
```

## Comparing `dems-0.3.0.tar` & `dems-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1076 2023-07-16 10:46:07.957393 dems-0.3.0/LICENSE
--rw-r--r--   0        0        0      664 2023-07-16 10:46:07.957393 dems-0.3.0/README.md
--rw-r--r--   0        0        0       94 2023-07-16 10:46:07.957393 dems-0.3.0/dems/__init__.py
--rw-r--r--   0        0        0     1182 2023-07-16 10:46:07.957393 dems-0.3.0/dems/d1.py
--rw-r--r--   0        0        0     6975 2023-07-16 10:46:07.957393 dems-0.3.0/dems/d2.py
--rw-r--r--   0        0        0        0 2023-07-16 10:46:07.957393 dems-0.3.0/dems/py.typed
--rw-r--r--   0        0        0      499 2023-07-16 10:46:07.957393 dems-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1246 1970-01-01 00:00:00.000000 dems-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-26 08:49:17.556738 dems-0.4.0/LICENSE
+-rw-r--r--   0        0        0      803 2023-07-26 08:49:17.556738 dems-0.4.0/README.md
+-rw-r--r--   0        0        0       94 2023-07-26 08:49:17.560737 dems-0.4.0/dems/__init__.py
+-rw-r--r--   0        0        0     1180 2023-07-26 08:49:17.560737 dems-0.4.0/dems/d1.py
+-rw-r--r--   0        0        0     6989 2023-07-26 08:49:17.560737 dems-0.4.0/dems/d2.py
+-rw-r--r--   0        0        0        0 2023-07-26 08:49:17.560737 dems-0.4.0/dems/py.typed
+-rw-r--r--   0        0        0      499 2023-07-26 08:49:17.560737 dems-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1385 1970-01-01 00:00:00.000000 dems-0.4.0/PKG-INFO
```

### Comparing `dems-0.3.0/LICENSE` & `dems-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dems-0.3.0/README.md` & `dems-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # dems
 
 [![Release](https://img.shields.io/pypi/v/dems?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/dems/)
 [![Python](https://img.shields.io/pypi/pyversions/dems?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/dems/)
 [![Downloads](https://img.shields.io/pypi/dm/dems?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/dems)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.8151950-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.8151950)
 [![Tests](https://img.shields.io/github/actions/workflow/status/deshima-dev/dems/tests.yaml?label=Tests&style=flat-square)](https://github.com/deshima-dev/dems/actions)
 
 DESHIMA measurement set
 
 ## Installation
 
 ```shell
```

### Comparing `dems-0.3.0/dems/d1.py` & `dems-0.4.0/dems/d1.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 class MS(AsDataArray):
     """Measurement set of DESHIMA 1.0."""
 
     data: Data[Tuple[Time, Chan], Any]
     vrad: Coord[Time, float] = 0.0
     x: Coord[Time, float] = 0.0
     y: Coord[Time, float] = 0.0
-    Timeme: Coord[Time, float] = 0.0
+    time: Coord[Time, float] = 0.0
     temp: Coord[Time, float] = 0.0
     pressure: Coord[Time, float] = 0.0
     vapor_pressure: Coord[Time, float] = 0.0
     windspd: Coord[Time, float] = 0.0
     winddir: Coord[Time, float] = 0.0
     scantype: Coord[Time, str] = "GRAD"
     scanid: Coord[Time, int] = 0
```

### Comparing `dems-0.3.0/dems/d2.py` & `dems-0.4.0/dems/d2.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 # standard library
 from dataclasses import dataclass
 from typing import Any, Literal, Tuple
 
 
 # dependencies
 from xarray_dataclasses import AsDataArray, Attr, Coordof, Data, Dataof
+from . import __version__
 
 
 # type hints
 Ti = Literal["time"]
 Ch = Literal["chan"]
 
 
 # constants
 ASTE_ITRS_COORDS = (
     +2230817.2140945992,
     -5440188.022176585,
     -2475718.801708271,
 )
-DEMS_VERSION = "v0.3.0"
-DMERGE_VERSION = "v1.0.0"
+DEMS_VERSION = __version__
+DMERGE_VERSION = "1.0.0"
 
 
 @dataclass
 class Data_:
     data: Data[Tuple[Ti, Ch], Any]
     long_name: Attr[str] = "Data values"
 
@@ -85,22 +86,22 @@
     data: Data[Ti, float]
     long_name: Attr[str] = "Sky latitude"
     units: Attr[str] = "deg"
 
 
 @dataclass
 class LonOrigin:
-    data: Data[Tuple[()], float]
+    data: Data[Ti, float]
     long_name: Attr[str] = "Reference sky longitude"
     units: Attr[str] = "deg"
 
 
 @dataclass
 class LatOrigin:
-    data: Data[Tuple[()], float]
+    data: Data[Ti, float]
     long_name: Attr[str] = "Reference sky latitude"
     units: Attr[str] = "deg"
 
 
 @dataclass
 class Frame:
     data: Data[Tuple[()], str]
```

### Comparing `dems-0.3.0/PKG-INFO` & `dems-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dems
-Version: 0.3.0
+Version: 0.4.0
 Summary: DESHIMA measurement set
 License: MIT
 Author: Akio Taniguchi
 Author-email: taniguchi@a.phys.nagoya-u.ac.jp
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 
 # dems
 
 [![Release](https://img.shields.io/pypi/v/dems?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/dems/)
 [![Python](https://img.shields.io/pypi/pyversions/dems?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/dems/)
 [![Downloads](https://img.shields.io/pypi/dm/dems?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/dems)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.8151950-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.8151950)
 [![Tests](https://img.shields.io/github/actions/workflow/status/deshima-dev/dems/tests.yaml?label=Tests&style=flat-square)](https://github.com/deshima-dev/dems/actions)
 
 DESHIMA measurement set
 
 ## Installation
 
 ```shell
```

