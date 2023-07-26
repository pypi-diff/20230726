# Comparing `tmp/aio_eapi-0.6.2.tar.gz` & `tmp/aio_eapi-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_eapi-0.6.2.tar", max compression
+gzip compressed data, was "aio_eapi-0.6.3.tar", max compression
```

## Comparing `aio_eapi-0.6.2.tar` & `aio_eapi-0.6.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    11347 2023-01-13 17:41:18.111093 aio_eapi-0.6.2/LICENSE
--rw-r--r--   0        0        0     1379 2023-02-18 18:45:23.202233 aio_eapi-0.6.2/README.md
--rw-r--r--   0        0        0      106 2023-02-18 18:45:23.202985 aio_eapi-0.6.2/aioeapi/__init__.py
--rw-r--r--   0        0        0     1642 2023-03-27 20:00:00.379138 aio_eapi-0.6.2/aioeapi/aio_portcheck.py
--rw-r--r--   0        0        0     8703 2023-06-16 21:10:11.483695 aio_eapi-0.6.2/aioeapi/config_session.py
--rw-r--r--   0        0        0     9881 2023-03-27 20:00:00.380051 aio_eapi-0.6.2/aioeapi/device.py
--rw-r--r--   0        0        0      894 2023-02-18 18:45:23.204799 aio_eapi-0.6.2/aioeapi/errors.py
--rw-r--r--   0        0        0      679 2023-06-16 21:11:27.624122 aio_eapi-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2031 1970-01-01 00:00:00.000000 aio_eapi-0.6.2/setup.py
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 aio_eapi-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11347 2023-07-26 14:28:39.844688 aio_eapi-0.6.3/LICENSE
+-rw-r--r--   0        0        0     1379 2023-07-26 14:28:39.845101 aio_eapi-0.6.3/README.md
+-rw-r--r--   0        0        0      106 2023-07-26 14:28:39.845344 aio_eapi-0.6.3/aioeapi/__init__.py
+-rw-r--r--   0        0        0     1642 2023-07-26 14:28:39.845537 aio_eapi-0.6.3/aioeapi/aio_portcheck.py
+-rw-r--r--   0        0        0     8729 2023-07-26 14:28:39.845776 aio_eapi-0.6.3/aioeapi/config_session.py
+-rw-r--r--   0        0        0     9881 2023-07-26 14:28:39.846028 aio_eapi-0.6.3/aioeapi/device.py
+-rw-r--r--   0        0        0      894 2023-07-26 14:28:39.846174 aio_eapi-0.6.3/aioeapi/errors.py
+-rw-r--r--   0        0        0      679 2023-07-26 14:28:39.846326 aio_eapi-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 aio_eapi-0.6.3/PKG-INFO
```

### Comparing `aio_eapi-0.6.2/LICENSE` & `aio_eapi-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.6.2/README.md` & `aio_eapi-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.6.2/aioeapi/aio_portcheck.py` & `aio_eapi-0.6.3/aioeapi/aio_portcheck.py`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.6.2/aioeapi/config_session.py` & `aio_eapi-0.6.3/aioeapi/config_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -----------------------------------------------------------------------------
 # System Imports
 # -----------------------------------------------------------------------------
 import re
-from typing import Optional, TYPE_CHECKING, Union
+from typing import Optional, TYPE_CHECKING, Union, List
 
 if TYPE_CHECKING:
     from .device import Device
 
 # -----------------------------------------------------------------------------
 # Exports
 # -----------------------------------------------------------------------------
@@ -128,23 +128,25 @@
                 "commitUser": "",
                 "description": ""
             }
         """
         res = await self.status_all()
         return res["sessions"].get(self.name)
 
-    async def push(self, content: Union[list[str], str], replace: Optional[bool] = False):
+    async def push(
+        self, content: Union[List[str], str], replace: Optional[bool] = False
+    ):
         """
         Sends the configuration content to the device.  If `replace` is true,
         then the command "rollback clean-config" is issued before sendig the
         configuration content.
 
         Parameters
         ----------
-        content: list[str] | str
+        content: Union[List[str], str]
             The text configuration CLI commands, as a list of strings, that
             will be sent to the device.  If the parameter is a string, and not
             a list, then split the string across linebreaks.  In either case
             any empty lines will be discarded before they are send to the
             device.
 
         replace: bool
```

