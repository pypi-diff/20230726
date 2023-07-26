# Comparing `tmp/hivecode-0.0.0.8.19.tar.gz` & `tmp/hivecode-0.0.0.8.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivecode-0.0.0.8.19.tar", last modified: Tue Jul 18 05:08:33 2023, max compression
+gzip compressed data, was "hivecode-0.0.0.8.20.tar", last modified: Wed Jul 26 06:19:30 2023, max compression
```

## Comparing `hivecode-0.0.0.8.19.tar` & `hivecode-0.0.0.8.20.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.675951 hivecode-0.0.0.8.19/
--rw-rw-rw-   0        0        0     3790 2023-07-18 05:08:33.676456 hivecode-0.0.0.8.19/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.19/README.rst
--rw-rw-rw-   0        0        0     1402 2023-07-18 05:08:24.000000 hivecode-0.0.0.8.19/pyproject.toml
--rw-rw-rw-   0        0        0      184 2023-07-17 06:05:11.000000 hivecode-0.0.0.8.19/requirements.txt
--rw-rw-rw-   0        0        0     1181 2023-07-18 05:08:33.676957 hivecode-0.0.0.8.19/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.640816 hivecode-0.0.0.8.19/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.649861 hivecode-0.0.0.8.19/src/hiveadb/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hiveadb/__init__.py
--rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.19/src/hiveadb/eda.py
--rw-rw-rw-   0        0        0    11311 2023-04-12 03:58:56.000000 hivecode-0.0.0.8.19/src/hiveadb/function.py
--rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.19/src/hiveadb/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hiveadb/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.661868 hivecode-0.0.0.8.19/src/hivecode.egg-info/
--rw-rw-rw-   0        0        0     3790 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      274 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.19/src/hivecode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.669912 hivecode-0.0.0.8.19/src/hivecore/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivecore/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.19/src/hivecore/constant.py
--rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.19/src/hivecore/decorator.py
--rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.19/src/hivecore/eda.py
--rw-rw-rw-   0        0        0     4261 2023-05-08 01:08:47.000000 hivecode-0.0.0.8.19/src/hivecore/function.py
--rw-rw-rw-   0        0        0    32125 2023-07-16 07:35:55.000000 hivecode-0.0.0.8.19/src/hivecore/patterns.py
--rw-rw-rw-   0        0        0    29856 2023-04-12 03:24:52.000000 hivecode-0.0.0.8.19/src/hivecore/preprocess.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivecore/py.typed
--rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.19/src/hivecore/visual.py
-drwxrwxrwx   0        0        0        0 2023-07-18 05:08:33.674946 hivecode-0.0.0.8.19/src/hivesignal/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/analysis.py
--rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/eda.py
--rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/py.typed
--rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.19/src/hivesignal/transform.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.548434 hivecode-0.0.0.8.20/
+-rw-rw-rw-   0        0        0     3790 2023-07-26 06:19:30.548434 hivecode-0.0.0.8.20/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.20/README.rst
+-rw-rw-rw-   0        0        0     1402 2023-07-26 06:07:55.000000 hivecode-0.0.0.8.20/pyproject.toml
+-rw-rw-rw-   0        0        0      226 2023-07-20 05:57:35.000000 hivecode-0.0.0.8.20/requirements.txt
+-rw-rw-rw-   0        0        0     1182 2023-07-26 06:19:30.562919 hivecode-0.0.0.8.20/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.487618 hivecode-0.0.0.8.20/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.498784 hivecode-0.0.0.8.20/src/hiveadb/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hiveadb/__init__.py
+-rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.20/src/hiveadb/eda.py
+-rw-rw-rw-   0        0        0    11500 2023-07-26 06:04:36.000000 hivecode-0.0.0.8.20/src/hiveadb/function.py
+-rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.20/src/hiveadb/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hiveadb/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.524418 hivecode-0.0.0.8.20/src/hivecode.egg-info/
+-rw-rw-rw-   0        0        0     3790 2023-07-26 06:19:30.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      749 2023-07-26 06:19:30.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 06:19:30.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      314 2023-07-26 06:19:30.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-26 06:19:30.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.537554 hivecode-0.0.0.8.20/src/hivecore/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivecore/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.20/src/hivecore/constant.py
+-rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.20/src/hivecore/decorator.py
+-rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.20/src/hivecore/eda.py
+-rw-rw-rw-   0        0        0     7676 2023-07-26 05:32:41.000000 hivecode-0.0.0.8.20/src/hivecore/functions.py
+-rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.20/src/hivecore/patterns.py
+-rw-rw-rw-   0        0        0    28728 2023-07-20 03:05:40.000000 hivecode-0.0.0.8.20/src/hivecore/preprocess.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivecore/py.typed
+-rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.20/src/hivecore/visual.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.546401 hivecode-0.0.0.8.20/src/hivesignal/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/analysis.py
+-rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/eda.py
+-rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/py.typed
+-rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/transform.py
```

### Comparing `hivecode-0.0.0.8.19/PKG-INFO` & `hivecode-0.0.0.8.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.19
+Version: 0.0.0.8.20
 Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
