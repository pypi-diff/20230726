# Comparing `tmp/freeplay-0.1.7.tar.gz` & `tmp/freeplay-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeplay-0.1.7.tar", max compression
+gzip compressed data, was "freeplay-0.1.8.tar", max compression
```

## Comparing `freeplay-0.1.7.tar` & `freeplay-0.1.8.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        0 2023-05-15 03:23:13.376261 freeplay-0.1.7/README.md
--rw-r--r--   0        0        0       61 2023-06-28 22:11:30.981007 freeplay-0.1.7/freeplay/__init__.py
--rw-r--r--   0        0        0     1834 2023-06-08 17:54:13.585930 freeplay-0.1.7/freeplay/api_support.py
--rw-r--r--   0        0        0      802 2023-07-13 15:23:08.878478 freeplay-0.1.7/freeplay/completions.py
--rw-r--r--   0        0        0      188 2023-07-11 16:57:31.087747 freeplay-0.1.7/freeplay/errors.py
--rw-r--r--   0        0        0     8971 2023-07-13 15:23:08.879014 freeplay-0.1.7/freeplay/flavors.py
--rw-r--r--   0        0        0    22477 2023-07-13 15:23:08.879647 freeplay-0.1.7/freeplay/freeplay.py
--rw-r--r--   0        0        0      828 2023-07-12 17:07:23.373407 freeplay-0.1.7/freeplay/llm_parameters.py
--rw-r--r--   0        0        0      369 2023-07-12 17:52:35.686687 freeplay-0.1.7/freeplay/utils.py
--rw-r--r--   0        0        0      391 2023-07-13 15:23:21.748924 freeplay-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-18 13:19:32.515553 freeplay-0.1.8/README.md
+-rw-r--r--   0        0        0       61 2023-06-29 11:36:19.640171 freeplay-0.1.8/freeplay/__init__.py
+-rw-r--r--   0        0        0     1834 2023-06-09 01:58:55.719111 freeplay-0.1.8/freeplay/api_support.py
+-rw-r--r--   0        0        0      833 2023-07-19 21:25:17.786018 freeplay-0.1.8/freeplay/completions.py
+-rw-r--r--   0        0        0      188 2023-06-15 16:32:13.004072 freeplay-0.1.8/freeplay/errors.py
+-rw-r--r--   0        0        0    11304 2023-07-19 21:25:17.786614 freeplay-0.1.8/freeplay/flavors.py
+-rw-r--r--   0        0        0    24684 2023-07-19 21:25:17.787170 freeplay-0.1.8/freeplay/freeplay.py
+-rw-r--r--   0        0        0      828 2023-06-27 18:52:46.171090 freeplay-0.1.8/freeplay/llm_parameters.py
+-rw-r--r--   0        0        0      955 2023-07-19 21:25:17.787505 freeplay-0.1.8/freeplay/provider_config.py
+-rw-r--r--   0        0        0      369 2023-07-19 21:25:17.788071 freeplay-0.1.8/freeplay/utils.py
+-rw-r--r--   0        0        0      391 2023-07-26 20:08:07.947400 freeplay-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 freeplay-0.1.8/PKG-INFO
```

### Comparing `freeplay-0.1.7/freeplay/api_support.py` & `freeplay-0.1.8/freeplay/api_support.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.7/freeplay/completions.py` & `freeplay-0.1.8/freeplay/completions.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 @dataclass
 class PromptTemplateWithMetadata:
     project_version_id: str
     prompt_template_id: str
     name: str
     content: str
+    flavor_name: Optional[str]
     params: Optional[dict[str, Any]]
 
     def get_params(self) -> LLMParameters:
         return LLMParameters.empty() if self.params is None else LLMParameters(self.params)
 
 
 @dataclass
```

### Comparing `freeplay-0.1.7/freeplay/flavors.py` & `freeplay-0.1.8/freeplay/flavors.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,219 +4,289 @@
 from typing import Optional, Generator, Any
 
 import anthropic  # type: ignore
 import openai
 
 from .completions import CompletionChunk, PromptTemplateWithMetadata, CompletionResponse, ChatCompletionResponse, \
     ChatMessage
-from .errors import APIKeyMissingError
+from .errors import APIKeyMissingError, FreeplayError
 from .llm_parameters import LLMParameters
