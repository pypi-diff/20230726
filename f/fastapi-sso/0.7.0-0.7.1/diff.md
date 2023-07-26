# Comparing `tmp/fastapi_sso-0.7.0.tar.gz` & `tmp/fastapi_sso-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_sso-0.7.0.tar", max compression
+gzip compressed data, was "fastapi_sso-0.7.1.tar", max compression
```

## Comparing `fastapi_sso-0.7.0.tar` & `fastapi_sso-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1093 2023-02-07 15:13:40.445140 fastapi_sso-0.7.0/LICENSE.md
--rw-r--r--   0        0        0     6118 2023-07-25 18:36:55.037625 fastapi_sso-0.7.0/README.md
--rw-r--r--   0        0        0     1110 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/__init__.py
--rw-r--r--   0        0        0        0 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/__init__.py
--rw-r--r--   0        0        0    11117 2023-07-25 18:00:47.042827 fastapi_sso-0.7.0/fastapi_sso/sso/base.py
--rw-r--r--   0        0        0     1215 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/facebook.py
--rw-r--r--   0        0        0     1146 2023-03-25 12:01:05.759478 fastapi_sso-0.7.0/fastapi_sso/sso/fitbit.py
--rw-r--r--   0        0        0     2506 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/generic.py
--rw-r--r--   0        0        0      913 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/github.py
--rw-r--r--   0        0        0      920 2023-07-25 18:02:43.979431 fastapi_sso-0.7.0/fastapi_sso/sso/gitlab.py
--rw-r--r--   0        0        0     1319 2023-03-25 12:01:05.771478 fastapi_sso-0.7.0/fastapi_sso/sso/google.py
--rw-r--r--   0        0        0      753 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/kakao.py
--rw-r--r--   0        0        0     1574 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/microsoft.py
--rw-r--r--   0        0        0      807 2023-07-25 09:20:48.153414 fastapi_sso-0.7.0/fastapi_sso/sso/naver.py
--rw-r--r--   0        0        0     1172 2023-02-07 15:13:40.449140 fastapi_sso-0.7.0/fastapi_sso/sso/spotify.py
--rw-r--r--   0        0        0      944 2023-07-25 18:36:55.041625 fastapi_sso-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     7224 1970-01-01 00:00:00.000000 fastapi_sso-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-02-07 15:13:40.445140 fastapi_sso-0.7.1/LICENSE.md
+-rw-r--r--   0        0        0     6118 2023-07-25 18:36:55.037625 fastapi_sso-0.7.1/README.md
+-rw-r--r--   0        0        0     1110 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/__init__.py
+-rw-r--r--   0        0        0    11117 2023-07-25 18:00:47.042827 fastapi_sso-0.7.1/fastapi_sso/sso/base.py
+-rw-r--r--   0        0        0     1215 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/facebook.py
+-rw-r--r--   0        0        0     1146 2023-03-25 12:01:05.759478 fastapi_sso-0.7.1/fastapi_sso/sso/fitbit.py
+-rw-r--r--   0        0        0     2506 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/generic.py
+-rw-r--r--   0        0        0      918 2023-07-26 10:46:06.524412 fastapi_sso-0.7.1/fastapi_sso/sso/github.py
+-rw-r--r--   0        0        0      920 2023-07-25 18:02:43.979431 fastapi_sso-0.7.1/fastapi_sso/sso/gitlab.py
+-rw-r--r--   0        0        0     1319 2023-03-25 12:01:05.771478 fastapi_sso-0.7.1/fastapi_sso/sso/google.py
+-rw-r--r--   0        0        0      753 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/kakao.py
+-rw-r--r--   0        0        0     1574 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/microsoft.py
+-rw-r--r--   0        0        0      807 2023-07-25 09:20:48.153414 fastapi_sso-0.7.1/fastapi_sso/sso/naver.py
+-rw-r--r--   0        0        0     1172 2023-02-07 15:13:40.449140 fastapi_sso-0.7.1/fastapi_sso/sso/spotify.py
+-rw-r--r--   0        0        0      944 2023-07-26 10:47:48.701371 fastapi_sso-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7224 1970-01-01 00:00:00.000000 fastapi_sso-0.7.1/PKG-INFO
```

### Comparing `fastapi_sso-0.7.0/LICENSE.md` & `fastapi_sso-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/README.md` & `fastapi_sso-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/__init__.py` & `fastapi_sso-0.7.1/fastapi_sso/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/base.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/facebook.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/facebook.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/fitbit.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/fitbit.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/generic.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/generic.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/github.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/github.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,11 +18,11 @@
         }
 
     @classmethod
     async def openid_from_response(cls, response: dict) -> OpenID:
         return OpenID(
             email=response["email"],
             provider=cls.provider,
-            id=response["id"],
+            id=str(response["id"]),
             display_name=response["login"],
             picture=response["avatar_url"],
         )
```

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/gitlab.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/gitlab.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/google.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/google.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/kakao.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/kakao.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/microsoft.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/microsoft.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/naver.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/naver.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/fastapi_sso/sso/spotify.py` & `fastapi_sso-0.7.1/fastapi_sso/sso/spotify.py`

 * *Files identical despite different names*

### Comparing `fastapi_sso-0.7.0/pyproject.toml` & `fastapi_sso-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-sso"
-version = "0.7.0"
+version = "0.7.1"
 description = "FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 Account)"
 authors = ["Tomas Votava <info@tomasvotava.eu>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/tomasvotava/fastapi-sso"
 homepage = "https://tomasvotava.github.io/fastapi-sso/"
 documentation = "https://tomasvotava.github.io/fastapi-sso/"
```

### Comparing `fastapi_sso-0.7.0/PKG-INFO` & `fastapi_sso-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-sso
-Version: 0.7.0
+Version: 0.7.1
 Summary: FastAPI plugin to enable SSO to most common providers (such as Facebook login, Google login and login via Microsoft Office 365 Account)
 Home-page: https://tomasvotava.github.io/fastapi-sso/
 License: MIT
 Keywords: fastapi,sso,oauth,google,facebook,spotify
 Author: Tomas Votava
 Author-email: info@tomasvotava.eu
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-sso Version: 0.7.0 Summary: FastAPI plugin
+Metadata-Version: 2.1 Name: fastapi-sso Version: 0.7.1 Summary: FastAPI plugin
 to enable SSO to most common providers (such as Facebook login, Google login
 and login via Microsoft Office 365 Account) Home-page: https://
 tomasvotava.github.io/fastapi-sso/ License: MIT Keywords:
 fastapi,sso,oauth,google,facebook,spotify Author: Tomas Votava Author-email:
 info@tomasvotava.eu Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