```

### Comparing `hivecode-0.0.0.8.19/README.rst` & `hivecode-0.0.0.8.20/README.rst`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.19/pyproject.toml` & `hivecode-0.0.0.8.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "hivecode"
 description = "Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell."
-version = "0.0.0.8.19"
+version = "0.0.0.8.20"
 requires-python = ">=3.8.0"
 readme = "README.rst"
 authors = [
     {name = "Juan Manuel Mejía Botero", email="juanmam941025@gmail.com"},
     {name = "Sebastian López Valencia", email="sebaslv12@hotmail.com"}
 ]
```

### Comparing `hivecode-0.0.0.8.19/setup.cfg` & `hivecode-0.0.0.8.20/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -33,42 +33,42 @@
 00000200: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 00000210: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
 00000220: 3a20 332e 3131 0d0a 0d0a 5b6f 7074 696f  : 3.11....[optio
 00000230: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
 00000240: 0d0a 0968 6976 6563 6f72 650d 0a09 6869  ...hivecore...hi
 00000250: 7665 6164 620d 0a09 6869 7665 7369 676e  veadb...hivesign
 00000260: 616c 0d0a 7079 7468 6f6e 5f72 6571 7569  al..python_requi
-00000270: 7265 7320 3d20 3e3d 332e 382e 300d 0a69  res = >=3.8.0..i
-00000280: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000290: 3d20 0d0a 0970 6172 616d 696b 6f3d 3d32  = ...paramiko==2
-000002a0: 2e31 312e 300d 0a09 7363 703e 3d30 2e31  .11.0...scp>=0.1
-000002b0: 342e 340d 0a09 736b 6c65 6172 6e3e 3d30  4.4...sklearn>=0
-000002c0: 2e32 342e 310d 0a09 617a 7572 652d 636f  .24.1...azure-co
-000002d0: 736d 6f73 3e3d 342e 332e 300d 0a09 6f70  smos>=4.3.0...op
-000002e0: 656e 7079 786c 3e3d 332e 302e 3130 0d0a  enpyxl>=3.0.10..
-000002f0: 0974 7164 6d3e 3d34 2e36 342e 310d 0a09  .tqdm>=4.64.1...
-00000300: 7363 6970 793e 3d31 2e36 2e32 0d0a 096d  scipy>=1.6.2...m
-00000310: 6174 706c 6f74 6c69 623e 3d33 2e34 2e32  atplotlib>=3.4.2
-00000320: 0d0a 096e 756d 7079 3e3d 312e 3230 2e31  ...numpy>=1.20.1
-00000330: 0d0a 0970 616e 6461 733e 3d31 2e32 2e34  ...pandas>=1.2.4
-00000340: 0d0a 0973 6561 626f 726e 3e3d 302e 3131  ...seaborn>=0.11
-00000350: 2e31 0d0a 096b 6f61 6c61 730d 0a70 6163  .1...koalas..pac
-00000360: 6b61 6765 5f64 6972 203d 200d 0a09 3d20  kage_dir = ...= 
-00000370: 7372 630d 0a7a 6970 5f73 6166 6520 3d20  src..zip_safe = 
-00000380: 6e6f 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  no....[options.e
-00000390: 7874 7261 735f 7265 7175 6972 655d 0d0a  xtras_require]..
-000003a0: 7465 7374 696e 6720 3d20 0d0a 0970 7974  testing = ...pyt
-000003b0: 6573 743e 3d36 2e30 0d0a 0970 7974 6573  est>=6.0...pytes
-000003c0: 742d 636f 763e 3d32 2e30 0d0a 096d 7970  t-cov>=2.0...myp
-000003d0: 793e 3d30 2e39 3130 0d0a 0966 6c61 6b65  y>=0.910...flake
-000003e0: 383e 3d33 2e39 0d0a 0974 6f78 3e3d 332e  8>=3.9...tox>=3.
-000003f0: 3234 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  24....[options.p
-00000400: 6163 6b61 6765 5f64 6174 615d 0d0a 6869  ackage_data]..hi
-00000410: 7665 636f 7265 203d 2070 792e 7479 7065  vecore = py.type
-00000420: 640d 0a68 6976 6561 6462 203d 2070 792e  d..hiveadb = py.
-00000430: 7479 7065 640d 0a68 6976 6573 6967 6e61  typed..hivesigna
-00000440: 6c20 3d20 7079 2e74 7970 6564 0d0a 0d0a  l = py.typed....
-00000450: 5b66 6c61 6b65 385d 0d0a 6d61 782d 6c69  [flake8]..max-li
-00000460: 6e65 2d6c 656e 6774 6820 3d20 3136 300d  ne-length = 160.
-00000470: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000480: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000490: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000270: 7265 7320 3d20 3e3d 332e 3130 2e30 0d0a  res = >=3.10.0..
+00000280: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+00000290: 203d 200d 0a09 7061 7261 6d69 6b6f 3d3d   = ...paramiko==
+000002a0: 322e 3131 2e30 0d0a 0973 6370 3e3d 302e  2.11.0...scp>=0.
+000002b0: 3134 2e34 0d0a 0973 6b6c 6561 726e 3e3d  14.4...sklearn>=
+000002c0: 302e 3234 2e31 0d0a 0961 7a75 7265 2d63  0.24.1...azure-c
+000002d0: 6f73 6d6f 733e 3d34 2e33 2e30 0d0a 096f  osmos>=4.3.0...o
+000002e0: 7065 6e70 7978 6c3e 3d33 2e30 2e31 300d  penpyxl>=3.0.10.
+000002f0: 0a09 7471 646d 3e3d 342e 3634 2e31 0d0a  ..tqdm>=4.64.1..
+00000300: 0973 6369 7079 3e3d 312e 362e 320d 0a09  .scipy>=1.6.2...
+00000310: 6d61 7470 6c6f 746c 6962 3e3d 332e 342e  matplotlib>=3.4.
+00000320: 320d 0a09 6e75 6d70 793e 3d31 2e32 302e  2...numpy>=1.20.
+00000330: 310d 0a09 7061 6e64 6173 3e3d 312e 322e  1...pandas>=1.2.
+00000340: 340d 0a09 7365 6162 6f72 6e3e 3d30 2e31  4...seaborn>=0.1
+00000350: 312e 310d 0a09 6b6f 616c 6173 0d0a 7061  1.1...koalas..pa
+00000360: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
+00000370: 2073 7263 0d0a 7a69 705f 7361 6665 203d   src..zip_safe =
+00000380: 206e 6f0d 0a0d 0a5b 6f70 7469 6f6e 732e   no....[options.
+00000390: 6578 7472 6173 5f72 6571 7569 7265 5d0d  extras_require].
+000003a0: 0a74 6573 7469 6e67 203d 200d 0a09 7079  .testing = ...py
+000003b0: 7465 7374 3e3d 362e 300d 0a09 7079 7465  test>=6.0...pyte
+000003c0: 7374 2d63 6f76 3e3d 322e 300d 0a09 6d79  st-cov>=2.0...my
+000003d0: 7079 3e3d 302e 3931 300d 0a09 666c 616b  py>=0.910...flak
+000003e0: 6538 3e3d 332e 390d 0a09 746f 783e 3d33  e8>=3.9...tox>=3
+000003f0: 2e32 340d 0a0d 0a5b 6f70 7469 6f6e 732e  .24....[options.
+00000400: 7061 636b 6167 655f 6461 7461 5d0d 0a68  package_data]..h
+00000410: 6976 6563 6f72 6520 3d20 7079 2e74 7970  ivecore = py.typ
+00000420: 6564 0d0a 6869 7665 6164 6220 3d20 7079  ed..hiveadb = py
+00000430: 2e74 7970 6564 0d0a 6869 7665 7369 676e  .typed..hivesign
+00000440: 616c 203d 2070 792e 7479 7065 640d 0a0d  al = py.typed...
+00000450: 0a5b 666c 616b 6538 5d0d 0a6d 6178 2d6c  .[flake8]..max-l
+00000460: 696e 652d 6c65 6e67 7468 203d 2031 3630  ine-length = 160
+00000470: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+00000480: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000490: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `hivecode-0.0.0.8.19/src/hiveadb/eda.py` & `hivecode-0.0.0.8.20/src/hiveadb/eda.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.19/src/hiveadb/function.py` & `hivecode-0.0.0.8.20/src/hiveadb/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from hivecore.constant import PANDAS_TYPES, PYSPARK_TYPES, KOALAS_TYPES, PANDAS_ON_SPARK_TYPES, PANDAS, KOALAS, SPARK, PYSPARK, PANDAS_ON_SPARK, IN_PANDAS_ON_SPARK, IN_PYSPARK
-from hivecore.function import lib_required
+from hivecore.functions import lib_required, LazyImport
+
+LazyImport.import_from("databricks.koalas", from_pandas = 'from_pandas', KoalasDataFrame = 'DataFrame')
+LazyImport.import_from('pyspark.context',  SparkContext = 'SparkContext')
+LazyImport.import_from('pyspark.context',  SparkContext = 'SparkSession')
+LazyImport.import_from('pyspark.context',  SparkContext = 'SparkSession')
+LazyImport.import_from('pyspark.pandas', ps_from_pandas = 'from_pandas')
 
 from typing import List, Union, Any
 
-# Pyspark
-from pyspark.context import SparkContext
-from pyspark.sql.session import SparkSession
-from pyspark.pandas import from_pandas as ps_from_pandas
-from databricks.koalas import from_pandas, DataFrame as KoalasDataFrame
 
 def get_spark() -> SparkSession:
     """
     Fetches the current instance of Spark. If none exists, creates a new one.
 
     :return: The current Spark session.
     :rtype: pyspark.sql.SparkSession
```

### Comparing `hivecode-0.0.0.8.19/src/hiveadb/io.py` & `hivecode-0.0.0.8.20/src/hiveadb/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.19/src/hivecode.egg-info/PKG-INFO` & `hivecode-0.0.0.8.20/src/hivecode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.19
+Version: 0.0.0.8.20
 Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
```

### Comparing `hivecode-0.0.0.8.19/src/hivecode.egg-info/SOURCES.txt` & `hivecode-0.0.0.8.20/src/hivecode.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 src/hivecode.egg-info/not-zip-safe
 src/hivecode.egg-info/requires.txt
 src/hivecode.egg-info/top_level.txt
 src/hivecore/__init__.py
 src/hivecore/constant.py
 src/hivecore/decorator.py
 src/hivecore/eda.py
-src/hivecore/function.py
+src/hivecore/functions.py
 src/hivecore/patterns.py
 src/hivecore/preprocess.py
 src/hivecore/py.typed
 src/hivecore/visual.py
 src/hivesignal/__init__.py
 src/hivesignal/analysis.py
 src/hivesignal/eda.py
```

### Comparing `hivecode-0.0.0.8.19/src/hivecore/constant.py` & `hivecode-0.0.0.8.20/src/hivecore/constant.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.19/src/hivecore/decorator.py` & `hivecode-0.0.0.8.20/src/hivecore/decorator.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.19/src/hivecore/eda.py` & `hivecode-0.0.0.8.20/src/hivecore/eda.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.19/src/hivecore/patterns.py` & `hivecode-0.0.0.8.20/src/hivecore/patterns.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,23 +10,22 @@
     A decorator used to turn a class into a Singleton. This makes it so that if a class has already been instanciated one, that instance will be returned instead of a second one.
 
     :param class_: A class to apply the singleton to. Applied as a Decorator.
     :type class_: Class
     :return: Singleton instance of that Class.
     :rtype: Object
     """
+    
     instances = {}
-
-    @wraps(class_)
-    def getinstance(*args, **kwargs):
-        if class_ not in instances:
-            instances[class_] = class_(*args, **kwargs)
-        return instances[class_]
-
-    return getinstance
+    class SingletonWrapper(class_):
+        def _new_(cls, *args, **kwargs):
+            if class_ not in instances:
+                instances[class_] = super(SingletonWrapper, cls)._new_(cls)
+            return instances[class_]
+    return SingletonWrapper
 
 
 @singleton
 class Observer:
     """
     An observer class. This type of class let's you to add attributes, fetch their values and remove them dynamiclly. Quite useful to access data inside a defined scope as it behaves as a Singleton.
     """
```

### Comparing `hivecode-0.0.0.8.19/src/hivecore/preprocess.py` & `hivecode-0.0.0.8.20/src/hivecore/preprocess.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,20 +22,30 @@
 
 from typing import List, Union
 from os import system
 from pyspark.sql.functions import abs as sabs, max as smax, min as smin, mean as _mean, stddev as _stddev, count as scount, first, last
 from sklearn.metrics.pairwise import cosine_similarity as sk_cosine_similarity
 from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
 from pandas import DataFrame, concat
-from typing import List
+from typing import List, Union
 
 import pandas
 import pyspark
 import databricks.koalas
 
+
+from textdistance import cosine, jaro, levenshtein, damerau_levenshtein, hamming
+from jellyfish import jaro_winkler
+from typing import Union, List, Mapping
+from pandas import DataFrame as PandasDataFrame, Series as PandasSeries, concat as PandasConcat
+from pyspark.sql import DataFrame as SparkDataFrame
+from pyspark.sql.functions import expr
+from pyspark.sql.types import DoubleType
+from polars import DataFrame as PolarsDataFrame, Series as PolarsSeries, Float64 as PolarsFloat64
+
 ##### NUMERIC FUNCTIONS #####
 def normalize(df: Union[pandas.DataFrame, databricks.koalas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame], 
               columns: List[str] = None, 
               method: str = "max-abs", 
               overwrite: bool = False) -> Union[pandas.DataFrame, databricks.koalas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]:
     """
     Normalize the values in the specified columns of a DataFrame using a given normalization method.
@@ -245,278 +255,186 @@
             df = df.dropna()
         if engine == PYSPARK:
             df = df.na.drop()
     return df
 
 
 ##### TEXT FUNCTIONS #####
-def text_similarity(
-    df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame], 
-    columns: List[str], 
-    method: str = "tfid", 
-    threshold: float = 0.95, 
-    overwrite: bool = False, 
-    engine: str = "cosine"
-) -> Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]:
+def text_similarity(original_source, comparison_text, engine="auto", threshold=None, dict_attr='values', columns=None, new_column=True) -> Union[float, List, Mapping, PandasDataFrame, PandasSeries, SparkDataFrame, PolarsDataFrame, PolarsSeries]:
     """
-    Compute the similarity between strings in the specified dataframe columns.
-
-    :param df: The dataframe whose columns will be used for computing text similarity.
-    :type df: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
+    Calculate the similarity between two texts using different algorithms.
 
-    :param columns: The list of column names whose string values will be compared.
-    :type columns: List[str]
+    :param original_source: The original text or column-like structure.
+    :type original_source: str, list, dict, pandas.DataFrame, pandas.Series, pyspark.sql.DataFrame
+    :param comparison_text: The text to compare with the original text.
+    :type comparison_text: str
+    :param engine: The algorithm/engine to use for similarity calculation. Defaults to "auto".
+    :type engine: str, optional
+    :param threshold: The similarity threshold. If specified, the result is a boolean indicating whether the similarity
+                      is above or equal to the threshold. If not specified, the similarity value is returned.
+    :type threshold: float, optional
+    :param dict_attr: An option to specify what to use as an iterator for the similarities, "values" or "keys". Defaults to "values".
+    :type dict_attr: str
+    :param columns: Used to define the columns to apply the similarity to. Defaults to None.
+    :type columns: List[str], optional
+    :param new_column: Whether to add new columns for similarity scores or overwrite existing columns. Defaults to False.
+    :type new_column: bool, optional
+    :return: The DataFrame with similarity scores.
+    :rtype: Union[float, List, Mapping, pandas.DataFrame, pandas.Series, pyspark.sql.DataFrame, polars.DataFrame, polars.Series]
+    """
 
