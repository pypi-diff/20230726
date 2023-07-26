# Comparing `tmp/zerocap_websocket_test-1.0.7.tar.gz` & `tmp/zerocap_websocket_test-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocap_websocket_test-1.0.7.tar", last modified: Tue Jul 25 02:33:21 2023, max compression
+gzip compressed data, was "zerocap_websocket_test-1.0.9.tar", last modified: Wed Jul 26 03:59:06 2023, max compression
```

## Comparing `zerocap_websocket_test-1.0.7.tar` & `zerocap_websocket_test-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:33:21.449846 zerocap_websocket_test-1.0.7/
--rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-21 07:23:19.000000 zerocap_websocket_test-1.0.7/LICENSE.txt
--rw-r--r--   0 gao        (501) staff       (20)     1067 2023-07-25 02:33:21.449519 zerocap_websocket_test-1.0.7/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)      679 2023-07-25 02:32:36.000000 zerocap_websocket_test-1.0.7/README.md
--rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-25 02:33:21.449936 zerocap_websocket_test-1.0.7/setup.cfg
--rw-r--r--   0 gao        (501) staff       (20)      799 2023-07-25 02:33:18.000000 zerocap_websocket_test-1.0.7/setup.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:33:21.446026 zerocap_websocket_test-1.0.7/zerocap_websocket_test/
--rw-r--r--   0 gao        (501) staff       (20)       80 2023-07-21 08:10:24.000000 zerocap_websocket_test-1.0.7/zerocap_websocket_test/__init__.py
--rw-r--r--   0 gao        (501) staff       (20)     3259 2023-07-25 01:52:08.000000 zerocap_websocket_test-1.0.7/zerocap_websocket_test/main.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-25 02:33:21.448998 zerocap_websocket_test-1.0.7/zerocap_websocket_test.egg-info/
--rw-r--r--   0 gao        (501) staff       (20)     1067 2023-07-25 02:33:21.000000 zerocap_websocket_test-1.0.7/zerocap_websocket_test.egg-info/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)      325 2023-07-25 02:33:21.000000 zerocap_websocket_test-1.0.7/zerocap_websocket_test.egg-info/SOURCES.txt
--rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-25 02:33:21.000000 zerocap_websocket_test-1.0.7/zerocap_websocket_test.egg-info/dependency_links.txt
--rw-r--r--   0 gao        (501) staff       (20)       19 2023-07-25 02:33:21.000000 zerocap_websocket_test-1.0.7/zerocap_websocket_test.egg-info/requires.txt
--rw-r--r--   0 gao        (501) staff       (20)       23 2023-07-25 02:33:21.000000 zerocap_websocket_test-1.0.7/zerocap_websocket_test.egg-info/top_level.txt
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-26 03:59:06.471555 zerocap_websocket_test-1.0.9/
+-rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-21 07:23:19.000000 zerocap_websocket_test-1.0.9/LICENSE.txt
+-rw-r--r--   0 gao        (501) staff       (20)     1271 2023-07-26 03:59:06.471254 zerocap_websocket_test-1.0.9/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)      883 2023-07-26 03:55:43.000000 zerocap_websocket_test-1.0.9/README.rst
+-rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-26 03:59:06.471642 zerocap_websocket_test-1.0.9/setup.cfg
+-rw-r--r--   0 gao        (501) staff       (20)      800 2023-07-26 03:59:04.000000 zerocap_websocket_test-1.0.9/setup.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-26 03:59:06.468125 zerocap_websocket_test-1.0.9/zerocap_websocket_test/
+-rw-r--r--   0 gao        (501) staff       (20)       80 2023-07-21 08:10:24.000000 zerocap_websocket_test-1.0.9/zerocap_websocket_test/__init__.py
+-rw-r--r--   0 gao        (501) staff       (20)     3259 2023-07-25 01:52:08.000000 zerocap_websocket_test-1.0.9/zerocap_websocket_test/main.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-26 03:59:06.470860 zerocap_websocket_test-1.0.9/zerocap_websocket_test.egg-info/
+-rw-r--r--   0 gao        (501) staff       (20)     1271 2023-07-26 03:59:06.000000 zerocap_websocket_test-1.0.9/zerocap_websocket_test.egg-info/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)      326 2023-07-26 03:59:06.000000 zerocap_websocket_test-1.0.9/zerocap_websocket_test.egg-info/SOURCES.txt
+-rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-26 03:59:06.000000 zerocap_websocket_test-1.0.9/zerocap_websocket_test.egg-info/dependency_links.txt
+-rw-r--r--   0 gao        (501) staff       (20)       19 2023-07-26 03:59:06.000000 zerocap_websocket_test-1.0.9/zerocap_websocket_test.egg-info/requires.txt
+-rw-r--r--   0 gao        (501) staff       (20)       23 2023-07-26 03:59:06.000000 zerocap_websocket_test-1.0.9/zerocap_websocket_test.egg-info/top_level.txt
```

### Comparing `zerocap_websocket_test-1.0.7/LICENSE.txt` & `zerocap_websocket_test-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_websocket_test-1.0.7/PKG-INFO` & `zerocap_websocket_test-1.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,58 @@
 Metadata-Version: 2.1
 Name: zerocap_websocket_test
