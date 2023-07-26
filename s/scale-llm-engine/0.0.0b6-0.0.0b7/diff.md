# Comparing `tmp/scale_llm_engine-0.0.0b6.tar.gz` & `tmp/scale_llm_engine-0.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0b6.tar", max compression
+gzip compressed data, was "scale_llm_engine-0.0.0b7.tar", max compression
```

## Comparing `scale_llm_engine-0.0.0b6.tar` & `scale_llm_engine-0.0.0b7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1002 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/README.md
--rw-r--r--   0        0        0     1576 2023-07-25 22:38:19.836819 scale_llm_engine-0.0.0b6/llmengine/__init__.py
--rw-r--r--   0        0        0     6190 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/llmengine/api_engine.py
--rw-r--r--   0        0        0    13065 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/llmengine/completion.py
--rw-r--r--   0        0        0    13437 2023-07-25 22:38:19.836819 scale_llm_engine-0.0.0b6/llmengine/data_types.py
--rw-r--r--   0        0        0     2745 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/llmengine/errors.py
--rw-r--r--   0        0        0    14021 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/llmengine/fine_tuning.py
--rw-r--r--   0        0        0    13738 2023-07-25 17:51:39.505581 scale_llm_engine-0.0.0b6/llmengine/model.py
--rw-r--r--   0        0        0      807 2023-07-25 22:38:19.836819 scale_llm_engine-0.0.0b6/pyproject.toml
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-07-21 08:53:27.233160 scale_llm_engine-0.0.0b7/README.md
+-rw-r--r--   0        0        0     1576 2023-07-26 17:20:58.423387 scale_llm_engine-0.0.0b7/llmengine/__init__.py
+-rw-r--r--   0        0        0     6201 2023-07-26 17:19:44.533261 scale_llm_engine-0.0.0b7/llmengine/api_engine.py
+-rw-r--r--   0        0        0    13065 2023-07-21 08:53:27.234217 scale_llm_engine-0.0.0b7/llmengine/completion.py
+-rw-r--r--   0        0        0    13437 2023-07-26 17:19:44.533815 scale_llm_engine-0.0.0b7/llmengine/data_types.py
+-rw-r--r--   0        0        0     2745 2023-07-18 18:23:40.550782 scale_llm_engine-0.0.0b7/llmengine/errors.py
+-rw-r--r--   0        0        0    14021 2023-07-21 08:53:27.235057 scale_llm_engine-0.0.0b7/llmengine/fine_tuning.py
+-rw-r--r--   0        0        0    13738 2023-07-21 08:53:27.235405 scale_llm_engine-0.0.0b7/llmengine/model.py
+-rw-r--r--   0        0        0      807 2023-07-26 17:20:58.407050 scale_llm_engine-0.0.0b7/pyproject.toml
+-rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b7/PKG-INFO
```

### Comparing `scale_llm_engine-0.0.0b6/README.md` & `scale_llm_engine-0.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b6/llmengine/__init__.py` & `scale_llm_engine-0.0.0b7/llmengine/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.0.beta6"
+__version__ = "0.0.0.beta7"
 
 from typing import Sequence
 
 from llmengine.completion import Completion
 from llmengine.data_types import (
     CancelFineTuneResponse,
     CompletionOutput,
```

### Comparing `scale_llm_engine-0.0.0b6/llmengine/api_engine.py` & `scale_llm_engine-0.0.0b7/llmengine/api_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import wraps
 from typing import Any, AsyncIterable, Dict, Iterator, Optional
 
 import requests
 from aiohttp import ClientSession, ClientTimeout
 from llmengine.errors import parse_error
 
-SPELLBOOK_API_URL = "https://api.spellbook.scale.com"
+SPELLBOOK_API_URL = "https://api.spellbook.scale.com/llm-engine"
 LLM_ENGINE_BASE_PATH = os.getenv("LLM_ENGINE_BASE_PATH", SPELLBOOK_API_URL)
 DEFAULT_TIMEOUT: int = 10
 
 
 def get_api_key() -> str:
     env_api_key = os.getenv("SCALE_API_KEY")
     return env_api_key or "root"
```

### Comparing `scale_llm_engine-0.0.0b6/llmengine/completion.py` & `scale_llm_engine-0.0.0b7/llmengine/completion.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b6/llmengine/data_types.py` & `scale_llm_engine-0.0.0b7/llmengine/data_types.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b6/llmengine/errors.py` & `scale_llm_engine-0.0.0b7/llmengine/errors.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b6/llmengine/fine_tuning.py` & `scale_llm_engine-0.0.0b7/llmengine/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b6/llmengine/model.py` & `scale_llm_engine-0.0.0b7/llmengine/model.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b6/pyproject.toml` & `scale_llm_engine-0.0.0b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale-llm-engine"
-version = "0.0.0.beta6"
+version = "0.0.0.beta7"
 description = "Scale LLM Engine Python client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/llm-engine/"
 repository = "https://github.com/scaleapi/llm-engine"
```

### Comparing `scale_llm_engine-0.0.0b6/PKG-INFO` & `scale_llm_engine-0.0.0b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-llm-engine
-Version: 0.0.0b6
+Version: 0.0.0b7
 Summary: Scale LLM Engine Python client
 Home-page: https://scaleapi.github.io/llm-engine/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
```

