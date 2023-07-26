# Comparing `tmp/noteable_origami-1.0.0a1.tar.gz` & `tmp/noteable_origami-1.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noteable_origami-1.0.0a1.tar", max compression
+gzip compressed data, was "noteable_origami-1.0.0a2.tar", max compression
```

## Comparing `noteable_origami-1.0.0a1.tar` & `noteable_origami-1.0.0a2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1516 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/LICENSE
--rw-r--r--   0        0        0     4589 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/README.md
--rw-r--r--   0        0        0       82 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/clients/__init__.py
--rw-r--r--   0        0        0    14228 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/clients/api.py
--rw-r--r--   0        0        0        0 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/clients/cache.py
--rw-r--r--   0        0        0    39670 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/clients/rtu.py
--rw-r--r--   0        0        0        0 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 13:13:34.274535 noteable_origami-1.0.0a1/origami/models/api/__init__.py
--rw-r--r--   0        0        0      238 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/base.py
--rw-r--r--   0        0        0      649 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/datasources.py
--rw-r--r--   0        0        0      924 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/files.py
--rw-r--r--   0        0        0      659 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/outputs.py
--rw-r--r--   0        0        0      475 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/projects.py
--rw-r--r--   0        0        0      437 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/spaces.py
--rw-r--r--   0        0        0      681 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/api/users.py
--rw-r--r--   0        0        0        0 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/__init__.py
--rw-r--r--   0        0        0      803 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/base.py
--rw-r--r--   0        0        0      953 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_contents.py
--rw-r--r--   0        0        0     1120 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_execute.py
--rw-r--r--   0        0        0     1222 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_metadata.py
--rw-r--r--   0        0        0      703 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_output_collection.py
--rw-r--r--   0        0        0     1115 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/nb_cells.py
--rw-r--r--   0        0        0      588 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/delta_types/nb_metadata.py
--rw-r--r--   0        0        0      850 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/deltas/discriminators.py
--rw-r--r--   0        0        0      451 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/kernels.py
--rw-r--r--   0        0        0     4010 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/notebook.py
--rw-r--r--   0        0        0        0 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/__init__.py
--rw-r--r--   0        0        0     1520 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/base.py
--rw-r--r--   0        0        0        0 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/channels/__init__.py
--rw-r--r--   0        0        0     7730 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/channels/files.py
--rw-r--r--   0        0        0     2508 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/channels/kernels.py
--rw-r--r--   0        0        0     2640 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/channels/system.py
--rw-r--r--   0        0        0     1210 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/discriminators.py
--rw-r--r--   0        0        0     1073 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/models/rtu/errors.py
--rw-r--r--   0        0        0        0 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/notebook/__init__.py
--rw-r--r--   0        0        0    11988 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/origami/notebook/builder.py
--rw-r--r--   0        0        0     2715 2023-07-25 13:13:34.278535 noteable_origami-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     5898 1970-01-01 00:00:00.000000 noteable_origami-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1516 2023-07-26 14:03:04.509735 noteable_origami-1.0.0a2/LICENSE
+-rw-r--r--   0        0        0     4615 2023-07-26 14:03:04.509735 noteable_origami-1.0.0a2/README.md
+-rw-r--r--   0        0        0       82 2023-07-26 14:03:04.509735 noteable_origami-1.0.0a2/origami/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:03:04.509735 noteable_origami-1.0.0a2/origami/clients/__init__.py
+-rw-r--r--   0        0        0    14644 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/clients/api.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/clients/cache.py
+-rw-r--r--   0        0        0    39670 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/clients/rtu.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/base.py
+-rw-r--r--   0        0        0      649 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/datasources.py
+-rw-r--r--   0        0        0      924 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/files.py
+-rw-r--r--   0        0        0      659 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/outputs.py
+-rw-r--r--   0        0        0      475 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/projects.py
+-rw-r--r--   0        0        0      437 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/spaces.py
+-rw-r--r--   0        0        0      681 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/api/users.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/__init__.py
+-rw-r--r--   0        0        0      803 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/base.py
+-rw-r--r--   0        0        0      953 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_contents.py
+-rw-r--r--   0        0        0     1120 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_execute.py
+-rw-r--r--   0        0        0     1222 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_metadata.py
+-rw-r--r--   0        0        0      703 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_output_collection.py
+-rw-r--r--   0        0        0     1115 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/nb_cells.py
+-rw-r--r--   0        0        0      588 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/delta_types/nb_metadata.py
+-rw-r--r--   0        0        0      850 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/deltas/discriminators.py
+-rw-r--r--   0        0        0      451 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/kernels.py
+-rw-r--r--   0        0        0     4010 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/notebook.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/__init__.py
+-rw-r--r--   0        0        0     1520 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/base.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/channels/__init__.py
+-rw-r--r--   0        0        0     7730 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/channels/files.py
+-rw-r--r--   0        0        0     2508 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/channels/kernels.py
+-rw-r--r--   0        0        0     2640 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/channels/system.py
+-rw-r--r--   0        0        0     1210 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/discriminators.py
+-rw-r--r--   0        0        0     1073 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/models/rtu/errors.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/notebook/__init__.py
+-rw-r--r--   0        0        0    11988 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/origami/notebook/builder.py
+-rw-r--r--   0        0        0     2715 2023-07-26 14:03:04.513735 noteable_origami-1.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     5924 1970-01-01 00:00:00.000000 noteable_origami-1.0.0a2/PKG-INFO
```

### Comparing `noteable_origami-1.0.0a1/LICENSE` & `noteable_origami-1.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/README.md` & `noteable_origami-1.0.0a2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,47 +40,48 @@
 <!-- --8<-- [end:requirements] -->
 
 <!-- --8<-- [start:install] -->
 
 ## Installation
 
 For stable release:
