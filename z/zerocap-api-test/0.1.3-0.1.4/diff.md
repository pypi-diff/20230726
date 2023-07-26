# Comparing `tmp/zerocap_api_test-0.1.3.tar.gz` & `tmp/zerocap_api_test-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerocap_api_test-0.1.3.tar", last modified: Wed Jul 26 07:08:23 2023, max compression
+gzip compressed data, was "dist/zerocap_api_test-0.1.4.tar", last modified: Wed Jul 26 08:02:23 2023, max compression
```

## Comparing `zerocap_api_test-0.1.3.tar` & `zerocap_api_test-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-26 07:08:23.514909 zerocap_api_test-0.1.3/
--rw-r--r--   0 gao        (501) staff       (20)    11323 2023-07-26 06:32:00.000000 zerocap_api_test-0.1.3/LICENSE.txt
--rw-r--r--   0 gao        (501) staff       (20)     1419 2023-07-26 07:08:23.514564 zerocap_api_test-0.1.3/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)     1039 2023-07-26 06:42:12.000000 zerocap_api_test-0.1.3/README.rst
--rw-r--r--   0 gao        (501) staff       (20)       38 2023-07-26 07:08:23.515025 zerocap_api_test-0.1.3/setup.cfg
--rw-r--r--   0 gao        (501) staff       (20)      792 2023-07-26 07:08:15.000000 zerocap_api_test-0.1.3/setup.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-26 07:08:23.511094 zerocap_api_test-0.1.3/zerocap_api_test/
--rw-r--r--   0 gao        (501) staff       (20)      121 2023-07-26 06:32:00.000000 zerocap_api_test-0.1.3/zerocap_api_test/__init__.py
--rw-r--r--   0 gao        (501) staff       (20)     6674 2023-07-26 06:57:14.000000 zerocap_api_test-0.1.3/zerocap_api_test/main.py
-drwxr-xr-x   0 gao        (501) staff       (20)        0 2023-07-26 07:08:23.514102 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/
--rw-r--r--   0 gao        (501) staff       (20)     1419 2023-07-26 07:08:23.000000 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/PKG-INFO
--rw-r--r--   0 gao        (501) staff       (20)      284 2023-07-26 07:08:23.000000 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/SOURCES.txt
--rw-r--r--   0 gao        (501) staff       (20)        1 2023-07-26 07:08:23.000000 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/dependency_links.txt
--rw-r--r--   0 gao        (501) staff       (20)       19 2023-07-26 07:08:23.000000 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/requires.txt
--rw-r--r--   0 gao        (501) staff       (20)       17 2023-07-26 07:08:23.000000 zerocap_api_test-0.1.3/zerocap_api_test.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/
+-rw-r--r--   0 mac        (501) staff       (20)    11323 2023-07-24 01:35:05.000000 zerocap_api_test-0.1.4/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1454 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1074 2023-07-26 07:10:20.000000 zerocap_api_test-0.1.4/README.rst
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      792 2023-07-26 08:02:15.000000 zerocap_api_test-0.1.4/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test/
+-rw-r--r--   0 mac        (501) staff       (20)      121 2023-07-26 05:40:03.000000 zerocap_api_test-0.1.4/zerocap_api_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     6928 2023-07-26 07:42:11.000000 zerocap_api_test-0.1.4/zerocap_api_test/main.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1454 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      284 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       17 2023-07-26 08:02:23.000000 zerocap_api_test-0.1.4/zerocap_api_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_test-0.1.3/LICENSE.txt` & `zerocap_api_test-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_api_test-0.1.3/PKG-INFO` & `zerocap_api_test-0.1.4/zerocap_api_test.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zerocap_api_test
-Version: 0.1.3
+Name: zerocap-api-test
+Version: 0.1.4
 Summary: zerocap_api
 Home-page: 
 Author: jiayu.gao
 Author-email: jiayu.gao@eigen.capital
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -28,17 +28,17 @@
 
     api_secret = ""
 
     client = ZerocapRestClient(api_key, api_secret)
 
     result = client.create_order(symbol, side, type, amount, price, client_order_id, note, third_identity_id)
 
-    result = client.fetch_order(id, note, third_identity_id)
+    result = client.fetch_order(id, note=None, third_identity_id=None)
 
-    result = client.fetch_orders(symbol, since, limit, note, third_identity_id)
+    result = client.fetch_orders(symbol=None, since=None, limit=None, note=None, third_identity_id=None)
 
 
 websocket_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
