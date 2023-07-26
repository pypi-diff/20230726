# Comparing `tmp/foundation-model-tool-0.0.6.tar.gz` & `tmp/foundation-model-tool-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation-model-tool-0.0.6.tar", last modified: Wed Jul 26 17:54:17 2023, max compression
+gzip compressed data, was "foundation-model-tool-0.0.7.tar", last modified: Wed Jul 26 20:38:55 2023, max compression
```

## Comparing `foundation-model-tool-0.0.6.tar` & `foundation-model-tool-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.424201 foundation-model-tool-0.0.6/
--rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      443 2023-07-26 17:54:17.424201 foundation-model-tool-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.287359 foundation-model-tool-0.0.6/foundation_model_pkg/
--rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.6/foundation_model_pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.329038 foundation-model-tool-0.0.6/foundation_model_pkg/tools/
--rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.6/foundation_model_pkg/tools/__init__.py
--rw-rw-rw-   0        0        0    16338 2023-07-26 17:15:44.000000 foundation-model-tool-0.0.6/foundation_model_pkg/tools/foundation_model.py
--rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.6/foundation_model_pkg/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.345640 foundation-model-tool-0.0.6/foundation_model_pkg/yamls/
--rw-rw-rw-   0        0        0      797 2023-07-26 17:29:54.000000 foundation-model-tool-0.0.6/foundation_model_pkg/yamls/foundation_model.yaml
-drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.401090 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/
--rw-rw-rw-   0        0        0      443 2023-07-26 17:54:16.000000 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-26 17:54:17.000000 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 17:54:16.000000 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-26 17:54:16.000000 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-07-26 17:54:17.000000 foundation-model-tool-0.0.6/foundation_model_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 17:54:17.425199 foundation-model-tool-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-07-26 17:54:03.000000 foundation-model-tool-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 17:54:17.422210 foundation-model-tool-0.0.6/tests/
--rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.6/tests/__init__.py
--rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.6/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:38:55.484534 foundation-model-tool-0.0.7/
+-rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      443 2023-07-26 20:38:55.484534 foundation-model-tool-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 20:38:55.294443 foundation-model-tool-0.0.7/foundation_model_pkg/
+-rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.7/foundation_model_pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:38:55.364506 foundation-model-tool-0.0.7/foundation_model_pkg/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.7/foundation_model_pkg/tools/__init__.py
+-rw-rw-rw-   0        0        0    15457 2023-07-26 19:40:41.000000 foundation-model-tool-0.0.7/foundation_model_pkg/tools/foundation_model.py
+-rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.7/foundation_model_pkg/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:38:55.404899 foundation-model-tool-0.0.7/foundation_model_pkg/yamls/
+-rw-rw-rw-   0        0        0      797 2023-07-26 17:29:54.000000 foundation-model-tool-0.0.7/foundation_model_pkg/yamls/foundation_model.yaml
+drwxrwxrwx   0        0        0        0 2023-07-26 20:38:55.452179 foundation-model-tool-0.0.7/foundation_model_tool.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-07-26 20:38:55.000000 foundation-model-tool-0.0.7/foundation_model_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-26 20:38:55.000000 foundation-model-tool-0.0.7/foundation_model_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 20:38:55.000000 foundation-model-tool-0.0.7/foundation_model_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-26 20:38:55.000000 foundation-model-tool-0.0.7/foundation_model_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-07-26 20:38:55.000000 foundation-model-tool-0.0.7/foundation_model_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 20:38:55.484534 foundation-model-tool-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-07-26 20:38:48.000000 foundation-model-tool-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 20:38:55.484534 foundation-model-tool-0.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.7/tests/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.7/tests/test_my_tool_1.py
```

### Comparing `foundation-model-tool-0.0.6/foundation_model_pkg/tools/foundation_model.py` & `foundation-model-tool-0.0.7/foundation_model_pkg/tools/foundation_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,34 @@
 import json
 import re
 import urllib.request
