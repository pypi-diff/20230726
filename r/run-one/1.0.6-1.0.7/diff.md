# Comparing `tmp/run_one-1.0.6.tar.gz` & `tmp/run_one-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_one-1.0.6.tar", max compression
+gzip compressed data, was "run_one-1.0.7.tar", max compression
```

## Comparing `run_one-1.0.6.tar` & `run_one-1.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-07-26 12:59:01.279157 run_one-1.0.6/LICENSE
--rw-r--r--   0        0        0     1708 2023-07-26 12:59:01.279157 run_one-1.0.6/README.md
--rw-r--r--   0        0        0      740 2023-07-26 12:59:01.279157 run_one-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      345 2023-07-26 12:59:01.279157 run_one-1.0.6/run_one/__init__.py
--rw-r--r--   0        0        0      282 2023-07-26 12:59:01.279157 run_one-1.0.6/run_one/action_handlers/SleepHandler.py
--rw-r--r--   0        0        0     1916 2023-07-26 12:59:01.279157 run_one-1.0.6/run_one/action_handlers/TH2ActHandler.py
--rw-r--r--   0        0        0     1182 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/action_handlers/TH2ActSSHHandler.py
--rw-r--r--   0        0        0     3391 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/action_handlers/TH2Check1Handler.py
--rw-r--r--   0        0        0        0 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/action_handlers/__init__.py
--rw-r--r--   0        0        0      325 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/action_handlers/abstract_action_handler.py
--rw-r--r--   0        0        0      304 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/action_handlers/context.py
--rw-r--r--   0        0        0        0 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/processors/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/processors/abstract_processor.py
--rw-r--r--   0        0        0     5608 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/processors/th2_processor.py
--rw-r--r--   0        0        0        0 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/util/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/util/config.py
--rw-r--r--   0        0        0     3225 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/util/util.py
--rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 run_one-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 13:29:23.686459 run_one-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1708 2023-07-26 13:29:23.686459 run_one-1.0.7/README.md
+-rw-r--r--   0        0        0      740 2023-07-26 13:29:23.686459 run_one-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      345 2023-07-26 13:29:23.686459 run_one-1.0.7/run_one/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-26 13:29:23.686459 run_one-1.0.7/run_one/action_handlers/SleepHandler.py
+-rw-r--r--   0        0        0     1916 2023-07-26 13:29:23.686459 run_one-1.0.7/run_one/action_handlers/TH2ActHandler.py
+-rw-r--r--   0        0        0     1182 2023-07-26 13:29:23.686459 run_one-1.0.7/run_one/action_handlers/TH2ActSSHHandler.py
+-rw-r--r--   0        0        0     3391 2023-07-26 13:29:23.686459 run_one-1.0.7/run_one/action_handlers/TH2Check1Handler.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:29:23.686459 run_one-1.0.7/run_one/action_handlers/__init__.py
+-rw-r--r--   0        0        0      325 2023-07-26 13:29:23.686459 run_one-1.0.7/run_one/action_handlers/abstract_action_handler.py
+-rw-r--r--   0        0        0      304 2023-07-26 13:29:23.690459 run_one-1.0.7/run_one/action_handlers/context.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:29:23.690459 run_one-1.0.7/run_one/processors/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-26 13:29:23.690459 run_one-1.0.7/run_one/processors/abstract_processor.py
+-rw-r--r--   0        0        0     5618 2023-07-26 13:29:23.690459 run_one-1.0.7/run_one/processors/th2_processor.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:29:23.690459 run_one-1.0.7/run_one/util/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-26 13:29:23.690459 run_one-1.0.7/run_one/util/config.py
+-rw-r--r--   0        0        0     3474 2023-07-26 13:29:23.690459 run_one-1.0.7/run_one/util/util.py
+-rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 run_one-1.0.7/PKG-INFO
```

### Comparing `run_one-1.0.6/LICENSE` & `run_one-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `run_one-1.0.6/README.md` & `run_one-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `run_one-1.0.6/pyproject.toml` & `run_one-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "run-one"
-version = "1.0.6"
+version = "1.0.7"
 description = "Tool for parsing matrix files, extracting actions and processing them according to user defined logic"
 authors = ["TH2-devs <th2-devs@exactprosystems.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/th2-net/run-one"
 repository = "https://github.com/th2-net/run-one"
 packages = [
```

### Comparing `run_one-1.0.6/run_one/action_handlers/TH2ActHandler.py` & `run_one-1.0.7/run_one/action_handlers/TH2ActHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.6/run_one/action_handlers/TH2ActSSHHandler.py` & `run_one-1.0.7/run_one/action_handlers/TH2ActSSHHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.6/run_one/action_handlers/TH2Check1Handler.py` & `run_one-1.0.7/run_one/action_handlers/TH2Check1Handler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.6/run_one/processors/abstract_processor.py` & `run_one-1.0.7/run_one/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.6/run_one/processors/th2_processor.py` & `run_one-1.0.7/run_one/processors/th2_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from th2_common.schema.factory.common_factory import CommonFactory
 from th2_common_utils import create_event, create_event_id
 
 from run_one.action_handlers.abstract_action_handler import AbstractActionHandler
 from run_one.action_handlers.context import Context
 from run_one.processors.abstract_processor import AbstractProcessor
 from run_one.util.config import Config
-from run_one.util.util import Action
+from run_one.util.util import Action, pairwise
 
 
 class Th2ProcessorConfig:
     def __init__(self, **kwargs) -> None:
 
         self.th2_configs = 'th2_configs'
         if 'th2_configs' in kwargs:
```

### Comparing `run_one-1.0.6/run_one/util/config.py` & `run_one-1.0.7/run_one/util/config.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.6/run_one/util/util.py` & `run_one-1.0.7/run_one/util/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 from datetime import datetime
+from itertools import tee
 import json
 from typing import Callable
 import uuid
 
 import pandas as pd
 
 from run_one.util.config import Config
@@ -91,7 +92,17 @@
                 for field in config.regenerate_time_fields:
                     if field in row and row[field] != '*':
                         row[field] = time_mapping.setdefault(row[field], time_function())
 
             result[test_case_name].append(Action(row.to_dict(), extracted_fields.to_dict()))
 
     return result
+
+
+def pairwise(iterable):
+    """
+    Return successive overlapping pairs taken from the input iterable.
+    pairwise('ABCDEFG') --> AB BC CD DE EF FG
+    """
+    a, b = tee(iterable)
+    next(b, None)
+    return zip(a, b)
```

### Comparing `run_one-1.0.6/PKG-INFO` & `run_one-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-one
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tool for parsing matrix files, extracting actions and processing them according to user defined logic
 Home-page: https://github.com/th2-net/run-one
 License: Apache-2.0
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

