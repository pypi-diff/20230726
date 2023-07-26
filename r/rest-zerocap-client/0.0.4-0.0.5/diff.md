# Comparing `tmp/rest_zerocap_client-0.0.4.tar.gz` & `tmp/rest_zerocap_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rest_zerocap_client-0.0.4.tar", last modified: Wed Jul 26 05:13:15 2023, max compression
+gzip compressed data, was "dist\rest_zerocap_client-0.0.5.tar", last modified: Wed Jul 26 05:42:31 2023, max compression
```

## Comparing `rest_zerocap_client-0.0.4.tar` & `rest_zerocap_client-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 05:13:15.000000 rest_zerocap_client-0.0.4/
--rw-rw-rw-   0        0        0      870 2023-07-26 05:13:15.000000 rest_zerocap_client-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-07-26 05:12:51.000000 rest_zerocap_client-0.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 05:13:15.000000 rest_zerocap_client-0.0.4/rest_client/
--rw-rw-rw-   0        0        0       91 2023-07-21 09:36:05.000000 rest_zerocap_client-0.0.4/rest_client/__init__.py
--rw-rw-rw-   0        0        0     4342 2023-07-25 01:25:52.000000 rest_zerocap_client-0.0.4/rest_client/zerpcap_rest_client.py
-drwxrwxrwx   0        0        0        0 2023-07-26 05:13:15.000000 rest_zerocap_client-0.0.4/rest_zerocap_client.egg-info/
--rw-rw-rw-   0        0        0      870 2023-07-26 05:13:15.000000 rest_zerocap_client-0.0.4/rest_zerocap_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-07-26 05:13:15.000000 rest_zerocap_client-0.0.4/rest_zerocap_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 05:13:15.000000 rest_zerocap_client-0.0.4/rest_zerocap_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-26 05:13:15.000000 rest_zerocap_client-0.0.4/rest_zerocap_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-26 05:13:15.000000 rest_zerocap_client-0.0.4/rest_zerocap_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 05:13:15.000000 rest_zerocap_client-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1270 2023-07-26 04:58:32.000000 rest_zerocap_client-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 05:42:31.000000 rest_zerocap_client-0.0.5/
+-rw-rw-rw-   0        0        0      870 2023-07-26 05:42:31.000000 rest_zerocap_client-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-07-26 05:12:51.000000 rest_zerocap_client-0.0.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 05:42:31.000000 rest_zerocap_client-0.0.5/rest_client/
+-rw-rw-rw-   0        0        0       91 2023-07-26 05:42:23.000000 rest_zerocap_client-0.0.5/rest_client/__init__.py
+-rw-rw-rw-   0        0        0     4342 2023-07-26 05:42:25.000000 rest_zerocap_client-0.0.5/rest_client/zerpcap_rest_client.py
+drwxrwxrwx   0        0        0        0 2023-07-26 05:42:31.000000 rest_zerocap_client-0.0.5/rest_zerocap_client.egg-info/
+-rw-rw-rw-   0        0        0      870 2023-07-26 05:42:31.000000 rest_zerocap_client-0.0.5/rest_zerocap_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-26 05:42:31.000000 rest_zerocap_client-0.0.5/rest_zerocap_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 05:42:31.000000 rest_zerocap_client-0.0.5/rest_zerocap_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 05:42:31.000000 rest_zerocap_client-0.0.5/rest_zerocap_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-26 05:42:31.000000 rest_zerocap_client-0.0.5/rest_zerocap_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 05:42:31.000000 rest_zerocap_client-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1276 2023-07-26 05:40:02.000000 rest_zerocap_client-0.0.5/setup.py
```

### Comparing `rest_zerocap_client-0.0.4/PKG-INFO` & `rest_zerocap_client-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest_zerocap_client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Order Operation
 Home-page: 
 Author: Tkon
 Author-email: 1741226849@qq.com
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rest_zerocap_client-0.0.4/README.rst` & `rest_zerocap_client-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `rest_zerocap_client-0.0.4/rest_client/zerpcap_rest_client.py` & `rest_zerocap_client-0.0.5/rest_client/zerpcap_rest_client.py`

 * *Files identical despite different names*

### Comparing `rest_zerocap_client-0.0.4/rest_zerocap_client.egg-info/PKG-INFO` & `rest_zerocap_client-0.0.5/rest_zerocap_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-zerocap-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Order Operation
 Home-page: 
 Author: Tkon
 Author-email: 1741226849@qq.com
 Platform: all
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `rest_zerocap_client-0.0.4/setup.py` & `rest_zerocap_client-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 #     version='0.1',
 #     # packages = find_packages(),
 #     py_modules=['zerocap_rest_client']      # py 文件
 # )
 
 REQUIRED = [
     'requests',
-    'json',
-    'hmac',
-    'hashlib'
+    # 'json',
+    # 'hmac',
+    # 'hashlib'
 ]
 
 with open("README.rst", "r", encoding="utf-8") as f:
   long_description = f.read()
 
 setup(
     name="rest_zerocap_client", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.4",    #包版本号，便于维护版本
+    version="0.0.5",    #包版本号，便于维护版本
     author="Tkon",    #作者，可以写自己的姓名
     author_email="1741226849@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="Order Operation",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     url="",    #自己项目地址，比如github的项目地址
     install_requires=REQUIRED,
     packages=find_packages(),
```