+from .provider_config import ProviderConfig, OpenAIConfig, AnthropicConfig
 from .utils import format_template_variables
 
 
 class Flavor(ABC):
+    @classmethod
+    def get_by_name(cls, flavor_name: str) -> 'Flavor':
+        match flavor_name:
+            case OpenAIText.record_format_type:
+                return OpenAIText()
+            case OpenAIChat.record_format_type:
+                return OpenAIChat()
+            case AnthropicClaudeText.record_format_type:
+                return AnthropicClaudeText()
+            case _:
+                raise FreeplayError(
+                    'Configured flavor not found in SDK. Please update your SDK version or configure a different model in the Freeplay UI.')
+
     @property
     @abstractmethod
     def record_format_type(self) -> str:
         raise NotImplementedError()
 
     @property
     def _model_params_with_defaults(self) -> LLMParameters:
         return LLMParameters.empty()
 
     @abstractmethod
     def format(self, prompt_template: PromptTemplateWithMetadata, variables: dict[str, str]) -> str:
         pass
 
     @abstractmethod
-    def call_service(self, formatted_prompt: str, llm_parameters: LLMParameters) -> CompletionResponse:
+    def call_service(
+            self,
+            formatted_prompt: str,
+            provider_config: ProviderConfig,
+            llm_parameters: LLMParameters
+    ) -> CompletionResponse:
         pass
 
     @abstractmethod
-    def call_service_stream(self, formatted_prompt: str, llm_parameters: LLMParameters) -> Generator[
-        CompletionChunk, None, None]:
+    def call_service_stream(
+            self,
+            formatted_prompt: str,
+            provider_config: ProviderConfig,
+            llm_parameters: LLMParameters
+    ) -> Generator[CompletionChunk, None, None]:
         pass
 
     def get_model_params(self, llm_parameters: LLMParameters) -> LLMParameters:
         return self._model_params_with_defaults.merge_and_override(llm_parameters)
 
 
 class ChatFlavor(Flavor, ABC):
     @abstractmethod
     def continue_chat(
             self,
             messages: list[ChatMessage],
+            provider_config: ProviderConfig,
             llm_parameters: LLMParameters
     ) -> ChatCompletionResponse:
         pass
 
     @abstractmethod
     def continue_chat_stream(
             self,
             messages: list[ChatMessage],
+            provider_config: ProviderConfig,
             llm_parameters: LLMParameters
     ) -> Generator[CompletionChunk, None, None]:
         pass
 
 
 class OpenAI(Flavor, ABC):
-    def __init__(self, openai_api_key: str, openai_api_base: Optional[str] = None):
+    def configure_openai(self, openai_config: Optional[OpenAIConfig]) -> None:
         super().__init__()
-        if openai_api_base:
-            openai.api_base = openai_api_base
+        if not openai_config:
+            raise APIKeyMissingError(
+                "Missing OpenAI key. Use a ProviderConfig to specify keys prior to getting completion.")
+
+        if openai_config.api_base:
+            openai.api_base = openai_config.api_base
 
-        if not openai_api_key or not openai_api_key.strip():
-            raise APIKeyMissingError("OpenAI API key not set. It must be set to make calls to the service.")
+        if not openai_config.api_key or not openai_config.api_key.strip():
+            raise APIKeyMissingError("OpenAI API key is not set. It must be set to make calls to the service.")
 
-        openai.api_key = openai_api_key
+        openai.api_key = openai_config.api_key
 
 
 class OpenAIText(OpenAI):
     record_format_type = "openai_text"
     _model_params_with_defaults = LLMParameters({
         "model": "text-davinci-003"
     })
 
-    def __init__(self, openai_api_key: str, openai_api_base: Optional[str] = None):
-        super().__init__(openai_api_key, openai_api_base)
-
     def format(self, prompt_template: PromptTemplateWithMetadata, variables: dict[str, str]) -> str:
         return format_template_variables(prompt_template.content, variables)
 
