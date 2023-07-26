# Comparing `tmp/betabageldb-0.1.80.tar.gz` & `tmp/betabageldb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betabageldb-0.1.80.tar", last modified: Wed Jul 19 09:48:57 2023, max compression
+gzip compressed data, was "betabageldb-0.2.0.tar", last modified: Wed Jul 26 14:56:55 2023, max compression
```

## Comparing `betabageldb-0.1.80.tar` & `betabageldb-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:48:57.368163 betabageldb-0.1.80/
--rw-r--r--   0 bidhan     (501) staff       (20)     2838 2023-07-19 09:48:57.367929 betabageldb-0.1.80/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)     2283 2023-07-19 08:55:03.000000 betabageldb-0.1.80/README.md
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:48:57.353137 betabageldb-0.1.80/bagel/
--rw-r--r--   0 bidhan     (501) staff       (20)      625 2023-07-19 08:55:03.000000 betabageldb-0.1.80/bagel/__init__.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:48:57.354515 betabageldb-0.1.80/bagel/api/
--rw-r--r--   0 bidhan     (501) staff       (20)    10695 2023-07-19 08:55:03.000000 betabageldb-0.1.80/bagel/api/__init__.py
--rw-r--r--   0 bidhan     (501) staff       (20)    12159 2023-07-19 08:55:03.000000 betabageldb-0.1.80/bagel/api/fastapi.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:48:57.359588 betabageldb-0.1.80/bagel/api/models/
--rw-r--r--   0 bidhan     (501) staff       (20)    15111 2023-07-19 08:55:03.000000 betabageldb-0.1.80/bagel/api/models/Cluster.py
--rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 09:42:32.000000 betabageldb-0.1.80/bagel/api/models/__init__.py
--rw-r--r--   0 bidhan     (501) staff       (20)    11570 2023-07-19 08:55:03.000000 betabageldb-0.1.80/bagel/api/types.py
--rw-r--r--   0 bidhan     (501) staff       (20)     6274 2023-07-19 08:55:03.000000 betabageldb-0.1.80/bagel/config.py
--rw-r--r--   0 bidhan     (501) staff       (20)      683 2023-07-19 08:55:03.000000 betabageldb-0.1.80/bagel/errors.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:48:57.363868 betabageldb-0.1.80/bagel/utils/
--rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 08:55:03.000000 betabageldb-0.1.80/bagel/utils/__init__.py
--rw-r--r--   0 bidhan     (501) staff       (20)    11810 2023-07-19 08:55:03.000000 betabageldb-0.1.80/bagel/utils/embedding_utils.py
-drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-19 09:48:57.367285 betabageldb-0.1.80/betabageldb.egg-info/
--rw-r--r--   0 bidhan     (501) staff       (20)     2838 2023-07-19 09:48:57.000000 betabageldb-0.1.80/betabageldb.egg-info/PKG-INFO
--rw-r--r--   0 bidhan     (501) staff       (20)      416 2023-07-19 09:48:57.000000 betabageldb-0.1.80/betabageldb.egg-info/SOURCES.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-19 09:48:57.000000 betabageldb-0.1.80/betabageldb.egg-info/dependency_links.txt
--rw-r--r--   0 bidhan     (501) staff       (20)      545 2023-07-19 09:48:57.000000 betabageldb-0.1.80/betabageldb.egg-info/requires.txt
--rw-r--r--   0 bidhan     (501) staff       (20)        6 2023-07-19 09:48:57.000000 betabageldb-0.1.80/betabageldb.egg-info/top_level.txt
--rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-19 09:48:57.368211 betabageldb-0.1.80/setup.cfg
--rw-r--r--   0 bidhan     (501) staff       (20)     1642 2023-07-19 09:48:50.000000 betabageldb-0.1.80/setup.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-26 14:56:55.370983 betabageldb-0.2.0/
+-rw-r--r--   0 bidhan     (501) staff       (20)     3197 2023-07-26 14:56:55.370774 betabageldb-0.2.0/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)     2643 2023-07-26 14:55:22.000000 betabageldb-0.2.0/README.md
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-26 14:56:55.362925 betabageldb-0.2.0/bagel/
+-rw-r--r--   0 bidhan     (501) staff       (20)      625 2023-07-19 08:55:03.000000 betabageldb-0.2.0/bagel/__init__.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-26 14:56:55.365964 betabageldb-0.2.0/bagel/api/
+-rw-r--r--   0 bidhan     (501) staff       (20)    13827 2023-07-24 20:40:18.000000 betabageldb-0.2.0/bagel/api/Cluster.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    10468 2023-07-26 14:53:36.000000 betabageldb-0.2.0/bagel/api/__init__.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    11927 2023-07-26 14:55:22.000000 betabageldb-0.2.0/bagel/api/fastapi.py
+-rw-r--r--   0 bidhan     (501) staff       (20)    11570 2023-07-19 08:55:03.000000 betabageldb-0.2.0/bagel/api/types.py
+-rw-r--r--   0 bidhan     (501) staff       (20)     5926 2023-07-24 20:40:18.000000 betabageldb-0.2.0/bagel/config.py
+-rw-r--r--   0 bidhan     (501) staff       (20)      683 2023-07-19 08:55:03.000000 betabageldb-0.2.0/bagel/errors.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-26 14:56:55.366474 betabageldb-0.2.0/bagel/utils/
+-rw-r--r--   0 bidhan     (501) staff       (20)        0 2023-07-19 08:55:03.000000 betabageldb-0.2.0/bagel/utils/__init__.py
+drwxr-xr-x   0 bidhan     (501) staff       (20)        0 2023-07-26 14:56:55.370018 betabageldb-0.2.0/betabageldb.egg-info/
+-rw-r--r--   0 bidhan     (501) staff       (20)     3197 2023-07-26 14:56:55.000000 betabageldb-0.2.0/betabageldb.egg-info/PKG-INFO
+-rw-r--r--   0 bidhan     (501) staff       (20)      349 2023-07-26 14:56:55.000000 betabageldb-0.2.0/betabageldb.egg-info/SOURCES.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        1 2023-07-26 14:56:55.000000 betabageldb-0.2.0/betabageldb.egg-info/dependency_links.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)      545 2023-07-26 14:56:55.000000 betabageldb-0.2.0/betabageldb.egg-info/requires.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)        6 2023-07-26 14:56:55.000000 betabageldb-0.2.0/betabageldb.egg-info/top_level.txt
+-rw-r--r--   0 bidhan     (501) staff       (20)       38 2023-07-26 14:56:55.371019 betabageldb-0.2.0/setup.cfg
+-rw-r--r--   0 bidhan     (501) staff       (20)     1641 2023-07-26 14:56:10.000000 betabageldb-0.2.0/setup.py
```

### Comparing `betabageldb-0.1.80/PKG-INFO` & `betabageldb-0.2.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.80
+Version: 0.2.0
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -41,19 +41,18 @@
 import uuid
 import bagel
 from bagel.config import Settings
 ```
 
 2. **Define the BagelDB server settings:**
 
-```python 
+```python
 server_settings = Settings(
     bagel_api_impl="rest",
-    bagel_server_host="api2.bageldb.ai",
-    bagel_server_http_port="8000"
+    bagel_server_host="api.bageldb.ai"
 )
 ```
 
 3. **Create the BagelDB client:**
 
 ```python
 client = bagel.Client(server_settings)
@@ -64,15 +63,15 @@
 ```python
 print(client.ping())
 ```
 
 5. **Get the BagelDB server version:**
 
 ```python