-    :param method: The method to use for computing text similarity. Possible values are "tfid" and "count".
-    :type method: str
+    def text_similarity_wrapper(original_source, comparison_text, engine, threshold):
+        # Validate threshold if specified
+        if threshold is not None and (not isinstance(threshold, float) or not 0 <= threshold <= 1):
+            raise ValueError("Threshold must be a float between 0 and 1.")
+
+        # Validate original_source type
+        if not isinstance(original_source, str):
+            raise ValueError(f"Original text must be a string, not type {type(original_source)}")
+        
+        # Validate original_source type
+        if not isinstance(comparison_text, str):
+            raise ValueError(f"Comparison text must be a string, not type {type(comparison_text)}")
+
+        # Validate engine
+        if engine == "auto":
+            if len(original_source) > 100 or len(comparison_text) > 100:
+                engine = "cosine"
+            else:
+                engine = "jaro"
+        elif engine not in ["cosine", "jaro", "jaro_winkler", "levenshtein", "damerau_levenshtein", "hamming"]:
+            raise ValueError(f"Invalid engine: {engine}")
 
-    :param threshold: The threshold above which two strings are considered similar. Should be a value between 0 and 1.
-    :type threshold: float
 
-    :param overwrite: If True, the original column values will be overwritten with the most similar ones.
-    :type overwrite: bool
 
