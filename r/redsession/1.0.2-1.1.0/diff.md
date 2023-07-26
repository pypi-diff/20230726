# Comparing `tmp/redsession-1.0.2.tar.gz` & `tmp/redsession-1.1.0.tar.gz`

## Comparing `redsession-1.0.2.tar` & `redsession-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 redsession-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 redsession-1.0.2/.readthedocs.yaml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 redsession-1.0.2/requirements-docs.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 redsession-1.0.2/requirements-tests.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 redsession-1.0.2/requirements.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 redsession-1.0.2/redsession/__init__.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 redsession-1.0.2/redsession/middleware.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 redsession-1.0.2/redsession/backend/__init__.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 redsession-1.0.2/redsession/backend/base.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 redsession-1.0.2/redsession/backend/redis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redsession-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 redsession-1.0.2/tests/test_session.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 redsession-1.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 redsession-1.0.2/LICENSE.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 redsession-1.0.2/README.rst
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 redsession-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 redsession-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 redsession-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 redsession-1.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 redsession-1.1.0/requirements-docs.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 redsession-1.1.0/requirements-tests.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 redsession-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 redsession-1.1.0/redsession/__init__.py
+-rw-r--r--   0        0        0     6268 2020-02-02 00:00:00.000000 redsession-1.1.0/redsession/middleware.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 redsession-1.1.0/redsession/backend/__init__.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 redsession-1.1.0/redsession/backend/base.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 redsession-1.1.0/redsession/backend/redis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redsession-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 redsession-1.1.0/tests/test_session.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 redsession-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 redsession-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 redsession-1.1.0/README.rst
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 redsession-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 redsession-1.1.0/PKG-INFO
```

### Comparing `redsession-1.0.2/.pre-commit-config.yaml` & `redsession-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `redsession-1.0.2/.readthedocs.yaml` & `redsession-1.1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `redsession-1.0.2/redsession/middleware.py` & `redsession-1.1.0/redsession/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,18 @@
             the session data asynchronously.
 
         secret_key (:class:`~typing.Iterable` | :obj:`str`): A secret
             key used for signing session data. If a list of strings
             is provided, the first element will be used for signing,
             and others for verification (useful for key rotation).
 
+        session_length (:obj:`int`, optional): Session length without hex conversion
+            and without signature. Default is 32. Session length * 2 + 26 (depending on
+            salt) = actual length
+
         name_cookie (:obj:`str`, optional): The name of the session
             cookie. Default is "s".
 
         max_age (:obj:`int`, optional): The maximum age of the session,
             in seconds. Default is 604800 (7 days). If set to 0 or :obj:`None`,
             the session will not expire (**Not recommended**)
 
@@ -47,23 +51,25 @@
     """
 
     def __init__(
         self,
         app: ASGIApp,
         backend: BaseAsyncBackend,
         secret_key: Union[Iterable[str], str],
+        session_length: int = 32,
         name_cookie: str = "s",
         max_age: Optional[int] = 604800,  # 7 days, in seconds
         path: str = "/",
         domain: Optional[str] = None,
         same_site: Literal["lax", "strict", "none"] = "lax",
         https_only: bool = False,
     ) -> None:
         self.app = app
         self.backend = backend
+        self.session_length = session_length
         self.name_cookie = name_cookie
         self.max_age = max_age
         self.path = path
         self.domain = domain
         self.security_flags = "httponly; samesite=" + same_site
 
         if https_only:  # Secure flag can be used with HTTPS only
@@ -105,15 +111,15 @@
 
             headers = MutableHeaders(scope=message)
             cookies = None
 
             if scope["session"]:
                 if initial_session_was_empty:
                     # new session
-                    new_session_id = os.urandom(32).hex()
+                    new_session_id = os.urandom(self.session_length).hex()
                     signer_session = self.signer.sign(new_session_id).decode()
                     await self.backend.set(
                         new_session_id, scope["session"], self.max_age
                     )
 
                     cookies = self._create_cookie(signer_session)
                 else:
```

### Comparing `redsession-1.0.2/redsession/backend/base.py` & `redsession-1.1.0/redsession/backend/base.py`

 * *Files identical despite different names*

### Comparing `redsession-1.0.2/redsession/backend/redis.py` & `redsession-1.1.0/redsession/backend/redis.py`

 * *Files identical despite different names*

### Comparing `redsession-1.0.2/LICENSE.md` & `redsession-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redsession-1.0.2/README.rst` & `redsession-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `redsession-1.0.2/pyproject.toml` & `redsession-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redsession-1.0.2/PKG-INFO` & `redsession-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redsession
-Version: 1.0.2
+Version: 1.1.0
 Summary: Simple and fastest library for Redis server sessions
 Project-URL: Repository, https://github.com/TheJecksMan/red-session
 Project-URL: Docs, https://red-session.readthedocs.io/en/stable/
 Author: TheJecksMan
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 4 - Beta
```

