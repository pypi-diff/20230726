# Comparing `tmp/tensor_parallel-1.3.0.tar.gz` & `tmp/tensor_parallel-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensor_parallel-1.3.0.tar", last modified: Sat Jul 22 12:02:22 2023, max compression
+gzip compressed data, was "tensor_parallel-1.3.1.tar", last modified: Wed Jul 26 18:49:17 2023, max compression
```

## Comparing `tensor_parallel-1.3.0.tar` & `tensor_parallel-1.3.1.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:02:22.628743 tensor_parallel-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-22 12:02:22.628743 tensor_parallel-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-22 12:02:22.628743 tensor_parallel-1.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:02:22.624743 tensor_parallel-1.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:02:22.624743 tensor_parallel-1.3.0/src/tensor_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/autoconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/aux_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/communications.py
--rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/cross_device_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/per_device_tensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/pretrained_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/shard.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/sharding.py
--rw-r--r--   0 runner    (1001) docker     (123)    22088 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/slicing_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/state_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/tensor_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/src/tensor_parallel/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:02:22.624743 tensor_parallel-1.3.0/src/tensor_parallel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-22 12:02:22.000000 tensor_parallel-1.3.0/src/tensor_parallel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-22 12:02:22.000000 tensor_parallel-1.3.0/src/tensor_parallel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 12:02:22.000000 tensor_parallel-1.3.0/src/tensor_parallel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-22 12:02:22.000000 tensor_parallel-1.3.0/src/tensor_parallel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-22 12:02:22.000000 tensor_parallel-1.3.0/src/tensor_parallel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 12:02:22.628743 tensor_parallel-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-07-22 12:02:08.000000 tensor_parallel-1.3.0/tests/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:49:17.597106 tensor_parallel-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-26 18:49:17.597106 tensor_parallel-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-26 18:49:17.597106 tensor_parallel-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:49:17.593106 tensor_parallel-1.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:49:17.597106 tensor_parallel-1.3.1/src/tensor_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/autoconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/aux_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/communications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4504 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/cross_device_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/per_device_tensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/pretrained_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/sharding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22131 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/slicing_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/state_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/tensor_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/src/tensor_parallel/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:49:17.597106 tensor_parallel-1.3.1/src/tensor_parallel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-26 18:49:17.000000 tensor_parallel-1.3.1/src/tensor_parallel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-07-26 18:49:17.000000 tensor_parallel-1.3.1/src/tensor_parallel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 18:49:17.000000 tensor_parallel-1.3.1/src/tensor_parallel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-26 18:49:17.000000 tensor_parallel-1.3.1/src/tensor_parallel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-26 18:49:17.000000 tensor_parallel-1.3.1/src/tensor_parallel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 18:49:17.597106 tensor_parallel-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-07-26 18:49:06.000000 tensor_parallel-1.3.1/tests/test_transformers.py
```

### Comparing `tensor_parallel-1.3.0/LICENCE` & `tensor_parallel-1.3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/PKG-INFO` & `tensor_parallel-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor_parallel
-Version: 1.3.0
+Version: 1.3.1
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor_parallel Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: tensor_parallel Version: 1.3.1 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.3.0/README.md` & `tensor_parallel-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/setup.cfg` & `tensor_parallel-1.3.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tensor_parallel
-version = 1.3.0
+version = 1.3.1
 author = Andrei Panferov and Yaroslav Lisnyak
 author_email = yalisnyak@nes.com
 description = Automatically shard your large model between multiple GPUs, works without torch.distributed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/BlackSamorez/tensor_parallel
 project_urls =
