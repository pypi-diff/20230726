# Comparing `tmp/pyenphase-0.1.0.tar.gz` & `tmp/pyenphase-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.1.0.tar", max compression
+gzip compressed data, was "pyenphase-0.2.0.tar", max compression
```

## Comparing `pyenphase-0.1.0.tar` & `pyenphase-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-05-28 00:12:42.225858 pyenphase-0.1.0/LICENSE
--rw-r--r--   0        0        0     3476 2023-05-28 00:12:42.225858 pyenphase-0.1.0/README.md
--rw-r--r--   0        0        0     2226 2023-05-28 00:12:42.989860 pyenphase-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-28 00:12:42.949860 pyenphase-0.1.0/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     4055 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/auth.py
--rw-r--r--   0        0        0      612 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/const.py
--rw-r--r--   0        0        0     3000 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/envoy.py
--rw-r--r--   0        0        0      446 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1618 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/py.typed
--rw-r--r--   0        0        0      915 2023-05-28 00:12:42.225858 pyenphase-0.1.0/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 pyenphase-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-26 14:39:47.578758 pyenphase-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3476 2023-07-26 14:39:47.578758 pyenphase-0.2.0/README.md
+-rw-r--r--   0        0        0     2246 2023-07-26 14:39:48.378770 pyenphase-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-26 14:39:48.350770 pyenphase-0.2.0/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     4849 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      612 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/const.py
+-rw-r--r--   0        0        0     4505 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0      635 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     1618 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0       53 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/main.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/py.typed
+-rw-r--r--   0        0        0      915 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4649 1970-01-01 00:00:00.000000 pyenphase-0.2.0/PKG-INFO
```

### Comparing `pyenphase-0.1.0/LICENSE` & `pyenphase-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.1.0/README.md` & `pyenphase-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.1.0/pyproject.toml` & `pyenphase-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.1.0"
+version = "0.2.0"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
@@ -24,14 +24,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = ">=0.24.0"
 lxml = ">=4.9.2"
 pyjwt = ">=2.7.0"
 awesomeversion = ">=22.9.0"
+tenacity = "^8.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `pyenphase-0.1.0/src/pyenphase/auth.py` & `pyenphase-0.2.0/src/pyenphase/auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,75 +6,81 @@
 
 from .exceptions import EnvoyAuthenticationError
 
 
 class EnvoyAuth:
     """Base class for Envoy authentication."""
 
-    def __init__(self) -> None:
+    def __init__(self, host: str) -> None:
         """Initialize the EnvoyAuth class."""
         pass
 
-    async def setup(self) -> None:
+    async def setup(self, client: httpx.AsyncClient) -> None:
         """Obtain the token for Envoy authentication."""
         raise NotImplementedError
 
     @property
     def token(self) -> str:
         """Return the Envoy token."""
         raise NotImplementedError
 
+    @property
+    def cookies(self) -> dict[str, str]:
+        """Return the Envoy cookie."""
+        raise NotImplementedError
+
 
 class EnvoyTokenAuth(EnvoyAuth):
     def __init__(
         self,
+        host: str,
         cloud_username: str | None = None,
         cloud_password: str | None = None,
         envoy_serial: str | None = None,
         token: str | None = None,
     ) -> None:
+        self.host = host
         self.cloud_username = cloud_username
         self.cloud_password = cloud_password
         self.envoy_serial = envoy_serial
         self._token = token
 
-    async def setup(self, client: httpx.AsyncClient | None = None) -> None:
+    async def setup(self, client: httpx.AsyncClient) -> None:
         """Obtain the token for Envoy authentication."""
 
         if not self._token:
             # Raise if we don't have cloud credentials
             if not self.cloud_username or not self.cloud_password:
                 raise EnvoyAuthenticationError(
                     "Your firmware requires token authentication, but no cloud credentials were provided to obtain the token."
                 )
             # Raise if we are missing the envoy serial number
             if not self.envoy_serial:
                 raise EnvoyAuthenticationError(
                     "Your firmware requires token authentication, but no envoy serial number was provided to obtain the token."
                 )
 
-            if client is None:
-                # Create a new client if one was not provided
-                self.cloud_client = (
-                    httpx.AsyncClient()
-                )  # we require a new client that checks SSL certs
+            # we require a new client that checks SSL certs
+            self.cloud_client = httpx.AsyncClient()
 
             # Login to Enlighten to obtain a session ID
             data = {
                 "user[email]": self.cloud_username,
                 "user[password]": self.cloud_password,
             }
             req = await self.cloud_client.post(
                 "https://enlighten.enphaseenergy.com/login/login.json?", data=data
             )
             if req.status_code != 200:
                 raise EnvoyAuthenticationError(
                     "Unable to login to Enlighten to obtain session ID."
                 )
             response = json.loads(req.text)