+
+# import uuid
 from abc import abstractmethod
 from enum import Enum
 from typing import Any, Dict, List, Mapping, Optional
 
+# from urllib.request import HTTPError
+
 from jinja2 import Template
 
 from promptflow import ToolProvider, tool
 from promptflow.connections import CustomConnection
-from promptflow.contracts.types import PromptTemplate
+
+# from promptflow.contracts.types import PromptTemplate
 from promptflow.core.tools_manager import register_builtins
 
 # from ..core.contracts import StoreStage
 # from ..core.logging.utils import LoggingUtils
 # from ..core.utils.retry_utils import retry_and_handle_exceptions
 # from .contracts.telemetry import StoreToolEventCustomDimensions, StoreToolEventNames
 # from .utils.logging import ToolLoggingUtils
 # from .utils.pf_runtime_utils import PromptflowRuntimeUtils
 
 
-def validate_role(role: str) -> None:
-    valid_roles = {"user", "assistant"}
-    if role not in valid_roles:
-        valid_roles_str = ",".join([f"'{role}:\\n'" for role in valid_roles])
-        error_message = f"""The Chat API requires a specific format for prompt definition, and the prompt should
-            include separate lines as role delimiters: {valid_roles_str}. Current parsed role '{role}' does not
-            meet the requirement. If you intend to use the Completion API, please select the appropriate API type
-            and deployment name. If you do intend to use the Chat API, please refer to the guideline at
-            https://aka.ms/pfdoc/chat-prompt or view the samples in our gallery that contain 'Chat' in the name."""
-        raise Exception(message=error_message)
-
-
-def parse_chat(chat_str: str) -> List[Dict[str, str]]:
-    # openai chat api only supports below roles.
-    separator = r"(?i)\n*(user|assistant)\s*:\s*\n"
-    chunks = re.split(separator, chat_str)
-    chat_list = []
-    for chunk in chunks:
-        last_message = chat_list[-1] if len(chat_list) > 0 else None
-        if last_message and "role" in last_message and "content" not in last_message:
-            last_message["content"] = chunk
-        else:
-            if chunk.strip() == "":
-                continue
-            # Check if prompt follows chat api message format and has valid role.
-            role = chunk.strip().lower()
-            validate_role(role)
-            new_message = {"role": role}
-            chat_list.append(new_message)
-    return chat_list
-
-
 class ModelFamily(str, Enum):
     LLAMA = "LLaMa"
     DOLLY = "Dolly"
     GPT2 = "GPT-2"
     FALCON = "Falcon"
 
 
