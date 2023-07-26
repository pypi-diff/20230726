# Comparing `tmp/unityparser-3.0.0.tar.gz` & `tmp/unityparser-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unityparser-3.0.0.tar", last modified: Fri Jul 21 08:42:41 2023, max compression
+gzip compressed data, was "unityparser-3.0.1.tar", last modified: Wed Jul 26 14:13:05 2023, max compression
```

## Comparing `unityparser-3.0.0.tar` & `unityparser-3.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:42:41.078597 unityparser-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-21 08:42:21.000000 unityparser-3.0.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-21 08:42:21.000000 unityparser-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-21 08:42:21.000000 unityparser-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-21 08:42:41.078597 unityparser-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-21 08:42:21.000000 unityparser-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:42:41.070597 unityparser-3.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/development.in
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/development.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/publish.in
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-21 08:42:21.000000 unityparser-3.0.0/requirements/publish.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-21 08:42:41.078597 unityparser-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-21 08:42:21.000000 unityparser-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:42:41.074597 unityparser-3.0.0/unityparser/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-21 08:42:38.000000 unityparser-3.0.0/unityparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/register.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/representer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-21 08:42:21.000000 unityparser-3.0.0/unityparser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 08:42:41.078597 unityparser-3.0.0/unityparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-21 08:42:41.000000 unityparser-3.0.0/unityparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-21 08:42:41.000000 unityparser-3.0.0/unityparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 08:42:41.000000 unityparser-3.0.0/unityparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-21 08:42:41.000000 unityparser-3.0.0/unityparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-21 08:42:41.000000 unityparser-3.0.0/unityparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:05.649252 unityparser-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-26 14:12:45.000000 unityparser-3.0.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-26 14:12:45.000000 unityparser-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 14:12:45.000000 unityparser-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-26 14:13:05.649252 unityparser-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-26 14:12:45.000000 unityparser-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:05.641251 unityparser-3.0.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/development.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/development.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/publish.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-26 14:12:45.000000 unityparser-3.0.1/requirements/publish.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 14:13:05.649252 unityparser-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-07-26 14:12:45.000000 unityparser-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:05.645251 unityparser-3.0.1/unityparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 14:13:02.000000 unityparser-3.0.1/unityparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/representer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-26 14:12:45.000000 unityparser-3.0.1/unityparser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:13:05.649252 unityparser-3.0.1/unityparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-26 14:13:05.000000 unityparser-3.0.1/unityparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-26 14:13:05.000000 unityparser-3.0.1/unityparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:13:05.000000 unityparser-3.0.1/unityparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-26 14:13:05.000000 unityparser-3.0.1/unityparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 14:13:05.000000 unityparser-3.0.1/unityparser.egg-info/top_level.txt
```

### Comparing `unityparser-3.0.0/LICENSE` & `unityparser-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/PKG-INFO` & `unityparser-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unityparser
-Version: 3.0.0
+Version: 3.0.1
 Summary: A python library to parse and dump Unity YAML files
 Home-page: https://github.com/socialpoint-labs/unity-yaml-parser
 Author: Ricard Valverde
 Author-email: ricard.valverde@socialpoint.es
 License: MIT License
 Keywords: unity,yaml,parser,serializer
 Platform: UNKNOWN
```

### Comparing `unityparser-3.0.0/README.md` & `unityparser-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/requirements/ci.txt` & `unityparser-3.0.1/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/requirements/development.txt` & `unityparser-3.0.1/requirements/development.txt`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/requirements/publish.txt` & `unityparser-3.0.1/requirements/publish.txt`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/setup.py` & `unityparser-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/commands.py` & `unityparser-3.0.1/unityparser/commands.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/composer.py` & `unityparser-3.0.1/unityparser/composer.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/constants.py` & `unityparser-3.0.1/unityparser/constants.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/constructor.py` & `unityparser-3.0.1/unityparser/constructor.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/dumper.py` & `unityparser-3.0.1/unityparser/dumper.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/emitter.py` & `unityparser-3.0.1/unityparser/emitter.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/loader.py` & `unityparser-3.0.1/unityparser/loader.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/parser.py` & `unityparser-3.0.1/unityparser/parser.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/resolver.py` & `unityparser-3.0.1/unityparser/resolver.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/scanner.py` & `unityparser-3.0.1/unityparser/scanner.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/serializer.py` & `unityparser-3.0.1/unityparser/serializer.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser/utils.py` & `unityparser-3.0.1/unityparser/utils.py`

 * *Files identical despite different names*

### Comparing `unityparser-3.0.0/unityparser.egg-info/PKG-INFO` & `unityparser-3.0.1/unityparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unityparser
-Version: 3.0.0
+Version: 3.0.1
 Summary: A python library to parse and dump Unity YAML files
 Home-page: https://github.com/socialpoint-labs/unity-yaml-parser
 Author: Ricard Valverde
 Author-email: ricard.valverde@socialpoint.es
 License: MIT License
 Keywords: unity,yaml,parser,serializer
 Platform: UNKNOWN
```

### Comparing `unityparser-3.0.0/unityparser.egg-info/SOURCES.txt` & `unityparser-3.0.1/unityparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

