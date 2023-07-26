# Comparing `tmp/peakventures-1.2.2.tar.gz` & `tmp/peakventures-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakventures-1.2.2.tar", max compression
+gzip compressed data, was "peakventures-1.2.3.tar", max compression
```

## Comparing `peakventures-1.2.2.tar` & `peakventures-1.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.2.2/peakventures/__init__.py
--rw-r--r--   0        0        0     1813 2023-07-12 17:49:47.662944 peakventures-1.2.2/peakventures/api.py
--rw-r--r--   0        0        0     4086 2023-07-26 19:37:35.703756 peakventures-1.2.2/peakventures/conversions.py
--rw-r--r--   0        0        0     1095 2023-07-26 09:29:28.910842 peakventures-1.2.2/peakventures/credentials.py
--rw-r--r--   0        0        0      830 2023-07-26 09:28:36.228718 peakventures-1.2.2/peakventures/storage.py
--rw-r--r--   0        0        0      366 2023-07-26 19:38:56.305020 peakventures-1.2.2/pyproject.toml
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 peakventures-1.2.2/setup.py
--rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 peakventures-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.2.3/peakventures/__init__.py
+-rw-r--r--   0        0        0     1813 2023-07-12 17:49:47.662944 peakventures-1.2.3/peakventures/api.py
+-rw-r--r--   0        0        0     4086 2023-07-26 19:37:35.703756 peakventures-1.2.3/peakventures/conversions.py
+-rw-r--r--   0        0        0     1095 2023-07-26 09:29:28.910842 peakventures-1.2.3/peakventures/credentials.py
+-rw-r--r--   0        0        0      830 2023-07-26 09:28:36.228718 peakventures-1.2.3/peakventures/storage.py
+-rw-r--r--   0        0        0      351 2023-07-26 19:39:24.146134 peakventures-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 peakventures-1.2.3/setup.py
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 peakventures-1.2.3/PKG-INFO
```

### Comparing `peakventures-1.2.2/peakventures/api.py` & `peakventures-1.2.3/peakventures/api.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.2.2/peakventures/conversions.py` & `peakventures-1.2.3/peakventures/conversions.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.2.2/peakventures/credentials.py` & `peakventures-1.2.3/peakventures/credentials.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.2.2/peakventures/storage.py` & `peakventures-1.2.3/peakventures/storage.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.2.2/setup.py` & `peakventures-1.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 install_requires = \
 ['boto3>=1.28.11,<2.0.0',
  'tenacity>=8.2.2,<9.0.0',
  'websockets>=11.0.3,<12.0.0']
 
 setup_kwargs = {
     'name': 'peakventures',
-    'version': '1.2.2',
-    'description': 'PeakVentures Python Utilities for DataBricks',
+    'version': '1.2.3',
+    'description': 'PeakVentures Python Utilities',
     'long_description': 'None',
     'author': 'Volodymyr Smirnov',
     'author_email': 'volodymyr@peakventures.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
```

### Comparing `peakventures-1.2.2/PKG-INFO` & `peakventures-1.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: peakventures
-Version: 1.2.2
-Summary: PeakVentures Python Utilities for DataBricks
+Version: 1.2.3
+Summary: PeakVentures Python Utilities
 Author: Volodymyr Smirnov
 Author-email: volodymyr@peakventures.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

