# Comparing `tmp/metrapy-0.1.1.tar.gz` & `tmp/metrapy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metrapy-0.1.1.tar", last modified: Tue Jul 25 04:44:40 2023, max compression
+gzip compressed data, was "metrapy-0.1.2.tar", last modified: Wed Jul 26 18:05:57 2023, max compression
```

## Comparing `metrapy-0.1.1.tar` & `metrapy-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 04:44:40.037428 metrapy-0.1.1/
--rw-rw-rw-   0        0        0     2670 2023-07-25 04:44:40.036433 metrapy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2347 2023-07-19 20:01:09.000000 metrapy-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 04:44:40.007860 metrapy-0.1.1/metrapy/
--rw-rw-rw-   0        0        0        0 2023-07-25 03:44:41.000000 metrapy-0.1.1/metrapy/__init__.py
--rw-rw-rw-   0        0        0    13702 2023-07-19 19:30:36.000000 metrapy-0.1.1/metrapy/connector.py
--rw-rw-rw-   0        0        0      205 2023-07-19 19:33:58.000000 metrapy-0.1.1/metrapy/defaults.py
--rw-rw-rw-   0        0        0     2414 2023-07-19 19:32:18.000000 metrapy-0.1.1/metrapy/maps.py
--rw-rw-rw-   0        0        0     1877 2023-07-19 19:33:47.000000 metrapy-0.1.1/metrapy/sync.py
--rw-rw-rw-   0        0        0      607 2023-07-19 19:33:51.000000 metrapy-0.1.1/metrapy/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-25 04:44:40.035431 metrapy-0.1.1/metrapy.egg-info/
--rw-rw-rw-   0        0        0     2670 2023-07-25 04:44:39.000000 metrapy-0.1.1/metrapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-25 04:44:39.000000 metrapy-0.1.1/metrapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 04:44:39.000000 metrapy-0.1.1/metrapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-25 04:44:39.000000 metrapy-0.1.1/metrapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-07-25 04:44:39.000000 metrapy-0.1.1/metrapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 04:44:40.037428 metrapy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1081 2023-07-25 04:44:37.000000 metrapy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:05:57.210042 metrapy-0.1.2/
+-rw-rw-rw-   0        0        0     2670 2023-07-26 18:05:57.210042 metrapy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2347 2023-07-19 20:01:09.000000 metrapy-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 18:05:57.170042 metrapy-0.1.2/metrapy/
+-rw-rw-rw-   0        0        0        0 2023-07-25 03:44:41.000000 metrapy-0.1.2/metrapy/__init__.py
+-rw-rw-rw-   0        0        0    13803 2023-07-26 18:03:45.000000 metrapy-0.1.2/metrapy/connector.py
+-rw-rw-rw-   0        0        0      205 2023-07-19 19:33:58.000000 metrapy-0.1.2/metrapy/defaults.py
+-rw-rw-rw-   0        0        0     2414 2023-07-19 19:32:18.000000 metrapy-0.1.2/metrapy/maps.py
+-rw-rw-rw-   0        0        0     1877 2023-07-19 19:33:47.000000 metrapy-0.1.2/metrapy/sync.py
+-rw-rw-rw-   0        0        0      607 2023-07-19 19:33:51.000000 metrapy-0.1.2/metrapy/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 18:05:57.202043 metrapy-0.1.2/metrapy.egg-info/
+-rw-rw-rw-   0        0        0     2670 2023-07-26 18:05:56.000000 metrapy-0.1.2/metrapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-07-26 18:05:56.000000 metrapy-0.1.2/metrapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 18:05:56.000000 metrapy-0.1.2/metrapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-26 18:05:56.000000 metrapy-0.1.2/metrapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-07-26 18:05:56.000000 metrapy-0.1.2/metrapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 18:05:57.210042 metrapy-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2023-07-26 18:04:49.000000 metrapy-0.1.2/setup.py
```

### Comparing `metrapy-0.1.1/PKG-INFO` & `metrapy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrapy
-Version: 0.1.1
+Version: 0.1.2
 Summary: batteries included wrapper utility for MetaTrader5's python integration
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `metrapy-0.1.1/README.md` & `metrapy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.1/metrapy/connector.py` & `metrapy-0.1.2/metrapy/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,20 +70,22 @@
             self.magic = params['magic_id']
 
     def get_account_info(self):
         return mt5.account_info()._asdict()
 
     def get_tickers(self, params={}):
         if "ticker" in params:
-            return mt5.symbol_info(params["ticker"])
+            sym = mt5.symbol_info(params["ticker"])
+            return filter_props(sym._asdict(), params["filter_props"])
 
         if "group" in params:
-            return mt5.symbols_get(group=params["group"])
-
-        symbols = mt5.symbols_get()
+            symbols = mt5.symbols_get(group=params["group"])
+        else:
+            symbols = mt5.symbols_get()
+        
         tickers = []
 
         for sym in symbols:
             if "filter_props" in params:
                 tickers.append(filter_props(sym._asdict(), params["filter_props"]))
                 continue
```

### Comparing `metrapy-0.1.1/metrapy/maps.py` & `metrapy-0.1.2/metrapy/maps.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.1/metrapy/sync.py` & `metrapy-0.1.2/metrapy/sync.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.1/metrapy/utils.py` & `metrapy-0.1.2/metrapy/utils.py`

 * *Files identical despite different names*

### Comparing `metrapy-0.1.1/metrapy.egg-info/PKG-INFO` & `metrapy-0.1.2/metrapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metrapy
-Version: 0.1.1
+Version: 0.1.2
 Summary: batteries included wrapper utility for MetaTrader5's python integration
 Author: pavittarx
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `metrapy-0.1.1/setup.py` & `metrapy-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="metrapy",  # This is the name of the package
-    version="0.1.1",  # The initial release version
+    version="0.1.2",  # The initial release version
     author="pavittarx",  # Full name of the author
     description="batteries included wrapper utility for MetaTrader5's python integration",
     long_description=long_description,  # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),  # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

