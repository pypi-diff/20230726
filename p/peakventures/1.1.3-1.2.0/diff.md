# Comparing `tmp/peakventures-1.1.3.tar.gz` & `tmp/peakventures-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakventures-1.1.3.tar", max compression
+gzip compressed data, was "peakventures-1.2.0.tar", max compression
```

## Comparing `peakventures-1.1.3.tar` & `peakventures-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.1.3/peakventures/__init__.py
--rw-r--r--   0        0        0     1813 2023-07-12 17:49:47.662944 peakventures-1.1.3/peakventures/api.py
--rw-r--r--   0        0        0     1153 2023-05-26 10:31:37.185812 peakventures-1.1.3/peakventures/credentials.py
--rw-r--r--   0        0        0     1336 2023-05-26 10:32:19.525020 peakventures-1.1.3/peakventures/storage.py
--rw-r--r--   0        0        0      376 2023-07-12 17:50:29.928161 peakventures-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 peakventures-1.1.3/setup.py
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 peakventures-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.2.0/peakventures/__init__.py
+-rw-r--r--   0        0        0     1813 2023-07-12 17:49:47.662944 peakventures-1.2.0/peakventures/api.py
+-rw-r--r--   0        0        0     3516 2023-07-26 09:31:16.618364 peakventures-1.2.0/peakventures/conversions.py
+-rw-r--r--   0        0        0     1095 2023-07-26 09:29:28.910842 peakventures-1.2.0/peakventures/credentials.py
+-rw-r--r--   0        0        0      830 2023-07-26 09:28:36.228718 peakventures-1.2.0/peakventures/storage.py
+-rw-r--r--   0        0        0      366 2023-07-26 09:30:18.751333 peakventures-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 peakventures-1.2.0/setup.py
+-rw-r--r--   0        0        0      580 1970-01-01 00:00:00.000000 peakventures-1.2.0/PKG-INFO
```

### Comparing `peakventures-1.1.3/peakventures/api.py` & `peakventures-1.2.0/peakventures/api.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.1.3/peakventures/credentials.py` & `peakventures-1.2.0/peakventures/credentials.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import json
 import os
 from typing import Any
 
 S3_CREDENTIALS_NAME = "db-s3"
-AZURE_CREDENTIALS_NAME = "db-azure-storage"
 API_CREDENTIALS_NAME = "db-api"
 
 
 def _get_dbutils() -> Any:
     from pyspark.sql import SparkSession
     from pyspark.dbutils import DBUtils
     return DBUtils(SparkSession.getActiveSession())
 
 
 def _get_credential(name: str) -> str:
     if os.getenv("DEVELOPMENT"):
         result = {
             S3_CREDENTIALS_NAME: os.getenv("S3_CREDENTIALS"),
-            AZURE_CREDENTIALS_NAME: os.getenv("AZURE_CREDENTIALS"),
             API_CREDENTIALS_NAME: os.getenv("API_CREDENTIALS")
         }.get(name)
     else:
         dbutils = _get_dbutils()
         result = dbutils.secrets.get("credentials", name)
 
     if not result:
@@ -39,8 +37,10 @@
     """Get credentials from the remote storage."""
     return json.loads(get_credentials(name))
 
 
 __all__ = [
     "get_credentials",
     "get_credentials_json",
+    "S3_CREDENTIALS_NAME",
+    "API_CREDENTIALS_NAME"
 ]
```

### Comparing `peakventures-1.1.3/peakventures/storage.py` & `peakventures-1.2.0/peakventures/storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,18 @@
 import json
 from io import BytesIO
 from typing import Any
 
 import boto3
-from azure.storage.blob import BlobClient, BlobServiceClient
 
-from peakventures.credentials import get_credentials, get_credentials_json, AZURE_CREDENTIALS_NAME, S3_CREDENTIALS_NAME
+from peakventures.credentials import get_credentials_json, S3_CREDENTIALS_NAME
 
 CONTAINER_NAME = "models"
 
 
-def _store_model_azure(name: str, payload: str) -> None:
-    connection_string = get_credentials(AZURE_CREDENTIALS_NAME)
-
-    blob_client: BlobClient = (
-        BlobServiceClient.from_connection_string(connection_string)
-        .get_container_client(CONTAINER_NAME)
-        .get_blob_client(name)
-    )
-
-    blob_client.upload_blob(payload, overwrite=True)
-
-
 def _store_model_s3(name: str, payload: str) -> None:
     credentials = get_credentials_json(S3_CREDENTIALS_NAME)
 
     s3 = boto3.client(
         "s3",
         endpoint_url=credentials["endpoint_url"],
         aws_access_key_id=credentials["access_key_id"],
@@ -36,14 +23,13 @@
         s3.upload_fileobj(buffer, CONTAINER_NAME, name)
 
 
 def store_model(name: str, payload: Any) -> None:
     """Store model on the remote storage."""
     json_payload = json.dumps(payload)
 
-    _store_model_azure(name, json_payload)
     _store_model_s3(name, json_payload)
 
 
 __all__ = [
     "store_model"
 ]
```

### Comparing `peakventures-1.1.3/setup.py` & `peakventures-1.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['peakventures']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['azure-storage-blob>=12.16.0,<13.0.0',
- 'boto3>=1.26.141,<2.0.0',
- 'tenacity>=8.2.2,<9.0.0']
+['boto3>=1.28.11,<2.0.0',
+ 'tenacity>=8.2.2,<9.0.0',
+ 'websockets>=11.0.3,<12.0.0']
 
 setup_kwargs = {
     'name': 'peakventures',
-    'version': '1.1.3',
+    'version': '1.2.0',
     'description': 'PeakVentures Python Utilities for DataBricks',
     'long_description': 'None',
     'author': 'Volodymyr Smirnov',
     'author_email': 'volodymyr@peakventures.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