+
 ```bash
 pip install noteable-origami
 ```
 
 ```bash
 poetry add noteable-origami
 ```
 
 For alpha pre-release:
+
 ```bash
 pip install noteable-origami --pre
 ```
 
 <!-- --8<-- [end:install] -->
 
 <!-- --8<-- [start:start] -->
 
 ## Getting Started
 
 > **Warning**
-Developer note: this documentation is written for the 1.0 alpha release. For stable release, see [pre-1.0 README](https://github.com/noteable-io/origami/blob/release/0.0.35/README.md)
-
+> Developer note: this documentation is written for the 1.0 alpha release. For stable release, see [pre-1.0 README](https://github.com/noteable-io/origami/blob/release/0.0.35/README.md)
 
 ### API Tokens
 
 The Noteable API requires an authentication token. You can manage tokens at the Noteable user settings page.
 
 1. Log in to Noteable (sign up is free)
 2. In the User Settings tab, navigate to `API Tokens` and generate a new token
 
 ### Usage
 
-The example below shows how to create a Notebook, launch a Kernel, add new cells, and execute code. 
+The example below shows how to create a Notebook, launch a Kernel, add new cells, and execute code.
 
 ```python
 # Grab a project_id from the Noteable UI, the url will look like: app.noteable.io/p/....
 api_token = '...'
 
 # Client for interacting with Noteables REST API
 from origami.clients.api import APIClient
@@ -95,41 +96,40 @@
 # Create a new Notebook
 file = await api_client.create_notebook(project_id=project_id, path="Demo.ipynb")
 
 # Start a Kernel
 await api_client.launch_kernel(file.id)
 
 # Client for Real-time Updates (RTU), used with Notebooks
-rtu_client = await api_client.rtu_client(file.id)
+realtime_notebook = await api_client.connect_realtime(file)
 
 # Add a new cell
 from origami.models.notebook import CodeCell
 cell = CodeCell(source="print('Hello World')")
-await rtu_client.add_cell(cell)
+await realtime_notebook.add_cell(cell)
 
 # Execute the cell
-queued_execution = await rtu_client.queue_execution(cell.id)
+queued_execution = await realtime_notebook.queue_execution(cell.id)
 
 # Wait for the execution to be complete, cell is an updated instance of CodeCell with metadata/outputs
 cell = await queued_execution
 
 # Grab the output
 output_collection = await api_client.get_output_collection(cell.output_collection_id)
 print(output_collection.outputs[0].content.raw) # 'Hello World\n'
 ```
 
-
 <!-- --8<-- [end:start] -->
 
-
 ## 1.0 Roadmap
 
 Origami is heading towards a 1.0 release. The alpha release candidate is on Pypi now, installable with a `--pre` flag. The 1.0 release represents a major refactor of the Origami using the best practices and lessons learned from creating multiple production API and RTU clients, including our ChatGPT plugin. It will likely come out of alpha once all of our internal applications are using the Origami 1.0 syntax.
 
 ## Contributing
 
 See [CONTRIBUTING.md](./CONTRIBUTING.md).
 
 ---
+
 <p align="center">Open sourced with ❤️ by <a href="https://noteable.io">Noteable</a> for the community.</p>
 
-<img href="https://pages.noteable.io/private-beta-access" src="https://assets.noteable.io/github/2022-07-29/noteable.png" alt="Boost Data Collaboration with Notebooks">
+<img href="https://pages.noteable.io/private-beta-access" src="https://assets.noteable.io/github/2022-07-29/noteable.png" alt="Boost Data Collaboration with Notebooks">
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 ## Intro to Origami Origami is a ð Python library for talking to [Noteable
 notebooks](https://noteable.io/). This is the official way to access the full
 breadth of API calls and access patterns in async Python for rich programmatic
 access to notebooks. You can use [Noteable for free](https://app.noteable.io)
 with a quick signup.   ## Requirements Python 3.8+   ## Installation For stable
 release: ```bash pip install noteable-origami ``` ```bash poetry add noteable-
 origami ``` For alpha pre-release: ```bash pip install noteable-origami --pre
-```   ## Getting Started > **Warning** Developer note: this documentation is
+```   ## Getting Started > **Warning** > Developer note: this documentation is
 written for the 1.0 alpha release. For stable release, see [pre-1.0 README]
 (https://github.com/noteable-io/origami/blob/release/0.0.35/README.md) ### API
 Tokens The Noteable API requires an authentication token. You can manage tokens
 at the Noteable user settings page. 1. Log in to Noteable (sign up is free) 2.
 In the User Settings tab, navigate to `API Tokens` and generate a new token ###
 Usage The example below shows how to create a Notebook, launch a Kernel, add
 new cells, and execute code. ```python # Grab a project_id from the Noteable
@@ -25,24 +25,25 @@
 for interacting with Noteables REST API from origami.clients.api import
 APIClient api_client = APIClient(api_token) # Sanity check your user
 information user = await api_client.user_info() # Choose a project to create
 the notebook in, here using the ChatGPT plugin default project project_id =
 user.origamist_default_project_id # Create a new Notebook file = await
 api_client.create_notebook(project_id=project_id, path="Demo.ipynb") # Start a
 Kernel await api_client.launch_kernel(file.id) # Client for Real-time Updates
-(RTU), used with Notebooks rtu_client = await api_client.rtu_client(file.id) #
-Add a new cell from origami.models.notebook import CodeCell cell = CodeCell
-(source="print('Hello World')") await rtu_client.add_cell(cell) # Execute the
-cell queued_execution = await rtu_client.queue_execution(cell.id) # Wait for
-the execution to be complete, cell is an updated instance of CodeCell with
-metadata/outputs cell = await queued_execution # Grab the output
-output_collection = await api_client.get_output_collection
-(cell.output_collection_id) print(output_collection.outputs[0].content.raw) #
-'Hello World\n' ```  ## 1.0 Roadmap Origami is heading towards a 1.0 release.
-The alpha release candidate is on Pypi now, installable with a `--pre` flag.
-The 1.0 release represents a major refactor of the Origami using the best
-practices and lessons learned from creating multiple production API and RTU
-clients, including our ChatGPT plugin. It will likely come out of alpha once
-all of our internal applications are using the Origami 1.0 syntax. ##
-Contributing See [CONTRIBUTING.md](./CONTRIBUTING.md). ---
+(RTU), used with Notebooks realtime_notebook = await
+api_client.connect_realtime(file) # Add a new cell from origami.models.notebook
+import CodeCell cell = CodeCell(source="print('Hello World')") await
+realtime_notebook.add_cell(cell) # Execute the cell queued_execution = await
+realtime_notebook.queue_execution(cell.id) # Wait for the execution to be
+complete, cell is an updated instance of CodeCell with metadata/outputs cell =
+await queued_execution # Grab the output output_collection = await
+api_client.get_output_collection(cell.output_collection_id) print
+(output_collection.outputs[0].content.raw) # 'Hello World\n' ```  ## 1.0
+Roadmap Origami is heading towards a 1.0 release. The alpha release candidate
+is on Pypi now, installable with a `--pre` flag. The 1.0 release represents a
+major refactor of the Origami using the best practices and lessons learned from
+creating multiple production API and RTU clients, including our ChatGPT plugin.
+It will likely come out of alpha once all of our internal applications are
+using the Origami 1.0 syntax. ## Contributing See [CONTRIBUTING.md](./
+CONTRIBUTING.md). ---
             Open sourced with â¤ï¸ by Noteable for the community.
 [Boost Data Collaboration with Notebooks]
```

### Comparing `noteable_origami-1.0.0a1/origami/clients/api.py` & `noteable_origami-1.0.0a2/origami/clients/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import os
 import uuid
-from typing import List, Literal, Optional
+from typing import List, Literal, Optional, Union
 
 import httpx
 import pydantic
 
 from origami.clients.rtu import RTUClient
 from origami.models.api.datasources import DataSource
 from origami.models.api.files import File
@@ -280,22 +280,35 @@
         self, output_collection_id: uuid.UUID
     ) -> KernelOutputCollection:
         endpoint = f'/outputs/collection/{output_collection_id}'
         resp = await self.client.get(endpoint)
         resp.raise_for_status()
         return KernelOutputCollection.parse_obj(resp.json())
 
-    async def rtu_client(self, file_id: uuid.UUID) -> RTUClient:
+    async def connect_realtime(self, file: Union[File, uuid.UUID, str]) -> RTUClient:
         """
         Create an RTUClient for a Notebook by file id. This will perform the following steps:
          - Check /v1/files to get the current version information and presigned download url
          - Download seed notebook and create a NotebookBuilder from it
          - Create an RTUClient, initialize the websocket connection, authenticate, and subscribe
          - Apply delts to in-memory NotebookBuilder
         """
+        file_id = None
+
+        if isinstance(file, str):
+            file_id = uuid.UUID(file)
+        elif isinstance(file, uuid.UUID):
+            file_id = file
+        elif isinstance(file, File):
+            file_id = file.id
+        else:
+            raise ValueError(f"Must provide a `file_id` or a File, not {file}")
+
+        self.add_tags_and_contextvars(file_id=str(file_id))
+
         logger.info(f"Creating RTUClient for file {file_id}")
         file = await self.get_file(file_id)
         if file.type != 'notebook':
             raise ValueError(f"File {file_id} is not a notebook")
         if not file.presigned_download_url:
             raise ValueError(f"File {file_id} does not have a presigned download url")
         # TODO: remove this hack if/when we get containers in Skaffold to be able to translate
```

### Comparing `noteable_origami-1.0.0a1/origami/clients/rtu.py` & `noteable_origami-1.0.0a2/origami/clients/rtu.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/api/datasources.py` & `noteable_origami-1.0.0a2/origami/models/api/datasources.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/api/files.py` & `noteable_origami-1.0.0a2/origami/models/api/files.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/api/outputs.py` & `noteable_origami-1.0.0a2/origami/models/api/outputs.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/api/users.py` & `noteable_origami-1.0.0a2/origami/models/api/users.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/deltas/base.py` & `noteable_origami-1.0.0a2/origami/models/deltas/base.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_contents.py` & `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_contents.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_execute.py` & `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_execute.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_metadata.py` & `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_metadata.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/deltas/delta_types/cell_output_collection.py` & `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/cell_output_collection.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/deltas/delta_types/nb_cells.py` & `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/nb_cells.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/deltas/delta_types/nb_metadata.py` & `noteable_origami-1.0.0a2/origami/models/deltas/delta_types/nb_metadata.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/deltas/discriminators.py` & `noteable_origami-1.0.0a2/origami/models/deltas/discriminators.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/notebook.py` & `noteable_origami-1.0.0a2/origami/models/notebook.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/rtu/base.py` & `noteable_origami-1.0.0a2/origami/models/rtu/base.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/rtu/channels/files.py` & `noteable_origami-1.0.0a2/origami/models/rtu/channels/files.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/rtu/channels/kernels.py` & `noteable_origami-1.0.0a2/origami/models/rtu/channels/kernels.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/rtu/channels/system.py` & `noteable_origami-1.0.0a2/origami/models/rtu/channels/system.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/rtu/discriminators.py` & `noteable_origami-1.0.0a2/origami/models/rtu/discriminators.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/models/rtu/errors.py` & `noteable_origami-1.0.0a2/origami/models/rtu/errors.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/origami/notebook/builder.py` & `noteable_origami-1.0.0a2/origami/notebook/builder.py`

 * *Files identical despite different names*

### Comparing `noteable_origami-1.0.0a1/pyproject.toml` & `noteable_origami-1.0.0a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.poetry]
 name = "noteable-origami"
