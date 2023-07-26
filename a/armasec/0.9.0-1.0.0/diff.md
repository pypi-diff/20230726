# Comparing `tmp/armasec-0.9.0.tar.gz` & `tmp/armasec-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armasec-0.9.0.tar", max compression
+gzip compressed data, was "armasec-1.0.0.tar", max compression
```

## Comparing `armasec-0.9.0.tar` & `armasec-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1114 2021-11-24 17:52:26.130754 armasec-0.9.0/LICENSE.rst
--rw-r--r--   0        0        0     2837 2021-11-24 17:52:26.130754 armasec-0.9.0/README.rst
--rw-r--r--   0        0        0      423 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/__init__.py
--rw-r--r--   0        0        0     3415 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/armasec.py
--rw-r--r--   0        0        0      614 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/exceptions.py
--rw-r--r--   0        0        0     3371 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/openid_config_loader.py
--rw-r--r--   0        0        0        0 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/py.typed
--rw-r--r--   0        0        0     7279 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/pytest_extension.py
--rw-r--r--   0        0        0      156 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/schemas/__init__.py
--rw-r--r--   0        0        0      737 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/schemas/jwks.py
--rw-r--r--   0        0        0      483 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/schemas/openid_config.py
--rw-r--r--   0        0        0     3806 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/token_decoder.py
--rw-r--r--   0        0        0     3347 2021-11-24 17:52:26.130754 armasec-0.9.0/armasec/token_manager.py
--rw-r--r--   0        0        0      839 2022-03-14 20:09:18.664165 armasec-0.9.0/armasec/token_payload.py
--rw-r--r--   0        0        0     5831 2022-03-14 18:28:16.514114 armasec-0.9.0/armasec/token_security.py
--rw-r--r--   0        0        0     1104 2022-03-14 18:28:16.514114 armasec-0.9.0/armasec/utilities.py
--rw-r--r--   0        0        0     1851 2022-03-14 20:09:18.664165 armasec-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3939 2022-03-14 20:09:22.319715 armasec-0.9.0/setup.py
--rw-r--r--   0        0        0     3930 2022-03-14 20:09:22.320062 armasec-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1114 2023-07-26 20:26:06.155398 armasec-1.0.0/LICENSE.rst
+-rw-r--r--   0        0        0     2837 2023-07-26 20:26:06.155398 armasec-1.0.0/README.rst
+-rw-r--r--   0        0        0      423 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/__init__.py
+-rw-r--r--   0        0        0     3764 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/armasec.py
+-rw-r--r--   0        0        0      614 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/exceptions.py
+-rw-r--r--   0        0        0     3784 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/openid_config_loader.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/py.typed
+-rw-r--r--   0        0        0     8293 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/pytest_extension.py
+-rw-r--r--   0        0        0      232 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/schemas/__init__.py
+-rw-r--r--   0        0        0     1273 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/schemas/armasec_config.py
+-rw-r--r--   0        0        0      737 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/schemas/jwks.py
+-rw-r--r--   0        0        0      492 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/schemas/openid_config.py
+-rw-r--r--   0        0        0     3806 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/token_decoder.py
+-rw-r--r--   0        0        0     3347 2023-07-26 20:26:06.155398 armasec-1.0.0/armasec/token_manager.py
+-rw-r--r--   0        0        0      804 2023-07-26 20:26:06.159398 armasec-1.0.0/armasec/token_payload.py
+-rw-r--r--   0        0        0     8972 2023-07-26 20:26:06.159398 armasec-1.0.0/armasec/token_security.py
+-rw-r--r--   0        0        0     1104 2023-07-26 20:26:06.159398 armasec-1.0.0/armasec/utilities.py
+-rw-r--r--   0        0        0     1755 2023-07-26 20:26:06.175398 armasec-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3904 1970-01-01 00:00:00.000000 armasec-1.0.0/PKG-INFO
```

### Comparing `armasec-0.9.0/LICENSE.rst` & `armasec-1.0.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `armasec-0.9.0/README.rst` & `armasec-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `armasec-0.9.0/armasec/armasec.py` & `armasec-1.0.0/armasec/armasec.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,58 @@
 """
 This module defines the core Armasec class.
 """
 
 from functools import lru_cache
