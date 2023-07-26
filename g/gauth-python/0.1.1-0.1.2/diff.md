# Comparing `tmp/gauth_python-0.1.1.tar.gz` & `tmp/gauth_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth_python-0.1.1.tar", last modified: Wed Jul 26 08:47:02 2023, max compression
+gzip compressed data, was "gauth_python-0.1.2.tar", last modified: Wed Jul 26 10:04:29 2023, max compression
```

## Comparing `gauth_python-0.1.1.tar` & `gauth_python-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 08:47:02.259791 gauth_python-0.1.1/
--rw-r--r--   0 yohan      (501) staff       (20)     1061 2023-07-26 08:05:07.000000 gauth_python-0.1.1/LICENSE
--rw-r--r--   0 yohan      (501) staff       (20)      190 2023-07-26 08:47:02.259648 gauth_python-0.1.1/PKG-INFO
--rw-r--r--   0 yohan      (501) staff       (20)       23 2023-07-25 08:41:42.000000 gauth_python-0.1.1/README.md
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 08:47:02.258747 gauth_python-0.1.1/gauth_python.egg-info/
--rw-r--r--   0 yohan      (501) staff       (20)      190 2023-07-26 08:47:02.000000 gauth_python-0.1.1/gauth_python.egg-info/PKG-INFO
--rw-r--r--   0 yohan      (501) staff       (20)      240 2023-07-26 08:47:02.000000 gauth_python-0.1.1/gauth_python.egg-info/SOURCES.txt
--rw-r--r--   0 yohan      (501) staff       (20)        1 2023-07-26 08:47:02.000000 gauth_python-0.1.1/gauth_python.egg-info/dependency_links.txt
--rw-r--r--   0 yohan      (501) staff       (20)       21 2023-07-26 08:47:02.000000 gauth_python-0.1.1/gauth_python.egg-info/top_level.txt
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 08:47:02.259181 gauth_python-0.1.1/gauth_python_package/
--rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 10:32:26.000000 gauth_python-0.1.1/gauth_python_package/__init__.py
--rw-r--r--   0 yohan      (501) staff       (20)     1310 2023-07-26 08:30:17.000000 gauth_python-0.1.1/gauth_python_package/gauth_python.py
--rw-r--r--   0 yohan      (501) staff       (20)       38 2023-07-26 08:47:02.259833 gauth_python-0.1.1/setup.cfg
--rw-r--r--   0 yohan      (501) staff       (20)      372 2023-07-26 08:46:56.000000 gauth_python-0.1.1/setup.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:04:29.421705 gauth_python-0.1.2/
+-rw-r--r--   0 yohan      (501) staff       (20)     1061 2023-07-26 08:05:07.000000 gauth_python-0.1.2/LICENSE
+-rw-r--r--   0 yohan      (501) staff       (20)      487 2023-07-26 10:04:29.421560 gauth_python-0.1.2/PKG-INFO
+-rw-r--r--   0 yohan      (501) staff       (20)       23 2023-07-25 08:41:42.000000 gauth_python-0.1.2/README.md
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:04:29.420359 gauth_python-0.1.2/gauth_python.egg-info/
+-rw-r--r--   0 yohan      (501) staff       (20)      487 2023-07-26 10:04:29.000000 gauth_python-0.1.2/gauth_python.egg-info/PKG-INFO
+-rw-r--r--   0 yohan      (501) staff       (20)      285 2023-07-26 10:04:29.000000 gauth_python-0.1.2/gauth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 yohan      (501) staff       (20)        1 2023-07-26 10:04:29.000000 gauth_python-0.1.2/gauth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 yohan      (501) staff       (20)       27 2023-07-26 10:04:29.000000 gauth_python-0.1.2/gauth_python.egg-info/top_level.txt
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:04:29.420558 gauth_python-0.1.2/gauth_python_package/
+-rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 10:32:26.000000 gauth_python-0.1.2/gauth_python_package/__init__.py
+-rw-r--r--   0 yohan      (501) staff       (20)     1300 2023-07-26 08:58:09.000000 gauth_python-0.1.2/gauth_python_package/gauth_python.py
+-rw-r--r--   0 yohan      (501) staff       (20)       38 2023-07-26 10:04:29.421750 gauth_python-0.1.2/setup.cfg
+-rw-r--r--   0 yohan      (501) staff       (20)      805 2023-07-26 10:04:21.000000 gauth_python-0.1.2/setup.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:04:29.421192 gauth_python-0.1.2/tests/
+-rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 08:46:30.000000 gauth_python-0.1.2/tests/__init__.py
+-rw-r--r--   0 yohan      (501) staff       (20)      360 2023-07-26 08:52:41.000000 gauth_python-0.1.2/tests/test_gauth_python.py
```

### Comparing `gauth_python-0.1.1/LICENSE` & `gauth_python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gauth_python-0.1.1/gauth_python_package/gauth_python.py` & `gauth_python-0.1.2/gauth_python_package/gauth_python.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 class GAuthPython:
     global server_url
     global open_url
 
     server_url = "https://server.gauth.co.kr"
     open_url = "https://open.gauth.co.kr/user"
     
-    def code_issuance(email: str, password:str) -> str :
+    def ㅊ(email: str, password:str) -> str :
         URL = server_url + "/oauth/code"
         response = requests.post(URL, json={"email":email, "password" : password})
         return response.content
         
     def token_issuance(code : str, clientId: str, clientSecret: str, redirectUri: str) -> str :
         URL = "https://server.gauth.co.kr/oauth/token"
         response = requests.post(URL, json={"code" : code,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

