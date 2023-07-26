# Comparing `tmp/imsize-1.3.2.tar.gz` & `tmp/imsize-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsize-1.3.2.tar", last modified: Tue May  9 10:32:46 2023, max compression
+gzip compressed data, was "imsize-1.3.3.tar", last modified: Wed Jul 26 13:51:22 2023, max compression
```

## Comparing `imsize-1.3.2.tar` & `imsize-1.3.3.tar`

### file list

```diff
@@ -1,27 +1,22 @@
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-09 10:32:46.482217 imsize-1.3.2/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imsize-1.3.2/LICENSE
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       59 2023-03-13 15:45:56.000000 imsize-1.3.2/MANIFEST.in
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      284 2023-05-09 10:32:46.482217 imsize-1.3.2/PKG-INFO
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      589 2023-03-13 15:45:56.000000 imsize-1.3.2/README.md
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-09 10:32:46.482217 imsize-1.3.2/imsize/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      346 2023-05-09 10:16:43.000000 imsize-1.3.2/imsize/__init__.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15567 2023-03-13 15:45:56.000000 imsize-1.3.2/imsize/argv.py
--rwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)     3982 2023-04-19 12:14:31.000000 imsize-1.3.2/imsize/consoleapp.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     2760 2023-03-13 15:45:56.000000 imsize-1.3.2/imsize/exrhdr.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    14618 2023-05-09 10:22:58.000000 imsize-1.3.2/imsize/imsize.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1785 2023-03-13 15:45:56.000000 imsize-1.3.2/imsize/pfmhdr.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1733 2023-03-13 15:45:56.000000 imsize-1.3.2/imsize/pnmhdr.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-09 10:32:46.482217 imsize-1.3.2/imsize.egg-info/
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      284 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/PKG-INFO
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      430 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/SOURCES.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/dependency_links.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       51 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/entry_points.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       57 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/requires.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       12 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/top_level.txt
--rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-05-09 10:32:46.000000 imsize-1.3.2/imsize.egg-info/zip-safe
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)       65 2023-03-13 15:45:56.000000 imsize-1.3.2/requirements.txt
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      107 2023-05-09 10:32:46.482217 imsize-1.3.2/setup.cfg
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      709 2023-03-13 15:45:56.000000 imsize-1.3.2/setup.py
-drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-05-09 10:32:46.482217 imsize-1.3.2/test/
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)        0 2023-03-13 15:45:56.000000 imsize-1.3.2/test/__init__.py
--rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4919 2023-03-13 15:45:57.000000 imsize-1.3.2/test/test_read.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 13:51:22.401034 imsize-1.3.3/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1068 2023-03-13 15:45:56.000000 imsize-1.3.3/LICENSE
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     2294 2023-07-26 13:51:22.401034 imsize-1.3.3/PKG-INFO
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)      589 2023-03-13 15:45:56.000000 imsize-1.3.3/README.md
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      619 2023-07-26 13:28:36.000000 imsize-1.3.3/pyproject.toml
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       38 2023-07-26 13:51:22.405034 imsize-1.3.3/setup.cfg
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 13:51:22.401034 imsize-1.3.3/src/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    15567 2023-03-13 15:45:56.000000 imsize-1.3.3/src/argv.py
+-rwxr-xr-x   0 toaarnio  (1000) toaarnio  (1000)     4052 2023-07-26 13:25:19.000000 imsize-1.3.3/src/consoleapp.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     2760 2023-03-13 15:45:56.000000 imsize-1.3.3/src/exrhdr.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 13:51:22.401034 imsize-1.3.3/src/imsize.egg-info/
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)     2294 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/PKG-INFO
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)      342 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/SOURCES.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)        1 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/dependency_links.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       43 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/entry_points.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       57 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/requires.txt
+-rw-rw-r--   0 toaarnio  (1000) toaarnio  (1000)       44 2023-07-26 13:51:22.000000 imsize-1.3.3/src/imsize.egg-info/top_level.txt
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)    14958 2023-07-26 13:23:53.000000 imsize-1.3.3/src/imsize.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1785 2023-03-13 15:45:56.000000 imsize-1.3.3/src/pfmhdr.py
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     1733 2023-03-13 15:45:56.000000 imsize-1.3.3/src/pnmhdr.py
+drwxrwxr-x   0 toaarnio  (1000) toaarnio  (1000)        0 2023-07-26 13:51:22.401034 imsize-1.3.3/test/
+-rw-r--r--   0 toaarnio  (1000) toaarnio  (1000)     4919 2023-03-13 15:45:57.000000 imsize-1.3.3/test/test_read.py
```

### Comparing `imsize-1.3.2/LICENSE` & `imsize-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imsize-1.3.2/README.md` & `imsize-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `imsize-1.3.2/imsize/argv.py` & `imsize-1.3.3/src/argv.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.2/imsize/consoleapp.py` & `imsize-1.3.3/src/consoleapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         print()
         print("  example:")
         print("    imsize ~/Pictures")
         print()
         print("  supported file types:")
         print("   ", '\n    '.join(FILETYPES))
         print()
+        print(f"imsize version {imsize.__version__}")
+        print()
         sys.exit(-1)
     else:
         if verbose:
             print("See 'imsize --help' for command-line options.")
         paths = sys.argv[1:] or ["."]  # scan current directory if no arguments
         filespecs = find_files(paths)
         scan_sizes(filespecs, verbose, show_all)
```

### Comparing `imsize-1.3.2/imsize/exrhdr.py` & `imsize-1.3.3/src/exrhdr.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.2/imsize/imsize.py` & `imsize-1.3.3/src/imsize.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 """
 Extracts image dimensions, bit depth, and other basic metadata.
+
+Example:
+  info = imsize.read("myfile.jpg")
+  factor = info.nbytes / info.filesize
+  print(f"{info.filespec}: compression factor = {factor.1f}")
+
+https://github.com/toaarnio/imsize
 """
 
 import os              # built-in library
 import math            # built-in library
 import struct          # built-in library
 import ast             # built-in library
 import pprint          # built-in library
@@ -19,14 +26,20 @@
     from imsize import exrhdr   # local import: exrhdr.py
 except ImportError:
     # stand-alone mode
     import pnmhdr
     import pfmhdr
     import exrhdr
 
+# Fetch version number from pyproject.toml
+
+import importlib.metadata  # built-in library
+
+__version__ = importlib.metadata.version(__package__ or __name__)
+
 
 ######################################################################################
 #
 #  P U B L I C   A P I
 #
 ######################################################################################
```

### Comparing `imsize-1.3.2/imsize/pfmhdr.py` & `imsize-1.3.3/src/pfmhdr.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.2/imsize/pnmhdr.py` & `imsize-1.3.3/src/pnmhdr.py`

 * *Files identical despite different names*

### Comparing `imsize-1.3.2/test/test_read.py` & `imsize-1.3.3/test/test_read.py`

 * *Files identical despite different names*

