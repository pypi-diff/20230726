# Comparing `tmp/jwthenticator-1.3.6.tar.gz` & `tmp/jwthenticator-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwthenticator-1.3.6.tar", max compression
+gzip compressed data, was "jwthenticator-1.3.7.tar", max compression
```

## Comparing `jwthenticator-1.3.6.tar` & `jwthenticator-1.3.7.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    11341 2022-12-13 10:19:32.895357 jwthenticator-1.3.6/LICENSE
--rw-r--r--   0        0        0     7375 2022-12-13 10:19:32.895357 jwthenticator-1.3.6/README.md
--rw-r--r--   0        0        0        0 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/__init__.py
--rw-r--r--   0        0        0     5166 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/api.py
--rw-r--r--   0        0        0    10564 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/client.py
--rw-r--r--   0        0        0     1490 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/consts.py
--rw-r--r--   0        0        0     1228 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/exceptions.py
--rw-r--r--   0        0        0     2842 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/keys.py
--rw-r--r--   0        0        0      207 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/loop_management.py
--rw-r--r--   0        0        0     1359 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/models.py
--rw-r--r--   0        0        0     3744 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/schemas.py
--rw-r--r--   0        0        0     8422 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/server.py
--rw-r--r--   0        0        0     3225 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/server_utils.py
--rw-r--r--   0        0        0     5063 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/tokens.py
--rw-r--r--   0        0        0     3347 2022-12-13 10:19:32.899357 jwthenticator-1.3.6/jwthenticator/utils.py
--rw-r--r--   0        0        0     1628 2022-12-13 10:19:55.979640 jwthenticator-1.3.6/pyproject.toml
--rw-r--r--   0        0        0     8540 1970-01-01 00:00:00.000000 jwthenticator-1.3.6/setup.py
--rw-r--r--   0        0        0     8527 1970-01-01 00:00:00.000000 jwthenticator-1.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/LICENSE
+-rw-r--r--   0        0        0     7375 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/__init__.py
+-rw-r--r--   0        0        0     5166 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/api.py
+-rw-r--r--   0        0        0    10564 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/client.py
+-rw-r--r--   0        0        0     1490 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/consts.py
+-rw-r--r--   0        0        0     1228 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/exceptions.py
+-rw-r--r--   0        0        0     2842 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/keys.py
+-rw-r--r--   0        0        0      207 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/loop_management.py
+-rw-r--r--   0        0        0     1359 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/models.py
+-rw-r--r--   0        0        0     3744 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/schemas.py
+-rw-r--r--   0        0        0     8422 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/server.py
+-rw-r--r--   0        0        0     3225 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/server_utils.py
+-rw-r--r--   0        0        0     5063 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/tokens.py
+-rw-r--r--   0        0        0     3347 2023-07-26 13:12:40.883275 jwthenticator-1.3.7/jwthenticator/utils.py
+-rw-r--r--   0        0        0     1628 2023-07-26 13:13:02.587462 jwthenticator-1.3.7/pyproject.toml
+-rw-r--r--   0        0        0     8527 1970-01-01 00:00:00.000000 jwthenticator-1.3.7/PKG-INFO
```

### Comparing `jwthenticator-1.3.6/LICENSE` & `jwthenticator-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/README.md` & `jwthenticator-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/api.py` & `jwthenticator-1.3.7/jwthenticator/api.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/client.py` & `jwthenticator-1.3.7/jwthenticator/client.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/consts.py` & `jwthenticator-1.3.7/jwthenticator/consts.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/exceptions.py` & `jwthenticator-1.3.7/jwthenticator/exceptions.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/keys.py` & `jwthenticator-1.3.7/jwthenticator/keys.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/models.py` & `jwthenticator-1.3.7/jwthenticator/models.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/schemas.py` & `jwthenticator-1.3.7/jwthenticator/schemas.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/server.py` & `jwthenticator-1.3.7/jwthenticator/server.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/server_utils.py` & `jwthenticator-1.3.7/jwthenticator/server_utils.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/tokens.py` & `jwthenticator-1.3.7/jwthenticator/tokens.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/jwthenticator/utils.py` & `jwthenticator-1.3.7/jwthenticator/utils.py`

 * *Files identical despite different names*

### Comparing `jwthenticator-1.3.6/pyproject.toml` & `jwthenticator-1.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jwthenticator"
-version = "1.3.6"   # For poetry-dynamic-versioning
+version = "1.3.7"   # For poetry-dynamic-versioning
 description = "A cloud first service for key to JWT authentication library and server written in Python 3."
 authors = ["Guy Zylberberg <guyzyl@gmail.com>", "Claroty Open Source <opensource@claroty.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/claroty/jwthenticator"
 documentation = "https://github.com/claroty/jwthenticator"
 exclude = ["jwthenticator/tests"]
@@ -14,15 +14,15 @@
 python = "^3.9"
 sqlalchemy = ">= 1.2.19, < 1.4.0"
 asyncalchemy = "^1.1.1"
 sqlalchemy-utils = ">=0.33.0, < 1.0.0"
 pg8000 = "1.16.5"   # Constant due to - https://github.com/tlocke/pg8000/issues/53
 aiohttp = "^3.6.0"
 pyjwt = ">= 1.7, < 3.0.0"
-cryptography = ">= 2.8, < 39.0.0"   # Required for pyjwt
+cryptography = ">= 2.8, < 40.0.0"   # Required for pyjwt
 marshmallow = "^3.9"
 marshmallow-dataclass = "^8.3"
 pycryptodomex = "^3.9"
 environs = "^9.3.1"
 
 
 [tool.poetry.dev-dependencies]
```

### Comparing `jwthenticator-1.3.6/setup.py` & `jwthenticator-1.3.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,156 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: jwthenticator
+Version: 1.3.7
+Summary: A cloud first service for key to JWT authentication library and server written in Python 3.
+Home-page: https://github.com/claroty/jwthenticator
+License: Apache-2.0
+Author: Guy Zylberberg
+Author-email: guyzyl@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.6.0,<4.0.0)
+Requires-Dist: asyncalchemy (>=1.1.1,<2.0.0)
+Requires-Dist: cryptography (>=2.8,<40.0.0)
+Requires-Dist: environs (>=9.3.1,<10.0.0)
+Requires-Dist: marshmallow (>=3.9,<4.0)
+Requires-Dist: marshmallow-dataclass (>=8.3,<9.0)
+Requires-Dist: pg8000 (==1.16.5)
+Requires-Dist: pycryptodomex (>=3.9,<4.0)
+Requires-Dist: pyjwt (>=1.7,<3.0.0)
+Requires-Dist: sqlalchemy (>=1.2.19,<1.4.0)
+Requires-Dist: sqlalchemy-utils (>=0.33.0,<1.0.0)
+Project-URL: Documentation, https://github.com/claroty/jwthenticator
+Description-Content-Type: text/markdown
+
+# JWThenticator
+A cloud first service for key to JWT authentication library and server written in Python 3.
+
+
+## Intro
+JWThenticator was written for client authentication in micro-services architectures with usage of API gateways in mind.\
+Although there are multiple open-source projects for authenticating users in exchange for JWT (json web token), we couldn't find any project that fit our need for a key based authentication for our clients. This is beneficial for any client authentication and more specifically for IoT.\
+The service is stateless, Docker first service for cloud authentication, but can generally be used for any key to JWT authentication and in multiple different architectures (see example [below](#example-architecture)).
+
+
+## How To Use
+### Pip
+```bash
+pip install jwthenticator
+```
+To run as a server you can run: `python3 -m jwthenticator.server`.\
+Make sure to configure the proper database to be used via the environment variables exposed in [jwthenticator/consts.py](jwthenticator/consts.py) file.\
+By default PostgreSQL is used and a basic local config setup is:
+```bash
+export DB_USER="my-postgres-user"
+export DB_PASS="my-postgres-pass"
+```
+Note - if RSA keys are not provided (via the environment variables `RSA_PUBLIC_KEY` + `RSA_PRIVATE_KEY` or `RSA_PUBLIC_KEY_PATH` + `RSA_PRIVATE_KEY_PATH`), a new RSA pair will be generated every time the systems goes up.
+
+### Docker
+```bash
+docker pull clarotyltd/jwthenticator
+docker run -p 8080:8080 clarotyltd/jwthenticator
+```
+A database is needed to be linked or configured to the image.\
+See [examples/docker-compose.yml](examples/docker-compose.yml) for a full example, run it using:
+```bash
+cd examples
+docker-compose up
+```
+
+### From Source
+The project uses [poetry](https://github.com/python-poetry/poetry) for dependency management and packaging.\
+To run from source clone project and:
+```bash
+pip install poetry
+poetry install
+```
+
+
+## Documentation
+- API documentation - [openapi.yaml](openapi.yaml) file (ex Swagger)
+- Configurable environment variables - [jwthenticator/consts.py](jwthenticator/consts.py)
+- Code usage examples - [Code Examples](#code-examples)
+- Example architecture - [Example Architecture](#example-architecture)
+- Diagrams - [docs](docs) folder for some UML [sequence diagrams](https://sequencediagram.org/) and Python diagrams using [diagrams](https://github.com/mingrammer/diagrams)
+
+
+## Code Examples
+For full examples see the [examples](jwthenticator/examples) folder.
+
+### Client
+To make it easier to work agains a JWThenticator protected server (either directly or via API gateway), a client class is provided.\
+The `Client` class handles auth state management against JWThenticator. It handles JWthenticator responses for you, performs authentication for you, and JWT refresh when needed.\
+It exposes a `request_with_auth` function (and the simpler `get_with_auth` and `post_with_auth`) that manages all interactions against the secured service and the JWThenticator itself for you.\
+Example usage:
+```python
+from uuid import uuid4
+from jwthenticator.client import Client
+
+identifier = uuid4()
+client = Client("https://my-jwthenticator-host/", identifier, key="my-awesome-key")
+response = await client.get_with_auth("https://my-secure-server/")
+```
+
+### Server
+Although JWThenticator was designed with an API gateway in mind, it can be used to authenticate server endpoints directly.\
+For easy usage with an [aiohttp](https://docs.aiohttp.org/en/stable/) Python server you can do the following:
+```python
+from aiohttp import web
+from jwthenticator.server_utils import authenticate
+
+app = web.Application()
+
+@authenticate("https://my-jwthenticator-host/")
+async def secure_index(request: web.Request) -> web.Response:
+    return "Secure hello world!"
+
+app.add_routes([web.get("/", secure_index)])
+web.run_app(app)
+```
+
+
+## Example Architecture
+A visual example on how JWThenticator is and can be used.\
+Additional ones can be found in [docs](docs) folder.
+
+### API Gateway Architecture
+Generated from [docs/api_gateway_architecture_diagram.py](docs/api_gateway_architecture_diagram.py)\
+![API Gateway Architecture](https://user-images.githubusercontent.com/3015856/103092541-3cdd1c00-4600-11eb-807d-6033f6fdfa72.png)
+
+### API Gateway REST Sequence Diagram
+Generated from [docs/api_gateway_flow.diag](docs/api_gateway_flow.diag)\
+![API Gateway REST Sequence Diagram](https://user-images.githubusercontent.com/3015856/103092521-2931b580-4600-11eb-8a0e-a4fb7ccf41c0.png)
+
+## How it works
+There are 3 key components to JWThenticator:
+
+### Keys
+Keys that are registered against the service and can then be used for authentication.\
+All keys are registered to the database, have an expiration time (change default of 30 minutes using the env var `KEY_EXPIRY` in seconds), identifier of the registrant and some other metadata stored about them.\
+The identifier is usefull if a key needs to be linked later to a specific server or route.
+
+### Refresh tokens
+Since JWTs are short lived and keys should be kept safe, an intermediate method is needed so we don't have a long lived JWTs or use our secret key every 30 minutes (by default). This is where refresh token come into play.\
+Refresh tokens are received from a successfull authentication and are used for receiving a new JWTs after they expire.\
+They are recoreded in the database, have an expiration time (change default of 60 days using  the env var `REFRESH_TOKEN_EXPIRY` in seconds) and some other metadata stored about them.\
+You can check out [jwthenticator/models.py](jwthenticator/models.py) to see what data is stored in the database.
+
+### JWTs
+The industry standard JWT ([RFC 7519](https://tools.ietf.org/html/rfc7519)). The JWT is used for verification against an API gateway, JWThenticator itself, or any service / code you use for you auth verification.\
+The JWTs are short lived (as they should be) with a configurable lease time via `JWT_LEASE_TIME` env var.\
+Additionaly, similarly to the keys we use a UUID identifier in the authentication process and store it in the JWT's payload. This is useful for better client identification or smarter k8s routing.
+
+
+## Addtional Features
+- All consts can be overriden via environment variables, see [jwthenticator/consts.py](jwthenticator/consts.py) for the full list.
+- Service contains both internal and public routes, the admin / public API's can be disabled by setting the `DISABLE_EXTERNAL_API` or `DISABLE_INTERNAL_API` env vars. This is very important when running the service in production environments, you don't want to expose the key registration to the general public :).
+- The service can be used with any JWT verification service or API gateway using the industry standard JWKS ([RFC 7517](https://tools.ietf.org/html/rfc7517)) via `/jwks` API call.
+- JWThenticator can be used as an [Nginx authentication](http://nginx.org/en/docs/http/ngx_http_auth_request_module.html) backend using the `/validate_request` API call.
+- Some requests require giving a UUID identifier. Even though the service doesn't enforce its verification, it can be used as a mean of identifiying incoming users, smart routing, and later for additional validations.
+- All REST API schemas are defined using Python `dataclass`es and validated using [marshmallow_dataclass](https://github.com/lovasoa/marshmallow_dataclass), see [schemas.py](jwthenticator/schemas.py).
 
-packages = \
-['jwthenticator']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiohttp>=3.6.0,<4.0.0',
- 'asyncalchemy>=1.1.1,<2.0.0',
- 'cryptography>=2.8,<39.0.0',
- 'environs>=9.3.1,<10.0.0',
- 'marshmallow-dataclass>=8.3,<9.0',
- 'marshmallow>=3.9,<4.0',
- 'pg8000==1.16.5',
- 'pycryptodomex>=3.9,<4.0',
- 'pyjwt>=1.7,<3.0.0',
- 'sqlalchemy-utils>=0.33.0,<1.0.0',
- 'sqlalchemy>=1.2.19,<1.4.0']
-
-setup_kwargs = {
-    'name': 'jwthenticator',
-    'version': '1.3.6',
-    'description': 'A cloud first service for key to JWT authentication library and server written in Python 3.',
-    'long_description': '# JWThenticator\nA cloud first service for key to JWT authentication library and server written in Python 3.\n\n\n## Intro\nJWThenticator was written for client authentication in micro-services architectures with usage of API gateways in mind.\\\nAlthough there are multiple open-source projects for authenticating users in exchange for JWT (json web token), we couldn\'t find any project that fit our need for a key based authentication for our clients. This is beneficial for any client authentication and more specifically for IoT.\\\nThe service is stateless, Docker first service for cloud authentication, but can generally be used for any key to JWT authentication and in multiple different architectures (see example [below](#example-architecture)).\n\n\n## How To Use\n### Pip\n```bash\npip install jwthenticator\n```\nTo run as a server you can run: `python3 -m jwthenticator.server`.\\\nMake sure to configure the proper database to be used via the environment variables exposed in [jwthenticator/consts.py](jwthenticator/consts.py) file.\\\nBy default PostgreSQL is used and a basic local config setup is:\n```bash\nexport DB_USER="my-postgres-user"\nexport DB_PASS="my-postgres-pass"\n```\nNote - if RSA keys are not provided (via the environment variables `RSA_PUBLIC_KEY` + `RSA_PRIVATE_KEY` or `RSA_PUBLIC_KEY_PATH` + `RSA_PRIVATE_KEY_PATH`), a new RSA pair will be generated every time the systems goes up.\n\n### Docker\n```bash\ndocker pull clarotyltd/jwthenticator\ndocker run -p 8080:8080 clarotyltd/jwthenticator\n```\nA database is needed to be linked or configured to the image.\\\nSee [examples/docker-compose.yml](examples/docker-compose.yml) for a full example, run it using:\n```bash\ncd examples\ndocker-compose up\n```\n\n### From Source\nThe project uses [poetry](https://github.com/python-poetry/poetry) for dependency management and packaging.\\\nTo run from source clone project and:\n```bash\npip install poetry\npoetry install\n```\n\n\n## Documentation\n- API documentation - [openapi.yaml](openapi.yaml) file (ex Swagger)\n- Configurable environment variables - [jwthenticator/consts.py](jwthenticator/consts.py)\n- Code usage examples - [Code Examples](#code-examples)\n- Example architecture - [Example Architecture](#example-architecture)\n- Diagrams - [docs](docs) folder for some UML [sequence diagrams](https://sequencediagram.org/) and Python diagrams using [diagrams](https://github.com/mingrammer/diagrams)\n\n\n## Code Examples\nFor full examples see the [examples](jwthenticator/examples) folder.\n\n### Client\nTo make it easier to work agains a JWThenticator protected server (either directly or via API gateway), a client class is provided.\\\nThe `Client` class handles auth state management against JWThenticator. It handles JWthenticator responses for you, performs authentication for you, and JWT refresh when needed.\\\nIt exposes a `request_with_auth` function (and the simpler `get_with_auth` and `post_with_auth`) that manages all interactions against the secured service and the JWThenticator itself for you.\\\nExample usage:\n```python\nfrom uuid import uuid4\nfrom jwthenticator.client import Client\n\nidentifier = uuid4()\nclient = Client("https://my-jwthenticator-host/", identifier, key="my-awesome-key")\nresponse = await client.get_with_auth("https://my-secure-server/")\n```\n\n### Server\nAlthough JWThenticator was designed with an API gateway in mind, it can be used to authenticate server endpoints directly.\\\nFor easy usage with an [aiohttp](https://docs.aiohttp.org/en/stable/) Python server you can do the following:\n```python\nfrom aiohttp import web\nfrom jwthenticator.server_utils import authenticate\n\napp = web.Application()\n\n@authenticate("https://my-jwthenticator-host/")\nasync def secure_index(request: web.Request) -> web.Response:\n    return "Secure hello world!"\n\napp.add_routes([web.get("/", secure_index)])\nweb.run_app(app)\n```\n\n\n## Example Architecture\nA visual example on how JWThenticator is and can be used.\\\nAdditional ones can be found in [docs](docs) folder.\n\n### API Gateway Architecture\nGenerated from [docs/api_gateway_architecture_diagram.py](docs/api_gateway_architecture_diagram.py)\\\n![API Gateway Architecture](https://user-images.githubusercontent.com/3015856/103092541-3cdd1c00-4600-11eb-807d-6033f6fdfa72.png)\n\n### API Gateway REST Sequence Diagram\nGenerated from [docs/api_gateway_flow.diag](docs/api_gateway_flow.diag)\\\n![API Gateway REST Sequence Diagram](https://user-images.githubusercontent.com/3015856/103092521-2931b580-4600-11eb-8a0e-a4fb7ccf41c0.png)\n\n## How it works\nThere are 3 key components to JWThenticator:\n\n### Keys\nKeys that are registered against the service and can then be used for authentication.\\\nAll keys are registered to the database, have an expiration time (change default of 30 minutes using the env var `KEY_EXPIRY` in seconds), identifier of the registrant and some other metadata stored about them.\\\nThe identifier is usefull if a key needs to be linked later to a specific server or route.\n\n### Refresh tokens\nSince JWTs are short lived and keys should be kept safe, an intermediate method is needed so we don\'t have a long lived JWTs or use our secret key every 30 minutes (by default). This is where refresh token come into play.\\\nRefresh tokens are received from a successfull authentication and are used for receiving a new JWTs after they expire.\\\nThey are recoreded in the database, have an expiration time (change default of 60 days using  the env var `REFRESH_TOKEN_EXPIRY` in seconds) and some other metadata stored about them.\\\nYou can check out [jwthenticator/models.py](jwthenticator/models.py) to see what data is stored in the database.\n\n### JWTs\nThe industry standard JWT ([RFC 7519](https://tools.ietf.org/html/rfc7519)). The JWT is used for verification against an API gateway, JWThenticator itself, or any service / code you use for you auth verification.\\\nThe JWTs are short lived (as they should be) with a configurable lease time via `JWT_LEASE_TIME` env var.\\\nAdditionaly, similarly to the keys we use a UUID identifier in the authentication process and store it in the JWT\'s payload. This is useful for better client identification or smarter k8s routing.\n\n\n## Addtional Features\n- All consts can be overriden via environment variables, see [jwthenticator/consts.py](jwthenticator/consts.py) for the full list.\n- Service contains both internal and public routes, the admin / public API\'s can be disabled by setting the `DISABLE_EXTERNAL_API` or `DISABLE_INTERNAL_API` env vars. This is very important when running the service in production environments, you don\'t want to expose the key registration to the general public :).\n- The service can be used with any JWT verification service or API gateway using the industry standard JWKS ([RFC 7517](https://tools.ietf.org/html/rfc7517)) via `/jwks` API call.\n- JWThenticator can be used as an [Nginx authentication](http://nginx.org/en/docs/http/ngx_http_auth_request_module.html) backend using the `/validate_request` API call.\n- Some requests require giving a UUID identifier. Even though the service doesn\'t enforce its verification, it can be used as a mean of identifiying incoming users, smart routing, and later for additional validations.\n- All REST API schemas are defined using Python `dataclass`es and validated using [marshmallow_dataclass](https://github.com/lovasoa/marshmallow_dataclass), see [schemas.py](jwthenticator/schemas.py).\n',
-    'author': 'Guy Zylberberg',
-    'author_email': 'guyzyl@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/claroty/jwthenticator',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

