# Comparing `tmp/aiormq-6.7.6.tar.gz` & `tmp/aiormq-6.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiormq-6.7.6.tar", max compression
+gzip compressed data, was "aiormq-6.7.7.tar", max compression
```

## Comparing `aiormq-6.7.6.tar` & `aiormq-6.7.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    17426 2023-02-18 21:26:40.811315 aiormq-6.7.6/README.rst
--rw-r--r--   0        0        0     1714 2022-12-15 11:27:13.176542 aiormq-6.7.6/aiormq/__init__.py
--rw-r--r--   0        0        0    17329 2023-05-11 09:07:24.799939 aiormq-6.7.6/aiormq/abc.py
--rw-r--r--   0        0        0      862 2022-12-12 22:30:18.703315 aiormq-6.7.6/aiormq/auth.py
--rw-r--r--   0        0        0     4800 2023-05-11 09:07:24.801438 aiormq-6.7.6/aiormq/base.py
--rw-r--r--   0        0        0    29505 2023-05-11 09:16:46.730769 aiormq-6.7.6/aiormq/channel.py
--rw-r--r--   0        0        0    29929 2023-05-12 13:43:04.496203 aiormq-6.7.6/aiormq/connection.py
--rw-r--r--   0        0        0     5831 2023-05-11 09:07:24.803621 aiormq-6.7.6/aiormq/exceptions.py
--rw-r--r--   0        0        0        0 2022-12-12 22:30:18.707721 aiormq-6.7.6/aiormq/py.typed
--rw-r--r--   0        0        0     3284 2023-05-11 09:07:24.804856 aiormq-6.7.6/aiormq/tools.py
--rw-r--r--   0        0        0      231 2023-05-11 09:07:24.805425 aiormq-6.7.6/aiormq/types.py
--rw-r--r--   0        0        0     2449 2023-05-12 13:43:13.645587 aiormq-6.7.6/pyproject.toml
--rw-r--r--   0        0        0    19407 1970-01-01 00:00:00.000000 aiormq-6.7.6/PKG-INFO
+-rw-r--r--   0        0        0    17426 2023-02-18 21:26:40.811315 aiormq-6.7.7/README.rst
+-rw-r--r--   0        0        0     1714 2022-12-15 11:27:13.176542 aiormq-6.7.7/aiormq/__init__.py
+-rw-r--r--   0        0        0    17329 2023-05-11 09:07:24.799939 aiormq-6.7.7/aiormq/abc.py
+-rw-r--r--   0        0        0      862 2022-12-12 22:30:18.703315 aiormq-6.7.7/aiormq/auth.py
+-rw-r--r--   0        0        0     4800 2023-05-11 09:07:24.801438 aiormq-6.7.7/aiormq/base.py
+-rw-r--r--   0        0        0    29505 2023-05-11 09:16:46.730769 aiormq-6.7.7/aiormq/channel.py
+-rw-r--r--   0        0        0    30139 2023-07-26 10:43:29.229674 aiormq-6.7.7/aiormq/connection.py
+-rw-r--r--   0        0        0     5831 2023-05-11 09:07:24.803621 aiormq-6.7.7/aiormq/exceptions.py
+-rw-r--r--   0        0        0        0 2022-12-12 22:30:18.707721 aiormq-6.7.7/aiormq/py.typed
+-rw-r--r--   0        0        0     3284 2023-05-11 09:07:24.804856 aiormq-6.7.7/aiormq/tools.py
+-rw-r--r--   0        0        0      231 2023-05-11 09:07:24.805425 aiormq-6.7.7/aiormq/types.py
+-rw-r--r--   0        0        0     2449 2023-07-26 10:43:24.287705 aiormq-6.7.7/pyproject.toml
+-rw-r--r--   0        0        0    19107 1970-01-01 00:00:00.000000 aiormq-6.7.7/PKG-INFO
```

### Comparing `aiormq-6.7.6/README.rst` & `aiormq-6.7.7/README.rst`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.6/aiormq/__init__.py` & `aiormq-6.7.7/aiormq/__init__.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.6/aiormq/abc.py` & `aiormq-6.7.7/aiormq/abc.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.6/aiormq/auth.py` & `aiormq-6.7.7/aiormq/auth.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.6/aiormq/base.py` & `aiormq-6.7.7/aiormq/base.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.6/aiormq/channel.py` & `aiormq-6.7.7/aiormq/channel.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.6/aiormq/connection.py` & `aiormq-6.7.7/aiormq/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,16 @@
     # Allow three missed heartbeats (based on heartbeat(timeout)
     HEARTBEAT_GRACE_MULTIPLIER = 3
 
     READER_CLOSE_TIMEOUT = 2
 
     _reader_task: TaskType
     _writer_task: TaskType
+    __create_connection_kwargs: Mapping[str, Any]
+
     write_queue: asyncio.Queue
     server_properties: ArgumentsType
     connection_tune: spec.Connection.Tune
     channels: Dict[int, Optional[AbstractChannel]]
 
     @staticmethod
     def _parse_ca_data(data: Optional[str]) -> Optional[bytes]:
@@ -268,14 +270,15 @@
 
     def __init__(
         self,
         url: URLorStr,
         *,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         context: Optional[ssl.SSLContext] = None,
+        **create_connection_kwargs: Any,
     ):
 
         super().__init__(loop=loop or asyncio.get_event_loop(), parent=None)
 
         self.url = URL(url)
         if self.url.is_absolute() and not self.url.port:
             self.url = self.url.with_port(DEFAULT_PORTS[self.url.scheme])
@@ -318,14 +321,15 @@
         self.__update_secret_lock: asyncio.Lock = asyncio.Lock()
         self.__update_secret_future: Optional[asyncio.Future] = None
         self.__connection_unblocked: asyncio.Event = asyncio.Event()
         self.__heartbeat_grace_timeout = (
             (self.heartbeat_timeout + 1) * self.HEARTBEAT_GRACE_MULTIPLIER
         )
         self.__last_frame_time: float = self.loop.time()
+        self.__create_connection_kwargs = create_connection_kwargs
 
     async def ready(self) -> None:
         await self.connected.wait()
         await self.__connection_unblocked.wait()
 
     def set_close_reason(
         self, reply_code: int = REPLY_SUCCESS,
@@ -446,14 +450,15 @@
             )
             self.ssl_context = ssl_context
 
         log.debug("Connecting to: %s", self)
         try:
             reader, writer = await asyncio.open_connection(
                 self.url.host, self.url.port, ssl=ssl_context,
+                **self.__create_connection_kwargs,
             )
 
             frame_receiver = FrameReceiver(reader)
         except OSError as e:
             raise AMQPConnectionError(*e.args) from e
 
         frame: Optional[FrameTypes]
```

