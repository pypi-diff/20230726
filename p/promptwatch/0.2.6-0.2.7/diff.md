# Comparing `tmp/promptwatch-0.2.6.tar.gz` & `tmp/promptwatch-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.2.6.tar", last modified: Tue Jul 18 16:08:39 2023, max compression
+gzip compressed data, was "promptwatch-0.2.7.tar", last modified: Wed Jul 26 12:46:14 2023, max compression
```

## Comparing `promptwatch-0.2.6.tar` & `promptwatch-0.2.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.373280 promptwatch-0.2.6/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-18 16:08:39.373089 promptwatch-0.2.6/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.6/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.6/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-07-18 16:08:39.373331 promptwatch-0.2.6/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.6/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.365479 promptwatch-0.2.6/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.368685 promptwatch-0.2.6/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-07-18 16:08:14.000000 promptwatch-0.2.6/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.6/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.6/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.6/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5281 2023-07-14 21:49:02.000000 promptwatch-0.2.6/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.6/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.371101 promptwatch-0.2.6/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.6/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.6/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    31322 2023-07-18 10:38:03.000000 promptwatch-0.2.6/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.6/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    18116 2023-07-18 10:44:42.000000 promptwatch-0.2.6/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.372450 promptwatch-0.2.6/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.6/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.6/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.6/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.6/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2368 2023-06-17 16:42:18.000000 promptwatch-0.2.6/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.369861 promptwatch-0.2.6/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-18 16:08:39.000000 promptwatch-0.2.6/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-07-18 16:08:39.000000 promptwatch-0.2.6/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-07-18 16:08:39.000000 promptwatch-0.2.6/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.6/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-07-18 16:08:39.000000 promptwatch-0.2.6/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-07-18 16:08:39.000000 promptwatch-0.2.6/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.144037 promptwatch-0.2.7/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-26 12:46:14.143818 promptwatch-0.2.7/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.7/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.7/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-07-26 12:46:14.144087 promptwatch-0.2.7/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.7/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.133565 promptwatch-0.2.7/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.137215 promptwatch-0.2.7/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-07-26 12:43:06.000000 promptwatch-0.2.7/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-07-22 21:21:26.000000 promptwatch-0.2.7/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.7/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.7/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5281 2023-07-14 21:49:02.000000 promptwatch-0.2.7/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.7/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.140639 promptwatch-0.2.7/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.7/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13202 2023-07-22 21:45:48.000000 promptwatch-0.2.7/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    31232 2023-07-25 15:13:47.000000 promptwatch-0.2.7/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.7/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    18116 2023-07-18 10:44:42.000000 promptwatch-0.2.7/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.142930 promptwatch-0.2.7/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.7/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.7/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.7/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.7/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2368 2023-06-17 16:42:18.000000 promptwatch-0.2.7/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-26 12:46:14.138965 promptwatch-0.2.7/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-26 12:46:14.000000 promptwatch-0.2.7/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-07-26 12:46:14.000000 promptwatch-0.2.7/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-07-26 12:46:14.000000 promptwatch-0.2.7/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.7/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-07-26 12:46:14.000000 promptwatch-0.2.7/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-07-26 12:46:14.000000 promptwatch-0.2.7/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.2.6/PKG-INFO` & `promptwatch-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.6
+Version: 0.2.7
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.6/README.md` & `promptwatch-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/setup.py` & `promptwatch-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch/caching.py` & `promptwatch-0.2.7/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch/client.py` & `promptwatch-0.2.7/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch/data_model.py` & `promptwatch-0.2.7/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch/decorators.py` & `promptwatch-0.2.7/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch/langchain/caching.py` & `promptwatch-0.2.7/src/promptwatch/langchain/caching.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-
-
-
 from __future__ import annotations
