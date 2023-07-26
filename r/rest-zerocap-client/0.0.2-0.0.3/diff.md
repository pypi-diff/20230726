# Comparing `tmp/rest_zerocap_client-0.0.2.tar.gz` & `tmp/rest_zerocap_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rest_zerocap_client-0.0.2.tar", last modified: Tue Jul 25 02:24:57 2023, max compression
+gzip compressed data, was "dist\rest_zerocap_client-0.0.3.tar", last modified: Wed Jul 26 04:34:21 2023, max compression
```

## Comparing `rest_zerocap_client-0.0.2.tar` & `rest_zerocap_client-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 02:24:57.000000 rest_zerocap_client-0.0.2/
--rw-rw-rw-   0        0        0     1453 2023-07-25 02:24:57.000000 rest_zerocap_client-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1107 2023-07-25 02:24:36.000000 rest_zerocap_client-0.0.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-25 02:24:57.000000 rest_zerocap_client-0.0.2/rest_client/
--rw-rw-rw-   0        0        0       91 2023-07-21 09:36:05.000000 rest_zerocap_client-0.0.2/rest_client/__init__.py
--rw-rw-rw-   0        0        0     4342 2023-07-25 01:25:52.000000 rest_zerocap_client-0.0.2/rest_client/zerpcap_rest_client.py
-drwxrwxrwx   0        0        0        0 2023-07-25 02:24:57.000000 rest_zerocap_client-0.0.2/rest_zerocap_client.egg-info/
--rw-rw-rw-   0        0        0     1453 2023-07-25 02:24:57.000000 rest_zerocap_client-0.0.2/rest_zerocap_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-07-25 02:24:57.000000 rest_zerocap_client-0.0.2/rest_zerocap_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 02:24:57.000000 rest_zerocap_client-0.0.2/rest_zerocap_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-07-25 02:24:57.000000 rest_zerocap_client-0.0.2/rest_zerocap_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-25 02:24:57.000000 rest_zerocap_client-0.0.2/rest_zerocap_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 02:24:57.000000 rest_zerocap_client-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-07-25 02:24:56.000000 rest_zerocap_client-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:34:21.000000 rest_zerocap_client-0.0.3/
+-rw-rw-rw-   0        0        0      348 2023-07-26 04:34:21.000000 rest_zerocap_client-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2023-07-26 04:32:40.000000 rest_zerocap_client-0.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-26 04:34:20.000000 rest_zerocap_client-0.0.3/rest_client/
+-rw-rw-rw-   0        0        0       91 2023-07-21 09:36:05.000000 rest_zerocap_client-0.0.3/rest_client/__init__.py
+-rw-rw-rw-   0        0        0     4342 2023-07-25 01:25:52.000000 rest_zerocap_client-0.0.3/rest_client/zerpcap_rest_client.py
+drwxrwxrwx   0        0        0        0 2023-07-26 04:34:20.000000 rest_zerocap_client-0.0.3/rest_zerocap_client.egg-info/
+-rw-rw-rw-   0        0        0      348 2023-07-26 04:34:20.000000 rest_zerocap_client-0.0.3/rest_zerocap_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-26 04:34:20.000000 rest_zerocap_client-0.0.3/rest_zerocap_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 04:34:20.000000 rest_zerocap_client-0.0.3/rest_zerocap_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-07-26 04:34:20.000000 rest_zerocap_client-0.0.3/rest_zerocap_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-26 04:34:20.000000 rest_zerocap_client-0.0.3/rest_zerocap_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 04:34:21.000000 rest_zerocap_client-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-07-26 04:34:09.000000 rest_zerocap_client-0.0.3/setup.py
```

### Comparing `rest_zerocap_client-0.0.2/rest_client/zerpcap_rest_client.py` & `rest_zerocap_client-0.0.3/rest_client/zerpcap_rest_client.py`

 * *Files identical despite different names*

### Comparing `rest_zerocap_client-0.0.2/setup.py` & `rest_zerocap_client-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     with io.open('README.MD', encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = "test"
 
 setup(
     name="rest_zerocap_client", # 用自己的名替换其中的YOUR_USERNAME_
-    version="0.0.2",    #包版本号，便于维护版本
+    version="0.0.3",    #包版本号，便于维护版本
     author="Tkon",    #作者，可以写自己的姓名
     author_email="1741226849@qq.com",    #作者联系方式，可写自己的邮箱地址
     description="Order Operation",#包的简述
     long_description=long_description,    #包的详细介绍，一般在README.md文件内
     url="",    #自己项目地址，比如github的项目地址
     install_requires=REQUIRED,
     packages=find_packages(),
```