-    :param engine: The similarity computation engine to use. Possible values are "cosine_similarity", "jaro",
-                   "levenshtein", "damerau_levenshtein", "jaro_winkler", and "hamming".
-    :type engine: str
+        # Calculate similarity based on the engine
+        if engine == "cosine":
+            similarity = cosine.normalized_similarity(original_source, comparison_text)
+        elif engine == "jaro":
+            similarity = jaro.normalized_similarity(original_source, comparison_text)
+        elif engine == "jaro_winkler":
+            similarity = jaro_winkler(original_source, comparison_text)
+        elif engine == "levenshtein":
+            similarity = levenshtein.normalized_similarity(original_source, comparison_text)
+        elif engine == "damerau_levenshtein":
+            similarity = damerau_levenshtein.normalized_similarity(original_source, comparison_text)
+        elif engine == "hamming":
+            similarity = hamming.normalized_similarity(original_source, comparison_text)
+
+        # Return similarity or boolean result based on threshold
+        if threshold is None:
+            return similarity
+        else:
+            return similarity >= threshold
 
-    :return: A dataframe with the similarity values between strings.
-    :rtype: Union[KoalasDataFrame, pandas.DataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]
-    """
-    def cosine_similarity(documents: List[str], header: bool = True, engine="tfid", i:int = 0):
-        if engine == "count":
-            count_vect = CountVectorizer()
-            trsfm = count_vect.fit_transform(documents)
-        elif engine == "tfid":
-            vectorizer = TfidfVectorizer()
-            trsfm=vectorizer.fit_transform(documents)
+    # Register the text_similarity_wrapper function as a UDF
+    spark.udf.register("text_similarity_wrapper", text_similarity_wrapper, DoubleType())
 
-        if header:
-            docs = [f'Document {i}' for i in range(1, len(documents) + 1)]
+    if isinstance(original_source, str):
+        # RETURN THE NORMAL CALL WHEN THE TYPE IS STR
+        return text_similarity_wrapper(original_source, comparison_text, engine, threshold)
+    elif isinstance(original_source, list):
+        # RETURN A LIST MAPPED BY THE LIST ITEMS.
+        if any(unexpected_type := list(filter(None,[item if not isinstance(item, str) else None for item in original_source]))):
+            raise ValueError(f"Found invalid item in list of type {', '.join(list(map(lambda item: type(item).name, unexpected_type)))}")
+        
+        return list(map(lambda text: text_similarity_wrapper(text, comparison_text, engine, threshold), original_source))
+    elif isinstance(original_source, dict):
+        # RETURNS A DICT MAPPED BY KEYS OR VALUES.
+        if dict_attr.lower() == "value" or dict_attr.lower() == "values":
+            iterator = original_source.items()
+            return dict(map(lambda item: (item[0],text_similarity_wrapper(item[1], comparison_text, engine, threshold)), iterator))
+        elif dict_attr.lower() == "key" or dict_attr.lower() == "keys":
+            iterator = original_source.keys()
+            return dict(map(lambda item: (item,text_similarity_wrapper(item, comparison_text, engine, threshold)), iterator))
         else:
-            docs = documents
-
-        vals = sk_cosine_similarity(trsfm[i:i+1], trsfm)[0].tolist()
-    #     return vals
-        return DataFrame(vals, columns=[documents[i]], index=docs)
-
-    def hamming(s1, s2):
-        if len(s1) != len(s2):
-            raise ValueError('expected two strings of the same length')
-        count = 0
-        for i in range(len(s1)):
-            if s1[i] != s2[i]:
-                count += 1
-        return count
-
-    def jaro(s1, s2):
-
-        if s1 == s2:
-            return 1.0
-
-        len_s1 = len(s1)
-        len_s2 = len(s2)
-
-        if len_s1 == 0 or len_s2 == 0:
-            return 0.0
-        if len_s1 > len_s2:
-            s1, s2 = s2, s1
-            len_s1, len_s2 = len_s2, len_s1
-
-        # Maxumum distance upto which matching is allowed
-        search_range = (len_s1 + 1) // 2
-        # search_range = floor(max(len_s1, len_s2) / 2) - 1
-
-        match = 0
-        match_s1 = [0] * len_s1
-        match_s2 = [0] * len_s2
-        # Check if there is any matches
-        for i in range(len_s1):
-            start = max(0, i - search_range)
-            end = min(len_s2, i + search_range + 1)
-            for j in range(start, end):
-                if s1[i] == s2[j] and match_s2[j] == 0:
-                    match_s1[i] = 1
-                    match_s2[j] = 1
-                    match += 1
-                    break
-
-        if not match:
-            return 0.0
-
-        # Number of transpositions
-        trans = k = 0
-        for i in range(len_s1):
-            if match_s1[i]:
-                while match_s2[k] == 0:
-                    k += 1
-                if s1[i] != s2[k]:
-                    k += 1
-                    trans += 1
-                else:
-                    k += 1
+            raise ValueError(f"Parameter dict_attr not recognized {dict_attr}")
+    elif isinstance(original_source, PandasDataFrame):
+        # RETURN A DATAFRAME AFTER APPLYING THE WRAPPER TO SELECTED COLUMNS.
+        if columns is None:
+            columns = original_source.columns.tolist()
+
+        similarity_df = original_source[columns].applymap(
+            lambda item: text_similarity_wrapper(item, comparison_text, engine, threshold)
+        )
 
-        trans = trans // 2
+        if new_column:
+            similarity_df = PandasConcat([original_source, similarity_df.add_suffix('_similarity')], axis=1)
+        else:
+            similarity_df.columns = original_source.columns
 
-        return ((match / len_s1 + match / len_s2 + (match - trans) / match ) / 3.0)
+        return similarity_df
+    elif isinstance(original_source, PandasSeries):
+        # RETURN A SERIES AFTER APPLYING THE WRAPPER TO ALL THE ITEMS IN IT.
+        return original_source.apply(lambda item: text_similarity_wrapper(item, comparison_text, engine, threshold))
+    elif isinstance(original_source, SparkDataFrame):
+        if columns is None:
+            columns = original_source.columns
+
+        similarity_exprs = []
+        for col in columns:
+            # Generate a new column name for similarity scores
+            if new_column:
+                new_col_name = col + "_similarity"
+                # Check if the new column name already exists in the DataFrame
+                while new_col_name in original_source.columns:
+                    new_col_name += "_1"
+            else:
+                new_col_name = col
 
-    def damerau_levenshtein(s1, s2):
-        len_s1 = len(s1)
-        len_s2 = len(s2)
-        max_dist = len_s1 + len_s2
-        charas = {}
-        arr = [[max_dist for _ in range(len_s2 + 2)] for _ in range(len_s1 + 2)]
-
-        for i in range(1, len_s1 + 2):
-            arr[i][1] = i - 1
-        for j in range(1, len_s2 + 2):
-            arr[1][j] = j - 1
-
-        for i in range(2, len_s1 + 2):
-            temp = 1
-            for j in range(2, len_s2 + 2):
-                k = charas.get(s2[j-2], 1)
-                l = temp
-                cost = 0 if s1[i-2] == s2[j-2] else 1
-                if not cost:
-                    temp = j
-                arr[i][j] = min(
-                    arr[i][j-1] + 1,
-                    arr[i-1][j] + 1,                      
-                    arr[i-1][j-1] + cost,
-                    arr[k-1][l-1] + max((i-k-1),(j-l-1)) + 1 # transposition
-                    )
-            charas[s1[i-2]] = i
-
-        return arr[-1][-1]
-
-    def jaro_winkler(s1, s2):
-        jaro_distance = jaro(s1, s2)
-
-        # If the jaro_distance is above a threshold
-        if jaro_distance > 0.7:
-            prefix = 0
-            for i in range(min(len(s1), len(s2))):
-                if s1[i] == s2[i]:
-                    prefix += 1
-                else:
-                    break
-            prefix = min(4, prefix)
-            jaro_distance += 0.1 * prefix * (1 - jaro_distance)
-
-        return jaro_distance
-
-    def levenshtein(s1, s2):
-        if s1 == s2:
-            return 0
-
-        s1_len = len(s1)
-        s2_len = len(s2)
-
-        if s1_len == 0:
-            return s2_len
-        if s2_len == 0:
-            return s1_len
-
-        arr = [[j for j in range(s2_len + 1)] if i == 0 \
-            else [i if j == 0 else 0 for j in range(s2_len+1)] for i in range(s1_len+1)]
-
-        for i in range(1, s1_len+1):
-            for j in range(1, s2_len+1):
-                d1 = arr[i-1][j] + 1
-                d2 = arr[i][j-1] + 1
-                d3 = arr[i-1][j-1] + (0 if s1[i-1]==s2[j-1] else 1)
-                arr[i][j] = min(d1, d2, d3)
-
-        return arr[s1_len][s2_len]
-    
-    def most_similar(_df, threshold: float = 0.95):
-                    similarity_score = _df[_df.columns.to_list()[0]].nlargest(2).tail(1).sum()
-                    if similarity_score >= threshold:
-                        return list(_df[_df.columns.to_list()[0]].nlargest(2).tail(1).index)[0]
-                    else:
-                        return list(_df[_df.columns.to_list()[0]].nlargest(2).head(1).index)[0]
+            # Create the expression to calculate the similarity score
+            expr_col = expr("text_similarity_wrapper({}, '{}', '{}', {})".format(
+                col, comparison_text, engine, "CAST({} AS DOUBLE)".format(threshold) if threshold is not None else "NULL"
+            )).alias(new_col_name)
+
+            # Append the expression to the list
+            similarity_exprs.append(expr_col)
+
+        # Select the similarity expressions along with the original columns
+        # Overwrite the existing columns inplace
+        if new_column:
+            df = original_source.select("*", *similarity_exprs)
+        else:
+            df = original_source.select(*[expr_col if col in columns else col for col, expr_col in zip(original_source.columns, similarity_exprs)])
 
-    if df_type(df) in [PANDAS, KOALAS, PANDAS_ON_SPARK]:
-        df = df.copy()
-    elif df_type(df) == PYSPARK:
-        df = df.alias("_copy")
+        return df
+    elif isinstance(original_source, PolarsDataFrame):
+        # Multiple columns case
+        if columns is None:
+            columns = original_source.columns
+
+        def text_similarity_func(item):
+            return text_similarity_wrapper(item, comparison_text, engine, threshold)
+        
+        new_columns = list()
+
+        for column in columns:
+            # Apply text_similarity to the selected column
+            similarity_col = f"{column}_similarity"
+            similarity = original_source[column].apply(lambda x: text_similarity_func(x), return_dtype=PolarsFloat64())
+            new_columns.append(similarity.alias(similarity_col))
 
-    if engine == "cosine_similarity" or engine == "cosine similarity" or engine == "cos" or engine == "cosine":
-        for col_name, corpus in zip(columns,to_list(df, columns)):
-            for i in range(len(corpus)):
-                _df = cosine_similarity(corpus, False, method, i)
-                if overwrite:
-                    df.loc[df[col_name] == corpus[i], f"{col_name}"] = most_similar(_df, threshold=threshold)
-                else:
-                    df.loc[df[col_name] == corpus[i], f"{col_name}_similarity"] = most_similar(_df, threshold=threshold)
-        if len(df) == 1:
-            return df[0]
-        else:
-            return df
-    elif engine == "jaro":
-        for col_name, column in zip(columns, to_list(df, columns)):
-            for corpus in column:
-                _df = DataFrame(list(map(lambda _corpus: jaro(corpus, _corpus), column)), columns = [corpus], index = column)
-                if overwrite:
-                    df.loc[df[col_name] == corpus, f"{col_name}"] = most_similar(_df, threshold=threshold)
-                else:
-                    df.loc[df[col_name] == corpus, f"{col_name}_similarity"] = most_similar(_df, threshold=threshold)
-        if len(df) == 1:
-            return df[0]
+        if new_column:
+            original_source = original_source.with_columns(new_columns)
         else:
-            return df
-    elif engine == "levenshtein":
-        for col_name, column in zip(columns, to_list(df, columns)):
-            for corpus in column:
-                _df = DataFrame(list(map(lambda _corpus: levenshtein(corpus, _corpus), column)), columns = [corpus], index = column)
-                if overwrite:
-                    df.loc[df[col_name] == corpus, f"{col_name}"] = most_similar(_df, threshold=threshold)
-                else:
-                    df.loc[df[col_name] == corpus, f"{col_name}_similarity"] = most_similar(_df, threshold=threshold)
-        if len(df) == 1:
-            return df[0]
-        else:
-            return df
-    elif engine == "damerau_levenshtein" or engine == "damerau levenshtein":
-        for col_name, column in zip(columns, to_list(df, columns)):
-            for corpus in column:
-                _df = DataFrame(list(map(lambda _corpus: damerau_levenshtein(corpus, _corpus), column)), columns = [corpus], index = column)
-                if overwrite:
-                    df.loc[df[col_name] == corpus, f"{col_name}"] = most_similar(_df, threshold=threshold)
-                else:
-                    df.loc[df[col_name] == corpus, f"{col_name}_similarity"] = most_similar(_df, threshold=threshold)
-        if len(df) == 1:
-            return df[0]
-        else:
-            return df
-    elif engine == "jaro_winkler" or engine == "jaro winkler":
-        for col_name, column in zip(columns, to_list(df, columns)):
-            for corpus in column:
-                _df = DataFrame(list(map(lambda _corpus: jaro_winkler(corpus, _corpus), column)), columns = [corpus], index = column)
-                if overwrite:
-                    df.loc[df[col_name] == corpus, f"{col_name}"] = most_similar(_df, threshold=threshold)
-                else:
-                    df.loc[df[col_name] == corpus, f"{col_name}_similarity"] = most_similar(_df, threshold=threshold)
-        if len(df) == 1:
-            return df[0]
-        else:
-            return df
-    elif engine == "hamming":
-        for col_name, column in zip(columns, to_list(df, columns)):
-            for corpus in column:
-                _df = DataFrame(list(map(lambda _corpus: hamming(corpus, _corpus), column)), columns = [corpus], index = column)
-                if overwrite:
-                    df.loc[df[col_name] == corpus, f"{col_name}"] = most_similar(_df, threshold=threshold)
-                else:
-                    df.loc[df[col_name] == corpus, f"{col_name}_similarity"] = most_similar(_df, threshold=threshold)
-        if len(df) == 1:
-            return df[0]
-        else:
-            return df
+            for column in columns:
+                original_source = original_source.drop(column)
+            original_source = original_source.with_columns(new_columns)
+
+        return original_source
+    elif isinstance(original_source, PolarsSeries):
+        # RETURN A SERIES AFTER APPLYING THE WRAPPER TO ALL THE ITEMS IN IT.
+        if columns is None:
+            columns = original_source.columns
+        def text_similarity_func(item):
+            return text_similarity_wrapper(item, comparison_text, engine, threshold)
+
+        return original_source.select(columns).apply(text_similarity_func)
+    else:
+        raise ValueError("Unsupported data type: {}".format(type(original_source)._name_))
 
 
 def encode(df: Union[pandas.DataFrame, KoalasDataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame], 
            columns: List[str], 
            encoder: str = "categorical", 
            overwrite: bool = False,
            as_type: str = None) -> Union[pandas.DataFrame, KoalasDataFrame, pyspark.sql.DataFrame, pyspark.pandas.DataFrame]:
```

### Comparing `hivecode-0.0.0.8.19/src/hivecore/visual.py` & `hivecode-0.0.0.8.20/src/hivecore/visual.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.19/src/hivesignal/analysis.py` & `hivecode-0.0.0.8.20/src/hivesignal/analysis.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.19/src/hivesignal/io.py` & `hivecode-0.0.0.8.20/src/hivesignal/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.19/src/hivesignal/transform.py` & `hivecode-0.0.0.8.20/src/hivesignal/transform.py`

 * *Files identical despite different names*

