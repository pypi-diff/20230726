# Comparing `tmp/gradio_client-0.2.9.tar.gz` & `tmp/gradio_client-0.3.0.tar.gz`

## Comparing `gradio_client-0.2.9.tar` & `gradio_client-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
--rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.2.9/README.md
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 gradio_client-0.2.9/requirements.txt
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/__init__.py
--rw-r--r--   0        0        0    48764 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/client.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/data_classes.py
--rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/documentation.py
--rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/media_data.py
--rw-r--r--   0        0        0    19131 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/serializing.py
--rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/types.json
--rw-r--r--   0        0        0    16933 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/utils.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.2.9/gradio_client/version.txt
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 gradio_client-0.2.9/.gitignore
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 gradio_client-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     7045 2020-02-02 00:00:00.000000 gradio_client-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     5654 2020-02-02 00:00:00.000000 gradio_client-0.3.0/README.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 gradio_client-0.3.0/requirements.txt
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/__init__.py
+-rw-r--r--   0        0        0    54987 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/client.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/data_classes.py
+-rw-r--r--   0        0        0    10494 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/documentation.py
+-rw-r--r--   0        0        0   722623 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/media_data.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/package.json
+-rw-r--r--   0        0        0    19054 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/serializing.py
+-rw-r--r--   0        0        0     4356 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/types.json
+-rw-r--r--   0        0        0    17121 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/utils.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/version.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/cli/__init__.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/cli/deploy_discord.py
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 gradio_client-0.3.0/gradio_client/templates/discord_chat.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 gradio_client-0.3.0/.gitignore
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 gradio_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 gradio_client-0.3.0/PKG-INFO
```

### Comparing `gradio_client-0.2.9/README.md` & `gradio_client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.9/gradio_client/client.py` & `gradio_client-0.3.0/gradio_client/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """The main Client class for the Python client."""
 from __future__ import annotations
 
 import concurrent.futures
 import json
 import os
 import re
+import secrets
 import tempfile
 import threading
 import time
 import urllib.parse
 import uuid
 import warnings
 from concurrent.futures import Future, TimeoutError
@@ -16,15 +17,15 @@
 from pathlib import Path
 from threading import Lock
 from typing import Any, Callable, Literal
 
 import huggingface_hub
 import requests
 import websockets
-from huggingface_hub import SpaceHardware, SpaceStage
+from huggingface_hub import CommitOperationAdd, SpaceHardware, SpaceStage
 from huggingface_hub.utils import (
     RepositoryNotFoundError,
     build_hf_headers,
     send_telemetry,
 )
 from packaging import version
 
@@ -423,15 +424,15 @@
         if self.serialize:
             api_info_url = urllib.parse.urljoin(self.src, utils.API_INFO_URL)
         else:
             api_info_url = urllib.parse.urljoin(self.src, utils.RAW_API_INFO_URL)
 
         # Versions of Gradio older than 3.29.0 returned format of the API info
         # from the /info endpoint
-        if version.parse(self.config.get("version", "2.0")) > version.Version("3.29.0"):
+        if version.parse(self.config.get("version", "2.0")) > version.Version("3.36.1"):
             r = requests.get(api_info_url, headers=self.headers)
             if r.ok:
                 info = r.json()
             else:
                 raise ValueError(f"Could not fetch api info for {self.src}")
         else:
             fetch = requests.post(
@@ -599,14 +600,155 @@
                 ) from ae
             if "allow_flagging" in config:
                 raise ValueError(
                     "Gradio 2.x is not supported by this client. Please upgrade your Gradio app to Gradio 3.x or higher."
                 )
             return config
 
