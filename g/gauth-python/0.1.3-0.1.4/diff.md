# Comparing `tmp/gauth_python-0.1.3.tar.gz` & `tmp/gauth_python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth_python-0.1.3.tar", last modified: Wed Jul 26 10:24:14 2023, max compression
+gzip compressed data, was "gauth_python-0.1.4.tar", last modified: Wed Jul 26 10:29:45 2023, max compression
```

## Comparing `gauth_python-0.1.3.tar` & `gauth_python-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:24:14.446213 gauth_python-0.1.3/
--rw-r--r--   0 yohan      (501) staff       (20)     1061 2023-07-26 08:05:07.000000 gauth_python-0.1.3/LICENSE
--rw-r--r--   0 yohan      (501) staff       (20)      487 2023-07-26 10:24:14.446031 gauth_python-0.1.3/PKG-INFO
--rw-r--r--   0 yohan      (501) staff       (20)       23 2023-07-25 08:41:42.000000 gauth_python-0.1.3/README.md
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:24:14.444377 gauth_python-0.1.3/gauth_python/
--rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 10:32:26.000000 gauth_python-0.1.3/gauth_python/__init__.py
--rw-r--r--   0 yohan      (501) staff       (20)     1141 2023-07-26 10:22:12.000000 gauth_python-0.1.3/gauth_python/requests.py
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:24:14.445259 gauth_python-0.1.3/gauth_python.egg-info/
--rw-r--r--   0 yohan      (501) staff       (20)      487 2023-07-26 10:24:14.000000 gauth_python-0.1.3/gauth_python.egg-info/PKG-INFO
--rw-r--r--   0 yohan      (501) staff       (20)      265 2023-07-26 10:24:14.000000 gauth_python-0.1.3/gauth_python.egg-info/SOURCES.txt
--rw-r--r--   0 yohan      (501) staff       (20)        1 2023-07-26 10:24:14.000000 gauth_python-0.1.3/gauth_python.egg-info/dependency_links.txt
--rw-r--r--   0 yohan      (501) staff       (20)       19 2023-07-26 10:24:14.000000 gauth_python-0.1.3/gauth_python.egg-info/top_level.txt
--rw-r--r--   0 yohan      (501) staff       (20)       38 2023-07-26 10:24:14.446322 gauth_python-0.1.3/setup.cfg
--rw-r--r--   0 yohan      (501) staff       (20)      816 2023-07-26 10:24:09.000000 gauth_python-0.1.3/setup.py
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:24:14.445494 gauth_python-0.1.3/tests/
--rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 08:46:30.000000 gauth_python-0.1.3/tests/__init__.py
--rw-r--r--   0 yohan      (501) staff       (20)      316 2023-07-26 10:22:58.000000 gauth_python-0.1.3/tests/test_gauth_python.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:29:45.854710 gauth_python-0.1.4/
+-rw-r--r--   0 yohan      (501) staff       (20)     1061 2023-07-26 08:05:07.000000 gauth_python-0.1.4/LICENSE
+-rw-r--r--   0 yohan      (501) staff       (20)      487 2023-07-26 10:29:45.854573 gauth_python-0.1.4/PKG-INFO
+-rw-r--r--   0 yohan      (501) staff       (20)       23 2023-07-25 08:41:42.000000 gauth_python-0.1.4/README.md
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:29:45.853228 gauth_python-0.1.4/gauth_python/
+-rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 10:32:26.000000 gauth_python-0.1.4/gauth_python/__init__.py
+-rw-r--r--   0 yohan      (501) staff       (20)     1197 2023-07-26 10:28:50.000000 gauth_python-0.1.4/gauth_python/requests.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:29:45.854010 gauth_python-0.1.4/gauth_python.egg-info/
+-rw-r--r--   0 yohan      (501) staff       (20)      487 2023-07-26 10:29:45.000000 gauth_python-0.1.4/gauth_python.egg-info/PKG-INFO
+-rw-r--r--   0 yohan      (501) staff       (20)      300 2023-07-26 10:29:45.000000 gauth_python-0.1.4/gauth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 yohan      (501) staff       (20)        1 2023-07-26 10:29:45.000000 gauth_python-0.1.4/gauth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 yohan      (501) staff       (20)        9 2023-07-26 10:29:45.000000 gauth_python-0.1.4/gauth_python.egg-info/requires.txt
+-rw-r--r--   0 yohan      (501) staff       (20)       19 2023-07-26 10:29:45.000000 gauth_python-0.1.4/gauth_python.egg-info/top_level.txt
+-rw-r--r--   0 yohan      (501) staff       (20)       38 2023-07-26 10:29:45.854760 gauth_python-0.1.4/setup.cfg
+-rw-r--r--   0 yohan      (501) staff       (20)      815 2023-07-26 10:29:34.000000 gauth_python-0.1.4/setup.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 10:29:45.854283 gauth_python-0.1.4/tests/
+-rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 08:46:30.000000 gauth_python-0.1.4/tests/__init__.py
+-rw-r--r--   0 yohan      (501) staff       (20)      316 2023-07-26 10:22:58.000000 gauth_python-0.1.4/tests/test_gauth_python.py
```

### Comparing `gauth_python-0.1.3/LICENSE` & `gauth_python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gauth_python-0.1.3/gauth_python/requests.py` & `gauth_python-0.1.4/gauth_python/requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 server_url = "https://server.gauth.co.kr"
 open_url = "https://open.gauth.co.kr/user"
     
 def code_issuance(email: str, password:str) -> str :
     URL = server_url + "/oauth/code"
     response = requests.post(URL, json={"email":email, "password" : password})
+    print("성공적으로 코드를 보냈습니다.")
     return response.content
 
 def token_issuance(code : str, clientId: str, clientSecret: str, redirectUri: str) -> str :
     URL = server_url + "/oauth/token"
     response = requests.post(URL, json={"code" : code,
                                     "clientId": clientId,
                                         "clientSecret": clientSecret,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gauth_python-0.1.3/setup.py` & `gauth_python-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='gauth_python',
-    version='0.1.3',
+    version='0.1.4',
     description='Python sdk from Gauth.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url = "https://github.com/GSM-MSG/GAuth-SDK-Python",
     packages=setuptools.find_packages(),
     classifiers = [        
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires = '>=3.7',
     author_email="dev.yohan05@gmail.com",
     author='Noh Gaseong',
     license='MIT',
-    install_requires=[],
-    setup_requires=['pytest-runner','requests'],
+    install_requires=['requests'],
+    setup_requires=['pytest-runner'],
     tests_require=['pytest==7.4.0'],
     test_suite='tests',
 )
```

