# Comparing `tmp/pyenphase-0.2.0.tar.gz` & `tmp/pyenphase-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.2.0.tar", max compression
+gzip compressed data, was "pyenphase-0.3.0.tar", max compression
```

## Comparing `pyenphase-0.2.0.tar` & `pyenphase-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-07-26 14:39:47.578758 pyenphase-0.2.0/LICENSE
--rw-r--r--   0        0        0     3476 2023-07-26 14:39:47.578758 pyenphase-0.2.0/README.md
--rw-r--r--   0        0        0     2246 2023-07-26 14:39:48.378770 pyenphase-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-26 14:39:48.350770 pyenphase-0.2.0/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     4849 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/auth.py
--rw-r--r--   0        0        0      612 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/const.py
--rw-r--r--   0        0        0     4505 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/envoy.py
--rw-r--r--   0        0        0      635 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1618 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/py.typed
--rw-r--r--   0        0        0      915 2023-07-26 14:39:47.578758 pyenphase-0.2.0/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4649 1970-01-01 00:00:00.000000 pyenphase-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-26 17:06:24.293280 pyenphase-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3476 2023-07-26 17:06:24.293280 pyenphase-0.3.0/README.md
+-rw-r--r--   0        0        0     2313 2023-07-26 17:06:25.277304 pyenphase-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-07-26 17:06:25.249303 pyenphase-0.3.0/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     6023 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      612 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/const.py
+-rw-r--r--   0        0        0     5280 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0      896 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     1765 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0       53 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/main.py
+-rw-r--r--   0        0        0        0 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/py.typed
+-rw-r--r--   0        0        0      915 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.3.0/PKG-INFO
```

### Comparing `pyenphase-0.2.0/LICENSE` & `pyenphase-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.2.0/README.md` & `pyenphase-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.2.0/pyproject.toml` & `pyenphase-0.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.2.0"
+version = "0.3.0"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
@@ -25,18 +25,21 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = ">=0.24.0"
 lxml = ">=4.9.2"
 pyjwt = ">=2.7.0"
 awesomeversion = ">=22.9.0"
 tenacity = "^8.2.2"
+envoy-utils = ">=0.0.1"
+orjson = ">=3.9.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
+types-orjson = "^3.6.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
```

### Comparing `pyenphase-0.2.0/src/pyenphase/auth.py` & `pyenphase-0.3.0/src/pyenphase/auth.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 """Envoy authentication methods."""
 
 import json
+from abc import abstractmethod, abstractproperty
 
 import httpx
 
 from .exceptions import EnvoyAuthenticationError
 
 
 class EnvoyAuth:
     """Base class for Envoy authentication."""
 
     def __init__(self, host: str) -> None:
         """Initialize the EnvoyAuth class."""
         pass
 
+    @abstractmethod
     async def setup(self, client: httpx.AsyncClient) -> None:
         """Obtain the token for Envoy authentication."""
-        raise NotImplementedError
 
-    @property
-    def token(self) -> str:
-        """Return the Envoy token."""
-        raise NotImplementedError
-
-    @property
+    @abstractproperty
     def cookies(self) -> dict[str, str]:
         """Return the Envoy cookie."""