+            self._is_consumer = response["is_consumer"]
+            self._manager_token = response["manager_token"]
 
             # Obtain the token
             data = {
                 "session_id": response["session_id"],
                 "serial_num": self.envoy_serial,
                 "username": self.cloud_username,
             }
@@ -89,24 +95,44 @@
 
         # Verify we have adequate credentials
         if not self.token:
             raise EnvoyAuthenticationError(
                 "Unable to obtain token for Envoy authentication."
             )
 
+        # Verify the token and obtain cookie with session ID necessary for some API calls
+        req = await client.get(
+            f"https://{self.host}/auth/check_jwt",
+            headers={"Authorization": f"Bearer {self.token}"},
+        )
+
+        if req.status_code != 200:
+            raise EnvoyAuthenticationError(
+                "Unable to verify token for Envoy authentication."
+            )
+
+        self._cookies = req.cookies
+
     @property
     def token(self) -> str:
         assert self._token is not None  # nosec
         return self._token
 
     @property
-    def token_header(self) -> str | None:
-        if not self._token:
-            return None
-        return f"Bearer {self._token}"
+    def manager_token(self) -> str:
+        assert self._manager_token is not None  # nosec
+        return self._manager_token
+
+    @property
+    def cookies(self) -> dict[str, str]:
+        return self._cookies
+
+    @property
+    def is_consumer(self) -> bool:
+        return self._is_consumer
 
 
 class EnvoyLegacyAuth(EnvoyAuth):
     """Class for legacy Envoy authentication."""
 
     def __init__(self, host: str, username: str, password: str) -> None:
         self.host = host
```

### Comparing `pyenphase-0.1.0/src/pyenphase/const.py` & `pyenphase-0.2.0/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.1.0/src/pyenphase/firmware.py` & `pyenphase-0.2.0/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.1.0/src/pyenphase/ssl.py` & `pyenphase-0.2.0/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.1.0/PKG-INFO` & `pyenphase-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 0.1.0
+Version: 0.2.0
 Summary: Library to control enphase envoy
 Home-page: https://github.com/pyenphase/pyenphase
 License: MIT
 Author: pyenphase
 Author-email: cgarwood@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: awesomeversion (>=22.9.0)
 Requires-Dist: httpx (>=0.24.0)
 Requires-Dist: lxml (>=4.9.2)
 Requires-Dist: pyjwt (>=2.7.0)
+Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Project-URL: Bug Tracker, https://github.com/pyenphase/pyenphase/issues
 Project-URL: Changelog, https://github.com/pyenphase/pyenphase/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://pyenphase.readthedocs.io
 Project-URL: Repository, https://github.com/pyenphase/pyenphase
 Description-Content-Type: text/markdown
 
 # pyenphase
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: pyenphase Version: 0.1.0 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 0.2.0 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
 Dist: awesomeversion (>=22.9.0) Requires-Dist: httpx (>=0.24.0) Requires-Dist:
-lxml (>=4.9.2) Requires-Dist: pyjwt (>=2.7.0) Project-URL: Bug Tracker, https:/
-/github.com/pyenphase/pyenphase/issues Project-URL: Changelog, https://
-github.com/pyenphase/pyenphase/blob/main/CHANGELOG.md Project-URL:
-Documentation, https://pyenphase.readthedocs.io Project-URL: Repository, https:
-//github.com/pyenphase/pyenphase Description-Content-Type: text/markdown #
-pyenphase
+lxml (>=4.9.2) Requires-Dist: pyjwt (>=2.7.0) Requires-Dist: tenacity
+(>=8.2.2,<9.0.0) Project-URL: Bug Tracker, https://github.com/pyenphase/
+pyenphase/issues Project-URL: Changelog, https://github.com/pyenphase/
+pyenphase/blob/main/CHANGELOG.md Project-URL: Documentation, https://
+pyenphase.readthedocs.io Project-URL: Repository, https://github.com/pyenphase/
+pyenphase Description-Content-Type: text/markdown # pyenphase
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Library to control enphase envoy ## Installation Install this via pip (or your
 favourite package manager): `pip install pyenphase` ## Contributors â¨ Thanks
 goes to these wonderful people ([emoji key](https://allcontributors.org/docs/
 en/emoji-key)):       This project follows the [all-contributors](https://
```