@@ -66,50 +39,50 @@
 
 class ContentFormatterBase:
     """Transform request and response of AzureML endpoint to match with
     required schema.
     """
 
     """
-    Example:
-        .. code-block:: python
+  Example:
+      .. code-block:: python
 
-            class ContentFormatter(ContentFormatterBase):
-                content_type = "application/json"
-                accepts = "application/json"
-
-                def format_request_payload(
-                    self,
-                    prompt: str,
-                    model_kwargs: Dict
-                ) -> bytes:
-                    input_str = json.dumps(
-                        {
-                            "inputs": {"input_string": [prompt]},
-                            "parameters": model_kwargs,
-                        }
-                    )
-                    return str.encode(input_str)
-
-                def format_response_payload(self, output: str) -> str:
-                    response_json = json.loads(output)
-                    return response_json[0]["0"]
-    """
+          class ContentFormatter(ContentFormatterBase):
+              content_type = "application/json"
+              accepts = "application/json"
+
+              def format_request_payload(
+                  self,
+                  prompt: str,
+                  model_kwargs: Dict
+              ) -> bytes:
+                  input_str = json.dumps(
+                      {
+                          "inputs": {"input_string": [prompt]},
+                          "parameters": model_kwargs,
+                      }
+                  )
+                  return str.encode(input_str)
+
+              def format_response_payload(self, output: str) -> str:
+                  response_json = json.loads(output)
+                  return response_json[0]["0"]
+  """
     content_type: Optional[str] = "application/json"
     """The MIME type of the input data passed to the endpoint"""
 
     accepts: Optional[str] = "application/json"
     """The MIME type of the response data returned form the endpoint"""
 
     @staticmethod
     def escape_special_characters(prompt: str) -> str:
         """Escapes any special characters in `prompt`"""
         escape_map = {
             "\\": "\\\\",
-            '"': '"',
+            '"': '\\"',
             "\b": "\\b",
             "\f": "\\f",
             "\n": "\\n",
             "\r": "\\r",
             "\t": "\\t",
         }
 
@@ -184,58 +157,73 @@
         response_json = json.loads(output)
         return response_json[0]
 
 
 class LlamaContentFormatter(ContentFormatterBase):
     """Content formatter for LLaMa"""
 
-    def __init__(self, api: API, chat_history: Optional[List[Dict]] = []):
+    def __init__(self, api: API, chat_history: Optional[str] = ""):
         super().__init__()
         self.api = api
         self.chat_history = chat_history
 
-    def format_history(self, prompt: str) -> str:
-        """Formats the chat history for a multi-turn request"""
-        chat_list = []
-        for interaction in self.chat_history:
-            if "inputs" in interaction and "question" in interaction["inputs"]:
-                chat_list.append(
-                    {
-                        "role": "user",
-                        "content": ContentFormatterBase.escape_special_characters(interaction["inputs"]["question"]),
-                    }
-                )
-            if "outputs" in interaction and "answer" in interaction["outputs"]:
-                chat_list.append(
-                    {
-                        "role": "assistant",
-                        "content": ContentFormatterBase.escape_special_characters(interaction["outputs"]["answer"]),
-                    }
-                )
+    @staticmethod
+    def validate_role(role: str) -> None:
+        valid_roles = {"system", "user", "assistant"}
+        if role not in valid_roles:
+            valid_roles_str = ",".join([f"'{role}:\\n'" for role in valid_roles])
+            error_message = f"""The Chat API requires a specific format for prompt definition, and the prompt should
+            include separate lines as role delimiters: {valid_roles_str}. Current parsed role '{role}' does not
+            meet the requirement. If you intend to use the Completion API, please select the appropriate API type
+            and deployment name. If you do intend to use the Chat API, please refer to the guideline at
+            https://aka.ms/pfdoc/chat-prompt or view the samples in our gallery that contain 'Chat' in the name."""
+            raise Exception(error_message)
 
-        chat_list.append({"role": "user", "content": f'"{prompt}"'})
+    @staticmethod
+    def parse_chat(chat_str: str) -> List[Dict[str, str]]:
+        # LLaMa only supports below roles.
+        separator = r"(?i)\n*(system|user|assistant)\s*:\s*\n"
+        chunks = re.split(separator, chat_str)
+        chat_list = []
+        for chunk in chunks:
+            last_message = chat_list[-1] if len(chat_list) > 0 else None
+            if last_message and "role" in last_message and "content" not in last_message:
+                last_message["content"] = chunk
+            else:
+                if chunk.strip() == "":
+                    continue
+                role = chunk.strip().lower()
+                # appends consecutive user messages together to support system hack
+                if last_message and last_message.get("role", "") == "user" and role not in {"user", "assistant"}:
+                    last_message["content"] += chunk
+                    continue
+                # Check if prompt follows chat api message format and has valid role.
+                LlamaContentFormatter.validate_role(role)
+                if last_message and last_message.get("role", "") == "user" and role == "user":
+                    continue
+                # system role not officially supported, so we hack a solution by making system role the user role
+                new_message = {"role": role} if role != "system" else {"role": "user"}
+                chat_list.append(new_message)
 
