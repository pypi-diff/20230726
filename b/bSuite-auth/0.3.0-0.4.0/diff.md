# Comparing `tmp/bSuite-auth-0.3.0.tar.gz` & `tmp/bSuite-auth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bSuite-auth-0.3.0.tar", last modified: Wed Jul 26 15:30:11 2023, max compression
+gzip compressed data, was "bSuite-auth-0.4.0.tar", last modified: Wed Jul 26 16:20:46 2023, max compression
```

## Comparing `bSuite-auth-0.3.0.tar` & `bSuite-auth-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-26 15:30:11.901052 bSuite-auth-0.3.0/
--rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-auth-0.3.0/LICENSE
--rw-r--r--   0 birdwell   (501) staff       (20)    40797 2023-07-26 15:30:11.900869 bSuite-auth-0.3.0/PKG-INFO
--rw-r--r--   0 birdwell   (501) staff       (20)       16 2023-07-05 15:45:08.000000 bSuite-auth-0.3.0/README.md
--rw-r--r--   0 birdwell   (501) staff       (20)      825 2023-07-26 15:29:37.000000 bSuite-auth-0.3.0/pyproject.toml
--rw-r--r--   0 birdwell   (501) staff       (20)       38 2023-07-26 15:30:11.901098 bSuite-auth-0.3.0/setup.cfg
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-26 15:30:11.897976 bSuite-auth-0.3.0/src/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-26 15:30:11.897896 bSuite-auth-0.3.0/src/bSuite/
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-26 15:30:11.899565 bSuite-auth-0.3.0/src/bSuite/auth/
--rw-r--r--   0 birdwell   (501) staff       (20)       82 2023-07-25 15:41:27.000000 bSuite-auth-0.3.0/src/bSuite/auth/__init__.py
--rw-r--r--   0 birdwell   (501) staff       (20)     6492 2023-07-25 15:49:48.000000 bSuite-auth-0.3.0/src/bSuite/auth/client.py
--rw-r--r--   0 birdwell   (501) staff       (20)      504 2023-07-25 14:51:11.000000 bSuite-auth-0.3.0/src/bSuite/auth/etc.py
--rw-r--r--   0 birdwell   (501) staff       (20)     3504 2023-07-25 15:58:43.000000 bSuite-auth-0.3.0/src/bSuite/auth/middleware.py
-drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-26 15:30:11.900553 bSuite-auth-0.3.0/src/bSuite_auth.egg-info/
--rw-r--r--   0 birdwell   (501) staff       (20)    40797 2023-07-26 15:30:11.000000 bSuite-auth-0.3.0/src/bSuite_auth.egg-info/PKG-INFO
--rw-r--r--   0 birdwell   (501) staff       (20)      333 2023-07-26 15:30:11.000000 bSuite-auth-0.3.0/src/bSuite_auth.egg-info/SOURCES.txt
--rw-r--r--   0 birdwell   (501) staff       (20)        1 2023-07-26 15:30:11.000000 bSuite-auth-0.3.0/src/bSuite_auth.egg-info/dependency_links.txt
--rw-r--r--   0 birdwell   (501) staff       (20)       27 2023-07-26 15:30:11.000000 bSuite-auth-0.3.0/src/bSuite_auth.egg-info/requires.txt
--rw-r--r--   0 birdwell   (501) staff       (20)        7 2023-07-26 15:30:11.000000 bSuite-auth-0.3.0/src/bSuite_auth.egg-info/top_level.txt
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-26 16:20:46.056572 bSuite-auth-0.4.0/
+-rw-r--r--   0 birdwell   (501) staff       (20)    35148 2023-07-05 15:31:16.000000 bSuite-auth-0.4.0/LICENSE
+-rw-r--r--   0 birdwell   (501) staff       (20)    41150 2023-07-26 16:20:46.056383 bSuite-auth-0.4.0/PKG-INFO
+-rw-r--r--   0 birdwell   (501) staff       (20)      369 2023-07-26 15:54:33.000000 bSuite-auth-0.4.0/README.md
+-rw-r--r--   0 birdwell   (501) staff       (20)      909 2023-07-26 16:20:20.000000 bSuite-auth-0.4.0/pyproject.toml
+-rw-r--r--   0 birdwell   (501) staff       (20)       38 2023-07-26 16:20:46.056625 bSuite-auth-0.4.0/setup.cfg
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-26 16:20:46.048416 bSuite-auth-0.4.0/src/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-26 16:20:46.048346 bSuite-auth-0.4.0/src/bSuite/
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-26 16:20:46.049817 bSuite-auth-0.4.0/src/bSuite/auth/
+-rw-r--r--   0 birdwell   (501) staff       (20)      137 2023-07-26 16:20:20.000000 bSuite-auth-0.4.0/src/bSuite/auth/__init__.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     6394 2023-07-26 16:06:12.000000 bSuite-auth-0.4.0/src/bSuite/auth/client.py
+-rw-r--r--   0 birdwell   (501) staff       (20)      527 2023-07-26 16:06:12.000000 bSuite-auth-0.4.0/src/bSuite/auth/etc.py
+-rw-r--r--   0 birdwell   (501) staff       (20)     3473 2023-07-26 16:06:12.000000 bSuite-auth-0.4.0/src/bSuite/auth/middleware.py
+drwxr-xr-x   0 birdwell   (501) staff       (20)        0 2023-07-26 16:20:46.055989 bSuite-auth-0.4.0/src/bSuite_auth.egg-info/
+-rw-r--r--   0 birdwell   (501) staff       (20)    41150 2023-07-26 16:20:46.000000 bSuite-auth-0.4.0/src/bSuite_auth.egg-info/PKG-INFO
+-rw-r--r--   0 birdwell   (501) staff       (20)      333 2023-07-26 16:20:46.000000 bSuite-auth-0.4.0/src/bSuite_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)        1 2023-07-26 16:20:46.000000 bSuite-auth-0.4.0/src/bSuite_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)       40 2023-07-26 16:20:46.000000 bSuite-auth-0.4.0/src/bSuite_auth.egg-info/requires.txt
+-rw-r--r--   0 birdwell   (501) staff       (20)        7 2023-07-26 16:20:46.000000 bSuite-auth-0.4.0/src/bSuite_auth.egg-info/top_level.txt
```

### Comparing `bSuite-auth-0.3.0/LICENSE` & `bSuite-auth-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bSuite-auth-0.3.0/PKG-INFO` & `bSuite-auth-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bSuite-auth
-Version: 0.3.0
+Version: 0.4.0
 Summary: authentication submodule of bSuite
 Author-email: John Birdwell <j.c.birdwell@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,8 +677,11 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Utility library