### Comparing `aio_eapi-0.6.2/aioeapi/device.py` & `aio_eapi-0.6.3/aioeapi/device.py`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.6.2/aioeapi/errors.py` & `aio_eapi-0.6.3/aioeapi/errors.py`

 * *Files identical despite different names*

### Comparing `aio_eapi-0.6.2/pyproject.toml` & `aio_eapi-0.6.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-eapi"
-version = "0.6.2"
+version = "0.6.3"
 description = "Arista EOS API asyncio client"
 readme = "README.md"
 authors = ["Jeremy Schulman"]
 packages = [
     { include  = 'aioeapi' },
 ]
```

### Comparing `aio_eapi-0.6.2/setup.py` & `aio_eapi-0.6.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,58 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aio-eapi
+Version: 0.6.3
+Summary: Arista EOS API asyncio client
+Author: Jeremy Schulman
+Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Description-Content-Type: text/markdown
+
+# Arista EOS API asyncio Client
+
+This repository contains an Arista EOS asyncio client.
+
+### Quick Example
+
+Thie following shows how to create a Device instance and run a list of
+commands.
+
+Device will use HTTPS transport by default.  The Device instance supports the
+following initialization parameters:
+
+   * `host` - The device hostname or IP address
+   * `username` - The login username
+   * `password` - The login password
+   * `proto` - *(Optional)* Choose either "https" or "http", defaults to "https"
+   * `port` - *(Optional)* Chose the protocol port to override proto default
+
+The Device class inherits directly from httpx.AsyncClient.  As such, the Caller
+can provide any initialization parameters.  The above specific parameters are
+all optional.
+
+```python
+import json
+from aioeapi import Device
+
+username = 'dummy-user'
+password = 'dummy-password'
+
+async def run_test(host):
+    dev = Device(host=host, username=username, password=password)
+    res = await dev.cli(commands=['show hostname', 'show version'])
+    json.dumps(res)
+```
+
+### References
+
+Arista eAPI documents require an Arista Portal customer login.  Once logged into the
+system you can find the documents in the Software Download area.  Select an EOS release
+and then select the Docs folder.
 
-packages = \
-['aioeapi']
+You can also take a look at the Arista community client, [here](https://github.com/arista-eosplus/pyeapi).
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['httpx>=0.23.3,<0.24.0']
-
-setup_kwargs = {
-    'name': 'aio-eapi',
-    'version': '0.6.2',
-    'description': 'Arista EOS API asyncio client',
-    'long_description': '# Arista EOS API asyncio Client\n\nThis repository contains an Arista EOS asyncio client.\n\n### Quick Example\n\nThie following shows how to create a Device instance and run a list of\ncommands.\n\nDevice will use HTTPS transport by default.  The Device instance supports the\nfollowing initialization parameters:\n\n   * `host` - The device hostname or IP address\n   * `username` - The login username\n   * `password` - The login password\n   * `proto` - *(Optional)* Choose either "https" or "http", defaults to "https"\n   * `port` - *(Optional)* Chose the protocol port to override proto default\n\nThe Device class inherits directly from httpx.AsyncClient.  As such, the Caller\ncan provide any initialization parameters.  The above specific parameters are\nall optional.\n\n```python\nimport json\nfrom aioeapi import Device\n\nusername = \'dummy-user\'\npassword = \'dummy-password\'\n\nasync def run_test(host):\n    dev = Device(host=host, username=username, password=password)\n    res = await dev.cli(commands=[\'show hostname\', \'show version\'])\n    json.dumps(res)\n```\n\n### References\n\nArista eAPI documents require an Arista Portal customer login.  Once logged into the\nsystem you can find the documents in the Software Download area.  Select an EOS release\nand then select the Docs folder.\n\nYou can also take a look at the Arista community client, [here](https://github.com/arista-eosplus/pyeapi).\n\n',
-    'author': 'Jeremy Schulman',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8',
-}
-
-
-setup(**setup_kwargs)
```