-        return json.dumps(chat_list)
+        return chat_list
 
     def format_request_payload(self, prompt: str, model_kwargs: Dict) -> bytes:
         """Formats the request according the the chosen api"""
-        request_payload = ""
-
         request_payload = (
             Template('{"input_data": {"input_string":{{history}},"parameters": {{model_kwargs}}}}').render(
-                history=json.dumps(self.chat_history),
+                history=json.dumps(LlamaContentFormatter.parse_chat(self.chat_history)),
                 model_kwargs=json.dumps(model_kwargs),
             )
             if self.api == API.CHAT
             else Template('{"input_data": {"input_string": ["{{prompt}}"], "parameters": {{model_kwargs}}}}').render(
                 prompt=ContentFormatterBase.escape_special_characters(prompt),
                 model_kwargs=json.dumps(model_kwargs),
             )
         )
-
+        print(request_payload)
         return str.encode(request_payload)
 
     def format_response_payload(self, output: bytes) -> str:
         """Formats response"""
         print(json.loads(output))
         return json.loads(output)["output"] if self.api == API.CHAT else json.loads(output)[0]["0"]
 
@@ -252,38 +240,14 @@
             return DollyContentFormatter()
         elif model_family == ModelFamily.GPT2:
             return OSSContentFormatter()
         elif model_family == ModelFamily.FALCON:
             return HFContentFormatter()
 
 
-class AzureMLEndpointClient(object):
-    """AzureML Managed Endpoint client."""
-
-    def __init__(self, endpoint_url: str, endpoint_api_key: str) -> json.dumps({}):
-        """Initialize the class."""
-        if not endpoint_api_key:
-            raise ValueError("A key should be provided to invoke the endpoint")
-        self.endpoint_url = endpoint_url
-        self.endpoint_api_key = endpoint_api_key
-
-    def call(self, body: bytes) -> bytes:
-        """call."""
-
-        headers = {
-            "Content-Type": "application/json",
-            "Authorization": ("Bearer " + self.endpoint_api_key),
-        }
-
-        req = urllib.request.Request(self.endpoint_url, body, headers)
-        response = urllib.request.urlopen(req, timeout=50)
-        result = response.read()
-        return result
-
-
 class AzureMLOnlineEndpoint:
     """Azure ML Online Endpoint models.
 
     Example:
         .. code-block:: python
 
             azure_llm = AzureMLModel(
@@ -297,16 +261,14 @@
     """URL of pre-existing Endpoint. Should be passed to constructor or specified as
         env var `AZUREML_ENDPOINT_URL`."""
 
     endpoint_api_key: str = ""
     """Authentication Key for Endpoint. Should be passed to constructor or specified as
         env var `AZUREML_ENDPOINT_API_KEY`."""
 
-    http_client: Any = None  #: :meta private:
-
     content_formatter: Any = None
     """The content formatter that provides an input and output
     transform function to handle formats between the LLM and
     the endpoint"""
 
     model_kwargs: Optional[Dict] = None
     """Key word arguments to pass to the model."""
@@ -316,18 +278,14 @@
         endpoint_url: str,
         endpoint_api_key: str,
         content_formatter: ContentFormatterBase,
         model_kwargs: Optional[Dict] = None,
     ):
         self.endpoint_url = endpoint_url
         self.endpoint_api_key = endpoint_api_key
-        self.http_client = AzureMLEndpointClient(
-            endpoint_url=self.endpoint_url,
-            endpoint_api_key=self.endpoint_api_key,
-        )
         self.content_formatter = content_formatter
         self.model_kwargs = model_kwargs
 
     @property
     def _identifying_params(self) -> Mapping[str, Any]:
         """Get the identifying parameters."""
         _model_kwargs = self.model_kwargs or {}
@@ -336,14 +294,27 @@
         }
 
     @property
     def _llm_type(self) -> str:
         """Return type of llm."""
         return "azureml_endpoint"
 
+    def _call_endpoint(self, body: bytes) -> bytes:
+        """call."""
+
+        headers = {
+            "Content-Type": "application/json",
+            "Authorization": ("Bearer " + self.endpoint_api_key),
+        }
+
+        req = urllib.request.Request(self.endpoint_url, body, headers)
+        response = urllib.request.urlopen(req, timeout=50)
+        result = response.read()
+        return result
+
     def __call__(
         self,
         prompt: str,
         stop: Optional[List[str]] = json.dumps({}),
         **kwargs: Any,
     ) -> str:
         """Call out to an AzureML Managed Online endpoint.