-    def call_service(self, formatted_prompt: str, llm_parameters: LLMParameters) -> CompletionResponse:
-        completion = openai.Completion.create(
-            prompt=formatted_prompt,
-            **self.get_model_params(llm_parameters)
-        )  # type: ignore
+    def call_service(
+            self,
+            formatted_prompt: str,
+            provider_config: ProviderConfig,
+            llm_parameters: LLMParameters
+    ) -> CompletionResponse:
+        completion = self.__call_openai(formatted_prompt, provider_config, llm_parameters, stream=False)
         return CompletionResponse(
             content=completion.choices[0].text,
             is_complete=completion.choices[0].finish_reason == "stop"
         )
 
     def call_service_stream(
             self,
             formatted_prompt: str,
+            provider_config: ProviderConfig,
             llm_parameters: LLMParameters
     ) -> Generator[CompletionChunk, None, None]:
-        completion = openai.Completion.create(
-            prompt=formatted_prompt,
-            stream=True,
-            **self.get_model_params(llm_parameters)
-        )  # type: ignore
+        completion = self.__call_openai(formatted_prompt, provider_config, llm_parameters, stream=True)
 
         for chunk in completion:
             yield CompletionChunk(
                 text=chunk.choices[0].text,
                 is_complete=chunk.choices[0].finish_reason == "stop"
             )
 
+    def __call_openai(
+            self,
+            prompt: str,
+            provider_config: ProviderConfig,
+            llm_parameters: LLMParameters,
+            stream: bool
+    ) -> Any:
+        self.configure_openai(provider_config.openai)
+        return openai.Completion.create(
+            prompt=prompt,
+            stream=stream,
+            **self.get_model_params(llm_parameters)
+        )  # type: ignore
+
 
 class OpenAIChat(OpenAI, ChatFlavor):
     record_format_type = "openai_chat"
     _model_params_with_defaults = LLMParameters({
         "model": "gpt-3.5-turbo"
     })
 
-    def __init__(self, openai_api_key: str, openai_api_base: Optional[str] = None):
-        super().__init__(openai_api_key, openai_api_base)
-
     def format(self, prompt_template: PromptTemplateWithMetadata, variables: dict[str, str]) -> str:
         # Extract messages JSON to enable formatting of individual content fields of each message. If we do not
         # extract the JSON, current variable interpolation will fail on JSON curly braces.
-        messages_as_json: list[dict[str,str]] = json.loads(prompt_template.content)
+        messages_as_json: list[dict[str, str]] = json.loads(prompt_template.content)
         formatted_messages = [
             {
                 "content": format_template_variables(message['content'], variables), "role": message['role']
             } for message in messages_as_json]
         return json.dumps(formatted_messages)
 
-    def call_service(self, formatted_prompt: str, llm_parameters: LLMParameters) -> CompletionResponse:
+    def call_service(
+            self,
+            formatted_prompt: str,
+            provider_config: ProviderConfig,
+            llm_parameters: LLMParameters
+    ) -> CompletionResponse:
         messages = json.loads(formatted_prompt)
-        completion = self.__call_openai(messages, llm_parameters, stream=False)
+        completion = self.__call_openai(messages, provider_config, llm_parameters, stream=False)
         return CompletionResponse(
             content=completion.choices[0].message.content,
             is_complete=completion.choices[0].finish_reason == 'stop'
         )
 
     def call_service_stream(
             self,
             formatted_prompt: str,
+            provider_config: ProviderConfig,
             llm_parameters: LLMParameters
     ) -> Generator[CompletionChunk, None, None]:
         messages = json.loads(formatted_prompt)
-        completion_stream = self.__call_openai(messages, llm_parameters, stream=True)
+        completion_stream = self.__call_openai(messages, provider_config, llm_parameters, stream=True)
         for chunk in completion_stream:
             yield CompletionChunk(
                 text=chunk.choices[0].delta.get('content', ""),
                 is_complete=chunk.choices[0].finish_reason == "stop"
             )
 
-    def continue_chat(self, messages: list[ChatMessage], llm_parameters: LLMParameters) -> ChatCompletionResponse:
-        completion = self.__call_openai(messages, llm_parameters, stream=False)
+    def continue_chat(
+            self,
+            messages: list[ChatMessage],
+            provider_config: ProviderConfig,
+            llm_parameters: LLMParameters
+    ) -> ChatCompletionResponse:
+        completion = self.__call_openai(messages, provider_config, llm_parameters, stream=False)
 
         message_history = copy(messages)
         message_history.append(completion.choices[0].message.to_dict())
         return ChatCompletionResponse(
             content=completion.choices[0].message.content,
             message_history=message_history,
             is_complete=completion.choices[0].finish_reason == "stop"
         )
 
     def continue_chat_stream(
             self,
             messages: list[ChatMessage],
+            provider_config: ProviderConfig,
             llm_parameters: LLMParameters
     ) -> Generator[CompletionChunk, None, None]:
