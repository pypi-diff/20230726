# Comparing `tmp/myds-0.1.4.tar.gz` & `tmp/myds-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myds-0.1.4.tar", last modified: Mon Jul 24 11:50:41 2023, max compression
+gzip compressed data, was "myds-0.1.5.tar", last modified: Wed Jul 26 13:51:34 2023, max compression
```

## Comparing `myds-0.1.4.tar` & `myds-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 11:50:41.526068 myds-0.1.4/
--rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 myds-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      278 2023-07-24 11:50:41.526068 myds-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-24 11:50:41.517090 myds-0.1.4/myds/
--rw-rw-rw-   0        0        0       52 2023-07-24 11:48:48.000000 myds-0.1.4/myds/__init__.py
--rw-rw-rw-   0        0        0     1625 2023-07-24 11:48:35.000000 myds-0.1.4/myds/database.py
--rw-rw-rw-   0        0        0      194 2023-07-24 11:49:48.000000 myds-0.1.4/myds/test.py
-drwxrwxrwx   0        0        0        0 2023-07-24 11:50:41.524073 myds-0.1.4/myds.egg-info/
--rw-rw-rw-   0        0        0      278 2023-07-24 11:50:41.000000 myds-0.1.4/myds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-07-24 11:50:41.000000 myds-0.1.4/myds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 11:50:41.000000 myds-0.1.4/myds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-24 11:50:41.000000 myds-0.1.4/myds.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-24 11:50:41.000000 myds-0.1.4/myds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 11:50:41.526068 myds-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      739 2023-07-24 11:50:09.000000 myds-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:51:34.174984 myds-0.1.5/
+-rw-rw-rw-   0        0        0     1082 2022-07-09 03:01:52.000000 myds-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      278 2023-07-26 13:51:34.174984 myds-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 13:51:34.164042 myds-0.1.5/myds/
+-rw-rw-rw-   0        0        0       59 2023-07-26 13:50:50.000000 myds-0.1.5/myds/__init__.py
+-rw-rw-rw-   0        0        0     1766 2023-07-26 13:50:50.000000 myds-0.1.5/myds/database.py
+-rw-rw-rw-   0        0        0      218 2023-07-26 13:50:29.000000 myds-0.1.5/myds/test.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:51:34.173029 myds-0.1.5/myds.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-07-26 13:51:34.000000 myds-0.1.5/myds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-07-26 13:51:34.000000 myds-0.1.5/myds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 13:51:34.000000 myds-0.1.5/myds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 13:51:34.000000 myds-0.1.5/myds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-26 13:51:34.000000 myds-0.1.5/myds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 13:51:34.174984 myds-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      739 2023-07-26 13:47:49.000000 myds-0.1.5/setup.py
```

### Comparing `myds-0.1.4/LICENSE` & `myds-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `myds-0.1.4/myds/database.py` & `myds-0.1.5/myds/database.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from requests.exceptions import (
     InvalidSchema,
 )
 import requests
 from urllib.parse import urlparse
 from urllib.parse import urlencode
 
+
 class HttpQuerier:
     def __init__(self, host="localhost", isSSL=False):
         self.host = host
         self.isSSL = isSSL
 
     def getQueryUrl(self, mydsUrl):
         parsed_url = urlparse(mydsUrl)
@@ -42,9 +43,16 @@
                 res = res[0:-1]
             while len(path) >= 3 and path[0:3] == "/..":
                 res = os.path.dirname(res)
                 path = path[3:]
             res += path
         return res
 
+
 def simpleQuery(dsName):
-    return HttpQuerier().query(f'myds://{dsName}')
+    return HttpQuerier().query(f'myds://{dsName}')
+
+
+def parse(pathName):
+    if pathName.startswith('myds://'):
+        return HttpQuerier().query(pathName);
+    return pathName;
```

### Comparing `myds-0.1.4/setup.py` & `myds-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name = "myds",
-    version = "0.1.4",
+    version = "0.1.5",
     keywords = ("database","localServer"),
     description = "A database name Getter",
     long_description = "A database name Getter",
     license = "MIT Licence",
     author = "Cai Jianping",
     author_email = "jpingcai@163.com",
```