+This package contains the bSuite authenticator client for use with WSGI/ASGI backends. 
+bSuite authentication implements a JWT/OAuth analogous flow with slight variations for security. 
+Package provides the base authentication client which can either be used on its own with any backend,
+or the drop-in FastAPI middleware can be used to add authentication in 2 lines.
```

### Comparing `bSuite-auth-0.3.0/pyproject.toml` & `bSuite-auth-0.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 [project]
 name = "bSuite-auth"
-version = "0.3.0"
+version = "0.4.0"
 description = "authentication submodule of bSuite"
 authors = [{name = "John Birdwell", email = "j.c.birdwell@gmail.com"}]
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 
 requires-python = ">=3.11"
-dependencies = ["fastapi", "requests", "starlette"]
+dependencies = ["fastapi", "requests", "starlette", "cryptography"]
 
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.4.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "version bumped {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
+"src/bSuite/auth/__init__.py" = [
+    '__version__ = "{version}"'
+]
```

### Comparing `bSuite-auth-0.3.0/src/bSuite/auth/client.py` & `bSuite-auth-0.4.0/src/bSuite/auth/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,18 @@
 from typing import Optional
 from os import environ as env
 
 from fastapi import Request, Depends
 
 from cryptography.hazmat.primitives.asymmetric.padding import PSS, MGF1
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
-from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives import serialization as cereal
+from cryptography.hazmat.primitives import hashes, serialization as cereal
 from cryptography.exceptions import InvalidSignature
 
-from .etc import AvailableEndpoints, FailedAuth, PreppedAuth, RevokedAuth
-
-
-class HostileEnvironment(Exception):
-    """Missing environmental keys"""
+from .etc import AvailableEndpoints, FailedAuth, PreppedAuth, RevokedAuth, HostileEnvironment
 
 
 class AuthClient:
     @classmethod
     def from_env(cls,
                  *void,
                  client_id: Optional[str] = None,
```

### Comparing `bSuite-auth-0.3.0/src/bSuite/auth/middleware.py` & `bSuite-auth-0.4.0/src/bSuite/auth/middleware.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 from starlette.types import ASGIApp, Receive, Scope, Send
 import typing
 
 from .client import AuthClient
 from .etc import RevokedAuth
 
 
-__all__ = ["AuthMiddleware"]
-
-
 # TODO: ADD base middleware super, implement for redirect jank
 class AuthMiddleware:
     def __init__(
             self,
             app: ASGIApp,
             client: AuthClient,
             available_scopes: typing.Optional[typing.Sequence[str]] = None,
```

### Comparing `bSuite-auth-0.3.0/src/bSuite_auth.egg-info/PKG-INFO` & `bSuite-auth-0.4.0/src/bSuite_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bSuite-auth
-Version: 0.3.0
+Version: 0.4.0
 Summary: authentication submodule of bSuite
 Author-email: John Birdwell <j.c.birdwell@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -677,8 +677,11 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Utility library
+This package contains the bSuite authenticator client for use with WSGI/ASGI backends. 
+bSuite authentication implements a JWT/OAuth analogous flow with slight variations for security. 
+Package provides the base authentication client which can either be used on its own with any backend,
+or the drop-in FastAPI middleware can be used to add authentication in 2 lines.
```

