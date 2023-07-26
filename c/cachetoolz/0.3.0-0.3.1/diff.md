# Comparing `tmp/cachetoolz-0.3.0.tar.gz` & `tmp/cachetoolz-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetoolz-0.3.0.tar", max compression
+gzip compressed data, was "cachetoolz-0.3.1.tar", max compression
```

## Comparing `cachetoolz-0.3.0.tar` & `cachetoolz-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1077 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/LICENSE
--rw-r--r--   0        0        0    11097 2023-07-19 13:12:21.864253 cachetoolz-0.3.0/README.md
--rw-r--r--   0        0        0      394 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/__init__.py
--rw-r--r--   0        0        0      223 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/abc/__init__.py
--rw-r--r--   0        0        0     2181 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/abc/backend.py
--rw-r--r--   0        0        0      618 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/abc/coder.py
--rw-r--r--   0        0        0      623 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/abc/serializer.py
--rw-r--r--   0        0        0      315 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/backend/__init__.py
--rw-r--r--   0        0        0     4619 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/backend/inmemory.py
--rw-r--r--   0        0        0     7162 2023-07-20 13:38:56.376102 cachetoolz-0.3.0/cachetoolz/backend/mongo.py
--rw-r--r--   0        0        0     4797 2023-07-20 13:38:56.384102 cachetoolz-0.3.0/cachetoolz/backend/redis.py
--rw-r--r--   0        0        0     2151 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/coder/__init__.py
--rw-r--r--   0        0        0     2413 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/coder/decoder.py
--rw-r--r--   0        0        0     3733 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/coder/encoder.py
--rw-r--r--   0        0        0     4259 2023-07-19 13:56:43.867298 cachetoolz-0.3.0/cachetoolz/decorator.py
--rw-r--r--   0        0        0      250 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/exceptions.py
--rw-r--r--   0        0        0      702 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/log.py
--rw-r--r--   0        0        0      633 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/types.py
--rw-r--r--   0        0        0     3194 2023-07-19 13:24:39.070373 cachetoolz-0.3.0/cachetoolz/utils.py
--rw-r--r--   0        0        0     3063 2023-07-20 13:39:21.839935 cachetoolz-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    12638 1970-01-01 00:00:00.000000 cachetoolz-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-19 02:08:29.819918 cachetoolz-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3912 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/README.md
+-rw-r--r--   0        0        0      394 2023-07-26 14:26:03.508728 cachetoolz-0.3.1/cachetoolz/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-19 02:08:29.819918 cachetoolz-0.3.1/cachetoolz/abc/__init__.py
+-rw-r--r--   0        0        0     3068 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/cachetoolz/abc/backend.py
+-rw-r--r--   0        0        0      677 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/cachetoolz/abc/coder.py
+-rw-r--r--   0        0        0      679 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/cachetoolz/abc/serializer.py
+-rw-r--r--   0        0        0      315 2023-07-19 02:08:29.819918 cachetoolz-0.3.1/cachetoolz/backend/__init__.py
+-rw-r--r--   0        0        0     5203 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/cachetoolz/backend/inmemory.py
+-rw-r--r--   0        0        0     7471 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/cachetoolz/backend/mongo.py
+-rw-r--r--   0        0        0     5040 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/cachetoolz/backend/redis.py
+-rw-r--r--   0        0        0     4287 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/cachetoolz/coder/__init__.py
+-rw-r--r--   0        0        0     2424 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/cachetoolz/coder/decoder.py
+-rw-r--r--   0        0        0     3738 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/cachetoolz/coder/encoder.py
+-rw-r--r--   0        0        0     6269 2023-07-26 19:01:15.589273 cachetoolz-0.3.1/cachetoolz/decorator.py
+-rw-r--r--   0        0        0      250 2023-07-19 02:08:29.819918 cachetoolz-0.3.1/cachetoolz/exceptions.py
+-rw-r--r--   0        0        0      702 2023-07-19 02:08:29.819918 cachetoolz-0.3.1/cachetoolz/log.py
+-rw-r--r--   0        0        0      633 2023-07-19 02:08:29.819918 cachetoolz-0.3.1/cachetoolz/types.py
+-rw-r--r--   0        0        0     3194 2023-07-19 13:24:39.070373 cachetoolz-0.3.1/cachetoolz/utils.py
+-rw-r--r--   0        0        0     3290 2023-07-26 19:02:27.125380 cachetoolz-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5455 1970-01-01 00:00:00.000000 cachetoolz-0.3.1/PKG-INFO
```

### Comparing `cachetoolz-0.3.0/LICENSE` & `cachetoolz-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.0/cachetoolz/abc/backend.py` & `cachetoolz-0.3.1/cachetoolz/abc/backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,103 +5,153 @@
 from datetime import timedelta
 from typing import Any, List
 
 from ..log import get_logger
 
 
 class BaseBackend:
-    """Base abstract backend."""
+    """Base abstract backend.
+
+    Attributes
+    ----------
+    logger : logging.Logger
+        Package logger.
+
+    """
 
     def _separate_namespace(self, key: str) -> List[str]:
         """Separete the namespace with key_hash.
 
         Parameters
         ----------
-        key
+        key : str
             Key with namespace and key_hash
 
+        Returns
+        -------
+        ns_key : list[str]
+            Separate namespace from cache identifier key
+
         """
         return key.split(':')
 
     @property
     def logger(self) -> logging.Logger:
-        """Get logger."""
+        """Get logger.
+
+        Returns
+        -------
+        logger : logging.Logger
+            Package logger.
+
+        """
         return get_logger()
 
 
 class BackendABC(BaseBackend, ABC):
-    """Abstract backend."""
+    """Abstract backend.
+
+    Attributes
+    ----------
+    logger : logging.Logger
+        Package logger.
+
+    """
 
     @abstractmethod
     def get(self, key: str) -> Any:
         """Get a value if not expired.
 
         Parameters
         ----------
-        key
-            Cache identifier key
+        key : str
+            Cache identifier key.
 
         Returns
         -------
-            Value cached if exists and not expired else return None
+        with_cache : Any
+            Value cached.
+        without_cache : None
+            If not exists or expired.
 
         """
 
     @abstractmethod
     def set(self, key: str, value: str, expires_at: timedelta) -> None:
-        """Set a value with expires time."""
+        """Set a value with expires time.
+
+        Parameters
+        ----------
+        key : str
+            cache identifier key.
+        value : str
+            value to cache encoded.
+        expires_at : datetime.timedelta
+            expiry time.
+
+        """
 
     @abstractmethod
     def clear(self, namespace: str) -> None:
         """Clear a namespace.
 
         Parameters
         ----------
-        namespaces
+        namespaces : str
             namespace to cache.
 
         """
 
 
 class AsyncBackendABC(BaseBackend, ABC):
-    """Abstract async backend."""
+    """Abstract async backend.
+
+    Attributes
+    ----------
+    logger : logging.Logger
+        Package logger.
+
+    """
 
     @abstractmethod
     async def get(self, key: str) -> Any:
         """Get a value if not expired.
 
         Parameters
         ----------
-        key
-            cache identifier key
+        key : str
+            cache identifier key.
 
         Returns
         -------
-            Value cached if exists and not expired else return None
+        with_cache : Any
+            Value cached.
+        without_cache : None
+            If not exists or expired.
 
         """
 
     @abstractmethod
     async def set(self, key: str, value: str, expires_at: timedelta) -> None:
         """Set a value with expires time.
 
         Parameters
         ----------
-        key
-            cache identifier key
-        value
-            value to cach
-        expires_at
-            expiry time
+        key : str
+            cache identifier key.
+        value : str
+            value to cache encoded.
+        expires_at : datetime.timedelta
+            expiry time.
 
         """
 
     @abstractmethod
     async def clear(self, namespace: str) -> None:
         """Clear a namespace.
 
         Parameters
         ----------
-        namespaces
-            namespace to cache
+        namespaces : str
+            namespace to cache.
 
         """
```

### Comparing `cachetoolz-0.3.0/cachetoolz/abc/coder.py` & `cachetoolz-0.3.1/cachetoolz/abc/serializer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Coder abstract module."""
 
 from abc import ABC, abstractmethod
 from typing import Any
 
 
-class CoderABC(ABC):
+class SerializerABC(ABC):
     """Abstract coder."""
 
     @abstractmethod
     def encode(self, value: Any) -> Any:
         """Encode value.
 
         Parameters
         ----------
-        value
+        value : Any
             Value to encode
 
         Returns
         -------