-Version: 1.0.7
+Version: 1.0.9
 Summary: websocket_test
 Home-page: 
 Author: jiayu.gao
 Author-email: y18362683626@gmail.com
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 License-File: LICENSE.txt
 
-# pip install zerocap-websocket-test -i https://www.pypi.org/simple/
+.. _pip-install-zerocap-websocket-test--i-httpswwwpypiorgsimple:
 
+pip install zerocap-websocket-test -i https://www.pypi.org/simple/
+==================================================================
 
-# demo:
+demo:
 
-# from zerocap_websocket_test import ZerocapWebsocketTest
-# # API key and secret required
-# apiKey = "***"
-# apiSecret = "***"
-# 
-# websocket = ZerocapWebsocketTest(apiKey, apiSecret)
-# 
-# # Subscribe to Market data
-# market_connect = websocket.get_market()
-# 
-# # Subscription order updates and transaction records
-# orders_connect = websocket.get_orders()
-# 
-# while True:
-#     # Get subscription messages
-#     message = websocket.get_message(market_connect)
-# 
-#     print(f"Receiving message from server: \n{message}")
-#     if not message:
-#         print("Connection close")
-#         break
+from zerocap_websocket_test import ZerocapWebsocketTest
+
+API key and secret required
+===========================
+
+apiKey = ""
+
+apiSecret = ""
+
+websocket = ZerocapWebsocketTest(apiKey, apiSecret)
+
+Subscribe to Market data
+========================
+
+market_connect = websocket.get_market()
+
+Subscription order updates and transaction records
+==================================================
+
+orders_connect = websocket.get_orders()
+
+while True:
+
+::
+
+      # Get subscription messages
+
+      message = websocket.get_message(market_connect)
+
+      print(f"Receiving message from server: \n{message}")
+
+      if not message:
+
+          print("Connection close")
+
+          break
```

### Comparing `zerocap_websocket_test-1.0.7/setup.py` & `zerocap_websocket_test-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from distutils.core import setup
 from setuptools import find_packages
 
-with open("README.MD", "r") as f:
+with open("README.rst", "r") as f:
   long_description = f.read()
 
 REQUIRED = [
     'requests',
     'websocket'
 ]
 
 setup(name='zerocap_websocket_test',  # 包名
-      version='1.0.7',  # 版本号
+      version='1.0.9',  # 版本号
       description='websocket_test',
       long_description=long_description,
       author='jiayu.gao',
       author_email='y18362683626@gmail.com',
       url='',
       install_requires=REQUIRED,
       license='BSD License',
```

### Comparing `zerocap_websocket_test-1.0.7/zerocap_websocket_test/main.py` & `zerocap_websocket_test-1.0.9/zerocap_websocket_test/main.py`

 * *Files identical despite different names*

### Comparing `zerocap_websocket_test-1.0.7/zerocap_websocket_test.egg-info/PKG-INFO` & `zerocap_websocket_test-1.0.9/zerocap_websocket_test.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,58 @@
 Metadata-Version: 2.1
 Name: zerocap-websocket-test
-Version: 1.0.7
+Version: 1.0.9
 Summary: websocket_test
 Home-page: 
 Author: jiayu.gao
 Author-email: y18362683626@gmail.com
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 License-File: LICENSE.txt
 
-# pip install zerocap-websocket-test -i https://www.pypi.org/simple/
+.. _pip-install-zerocap-websocket-test--i-httpswwwpypiorgsimple:
 
+pip install zerocap-websocket-test -i https://www.pypi.org/simple/
+==================================================================
 
-# demo:
+demo:
 
-# from zerocap_websocket_test import ZerocapWebsocketTest
-# # API key and secret required
-# apiKey = "***"
-# apiSecret = "***"
-# 
-# websocket = ZerocapWebsocketTest(apiKey, apiSecret)
-# 
-# # Subscribe to Market data
-# market_connect = websocket.get_market()
-# 
-# # Subscription order updates and transaction records
-# orders_connect = websocket.get_orders()
-# 
-# while True:
-#     # Get subscription messages
-#     message = websocket.get_message(market_connect)
-# 
-#     print(f"Receiving message from server: \n{message}")
-#     if not message:
-#         print("Connection close")
-#         break
+from zerocap_websocket_test import ZerocapWebsocketTest
+
+API key and secret required
+===========================
+
+apiKey = ""
+
+apiSecret = ""
+
+websocket = ZerocapWebsocketTest(apiKey, apiSecret)
+
+Subscribe to Market data
+========================
+
+market_connect = websocket.get_market()
+
+Subscription order updates and transaction records
+==================================================
+
+orders_connect = websocket.get_orders()
+
+while True:
+
+::
+
+      # Get subscription messages
+
+      message = websocket.get_message(market_connect)
+
+      print(f"Receiving message from server: \n{message}")
+
+      if not message:
+
+          print("Connection close")
+
+          break
```