-print(client.get_version()) 
+print(client.get_version())
 ```
 
 6. **Create and delete a cluster:**
 
 ```python
 name = str(uuid.uuid4())
 client.create_cluster(name)
@@ -80,41 +79,53 @@
 ```
 
 7. **Create, add documents, and query a cluster:**
 
 ```python
 cluster = client.get_or_create_cluster("testing")
 
-cluster.add(documents=["doc1", "doc2"]) 
+cluster.add(
+    documents=["This is doc", "This is gooogle doc"],
+    metadatas=[{"source": "notion"},
+               {"source": "google-doc"}],
+    ids=[str(uuid.uuid4()), str(uuid.uuid4())],
+)
 
 results = cluster.find(query_texts=["query"], n_results=5)
 ```
 
 8. **Add embeddings and query (without needing to generate embeddings yourself!):**
 
 ```python
-cluster.add(embeddings=[[1.1, 2.3], [4.5, 6.9]])
+cluster = client.get_or_create_cluster("new_testing")
 
-results = cluster.find(query_embeddings=[[1.1, 2.3]], n_results=2) 
+cluster.add(embeddings=[[1.1, 2.3], [4.5, 6.9]],
+            metadatas=[{"info": "M1"}, {"info": "M1"}],
+            documents=["doc1", "doc2"],
+            ids=["id1", "id2"])
+
+results = cluster.find(query_embeddings=[[1.1, 2.3]], n_results=2)
 ```
 
 9. **Modify cluster name:**
 
-```python 
+```python
 cluster.modify(name="new_name")
 ```
 
 10. **Update document metadata:**
 
 ```python
-cluster.update(ids=["doc1"], metadatas=[{"new":"metadata"}])
+cluster.update(ids=["id1"], metadatas=[{"new":"metadata"}])
 ```
 
 11. **Upsert documents:**
 
 ```python
-cluster.upsert(documents=["new doc"], ids=["doc1"])
+cluster.upsert(documents=["new doc"],
+               metadatas=[{"new": "metadata"}],
+               ids=["doc1"])
 ```
 
 Need more dough-tails? See the [example code](example.py) for a more comprehensive guide on using the BagelDB Python client.
 
 Happy coding and enjoy your fresh Bagels! 🥯👩‍💻👨‍💻
