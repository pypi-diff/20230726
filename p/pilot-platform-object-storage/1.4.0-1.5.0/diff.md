# Comparing `tmp/pilot_platform_object_storage-1.4.0.tar.gz` & `tmp/pilot_platform_object_storage-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot_platform_object_storage-1.4.0.tar", max compression
+gzip compressed data, was "pilot_platform_object_storage-1.5.0.tar", max compression
```

## Comparing `pilot_platform_object_storage-1.4.0.tar` & `pilot_platform_object_storage-1.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3493 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/README.md
--rw-r--r--   0        0        0      120 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/__init__.py
--rw-r--r--   0        0        0      324 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/clients/__init__.py
--rw-r--r--   0        0        0     6885 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/clients/azure_blob_client.py
--rw-r--r--   0        0        0     8332 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/clients/azure_container_client.py
--rw-r--r--   0        0        0     2649 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/clients/base_container_client.py
--rw-r--r--   0        0        0     2190 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/clients/base_file_client.py
--rw-r--r--   0        0        0     1902 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/factories.py
--rw-r--r--   0        0        0      239 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/managers/__init__.py
--rw-r--r--   0        0        0     4530 2023-07-17 08:56:22.060564 pilot_platform_object_storage-1.4.0/object_storage/managers/azure_blob_manager.py
--rw-r--r--   0        0        0     1134 2023-07-17 08:56:22.064564 pilot_platform_object_storage-1.4.0/object_storage/managers/base_manager.py
--rw-r--r--   0        0        0      266 2023-07-17 08:56:22.064564 pilot_platform_object_storage-1.4.0/object_storage/providers/__init__.py
--rw-r--r--   0        0        0     7186 2023-07-17 08:56:22.064564 pilot_platform_object_storage-1.4.0/object_storage/providers/azure.py
--rw-r--r--   0        0        0      444 2023-07-17 08:56:22.064564 pilot_platform_object_storage-1.4.0/object_storage/providers/enum.py
--rw-r--r--   0        0        0     1181 2023-07-17 08:56:22.064564 pilot_platform_object_storage-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.4.0/setup.py
--rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     3493 2023-07-26 13:58:38.139773 pilot_platform_object_storage-1.5.0/README.md
+-rw-r--r--   0        0        0      120 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/__init__.py
+-rw-r--r--   0        0        0      324 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/clients/__init__.py
+-rw-r--r--   0        0        0     7574 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/clients/azure_blob_client.py
+-rw-r--r--   0        0        0     9116 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/clients/azure_container_client.py
+-rw-r--r--   0        0        0     2649 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/clients/base_container_client.py
+-rw-r--r--   0        0        0     2190 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/clients/base_file_client.py
+-rw-r--r--   0        0        0     1902 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/factories.py
+-rw-r--r--   0        0        0      239 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/managers/__init__.py
+-rw-r--r--   0        0        0     4530 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/managers/azure_blob_manager.py
+-rw-r--r--   0        0        0     1134 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/managers/base_manager.py
+-rw-r--r--   0        0        0      266 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/providers/__init__.py
+-rw-r--r--   0        0        0     7896 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/providers/azure.py
+-rw-r--r--   0        0        0      444 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/object_storage/providers/enum.py
+-rw-r--r--   0        0        0     1181 2023-07-26 13:58:38.143773 pilot_platform_object_storage-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4437 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.5.0/setup.py
+-rw-r--r--   0        0        0     4221 1970-01-01 00:00:00.000000 pilot_platform_object_storage-1.5.0/PKG-INFO
```

### Comparing `pilot_platform_object_storage-1.4.0/README.md` & `pilot_platform_object_storage-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.4.0/object_storage/clients/azure_blob_client.py` & `pilot_platform_object_storage-1.5.0/object_storage/clients/azure_blob_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
 import logging