+        encoded : Any
             Value encoded
 
         """
 
     @abstractmethod
     def decode(self, value: Any) -> Any:
         """Decode value.
 
         Parameters
         ----------
-        value
+        value : Any
             Value to decode
 
         Returns
         -------
+        decoded : Any
             Value decoded
 
         """
```

### Comparing `cachetoolz-0.3.0/cachetoolz/abc/serializer.py` & `cachetoolz-0.3.1/cachetoolz/abc/coder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Coder abstract module."""
 
 from abc import ABC, abstractmethod
 from typing import Any
 
 
-class SerializerABC(ABC):
+class CoderABC(ABC):
     """Abstract coder."""
 
     @abstractmethod
     def encode(self, value: Any) -> Any:
         """Encode value.
 
         Parameters
         ----------
-        value
-            Value to encode
+        value : Any
+            Value to encode.
 
         Returns
         -------
-            Value encoded
+        encode : Any
+            Value encoded.
 
         """
 
     @abstractmethod
     def decode(self, value: Any) -> Any:
         """Decode value.
 
         Parameters
         ----------
-        value
-            Value to decode
+        value : Any
+            Value to decode.
 
         Returns
         -------
-            Value decoded
+        decoded : Any
+            Value decoded.
 
         """
```

### Comparing `cachetoolz-0.3.0/cachetoolz/backend/mongo.py` & `cachetoolz-0.3.1/cachetoolz/backend/mongo.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,35 +4,37 @@
 from datetime import datetime, timedelta
 from typing import Any, Dict
 
 from ..abc import AsyncBackendABC, BackendABC
 
 
 class MongoBackend(BackendABC):
-    """MongoDB cache."""
+    """MongoDB cache.
+
+    This backend is used to store caches mongo synchronous.
+
+    Parameters
+    ----------
+    host : str
+        MongoDB URI.
+    database : str
+        Cache database name.
+    kwargs : dict[str, Any]
+        Takes the same constructor arguments as
+        `pymongo.mongo_client.MongoClient`.
+
+    """
 
     def __init__(
         self,
         host: str = 'localhost',
         database: str = '.cachetoolz',
         **kwargs: Dict[str, Any],
     ):
-        """Initialize the instance.
-
-        Parameters
-        ----------
-        host
-            MongoDB URI
-        database
-            Cache database name
-        kwargs
-            Takes the same constructor arguments as
-            :class:`~pymongo.mongo_client.MongoClient`
-
-        """
+        """Initialize the instance."""
         try:
             from pymongo import MongoClient
         except ImportError as exc:
             raise RuntimeError(
                 "Install cachetoolz with the 'mongo' extra in order "
                 "to use mongo backend."
             ) from exc
@@ -59,20 +61,23 @@
                 yield client[self._database]
 
     def get(self, key: str) -> Any:
         """Get a value if not expired.
 
         Parameters
         ----------
-        key
-            cache identifier key
+        key : str
+            cache identifier key.
 
         Returns
         -------
-            Value cached if exists and not expired else return None
+        with_cache : Any
+            Value cached.
+        without_cache : None
+            If not exists or expired.
 
         """
         self.logger.debug("Get 'key=%s'", key)
 
         namespace, key_hash = self._separate_namespace(key)
 
         with self._get_database_or_collection(namespace) as collection:
@@ -84,20 +89,20 @@
         self.logger.debug("No cache to 'key=%s'", key)
 
     def set(self, key: str, value: str, expires_at: timedelta) -> None:
         """Set a value with expires time.
 
         Parameters
         ----------
-        key
-            cache identifier key
-        value
-            value to cach
-        expires_at
-            expiry time
+        key : str
+            cache identifier key.
+        value : str
+            value to cache encoded.
+        expires_at : datetime.timedelta
+            expiry time.
 
         """
         self.logger.debug(
             "Set 'key=%s', 'value=%s', 'expires_at=%s'",
             key,
             value,
             expires_at,
@@ -121,46 +126,48 @@
             )
 
     def clear(self, namespace: str) -> None:
         """Clear a namespace.
 
         Parameters
         ----------
-        namespaces
-            namespace to cache
+        namespaces : str
+            namespace to cache.
 
         """
         self.logger.debug("Clear 'namespace=%s'", namespace)
 
         with self._get_database_or_collection() as database:
             database.drop_collection(namespace)
 
 
 class AsyncMongoBackend(AsyncBackendABC):