```

### Comparing `betabageldb-0.1.80/README.md` & `betabageldb-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -26,19 +26,18 @@
 import uuid
 import bagel
 from bagel.config import Settings
 ```
 
 2. **Define the BagelDB server settings:**
 
-```python 
+```python
 server_settings = Settings(
     bagel_api_impl="rest",
-    bagel_server_host="api2.bageldb.ai",
-    bagel_server_http_port="8000"
+    bagel_server_host="api.bageldb.ai"
 )
 ```
 
 3. **Create the BagelDB client:**
 
 ```python
 client = bagel.Client(server_settings)
@@ -49,15 +48,15 @@
 ```python
 print(client.ping())
 ```
 
 5. **Get the BagelDB server version:**
 
 ```python
-print(client.get_version()) 
+print(client.get_version())
 ```
 
 6. **Create and delete a cluster:**
 
 ```python
 name = str(uuid.uuid4())
 client.create_cluster(name)
@@ -65,41 +64,53 @@
 ```
 
 7. **Create, add documents, and query a cluster:**
 
 ```python
 cluster = client.get_or_create_cluster("testing")
 
-cluster.add(documents=["doc1", "doc2"]) 
+cluster.add(
+    documents=["This is doc", "This is gooogle doc"],
+    metadatas=[{"source": "notion"},
+               {"source": "google-doc"}],
+    ids=[str(uuid.uuid4()), str(uuid.uuid4())],
+)
 
 results = cluster.find(query_texts=["query"], n_results=5)
 ```
 
 8. **Add embeddings and query (without needing to generate embeddings yourself!):**
 
 ```python
-cluster.add(embeddings=[[1.1, 2.3], [4.5, 6.9]])
+cluster = client.get_or_create_cluster("new_testing")
 
