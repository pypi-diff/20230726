# Comparing `tmp/foundation-model-tool-0.0.4.tar.gz` & `tmp/foundation-model-tool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation-model-tool-0.0.4.tar", last modified: Wed Jul 26 16:55:54 2023, max compression
+gzip compressed data, was "foundation-model-tool-0.0.5.tar", last modified: Wed Jul 26 17:16:27 2023, max compression
```

## Comparing `foundation-model-tool-0.0.4.tar` & `foundation-model-tool-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 16:55:54.818082 foundation-model-tool-0.0.4/
--rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      443 2023-07-26 16:55:54.786124 foundation-model-tool-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 16:55:54.518404 foundation-model-tool-0.0.4/foundation_model_pkg/
--rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.4/foundation_model_pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:55:54.613244 foundation-model-tool-0.0.4/foundation_model_pkg/tools/
--rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.4/foundation_model_pkg/tools/__init__.py
--rw-rw-rw-   0        0        0    16366 2023-07-25 23:19:14.000000 foundation-model-tool-0.0.4/foundation_model_pkg/tools/foundation_model.py
--rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.4/foundation_model_pkg/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:55:54.628983 foundation-model-tool-0.0.4/foundation_model_pkg/yamls/
--rw-rw-rw-   0        0        0      686 2023-07-26 16:55:01.000000 foundation-model-tool-0.0.4/foundation_model_pkg/yamls/foundation_model.yaml
-drwxrwxrwx   0        0        0        0 2023-07-26 16:55:54.739354 foundation-model-tool-0.0.4/foundation_model_tool.egg-info/
--rw-rw-rw-   0        0        0      443 2023-07-26 16:55:54.000000 foundation-model-tool-0.0.4/foundation_model_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-26 16:55:54.000000 foundation-model-tool-0.0.4/foundation_model_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 16:55:54.000000 foundation-model-tool-0.0.4/foundation_model_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-07-26 16:55:54.000000 foundation-model-tool-0.0.4/foundation_model_tool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-07-26 16:55:54.000000 foundation-model-tool-0.0.4/foundation_model_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 16:55:54.818082 foundation-model-tool-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      719 2023-07-26 16:55:47.000000 foundation-model-tool-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 16:55:54.786124 foundation-model-tool-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.4/tests/test_my_tool_1.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.433250 foundation-model-tool-0.0.5/
+-rw-rw-rw-   0        0        0       41 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      443 2023-07-26 17:16:27.432247 foundation-model-tool-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      109 2023-07-07 21:32:34.000000 foundation-model-tool-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.385139 foundation-model-tool-0.0.5/foundation_model_pkg/
+-rw-rw-rw-   0        0        0       82 2023-07-25 21:36:35.000000 foundation-model-tool-0.0.5/foundation_model_pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.385139 foundation-model-tool-0.0.5/foundation_model_pkg/tools/
+-rw-rw-rw-   0        0        0       82 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.5/foundation_model_pkg/tools/__init__.py
+-rw-rw-rw-   0        0        0    16338 2023-07-26 17:15:44.000000 foundation-model-tool-0.0.5/foundation_model_pkg/tools/foundation_model.py
+-rw-rw-rw-   0        0        0      524 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.5/foundation_model_pkg/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.385139 foundation-model-tool-0.0.5/foundation_model_pkg/yamls/
+-rw-rw-rw-   0        0        0      796 2023-07-26 17:14:40.000000 foundation-model-tool-0.0.5/foundation_model_pkg/yamls/foundation_model.yaml
+drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.426247 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-07-26 17:16:27.000000 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-26 17:16:27.000000 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:16:27.000000 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-26 17:16:27.000000 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-07-26 17:16:27.000000 foundation-model-tool-0.0.5/foundation_model_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:16:27.433250 foundation-model-tool-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-07-26 17:16:24.000000 foundation-model-tool-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:16:27.430249 foundation-model-tool-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-07-20 19:20:36.000000 foundation-model-tool-0.0.5/tests/test_my_tool_1.py
```

### Comparing `foundation-model-tool-0.0.4/foundation_model_pkg/tools/foundation_model.py` & `foundation-model-tool-0.0.5/foundation_model_pkg/tools/foundation_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,28 @@
 # from ..core.utils.retry_utils import retry_and_handle_exceptions
 # from .contracts.telemetry import StoreToolEventCustomDimensions, StoreToolEventNames
 # from .utils.logging import ToolLoggingUtils
 # from .utils.pf_runtime_utils import PromptflowRuntimeUtils
 
 
 def validate_role(role: str) -> None:
-    valid_roles = {"system", "user", "assistant"}
+    valid_roles = {"user", "assistant"}
     if role not in valid_roles:
         valid_roles_str = ",".join([f"'{role}:\\n'" for role in valid_roles])
         error_message = f"""The Chat API requires a specific format for prompt definition, and the prompt should
             include separate lines as role delimiters: {valid_roles_str}. Current parsed role '{role}' does not
             meet the requirement. If you intend to use the Completion API, please select the appropriate API type
             and deployment name. If you do intend to use the Chat API, please refer to the guideline at
             https://aka.ms/pfdoc/chat-prompt or view the samples in our gallery that contain 'Chat' in the name."""
         raise Exception(message=error_message)
 
 
 def parse_chat(chat_str: str) -> List[Dict[str, str]]:
     # openai chat api only supports below roles.
-    separator = r"(?i)\n*(system|user|assistant)\s*:\s*\n"
+    separator = r"(?i)\n*(user|assistant)\s*:\s*\n"
     chunks = re.split(separator, chat_str)
     chat_list = []
     for chunk in chunks:
         last_message = chat_list[-1] if len(chat_list) > 0 else None
         if last_message and "role" in last_message and "content" not in last_message:
             last_message["content"] = chunk
         else:
@@ -398,15 +398,15 @@
         # self.__logger.telemetry_event_completed(event_name=StoreToolEventNames.INIT)
         # self.__logger.flush()
 
     # @retry_and_handle_exceptions(HTTPError)
     @tool
     def foundation_model(
         self,
-        prompt: PromptTemplate,
+        prompt: str,
         api: API,
         model_kwargs: Optional[Dict] = {},
         **kwargs,
     ) -> str:
         prompt = Template(prompt, trim_blocks=True, keep_trailing_newline=True).render(**kwargs)
 
         content_formatter = ContentFormatterFactory.get_content_formatter(
```

### Comparing `foundation-model-tool-0.0.4/foundation_model_pkg/tools/utils.py` & `foundation-model-tool-0.0.5/foundation_model_pkg/tools/utils.py`

 * *Files identical despite different names*

### Comparing `foundation-model-tool-0.0.4/setup.py` & `foundation-model-tool-0.0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foundation-model-tool",
-    version="0.0.4",
+    version="0.0.5",
     author="Matthew DeGuzman",
     author_email="t-madeguzman@microsoft.com",
     description="Package to use Foundation Models in Prompt Flow",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     entry_points={"package_tools": ["foundation_model = foundation_model_pkg.tools.utils:list_package_tools"]},
```

### Comparing `foundation-model-tool-0.0.4/tests/test_my_tool_1.py` & `foundation-model-tool-0.0.5/tests/test_my_tool_1.py`

 * *Files identical despite different names*

