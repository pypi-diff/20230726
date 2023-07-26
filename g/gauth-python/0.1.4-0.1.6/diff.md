# Comparing `tmp/gauth_python-0.1.4.tar.gz` & `tmp/gauth_python-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth_python-0.1.4.tar", last modified: Wed Jul 26 10:29:45 2023, max compression
+gzip compressed data, was "gauth_python-0.1.6.tar", last modified: Wed Jul 26 11:10:03 2023, max compression
```

## Comparing `gauth_python-0.1.4.tar` & `gauth_python-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:29:45.854710 gauth_python-0.1.4/
--rw-r--r--   0 yohan      (501) staff       (20)     1061 2023-07-26 08:05:07.000000 gauth_python-0.1.4/LICENSE
--rw-r--r--   0 yohan      (501) staff       (20)      487 2023-07-26 10:29:45.854573 gauth_python-0.1.4/PKG-INFO
--rw-r--r--   0 yohan      (501) staff       (20)       23 2023-07-25 08:41:42.000000 gauth_python-0.1.4/README.md
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:29:45.853228 gauth_python-0.1.4/gauth_python/
--rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 10:32:26.000000 gauth_python-0.1.4/gauth_python/__init__.py
--rw-r--r--   0 yohan      (501) staff       (20)     1197 2023-07-26 10:28:50.000000 gauth_python-0.1.4/gauth_python/requests.py
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:29:45.854010 gauth_python-0.1.4/gauth_python.egg-info/
--rw-r--r--   0 yohan      (501) staff       (20)      487 2023-07-26 10:29:45.000000 gauth_python-0.1.4/gauth_python.egg-info/PKG-INFO
--rw-r--r--   0 yohan      (501) staff       (20)      300 2023-07-26 10:29:45.000000 gauth_python-0.1.4/gauth_python.egg-info/SOURCES.txt
--rw-r--r--   0 yohan      (501) staff       (20)        1 2023-07-26 10:29:45.000000 gauth_python-0.1.4/gauth_python.egg-info/dependency_links.txt
--rw-r--r--   0 yohan      (501) staff       (20)        9 2023-07-26 10:29:45.000000 gauth_python-0.1.4/gauth_python.egg-info/requires.txt
--rw-r--r--   0 yohan      (501) staff       (20)       19 2023-07-26 10:29:45.000000 gauth_python-0.1.4/gauth_python.egg-info/top_level.txt
--rw-r--r--   0 yohan      (501) staff       (20)       38 2023-07-26 10:29:45.854760 gauth_python-0.1.4/setup.cfg
--rw-r--r--   0 yohan      (501) staff       (20)      815 2023-07-26 10:29:34.000000 gauth_python-0.1.4/setup.py
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:29:45.854283 gauth_python-0.1.4/tests/
--rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 08:46:30.000000 gauth_python-0.1.4/tests/__init__.py
--rw-r--r--   0 yohan      (501) staff       (20)      316 2023-07-26 10:22:58.000000 gauth_python-0.1.4/tests/test_gauth_python.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:10:03.010054 gauth_python-0.1.6/
+-rw-r--r--   0 yohan      (501) staff       (20)     1061 2023-07-26 08:05:07.000000 gauth_python-0.1.6/LICENSE
+-rw-r--r--   0 yohan      (501) staff       (20)     2424 2023-07-26 11:10:03.009904 gauth_python-0.1.6/PKG-INFO
+-rw-r--r--   0 yohan      (501) staff       (20)     1960 2023-07-26 11:07:34.000000 gauth_python-0.1.6/README.md
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:10:03.008757 gauth_python-0.1.6/gauth_python/
+-rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 10:32:26.000000 gauth_python-0.1.6/gauth_python/__init__.py
+-rw-r--r--   0 yohan      (501) staff       (20)     1342 2023-07-26 11:04:45.000000 gauth_python-0.1.6/gauth_python/requests.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:10:03.009364 gauth_python-0.1.6/gauth_python.egg-info/
+-rw-r--r--   0 yohan      (501) staff       (20)     2424 2023-07-26 11:10:02.000000 gauth_python-0.1.6/gauth_python.egg-info/PKG-INFO
+-rw-r--r--   0 yohan      (501) staff       (20)      300 2023-07-26 11:10:02.000000 gauth_python-0.1.6/gauth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 yohan      (501) staff       (20)        1 2023-07-26 11:10:02.000000 gauth_python-0.1.6/gauth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 yohan      (501) staff       (20)        9 2023-07-26 11:10:02.000000 gauth_python-0.1.6/gauth_python.egg-info/requires.txt
+-rw-r--r--   0 yohan      (501) staff       (20)       19 2023-07-26 11:10:02.000000 gauth_python-0.1.6/gauth_python.egg-info/top_level.txt
+-rw-r--r--   0 yohan      (501) staff       (20)       38 2023-07-26 11:10:03.010099 gauth_python-0.1.6/setup.cfg
+-rw-r--r--   0 yohan      (501) staff       (20)      815 2023-07-26 11:05:01.000000 gauth_python-0.1.6/setup.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 11:10:03.009580 gauth_python-0.1.6/tests/
+-rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 08:46:30.000000 gauth_python-0.1.6/tests/__init__.py
+-rw-r--r--   0 yohan      (501) staff       (20)      296 2023-07-26 10:49:49.000000 gauth_python-0.1.6/tests/test_gauth_python.py
```

### Comparing `gauth_python-0.1.4/LICENSE` & `gauth_python-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gauth_python-0.1.4/gauth_python/requests.py` & `gauth_python-0.1.6/gauth_python/requests.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 
 server_url = "https://server.gauth.co.kr"
 open_url = "https://open.gauth.co.kr/user"
     
 def code_issuance(email: str, password:str) -> str :
     URL = server_url + "/oauth/code"
     response = requests.post(URL, json={"email":email, "password" : password})
-    print("성공적으로 코드를 보냈습니다.")
-    return response.content
+    response_json = response.content.decode("utf-8")
+    return response_json
 
 def token_issuance(code : str, clientId: str, clientSecret: str, redirectUri: str) -> str :
     URL = server_url + "/oauth/token"
     response = requests.post(URL, json={"code" : code,
-                                    "clientId": clientId,
+                                        "clientId": clientId,
                                         "clientSecret": clientSecret,
                                         "redirectUri" : redirectUri})
-    return response.content
+    response_json = response.content.decode("utf-8")
+    return response_json
 
 def token_reissuance(refreshToken : str) -> str:
     URL = server_url + "/oauth/token"
     response = requests.patch(URL, headers={"refreshToken" : "Bearer " + refreshToken})
-    return response.content
+    response_json = response.content.decode("utf-8")
+    return response_json
 
-def user_info(refreshToken : str) -> str:
+def user_info(accessToken : str) -> str:
     URL = open_url + "/user"
-    response = requests.get(URL, headers={"Authorization": "Bearer " + refreshToken})
-
-    return response.content
+    response = requests.get(URL, headers={"Authorization": "Bearer " + accessToken})
+    response_json = response.content.decode("utf-8")
+    return response_json
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gauth_python-0.1.4/setup.py` & `gauth_python-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='gauth_python',
-    version='0.1.4',
+    version='0.1.6',
     description='Python sdk from Gauth.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = "https://github.com/GSM-MSG/GAuth-SDK-Python",
     packages=setuptools.find_packages(),
     classifiers = [        
         "Programming Language :: Python :: 3",
```