-results = cluster.find(query_embeddings=[[1.1, 2.3]], n_results=2) 
+cluster.add(embeddings=[[1.1, 2.3], [4.5, 6.9]],
+            metadatas=[{"info": "M1"}, {"info": "M1"}],
+            documents=["doc1", "doc2"],
+            ids=["id1", "id2"])
+
+results = cluster.find(query_embeddings=[[1.1, 2.3]], n_results=2)
 ```
 
 9. **Modify cluster name:**
 
-```python 
+```python
 cluster.modify(name="new_name")
 ```
 
 10. **Update document metadata:**
 
 ```python
-cluster.update(ids=["doc1"], metadatas=[{"new":"metadata"}])
+cluster.update(ids=["id1"], metadatas=[{"new":"metadata"}])
 ```
 
 11. **Upsert documents:**
 
 ```python
-cluster.upsert(documents=["new doc"], ids=["doc1"])
+cluster.upsert(documents=["new doc"],
+               metadatas=[{"new": "metadata"}],
+               ids=["doc1"])
 ```
 
 Need more dough-tails? See the [example code](example.py) for a more comprehensive guide on using the BagelDB Python client.
 
 Happy coding and enjoy your fresh Bagels! 🥯👩‍💻👨‍💻
```

### Comparing `betabageldb-0.1.80/bagel/__init__.py` & `betabageldb-0.2.0/bagel/__init__.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.80/bagel/api/__init__.py` & `betabageldb-0.2.0/bagel/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from abc import ABC, abstractmethod
 from typing import Sequence, Optional
 import pandas as pd
 from uuid import UUID
-from bagel.api.models.Cluster import Cluster
+from bagel.api.Cluster import Cluster
 from bagel.api.types import (
     ClusterMetadata,
+    Document,
     Documents,
     EmbeddingFunction,
     Embeddings,
     IDs,
     Include,
     Metadatas,
     Where,
     QueryResult,
     GetResult,
     WhereDocument,
+    OneOrMany,
 )
 from bagel.config import Component
-import bagel.utils.embedding_utils as ef
 from overrides import override
 
 
 class API(Component, ABC):
     @abstractmethod
     def ping(self) -> int:
         """Returns the current server time in nanoseconds to check if the server is alive
@@ -49,15 +50,14 @@
         pass
 
     @abstractmethod
     def create_cluster(
         self,
         name: str,
         metadata: Optional[ClusterMetadata] = None,
-        embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
         get_or_create: bool = False,
     ) -> Cluster:
         """Creates a new cluster in the database
 
         Args:
             name  The name of the cluster to create. The name must be unique.
             metadata: A dictionary of metadata to associate with the cluster. Defaults to None.
@@ -83,15 +83,14 @@
         """
 
     @abstractmethod
     def get_or_create_cluster(
         self,
         name: str,
         metadata: Optional[ClusterMetadata] = None,
-        embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Cluster:
         """Calls create_cluster with get_or_create=True.
            If the cluster exists, but with different metadata, the metadata will be replaced.
 
         Args:
             name: The name of the cluster to create. The name must be unique.
             metadata: A dictionary of metadata to associate with the cluster. Defaults to None.
@@ -102,15 +101,14 @@
         """
         pass
 
     @abstractmethod
     def get_cluster(
         self,
         name: str,
-        embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
     ) -> Cluster:
         """Gets a cluster from the database by either name or uuid
 
         Args:
             name: The name of the cluster to get. Defaults to None.
             embedding_function: A function that takes documents and returns an embedding. Should be the same as the one used to create the cluster. Defaults to None.
 
@@ -271,14 +269,15 @@
         self,
         cluster_id: UUID,
         query_embeddings: Embeddings,
         n_results: int = 10,
         where: Where = {},
         where_document: WhereDocument = {},
         include: Include = ["embeddings", "metadatas", "documents", "distances"],
