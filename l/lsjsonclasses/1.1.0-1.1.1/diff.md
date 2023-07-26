# Comparing `tmp/lsjsonclasses-1.1.0.tar.gz` & `tmp/lsjsonclasses-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsjsonclasses-1.1.0.tar", max compression
+gzip compressed data, was "lsjsonclasses-1.1.1.tar", max compression
```

## Comparing `lsjsonclasses-1.1.0.tar` & `lsjsonclasses-1.1.1.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     1227 2023-07-25 13:46:20.436557 lsjsonclasses-1.1.0/lsjsonclasses/__init__.py
--rw-r--r--   0        0        0      409 2023-07-25 13:46:20.436557 lsjsonclasses-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      430 1970-01-01 00:00:00.000000 lsjsonclasses-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1227 2023-07-25 13:46:20.436557 lsjsonclasses-1.1.1/lsjsonclasses/__init__.py
+-rw-r--r--   0        0        0      407 2023-07-26 06:49:04.419088 lsjsonclasses-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 lsjsonclasses-1.1.1/PKG-INFO
```

### Comparing `lsjsonclasses-1.1.0/lsjsonclasses/__init__.py` & `lsjsonclasses-1.1.1/lsjsonclasses/__init__.py`

 * *Files identical despite different names*

