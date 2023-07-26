# Comparing `tmp/zerocap_api_test-0.1.1.tar.gz` & `tmp/zerocap_api_test-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zerocap_api_test-0.1.1.tar", last modified: Wed Jul 26 05:50:53 2023, max compression
+gzip compressed data, was "dist/zerocap_api_test-0.1.2.tar", last modified: Wed Jul 26 06:05:03 2023, max compression
```

## Comparing `zerocap_api_test-0.1.1.tar` & `zerocap_api_test-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 05:50:53.000000 zerocap_api_test-0.1.1/
--rw-r--r--   0 mac        (501) staff       (20)    11323 2023-07-24 01:35:05.000000 zerocap_api_test-0.1.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     1404 2023-07-26 05:50:53.000000 zerocap_api_test-0.1.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1025 2023-07-26 05:48:22.000000 zerocap_api_test-0.1.1/README.rst
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-26 05:50:53.000000 zerocap_api_test-0.1.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      791 2023-07-26 05:44:22.000000 zerocap_api_test-0.1.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 05:50:53.000000 zerocap_api_test-0.1.1/zerocap_api_test/
--rw-r--r--   0 mac        (501) staff       (20)      121 2023-07-26 05:40:03.000000 zerocap_api_test-0.1.1/zerocap_api_test/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     7275 2023-07-26 05:44:10.000000 zerocap_api_test-0.1.1/zerocap_api_test/main.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 05:50:53.000000 zerocap_api_test-0.1.1/zerocap_api_test.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1404 2023-07-26 05:50:53.000000 zerocap_api_test-0.1.1/zerocap_api_test.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      284 2023-07-26 05:50:53.000000 zerocap_api_test-0.1.1/zerocap_api_test.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-26 05:50:53.000000 zerocap_api_test-0.1.1/zerocap_api_test.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-26 05:50:53.000000 zerocap_api_test-0.1.1/zerocap_api_test.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       17 2023-07-26 05:50:53.000000 zerocap_api_test-0.1.1/zerocap_api_test.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/
+-rw-r--r--   0 mac        (501) staff       (20)    11323 2023-07-24 01:35:05.000000 zerocap_api_test-0.1.2/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1404 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1025 2023-07-26 05:48:22.000000 zerocap_api_test-0.1.2/README.rst
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      791 2023-07-26 06:04:52.000000 zerocap_api_test-0.1.2/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test/
+-rw-r--r--   0 mac        (501) staff       (20)      121 2023-07-26 05:40:03.000000 zerocap_api_test-0.1.2/zerocap_api_test/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     7270 2023-07-26 06:04:05.000000 zerocap_api_test-0.1.2/zerocap_api_test/main.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1404 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      284 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       19 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       17 2023-07-26 06:05:03.000000 zerocap_api_test-0.1.2/zerocap_api_test.egg-info/top_level.txt
```

### Comparing `zerocap_api_test-0.1.1/LICENSE.txt` & `zerocap_api_test-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerocap_api_test-0.1.1/PKG-INFO` & `zerocap_api_test-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap_api_test
-Version: 0.1.1
+Version: 0.1.2
 Summary: zerocap_api
 Home-page: 
 Author: jiayu.gao
 Author-email: y18362683626@gmail.com
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zerocap_api_test-0.1.1/README.rst` & `zerocap_api_test-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `zerocap_api_test-0.1.1/setup.py` & `zerocap_api_test-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 REQUIRED = [
     'requests',
     'websocket'
 ]
 
 setup(name='zerocap_api_test',  # 包名
-      version='0.1.1',  # 版本号
+      version='0.1.2',  # 版本号
       description='zerocap_api',
       long_description=long_description,
       author='jiayu.gao',
       author_email='y18362683626@gmail.com',
       url='',
       install_requires=REQUIRED,
       license='BSD License',
```

### Comparing `zerocap_api_test-0.1.1/zerocap_api_test/main.py` & `zerocap_api_test-0.1.2/zerocap_api_test/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         
     def hashing(self):
         return  hmac.new(
 			self.apiSecret.encode("utf-8"), self.apiKey.encode("utf-8"), hashlib.sha256
 		).hexdigest()
 
     def encryption_api_key(self):
-        signature = self.hashing(self.secret, self.api_key)
+        signature = self.hashing()
         return signature
 
     def create_order(self, symbol, side, type, amount, price, client_order_id, note, third_identity_id):
         signature = self.encryption_api_key()
         if signature == "fail":
             return "Create Order Api Key error"
 
@@ -167,15 +167,15 @@
             response = requests.post(url, data=json.dumps(data), headers=headers)
             if response.status_code == 200:
                 res = response.json()
                 return res["data"]
         except Exception as e:
             return "Dma Server error, create order fail"
 
-    def fetch_order(self, id, note, third_identity_id):
+    def fetch_order(self, id, note='', third_identity_id=''):
         signature = self.encryption_api_key()
         if signature == "fail":
             return "Fetch Order Api Key error"
 
         url = f"{self.base_url}/fetch_order"
         headers = {
             'Content-Type': 'application/json',
@@ -193,15 +193,15 @@
             response = requests.post(url, data=json.dumps(data), headers=headers)
             if response.status_code == 200:
                 res = response.json()
                 return res["data"]
         except Exception as e:
             return "Dma Server error, fetch order fail"
 
-    def fetch_orders(self, symbol: str, since: int, limit: int, note: str, third_identity_id:str):
+    def fetch_orders(self, symbol: str='', since: int='', limit: int=0, note: str='', third_identity_id:str=''):
         signature = self.encryption_api_key()
         if signature == "fail":
             return "Fetch Orders Api Key error"
 
         url = f"{self.base_url}/fetch_orders"
         headers = {
             'Content-Type': 'application/json',
```

### Comparing `zerocap_api_test-0.1.1/zerocap_api_test.egg-info/PKG-INFO` & `zerocap_api_test-0.1.2/zerocap_api_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerocap-api-test
-Version: 0.1.1
+Version: 0.1.2
 Summary: zerocap_api
 Home-page: 
 Author: jiayu.gao
 Author-email: y18362683626@gmail.com
 License: BSD License
 Platform: all
 Classifier: Programming Language :: Python :: 3
```