+from io import BytesIO
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
@@ -70,14 +71,29 @@
         key = self._get_blob_name_from_sas()
         try:
             async with BlobClient.from_blob_url(blob_url=self.blob_sas_url, max_block_size=chunk_size) as blob_client:
                 return await self._upload(blob_client, file_path, key, progress_callback, chunk_size=chunk_size)
         except Exception as exc:
             raise self._handle_exception(exc)
 
+    async def upload_file_from_bytes(
+        self,
+        buffer: BytesIO,
+        chunk_size: int = 4 * 1024 * 1024,
+        progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
+    ) -> Dict[str, Any]:
+        """Uploads a file to a blob in the specified container."""
+
+        key = self._get_blob_name_from_sas()
+        try:
+            async with BlobClient.from_blob_url(blob_url=self.blob_sas_url, max_block_size=chunk_size) as blob_client:
+                return await self._upload_from_byte(blob_client, key, buffer, chunk_size, progress_callback)
+        except Exception as exc:
+            raise self._handle_exception(exc)
+
     async def resume_upload(
         self,
         file_path: str,
         chunk_size: int = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
         """Uploads a file to an Azure Blob Storage container, resuming an interrupted upload if there is an uncommitted
```

### Comparing `pilot_platform_object_storage-1.4.0/object_storage/clients/azure_container_client.py` & `pilot_platform_object_storage-1.5.0/object_storage/clients/azure_container_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
 import logging
+from io import BytesIO
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
@@ -78,14 +79,31 @@
                 container_url=self.container_sas_url, max_block_size=chunk_size
             ) as container_client:
                 blob_client = container_client.get_blob_client(key)
                 return await self._upload(blob_client, file_path, key, progress_callback, chunk_size=chunk_size)
         except Exception as exc:
             raise self._handle_exception(exc)
 
+    async def upload_file_from_bytes(
+        self,
+        key: str,
+        buffer: BytesIO,
+        chunk_size: int = 4 * 1024 * 1024,
+        progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
+    ) -> Dict[str, Any]:
+        """Uploads a file to a blob in the specified container."""
+        try:
+            async with ContainerClient.from_container_url(
+                container_url=self.container_sas_url, max_block_size=chunk_size
+            ) as container_client:
+                blob_client = container_client.get_blob_client(key)
+                return await self._upload_from_byte(blob_client, key, buffer, chunk_size, progress_callback)
+        except Exception as exc:
+            raise self._handle_exception(exc)
+
     async def resume_upload(
         self,
         key: str,
         file_path: str,
         chunk_size: int = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
     ) -> None:
```

### Comparing `pilot_platform_object_storage-1.4.0/object_storage/clients/base_container_client.py` & `pilot_platform_object_storage-1.5.0/object_storage/clients/base_container_client.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.4.0/object_storage/clients/base_file_client.py` & `pilot_platform_object_storage-1.5.0/object_storage/clients/base_file_client.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.4.0/object_storage/factories.py` & `pilot_platform_object_storage-1.5.0/object_storage/factories.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.4.0/object_storage/managers/azure_blob_manager.py` & `pilot_platform_object_storage-1.5.0/object_storage/managers/azure_blob_manager.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.4.0/object_storage/managers/base_manager.py` & `pilot_platform_object_storage-1.5.0/object_storage/managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `pilot_platform_object_storage-1.4.0/object_storage/providers/azure.py` & `pilot_platform_object_storage-1.5.0/object_storage/providers/azure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Copyright (C) 2023 Indoc Research
 #
 # Contact Indoc Research for any questions regarding the use of this source code.
 
 import logging
+from io import BytesIO
 from pathlib import Path
 from typing import Any
 from typing import Awaitable
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
+from typing import Union
 from uuid import uuid4
 
 import aiofiles
 import aiofiles.os
 from aiofiles.os import makedirs
 from aiofiles.threadpool.binary import AsyncBufferedReader
 from azure.core.exceptions import ClientAuthenticationError
@@ -56,46 +58,62 @@
         key: str,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
         chunk_size: int = 4 * 1024 * 1024,
     ) -> Dict[str, Any]:
         """Upload a file to sas URL."""
 
         async with aiofiles.open(file_path, mode='rb') as f:
-            uploaded_blocks = await self._upload_chunks(client, file_path, key, f, chunk_size, progress_callback)
+            file_length = (await aiofiles.os.stat(file_path)).st_size
+            uploaded_blocks = await self._upload_chunks(client, f, file_length, key, chunk_size, progress_callback)
             return await self._commit_blob(client, uploaded_blocks)
 
     async def _upload_chunks(
         self,
         client: BlobClient,
-        file_path: str,
+        file_obj: Union[AsyncBufferedReader, BytesIO],
+        file_length: int,
         key: str,
-        file_obj: AsyncBufferedReader,  # has to be checked the correct type
         chunk_size: int = 4 * 1024 * 1024,
         progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
         current: int = 0,
     ) -> List[BlobBlock]:
         """Upload the file by cutting into chunks.
 
         If there is progress callback, will upload the chunk from the current point.
         """
         uploaded_blocks = []
-        file_length = (await aiofiles.os.stat(file_path)).st_size
-
         while True:
-            chunk = await file_obj.read(chunk_size)
+            if isinstance(file_obj, BytesIO):
+                chunk = file_obj.read(chunk_size)
+            else:
+                chunk = await file_obj.read(chunk_size)
             if not chunk:
                 break
             block_id = str(uuid4())
             await client.stage_block(block_id=block_id, data=chunk)
+            current = min(current + len(chunk), file_length)
             if progress_callback:
-                current = min(current + chunk_size, file_length)
                 await progress_callback(key, current, file_length)
             uploaded_blocks.append(BlobBlock(block_id=block_id))
         return uploaded_blocks
 
+    async def _upload_from_byte(
+        self,
+        client: BlobClient,
+        key: str,
+        buffer: BytesIO,
+        chunk_size: int = 4 * 1024 * 1024,
+        progress_callback: Optional[Callable[[str, int, int], Awaitable[Any]]] = None,
+    ) -> Dict[str, Any]:
+        """Upload a file from bytes to the specified container."""
+
+        length = buffer.getbuffer().nbytes
+        uploaded_blocks = await self._upload_chunks(client, buffer, length, key, chunk_size, progress_callback)
+        return await self._commit_blob(client, uploaded_blocks)
+
     async def _commit_blob(self, client: BlobClient, block_list: Optional[List[BlobBlock]] = None) -> Dict[str, Any]:
         """Commits the uncommitted blocks of a blob, making them a part of the blob's content."""
         if block_list:
             return await client.commit_block_list(block_list)
         _, block_list = await client.get_block_list('uncommitted')
         return await client.commit_block_list(block_list)
 
@@ -173,15 +191,15 @@
         file_length = (await aiofiles.os.stat(file_path)).st_size
         file_renaming_length = file_length - offset
 
         if file_renaming_length:
             async with aiofiles.open(file_path, mode='rb') as f:
                 await f.seek(offset)
                 uploaded_blocks += await self._upload_chunks(
-                    client, file_path, key, f, chunk_size, progress_callback, current
+                    client, f, file_length, key, chunk_size, progress_callback, current
                 )
 
         await self._commit_blob(client, uploaded_blocks)
 
     async def _get_blob_chunks(
         self,
         client: BlobClient,
```

### Comparing `pilot_platform_object_storage-1.4.0/pyproject.toml` & `pilot_platform_object_storage-1.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pilot-platform-object-storage"
-version = "1.4.0"
+version = "1.5.0"
 description = "Python library for interacting with multiple object storage APIs."
 authors = ["Indoc Research"]
 readme = "README.md"
 packages = [{include = "object_storage"}]
 license = "Proprietary"
 documentation = "https://pilotdataplatform.github.io/object-storage/"
```

### Comparing `pilot_platform_object_storage-1.4.0/setup.py` & `pilot_platform_object_storage-1.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 install_requires = \
 ['aiofiles>=23.1.0,<24.0.0',
  'aiohttp>=3.8.4,<4.0.0',
  'azure-storage-blob>=12.16.0,<13.0.0']
 
 setup_kwargs = {
     'name': 'pilot-platform-object-storage',
-    'version': '1.4.0',
+    'version': '1.5.0',
     'description': 'Python library for interacting with multiple object storage APIs.',
     'long_description': '# Pilot Platform Storage Manager\n\n[![Run Tests](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml/badge.svg?branch=develop)](https://github.com/PilotDataPlatform/object-storage/actions/workflows/run-tests.yml)\n[![Python](https://img.shields.io/badge/python-3.9-brightgreen.svg)](https://www.python.org/)\n[![PyPI](https://img.shields.io/pypi/v/pilot-platform-object-storage.svg)](https://pypi.org/project/pilot-platform-object-storage/)\n\nProvides a simple and flexible Python library for efficient and reliable object storage solutions. Enables direct interaction with multiple object storage APIs, starting with Azure Blob API and with plans to add more in the future\n\n## Getting Started\n\n### Manager\n```python\nimport asyncio\nfrom object_storage.factories import get_manager\n\nconnection_string = \'DefaultEndpointsProtocol=https;AccountName=pilot;AccountKey=any;EndpointSuffix=core.windows.net\'\nazr_manager = get_manager(\'azure\', connection_string)\n\naccount_sas = asyncio.run(azr_manager.get_container_sas(\'test\'))\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\n\n\nblob_sas = asyncio.run(azr_manager.get_blob_sas(\'test\', \'small.txt\'))\n\nprint(blob_sas)\n> \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=blob_signature\'\n\n\nblobs_list = asyncio.run(azr_manager.list_objects(\'test\'))\nprint(blobs_list)\n> [<class \'azure.storage.blob._models.BlobProperties\'>, ...]\n\n\nblobs_list = asyncio.run(azr_manager.create_container(\'test\'))\n```\n\n### File Client\n```python\nimport asyncio\nfrom object_storage.factories import get_file_client\n\nblob_sas_url = \'https://pilot.blob.core.windows.net/test/file.txt?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_file_client = get_file_client(\'azure\', blob_sas_url)\nasyncio.run(azr_file_client.upload_file(\'./small.txt\'))\n```\n\n### Container Client\n```python\nimport asyncio\nfrom object_storage.factories import get_container_client\n\ncontainer_sas_url = \'https://pilot.blob.core.windows.net/test?sp=rw&st=2023-04-28T15:15:14Z&se=2023-04-28T23:15:14Z&spr=https&sv=2021-12-02&sr=b&sig=account_signature\'\nazr_container_client = get_container_client(\'azure\', container_sas_url)\nasyncio.run(azr_container_client.upload_file(\'small.txt\', \'./small.txt\'))\n\n```\n\n## Installation & Quick Start\nThe latest version of the object-storage package is available on [PyPi](https://pypi.org/project/pilot-platform-object-storage/) and can be installed into another service via Pip.\n\nPip install from PyPi:\n```\npip install pilot-platform-object-storage\n```\n\nIn `pyproject.toml`:\n```\npilot-platform-object-storage = "^<VERSION>"\n```\n\nPip install from a local `.whl` file:\n```\npip install pilot_platform_object_storage-<VERSION>-py3-none-any.whl\n```\n\n## Documentation\n\nAPI Reference and User Guide available at [pilotdataplatform.github.io/object-storage](https://pilotdataplatform.github.io/object-storage/)\n\n## Contribution\n\nYou can contribute the project in following ways:\n\n* Report a bug.\n* Suggest a feature.\n* Open a pull request for fixing issues or adding functionality. Please consider using [pre-commit](https://pre-commit.com) in this case.\n* For general guidelines on how to contribute to the project, please take a look at the [contribution guide](CONTRIBUTING.md).\n',
     'author': 'Indoc Research',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pilot_platform_object_storage-1.4.0/PKG-INFO` & `pilot_platform_object_storage-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilot-platform-object-storage
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python library for interacting with multiple object storage APIs.
 License: Proprietary
 Author: Indoc Research
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