+import json
 from typing import Any, Optional, Union
 from langchain.prompts.chat import ChatPromptValue
 from langchain.llms.base import LLM, BaseLLM
 from langchain.chat_models.base import BaseChatModel
 from langchain.embeddings.base import Embeddings
 from langchain.schema import AIMessage, BaseMessage, ChatGeneration, ChatResult
 from langchain.schema import PromptValue
 from langchain.schema import LLMResult
-
 from ..data_model import LlmPrompt, NamedPromptTemplateDescription
 from ..decorators import FORMATTED_PROMPT_CONTEXT_KEY
 from typing import List
 from .. import PromptWatch
 from langchain.schema import Generation
 from typing import Any, Optional, Union
 import datetime
@@ -187,18 +184,30 @@
     ):
         cached_res,callback=self._get_from_cache(messages, stop=stop)
         
         if not cached_res:
 
             chat_result:ChatResult = await self.inner_llm._agenerate(messages, stop, **kwargs) 
             if callback:
-                callback(cached_res, chat_result.generations[0].text)
+                function_call = chat_result.generations[0].message and chat_result.generations[0].message.additional_kwargs and chat_result.generations[0].message.additional_kwargs.get("function_call")
+                if function_call:
+                    additional_data={"function_call":function_call}
+                    result =  chat_result.generations[0].message.content + '\x03'+ json.dumps(additional_data)
+                else:
+                    result = chat_result.generations[0].message.content
+
+                callback(cached_res, result)
             return chat_result
         else:
-            generated_msg = AIMessage(content=cached_res.result)
+            if '\x03' in cached_res.result:
+                result, additional_data = cached_res.result.split('\x03')
+                additional_data = json.loads(additional_data)
+                generated_msg = AIMessage(content=result, additional_kwargs=additional_data)
+            else:
+                generated_msg = AIMessage(content=cached_res.result)
             generation = ChatGeneration(message=generated_msg, generation_info={"cached":True, **cached_res.metadata, "cache_namespace_key":cached_res.cache_namespace_key})
             return ChatResult(generations=[generation],llm_output={"cached":True})
 
         
     def _generate(
         self, messages: List[BaseMessage], stop: Optional[List[str]] = None,**kwargs
     ) -> ChatResult:
```

### Comparing `promptwatch-0.2.6/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.2.7/src/promptwatch/langchain/langchain_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,27 +139,27 @@
 
     def reverse_monkey_patching(self):
         for func in self.monkey_patched_functions:
             #TODO: .. we should restore the state of the things as were before...
             pass
             
         
-    async def on_chat_model_start(
+    def on_chat_model_start(
         self,
         serialized: Dict[str, Any],
         messages: List[List[BaseMessage]],
         *,
         run_id,
         parent_run_id = None,
         **kwargs: Any,
     ) -> Any:
-        await self.on_llm_start(serialized, messages, run_id=run_id, parent_run_id=parent_run_id, **kwargs)
+        self.on_llm_start(serialized, messages, run_id=run_id, parent_run_id=parent_run_id, **kwargs)
     
 
-    async  def on_llm_start(
+    def on_llm_start(
         self, serialized: Dict[str, Any], prompts: List[str, List[BaseMessage]], **kwargs: Any
     ) -> Any:
         """Run when LLM starts running."""
 
         prompt_template = None
         prompt_input_values=None
         llm_info=None
@@ -256,20 +256,20 @@
                     info_message=info_message,
                 )
             )
 
 
 
     
-    async  def on_llm_new_token(self, token: str, **kwargs: Any) -> Any:
+    def on_llm_new_token(self, token: str, **kwargs: Any) -> Any:
         """Run on new LLM token. Only available when streaming is enabled."""
         pass
 
     
-    async def on_llm_end(self, response: LLMResult, **kwargs: Any) -> Any:
+    def on_llm_end(self, response: LLMResult, **kwargs: Any) -> Any:
         """Run when LLM ends running."""
         if len(response.generations)>1:
             prompts =  self.prompt_watch.current_activity.prompts
         else:
             prompts=[self.prompt_watch.current_activity]
         
         
