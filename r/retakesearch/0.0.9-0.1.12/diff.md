# Comparing `tmp/retakesearch-0.0.9.tar.gz` & `tmp/retakesearch-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retakesearch-0.0.9.tar", max compression
+gzip compressed data, was "retakesearch-0.1.12.tar", max compression
```

## Comparing `retakesearch-0.0.9.tar` & `retakesearch-0.1.12.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-07-24 22:36:24.045322 retakesearch-0.0.9/README.md
--rw-r--r--   0        0        0      412 2023-07-24 22:36:42.666471 retakesearch-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      124 2023-07-24 22:36:24.045322 retakesearch-0.0.9/retakesearch/__init__.py
--rw-r--r--   0        0        0     2471 2023-07-24 22:36:24.045322 retakesearch-0.0.9/retakesearch/client.py
--rw-r--r--   0        0        0       67 2023-07-24 22:36:24.045322 retakesearch-0.0.9/retakesearch/search.py
--rw-r--r--   0        0        0      683 1970-01-01 00:00:00.000000 retakesearch-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 16:07:18.332412 retakesearch-0.1.12/README.md
+-rw-r--r--   0        0        0      412 2023-07-26 16:07:39.896618 retakesearch-0.1.12/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-07-26 16:07:18.332412 retakesearch-0.1.12/retakesearch/__init__.py
+-rw-r--r--   0        0        0     2471 2023-07-26 16:07:18.332412 retakesearch-0.1.12/retakesearch/client.py
+-rw-r--r--   0        0        0      159 2023-07-26 16:07:18.332412 retakesearch-0.1.12/retakesearch/search.py
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 retakesearch-0.1.12/PKG-INFO
```

### Comparing `retakesearch-0.0.9/retakesearch/client.py` & `retakesearch-0.1.12/retakesearch/client.py`

 * *Files identical despite different names*

### Comparing `retakesearch-0.0.9/PKG-INFO` & `retakesearch-0.1.12/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: retakesearch
-Version: 0.0.9
-Summary: Open Source Search Infrastructure for Developers
+Version: 0.1.12
+Summary: Open Source Neural Search Engine Python Client
 Author: Ming Ying
 Author-email: ming.ying.nyc@gmail.com
 Requires-Python: >=3.6,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

