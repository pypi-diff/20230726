# Comparing `tmp/metabolabpytools-0.9.5.tar.gz` & `tmp/metabolabpytools-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metabolabpytools-0.9.5.tar", last modified: Tue Jul 25 19:33:25 2023, max compression
+gzip compressed data, was "metabolabpytools-0.9.6.tar", last modified: Tue Jul 25 22:36:58 2023, max compression
```

## Comparing `metabolabpytools-0.9.5.tar` & `metabolabpytools-0.9.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:33:25.554418 metabolabpytools-0.9.5/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079    35149 2023-06-29 16:08:10.000000 metabolabpytools-0.9.5/LICENSE
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       78 2023-06-29 16:08:10.000000 metabolabpytools-0.9.5/MANIFEST.in
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     3709 2023-07-25 19:33:25.554240 metabolabpytools-0.9.5/PKG-INFO
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       67 2023-06-29 16:08:10.000000 metabolabpytools-0.9.5/README.md
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     2977 2023-06-29 16:08:10.000000 metabolabpytools-0.9.5/README.rst
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:33:25.553013 metabolabpytools-0.9.5/metabolabpytools/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      153 2023-07-25 19:29:45.000000 metabolabpytools-0.9.5/metabolabpytools/__init__.py
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     1893 2023-06-29 16:08:10.000000 metabolabpytools-0.9.5/metabolabpytools/analysis.py
--rw-r--r--   0 ludwigc  (1699341573) 1311385079    25753 2023-07-16 14:50:21.000000 metabolabpytools-0.9.5/metabolabpytools/isotopomerAnalysis.py
-drwxr-xr-x   0 ludwigc  (1699341573) 1311385079        0 2023-07-25 19:33:25.554064 metabolabpytools-0.9.5/metabolabpytools.egg-info/
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     3709 2023-07-25 19:33:25.000000 metabolabpytools-0.9.5/metabolabpytools.egg-info/PKG-INFO
--rw-r--r--   0 ludwigc  (1699341573) 1311385079      362 2023-07-25 19:33:25.000000 metabolabpytools-0.9.5/metabolabpytools.egg-info/SOURCES.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079        1 2023-07-25 19:33:25.000000 metabolabpytools-0.9.5/metabolabpytools.egg-info/dependency_links.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       19 2023-07-25 19:33:25.000000 metabolabpytools-0.9.5/metabolabpytools.egg-info/requires.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       17 2023-07-25 19:33:25.000000 metabolabpytools-0.9.5/metabolabpytools.egg-info/top_level.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       19 2023-06-29 16:08:10.000000 metabolabpytools-0.9.5/requirements.txt
--rw-r--r--   0 ludwigc  (1699341573) 1311385079       38 2023-07-25 19:33:25.554476 metabolabpytools-0.9.5/setup.cfg
--rw-r--r--   0 ludwigc  (1699341573) 1311385079     1507 2023-06-29 16:08:10.000000 metabolabpytools-0.9.5/setup.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:58.898213 metabolabpytools-0.9.6/
+-rw-r--r--   0 ludwigc    (501) staff       (20)    35149 2023-07-11 16:28:03.000000 metabolabpytools-0.9.6/LICENSE
+-rw-r--r--   0 ludwigc    (501) staff       (20)       78 2023-07-11 16:28:03.000000 metabolabpytools-0.9.6/MANIFEST.in
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3709 2023-07-25 22:36:58.898081 metabolabpytools-0.9.6/PKG-INFO
+-rw-r--r--   0 ludwigc    (501) staff       (20)       67 2023-07-11 16:28:03.000000 metabolabpytools-0.9.6/README.md
+-rw-r--r--   0 ludwigc    (501) staff       (20)     2977 2023-07-11 16:28:03.000000 metabolabpytools-0.9.6/README.rst
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:58.896861 metabolabpytools-0.9.6/metabolabpytools/
+-rw-r--r--   0 ludwigc    (501) staff       (20)      153 2023-07-25 22:36:52.000000 metabolabpytools-0.9.6/metabolabpytools/__init__.py
+-rw-r--r--   0 ludwigc    (501) staff       (20)     1893 2023-07-11 16:28:03.000000 metabolabpytools-0.9.6/metabolabpytools/analysis.py
+-rw-r--r--   0 ludwigc    (501) staff       (20)    25753 2023-07-16 14:32:50.000000 metabolabpytools-0.9.6/metabolabpytools/isotopomerAnalysis.py
+drwxr-xr-x   0 ludwigc    (501) staff       (20)        0 2023-07-25 22:36:58.897895 metabolabpytools-0.9.6/metabolabpytools.egg-info/
+-rw-r--r--   0 ludwigc    (501) staff       (20)     3709 2023-07-25 22:36:58.000000 metabolabpytools-0.9.6/metabolabpytools.egg-info/PKG-INFO
+-rw-r--r--   0 ludwigc    (501) staff       (20)      362 2023-07-25 22:36:58.000000 metabolabpytools-0.9.6/metabolabpytools.egg-info/SOURCES.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)        1 2023-07-25 22:36:58.000000 metabolabpytools-0.9.6/metabolabpytools.egg-info/dependency_links.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       19 2023-07-25 22:36:58.000000 metabolabpytools-0.9.6/metabolabpytools.egg-info/requires.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       17 2023-07-25 22:36:58.000000 metabolabpytools-0.9.6/metabolabpytools.egg-info/top_level.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       19 2023-07-11 16:28:03.000000 metabolabpytools-0.9.6/requirements.txt
+-rw-r--r--   0 ludwigc    (501) staff       (20)       38 2023-07-25 22:36:58.898258 metabolabpytools-0.9.6/setup.cfg
+-rw-r--r--   0 ludwigc    (501) staff       (20)     1507 2023-07-11 16:28:03.000000 metabolabpytools-0.9.6/setup.py
```

### Comparing `metabolabpytools-0.9.5/LICENSE` & `metabolabpytools-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.5/PKG-INFO` & `metabolabpytools-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolabpytools
-Version: 0.9.5
+Version: 0.9.6
 Summary: Tools for metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/metabolabpytools
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `metabolabpytools-0.9.5/README.rst` & `metabolabpytools-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.5/metabolabpytools/analysis.py` & `metabolabpytools-0.9.6/metabolabpytools/analysis.py`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.5/metabolabpytools/isotopomerAnalysis.py` & `metabolabpytools-0.9.6/metabolabpytools/isotopomerAnalysis.py`

 * *Files identical despite different names*

### Comparing `metabolabpytools-0.9.5/metabolabpytools.egg-info/PKG-INFO` & `metabolabpytools-0.9.6/metabolabpytools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metabolabpytools
-Version: 0.9.5
+Version: 0.9.6
 Summary: Tools for metabolomics and metabolism tracing data
 Home-page: https://github.com/ludwigc/metabolabpytools
 Author: Christian Ludwig
 Author-email: C.Ludwig@bham.ac.uk 
 License: GPLv3
 Keywords: Metabolomics,Tracing,NMR,Data Processing,13C
 Platform: MacOS, Windows, UNIX
```

### Comparing `metabolabpytools-0.9.5/setup.py` & `metabolabpytools-0.9.6/setup.py`

 * *Files identical despite different names*