-    """Async MongoDB cache."""
+    """Async MongoDB cache.
+
+    This backend is used to store caches mongo asynchronous.
+
+    Parameters
+    ----------
+    host : str
+        MongoDB URI.
+    database : str
+        Cache database name.
+    kwargs : dict[str, Any]
+        Takes the same constructor arguments as
+        `pymongo.mongo_client.MongoClient`.
+
+    """
 
     def __init__(
         self,
         host: str = 'localhost',
         database: str = '.cachetoolz',
         **kwargs: Dict[str, Any],
     ):
-        """Initialize the instance.
-
-        Parameters
-        ----------
-        host
-            MongoDB URI
-        database
-            Cache database name
-        kwargs
-            Takes the same constructor arguments as
-            :class:`~pymongo.mongo_client.MongoClient`
-
-        """
+        """Initialize the instance."""
         try:
             from motor.motor_asyncio import AsyncIOMotorClient
         except ImportError as exc:
             raise RuntimeError(
                 "Install cachetoolz with the 'mongo' extra in order "
                 "to use mongo backend."
             ) from exc
@@ -189,20 +196,23 @@
             client.close()
 
     async def get(self, key: str) -> Any:
         """Get a value if not expired.
 
         Parameters
         ----------
-        key
-            cache identifier key
+        key : str
+            cache identifier key.
 
         Returns
         -------
-            Value cached if exists and not expired else return None
+        with_cache : Any
+            Value cached.
+        without_cache : None
+            If not exists or expired.
 
         """
         self.logger.debug("Get 'key=%s'", key)
 
         namespace, key_hash = self._separate_namespace(key)
 
         with self._get_database_or_collection(namespace) as collection:
@@ -214,20 +224,20 @@
         self.logger.debug("No cache to 'key=%s'", key)
 
     async def set(self, key: str, value: str, expires_at: timedelta) -> None:
         """Set a value with expires time.
 
         Parameters
         ----------
-        key
-            cache identifier key
-        value
-            value to cach
-        expires_at
-            expiry time
+        key : str
+            cache identifier key.
+        value : str
+            value to cache encoded.
+        expires_at : datetime.timedelta
+            expiry time.
 
         """
         self.logger.debug(
             "Set 'key=%s', 'value=%s', 'expires_at=%s'",
             key,
             value,
             expires_at,
@@ -251,15 +261,15 @@
             )
 
     async def clear(self, namespace: str) -> None:
         """Clear a namespace.
 
         Parameters
         ----------
-        namespaces
-            namespace to cache
+        namespaces : str
+            namespace to cache.
 
         """
         self.logger.debug("Clear 'namespace=%s'", namespace)
 
         with self._get_database_or_collection() as database:
             await database.drop_collection(namespace)
```

### Comparing `cachetoolz-0.3.0/cachetoolz/backend/redis.py` & `cachetoolz-0.3.1/cachetoolz/backend/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,30 @@
 from datetime import timedelta
 from typing import Any, Dict
 
 from ..abc import AsyncBackendABC, BackendABC
 
 
 class RedisBackend(BackendABC):
-    """Redis cache."""
-
-    def __init__(self, url: str, **kwargs: Dict[str, Any]):
-        """Initialize the instance.
+    """Redis cache.
 
+    Parameters
+    ----------
+    url : str
+        Redis url.
+    kwargs : dict[str, Any]
+        Takes the same constructor arguments as
+        `redis.client.Redis.from_url`.
         The ``decode_responses`` parameter will always be True
         as the result needs to be returned as a string.
 
-        Parameters
-        ----------
-        url
-            Redis url
-        kwargs
-            Takes the same constructor arguments as
-            :method:`~redis.client.Redis.from_url`
+    """
 
-        """
+    def __init__(self, url: str, **kwargs: Dict[str, Any]):
+        """Initialize the instance."""
         try:
             from redis import Redis
         except ImportError as exc:
             raise RuntimeError(
                 "Install cachetoolz with the 'redis' extra in order "
                 "to use redis backend."
             ) from exc