-        raise NotImplementedError
+
+    @abstractproperty
+    def auth(self) -> httpx.DigestAuth | None:
+        """Return the httpx auth object."""
+
+    @abstractproperty
+    def headers(self) -> dict[str, str]:
+        """Return the auth headers."""
+
+    @abstractmethod
+    def get_endpoint_url(self, endpoint: str) -> str:
+        """Return the URL for the endpoint."""
 
 
 class EnvoyTokenAuth(EnvoyAuth):
     def __init__(
         self,
         host: str,
         cloud_username: str | None = None,
@@ -126,22 +133,53 @@
     def cookies(self) -> dict[str, str]:
         return self._cookies
 
     @property
     def is_consumer(self) -> bool:
         return self._is_consumer
 
+    @property
+    def auth(self) -> None:
+        """No auth required for token authentication."""
+        return None
+
+    @property
+    def headers(self) -> dict[str, str]:
+        """Return the headers for Envoy authentication."""
+        return {"Authorization": f"Bearer {self.token}"}
+
+    def get_endpoint_url(self, endpoint: str) -> str:
+        """Return the URL for the endpoint."""
+        return f"https://{self.host}{endpoint}"
+
 
 class EnvoyLegacyAuth(EnvoyAuth):
     """Class for legacy Envoy authentication."""
 
     def __init__(self, host: str, username: str, password: str) -> None:
         self.host = host
         self.local_username = username
         self.local_password = password
 
     @property
-    def local_auth(self) -> httpx.DigestAuth:
+    def auth(self) -> httpx.DigestAuth:
         """Digest authentication for local Envoy."""
         if not self.local_username or not self.local_password:
             return None
         return httpx.DigestAuth(self.local_username, self.local_password)
+
+    async def setup(self, client: httpx.AsyncClient) -> None:
+        """Setup auth"""
+        # No setup required for legacy authentication
+
+    @property
+    def headers(self) -> dict[str, str]:
+        """Return the headers for legacy Envoy authentication."""
+        return {}
+
+    def get_endpoint_url(self, endpoint: str) -> str:
+        """Return the URL for the endpoint."""
+        return f"http://{self.host}{endpoint}"
+
+    @property
+    def cookies(self) -> dict[str, str]:
+        return {}
```

### Comparing `pyenphase-0.2.0/src/pyenphase/const.py` & `pyenphase-0.3.0/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.2.0/src/pyenphase/envoy.py` & `pyenphase-0.3.0/src/pyenphase/envoy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import contextlib
 import logging
 import ssl
 from typing import Any
 
 import httpx
+import orjson
 from awesomeversion import AwesomeVersion
+from envoy_utils.envoy_utils import EnvoyUtils
 from tenacity import retry, retry_if_exception_type, wait_random_exponential
 
-from .auth import EnvoyAuth, EnvoyTokenAuth
+from .auth import EnvoyAuth, EnvoyLegacyAuth, EnvoyTokenAuth
 from .exceptions import EnvoyAuthenticationRequired
 from .firmware import EnvoyFirmware, EnvoyFirmwareCheckError
 
 _LOGGER = logging.getLogger(__name__)
 
+TIMEOUT = 15
+LEGACY_ENVOY_VERSION = AwesomeVersion("3.9.0")
+AUTH_TOKEN_MIN_VERSION = AwesomeVersion("7.0.0")
+DEFAULT_HEADERS = {
+    "Accept": "application/json",
+}
+
 
 def create_no_verify_ssl_context() -> ssl.SSLContext:
     """Return an SSL context that does not verify the server certificate.
     This is a copy of aiohttp's create_default_context() function, with the
     ssl verify turned off and old SSL versions enabled.
 
     https://github.com/aio-libs/aiohttp/blob/33953f110e97eecc707e1402daa8d543f38a189b/aiohttp/connector.py#L911
@@ -38,15 +47,17 @@
 
 class Envoy:
     """Class for querying and determining the Envoy firmware version."""
 
     def __init__(self, host: str) -> None:
         """Initialize the Envoy class."""
         # We use our own httpx client session so we can disable SSL verification (Envoys use self-signed SSL certs)
-        self._client = httpx.AsyncClient(verify=_NO_VERIFY_SSL_CONTEXT)  # nosec
+        self._client = httpx.AsyncClient(
+            verify=_NO_VERIFY_SSL_CONTEXT, timeout=TIMEOUT
+        )  # nosec
         self.auth: EnvoyAuth | None = None
         self._host = host
         self._firmware = EnvoyFirmware(self._client, self._host)
 
     @retry(
         retry=retry_if_exception_type(EnvoyFirmwareCheckError),
         wait=wait_random_exponential(multiplier=2, max=10),
@@ -58,62 +69,71 @@
     async def authenticate(
         self,
         username: str | None = None,
         password: str | None = None,
         token: str | None = None,
     ) -> None:
         """Authenticate to the Envoy based on firmware version."""
-        if self._firmware.version < AwesomeVersion("3.9.0"):
+        if self._firmware.version < LEGACY_ENVOY_VERSION:
             # Legacy Envoy firmware
             _LOGGER.debug("Authenticating to Envoy using legacy authentication")
 
-        if AwesomeVersion("3.9.0") <= self._firmware.version < AwesomeVersion("7.0.0"):
+        if LEGACY_ENVOY_VERSION <= self._firmware.version < AUTH_TOKEN_MIN_VERSION:
             # Envoy firmware using old envoy/installer authentication
             _LOGGER.debug(
                 "Authenticating to Envoy using envoy/installer authentication"
             )
+            full_serial = self._firmware.serial
+            if username is None:
+                username = "installer"
+                password = EnvoyUtils.get_password(full_serial, username)
+            elif username == "envoy" and password is None:
+                # The default password for the envoy user is the first 6 digits of the serial number
+                password = full_serial[:6]
+
+            if username and password:
+                self.auth = EnvoyLegacyAuth(self.host, username, password)
 
-        if self._firmware.version >= AwesomeVersion("7.0.0"):
+        if self._firmware.version >= AUTH_TOKEN_MIN_VERSION:
             # Envoy firmware using new token authentication
             _LOGGER.debug("Authenticating to Envoy using token authentication")
             if token is not None:
                 self.auth = EnvoyTokenAuth(self.host, token=token)
             elif (
                 username is not None
                 and password is not None
                 and self._firmware.serial is not None
             ):
                 self.auth = EnvoyTokenAuth(
                     self.host, username, password, self._firmware.serial
                 )
 
-        if self.auth is not None:
-            await self.auth.setup(self._client)
-        else:
+        if not self.auth:
             _LOGGER.error(
                 "You must include username/password or token to authenticate to the Envoy."
             )
             raise EnvoyAuthenticationRequired("Could not setup authentication object.")
 
+        await self.auth.setup(self._client)
+
     async def request(self, endpoint: str) -> dict[str, Any]:
         """Make a request to the Envoy."""
         if self.auth is None:
             raise EnvoyAuthenticationRequired(
                 "You must authenticate to the Envoy before making requests."
             )
 
-        r = await self._client.get(
-            f"https://{self._host}{endpoint}",
-            headers={
-                "Accept": "application/json",
-                "Authorization": f"Bearer {self.auth.token}",
-            },
+        response = await self._client.get(
+            self.auth.get_endpoint_url(endpoint),
+            headers={**DEFAULT_HEADERS, **self.auth.headers},
             cookies=self.auth.cookies,
+            follow_redirects=True,
+            auth=self.auth.auth,
         )
-        return r.json()
+        return orjson.loads(response.text)
 
     @property
     def host(self) -> str:
         """Return the Envoy host."""
         return self._host
 
     @property
```

### Comparing `pyenphase-0.2.0/src/pyenphase/exceptions.py` & `pyenphase-0.3.0/src/pyenphase/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,22 @@
     """Exception raised when unable to query the Envoy firmware version."""
 
     def __init__(self, status_code: int, status: str) -> None:
         self.status_code = status_code
         self.status = status
 
 
+class EnvoyFirmwareFatalCheckError(Exception):
+    """Exception raised when we should not retry the Envoy firmware version."""
+
+    def __init__(self, status_code: int, status: str) -> None:
+        self.status_code = status_code
+        self.status = status
+
+
 class EnvoyAuthenticationError(Exception):
     """Exception raised when unable to query the Envoy firmware version."""
 
     def __init__(self, status: str) -> None:
         self.status = status
```

### Comparing `pyenphase-0.2.0/src/pyenphase/firmware.py` & `pyenphase-0.3.0/src/pyenphase/firmware.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import httpx
 from awesomeversion import AwesomeVersion
 from lxml import etree  # nosec
 
-from .exceptions import EnvoyFirmwareCheckError
+from .exceptions import EnvoyFirmwareCheckError, EnvoyFirmwareFatalCheckError
 
 
 class EnvoyFirmware:
     """Class for querying and determining the Envoy firmware version."""
 
     def __init__(self, _client: httpx.AsyncClient, host: str) -> None:
         self._client = _client
         self._host = host
 
     async def setup(self) -> None:
         """Obtain the firmware version for Envoy authentication."""
         # <envoy>/info will return XML with the firmware version
         try:
             result = await self._client.get(f"http://{self._host}/info")
+        except httpx.ConnectError:
+            raise EnvoyFirmwareFatalCheckError(500, "Unable to connect to Envoy")
         except httpx.HTTPError:
             raise EnvoyFirmwareCheckError(500, "Unable to query firmware version")
 
         if result.status_code == 200:
             xml = etree.fromstring(result.content)  # nosec
             if (device_tag := xml.find("device")) is not None:
                 if (software_tag := device_tag.find("software")) is not None:
```

### Comparing `pyenphase-0.2.0/src/pyenphase/ssl.py` & `pyenphase-0.3.0/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.2.0/PKG-INFO` & `pyenphase-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 0.2.0
+Version: 0.3.0
 Summary: Library to control enphase envoy
 Home-page: https://github.com/pyenphase/pyenphase
 License: MIT
 Author: pyenphase
 Author-email: cgarwood@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -13,16 +13,18 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: awesomeversion (>=22.9.0)
+Requires-Dist: envoy-utils (>=0.0.1)
 Requires-Dist: httpx (>=0.24.0)
 Requires-Dist: lxml (>=4.9.2)
+Requires-Dist: orjson (>=3.9.2)
 Requires-Dist: pyjwt (>=2.7.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Project-URL: Bug Tracker, https://github.com/pyenphase/pyenphase/issues
 Project-URL: Changelog, https://github.com/pyenphase/pyenphase/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://pyenphase.readthedocs.io
 Project-URL: Repository, https://github.com/pyenphase/pyenphase
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: pyenphase Version: 0.2.0 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 0.3.0 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Topic :: Software Development :: Libraries Requires-
-Dist: awesomeversion (>=22.9.0) Requires-Dist: httpx (>=0.24.0) Requires-Dist:
-lxml (>=4.9.2) Requires-Dist: pyjwt (>=2.7.0) Requires-Dist: tenacity
+Dist: awesomeversion (>=22.9.0) Requires-Dist: envoy-utils (>=0.0.1) Requires-
+Dist: httpx (>=0.24.0) Requires-Dist: lxml (>=4.9.2) Requires-Dist: orjson
+(>=3.9.2) Requires-Dist: pyjwt (>=2.7.0) Requires-Dist: tenacity
 (>=8.2.2,<9.0.0) Project-URL: Bug Tracker, https://github.com/pyenphase/
 pyenphase/issues Project-URL: Changelog, https://github.com/pyenphase/
 pyenphase/blob/main/CHANGELOG.md Project-URL: Documentation, https://
 pyenphase.readthedocs.io Project-URL: Repository, https://github.com/pyenphase/
 pyenphase Description-Content-Type: text/markdown # pyenphase
          [CI_Status] [Documentation_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
```