@@ -295,15 +295,15 @@
                 if total_tokens:
                     self.prompt_watch.current_activity.metadata["total_tokens"] = self.prompt_watch.current_activity.metadata.get("total_tokens",0)+ token_usage["total_tokens"]
         self.prompt_watch._close_current_activity()
 
         
 
     
-    async def on_llm_error(
+    def on_llm_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when LLM errors."""
         self.prompt_watch._on_error(error, kwargs)
 
     
     def on_chain_start(
@@ -358,15 +358,15 @@
                 docs.append(DocumentSnippet(
                     text=doc.page_content, 
                     source=source,
                     metadata=metadata if metadata else None # to not pass empty objects
                     ))
             self.prompt_watch._add_activity(RetrievedDocuments(documents=docs))
     
-    async  def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> Any:
+    def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> Any:
         """Run when chain ends running."""
         
         
         self.prompt_watch._remove_context(LLM_CHAIN_CONTEXT_KEY)
         outputs = copy_dict_serializable_values(outputs)
         self.prompt_watch.current_activity.outputs=outputs
         if outputs.get("answer"):
@@ -380,61 +380,61 @@
                 parent_activity.metadata={"total_tokens":self.prompt_watch.current_activity.metadata["total_tokens"]}
             else:
                 parent_activity.metadata["total_tokens"] = parent_activity.metadata.get("total_tokens",0)+ self.prompt_watch.current_activity.metadata["total_tokens"]
         
         self.prompt_watch._close_current_activity()
 
     
-    async  def on_chain_error(
+    def on_chain_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when chain errors."""
         self.prompt_watch._on_error(error, kwargs)
 
     
-    async def on_tool_start(
+    def on_tool_start(
         self, serialized: Dict[str, Any], input_str: str, **kwargs: Any
     ) -> Any:
         """Run when tool starts running."""
         self.prompt_watch._open_activity(
                 Action(tool_type=serialized.get("name") or "undefined", input=input_str, input_data=kwargs)
             )
 
     
-    async  def on_tool_end(self, output: str, **kwargs: Any) -> Any:
+    def on_tool_end(self, output: str, **kwargs: Any) -> Any:
         """Run when tool ends running."""
         self.prompt_watch.current_activity.output=output
         self.prompt_watch.current_activity.output_data=kwargs
         self.prompt_watch._close_current_activity()
 
 
         
     
 
     
-    async  def on_tool_error(
+    def on_tool_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when tool errors."""
         self.prompt_watch._on_error(error, kwargs)
 
     
-    async def on_text(self, text: str, **kwargs: Any) -> Any:
+    def on_text(self, text: str, **kwargs: Any) -> Any:
         """Run on arbitrary text."""
 
     
-    async def on_agent_action(self, action: AgentAction, **kwargs: Any) -> Any:
+    def on_agent_action(self, action: AgentAction, **kwargs: Any) -> Any:
         """Run on agent action."""
         
         
 
 
 
     
-    async def on_agent_finish(self, finish: AgentFinish, **kwargs: Any) -> Any:
+    def on_agent_finish(self, finish: AgentFinish, **kwargs: Any) -> Any:
         """Run on agent end."""
         answer_text = finish[0].get("output")
         answer_activity = Answer(text=answer_text)
         self.prompt_watch._add_activity(answer_activity, as_root=True)
         if finish.return_values:
             answer_activity.metadata["outputs"]:finish.return_values
```

### Comparing `promptwatch-0.2.6/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.2.7/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch/promptwatch_context.py` & `promptwatch-0.2.7/src/promptwatch/promptwatch_context.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.2.7/src/promptwatch/unit_tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.2.7/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.2.7/src/promptwatch/unit_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch/utils.py` & `promptwatch-0.2.7/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.6/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.2.7/src/promptwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.6
+Version: 0.2.7
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.6/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.2.7/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

