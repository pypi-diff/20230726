# Comparing `tmp/mcqgen-0.1.1.tar.gz` & `tmp/mcqgen-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqgen-0.1.1.tar", last modified: Tue Jul 25 23:50:37 2023, max compression
+gzip compressed data, was "mcqgen-0.1.2.tar", last modified: Wed Jul 26 00:02:00 2023, max compression
```

## Comparing `mcqgen-0.1.1.tar` & `mcqgen-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:50:37.089870 mcqgen-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 23:50:35.000000 mcqgen-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-25 23:50:37.089870 mcqgen-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-25 23:50:35.000000 mcqgen-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:50:37.089870 mcqgen-0.1.1/mcqgen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:50:35.000000 mcqgen-0.1.1/mcqgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-25 23:50:35.000000 mcqgen-0.1.1/mcqgen/mcqgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:50:37.089870 mcqgen-0.1.1/mcqgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-25 23:50:37.000000 mcqgen-0.1.1/mcqgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 23:50:37.000000 mcqgen-0.1.1/mcqgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:50:37.000000 mcqgen-0.1.1/mcqgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 23:50:37.000000 mcqgen-0.1.1/mcqgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 23:50:37.000000 mcqgen-0.1.1/mcqgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:50:37.089870 mcqgen-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-25 23:50:35.000000 mcqgen-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:02:00.673528 mcqgen-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 00:01:56.000000 mcqgen-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-26 00:02:00.673528 mcqgen-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-26 00:01:56.000000 mcqgen-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:02:00.673528 mcqgen-0.1.2/mcqgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:01:56.000000 mcqgen-0.1.2/mcqgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-26 00:01:56.000000 mcqgen-0.1.2/mcqgen/mcqgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:02:00.673528 mcqgen-0.1.2/mcqgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-26 00:02:00.000000 mcqgen-0.1.2/mcqgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-26 00:02:00.000000 mcqgen-0.1.2/mcqgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:02:00.000000 mcqgen-0.1.2/mcqgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:02:00.000000 mcqgen-0.1.2/mcqgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:02:00.000000 mcqgen-0.1.2/mcqgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 00:02:00.673528 mcqgen-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-26 00:01:56.000000 mcqgen-0.1.2/setup.py
```

### Comparing `mcqgen-0.1.1/LICENSE` & `mcqgen-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqgen-0.1.1/mcqgen/mcqgen.py` & `mcqgen-0.1.2/mcqgen/mcqgen.py`

 * *Files identical despite different names*