-        completion_stream = self.__call_openai(messages, llm_parameters, stream=True)
+        completion_stream = self.__call_openai(messages, provider_config, llm_parameters, stream=True)
         for chunk in completion_stream:
             yield CompletionChunk(
                 text=chunk.choices[0].delta.get('content', ''),
                 is_complete=chunk.choices[0].finish_reason == "stop"
             )
 
-    def __call_openai(self, messages: list[ChatMessage], llm_parameters: LLMParameters, stream: bool) -> Any:
+    def __call_openai(
+            self,
+            messages: list[ChatMessage],
+            provider_config: ProviderConfig,
+            llm_parameters: LLMParameters,
+            stream: bool
+    ) -> Any:
+        self.configure_openai(provider_config.openai)
         return openai.ChatCompletion.create(
             messages=messages,
             **self.get_model_params(llm_parameters),
             stream=stream
         )  # type: ignore
 
 
 class AnthropicClaudeText(Flavor):
     record_format_type = "anthropic_text"
     _model_params_with_defaults = LLMParameters({
         "model": "claude-v1",
         "max_tokens_to_sample": 100
     })
 
-    def __init__(self, anthropic_api_key: str):
-        self.client = anthropic.Client(anthropic_api_key)
+    def __init__(self) -> None:
+        self.client = None
+
+    def get_anthropic_client(self, anthropic_config: Optional[AnthropicConfig]) -> Any:
+        if self.client:
+            return self.client
+
+        if not anthropic_config:
+            raise APIKeyMissingError(
+                "Missing Anthropic key. Use a ProviderConfig to specify keys prior to getting completion.")
+
+        self.client = anthropic.Client(anthropic_config.api_key)
+        return self.client
 
     def format(self, prompt_template: PromptTemplateWithMetadata, variables: dict[str, str]) -> str:
         interpolated_prompt = format_template_variables(prompt_template.content, variables)
         # Anthropic expects a specific Chat format "Human: $PROMPT_TEXT\n\nAssistant:". We add the wrapping for Text.
         chat_formatted_prompt = f"{anthropic.HUMAN_PROMPT} {interpolated_prompt} {anthropic.AI_PROMPT}"
         return chat_formatted_prompt
 