### Comparing `aiormq-6.7.6/aiormq/exceptions.py` & `aiormq-6.7.7/aiormq/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.6/aiormq/tools.py` & `aiormq-6.7.7/aiormq/tools.py`

 * *Files identical despite different names*

### Comparing `aiormq-6.7.6/pyproject.toml` & `aiormq-6.7.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiormq"
-version = "6.7.6"
+version = "6.7.7"
 description = "Pure python AMQP asynchronous client library"
 authors = ["Dmitry Orlov <me@mosquito.su>"]
 readme = "README.rst"
 license = "Apache-2.0"
 keywords=["rabbitmq", "asyncio", "amqp", "amqp 0.9.1", "driver", "pamqp"]
 homepage = "https://github.com/mosquito/aiormq"
 classifiers = [
```

### Comparing `aiormq-6.7.6/PKG-INFO` & `aiormq-6.7.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiormq
-Version: 6.7.6
+Version: 6.7.7
 Summary: Pure python AMQP asynchronous client library
 Home-page: https://github.com/mosquito/aiormq
 License: Apache-2.0
 Keywords: rabbitmq,asyncio,amqp,amqp 0.9.1,driver,pamqp
 Author: Dmitry Orlov
 Author-email: me@mosquito.su
 Requires-Python: >=3.7,<4.0
@@ -18,21 +18,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Clustering
 Requires-Dist: pamqp (==3.2.1)
```