-version = "1.0.0-alpha.1"
+version = "1.0.0-alpha.2"
 description = "The Noteable API interface"
 authors = ["Matt Seal <matt@noteable.io>"]
 maintainers = ["Matt Seal <matt@noteable.io>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://github.com/noteable-io/origami"
 # old setup.cfg had a bdist_wheel option.
```

### Comparing `noteable_origami-1.0.0a1/PKG-INFO` & `noteable_origami-1.0.0a2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noteable-origami
-Version: 1.0.0a1
+Version: 1.0.0a2
 Summary: The Noteable API interface
 Home-page: https://github.com/noteable-io/origami
 License: BSD-3-Clause
 Keywords: notebook,api,noteable
 Author: Matt Seal
 Author-email: matt@noteable.io
 Maintainer: Matt Seal
@@ -75,47 +75,48 @@
 <!-- --8<-- [end:requirements] -->
 
 <!-- --8<-- [start:install] -->
 
 ## Installation
 
 For stable release:
+
 ```bash
 pip install noteable-origami
 ```
 
 ```bash
 poetry add noteable-origami
 ```
 
 For alpha pre-release:
+
 ```bash
 pip install noteable-origami --pre
 ```
 
 <!-- --8<-- [end:install] -->
 
 <!-- --8<-- [start:start] -->
 
 ## Getting Started
 
 > **Warning**
-Developer note: this documentation is written for the 1.0 alpha release. For stable release, see [pre-1.0 README](https://github.com/noteable-io/origami/blob/release/0.0.35/README.md)
-
+> Developer note: this documentation is written for the 1.0 alpha release. For stable release, see [pre-1.0 README](https://github.com/noteable-io/origami/blob/release/0.0.35/README.md)
 
 ### API Tokens
 
 The Noteable API requires an authentication token. You can manage tokens at the Noteable user settings page.
 
 1. Log in to Noteable (sign up is free)
 2. In the User Settings tab, navigate to `API Tokens` and generate a new token
 
 ### Usage
 
-The example below shows how to create a Notebook, launch a Kernel, add new cells, and execute code. 
+The example below shows how to create a Notebook, launch a Kernel, add new cells, and execute code.
 
 ```python
 # Grab a project_id from the Noteable UI, the url will look like: app.noteable.io/p/....
 api_token = '...'
 
 # Client for interacting with Noteables REST API
 from origami.clients.api import APIClient
@@ -130,41 +131,41 @@
 # Create a new Notebook
 file = await api_client.create_notebook(project_id=project_id, path="Demo.ipynb")
 
 # Start a Kernel
 await api_client.launch_kernel(file.id)
 
 # Client for Real-time Updates (RTU), used with Notebooks
-rtu_client = await api_client.rtu_client(file.id)
+realtime_notebook = await api_client.connect_realtime(file)
 
 # Add a new cell
 from origami.models.notebook import CodeCell
 cell = CodeCell(source="print('Hello World')")
-await rtu_client.add_cell(cell)
+await realtime_notebook.add_cell(cell)
 
 # Execute the cell
-queued_execution = await rtu_client.queue_execution(cell.id)
+queued_execution = await realtime_notebook.queue_execution(cell.id)
 
 # Wait for the execution to be complete, cell is an updated instance of CodeCell with metadata/outputs
 cell = await queued_execution
 
 # Grab the output
 output_collection = await api_client.get_output_collection(cell.output_collection_id)
 print(output_collection.outputs[0].content.raw) # 'Hello World\n'
 ```
 
-
 <!-- --8<-- [end:start] -->
 
-
 ## 1.0 Roadmap
 
 Origami is heading towards a 1.0 release. The alpha release candidate is on Pypi now, installable with a `--pre` flag. The 1.0 release represents a major refactor of the Origami using the best practices and lessons learned from creating multiple production API and RTU clients, including our ChatGPT plugin. It will likely come out of alpha once all of our internal applications are using the Origami 1.0 syntax.
 
 ## Contributing
 
 See [CONTRIBUTING.md](./CONTRIBUTING.md).
 
 ---
+
 <p align="center">Open sourced with ❤️ by <a href="https://noteable.io">Noteable</a> for the community.</p>
 
 <img href="https://pages.noteable.io/private-beta-access" src="https://assets.noteable.io/github/2022-07-29/noteable.png" alt="Boost Data Collaboration with Notebooks">
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: noteable-origami Version: 1.0.0a1 Summary: The
+Metadata-Version: 2.1 Name: noteable-origami Version: 1.0.0a2 Summary: The
 Noteable API interface Home-page: https://github.com/noteable-io/origami
 License: BSD-3-Clause Keywords: notebook,api,noteable Author: Matt Seal Author-
 email: matt@noteable.io Maintainer: Matt Seal Maintainer-email:
 matt@noteable.io Requires-Python: >=3.8,<4.0 Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
@@ -26,15 +26,15 @@
 ## Intro to Origami Origami is a ð Python library for talking to [Noteable
 notebooks](https://noteable.io/). This is the official way to access the full
 breadth of API calls and access patterns in async Python for rich programmatic
 access to notebooks. You can use [Noteable for free](https://app.noteable.io)
 with a quick signup.   ## Requirements Python 3.8+   ## Installation For stable
 release: ```bash pip install noteable-origami ``` ```bash poetry add noteable-
 origami ``` For alpha pre-release: ```bash pip install noteable-origami --pre
-```   ## Getting Started > **Warning** Developer note: this documentation is
+```   ## Getting Started > **Warning** > Developer note: this documentation is
 written for the 1.0 alpha release. For stable release, see [pre-1.0 README]
 (https://github.com/noteable-io/origami/blob/release/0.0.35/README.md) ### API
 Tokens The Noteable API requires an authentication token. You can manage tokens
 at the Noteable user settings page. 1. Log in to Noteable (sign up is free) 2.
 In the User Settings tab, navigate to `API Tokens` and generate a new token ###
 Usage The example below shows how to create a Notebook, launch a Kernel, add
 new cells, and execute code. ```python # Grab a project_id from the Noteable
@@ -42,24 +42,25 @@
 for interacting with Noteables REST API from origami.clients.api import
 APIClient api_client = APIClient(api_token) # Sanity check your user
 information user = await api_client.user_info() # Choose a project to create
 the notebook in, here using the ChatGPT plugin default project project_id =
 user.origamist_default_project_id # Create a new Notebook file = await
 api_client.create_notebook(project_id=project_id, path="Demo.ipynb") # Start a
 Kernel await api_client.launch_kernel(file.id) # Client for Real-time Updates
-(RTU), used with Notebooks rtu_client = await api_client.rtu_client(file.id) #
-Add a new cell from origami.models.notebook import CodeCell cell = CodeCell
-(source="print('Hello World')") await rtu_client.add_cell(cell) # Execute the
-cell queued_execution = await rtu_client.queue_execution(cell.id) # Wait for
-the execution to be complete, cell is an updated instance of CodeCell with
-metadata/outputs cell = await queued_execution # Grab the output
-output_collection = await api_client.get_output_collection
-(cell.output_collection_id) print(output_collection.outputs[0].content.raw) #
-'Hello World\n' ```  ## 1.0 Roadmap Origami is heading towards a 1.0 release.
-The alpha release candidate is on Pypi now, installable with a `--pre` flag.
-The 1.0 release represents a major refactor of the Origami using the best
-practices and lessons learned from creating multiple production API and RTU
-clients, including our ChatGPT plugin. It will likely come out of alpha once
-all of our internal applications are using the Origami 1.0 syntax. ##
-Contributing See [CONTRIBUTING.md](./CONTRIBUTING.md). ---
+(RTU), used with Notebooks realtime_notebook = await
+api_client.connect_realtime(file) # Add a new cell from origami.models.notebook
+import CodeCell cell = CodeCell(source="print('Hello World')") await
+realtime_notebook.add_cell(cell) # Execute the cell queued_execution = await
+realtime_notebook.queue_execution(cell.id) # Wait for the execution to be
+complete, cell is an updated instance of CodeCell with metadata/outputs cell =
+await queued_execution # Grab the output output_collection = await
+api_client.get_output_collection(cell.output_collection_id) print
+(output_collection.outputs[0].content.raw) # 'Hello World\n' ```  ## 1.0
+Roadmap Origami is heading towards a 1.0 release. The alpha release candidate
+is on Pypi now, installable with a `--pre` flag. The 1.0 release represents a
+major refactor of the Origami using the best practices and lessons learned from
+creating multiple production API and RTU clients, including our ChatGPT plugin.
+It will likely come out of alpha once all of our internal applications are
+using the Origami 1.0 syntax. ## Contributing See [CONTRIBUTING.md](./
+CONTRIBUTING.md). ---
             Open sourced with â¤ï¸ by Noteable for the community.
 [Boost Data Collaboration with Notebooks]
```

