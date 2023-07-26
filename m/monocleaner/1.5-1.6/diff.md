# Comparing `tmp/monocleaner-1.5.tar.gz` & `tmp/monocleaner-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monocleaner-1.5.tar", last modified: Fri Jul 14 09:43:28 2023, max compression
+gzip compressed data, was "monocleaner-1.6.tar", last modified: Wed Jul 26 11:10:04 2023, max compression
```

## Comparing `monocleaner-1.5.tar` & `monocleaner-1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 09:43:28.646980 monocleaner-1.5/
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-07-14 09:43:13.000000 monocleaner-1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     6114 2023-07-14 09:43:28.646980 monocleaner-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5020 2023-07-14 09:43:13.000000 monocleaner-1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1539 2023-07-14 09:43:13.000000 monocleaner-1.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 09:43:28.642980 monocleaner-1.5/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1304 2023-07-14 09:43:13.000000 monocleaner-1.5/scripts/monocleaner-download
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-14 09:43:28.646980 monocleaner-1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 09:43:28.642980 monocleaner-1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 09:43:28.646980 monocleaner-1.5/src/monocleaner/
--rw-r--r--   0 runner    (1001) docker     (122)       77 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7703 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/hardrules.py
--rw-r--r--   0 runner    (1001) docker     (122)    13458 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/lm.py
--rw-r--r--   0 runner    (1001) docker     (122)     6516 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/monocleaner.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/monocleaner_train.py
--rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/normalize.py
--rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-07-14 09:43:13.000000 monocleaner-1.5/src/monocleaner/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-14 09:43:28.646980 monocleaner-1.5/src/monocleaner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6114 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      526 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      116 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-14 09:43:28.000000 monocleaner-1.5/src/monocleaner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 11:10:04.386776 monocleaner-1.6/
+-rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-07-26 11:09:54.000000 monocleaner-1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    11218 2023-07-26 11:10:04.386776 monocleaner-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    10124 2023-07-26 11:09:54.000000 monocleaner-1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1592 2023-07-26 11:09:54.000000 monocleaner-1.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 11:10:04.382776 monocleaner-1.6/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1304 2023-07-26 11:09:54.000000 monocleaner-1.6/scripts/monocleaner-download
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-26 11:10:04.386776 monocleaner-1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 11:10:04.382776 monocleaner-1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 11:10:04.386776 monocleaner-1.6/src/monocleaner/
+-rw-r--r--   0 runner    (1001) docker     (122)       77 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14650 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/hardrules.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13458 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/lm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6516 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/monocleaner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/monocleaner_train.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6878 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2193 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3124 2023-07-26 11:09:54.000000 monocleaner-1.6/src/monocleaner/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-26 11:10:04.386776 monocleaner-1.6/src/monocleaner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    11218 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      526 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-07-26 11:10:04.000000 monocleaner-1.6/src/monocleaner.egg-info/top_level.txt
```

### Comparing `monocleaner-1.5/LICENSE` & `monocleaner-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `monocleaner-1.5/pyproject.toml` & `monocleaner-1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "monocleaner"
-version = "1.5"
+version = "1.6"
 requires-python = ">=3.8"
 authors = [
     { name = "Prompsit Language Engineering", email = "info@prompsit.com" },
 ]
 maintainers = [
     { name = "Jaume Zaragoza", email = "jzaragoza@prompsit.com" },
 ]
@@ -50,7 +50,8 @@
 script-files = [
     "scripts/monocleaner-download",
 ]
 
 [project.scripts]
 monocleaner = "monocleaner.monocleaner:main"
 monocleaner-train = "monocleaner.monocleaner_train:main"
+monocleaner-hardrules = "monocleaner.hardrules:main"
```

### Comparing `monocleaner-1.5/scripts/monocleaner-download` & `monocleaner-1.6/scripts/monocleaner-download`

 * *Files identical despite different names*

### Comparing `monocleaner-1.5/src/monocleaner/lm.py` & `monocleaner-1.6/src/monocleaner/lm.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.5/src/monocleaner/monocleaner.py` & `monocleaner-1.6/src/monocleaner/monocleaner.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.5/src/monocleaner/monocleaner_train.py` & `monocleaner-1.6/src/monocleaner/monocleaner_train.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.5/src/monocleaner/normalize.py` & `monocleaner-1.6/src/monocleaner/normalize.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.5/src/monocleaner/tokenizer.py` & `monocleaner-1.6/src/monocleaner/tokenizer.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.5/src/monocleaner/util.py` & `monocleaner-1.6/src/monocleaner/util.py`

 * *Files identical despite different names*

### Comparing `monocleaner-1.5/src/monocleaner.egg-info/SOURCES.txt` & `monocleaner-1.6/src/monocleaner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

