# Comparing `tmp/octoai_sdk-0.1.2.tar.gz` & `tmp/octoai_sdk-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoai_sdk-0.1.2.tar", max compression
+gzip compressed data, was "octoai_sdk-0.2.0.tar", max compression
```

## Comparing `octoai_sdk-0.1.2.tar` & `octoai_sdk-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      227 2023-06-13 16:22:01.228527 octoai_sdk-0.1.2/octoai/__init__.py
--rw-r--r--   0        0        0     9967 2023-06-30 15:47:18.275698 octoai_sdk-0.1.2/octoai/client.py
--rw-r--r--   0        0        0      995 2023-06-09 21:08:23.293946 octoai_sdk-0.1.2/octoai/errors.py
--rw-r--r--   0        0        0       56 2023-06-09 21:08:23.294496 octoai_sdk-0.1.2/octoai/scaffolds/flan-t5/requirements.txt
--rw-r--r--   0        0        0     1323 2023-06-21 00:01:12.459613 octoai_sdk-0.1.2/octoai/scaffolds/flan-t5/service.py
--rw-r--r--   0        0        0     1290 2023-06-12 17:09:46.783772 octoai_sdk-0.1.2/octoai/scaffolds/flan-t5/test_request.py
--rw-r--r--   0        0        0        0 2023-06-09 21:08:23.296075 octoai_sdk-0.1.2/octoai/scaffolds/hello-world/requirements.txt
--rw-r--r--   0        0        0      395 2023-06-09 21:08:23.296287 octoai_sdk-0.1.2/octoai/scaffolds/hello-world/service.py
--rw-r--r--   0        0        0     1272 2023-06-12 17:09:46.788205 octoai_sdk-0.1.2/octoai/scaffolds/hello-world/test_request.py
--rw-r--r--   0        0        0       34 2023-06-13 16:21:58.470830 octoai_sdk-0.1.2/octoai/scaffolds/wav2vec/requirements.txt
--rw-r--r--   0        0        0     1956 2023-06-21 00:01:12.461702 octoai_sdk-0.1.2/octoai/scaffolds/wav2vec/service.py
--rw-r--r--   0        0        0     1458 2023-06-13 16:21:58.473214 octoai_sdk-0.1.2/octoai/scaffolds/wav2vec/test_request.py
--rw-r--r--   0        0        0       33 2023-06-09 21:08:23.297221 octoai_sdk-0.1.2/octoai/scaffolds/yolov8/requirements.txt
--rw-r--r--   0        0        0     3474 2023-06-21 00:01:12.463890 octoai_sdk-0.1.2/octoai/scaffolds/yolov8/service.py
--rw-r--r--   0        0        0     1809 2023-06-12 17:09:46.790769 octoai_sdk-0.1.2/octoai/scaffolds/yolov8/test_request.py
--rw-r--r--   0        0        0     6788 2023-06-28 18:01:35.201394 octoai_sdk-0.1.2/octoai/server.py
--rw-r--r--   0        0        0     2698 2023-06-12 17:09:46.799814 octoai_sdk-0.1.2/octoai/service.py
--rw-r--r--   0        0        0    13192 2023-06-29 17:19:44.000199 octoai_sdk-0.1.2/octoai/types.py
--rw-r--r--   0        0        0     4000 2023-06-29 01:18:48.788389 octoai_sdk-0.1.2/octoai/utils.py
--rw-r--r--   0        0        0     1050 2023-06-30 15:49:19.565770 octoai_sdk-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 octoai_sdk-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3119 2023-07-18 16:44:57.986412 octoai_sdk-0.2.0/octoai/README.md
+-rw-r--r--   0        0        0      227 2023-06-13 16:22:01.228527 octoai_sdk-0.2.0/octoai/__init__.py
+-rw-r--r--   0        0        0    13201 2023-07-26 19:32:26.932359 octoai_sdk-0.2.0/octoai/client.py
+-rw-r--r--   0        0        0      995 2023-06-09 21:08:23.293946 octoai_sdk-0.2.0/octoai/errors.py
+-rw-r--r--   0        0        0       56 2023-07-11 00:00:05.180672 octoai_sdk-0.2.0/octoai/scaffolds/flan-t5/requirements.txt
+-rw-r--r--   0        0        0     1323 2023-06-21 00:01:12.459613 octoai_sdk-0.2.0/octoai/scaffolds/flan-t5/service.py
+-rw-r--r--   0        0        0     1290 2023-06-12 17:09:46.783772 octoai_sdk-0.2.0/octoai/scaffolds/flan-t5/test_request.py
+-rw-r--r--   0        0        0        0 2023-06-09 21:08:23.296075 octoai_sdk-0.2.0/octoai/scaffolds/hello-world/requirements.txt
+-rw-r--r--   0        0        0      395 2023-06-09 21:08:23.296287 octoai_sdk-0.2.0/octoai/scaffolds/hello-world/service.py
+-rw-r--r--   0        0        0     1272 2023-06-12 17:09:46.788205 octoai_sdk-0.2.0/octoai/scaffolds/hello-world/test_request.py
+-rw-r--r--   0        0        0       34 2023-07-11 00:00:05.181513 octoai_sdk-0.2.0/octoai/scaffolds/wav2vec/requirements.txt
+-rw-r--r--   0        0        0     1956 2023-06-21 00:01:12.461702 octoai_sdk-0.2.0/octoai/scaffolds/wav2vec/service.py
+-rw-r--r--   0        0        0     1458 2023-06-13 16:21:58.473214 octoai_sdk-0.2.0/octoai/scaffolds/wav2vec/test_request.py
+-rw-r--r--   0        0        0       33 2023-06-09 21:08:23.297221 octoai_sdk-0.2.0/octoai/scaffolds/yolov8/requirements.txt
+-rw-r--r--   0        0        0     3474 2023-06-21 00:01:12.463890 octoai_sdk-0.2.0/octoai/scaffolds/yolov8/service.py
+-rw-r--r--   0        0        0     1809 2023-06-12 17:09:46.790769 octoai_sdk-0.2.0/octoai/scaffolds/yolov8/test_request.py
+-rw-r--r--   0        0        0     6788 2023-06-28 18:01:35.201394 octoai_sdk-0.2.0/octoai/server.py
+-rw-r--r--   0        0        0     2698 2023-07-10 18:36:55.809355 octoai_sdk-0.2.0/octoai/service.py
+-rw-r--r--   0        0        0    13192 2023-06-29 17:19:44.000199 octoai_sdk-0.2.0/octoai/types.py
+-rw-r--r--   0        0        0     4000 2023-07-18 16:44:55.338153 octoai_sdk-0.2.0/octoai/utils.py
+-rw-r--r--   0        0        0     1050 2023-07-26 19:33:12.234661 octoai_sdk-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      774 1970-01-01 00:00:00.000000 octoai_sdk-0.2.0/PKG-INFO
```

### Comparing `octoai_sdk-0.1.2/octoai/client.py` & `octoai_sdk-0.2.0/octoai/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class StreamResponse(BaseModel):
     """Response class for LLMs that allow :class:`Client.infer_stream`.
 
     :param token: Generated token
     :type token: :Class:`Token`
     :param generated_text: Complete generated text - only available from final token.
-    :type generated_text: Optional[str]
+    :type generated_text: str, optional
     """
 
     class Token(BaseModel):
         """Tokens generated for :class:`StreamResponse`.
 
         :param id: Token ID from model tokenizer
         :type id: int
@@ -42,41 +42,54 @@
         logprob: float
         special: bool
 
     token: Token
     generated_text: Optional[str]
 
 
+class InferenceFuture(BaseModel):
+    """Response class for endpoints that support server side async inferences.
+
+    :param response_id: Unique identifier for inference
+    :type response_id: str
+    :param poll_url: URL to poll status of inference.
+    :type poll_url: str
+    """
+
+    response_id: str
+    poll_url: str
+
+
 class Client:
     """A class that allows inferences from existing endpoints.
 
     :param token: api token, defaults to None
     :type token: str, optional
     :param public_endpoints_url: str, url to fetch available public models,
         defaults to "https://api.octoai.cloud/v1/public-endpoints"
     :type public_endpoints_url: str
     :param config_path: path to '/.octoai/config.yaml'.  Installed in ~,
         defaults to None and will check home path