-    def call_service(self, formatted_prompt: str, llm_parameters: LLMParameters) -> CompletionResponse:
-        anthropic_response = self.client.completion(
+    def call_service(self, formatted_prompt: str, provider_config: ProviderConfig,
+                     llm_parameters: LLMParameters) -> CompletionResponse:
+        client = self.get_anthropic_client(provider_config.anthropic)
+        anthropic_response = client.completion(
             prompt=formatted_prompt,
             **self.get_model_params(llm_parameters)
         )
         return CompletionResponse(
             content=anthropic_response['completion'],
             is_complete=anthropic_response['stop_reason'] == 'stop_sequence'
         )
 
     def call_service_stream(
             self,
             formatted_prompt: str,
+            provider_config: ProviderConfig,
             llm_parameters: LLMParameters
     ) -> Generator[CompletionChunk, None, None]:
-        anthropic_response = self.client.completion_stream(
+        client = self.get_anthropic_client(provider_config.anthropic)
+        anthropic_response = client.completion_stream(
             prompt=formatted_prompt,
             **self.get_model_params(llm_parameters)
         )
 
         # Yield incremental text completions. Claude returns the full text output in every chunk.
         # We want to predictably return a stream like we do for OpenAI.
         prev_chunk = ''
```

### Comparing `freeplay-0.1.7/freeplay/freeplay.py` & `freeplay-0.1.8/freeplay/freeplay.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from copy import copy
 import json
 import logging
 import time
+from copy import copy
 from dataclasses import dataclass
 from typing import Optional, Generator, Any, cast, Tuple
 
 from . import api_support
 from .completions import PromptTemplates, CompletionResponse, CompletionChunk, PromptTemplateWithMetadata, \
     ChatCompletionResponse, ChatMessage
 from .errors import TemplateNotFoundError, APIKeyMissingError, AuthorizationError, FreeplayError
 from .flavors import Flavor, ChatFlavor
 from .llm_parameters import LLMParameters
+from .provider_config import ProviderConfig
 
 JsonDom = dict[str, Any]
 Variables = dict[str, str]
 
 logger = logging.getLogger(__name__)
 default_tag = 'latest'
 
@@ -58,14 +59,15 @@
         )
         return prompts
 
     def prepare_and_make_chat_call(
             self,
             session_id: str,
             flavor: ChatFlavor,
+            provider_config: ProviderConfig,
             tag: str,
             target_template: PromptTemplateWithMetadata,
             variables: Variables,
             message_history: list[ChatMessage],
             new_messages: Optional[list[ChatMessage]],
             test_run_id: Optional[str] = None,
             completion_parameters: Optional[LLMParameters] = None) -> ChatCompletionResponse:
@@ -74,15 +76,16 @@
         try:
             params = target_template.get_params() \
                 .merge_and_override(self.client_params) \
                 .merge_and_override(completion_parameters)
             prompt_messages = copy(message_history)
             if new_messages is not None:
                 prompt_messages.extend(new_messages)
-            completion_response = flavor.continue_chat(messages=prompt_messages, llm_parameters=params)
+            completion_response = flavor.continue_chat(messages=prompt_messages, provider_config=provider_config,
+                                                       llm_parameters=params)
         except Exception as e:
             raise FreeplayError("Error calling service") from e
         end = int(time.time())
 
         model = flavor.get_model_params(params).get('model')
         formatted_prompt = json.dumps(prompt_messages)
         # record data
@@ -103,14 +106,15 @@
 
         return completion_response
 
     def prepare_and_make_chat_call_stream(
             self,
             session_id: str,
             flavor: ChatFlavor,
+            provider_config: ProviderConfig,
             tag: str,
             target_template: PromptTemplateWithMetadata,
             variables: Variables,
             message_history: list[ChatMessage],
             new_messages: Optional[list[ChatMessage]],
             test_run_id: Optional[str] = None,
             completion_parameters: Optional[LLMParameters] = None
@@ -120,15 +124,15 @@
         try:
             prompt_messages = copy(message_history)
             if new_messages is not None:
                 prompt_messages.extend(new_messages)
             params = target_template.get_params() \
                 .merge_and_override(self.client_params) \
                 .merge_and_override(completion_parameters)
-            completion_response = flavor.continue_chat_stream(prompt_messages, llm_parameters=params)
+            completion_response = flavor.continue_chat_stream(prompt_messages, provider_config, llm_parameters=params)
         except Exception as e:
             raise FreeplayError("Error calling service") from e
         end = int(time.time())
 
         str_content = ''
         last_is_complete = False
         for chunk in completion_response:
@@ -155,94 +159,100 @@
 
     def prepare_and_make_call(
             self,
             session_id: str,
             prompts: PromptTemplates,
             template_name: str,
             variables: dict[str, str],
-            flavor: Flavor,
+            flavor: Optional[Flavor],
+            provider_config: ProviderConfig,
             tag: str,
             test_run_id: Optional[str] = None,
             completion_parameters: Optional[LLMParameters] = None
     ) -> CompletionResponse:
         target_template = self.find_template_by_name(prompts, template_name)
-        formatted_prompt = flavor.format(target_template, variables)
+        params = target_template.get_params() \
+            .merge_and_override(self.client_params) \
+            .merge_and_override(completion_parameters)
+
+        final_flavor = pick_flavor_from_config(flavor, target_template.flavor_name)
+        formatted_prompt = final_flavor.format(target_template, variables)
 
         # make call
         start = int(time.time())
         try:
-            params = target_template.get_params() \
-                .merge_and_override(self.client_params) \
-                .merge_and_override(completion_parameters)
-
-            completion_response = flavor.call_service(
-                formatted_prompt=formatted_prompt, llm_parameters=params)
+            completion_response = final_flavor.call_service(
+                formatted_prompt=formatted_prompt, provider_config=provider_config, llm_parameters=params)
         except Exception as e:
             raise FreeplayError("Error calling service") from e
         end = int(time.time())
 
-        model = flavor.get_model_params(params).get('model')
+        model = final_flavor.get_model_params(params).get('model')
 
         # record data
         self.__record_call(
             completion_response.content,
             completion_response.is_complete,
             end,
             formatted_prompt,
             session_id,
             start,
             target_template,
             variables,
-            flavor.record_format_type,
+            final_flavor.record_format_type,
             tag,
             test_run_id,
             model
         )
 
         return completion_response
 
     def prepare_and_make_call_stream(
             self,
             session_id: str,
             prompts: PromptTemplates,
             template_name: str,
             variables: dict[str, str],
-            flavor: Flavor,
+            flavor: Optional[Flavor],
+            provider_config: ProviderConfig,
             tag: str,
             test_run_id: Optional[str] = None,
             completion_parameters: Optional[LLMParameters] = None
     ) -> Generator[CompletionChunk, None, None]:
         target_template = self.find_template_by_name(prompts, template_name)
-        formatted_prompt = flavor.format(target_template, variables)
-
-        # make call
-        start = int(time.time())
         params = target_template.get_params() \
             .merge_and_override(self.client_params) \
             .merge_and_override(completion_parameters)
-        completion_response = flavor.call_service_stream(formatted_prompt=formatted_prompt, llm_parameters=params)
+
+        final_flavor = pick_flavor_from_config(flavor, target_template.flavor_name)
+        formatted_prompt = final_flavor.format(target_template, variables)
+
+        # make call
+        start = int(time.time())
+        completion_response = final_flavor.call_service_stream(
+            formatted_prompt=formatted_prompt, provider_config=provider_config, llm_parameters=params)
         text_chunks = []
         last_is_complete = False
         for chunk in completion_response:
             text_chunks.append(chunk.text)
             last_is_complete = chunk.is_complete
             yield chunk
         end = int(time.time())
 
-        model = flavor.get_model_params(params).get('model')
+        model = final_flavor.get_model_params(params).get('model')
 
         self.__record_call(''.join(text_chunks),
                            last_is_complete,
                            end,
                            formatted_prompt,
                            session_id,
                            start,
                            target_template,
                            variables,
-                           flavor.record_format_type,
+                           final_flavor.record_format_type,
                            tag,
                            test_run_id,
                            model)
 
     def __record_call(
             self,
             completion_content: str,
@@ -294,21 +304,23 @@
 
 class Session:
     def __init__(
             self,
             call_support: CallSupport,
             session_id: str,
             prompts: PromptTemplates,
-            flavor: Flavor,
+            flavor: Optional[Flavor],
+            provider_config: ProviderConfig,
             tag: str = default_tag,
             test_run_id: Optional[str] = None
     ) -> None:
         self.tag = tag
         self.call_support = call_support
         self.session_flavor = flavor
+        self.provider_config = provider_config
         self.session_id = session_id
         self.prompts = prompts
         self.test_run_id = test_run_id
 
     def get_completion(
             self,
             template_name: str,
@@ -318,14 +330,15 @@
     ) -> CompletionResponse:
         completion_flavor = flavor or self.session_flavor
         return self.call_support.prepare_and_make_call(self.session_id,
                                                        self.prompts,
                                                        template_name,
                                                        variables,
                                                        completion_flavor,
+                                                       self.provider_config,
                                                        self.tag,
                                                        self.test_run_id,
                                                        completion_parameters=LLMParameters(kwargs))
 
     def get_completion_stream(
             self,
             template_name: str,
@@ -335,56 +348,60 @@
     ) -> Generator[CompletionChunk, None, None]:
         completion_flavor = flavor or self.session_flavor
         return self.call_support.prepare_and_make_call_stream(self.session_id,
                                                               self.prompts,
                                                               template_name,
                                                               variables,
                                                               completion_flavor,
+                                                              self.provider_config,
                                                               self.tag,
                                                               self.test_run_id,
                                                               completion_parameters=LLMParameters(kwargs))
 
 
 class ChatSession(Session):
     def __init__(
             self,
             call_support: CallSupport,
             session_id: str,
             prompts: PromptTemplates,
             flavor: ChatFlavor,
+            provider_config: ProviderConfig,
             template_name: str,
             variables: Variables,
             tag: str = default_tag,
             test_run_id: Optional[str] = None
     ) -> None:
-        super().__init__(call_support, session_id, prompts, flavor, tag, test_run_id)
+        super().__init__(call_support, session_id, prompts, flavor, provider_config, tag, test_run_id)
         self.flavor = flavor  # Ensures a ChatFlavor is set for this session.
         # A Chat Session tracks the template_name and variables for a set of chat completions.
         # Assumes these will be the same for subsequent chat messages.
         self.variables = variables
         self.target_template = self.call_support.find_template_by_name(self.prompts, template_name)
-        self.__initial_messages = json.loads(self.session_flavor.format(self.target_template, self.variables))
+        self.__initial_messages = json.loads(self.flavor.format(self.target_template, self.variables))
 
     def start_chat(self, **kwargs: Any) -> ChatCompletionResponse:
         return self.call_support.prepare_and_make_chat_call(
             self.session_id,
             flavor=self.flavor,
+            provider_config=self.provider_config,
             tag=self.tag,
             test_run_id=self.test_run_id,
             target_template=self.target_template,
             variables=self.variables,
             message_history=self.__initial_messages,
             new_messages=None,
             completion_parameters=LLMParameters(kwargs)
         )
 
     def start_chat_stream(self, **kwargs: Any) -> Tuple[Generator[CompletionChunk, None, None], list[ChatMessage]]:
         return self.call_support.prepare_and_make_chat_call_stream(
             self.session_id,
             flavor=self.flavor,
+            provider_config=self.provider_config,
             tag=self.tag,
             test_run_id=self.test_run_id,
             target_template=self.target_template,
             variables=self.variables,
             message_history=self.__initial_messages,
             new_messages=None,
             completion_parameters=LLMParameters(kwargs)
@@ -395,14 +412,15 @@
             message_history: list[ChatMessage],
             new_messages: Optional[list[ChatMessage]] = None,
             **kwargs: Any
     ) -> ChatCompletionResponse:
         return self.call_support.prepare_and_make_chat_call(
             self.session_id,
             flavor=self.flavor,
+            provider_config=self.provider_config,
             tag=self.tag,
             test_run_id=self.test_run_id,
             target_template=self.target_template,
             variables=self.variables,
             message_history=message_history,
             new_messages=new_messages,
             completion_parameters=LLMParameters(kwargs)
@@ -413,14 +431,15 @@
             message_history: list[ChatMessage],
             new_messages: Optional[list[ChatMessage]] = None,
             **kwargs: Any
     ) -> Generator[CompletionChunk, None, None]:
         return self.call_support.prepare_and_make_chat_call_stream(
             self.session_id,
             flavor=self.flavor,
+            provider_config=self.provider_config,
             tag=self.tag,
             test_run_id=self.test_run_id,
             target_template=self.target_template,
             variables=self.variables,
             message_history=message_history,
             new_messages=new_messages,
             completion_parameters=LLMParameters(kwargs)
@@ -428,56 +447,63 @@
 
 
 @dataclass()
 class FreeplayTestRun:
     def __init__(
             self,
             call_support: CallSupport,
-            flavor: Flavor,
+            flavor: Optional[Flavor],
+            provider_config: ProviderConfig,
             test_run_id: str,
             inputs: list[dict[str, str]]
     ):
         self.call_support = call_support
         self.flavor = flavor
+        self.provider_config = provider_config
         self.test_run_id = test_run_id
         self.inputs = inputs
 
     def get_inputs(self) -> list[dict[str, str]]:
         return self.inputs
 
     def create_session(self, project_id: str, tag: str = default_tag) -> Session:
         project_session = self.call_support.create_session(project_id, tag, self.test_run_id)
         prompts = self.call_support.get_prompts(project_id, tag)
-        return Session(self.call_support, project_session['session_id'], prompts, self.flavor, tag, self.test_run_id)
+        return Session(self.call_support, project_session['session_id'], prompts, self.flavor, self.provider_config,
+                       tag, self.test_run_id)
 
 
 # This SDK prototype does not support full functionality of either OpenAI's API or Freeplay's
 # The simplifications are:
 #  - Always assumes there is a single choice returned, does not support multiple
 #  - Does not support an "escape hatch" to allow use of features we don't explicitly expose
 class Freeplay:
     def __init__(
             self,
-            flavor: Flavor,
             freeplay_api_key: str,
             api_base: str,
+            provider_config: ProviderConfig,
+            flavor: Optional[Flavor] = None,
             **kwargs: Any
     ) -> None:
         if not freeplay_api_key or not freeplay_api_key.strip():
             raise APIKeyMissingError("Freeplay API key not set. It must be set to the Freeplay API.")
+        provider_config.validate()
 
         self.call_support = CallSupport(freeplay_api_key, api_base, **kwargs)
+        self.provider_config = provider_config
         self.client_flavor = flavor
         self.freeplay_api_key = freeplay_api_key
         self.api_base = api_base
 
     def create_session(self, project_id: str, tag: str = default_tag) -> Session:
         project_session = self.call_support.create_session(project_id, tag)
         prompts = self.call_support.get_prompts(project_id, tag)
-        return Session(self.call_support, project_session['session_id'], prompts, self.client_flavor, tag)
+        return Session(self.call_support, project_session['session_id'], prompts, self.client_flavor,
+                       self.provider_config, tag)
 
     def get_completion(
             self,
             project_id: str,
             template_name: str,
             variables: dict[str, str],
             tag: str = default_tag,
@@ -489,14 +515,15 @@
         completion_flavor = flavor or self.client_flavor
 
         return self.call_support.prepare_and_make_call(project_session['session_id'],
                                                        prompts,
                                                        template_name,
                                                        variables,
                                                        completion_flavor,
+                                                       self.provider_config,
                                                        tag,
                                                        completion_parameters=LLMParameters(kwargs))
 
     def get_completion_stream(
             self,
             project_id: str,
             template_name: str,
@@ -510,27 +537,33 @@
         completion_flavor = flavor or self.client_flavor
 
         return self.call_support.prepare_and_make_call_stream(project_session['session_id'],
                                                               prompts,
                                                               template_name,
                                                               variables,
                                                               completion_flavor,
+                                                              self.provider_config,
                                                               tag,
                                                               completion_parameters=LLMParameters(kwargs))
 
     def create_test_run(self, project_id: str, playlist: str) -> FreeplayTestRun:
         response = api_support.post_raw(
             api_key=self.freeplay_api_key,
             url=f'{self.api_base}/projects/{project_id}/test-runs',
             payload={'playlist_name': playlist},
         )
 
         json_dom = response.json()
 
-        return FreeplayTestRun(self.call_support, self.client_flavor, json_dom['test_run_id'], json_dom['inputs'])
+        return FreeplayTestRun(
+            self.call_support,
+            self.client_flavor,
+            self.provider_config,
+            json_dom['test_run_id'],
+            json_dom['inputs'])
 
     def start_chat(
             self,
             project_id: str,
             template_name: str,
             variables: Variables,
             tag: str = default_tag,
@@ -559,10 +592,22 @@
         project_session = self.call_support.create_session(project_id, tag)
         prompts = self.call_support.get_prompts(project_id, tag)
         return ChatSession(
             self.call_support,
             project_session['session_id'],
             prompts,
             self.client_flavor,
+            self.provider_config,
             template_name,
             variables,
             tag)
+
+
+def pick_flavor_from_config(completion_flavor: Optional[Flavor], ui_flavor_name: Optional[str]) -> Flavor:
+    ui_flavor = Flavor.get_by_name(ui_flavor_name) if ui_flavor_name else None
+    flavor = completion_flavor or ui_flavor
+
+    if flavor is None:
+        raise FreeplayError(
+            "Flavor must be configured on either the Freeplay client, completion call, or in the Freeplay UI. Unable to fulfill request.")
+
+    return flavor
```

### Comparing `freeplay-0.1.7/freeplay/llm_parameters.py` & `freeplay-0.1.8/freeplay/llm_parameters.py`

 * *Files identical despite different names*

### Comparing `freeplay-0.1.7/PKG-INFO` & `freeplay-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeplay
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 License: MIT
 Author: FreePlay Engineering
 Author-email: engineering@freeplay.ai
 Requires-Python: >=3.8,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

