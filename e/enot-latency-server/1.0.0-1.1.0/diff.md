# Comparing `tmp/enot_latency_server-1.0.0-py3-none-any.whl.zip` & `tmp/enot_latency_server-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 12063 bytes, number of entries: 8
--rw-r--r--  2.0 unx      142 b- defN 23-May-12 10:34 enot_latency_server/__init__.py
--rw-r--r--  2.0 unx     2223 b- defN 23-May-12 10:34 enot_latency_server/client.py
--rw-r--r--  2.0 unx     2489 b- defN 23-May-12 10:34 enot_latency_server/server.py
--rw-rw-rw-  2.0 unx    11338 b- defN 23-May-17 15:12 enot_latency_server-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    13637 b- defN 23-May-17 15:12 enot_latency_server-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 15:12 enot_latency_server-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-May-17 15:12 enot_latency_server-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      707 b- defN 23-May-17 15:12 enot_latency_server-1.0.0.dist-info/RECORD
-8 files, 30648 bytes uncompressed, 10817 bytes compressed:  64.7%
+Zip file size: 12253 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      142 b- defN 23-Jul-26 14:18 enot_latency_server/__init__.py
+-rw-r--r--  2.0 unx     2417 b- defN 23-Jul-26 14:18 enot_latency_server/client.py
+-rw-r--r--  2.0 unx     2680 b- defN 23-Jul-26 14:18 enot_latency_server/server.py
+-rw-rw-rw-  2.0 unx    11338 b- defN 23-Jul-26 14:26 enot_latency_server-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13637 b- defN 23-Jul-26 14:26 enot_latency_server-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-26 14:26 enot_latency_server-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-26 14:26 enot_latency_server-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      707 b- defN 23-Jul-26 14:26 enot_latency_server-1.1.0.dist-info/RECORD
+8 files, 31033 bytes uncompressed, 11007 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: enot_latency_server/client.py
 Comment: 
 
 Filename: enot_latency_server/server.py
 Comment: 
 
-Filename: enot_latency_server-1.0.0.dist-info/LICENSE
+Filename: enot_latency_server-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: enot_latency_server-1.0.0.dist-info/METADATA
+Filename: enot_latency_server-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: enot_latency_server-1.0.0.dist-info/WHEEL
+Filename: enot_latency_server-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: enot_latency_server-1.0.0.dist-info/top_level.txt
+Filename: enot_latency_server-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: enot_latency_server-1.0.0.dist-info/RECORD
+Filename: enot_latency_server-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## enot_latency_server/client.py

```diff
@@ -1,9 +1,10 @@
 """Client implementation, use it to send model to latency measurement server."""
 import logging
+import pickle
 import time
 from typing import Dict
 from typing import Optional
 
 import requests
 from requests.exceptions import RequestException
 
@@ -20,14 +21,15 @@
 
 def measure_latency_remote(
     model: bytes,
     host: str = _DEFAULT_HOST,
     port: int = _DEFAULT_PORT,
     endpoint: str = _DEFAULT_ENDPOINT,
     timeout: Optional[float] = None,
+    **kwargs,
 ) -> Dict[str, float]:
     """
     Send model to remote measurement server and return latency in ms.
 
     Parameters
     ----------
     model : bytes
@@ -37,33 +39,35 @@
     port : int
         Port of measurement service.
     endpoint : str
         Endpoint of measurement service, default value is 'measurement_latency'.
     timeout : Optional[float]
         A number indicating how many seconds to wait for a client to make a connection or send a response.
         The default value of None means that the request will wait indefinitely.
+    kwargs : Dict
+        Keyword arguments to be passed to measure_latency on the server side.
 
     Returns
     -------
     Dict[str, float]
         Latency in milliseconds and anything else (optional).
 
     """
     for trial_timeout in _TRIAL_TIMEOUTS:
         try:
             response = requests.post(
                 url=f'http://{host}:{port}/{endpoint}',
-                data=model,
+                data=pickle.dumps({**{'model': model}, **kwargs}),
                 headers={'Content-Type': 'application/octet-stream'},
                 timeout=timeout,
             )
             if response.status_code == 200:
                 return response.json()
 
-            logger.warning(f'Expected status code is 200, got {response.status_code}')
+            raise RuntimeError(f'Expected status code is 200, got {response.status_code}; reason: {response.reason}')
         except RequestException as exc:
             logger.warning(f'An exception occured during latency measurement: {exc}')
 
         logger.warning(f'Next try will be in {trial_timeout}s')
         time.sleep(trial_timeout)
 
     raise RuntimeError('All attempts failed, latency cannot be measured, please check server log')
```

## enot_latency_server/server.py

```diff
@@ -1,8 +1,9 @@
 """Extendable latency measurement server."""
+import pickle
 from abc import ABC
 from abc import abstractmethod
 from typing import Dict
 
 from aiohttp import web
 
 _DEFAULT_HOST: str = '0.0.0.0'
@@ -45,36 +46,39 @@
 
         self._app = web.Application(client_max_size=self.__CLIENT_MAX_SIZE)
 
     def run(self) -> None:
         """Start latency measurement server."""
 
         async def _measure_latency_handler(request: web.Request) -> web.Response:
-            model: bytes = await request.read()
-            latency: Dict[str, float] = self.measure_latency(model)
+            data: Dict = pickle.loads(await request.read())
+            latency: Dict[str, float] = self.measure_latency(**data)
             return web.json_response(data=latency, status=200)
 
         route = web.post(path=f'/{self._endpoint}', handler=_measure_latency_handler)
         self._app.add_routes([route])
         web.run_app(app=self._app, host=self._host, port=self._port)
 
     @staticmethod
     @abstractmethod
-    def measure_latency(model: bytes) -> Dict[str, float]:
+    def measure_latency(model: bytes, **kwargs) -> Dict[str, float]:
         """
         Latency measuring implementation for concrete device/framework/task/etc.
 
         Must return time in **MILLISECONDS** in the form: {'latency': latency}.
         You can also put in anything else like memory consumption: {'latency': latency, 'memory': memory}.
-        When something bad happens you should raise ``web.HTTPBadRequest`` for correct reponse for client.
+        When something bad happens you should raise ``aiohttp.web.<Exception>`` for correct reponse for client,
+        see https://docs.aiohttp.org/en/latest/web_exceptions.html for more details.
 
         Parameters
         ----------
         model : bytes
             Packaged model: pickled python object, ONNX, etc.
+        kwargs : Dict
+            Additional keyword arguments.
 
         Returns
         -------
         Dict[str, float]
             Latency in milliseconds and anything else (optional).
 
         """
```

## Comparing `enot_latency_server-1.0.0.dist-info/LICENSE` & `enot_latency_server-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `enot_latency_server-1.0.0.dist-info/METADATA` & `enot_latency_server-1.1.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enot-latency-server
-Version: 1.0.0
+Version: 1.1.0
 Summary: Latency measurement server/client for ENOT Framework
 Author-email: ENOT LLC <enot@enot.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