-    :type config_path: Optional[str]
+    :type config_path: str, optional
 
     Sets various headers. Gets auth token from environment if none is provided.
     """
 
     def __init__(
         self,
         token: Optional[str] = None,
         public_endpoints_url: Optional[
             str
         ] = "https://api.octoai.cloud/v1/public-endpoints",
         config_path: Optional[str] = None,
     ) -> None:
         """Initialize the :class: `octoai.Client` with an auth token.
 
-        :raises OctoAIServerError: server-side failures (unreachable, etc)
-        :raises OctoAIClientError: client-side failures (throttling, unset token)
+        :raises :class:`OctoAIServerError`: server-side failure (unreachable, etc)
+        :raises :class:`OctoAIClientError`: client-side failure (throttled, no token)
         """
         self._public_endpoints: Dict[str, str] = {}
         self._public_endpoints_url = public_endpoints_url
 
         token = token if token else os.environ.get("OCTOAI_TOKEN", None)
 
         if not token:
@@ -97,21 +110,19 @@
                 + "You won't be able to reach OctoAI endpoints."
             )
 
         version = octoai.__version__  # type: ignore
         headers = {
             "Content-Type": "application/json",
             "user-agent": f"octoai-{version}",
-            "accept": "text/event-stream",
         }
 
         if token:
             headers["Authorization"] = f"Bearer {token}"
 
-        self._headers = headers
         # Set all timeouts to 900 seconds to account for cold starts, latency.
         timeout = httpx.Timeout(timeout=900.0)
         self._httpx_client = httpx.Client(timeout=timeout, headers=headers)
 
     def _initialize_public_endpoints(self) -> None:
         """Initialize self._public_endpoints with dict of names to quickstart urls."""
         response = utils.retry(
@@ -120,14 +131,33 @@
         if response.status_code == 200:
             response_json = response.json()
             for model in response_json:
                 self._public_endpoints[model["name"]] = model["endpoint"]
         else:
             self._error(response.status_code, response.text)
 
+    @staticmethod
+    def _error(status_code: int, text: str):
+        """Raise error of correct type for status code including message.
+
+        :param status_code: HTTP status_code
+        :type status_code: int
+        :param text: error message from API server
+        :type text: str
+
+        :raises OctoAIServerError: server-side failures (unreachable, etc)
+        :raises OctoAIClientError: client-side failures (throttling, unset token)
+        """
+        if status_code >= 500:
+            raise OctoAIServerError(f"Server error: {status_code} {text}")
+        elif status_code == 429:
+            raise OctoAIClientError(f"Throttling error: {status_code} {text}")
+        else:
+            raise OctoAIClientError(f"Error: {status_code} {text}")
+
     def infer(self, endpoint_url: str, inputs: Mapping[str, Any]) -> Mapping[str, Any]:
         """Send a request to the given endpoint URL with inputs as request body.
 
         :param endpoint_url: target endpoint
         :type endpoint_url: str
         :param inputs: inputs for target endpoint
         :type inputs: Mapping[str, Any]