@@ -355,15 +326,15 @@
         Example:
             .. code-block:: python
                 response = azureml_model("Tell me a joke.")
         """
         _model_kwargs = self.model_kwargs or {}
 
         body = self.content_formatter.format_request_payload(prompt, _model_kwargs)
-        endpoint_response = self.http_client.call(body)
+        endpoint_response = self._call_endpoint(body)
         response = self.content_formatter.format_response_payload(endpoint_response)
         return response
 
 
 class FoundationModel(ToolProvider):
     REQUIRED_KEYS = ["endpoint_url", "endpoint_api_key", "model_family"]
 
@@ -371,23 +342,23 @@
         super().__init__()
 
         for key in self.REQUIRED_KEYS:
             accepted_keys = ",".join([key for key in self.REQUIRED_KEYS])
             if key not in connection:
                 raise KeyError(
                     f"""Required key `{key}` not found in given custom connection.
-                        Required keys are: {accepted_keys}."""
+                      Required keys are: {accepted_keys}."""
                 )
         try:
             self.model_family = ModelFamily[connection.model_family]
         except KeyError:
             accepted_models = ",".join([model.name for model in ModelFamily])
             raise KeyError(
                 f"""Given model_family '{connection.model_family}' not recognized.
-                    Supported models are: {accepted_models}."""
+                  Supported models are: {accepted_models}."""
             )
         self.connection = connection
 
         # logging_config = ToolLoggingUtils.generate_config(tool_name=self.__class__.__name__)
         # self.__logger = LoggingUtils.sdk_logger(__package__, logging_config)
         # self.__logger.update_telemetry_context({StoreToolEventCustomDimensions.TOOL_INSTANCE_ID: str(uuid.uuid4())})
 
@@ -408,15 +379,15 @@
         **kwargs,
     ) -> str:
         prompt = Template(prompt, trim_blocks=True, keep_trailing_newline=True).render(**kwargs)
 
         content_formatter = ContentFormatterFactory.get_content_formatter(
             model_family=self.model_family,
             api=api,
-            chat_history=parse_chat(prompt) if api == API.CHAT else [],
+            chat_history=prompt,
         )
 
         llm = AzureMLOnlineEndpoint(
             endpoint_url=self.connection.endpoint_url,
             endpoint_api_key=self.connection.endpoint_api_key,
             content_formatter=content_formatter,
             model_kwargs=model_kwargs,
```

### Comparing `foundation-model-tool-0.0.6/foundation_model_pkg/tools/utils.py` & `foundation-model-tool-0.0.7/foundation_model_pkg/tools/utils.py`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.6/foundation_model_pkg/yamls/foundation_model.yaml` & `foundation-model-tool-0.0.7/foundation_model_pkg/yamls/foundation_model.yaml`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.6/setup.py` & `foundation-model-tool-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foundation-model-tool",
-    version="0.0.6",
+    version="0.0.7",
     author="Matthew DeGuzman",
     author_email="t-madeguzman@microsoft.com",
     description="Package to use Foundation Models in Prompt Flow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     entry_points={"package_tools": ["foundation_model = foundation_model_pkg.tools.utils:list_package_tools"]},
```

### Comparing `foundation-model-tool-0.0.6/tests/test_my_tool_1.py` & `foundation-model-tool-0.0.7/tests/test_my_tool_1.py`

 * *Files identical despite different names*

