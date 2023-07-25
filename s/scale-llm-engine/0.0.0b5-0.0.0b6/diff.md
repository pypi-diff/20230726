# Comparing `tmp/scale_llm_engine-0.0.0b5.tar.gz` & `tmp/scale_llm_engine-0.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0b5.tar", max compression
+gzip compressed data, was "scale_llm_engine-0.0.0b6.tar", max compression
```

## Comparing `scale_llm_engine-0.0.0b5.tar` & `scale_llm_engine-0.0.0b6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1002 2023-07-19 01:36:28.535119 scale_llm_engine-0.0.0b5/README.md
--rw-r--r--   0        0        0     1576 2023-07-21 01:19:40.651366 scale_llm_engine-0.0.0b5/llmengine/__init__.py
--rw-r--r--   0        0        0     6190 2023-07-19 23:57:12.780752 scale_llm_engine-0.0.0b5/llmengine/api_engine.py
--rw-r--r--   0        0        0    13065 2023-07-19 01:36:28.535834 scale_llm_engine-0.0.0b5/llmengine/completion.py
--rw-r--r--   0        0        0    13457 2023-07-20 18:43:29.437750 scale_llm_engine-0.0.0b5/llmengine/data_types.py
--rw-r--r--   0        0        0     2745 2023-07-16 23:34:18.820164 scale_llm_engine-0.0.0b5/llmengine/errors.py
--rw-r--r--   0        0        0    14021 2023-07-20 18:43:29.438456 scale_llm_engine-0.0.0b5/llmengine/fine_tuning.py
--rw-r--r--   0        0        0    13738 2023-07-19 17:53:11.210172 scale_llm_engine-0.0.0b5/llmengine/model.py
--rw-r--r--   0        0        0      807 2023-07-21 01:19:40.652418 scale_llm_engine-0.0.0b5/pyproject.toml
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/README.md
+-rw-r--r--   0        0        0     1576 2023-07-25 22:38:19.836819 scale_llm_engine-0.0.0b6/llmengine/__init__.py
+-rw-r--r--   0        0        0     6190 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/llmengine/api_engine.py
+-rw-r--r--   0        0        0    13065 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/llmengine/completion.py
+-rw-r--r--   0        0        0    13437 2023-07-25 22:38:19.836819 scale_llm_engine-0.0.0b6/llmengine/data_types.py
+-rw-r--r--   0        0        0     2745 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/llmengine/errors.py
+-rw-r--r--   0        0        0    14021 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/llmengine/fine_tuning.py
+-rw-r--r--   0        0        0    13738 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/llmengine/model.py
+-rw-r--r--   0        0        0      807 2023-07-25 22:38:19.836819 scale_llm_engine-0.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b6/PKG-INFO
```

### Comparing `scale_llm_engine-0.0.0b5/README.md` & `scale_llm_engine-0.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b5/llmengine/__init__.py` & `scale_llm_engine-0.0.0b6/llmengine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.0.beta5"
+__version__ = "0.0.0.beta6"
 
 from typing import Sequence
 
 from llmengine.completion import Completion
 from llmengine.data_types import (
     CancelFineTuneResponse,
     CompletionOutput,
```

### Comparing `scale_llm_engine-0.0.0b5/llmengine/api_engine.py` & `scale_llm_engine-0.0.0b6/llmengine/api_engine.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b5/llmengine/completion.py` & `scale_llm_engine-0.0.0b6/llmengine/completion.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b5/llmengine/data_types.py` & `scale_llm_engine-0.0.0b6/llmengine/data_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 
 
 class CreateFineTuneResponse(BaseModel):
     """
     Response object for creating a FineTune.
     """
 
-    fine_tune_id: str = Field(..., description="ID of the created fine-tuning job.")
+    id: str = Field(..., description="ID of the created fine-tuning job.")
     """
     The ID of the FineTune.
     """
 
 
 class BatchJobStatus(str, Enum):
     PENDING = "PENDING"
@@ -372,15 +372,15 @@
 
 
 class GetFineTuneResponse(BaseModel):
     """
     Response object for retrieving a FineTune.
     """
 
-    fine_tune_id: str = Field(..., description="ID of the requested job.")
+    id: str = Field(..., description="ID of the requested job.")
     """
     The ID of the FineTune.
     """
 
     fine_tuned_model: Optional[str] = Field(
         default=None,
         description="Name of the resulting fine-tuned model. This can be plugged into the "
```

### Comparing `scale_llm_engine-0.0.0b5/llmengine/errors.py` & `scale_llm_engine-0.0.0b6/llmengine/errors.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b5/llmengine/fine_tuning.py` & `scale_llm_engine-0.0.0b6/llmengine/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b5/llmengine/model.py` & `scale_llm_engine-0.0.0b6/llmengine/model.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b5/pyproject.toml` & `scale_llm_engine-0.0.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale-llm-engine"
-version = "0.0.0.beta5"
+version = "0.0.0.beta6"
 description = "Scale LLM Engine Python client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/llm-engine/"
 repository = "https://github.com/scaleapi/llm-engine"
```

### Comparing `scale_llm_engine-0.0.0b5/PKG-INFO` & `scale_llm_engine-0.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-llm-engine
-Version: 0.0.0b5
+Version: 0.0.0b6
 Summary: Scale LLM Engine Python client
 Home-page: https://scaleapi.github.io/llm-engine/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
```

