# Comparing `tmp/finterion-0.5.tar.gz` & `tmp/finterion-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finterion-0.5.tar", last modified: Wed Jul 26 09:31:39 2023, max compression
+gzip compressed data, was "finterion-0.5.1.tar", last modified: Wed Jul 26 14:27:08 2023, max compression
```

## Comparing `finterion-0.5.tar` & `finterion-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:31:39.408514 finterion-0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-26 09:31:28.000000 finterion-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-26 09:31:39.408514 finterion-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-26 09:31:28.000000 finterion-0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:31:39.404513 finterion-0.5/finterion/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-26 09:31:28.000000 finterion-0.5/finterion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:31:39.408514 finterion-0.5/finterion/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 09:31:28.000000 finterion-0.5/finterion/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-26 09:31:28.000000 finterion-0.5/finterion/configuration/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 09:31:28.000000 finterion-0.5/finterion/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-26 09:31:28.000000 finterion-0.5/finterion/finterion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:31:39.408514 finterion-0.5/finterion/models/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 09:31:28.000000 finterion-0.5/finterion/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-26 09:31:28.000000 finterion-0.5/finterion/models/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 09:31:28.000000 finterion-0.5/finterion/models/algorithm_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-26 09:31:28.000000 finterion-0.5/finterion/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-26 09:31:28.000000 finterion-0.5/finterion/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 09:31:28.000000 finterion-0.5/finterion/models/order_side.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 09:31:28.000000 finterion-0.5/finterion/models/order_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-26 09:31:28.000000 finterion-0.5/finterion/models/order_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-26 09:31:28.000000 finterion-0.5/finterion/models/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-26 09:31:28.000000 finterion-0.5/finterion/models/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-26 09:31:28.000000 finterion-0.5/finterion/services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 09:31:39.408514 finterion-0.5/finterion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-26 09:31:39.000000 finterion-0.5/finterion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-26 09:31:39.000000 finterion-0.5/finterion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 09:31:39.000000 finterion-0.5/finterion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 09:31:39.000000 finterion-0.5/finterion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 09:31:39.000000 finterion-0.5/finterion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 09:31:39.408514 finterion-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-26 09:31:28.000000 finterion-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:08.988398 finterion-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-07-26 14:26:58.000000 finterion-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-26 14:27:08.988398 finterion-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-26 14:26:58.000000 finterion-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:08.984398 finterion-0.5.1/finterion/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:08.984398 finterion-0.5.1/finterion/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/configuration/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/finterion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:08.988398 finterion-0.5.1/finterion/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/algorithm_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/order_side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/order_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/models/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-26 14:26:58.000000 finterion-0.5.1/finterion/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:27:08.984398 finterion-0.5.1/finterion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-26 14:27:08.000000 finterion-0.5.1/finterion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-26 14:27:08.000000 finterion-0.5.1/finterion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:27:08.000000 finterion-0.5.1/finterion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-26 14:27:08.000000 finterion-0.5.1/finterion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 14:27:08.000000 finterion-0.5.1/finterion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:27:08.988398 finterion-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-26 14:26:58.000000 finterion-0.5.1/setup.py
```

### Comparing `finterion-0.5/LICENSE` & `finterion-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `finterion-0.5/PKG-INFO` & `finterion-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion
-Version: 0.5
+Version: 0.5.1
 Summary: Official python client for Finterion
 Home-page: https://github.com/finterion/finterion-python-client.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `finterion-0.5/README.md` & `finterion-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion/configuration/urls.py` & `finterion-0.5.1/finterion/configuration/urls.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion/finterion.py` & `finterion-0.5.1/finterion/finterion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from finterion import services, ClientException, OrderSide
 
 
 class Finterion:
 
-    def __init__(self, api_key, base_url="https://api.finterion.com/algs"):
+    def __init__(self, api_key, base_url=None):
         self.api_key = api_key
         self.base_url = base_url
+
+        if self.base_url is None:
+            self.base_url = "https://api.finterion.com/algs"
+
         self.ping()
         self.algorithm = self.get_algorithm_model()
 
     def ping(self):
         return services.ping(self.api_key, base_url=self.base_url)
 
     def get_algorithm_model(self):
```

### Comparing `finterion-0.5/finterion/models/algorithm.py` & `finterion-0.5.1/finterion/models/algorithm.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion/models/algorithm_profile.py` & `finterion-0.5.1/finterion/models/algorithm_profile.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion/models/order.py` & `finterion-0.5.1/finterion/models/order.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion/models/order_side.py` & `finterion-0.5.1/finterion/models/order_side.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion/models/order_status.py` & `finterion-0.5.1/finterion/models/order_status.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion/models/order_type.py` & `finterion-0.5.1/finterion/models/order_type.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion/models/portfolio.py` & `finterion-0.5.1/finterion/models/portfolio.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion/models/position.py` & `finterion-0.5.1/finterion/models/position.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion/services.py` & `finterion-0.5.1/finterion/services.py`

 * *Files identical despite different names*

### Comparing `finterion-0.5/finterion.egg-info/PKG-INFO` & `finterion-0.5.1/finterion.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finterion
-Version: 0.5
+Version: 0.5.1
 Summary: Official python client for Finterion
 Home-page: https://github.com/finterion/finterion-python-client.git
 Author: Finterion
 License: Apache License 2.0
 Keywords: Finterion,finterion,investing-algorithm,INVESTING,BOT,ALGORITHM,FRAMEWORK,investing-bots,trading-bots
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `finterion-0.5/finterion.egg-info/SOURCES.txt` & `finterion-0.5.1/finterion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finterion-0.5/setup.py` & `finterion-0.5.1/setup.py`

 * *Files identical despite different names*