+        query_texts: Optional[OneOrMany[Document]] = None,
     ) -> QueryResult:
         """Gets the nearest neighbors of a single embedding
         ⚠️ This method should not be used directly.
 
         Args:
             embedding: The embedding to find the nearest neighbors of
             n_results: The number of nearest neighbors to return. Defaults to 10.
```

### Comparing `betabageldb-0.1.80/bagel/api/fastapi.py` & `betabageldb-0.2.0/bagel/api/fastapi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 from typing import Optional, cast
 from bagel.api import API
 from bagel.config import System
 from bagel.api.types import (
+    Document,
     Documents,
     Embeddings,
-    EmbeddingFunction,
     IDs,
     Include,
     Metadatas,
     Where,
     WhereDocument,
     GetResult,
     QueryResult,
     ClusterMetadata,
+    OneOrMany,
 )
-import bagel.utils.embedding_utils as emb
 import pandas as pd
 import requests
 import json
 from typing import Sequence
-from bagel.api.models.Cluster import Cluster
+from bagel.api.Cluster import Cluster
 import bagel.errors as errors
 from uuid import UUID
 from overrides import override
 
 
 class FastAPI(API):
     def __init__(self, system: System):
         super().__init__(system)
         url_prefix = "https" if system.settings.bagel_server_ssl_enabled else "http"
         system.settings.require("bagel_server_host")
-        system.settings.require("bagel_server_http_port")
-        self._api_url = f"{url_prefix}://{system.settings.bagel_server_host}:{system.settings.bagel_server_http_port}/api/v1"
+        if system.settings.bagel_server_http_port:
+            self._api_url = f"{url_prefix}://{system.settings.bagel_server_host}:{system.settings.bagel_server_http_port}/api/v1"
+        else:
+            self._api_url = f"{url_prefix}://{system.settings.bagel_server_host}/api/v1"
 
     @override
     def ping(self) -> int:
         """Returns the current server time in nanoseconds to check if the server is alive"""
-        print(f'url {self._api_url}')
         resp = requests.get(self._api_url)
         raise_bagel_error(resp)
         return int(resp.json()["nanosecond heartbeat"])
 
     @override
     def get_all_clusters(self) -> Sequence[Cluster]:
         """Returns a list of all clusters"""
@@ -54,15 +55,14 @@
         return clusters
 
     @override
     def create_cluster(
         self,
         name: str,
         metadata: Optional[ClusterMetadata] = None,
-        embedding_function: Optional[EmbeddingFunction] = emb.DefaultEmbeddingFunction(),
         get_or_create: bool = False,
     ) -> Cluster:
         """Creates a cluster"""
         resp = requests.post(
             self._api_url + "/clusters",
             data=json.dumps(
                 {"name": name, "metadata": metadata, "get_or_create": get_or_create}
@@ -70,47 +70,43 @@
         )
         raise_bagel_error(resp)
         resp_json = resp.json()
         return Cluster(
             client=self,
             id=resp_json["id"],
             name=resp_json["name"],
-            embedding_function=embedding_function,
             metadata=resp_json["metadata"],
         )
 
     @override
     def get_cluster(
         self,
         name: str,
-        embedding_function: Optional[EmbeddingFunction] = emb.DefaultEmbeddingFunction(),
     ) -> Cluster:
         """Returns a cluster"""
         resp = requests.get(self._api_url + "/clusters/" + name)
         raise_bagel_error(resp)
         resp_json = resp.json()
         return Cluster(
             client=self,
             name=resp_json["name"],
             id=resp_json["id"],
-            embedding_function=embedding_function,
             metadata=resp_json["metadata"],
         )
 
     @override
     def get_or_create_cluster(
         self,
         name: str,
         metadata: Optional[ClusterMetadata] = None,
-        embedding_function: Optional[EmbeddingFunction] = emb.DefaultEmbeddingFunction(),
     ) -> Cluster:
         """Get a cluster, or return it if it exists"""
 
         return self.create_cluster(
-            name, metadata, embedding_function, get_or_create=True
+            name, metadata, get_or_create=True
         )
 
     @override
     def _modify(
         self,
         id: UUID,
         new_name: Optional[str] = None,
@@ -208,25 +204,25 @@
         return cast(IDs, resp.json())
 
     @override
     def _add(
         self,
         ids: IDs,
         cluster_id: UUID,
-        embeddings: Embeddings,
+        embeddings: Optional[Embeddings] = None,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
         """
         Adds a batch of embeddings to the database
         - pass in column oriented data lists
         - by default, the index is progressively built up as you add more data. If for ingestion performance reasons you want to disable this, set increment_index to False
         -     and then manually create the index yourself with cluster.create_index()