```

### Comparing `zerocap_api_test-0.1.3/README.rst` & `zerocap_api_test-0.1.4/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
     api_secret = ""
 
     client = ZerocapRestClient(api_key, api_secret)
 
     result = client.create_order(symbol, side, type, amount, price, client_order_id, note, third_identity_id)
 
-    result = client.fetch_order(id, note, third_identity_id)
+    result = client.fetch_order(id, note=None, third_identity_id=None)
 
-    result = client.fetch_orders(symbol, since, limit, note, third_identity_id)
+    result = client.fetch_orders(symbol=None, since=None, limit=None, note=None, third_identity_id=None)
 
 
 websocket_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
```

### Comparing `zerocap_api_test-0.1.3/setup.py` & `zerocap_api_test-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 REQUIRED = [
     'requests',
     'websocket'
 ]
 
 setup(name='zerocap_api_test',  # 包名
-      version='0.1.3',  # 版本号
+      version='0.1.4',  # 版本号
       description='zerocap_api',
       long_description=long_description,
       author='jiayu.gao',
       author_email='jiayu.gao@eigen.capital',
       url='',
       install_requires=REQUIRED,
       license='BSD License',
```

### Comparing `zerocap_api_test-0.1.3/zerocap_api_test/main.py` & `zerocap_api_test-0.1.4/zerocap_api_test/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,23 +39,26 @@
         return {
             "api_key": self.api_key,
             "signature": self.signature,
             "data_type": data_type,
         }
 
     def close(self, channel=None):
-        if channel == "orders" and self.order_websocket:
-            self.order_websocket.close()
-        elif channel == "market" and self.market_websocket:
-            self.market_websocket.close()
-        else:
-            if self.order_websocket:
+        try:
+            if channel == "orders" and self.order_websocket:
                 self.order_websocket.close()
-            if self.market_websocket:
+            elif channel == "market" and self.market_websocket:
                 self.market_websocket.close()
+            else:
+                if self.order_websocket:
+                    self.order_websocket.close()
+                if self.market_websocket:
+                    self.market_websocket.close()
+        except:
+            pass
         return
 
     def get_message(self, ws_recv):
         return ws_recv.__next__()
     
     def get_orders(self):
         try:
@@ -139,14 +142,16 @@
                 "note": note,
             }
         }
         response = requests.post(url, data=json.dumps(data), headers=headers)
         if response.status_code == 200:
             res = response.json()
             return res["data"]
+        else:
+            raise Exception(response.text)
 
     def fetch_order(self, id, note='', third_identity_id=''):
         signature = self.encryption_api_key()
         if signature == "fail":
             return "Fetch Order Api Key error"
 
         url = f"{self.base_url}/fetch_order"
@@ -162,14 +167,16 @@
                 "note": note,
             }
         }
         response = requests.post(url, data=json.dumps(data), headers=headers)
         if response.status_code == 200:
             res = response.json()
             return res["data"]
+        else:
+            raise Exception(response.text)
 
     def fetch_orders(self, symbol: str='', since: int='', limit: int=0, note: str='', third_identity_id:str=''):
         signature = self.encryption_api_key()
         if signature == "fail":
             return "Fetch Orders Api Key error"
 
         url = f"{self.base_url}/fetch_orders"
@@ -186,8 +193,10 @@
                 "signature": signature,
                 "note": note,
             }
         }
         response = requests.post(url, data=json.dumps(data), headers=headers)
         if response.status_code == 200:
             res = response.json()
-            return res["data"]
+            return res["data"]
+        else:
+            raise Exception(response.text)
```

### Comparing `zerocap_api_test-0.1.3/zerocap_api_test.egg-info/PKG-INFO` & `zerocap_api_test-0.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: zerocap-api-test
-Version: 0.1.3
+Name: zerocap_api_test
+Version: 0.1.4
 Summary: zerocap_api
 Home-page: 
 Author: jiayu.gao
 Author-email: jiayu.gao@eigen.capital
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
@@ -28,17 +28,17 @@
 
     api_secret = ""
 
     client = ZerocapRestClient(api_key, api_secret)
 
     result = client.create_order(symbol, side, type, amount, price, client_order_id, note, third_identity_id)
 
-    result = client.fetch_order(id, note, third_identity_id)
+    result = client.fetch_order(id, note=None, third_identity_id=None)
 
-    result = client.fetch_orders(symbol, since, limit, note, third_identity_id)
+    result = client.fetch_orders(symbol=None, since=None, limit=None, note=None, third_identity_id=None)
 
 
 websocket_demo
 ::
 
     from zerocap_api_test import ZerocapRestClient
```