-from typing import Callable, Optional
+from typing import Callable, List, Optional
 
+from fastapi import HTTPException, status
+
+from armasec.schemas import DomainConfig
 from armasec.token_security import PermissionMode, TokenSecurity
 from armasec.utilities import noop
 
 
 class Armasec:
     """
     This is a factory class for TokenSecurity. It allows the machinery of armasec to be initialized
     correctly so that the factory method `lockdown` can initialize new instances of TokenSecurity
     to protect routes. It's not essential to use Armasec to secure routes, but it cuts down on the
     boilerplate necessary to do so.
     """
 
     def __init__(
         self,
-        domain: str,
-        audience: Optional[str] = None,
-        algorithm: str = "RS256",
+        domain_configs: Optional[List[DomainConfig]] = None,
         debug_logger: Optional[Callable[[str], None]] = noop,
         debug_exceptions: bool = False,
+        **kargs,
     ):
         """
         Stores initialization values for the TokenSecurity. All are passed through.
 
         Args:
-            domain:           The OIDC domain where resources are loaded
-            audience:         Optional designation of the token audience.
-            algorithm:        The the algorithm to use for decoding. Defaults to RS256.
+            domain_configs:   List of domain configuration to authenticate the tokens against.
             debug_logger:     A callable, that if provided, will allow debug logging. Should be
                               passed as a logger method like `logger.debug`
             debug_exceptions: If True, raise original exceptions. Should only be used in a testing
                               or debugging context.
+            kargs:             Arguments compatible to instantiate the DomainConfig model.
         """
-        self.domain = domain
-        self.audience = audience
-        self.algorithm = algorithm
+        primary_domain_config = DomainConfig(**kargs)
+        if primary_domain_config.domain:
+            self.domain_configs = [primary_domain_config]
+        elif domain_configs is not None:
+            self.domain_configs = domain_configs
+        else:
+            raise HTTPException(
+                status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                detail="No domain was input.",
+                headers={"WWW-Authenticate": "Bearer"},
+            )
         self.debug_logger = debug_logger
         self.debug_exceptions = debug_exceptions
 
     @lru_cache(maxsize=128)
     def lockdown(
         self,
         *scopes: str,
@@ -51,17 +60,15 @@
     ) -> TokenSecurity:
         """
         Initialize an instance of TokenSecurity to lockdown a route. Uses memoization to minimize
         the number of TokenSecurity instances initialized. Applies supplied permission_mode when
         checking token permssions against TokenSecurity scopes.
         """
         return TokenSecurity(
-            self.domain,
-            audience=self.audience,
-            algorithm=self.algorithm,
+            domain_configs=self.domain_configs,
             scopes=scopes,
             permission_mode=permission_mode,
             debug_logger=self.debug_logger,
             debug_exceptions=self.debug_exceptions,
         )
 
     def lockdown_all(self, *scopes: str) -> TokenSecurity:
```

### Comparing `armasec-0.9.0/armasec/exceptions.py` & `armasec-1.0.0/armasec/exceptions.py`

 * *Files identical despite different names*

### Comparing `armasec-0.9.0/armasec/openid_config_loader.py` & `armasec-1.0.0/armasec/openid_config_loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,35 +14,45 @@
 from armasec.utilities import log_error, noop
 
 
 class OpenidConfigLoader:
     _config: Optional[OpenidConfig] = None
     _jwks: Optional[JWKs] = None
 