+    def deploy_discord(
+        self,
+        discord_bot_token: str | None = None,
+        api_names: list[str | tuple[str, str]] | None = None,
+        to_id: str | None = None,
+        hf_token: str | None = None,
+        private: bool = False,
+    ):
+        """
+        Deploy the upstream app as a discord bot. Currently only supports gr.ChatInterface.
+        Parameters:
+            discord_bot_token: This is the "password" needed to be able to launch the bot. Users can get a token by creating a bot app on the discord website. If run the method without specifying a token, the space will explain how to get one. See here: https://huggingface.co/spaces/freddyaboulton/test-discord-bot-v1.
+            api_names: The api_names of the app to turn into bot commands. This parameter currently has no effect as ChatInterface only has one api_name ('/chat').
+            to_id: The name of the space hosting the discord bot. If None, the name will be gradio-discord-bot-{random-substring}
+            hf_token: HF api token with write priviledges in order to upload the files to HF space. Can be ommitted if logged in via the HuggingFace CLI, unless the upstream space is private. Obtain from: https://huggingface.co/settings/token
+            private: Whether the space hosting the discord bot is private. The visibility of the discord bot itself is set via the discord website. See https://huggingface.co/spaces/freddyaboulton/test-discord-bot-v1
+        """
+
+        if self.config["mode"] == "chat_interface" and not api_names:
+            api_names = [("chat", "chat")]
+
+        valid_list = isinstance(api_names, list) and (
+            isinstance(n, str)
+            or (
+                isinstance(n, tuple) and isinstance(n[0], str) and isinstance(n[1], str)
+            )
+            for n in api_names
+        )
+        if api_names is None or not valid_list:
+            raise ValueError(
+                f"Each entry in api_names must be either a string or a tuple of strings. Received {api_names}"
+            )
+        assert (
+            len(api_names) == 1
+        ), "Currently only one api_name can be deployed to discord."
+
+        for i, name in enumerate(api_names):
+            if isinstance(name, str):
+                api_names[i] = (name, name)
+
+        fn = next(
+            (ep for ep in self.endpoints if ep.api_name == f"/{api_names[0][0]}"), None
+        )
+        if not fn:
+            raise ValueError(
+                f"api_name {api_names[0][0]} not present in {self.space_id or self.src}"
+            )
+        inputs = [
+            inp for inp in fn.input_component_types if fn not in utils.SKIP_COMPONENTS
+        ]
+        outputs = [
+            inp for inp in fn.input_component_types if fn not in utils.SKIP_COMPONENTS
+        ]
+        if not inputs == ["textbox"] and outputs == ["textbox"]:
+            raise ValueError(
+                "Currently only api_names with a single textbox as input and output are supported. "
+                f"Received {inputs} and {outputs}"
+            )
+
+        is_private = False
+        if self.space_id:
+            is_private = huggingface_hub.space_info(self.space_id).private
+            if is_private:
+                assert hf_token, (
+                    f"Since {self.space_id} is private, you must explicitly pass in hf_token "
+                    "so that it can be added as a secret in the discord bot space."
+                )
+
+        if to_id:
+            if "/" in to_id:
+                to_id = to_id.split("/")[1]
+            space_id = huggingface_hub.get_full_repo_name(to_id, token=hf_token)
+        else:
+            if self.space_id:
+                space_id = f'{self.space_id.split("/")[1]}-gradio-discord-bot'
+            else:
+                space_id = f"gradio-discord-bot-{secrets.token_hex(4)}"
+            space_id = huggingface_hub.get_full_repo_name(space_id, token=hf_token)
+
+        api = huggingface_hub.HfApi()
+
+        try:
+            huggingface_hub.space_info(space_id)
+            first_upload = False
+        except huggingface_hub.utils.RepositoryNotFoundError:
+            first_upload = True
+
+        huggingface_hub.create_repo(
+            space_id,
+            repo_type="space",
+            space_sdk="gradio",
+            token=hf_token,
+            exist_ok=True,
+            private=private,
+        )
+        if first_upload:
+            huggingface_hub.metadata_update(
+                repo_id=space_id,
+                repo_type="space",
+                metadata={"tags": ["gradio-discord-bot"]},
+            )
+
+        with open(str(Path(__file__).parent / "templates" / "discord_chat.py")) as f:
+            app = f.read()
+        app = app.replace("<<app-src>>", self.src)
+        app = app.replace("<<api-name>>", api_names[0][0])
+        app = app.replace("<<command-name>>", api_names[0][1])
+
+        with tempfile.NamedTemporaryFile(mode="w", delete=False) as app_file:
+            with tempfile.NamedTemporaryFile(mode="w", delete=False) as requirements:
+                app_file.write(app)
+                requirements.write("\n".join(["discord.py==2.3.1"]))
+
+        operations = [
+            CommitOperationAdd(path_in_repo="app.py", path_or_fileobj=app_file.name),
+            CommitOperationAdd(
+                path_in_repo="requirements.txt", path_or_fileobj=requirements.name
+            ),
+        ]
+
+        api.create_commit(
+            repo_id=space_id,
+            commit_message="Deploy Discord Bot",
+            repo_type="space",
+            operations=operations,
+            token=hf_token,
+        )
+
+        if discord_bot_token:
+            huggingface_hub.add_space_secret(
+                space_id, "DISCORD_TOKEN", discord_bot_token, token=hf_token
+            )
+        if is_private:
+            huggingface_hub.add_space_secret(
+                space_id, "HF_TOKEN", hf_token, token=hf_token
+            )
+
+        url = f"https://huggingface.co/spaces/{space_id}"
+        print(f"See your discord bot here! {url}")
+        return url
+
 
 class Endpoint:
     """Helper class for storing all the information about a single API endpoint."""
 
     def __init__(self, client: Client, fn_index: int, dependency: dict):
         self.client: Client = client
         self.fn_index = fn_index
