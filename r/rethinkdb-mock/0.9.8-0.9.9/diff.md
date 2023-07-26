# Comparing `tmp/rethinkdb_mock-0.9.8.tar.gz` & `tmp/rethinkdb_mock-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rethinkdb_mock-0.9.8.tar", last modified: Tue Jan 19 12:51:17 2021, max compression
+gzip compressed data, was "rethinkdb_mock-0.9.9.tar", last modified: Tue Jan 19 17:11:10 2021, max compression
```

## Comparing `rethinkdb_mock-0.9.8.tar` & `rethinkdb_mock-0.9.9.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 12:51:17.056176 rethinkdb_mock-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      473 2021-01-19 12:51:17.056176 rethinkdb_mock-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5528 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 12:51:17.052176 rethinkdb_mock-0.9.8/rethinkdb_mock/
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/rethinkdb_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28814 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/rethinkdb_mock/ast.py
--rw-r--r--   0 runner    (1001) docker     (121)     8544 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/rethinkdb_mock/ast_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    12921 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/rethinkdb_mock/db.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/rethinkdb_mock/joins.py
--rw-r--r--   0 runner    (1001) docker     (121)    15769 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/rethinkdb_mock/rql_rewrite.py
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/rethinkdb_mock/rtime.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/rethinkdb_mock/scope.py
--rw-r--r--   0 runner    (1001) docker     (121)     9178 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/rethinkdb_mock/util.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/rethinkdb_mock/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-01-19 12:51:17.056176 rethinkdb_mock-0.9.8/rethinkdb_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      473 2021-01-19 12:51:16.000000 rethinkdb_mock-0.9.8/rethinkdb_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      498 2021-01-19 12:51:17.000000 rethinkdb_mock-0.9.8/rethinkdb_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-01-19 12:51:16.000000 rethinkdb_mock-0.9.8/rethinkdb_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-01-19 12:51:16.000000 rethinkdb_mock-0.9.8/rethinkdb_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-01-19 12:51:17.000000 rethinkdb_mock-0.9.8/rethinkdb_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-01-19 12:51:16.000000 rethinkdb_mock-0.9.8/rethinkdb_mock.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-01-19 12:51:17.056176 rethinkdb_mock-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      751 2021-01-19 12:51:14.000000 rethinkdb_mock-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:11:10.982434 rethinkdb_mock-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     7430 2021-01-19 17:11:10.982434 rethinkdb_mock-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     5527 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:11:10.978434 rethinkdb_mock-0.9.9/rethinkdb_mock/
+-rw-r--r--   0 runner    (1001) docker     (116)       53 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/rethinkdb_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28814 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/rethinkdb_mock/ast.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8544 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/rethinkdb_mock/ast_base.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12921 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/rethinkdb_mock/db.py
+-rw-r--r--   0 runner    (1001) docker     (116)      971 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/rethinkdb_mock/joins.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15769 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/rethinkdb_mock/rql_rewrite.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1489 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/rethinkdb_mock/rtime.py
+-rw-r--r--   0 runner    (1001) docker     (116)      967 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/rethinkdb_mock/scope.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9178 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/rethinkdb_mock/util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-19 17:11:10.982434 rethinkdb_mock-0.9.9/rethinkdb_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     7430 2021-01-19 17:11:10.000000 rethinkdb_mock-0.9.9/rethinkdb_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      472 2021-01-19 17:11:10.000000 rethinkdb_mock-0.9.9/rethinkdb_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 17:11:10.000000 rethinkdb_mock-0.9.9/rethinkdb_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       40 2021-01-19 17:11:10.000000 rethinkdb_mock-0.9.9/rethinkdb_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       15 2021-01-19 17:11:10.000000 rethinkdb_mock-0.9.9/rethinkdb_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-19 17:11:10.000000 rethinkdb_mock-0.9.9/rethinkdb_mock.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       79 2021-01-19 17:11:10.982434 rethinkdb_mock-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      958 2021-01-19 17:11:03.000000 rethinkdb_mock-0.9.9/setup.py
```

### Comparing `rethinkdb_mock-0.9.8/README.md` & `rethinkdb_mock-0.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-![build](https://github.com/Inveracity/rethinkdb-mock/workflows/build/badge.svg?branch=master) ![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Inveracity/bade1568c33344c896cbfa5cdef91270/raw/af4b61e83c8705869dba3f8801a28c07d8c6d3e0/coverage.json) ![python](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Inveracity/5eb80ff1c1b5eedd820a7b827ac02603/raw/e7ac8997ae5bddfec5d6cbc86b948584158acd83/python3.9) ![rethinkdb](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Inveracity/ee29dbdeafff4549e9a7fb0ad114358c/raw/a4f809e51f9c269af81490c03a7c88a38764b8f3/rethinkdb-python)
-
+![build](https://github.com/Inveracity/rethinkdb-mock/workflows/build/badge.svg?branch=master) ![coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Inveracity/bade1568c33344c896cbfa5cdef91270/raw/af4b61e83c8705869dba3f8801a28c07d8c6d3e0/coverage.json) ![python](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Inveracity/5eb80ff1c1b5eedd820a7b827ac02603/raw/0b8d7cb67274354d05cc3defcb522186b3ca01a8/python3.9) ![rethinkdb](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Inveracity/ee29dbdeafff4549e9a7fb0ad114358c/raw/a4f809e51f9c269af81490c03a7c88a38764b8f3/rethinkdb-python)
 
 # RethinkDB Mock
 
 Formerly known as [MockThink](https://github.com/scivey/mockthink) by Scivey, this is a continuation of that work released under a new name.
 
 Rethinkdb-mock is an in-process Python clone of RethinkDB's API. For testing.
```

### Comparing `rethinkdb_mock-0.9.8/rethinkdb_mock/ast.py` & `rethinkdb_mock-0.9.9/rethinkdb_mock/ast.py`

 * *Files identical despite different names*

### Comparing `rethinkdb_mock-0.9.8/rethinkdb_mock/ast_base.py` & `rethinkdb_mock-0.9.9/rethinkdb_mock/ast_base.py`

 * *Files identical despite different names*

### Comparing `rethinkdb_mock-0.9.8/rethinkdb_mock/db.py` & `rethinkdb_mock-0.9.9/rethinkdb_mock/db.py`

 * *Files identical despite different names*

### Comparing `rethinkdb_mock-0.9.8/rethinkdb_mock/joins.py` & `rethinkdb_mock-0.9.9/rethinkdb_mock/joins.py`

 * *Files identical despite different names*

### Comparing `rethinkdb_mock-0.9.8/rethinkdb_mock/rql_rewrite.py` & `rethinkdb_mock-0.9.9/rethinkdb_mock/rql_rewrite.py`

 * *Files identical despite different names*

### Comparing `rethinkdb_mock-0.9.8/rethinkdb_mock/rtime.py` & `rethinkdb_mock-0.9.9/rethinkdb_mock/rtime.py`

 * *Files identical despite different names*

### Comparing `rethinkdb_mock-0.9.8/rethinkdb_mock/scope.py` & `rethinkdb_mock-0.9.9/rethinkdb_mock/scope.py`

 * *Files identical despite different names*

### Comparing `rethinkdb_mock-0.9.8/rethinkdb_mock/util.py` & `rethinkdb_mock-0.9.9/rethinkdb_mock/util.py`

 * *Files identical despite different names*