@@ -141,14 +171,38 @@
         resp = utils.retry(
             lambda: self._httpx_client.post(url=endpoint_url, json=inputs)
         )
         if resp.status_code != 200:
             self._error(resp.status_code, resp.text)
         return resp.json()
 
+    def infer_async(
+        self, endpoint_url: str, inputs: Mapping[str, Any]
+    ) -> InferenceFuture:
+        """Execute an inference in the background on the server.
+
+        :class:`InferenceFuture` allows you to query status and get results
+        once it's ready.
+
+        :param endpoint_url: url to post inference request
+        :type endpoint_url: str
+        :param inputs: inputs to send to endpoint
+        :type inputs: Mapping[str, Any]
+        """
+        resp = utils.retry(
+            lambda: self._httpx_client.post(
+                url=endpoint_url, json=inputs, headers={"X-OctoAI-Async": "1"}
+            )
+        )
+        if resp.status_code >= 400:
+            self._error(resp.status_code, resp.text)
+        resp_json = resp.json()
+        future = InferenceFuture(**resp_json)
+        return future
+
     def infer_stream(
         self,
         endpoint_url: str,
         inputs: Mapping[str, Any],
         parameters: Mapping[str, Any],
     ) -> Iterator[StreamResponse]:
         """Stream infer response body for supporting LLM endpoints.
@@ -165,16 +219,17 @@
         :rtype: Iterator[:class:`StreamResponse`]
         """
         with self._httpx_client.stream(
             method="POST",
             url=endpoint_url,
             json=inputs,
             params=parameters,
+            headers={"accept": "text/event-stream"},
         ) as resp:
-            if resp.status_code != 200:
+            if resp.status_code >= 400:
                 self._error(resp.status_code, resp.text)
 
             for payload in resp.iter_lines():
                 # New lines used to separate payloads
                 if payload == "\n":
                     continue
                 # Event data identified with "data:"  JSON inside.
@@ -183,49 +238,81 @@
                     # Parse payload kwargs, validate expected stream.
                     try:
                         stream_response = StreamResponse(**payload_dict)
                     except ValidationError:
                         self._error(resp.status_code, resp.text)
                     yield stream_response
 