@@ -771,29 +913,29 @@
     def insert_state(self, *data) -> tuple:
         data = list(data)
         for i, input_component_type in enumerate(self.input_component_types):
             if input_component_type == utils.STATE_COMPONENT:
                 data.insert(i, None)
         return tuple(data)
 
-    def remove_state(self, *data) -> tuple:
+    def remove_skipped_components(self, *data) -> tuple:
         data = [
             d
             for d, oct in zip(data, self.output_component_types)
-            if oct != utils.STATE_COMPONENT
+            if oct not in utils.SKIP_COMPONENTS
         ]
         return tuple(data)
 
     def reduce_singleton_output(self, *data) -> Any:
         if (
             len(
                 [
                     oct
                     for oct in self.output_component_types
-                    if oct != utils.STATE_COMPONENT
+                    if oct not in utils.SKIP_COMPONENTS
                 ]
             )
             == 1
         ):
             return data[0]
         else:
             return data
@@ -830,15 +972,15 @@
             ]
         )
         return outputs
 
     def process_predictions(self, *predictions):
         if self.client.serialize:
             predictions = self.deserialize(*predictions)
-        predictions = self.remove_state(*predictions)
+        predictions = self.remove_skipped_components(*predictions)
         predictions = self.reduce_singleton_output(*predictions)
         return predictions
 
     def _setup_serializers(self) -> tuple[list[Serializable], list[Serializable]]:
         inputs = self.dependency["inputs"]
         serializers = []
 
@@ -869,14 +1011,16 @@
                     self.output_component_types.append(component_name)
                     if component.get("serializer"):
                         serializer_name = component["serializer"]
                         assert (
                             serializer_name in serializing.SERIALIZER_MAPPING
                         ), f"Unknown serializer: {serializer_name}, you may need to update your gradio_client version."
                         deserializer = serializing.SERIALIZER_MAPPING[serializer_name]
+                    elif component_name in utils.SKIP_COMPONENTS:
+                        deserializer = serializing.SimpleSerializable
                     else:
                         assert (
                             component_name in serializing.COMPONENT_MAPPING
                         ), f"Unknown component: {component_name}, you may need to update your gradio_client version."
                         deserializer = serializing.COMPONENT_MAPPING[component_name]
                     deserializers.append(deserializer())  # type: ignore