@@ -41,40 +40,43 @@
         return f'{self.__class__.__name__}(url="{self._url}")'
 
     def get(self, key: str) -> Any:
         """Get a value if not expired.
 
         Parameters
         ----------
-        key
+        key : str
             cache identifier key.
 
         Returns
         -------
-            Value cached if exists and not expired else return None
+        with_cache : Any
+            Value cached.
+        without_cache : None
+            If not exists or expired.
 
         """
         self.logger.debug("Get 'key=%s'", key)
 
         if result := self._backend.get(key):
             return result
 
         self.logger.debug("No cache to 'key=%s'", key)
 
     def set(self, key: str, value: str, expires_at: timedelta) -> None:
         """Set a value with expires time.
 
         Parameters
         ----------
-        key
-            cache identifier key
-        value
-            value to cach
-        expires_at
-            expiry time
+        key : str
+            cache identifier key.
+        value : str
+            value to cache encoded.
+        expires_at : datetime.timedelta
+            expiry time.
 
         """
         self.logger.debug(
             "Set 'key=%s', 'value=%s', 'expires_at=%s'",
             key,
             value,
             expires_at,
@@ -83,42 +85,43 @@
         self._backend.set(key, str(value), ex=expires_at)
 
     def clear(self, namespace: str) -> None:
         """Clear a namespace.
 
         Parameters
         ----------
-        namespaces
+        namespaces : str
             namespace to cache.
 
         """
         self.logger.debug("Clear 'namespace=%s'", namespace)
 
         for key in self._backend.scan_iter(f'{namespace}:*'):
             self._backend.delete(key)
 
 
 class AsyncRedisBackend(AsyncBackendABC):
-    """Async Redis backend."""
+    """Async Redis backend.
 
-    def __init__(self, url: str, **kwargs):
-        """Initialize the instance.
+    This backend is used to store caches redis asynchronous.
 
+    Parameters
+    ----------
+    url : str
+        Redis url.
+    kwargs : dict[str, Any]
+        Takes the same constructor arguments as
+        `redis.asyncio. client.Redis.from_url`.
         The ``decode_responses`` parameter will always be True
         as the result needs to be returned as a string.
 
-        Parameters
-        ----------
-        url
-            Redis url
-        kwargs
-            Takes the same constructor arguments as
-            :method:`~redis.asyncio. client.Redis.from_url`
+    """
 
-        """
+    def __init__(self, url: str, **kwargs):
+        """Initialize the instance."""
         try:
             from redis.asyncio import Redis
         except ImportError as exc:
             raise RuntimeError(
                 "Install cachetoolz with the 'redis' extra in order "
                 "to use redis backend."
             ) from exc
@@ -132,40 +135,43 @@
         return f'{self.__class__.__name__}(url="{self._url}")'
 
     async def get(self, key: str) -> Any:
         """Get a value if not expired.
 
         Parameters
         -----------
-        key
-            cache identifier key
+        key : str
+            cache identifier key.
 
         Returns
         -------
-            Value cached if exists and not expired else return None
+        with_cache : Any
+            Value cached.
+        without_cache : None
+            If not exists or expired.
 
         """
         self.logger.debug("Get 'key=%s'", key)
 
         if result := await self._backend.get(key):
             return result
 
         self.logger.debug("No cache to 'key=%s'", key)
 
     async def set(self, key: str, value: str, expires_at: timedelta) -> None:
         """Set a value with expires time.
 
         Parameters
         ----------
-        key
-            cache identifier key
-        value
-            value to cach
-        expires_at
-            expiry time
+        key : str
+            cache identifier key.
+        value : str
+            value to cache encoded.
+        expires_at : datetime.timedelta
+            expiry time.
 
         """
         self.logger.debug(
             "Set 'key=%s', 'value=%s', 'expires_at=%s'",
             key,
             value,
             expires_at,
@@ -174,15 +180,15 @@
         await self._backend.set(key, str(value), ex=expires_at)
 
     async def clear(self, namespace: str) -> None:
         """Clear a namespace.
 
         Parameters
         ----------
-        namespaces
+        namespaces : str
             namespace to cache.
 
         """
         self.logger.debug("Clear 'namespace=%s'", namespace)
 
         async for key in self._backend.scan_iter(f'{namespace}:*'):
             await self._backend.delete(key)
```

### Comparing `cachetoolz-0.3.0/cachetoolz/coder/decoder.py` & `cachetoolz-0.3.1/cachetoolz/coder/decoder.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from uuid import UUID
 
 from .. import types
 from ..exceptions import RegistryError, UnknownDecoderError
 
 
 class Decoder(JSONDecoder):
-    """Decoder class."""
+    """JSON decoder class."""
 
     DECODERS: ClassVar[Dict[str, types.Decoder]] = {
         'time': time.fromisoformat,
         'date': date.fromisoformat,
         'datetime': datetime.fromisoformat,
         'timedelta': lambda val: timedelta(seconds=val),
         'decimal': Decimal,
@@ -64,15 +64,15 @@
 
 
 def register(name: str) -> types.Decorator:
     """Register a decoder.
 
     Parameters
     ----------
-    name
+    name : str
         Decoder name.
 
     Examples
     --------
     >>> from collections import deque
     >>> from typing import Any
     >>> @register('deque')
```

### Comparing `cachetoolz-0.3.0/cachetoolz/coder/encoder.py` & `cachetoolz-0.3.1/cachetoolz/coder/encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from .. import types
 from ..exceptions import RegistryError, UnknownEncoderError
 from ..utils import decoder_name
 
 
 class Encoder(JSONEncoder):
-    """Encoder class."""
+    """JSON encoder class."""
 
     def default(self, o):
         """Turns a python object into a json object.
 
         Parameters
         ----------
         o
```

### Comparing `cachetoolz-0.3.0/cachetoolz/log.py` & `cachetoolz-0.3.1/cachetoolz/log.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.0/cachetoolz/types.py` & `cachetoolz-0.3.1/cachetoolz/types.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.0/cachetoolz/utils.py` & `cachetoolz-0.3.1/cachetoolz/utils.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.3.0/pyproject.toml` & `cachetoolz-0.3.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cachetoolz"
-version = "0.3.0"
+version = "0.3.1"
 description = "This library provides a decorator for caching functions"
 license = "MIT"
 authors = ["Igor Taconi <igor.taconi@protonmail.com>"]
 maintainers = ["Igor Taconi <igor.taconi@protonmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/taconi/cachetoolz/#readme"
 repository = "https://github.com/taconi/cachetoolz/"
@@ -25,15 +25,15 @@
     "Operating System :: OS Independent",
     "Topic :: Utilities",
 ]
 include = ["cachetoolz"]
 exclude = ["reports", "docs", "examples", "tests"]
 
 [tool.poetry.urls]
-"Bug Tracker" = "https://github.com/taconi/cachetoolz/issues"
+"Issue Tracker" = "https://github.com/taconi/cachetoolz/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 funcy = "^2.0"
 nest-asyncio = "^1.5.6"
 charset-normalizer = "^3.2.0"
 redis = {version = "^4.6.0", optional = true}
@@ -42,14 +42,18 @@
 typing-extensions = "^4.7.1"
 get-annotations = "^0.1.2"
 
 [tool.poetry.extras]
 redis = ["redis"]
 mongo = ["motor", "pymongo"]
 
+[tool.poetry.group.ci.dependencies]
+nox = "^2023.4.22"
+nox-poetry = "^1.0.3"
+
 [tool.poetry.group.test.dependencies]
 ward = "^0.67.2b0"
 coverage = {extras = ["toml"], version = "^7.2.7"}
 faker = "^19.1.0"
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.13"
@@ -59,27 +63,32 @@
 flake8-html = "^0.4.3"
 flake8-docstrings = "^1.7.0"
 flake8-bugbear = "^23.6.5"
 flake8-pyproject = "^1.2.3"
 black = "^23.3.0"
 autoflake = "^2.2.0"
 docformatter = {extras = ["tomli"], version = "^1.7.3"}
+pre-commit = "^3.3.3"
+gitlint = "^0.19.1"
 
+[tool.poetry.group.docs.dependencies]
+mkdocs-material = "^9.1.19"
+mkdocstrings-python = "^1.2.1"
 
 [tool.isort]
 multi_line_output = 3
 line_length = 79
 include_trailing_comma = true
 
 [tool.black]
 line_length = 79
 skip-string-normalization = true
 
 [tool.flake8]
-ignore = ["E121", "E123", "E126", "E226", "E24", "E704", "W503", "W504", "D401"]
+ignore = ["E121", "E123", "E126", "E226", "E24", "E704", "W503", "W504", "D401", "D412"]
 max-line-length = 79
 max-complexity = 8
 docstring-convention = "pep257"
 format = "html"
 htmltitle = "Flake8 Report"
 htmldir = "reports/flake8"
```