-    def __init__(self, domain: str, debug_logger: Optional[Callable[..., None]] = None):
+    def __init__(
+        self,
+        domain: str,
+        use_https: bool = True,
+        debug_logger: Optional[Callable[..., None]] = None,
+    ):
         """
         Initializes a base TokenManager.
 
         Args:
 
             secret:                  The secret key needed to decode a token
             domain:                  The domain of the OIDC provider. This is to construct the
                                      openid-configuration url
+            use_https:               If falsey, use ``http`` instead of ``https`` (the default).
             debug_logger:            A callable, that if provided, will allow debug logging. Should
                                      be passed as a logger method like `logger.debug`
         """
         self.domain = domain
+        self.use_https = use_https
         self.debug_logger = debug_logger if debug_logger else noop
 
     @staticmethod
-    def build_openid_config_url(domain):
+    def build_openid_config_url(domain: str, use_https: bool = True):
         """
         Builds a url for an openid configuration given a domain.
+
+        If ``use_https`` is not truthy, the url will be built with ``http`` instead.
         """
-        return f"https://{domain}/.well-known/openid-configuration"
+        protocol = "https" if use_https else "http"
+        return f"{protocol}://{domain}/.well-known/openid-configuration"
 
     def _load_openid_resource(self, url: str):
         """
         Helper method to load data from an openid connect resource.
         """
         self.debug_logger(f"Attempting to fetch from openid resource '{url}'")
         with AuthenticationError.handle_errors(
@@ -60,15 +70,17 @@
     def config(self) -> OpenidConfig:
         """
         Retrive the openid config from an OIDC provider. Lazy loads the config so that API calls are
         deferred until the coniguration is needed.
         """
         if not self._config:
             self.debug_logger("Fetching openid configration")
-            data = self._load_openid_resource(self.build_openid_config_url(self.domain))
+            data = self._load_openid_resource(
+                self.build_openid_config_url(self.domain, self.use_https)
+            )
             with AuthenticationError.handle_errors(
                 message="openid config data was invalid",
                 do_except=partial(log_error, self.debug_logger),
             ):
                 self._config = OpenidConfig(**data)
 
         return self._config
```

### Comparing `armasec-0.9.0/armasec/pytest_extension.py` & `armasec-1.0.0/armasec/pytest_extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 """
 This module provides a pytest plugin for testing.
 """
 
 from collections import namedtuple
+from contextlib import _GeneratorContextManager, contextmanager
 from datetime import datetime
-from typing import Optional
+from typing import Callable, Optional
 
 import httpx
 import pytest
 import respx
 import starlette
 from jose import jwt
 from snick import dedent, strip_whitespace
 
 from armasec.openid_config_loader import OpenidConfigLoader
+from armasec.schemas.armasec_config import DomainConfig
 from armasec.schemas.jwks import JWK, JWKs
 from armasec.schemas.openid_config import OpenidConfig
 
 
 @pytest.fixture()
 def rs256_domain():
     """
     Return a domain for use in fixtures from the armasec pytest extension.
     The value here doesn't really have anything to do with an actual domain name.
     """
     return "armasec.dev"
 
 
 @pytest.fixture()
+def rs256_domain_config(rs256_domain):
+    """
+    Return the DomainConfig model for the default rs256 domain.
+    """
+    return DomainConfig(domain=rs256_domain, audience="https://this.api")
+
+
+@pytest.fixture()
 def rs256_iss(rs256_domain):
     """
     Return an issuer claim for use in fixtures from the armasec pytest extension.
     """
     return f"https://{rs256_domain}"
 
 
@@ -190,30 +200,51 @@
     """
     return OpenidConfig(
         issuer=rs256_iss,
         jwks_uri=rs256_jwks_uri,
     )
 
 
+def build_mock_openid_server(
+    domain, openid_config, jwk, jwks_uri
+) -> Callable[[str, OpenidConfig, JWK, str], _GeneratorContextManager]:
+    """
+    Build a helper function to mock the routes used to load the openid-configuration.
+    """
+
+    @contextmanager
+    def _helper(
+        domain: str = domain,
+        openid_config: OpenidConfig = openid_config,
+        jwk: JWK = jwk,
+        jwks_uri: str = jwks_uri,
+    ):
+        MockOpenidRoutes = namedtuple("MockOpenidRoutes", ["openid_config_route", "jwks_route"])
+        with respx.mock:
+            openid_config_route = respx.get(
+                OpenidConfigLoader.build_openid_config_url(domain),
+            )
+            openid_config_route.return_value = httpx.Response(
+                starlette.status.HTTP_200_OK,
+                json=openid_config.dict(),
+            )
+
+            jwks = JWKs(keys=[jwk])
+            jwks_route = respx.get(jwks_uri)
+            jwks_route.return_value = httpx.Response(
+                starlette.status.HTTP_200_OK,
+                json=jwks.dict(),
+            )
+            yield MockOpenidRoutes(openid_config_route, jwks_route)
+
+    return _helper
+
+
 @pytest.fixture
 def mock_openid_server(rs256_domain, rs256_openid_config, rs256_jwk, rs256_jwks_uri):
     """
     Mock routes that would be used in loading an openid-configuration and jwks from a typical
     openid server.
     """
-    MockOpenidRoutes = namedtuple("MockOpenidRoutes", ["openid_config_route", "jwks_route"])
-    with respx.mock:
-        openid_config_route = respx.get(
-            OpenidConfigLoader.build_openid_config_url(rs256_domain),
-        )
-        openid_config_route.return_value = httpx.Response(
-            starlette.status.HTTP_200_OK,
-            json=rs256_openid_config.dict(),
-        )
-
-        jwks = JWKs(keys=[rs256_jwk])
-        jwks_route = respx.get(rs256_jwks_uri)
-        jwks_route.return_value = httpx.Response(
-            starlette.status.HTTP_200_OK,
-            json=jwks.dict(),
-        )
-        yield MockOpenidRoutes(openid_config_route, jwks_route)
+    builder = build_mock_openid_server(rs256_domain, rs256_openid_config, rs256_jwk, rs256_jwks_uri)
+    with builder() as constructed_builder:
+        yield constructed_builder
```

### Comparing `armasec-0.9.0/armasec/schemas/jwks.py` & `armasec-1.0.0/armasec/schemas/jwks.py`

 * *Files identical despite different names*

### Comparing `armasec-0.9.0/armasec/token_decoder.py` & `armasec-1.0.0/armasec/token_decoder.py`

 * *Files identical despite different names*

### Comparing `armasec-0.9.0/armasec/token_manager.py` & `armasec-1.0.0/armasec/token_manager.py`

 * *Files identical despite different names*

### Comparing `armasec-0.9.0/armasec/token_payload.py` & `armasec-1.0.0/armasec/token_payload.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 This module defines a pydantic schema for the payload of a jwt.
 """
-from __future__ import annotations
 
 from datetime import datetime
 from typing import List
 
 from pydantic import BaseModel, Field
```

### Comparing `armasec-0.9.0/armasec/utilities.py` & `armasec-1.0.0/armasec/utilities.py`

 * *Files identical despite different names*

### Comparing `armasec-0.9.0/pyproject.toml` & `armasec-1.0.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 [tool.poetry]
 name = "armasec"
-version = "0.9.0"
+version = "1.0.0"
 description = "Injectable FastAPI auth via OIDC"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/armasec"
 documentation = "https://omnivector-solutions.github.io/armasec"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-python-jose = {extras = ["cryptography"], version = "^3.2.0"}
-fastapi = "^0.68.0"
-httpx = "^0.18.2"
-snick = "^1.0.0"
-py-buzz = "^3.0.0"
+python = "^3.8"
+python-jose = {extras = ["cryptography"], version = "^3.2"}
+fastapi = ">=0.68"
+pydantic = "<2.0"
+httpx = "^0"
+snick = "^1.3"
+py-buzz = "^3.1"
 
 # These must be included as a main dependency for the pytest extension to work out of the box
-respx = "^0.17.1"
-pytest = "^6.2.5"
-auto-name-enum = "^1.0.2"
-
-[tool.poetry.dev-dependencies]
-ipython = "^7.31.0"
-pytest-freezegun = "^0.4.2"
+respx = "^0"
+pytest = ">=6, <8"
+auto-name-enum = "^2"
+
+[tool.poetry.group.dev.dependencies]
+ipython = "^7"
 asgi-lifespan = "^1.0.1"
-httpx = "^0.18.2"
-pytest-asyncio = "^0.15.1"
+pytest-asyncio = "^0"
 pytest-random-order = "^1.0.4"
-mypy = "^0.910"
-isort = "^5.9.3"
+mypy = "^0"
+isort = "^5"
 pytest-sugar = "^0.9.4"
-black = "^22.0"
-python-dotenv = "^0.19.0"
-pytest-cov = "^2.12.1"
-uvicorn = "^0.15.0"
+black = "^22"
+python-dotenv = "^0.19"
+pytest-cov = "^4"
+uvicorn = "^0.15"
 loguru = "^0.5.3"
-Sphinx = "^4.2.0"
-pyproject-flake8 = "^0.0.1-alpha.2"
+Sphinx = "^4"
+pyproject-flake8 = "^5"
+plummet = {extras = ["time-machine"], version = "^1.1.0"}
 
 [tool.poetry.plugins.pytest11]
 pytest_armasec = "armasec.pytest_extension"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 # Unfortunately, pytest-cov breaks when we add armasec.pytest_extension as a pytest plugin
 # TODO: Figure out why this is and how to fix it
-# addopts = "--random-order --cov=armasec --cov-report=term-missing --cov-fail-under=85"
 addopts = "--random-order"
 testpaths = ["tests"]
+asyncio_mode = "auto"
 
 [[tool.mypy.overrides]]
 module = [
     "jose",
     "buzz",
     "snick",
     "auto_name_enum",
```

### Comparing `armasec-0.9.0/PKG-INFO` & `armasec-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: armasec
-Version: 0.9.0
+Version: 1.0.0
 Summary: Injectable FastAPI auth via OIDC
 Home-page: https://github.com/omnivector-solutions/armasec
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: auto-name-enum (>=1.0.2,<2.0.0)
-Requires-Dist: fastapi (>=0.68.0,<0.69.0)
-Requires-Dist: httpx (>=0.18.2,<0.19.0)
-Requires-Dist: py-buzz (>=3.0.0,<4.0.0)
-Requires-Dist: pytest (>=6.2.5,<7.0.0)
-Requires-Dist: python-jose[cryptography] (>=3.2.0,<4.0.0)
-Requires-Dist: respx (>=0.17.1,<0.18.0)
-Requires-Dist: snick (>=1.0.0,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: auto-name-enum (>=2,<3)
+Requires-Dist: fastapi (>=0.68)
+Requires-Dist: httpx (>=0,<1)
+Requires-Dist: py-buzz (>=3.1,<4.0)
+Requires-Dist: pydantic (<2.0)
+Requires-Dist: pytest (>=6,<8)
+Requires-Dist: python-jose[cryptography] (>=3.2,<4.0)
+Requires-Dist: respx (>=0,<1)
+Requires-Dist: snick (>=1.3,<2.0)
 Project-URL: Documentation, https://omnivector-solutions.github.io/armasec
 Project-URL: Repository, https://github.com/omnivector-solutions/armasec
 Description-Content-Type: text/x-rst
 
 .. image:: https://img.shields.io/github/workflow/status/omnivector-solutions/armasec/test_on_push/main?label=main-build&logo=github&style=plastic
    :alt: main build
 .. image:: https://img.shields.io/github/issues/omnivector-solutions/armasec?label=issues&logo=github&style=plastic
```