```

### Comparing `gradio_client-0.2.9/gradio_client/documentation.py` & `gradio_client-0.3.0/gradio_client/documentation.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.9/gradio_client/media_data.py` & `gradio_client-0.3.0/gradio_client/media_data.py`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.9/gradio_client/serializing.py` & `gradio_client-0.3.0/gradio_client/serializing.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,12 +539,10 @@
     "chatbot": JSONSerializable,
     "model3d": FileSerializable,
     "plot": JSONSerializable,
     "barplot": JSONSerializable,
     "lineplot": JSONSerializable,
     "scatterplot": JSONSerializable,
     "markdown": StringSerializable,
-    "dataset": StringSerializable,
     "code": StringSerializable,
-    "interpretation": SimpleSerializable,
     "annotatedimage": JSONSerializable,
 }
```

### Comparing `gradio_client-0.2.9/gradio_client/types.json` & `gradio_client-0.3.0/gradio_client/types.json`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.9/gradio_client/utils.py` & `gradio_client-0.3.0/gradio_client/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,28 @@
 CONFIG_URL = "config"
 API_INFO_URL = "info"
 RAW_API_INFO_URL = "info?serialize=False"
 SPACE_FETCHER_URL = "https://gradio-space-api-fetcher-v2.hf.space/api"
 RESET_URL = "reset"
 SPACE_URL = "https://hf.space/{}"
 
+SKIP_COMPONENTS = {
+    "state",
+    "row",
+    "column",
+    "tabs",
+    "tab",
+    "tabitem",
+    "box",
+    "form",
+    "accordion",
+    "group",
+    "interpretation",
+    "dataset",
+}
 STATE_COMPONENT = "state"
 INVALID_RUNTIME = [
     SpaceStage.NO_APP_FILE,
     SpaceStage.CONFIG_ERROR,
     SpaceStage.BUILD_ERROR,
     SpaceStage.RUNTIME_ERROR,
     SpaceStage.PAUSED,
```

### Comparing `gradio_client-0.2.9/.gitignore` & `gradio_client-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gradio_client-0.2.9/pyproject.toml` & `gradio_client-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -60,7 +60,11 @@
 [tool.ruff]
 extend = "../../pyproject.toml"
 
 [tool.ruff.isort]
 known-first-party = [
   "gradio_client"
 ]
+
+[tool.pytest.ini_options]
+GRADIO_ANALYTICS_ENABLED = "False"
+HF_HUB_DISABLE_TELEMETRY =  "1"
```

### Comparing `gradio_client-0.2.9/PKG-INFO` & `gradio_client-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_client
-Version: 0.2.9
+Version: 0.3.0
 Summary: Python library for easily interacting with trained machine learning models
 Project-URL: Homepage, https://github.com/gradio-app/gradio
 Author-email: Abubakar Abid <team@gradio.app>, Ali Abid <team@gradio.app>, Ali Abdalla <team@gradio.app>, Dawood Khan <team@gradio.app>, Ahsen Khaliq <team@gradio.app>, Pete Allen <team@gradio.app>, Freddy Boulton <team@gradio.app>
 License-Expression: Apache-2.0
 Keywords: API,client,machine learning
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
@@ -19,17 +19,17 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: User Interfaces
 Requires-Python: >=3.8
 Requires-Dist: fsspec
 Requires-Dist: httpx
 Requires-Dist: huggingface-hub>=0.13.0
 Requires-Dist: packaging
-Requires-Dist: requests
-Requires-Dist: typing-extensions
-Requires-Dist: websockets
+Requires-Dist: requests~=2.0
+Requires-Dist: typing-extensions~=4.0
+Requires-Dist: websockets<12.0,>=10.0
 Description-Content-Type: text/markdown
 
 # `gradio_client`: Use a Gradio app as an API -- in 3 lines of Python
 
 This directory contains the source code for `gradio_client`, a lightweight Python library that makes it very easy to use any Gradio app as an API. 
 
 As an example, consider this [Hugging Face Space that transcribes audio files](https://huggingface.co/spaces/abidlabs/whisper) that are recorded from the microphone.
```