```

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/__init__.py` & `tensor_parallel-1.3.1/src/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/autoconfig.py` & `tensor_parallel-1.3.1/src/tensor_parallel/autoconfig.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/aux_actions.py` & `tensor_parallel-1.3.1/src/tensor_parallel/aux_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/communications.py` & `tensor_parallel-1.3.1/src/tensor_parallel/communications.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/config.py` & `tensor_parallel-1.3.1/src/tensor_parallel/config.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/cross_device_ops.py` & `tensor_parallel-1.3.1/src/tensor_parallel/cross_device_ops.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/dispatch.py` & `tensor_parallel-1.3.1/src/tensor_parallel/dispatch.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/factory.py` & `tensor_parallel-1.3.1/src/tensor_parallel/factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/per_device_tensors.py` & `tensor_parallel-1.3.1/src/tensor_parallel/per_device_tensors.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/pretrained_model.py` & `tensor_parallel-1.3.1/src/tensor_parallel/pretrained_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 
 def find_predefined_tensor_parallel_config(
     model_config: PretrainedConfig, device_ids: Optional[Sequence[torch.device]]
 ) -> Optional[Config]:
     device_ids = check_device_ids(device_ids)
 
-    try:
+    if model_config.model_type in PREDEFINED_CONFIGS:
         return PREDEFINED_CONFIGS[model_config.model_type](model_config, device_ids)
-    except KeyError:
+    else:
         logger.warning(
             "Using automatic config: tensor parallel config not provided and no custom config registered for the model"
         )
         return None
 
 
 class TensorParallelPreTrainedModel(PreTrainedModel):
```

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/shard.py` & `tensor_parallel-1.3.1/src/tensor_parallel/shard.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/sharding.py` & `tensor_parallel-1.3.1/src/tensor_parallel/sharding.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/slicing_configs.py` & `tensor_parallel-1.3.1/src/tensor_parallel/slicing_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Optimized configs for selected models. These configs are not necessary, but they can improve performance in some
 cases, e.g. training with very small batches or inference with long sequences.
 
 NB: some of these configs get fairly complicated in order to squeeze a bit of extra performance. When developing your
   own config, you can get most of the performance benefits by using auto config -- and maybe splitting MLP layers.
 """
+import re
 from functools import partial
 from itertools import chain
 from typing import Callable, Dict, Sequence
 
 import torch
 from transformers import BertConfig, BloomConfig, CodeGenConfig, GPT2Config, GPTNeoXConfig, PretrainedConfig, T5Config
 
@@ -394,15 +395,17 @@
                 "num_heads": lambda n, rank: q_per_kv
                 * split_num_heads(n // q_per_kv, rank=rank, world_size=world_size),
             }
         },
     )
 
     if new_modeling:
-        config.attr_rules[r".*self_attn$"]["num_key_value_heads"] = partial(split_num_heads, world_size=world_size)
+        config.attr_rules[re.compile(".*self_attn$")]["num_key_value_heads"] = partial(
+            split_num_heads, world_size=world_size
+        )
 
     return config
 
 
 def get_refined_web_config(model_config: PretrainedConfig, devices: Sequence[torch.device]) -> Config:
     # We can't use `RWConfig`` since it's custom code
     assert model_config.model_type == "RefinedWeb", f"Trying to pass {model_config.model_type} as RefinedWeb config"
```

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/state_actions.py` & `tensor_parallel-1.3.1/src/tensor_parallel/state_actions.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/tensor_parallel.py` & `tensor_parallel-1.3.1/src/tensor_parallel/tensor_parallel.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/utils.py` & `tensor_parallel-1.3.1/src/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel/wrapper.py` & `tensor_parallel-1.3.1/src/tensor_parallel/wrapper.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel.egg-info/PKG-INFO` & `tensor_parallel-1.3.1/src/tensor_parallel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensor-parallel
-Version: 1.3.0
+Version: 1.3.1
 Summary: Automatically shard your large model between multiple GPUs, works without torch.distributed
 Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak
 Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tensor-parallel Version: 1.3.0 Summary:
+Metadata-Version: 2.1 Name: tensor-parallel Version: 1.3.1 Summary:
 Automatically shard your large model between multiple GPUs, works without
 torch.distributed Home-page: https://github.com/BlackSamorez/tensor_parallel
 Author: Andrei Panferov and Yaroslav Lisnyak Author-email: yalisnyak@nes.com
 Project-URL: Bug Tracker, https://github.com/BlackSamorez/tensor_parallel/
 issues Classifier: Development Status :: 4 - Beta Classifier: Intended Audience
 :: Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
```

### Comparing `tensor_parallel-1.3.0/src/tensor_parallel.egg-info/SOURCES.txt` & `tensor_parallel-1.3.1/src/tensor_parallel.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 src/tensor_parallel.egg-info/SOURCES.txt
 src/tensor_parallel.egg-info/dependency_links.txt
 src/tensor_parallel.egg-info/requires.txt
 src/tensor_parallel.egg-info/top_level.txt
 tests/test_basic.py
 tests/test_factory.py
 tests/test_integration.py
+tests/test_legacy.py
 tests/test_saving.py
 tests/test_transformers.py
```

### Comparing `tensor_parallel-1.3.0/tests/test_basic.py` & `tensor_parallel-1.3.1/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/tests/test_factory.py` & `tensor_parallel-1.3.1/tests/test_factory.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/tests/test_integration.py` & `tensor_parallel-1.3.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/tests/test_saving.py` & `tensor_parallel-1.3.1/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `tensor_parallel-1.3.0/tests/test_transformers.py` & `tensor_parallel-1.3.1/tests/test_transformers.py`

 * *Files identical despite different names*