-        """
+        """ 
         resp = requests.post(
             self._api_url + "/clusters/" + str(cluster_id) + "/add",
             data=json.dumps(
                 {
                     "ids": ids,
                     "embeddings": embeddings,
                     "metadatas": metadatas,
@@ -269,15 +265,15 @@
         return True
 
     @override
     def _upsert(
         self,
         cluster_id: UUID,
         ids: IDs,
-        embeddings: Embeddings,
+        embeddings: Optional[Embeddings] = None,
         metadatas: Optional[Metadatas] = None,
         documents: Optional[Documents] = None,
         increment_index: bool = True,
     ) -> bool:
         """
         Updates a batch of embeddings in the database
         - pass in column oriented data lists
@@ -304,26 +300,27 @@
         self,
         cluster_id: UUID,
         query_embeddings: Embeddings,
         n_results: int = 10,
         where: Optional[Where] = {},
         where_document: Optional[WhereDocument] = {},
         include: Include = ["metadatas", "documents", "distances"],
+        query_texts: Optional[OneOrMany[Document]] = None,
     ) -> QueryResult:
         """Gets the nearest neighbors of a single embedding"""
-
         resp = requests.post(
             self._api_url + "/clusters/" + str(cluster_id) + "/query",
             data=json.dumps(
                 {
                     "query_embeddings": query_embeddings,
                     "n_results": n_results,
                     "where": where,
                     "where_document": where_document,
                     "include": include,
+                    "query_texts": query_texts,
                 }
             ),
         )
 
         raise_bagel_error(resp)
         body = resp.json()
```

### Comparing `betabageldb-0.1.80/bagel/api/models/Cluster.py` & `betabageldb-0.2.0/bagel/api/Cluster.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import TYPE_CHECKING, Optional, Tuple, cast, List
 from pydantic import BaseModel, PrivateAttr
 from uuid import UUID
-import bagel.utils.embedding_utils as ef
 
 from bagel.api.types import (
     ClusterMetadata,
     Embedding,
     Include,
     Metadata,
     Document,
@@ -35,26 +34,23 @@
 
 
 class Cluster(BaseModel):
     name: str
     id: UUID
     metadata: Optional[ClusterMetadata] = None
     _client: "API" = PrivateAttr()
-    _embedding_function: Optional[EmbeddingFunction] = PrivateAttr()
 
     def __init__(
         self,
         client: "API",
         name: str,
         id: UUID,
-        embedding_function: Optional[EmbeddingFunction] = ef.DefaultEmbeddingFunction(),
         metadata: Optional[ClusterMetadata] = None,
     ):
         self._client = client
-        self._embedding_function = embedding_function
         super().__init__(name=name, metadata=metadata, id=id)
 
     def __repr__(self) -> str:
         return f"Cluster(name={self.name})"
 
     def count(self) -> int:
         """The total number of embeddings added to the database
@@ -196,26 +192,15 @@
         n_results = validate_n_results(n_results)
 
         # If neither query_embeddings nor query_texts are provided, or both are provided, raise an error
         if (query_embeddings is None and query_texts is None) or (
             query_embeddings is not None and query_texts is not None
         ):
             raise ValueError(
-                "You must provide either query embeddings or query texts, but not both"
-            )
-
-        # If query_embeddings are not provided, we need to compute them from the query_texts
-        if query_embeddings is None:
-            if self._embedding_function is None:
-                raise ValueError(
-                    "You must provide embeddings or a function to compute them"
-                )
-            # We know query texts is not None at this point, cast for the typechecker
-            query_embeddings = self._embedding_function(
-                cast(List[Document], query_texts)
+                "You must provide either embeddings or texts to find, but not both"
             )
 
         if where is None:
             where = {}
 
         if where_document is None:
             where_document = {}
@@ -223,14 +208,15 @@
         return self._client._query(
             cluster_id=self.id,
             query_embeddings=query_embeddings,
             n_results=n_results,
             where=where,
             where_document=where_document,
             include=include,
+            query_texts=query_texts
         )
 
     def modify(
         self, name: Optional[str] = None, metadata: Optional[ClusterMetadata] = None
     ) -> None:
         """Modify the cluster name or metadata
 
@@ -373,22 +359,8 @@
             raise ValueError(
                 f"Number of metadatas {len(metadatas)} must match number of ids {len(ids)}"
             )
         if documents is not None and len(documents) != len(ids):
             raise ValueError(
                 f"Number of documents {len(documents)} must match number of ids {len(ids)}"
             )
-
-        # If document embeddings are not provided, we need to compute them
-        if embeddings is None and documents is not None:
-            if self._embedding_function is None:
-                raise ValueError(
-                    "You must provide embeddings or a function to compute them"
-                )
-            embeddings = self._embedding_function(documents)
-
-        # if embeddings is None:
-        #     raise ValueError(
-        #         "Something went wrong. Embeddings should be computed at this point"
-        #     )
-
         return ids, embeddings, metadatas, documents  # type: ignore
```

### Comparing `betabageldb-0.1.80/bagel/api/types.py` & `betabageldb-0.2.0/bagel/api/types.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.80/bagel/config.py` & `betabageldb-0.2.0/bagel/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,51 +7,44 @@
 from overrides import EnforceOverrides, override
 from graphlib import TopologicalSorter
 import inspect
 
 # The thin client will have a flag to control which implementations to use
 is_thin_client = False
 try:
-    from bagel.is_thin_client import is_thin_client  # type: ignore
+    from bagel.is_thin_client import is_thin_client
 except ImportError:
     is_thin_client = False
 
 
 logger = logging.getLogger(__name__)
 
 _legacy_config_values = {
     "rest": "bagel.api.fastapi.FastAPI",
 }
 
-# TODO: Don't use concrete types here to avoid circular deps. Strings are fine for right here!
 _abstract_type_keys: Dict[str, str] = {
-    "bagel.db.DB": "bagel_impl",
     "bagel.api.API": "bagel_api_impl",
-    "bagel.telemetry.Telemetry": "bagel_telemetry_impl",
 }
 
 
 class Settings(BaseSettings):
     environment: str = ""
-
-    bagel_impl: str = "bagel.db.duckdb.DuckDB"
     bagel_api_impl: str = "bagel.api.fastapi.FastAPI"
-    bagel_telemetry_impl: str = "bagel.telemetry.posthog.Posthog"
 
     clickhouse_host: Optional[str] = None
     clickhouse_port: Optional[str] = None
 
     persist_directory: str = ".bagel"
 
     bagel_server_host: Optional[str] = None
     bagel_server_http_port: Optional[str] = None
     bagel_server_ssl_enabled: Optional[bool] = False
     bagel_server_grpc_port: Optional[str] = None
-    bagel_server_cors_allow_origins: List[str] = []  # eg ["http://localhost:3000"]
-
+    bagel_server_cors_allow_origins: List[str] = []
     anonymized_telemetry: bool = True
 
     allow_reset: bool = False
 
     sqlite_database: Optional[str] = ":memory:"
     migrations: Literal["none", "validate", "apply"] = "apply"
```

### Comparing `betabageldb-0.1.80/bagel/errors.py` & `betabageldb-0.2.0/bagel/errors.py`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.80/betabageldb.egg-info/PKG-INFO` & `betabageldb-0.2.0/betabageldb.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betabageldb
-Version: 0.1.80
+Version: 0.2.0
 Summary: BagelDB is a Python library for interacting with the BagelDB API.
 Home-page: https://github.com/Bagel-DB/Client
 Author: Bidhan Roy
 Author-email: bidhan@bageldb.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -41,19 +41,18 @@
 import uuid
 import bagel
 from bagel.config import Settings
 ```
 
 2. **Define the BagelDB server settings:**
 
-```python 
+```python
 server_settings = Settings(
     bagel_api_impl="rest",
-    bagel_server_host="api2.bageldb.ai",
-    bagel_server_http_port="8000"
+    bagel_server_host="api.bageldb.ai"
 )
 ```
 
 3. **Create the BagelDB client:**
 
 ```python
 client = bagel.Client(server_settings)
@@ -64,15 +63,15 @@
 ```python
 print(client.ping())
 ```
 
 5. **Get the BagelDB server version:**
 
 ```python
-print(client.get_version()) 
+print(client.get_version())
 ```
 
 6. **Create and delete a cluster:**
 
 ```python
 name = str(uuid.uuid4())
 client.create_cluster(name)
@@ -80,41 +79,53 @@
 ```
 
 7. **Create, add documents, and query a cluster:**
 
 ```python
 cluster = client.get_or_create_cluster("testing")
 
-cluster.add(documents=["doc1", "doc2"]) 
+cluster.add(
+    documents=["This is doc", "This is gooogle doc"],
+    metadatas=[{"source": "notion"},
+               {"source": "google-doc"}],
+    ids=[str(uuid.uuid4()), str(uuid.uuid4())],
+)
 
 results = cluster.find(query_texts=["query"], n_results=5)
 ```
 
 8. **Add embeddings and query (without needing to generate embeddings yourself!):**
 
 ```python
-cluster.add(embeddings=[[1.1, 2.3], [4.5, 6.9]])
+cluster = client.get_or_create_cluster("new_testing")
 
-results = cluster.find(query_embeddings=[[1.1, 2.3]], n_results=2) 
+cluster.add(embeddings=[[1.1, 2.3], [4.5, 6.9]],
+            metadatas=[{"info": "M1"}, {"info": "M1"}],
+            documents=["doc1", "doc2"],
+            ids=["id1", "id2"])
+
+results = cluster.find(query_embeddings=[[1.1, 2.3]], n_results=2)
 ```
 
 9. **Modify cluster name:**
 
-```python 
+```python
 cluster.modify(name="new_name")
 ```
 
 10. **Update document metadata:**
 
 ```python
-cluster.update(ids=["doc1"], metadatas=[{"new":"metadata"}])
+cluster.update(ids=["id1"], metadatas=[{"new":"metadata"}])
 ```
 
 11. **Upsert documents:**
 
 ```python
-cluster.upsert(documents=["new doc"], ids=["doc1"])
+cluster.upsert(documents=["new doc"],
+               metadatas=[{"new": "metadata"}],
+               ids=["doc1"])
 ```
 
 Need more dough-tails? See the [example code](example.py) for a more comprehensive guide on using the BagelDB Python client.
 
 Happy coding and enjoy your fresh Bagels! 🥯👩‍💻👨‍💻
```

### Comparing `betabageldb-0.1.80/betabageldb.egg-info/requires.txt` & `betabageldb-0.2.0/betabageldb.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `betabageldb-0.1.80/setup.py` & `betabageldb-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="betabageldb",
-    version="0.1.80",
+    version="0.2.0",
     description="BagelDB is a Python library for interacting with the BagelDB API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bageldb.ai",
     url="https://github.com/Bagel-DB/Client",
     packages=find_packages(),
```

