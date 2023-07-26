# Comparing `tmp/zerocap_api_test-0.1.2.tar.gz` & `tmp/zerocap_api_test-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zerocap_api_test-0.1.2.tar", last modified: Wed Jul 26 06:05:03 2023, max compression
+gzip compressed data, was "zerocap_api_test-0.1.3.tar", last modified: Wed Jul 26 07:08:23 2023, max compression
```

## Comparing `zerocap_api_test-0.1.2.tar` & `zerocap_api_test-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/
--rw-r--r--   0 mac        (501) staff       (20)    11323 2023-07-24 01:35:05.000000 zerocap_api_test-0.1.2/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1404 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1025 2023-07-26 05:48:22.000000 zerocap_api_test-0.1.2/README.rst
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      791 2023-07-26 06:04:52.000000 zerocap_api_test-0.1.2/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test/
--rw-r--r--   0 mac        (501) staff       (20)      121 2023-07-26 05:40:03.000000 zerocap_api_test-0.1.2/zerocap_api_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     7270 2023-07-26 06:04:05.000000 zerocap_api_test-0.1.2/zerocap_api_test/main.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1404 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      284 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       17 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/top_level.txt
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-26 07:08:23.514909 zerocap_api_test-0.1.3/
+-rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-26 06:32:00.000000 zerocap_api_test-0.1.3/LICENSE.txt
+-rw-r--r--   0 gao        (501) staff       (20)     1419 2023-07-26 07:08:23.514564 zerocap_api_test-0.1.3/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)     1039 2023-07-26 06:42:12.000000 zerocap_api_test-0.1.3/README.rst
+-rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-26 07:08:23.515025 zerocap_api_test-0.1.3/setup.cfg
+-rw-r--r--   0 gao        (501) staff       (20)      792 2023-07-26 07:08:15.000000 zerocap_api_test-0.1.3/setup.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-26 07:08:23.511094 zerocap_api_test-0.1.3/zerocap_api_test/
+-rw-r--r--   0 gao        (501) staff       (20)      121 2023-07-26 06:32:00.000000 zerocap_api_test-0.1.3/zerocap_api_test/__init__.py
+-rw-r--r--   0 gao        (501) staff       (20)     6674 2023-07-26 06:57:14.000000 zerocap_api_test-0.1.3/zerocap_api_test/main.py
+drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-26 07:08:23.514102 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/
+-rw-r--r--   0 gao        (501) staff       (20)     1419 2023-07-26 07:08:23.000000 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/PKG-INFO
+-rw-r--r--   0 gao        (501) staff       (20)      284 2023-07-26 07:08:23.000000 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/SOURCES.txt
+-rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-26 07:08:23.000000 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/dependency_links.txt
+-rw-r--r--   0 gao        (501) staff       (20)       19 2023-07-26 07:08:23.000000 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/requires.txt
+-rw-r--r--   0 gao        (501) staff       (20)       17 2023-07-26 07:08:23.000000 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_test-0.1.2/LICENSE.txt` & `zerocap_api_test-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_api_test-0.1.2/PKG-INFO` & `zerocap_api_test-0.1.3/zerocap_api_test.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: zerocap_api_test
-Version: 0.1.2
+Name: zerocap-api-test
+Version: 0.1.3
 Summary: zerocap_api
 Home-page: 
 Author: jiayu.gao
-Author-email: y18362683626@gmail.com
+Author-email: jiayu.gao@eigen.capital
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 License-File: LICENSE.txt
@@ -22,17 +22,17 @@
 rest_api_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
 
     api_key = ""
 
-    secret = ""
+    api_secret = ""
 
-    client = ZerocapRestClient(api_key, secret)
+    client = ZerocapRestClient(api_key, api_secret)
 
     result = client.create_order(symbol, side, type, amount, price, client_order_id, note, third_identity_id)
 
     result = client.fetch_order(id, note, third_identity_id)
 
     result = client.fetch_orders(symbol, since, limit, note, third_identity_id)
 
@@ -40,17 +40,17 @@
 websocket_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
 
     api_key = ""
 
-    secret = ""
+    api_secret = ""
 
-    websocket_client = ZerocapWebsocketTest(apiKey, apiSecret)
+    websocket_client = ZerocapWebsocketTest(api_key, api_secret)
 
     market_connect = websocket_client.get_market()
 
     orders_connect = websocket_client.get_orders()
 
     while True:
```

### Comparing `zerocap_api_test-0.1.2/README.rst` & `zerocap_api_test-0.1.3/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 rest_api_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
 
     api_key = ""
 
-    secret = ""
+    api_secret = ""
 
-    client = ZerocapRestClient(api_key, secret)
+    client = ZerocapRestClient(api_key, api_secret)
 
     result = client.create_order(symbol, side, type, amount, price, client_order_id, note, third_identity_id)
 
     result = client.fetch_order(id, note, third_identity_id)
 
     result = client.fetch_orders(symbol, since, limit, note, third_identity_id)
 
@@ -25,17 +25,17 @@
 websocket_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
 
     api_key = ""
 
-    secret = ""
+    api_secret = ""
 
-    websocket_client = ZerocapWebsocketTest(apiKey, apiSecret)
+    websocket_client = ZerocapWebsocketTest(api_key, api_secret)
 
     market_connect = websocket_client.get_market()
 
     orders_connect = websocket_client.get_orders()
 
     while True:
```

### Comparing `zerocap_api_test-0.1.2/setup.py` & `zerocap_api_test-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 REQUIRED = [
     'requests',
     'websocket'
 ]
 
 setup(name='zerocap_api_test',  # 包名
-      version='0.1.2',  # 版本号
+      version='0.1.3',  # 版本号
       description='zerocap_api',
       long_description=long_description,
       author='jiayu.gao',
-      author_email='y18362683626@gmail.com',
+      author_email='jiayu.gao@eigen.capital',
       url='',
       install_requires=REQUIRED,
       license='BSD License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
           "Programming Language :: Python :: 3",
```

### Comparing `zerocap_api_test-0.1.2/zerocap_api_test.egg-info/PKG-INFO` & `zerocap_api_test-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
-Name: zerocap-api-test
-Version: 0.1.2
+Name: zerocap_api_test
+Version: 0.1.3
 Summary: zerocap_api
 Home-page: 
 Author: jiayu.gao
-Author-email: y18362683626@gmail.com
+Author-email: jiayu.gao@eigen.capital
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 License-File: LICENSE.txt
@@ -22,17 +22,17 @@
 rest_api_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
 
     api_key = ""
 
-    secret = ""
+    api_secret = ""
 
-    client = ZerocapRestClient(api_key, secret)
+    client = ZerocapRestClient(api_key, api_secret)
 
     result = client.create_order(symbol, side, type, amount, price, client_order_id, note, third_identity_id)
 
     result = client.fetch_order(id, note, third_identity_id)
 
     result = client.fetch_orders(symbol, since, limit, note, third_identity_id)
 
@@ -40,17 +40,17 @@
 websocket_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
 
     api_key = ""
 
-    secret = ""
+    api_secret = ""
 
-    websocket_client = ZerocapWebsocketTest(apiKey, apiSecret)
+    websocket_client = ZerocapWebsocketTest(api_key, api_secret)
 
     market_connect = websocket_client.get_market()
 
     orders_connect = websocket_client.get_orders()
 
     while True:
```