+    def _poll_future(self, future: InferenceFuture) -> Dict[str, str]:
+        """Get from poll_url and return response.
+
+        :param future: Future from :meth:`Client.infer_async`
+        :type future: :class:`InferenceFuture`
+        :raises: :class:`OctoAIClientError`
+        :raises: :class:`OctoAIServerError`
+        :returns: Dictionary with response
+        :rtype: Dict[str, str]
+        """
+        response = self._httpx_client.get(url=future.poll_url)
+        if response.status_code >= 400:
+            self._error(response.status_code, response.text)
+        return response.json()
+
+    def is_future_ready(self, future: InferenceFuture) -> bool:
+        """Return whether the future's result has been computed.
+
+        This class will raise any errors if the status code is >= 400.
+
+        :param future: Future from :meth:`Client.infer_async`
+        :type future: :class:`InferenceFuture`
+        :raises: :class:`OctoAIClientError`
+        :raises: :class:`OctoAIServerError`
+        :returns: True if able to use :meth:`Client.get_future_result`
+        """
+        resp_dict = self._poll_future(future)
+        return "completed" == resp_dict.get("status")
+
+    def get_future_result(self, future: InferenceFuture) -> Optional[Dict[str, Any]]:
+        """Return the result of an inference.
+
+        This class will raise any errors if the status code is >= 400.
+
+        :param future: Future from :meth:`Client.infer_async`
+        :type future: :class:`InferenceFuture`
+        :raises: :class:`OctoAIClientError`
+        :raises: :class:`OctoAIServerError`
+        :returns: None if future is not ready, or dict of the response.
+        :rtype: Dict[str, Any], optional
+        """
+        resp_dict = self._poll_future(future)
+        if resp_dict.get("status") != "completed":
+            return None
+        response_url = resp_dict.get("response_url")
+        response = self._httpx_client.get(response_url)
+        if response.status_code >= 400:
+            self._error(response.status_code, response.text)
+        return response.json()
+
     def health_check(self, endpoint_url: str, timeout: float = 900.0) -> int:
         """Check health of an endpoint using a get request.  Try until timeout.
 
         :param endpoint_url: URL as a str starting with https permitting get requests.
         :type endpoint_url: str
         :param timeout: Seconds before request times out, defaults to 900.
         :type timeout: float
         :return: status code from get request.  200 means ready.
         :rtype: int
         """
         resp = utils.health_check(
             lambda: self._httpx_client.get(url=endpoint_url), timeout=timeout
         )
-        if resp.status_code != 200:
+        if resp.status_code >= 400:
             self._error(resp.status_code, resp.text)
         return resp.status_code
 
-    def _error(self, status_code: int, text: str):
-        """Raise error of correct type for status code including message.
-
-        :param status_code: HTTP status_code
-        :type status_code: int
-        :param text: error message from API server
-        :type text: str
-
-        :raises OctoAIServerError: server-side failures (unreachable, etc)
-        :raises OctoAIClientError: client-side failures (throttling, unset token)
-        """
-        if status_code >= 500:
-            raise OctoAIServerError(f"Server error: {status_code} {text}")
-        elif status_code == 429:
-            raise OctoAIClientError(f"Throttling error: {status_code} {text}")
-        else:
-            raise OctoAIClientError(f"Error: {status_code} {text}")
-
     @property
     def public_endpoints(self) -> Dict[str, str]:
         """Return dict of public endpoint names as strs to endpoint urls as strs.
 
         :return: Dict of public endpoint name to URL.
         :rtype: Dict[str, str]
         """
```

### Comparing `octoai_sdk-0.1.2/octoai/errors.py` & `octoai_sdk-0.2.0/octoai/errors.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/scaffolds/flan-t5/service.py` & `octoai_sdk-0.2.0/octoai/scaffolds/flan-t5/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/scaffolds/flan-t5/test_request.py` & `octoai_sdk-0.2.0/octoai/scaffolds/flan-t5/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/scaffolds/hello-world/test_request.py` & `octoai_sdk-0.2.0/octoai/scaffolds/hello-world/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/scaffolds/wav2vec/service.py` & `octoai_sdk-0.2.0/octoai/scaffolds/wav2vec/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/scaffolds/wav2vec/test_request.py` & `octoai_sdk-0.2.0/octoai/scaffolds/wav2vec/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/scaffolds/yolov8/service.py` & `octoai_sdk-0.2.0/octoai/scaffolds/yolov8/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/scaffolds/yolov8/test_request.py` & `octoai_sdk-0.2.0/octoai/scaffolds/yolov8/test_request.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/server.py` & `octoai_sdk-0.2.0/octoai/server.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/service.py` & `octoai_sdk-0.2.0/octoai/service.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/types.py` & `octoai_sdk-0.2.0/octoai/types.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/octoai/utils.py` & `octoai_sdk-0.2.0/octoai/utils.py`

 * *Files identical despite different names*

### Comparing `octoai_sdk-0.1.2/pyproject.toml` & `octoai_sdk-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octoai-sdk"
-version = "0.1.2"
+version = "0.2.0"
 description = "A runtime library for OctoAI."
 authors = ["OctoML"]
 packages = [
     { include = "octoai" }
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `octoai_sdk-0.1.2/PKG-INFO` & `octoai_sdk-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoai-sdk
-Version: 0.1.2
+Version: 0.2.0
 Summary: A runtime library for OctoAI.
 Author: OctoML
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

