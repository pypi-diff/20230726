# Comparing `tmp/eyeball_pp-0.0.2.tar.gz` & `tmp/eyeball_pp-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyeball_pp-0.0.2.tar", last modified: Thu Jul 13 04:43:51 2023, max compression
+gzip compressed data, was "eyeball_pp-0.0.3.tar", last modified: Wed Jul 26 18:55:40 2023, max compression
```

## Comparing `eyeball_pp-0.0.2.tar` & `eyeball_pp-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-13 04:43:51.671836 eyeball_pp-0.0.2/
--rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.2/LICENSE
--rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-13 04:43:51.671933 eyeball_pp-0.0.2/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)     8520 2023-07-12 19:49:37.000000 eyeball_pp-0.0.2/README.md
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-13 04:43:51.670347 eyeball_pp-0.0.2/eyeball_pp/
--rw-r--r--   0 revant     (501) staff       (20)      757 2023-06-27 22:22:21.000000 eyeball_pp-0.0.2/eyeball_pp/__init__.py
--rw-r--r--   0 revant     (501) staff       (20)     2096 2023-07-12 21:34:21.000000 eyeball_pp-0.0.2/eyeball_pp/classes.py
--rw-r--r--   0 revant     (501) staff       (20)     2137 2023-07-12 21:50:50.000000 eyeball_pp-0.0.2/eyeball_pp/comparators.py
--rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.2/eyeball_pp/compare_checkpoints.py
--rw-r--r--   0 revant     (501) staff       (20)    39224 2023-07-13 04:42:50.000000 eyeball_pp-0.0.2/eyeball_pp/eval.py
--rw-r--r--   0 revant     (501) staff       (20)    25534 2023-07-13 04:40:36.000000 eyeball_pp-0.0.2/eyeball_pp/recorders.py
--rw-r--r--   0 revant     (501) staff       (20)      374 2023-06-30 00:16:29.000000 eyeball_pp-0.0.2/eyeball_pp/utils.py
-drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-13 04:43:51.671639 eyeball_pp-0.0.2/eyeball_pp.egg-info/
--rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-13 04:43:51.000000 eyeball_pp-0.0.2/eyeball_pp.egg-info/PKG-INFO
--rw-r--r--   0 revant     (501) staff       (20)      340 2023-07-13 04:43:51.000000 eyeball_pp-0.0.2/eyeball_pp.egg-info/SOURCES.txt
--rw-r--r--   0 revant     (501) staff       (20)        1 2023-07-13 04:43:51.000000 eyeball_pp-0.0.2/eyeball_pp.egg-info/dependency_links.txt
--rw-r--r--   0 revant     (501) staff       (20)       11 2023-07-13 04:43:51.000000 eyeball_pp-0.0.2/eyeball_pp.egg-info/top_level.txt
--rw-r--r--   0 revant     (501) staff       (20)      527 2023-07-13 04:43:51.672428 eyeball_pp-0.0.2/setup.cfg
--rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.2/setup.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-26 18:55:40.415377 eyeball_pp-0.0.3/
+-rw-r--r--   0 revant     (501) staff       (20)    11357 2023-06-21 17:31:20.000000 eyeball_pp-0.0.3/LICENSE
+-rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-26 18:55:40.415510 eyeball_pp-0.0.3/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)     8520 2023-07-12 19:49:37.000000 eyeball_pp-0.0.3/README.md
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-26 18:55:40.400505 eyeball_pp-0.0.3/eyeball_pp/
+-rw-r--r--   0 revant     (501) staff       (20)      757 2023-06-27 22:22:21.000000 eyeball_pp-0.0.3/eyeball_pp/__init__.py
+-rw-r--r--   0 revant     (501) staff       (20)     2307 2023-07-13 18:39:56.000000 eyeball_pp-0.0.3/eyeball_pp/classes.py
+-rw-r--r--   0 revant     (501) staff       (20)     2137 2023-07-12 21:50:50.000000 eyeball_pp-0.0.3/eyeball_pp/comparators.py
+-rw-r--r--   0 revant     (501) staff       (20)      201 2023-06-27 19:58:23.000000 eyeball_pp-0.0.3/eyeball_pp/compare_checkpoints.py
+-rw-r--r--   0 revant     (501) staff       (20)    38808 2023-07-26 18:52:02.000000 eyeball_pp-0.0.3/eyeball_pp/eval.py
+-rw-r--r--   0 revant     (501) staff       (20)    33398 2023-07-26 18:52:02.000000 eyeball_pp-0.0.3/eyeball_pp/recorders.py
+-rw-r--r--   0 revant     (501) staff       (20)      728 2023-07-26 18:52:02.000000 eyeball_pp-0.0.3/eyeball_pp/utils.py
+drwxr-xr-x   0 revant     (501) staff       (20)        0 2023-07-26 18:55:40.415050 eyeball_pp-0.0.3/eyeball_pp.egg-info/
+-rw-r--r--   0 revant     (501) staff       (20)     8903 2023-07-26 18:55:40.000000 eyeball_pp-0.0.3/eyeball_pp.egg-info/PKG-INFO
+-rw-r--r--   0 revant     (501) staff       (20)      340 2023-07-26 18:55:40.000000 eyeball_pp-0.0.3/eyeball_pp.egg-info/SOURCES.txt
+-rw-r--r--   0 revant     (501) staff       (20)        1 2023-07-26 18:55:40.000000 eyeball_pp-0.0.3/eyeball_pp.egg-info/dependency_links.txt
+-rw-r--r--   0 revant     (501) staff       (20)       11 2023-07-26 18:55:40.000000 eyeball_pp-0.0.3/eyeball_pp.egg-info/top_level.txt
+-rw-r--r--   0 revant     (501) staff       (20)      527 2023-07-26 18:55:40.416155 eyeball_pp-0.0.3/setup.cfg
+-rw-r--r--   0 revant     (501) staff       (20)       38 2023-06-23 17:41:10.000000 eyeball_pp-0.0.3/setup.py
```

### Comparing `eyeball_pp-0.0.2/LICENSE` & `eyeball_pp-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.2/PKG-INFO` & `eyeball_pp-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball_pp
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `eyeball_pp-0.0.2/README.md` & `eyeball_pp-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.2/eyeball_pp/__init__.py` & `eyeball_pp-0.0.3/eyeball_pp/__init__.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.2/eyeball_pp/classes.py` & `eyeball_pp-0.0.3/eyeball_pp/classes.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 
 
 class FeedbackResult(IntEnum):
     POSITIVE = 1
     NEGATIVE = -1
     NEUTRAL = 0
 
+    def __str__(self) -> str:
+        if self == FeedbackResult.POSITIVE:
+            return "📈 +ve"
+        elif self == FeedbackResult.NEGATIVE:
+            return "📉 -ve"
+        else:
+            return "📊 neutral"
+
 
 @dataclass
 class OutputFeedback:
     result: FeedbackResult
     message: str
 
     def as_dict(self):
@@ -61,9 +69,12 @@
         newer_checkpoint_output: str,
     ) -> OutputFeedback:
         ...
 
 
 # The output scorer is used to score the output of a model given the objective and inputs
 # The scorer should return a float with a higher value indicating a better output
-# First input is the objective , second is a dictionary of input variables, third is the value for the output
-OutputScorer = Callable[[str, dict[str, str], str], OutputScore]
+class OutputScorer(Protocol):
+    def __call__(
+        self, objective: str, input_variables: dict[str, str], output: str
+    ) -> OutputScore:
+        ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eyeball_pp-0.0.2/eyeball_pp/comparators.py` & `eyeball_pp-0.0.3/eyeball_pp/comparators.py`

 * *Files identical despite different names*

### Comparing `eyeball_pp-0.0.2/eyeball_pp/eval.py` & `eyeball_pp-0.0.3/eyeball_pp/eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import defaultdict
 from contextlib import contextmanager
 from enum import Enum
 import inspect
 import json
 import os
 from .recorders import (
+    ApiClientRecorder,
     Checkpoint,
     ComparisonResult,
     DiskRecorder,
     FileRecorder,
     MemoryRecorder,
     EvalRecorder,
     get_input_hash,
@@ -67,14 +68,16 @@
 T = TypeVar("T", int, float, str, bool, bytes, dict, list, None, JsonSerializable)
 
 
 @dataclass
 class EvaluatorConfig:
     sample_rate: float = 1.0
     dir_path: str = "./eyeball_data"
+    api_key: Optional[str] = None
+    api_url: Optional[str] = None
 
     @staticmethod
     def _merge(original_config: "EvaluatorConfig", **kwargs) -> "EvaluatorConfig":
         """Kwargs should be a subset of the fields of the original config."""
         if len(kwargs) == 0:
             return original_config
 
@@ -105,15 +108,20 @@
 
     def _get_config(self, **override_config_kwargs) -> EvaluatorConfig:
         return EvaluatorConfig._merge(self.config, **override_config_kwargs)
 
     def set_config(self, **config_kwargs) -> None:
         self.config = EvaluatorConfig._merge(self.config, **config_kwargs)
         self.data_dir = os.path.join(self.config.dir_path, "eyeball_data")
-        self.recorder: EvalRecorder = FileRecorder(self.data_dir)
+        if self.config.api_key is not None:
+            self.recorder: EvalRecorder = ApiClientRecorder(
+                api_key=self.config.api_key, api_url=self.config.api_url
+            )
+        else:
+            self.recorder = FileRecorder(self.data_dir)
 
     @contextmanager
     def start_recording_session(
         self,
         task_name: str,
         checkpoint_id: Optional[str] = None,
         checkpoint_id_to_rerun: Optional[str] = None,
@@ -187,29 +195,33 @@
             )
             self.recorder.record_output(
                 task_name=task_name,
                 checkpoint_id=checkpoint_id,
                 output=self._serialize(value),
             )
 
-    def _get_last_checkpoint_id(
+    def _get_last_checkpoint(
         self,
         task_name: str,
         input_hash: str,
         current_checkpoint_id: str,
-    ) -> Optional[str]:
+    ) -> Optional[Checkpoint]:
         checkpoints = self.recorder.get_latest_checkpoints(
             task_name, input_hash, num_checkpoints=2
         )
+        if len(checkpoints) == 0:
+            return None
 
-        for checkpoint_id in reversed(checkpoints):
-            if checkpoint_id == current_checkpoint_id:
-                continue
-            return checkpoint_id
-        return None
+        if checkpoints[0].checkpoint_id == current_checkpoint_id:
+            if len(checkpoints) == 1:
+                return None
+            return checkpoints[1]
+
+        else:
+            return checkpoints[0]
 
     def _get_recorder_state(
         self,
         task_name: Optional[str] = None,
         recorder_checkpoint_id: Optional[str] = None,
     ) -> tuple[str, str]:
         if task_name is None and hasattr(self.current_recorder_state, "task_name"):
@@ -439,27 +451,24 @@
                 "id": datetime.datetime.utcnow().isoformat(),
             }
 
             print(f"Will rerun {len(input_hashes)} inputs for task:`{task_name}`")
 
             for idx, input_hash in enumerate(input_hashes):
                 recorder_checkpoint_id = datetime.datetime.utcnow().isoformat()
-                last_checkpoind_id = self._get_last_checkpoint_id(
+                last_checkpoint = self._get_last_checkpoint(
                     task_name=task_name,
                     input_hash=input_hash,
                     current_checkpoint_id=recorder_checkpoint_id,
                 )
-                if last_checkpoind_id is None:
+                if last_checkpoint is None:
                     continue
 
-                self.checkpoint_id_to_rerun = last_checkpoind_id
-                checkpoint_to_rerun = self.recorder.get_checkpoint(
-                    task_name=task_name,
-                    checkpoint_id=last_checkpoind_id,
-                )
+                self.checkpoint_id_to_rerun = last_checkpoint.checkpoint_id
+                checkpoint_to_rerun = last_checkpoint
                 if checkpoint_to_rerun is None:
                     continue
 
                 input_vars = {
                     k: json.loads(v)
                     for k, v in checkpoint_to_rerun.get_input_variables().items()
                 }
@@ -468,15 +477,15 @@
                 )
 
                 if len(eval_params_list) > 0:
                     for eval_params in eval_params_list:
                         with self.start_recording_session(
                             task_name=task_name,
                             checkpoint_id=recorder_checkpoint_id,
-                            checkpoint_id_to_rerun=last_checkpoind_id,
+                            checkpoint_id_to_rerun=checkpoint_to_rerun.checkpoint_id,
                         ):
                             self.recorder.record_eval_params(
                                 task_name=task_name,
                                 checkpoint_id=recorder_checkpoint_id,
                                 eval_params=eval_params,
                                 rerun_metadata=rerun_metadata,
                             )
@@ -518,23 +527,18 @@
         if len(input_hashes_lst) == 0:
             input_hashes_lst = self.recorder.get_input_hashes(task_name=task_name)
 
         try:
             self.mode = EvaluatorMode.RATE_EXAMPLES
             for input_hash in input_hashes_lst:
                 already_seen_outputs_to_feedback: dict[str:OutputFeedback] = {}
-                checkpoint_ids = self.recorder.get_latest_checkpoints(
+                checkpoints = self.recorder.get_latest_checkpoints(
                     task_name, input_hash, num_checkpoints=4
                 )
-                raw_checkpoints = [
-                    self.recorder.get_checkpoint(task_name, c) for c in checkpoint_ids
-                ]
-                checkpoints: list[Checkpoint] = [
-                    c for c in raw_checkpoints if c is not None
-                ]
+
                 if len(checkpoints) == 0:
                     continue
 
                 print(f"For the inputs:\n{checkpoints[0].get_input_var_str()}")
                 for checkpoint in checkpoints:
                     if checkpoint.output_feedback is None:
                         if feedback := already_seen_outputs_to_feedback.get(
@@ -615,15 +619,15 @@
         for input_hash in self.recorder.get_input_hashes(task_name):
             checkpoints = self.recorder.get_latest_checkpoints(
                 task_name, input_hash, num_checkpoints=1
             )
             if len(checkpoints) == 0:
                 continue
 
-            checkpoint = self.recorder.get_checkpoint(task_name, checkpoints[0])
+            checkpoint = checkpoints[0]
             if checkpoint is None:
                 continue
 
             row_data = {}
             input_names.update(checkpoint.input_variables.keys())
             for input_name, input_value in checkpoint.input_variables.items():
                 row_data[input_name] = input_value
@@ -635,15 +639,15 @@
             )
             sorted_comparison_results = sorted(
                 comparison_results,
                 key=lambda x: x.newer_checkpoint_id,
                 reverse=True,
             )
             for idx, comparison_result in enumerate(sorted_comparison_results):
-                msg = comparison_result.output_feedback.result.name
+                msg = str(comparison_result.output_feedback.result)
                 new_checkpoint = self.recorder.get_checkpoint(
                     task_name=task_name,
                     checkpoint_id=comparison_result.newer_checkpoint_id,
                 )
                 if new_checkpoint is not None:
                     if new_checkpoint.output_score is not None:
                         msg += f" (score: {new_checkpoint.output_score})"
@@ -661,14 +665,15 @@
 
         if len(rows) > 0:
             column_names = sorted(list(input_names)) + comparison_column_names
             for column_name in column_names:
                 table.add_column(column_name, justify="left")
 
             md_data.append("| " + " | ".join(column_names) + " |")
+            md_data.append("| " + " | ".join(["---"] * len(column_names)) + " |")
 
             for row in rows:
                 row_tuple = tuple(
                     row.get(column_name, "") for column_name in column_names
                 )
                 table.add_row(*row_tuple)
                 md_data.append("| " + " | ".join(row_tuple) + " |")
@@ -724,36 +729,28 @@
             self.mode = EvaluatorMode.COMPARE_CHECKPOINTS
 
             params_to_succesful_examples: dict[str, int] = defaultdict(int)
             rerun_to_succesful_examples: dict[str, int] = defaultdict(int)
 
             num_comparisons = 0
             for idx, input_hash in enumerate(input_hashes_list):
-                checkpoint_ids = self.recorder.get_latest_checkpoints(
+                checkpoints_list = self.recorder.get_latest_checkpoints(
                     task_name,
                     input_hash,
                     num_checkpoints=num_checkpoints_per_input_hash,
                 )
 
-                checkpoints: dict[str, Checkpoint] = {}
-                filtered_checkpoint_ids = []
-                for checkpoind_id in checkpoint_ids:
-                    checkpoint = self.recorder.get_checkpoint(
-                        task_name=task_name,
-                        checkpoint_id=checkpoind_id,
-                    )
-                    if (
-                        checkpoint is not None
-                        and checkpoint.output is not None
-                        and checkpoint.output != "null"
-                        and checkpoint.output != "None"
-                    ):
-                        filtered_checkpoint_ids.append(checkpoind_id)
-                        checkpoints[checkpoind_id] = checkpoint
-                checkpoint_ids = sorted(filtered_checkpoint_ids, reverse=True)
+                checkpoints: dict[str, Checkpoint] = {
+                    c.checkpoint_id: c
+                    for c in checkpoints_list
+                    if c.output is not None
+                    and c.output != "null"
+                    and c.output != "None"
+                }
+                checkpoint_ids = sorted(checkpoints.keys(), reverse=True)
 
                 if len(checkpoint_ids) == 0:
                     continue
 
                 scores: dict[str, OutputScore] = {}
                 if output_scorer is not None:
                     print(f"\nInput #{idx} - Scoring {len(checkpoint_ids)} checkpoints")
```

### Comparing `eyeball_pp-0.0.2/eyeball_pp/recorders.py` & `eyeball_pp-0.0.3/eyeball_pp/recorders.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,39 @@
+from concurrent.futures import ThreadPoolExecutor
 import hashlib
 import json
+import pkg_resources
 import yaml
 import os
 import pickle
 from typing import Any, Optional, Protocol
 from dataclasses import dataclass
 import dataclasses
+import requests
 
+from .utils import LruCache
 from .classes import OutputFeedback, OutputScore
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ComparisonResult:
     older_checkpoint_id: str
     newer_checkpoint_id: str
     output_feedback: OutputFeedback
 
+    def as_dict(self):
+        return {
+            "older_checkpoint_id": self.older_checkpoint_id,
+            "newer_checkpoint_id": self.newer_checkpoint_id,
+            "output_feedback": self.output_feedback.as_dict(),
+        }
+
 
 def get_input_hash(input_variables: dict[str, str]) -> str:
     sorted_input_vars = sorted(
         [
             (str(var_name), str(var_val))
             for var_name, var_val in input_variables.items()
         ],
@@ -110,15 +124,15 @@
     def get_checkpoint(
         self, task_name: str, checkpoint_id: str
     ) -> Optional[Checkpoint]:
         ...
 
     def get_latest_checkpoints(
         self, task_name: str, input_hash: str, num_checkpoints: int = 2
-    ) -> list[str]:
+    ) -> list[Checkpoint]:
         ...
 
     def get_input_hashes(self, task_name: str) -> list[str]:
         ...
 
     def get_task_names(self) -> list[str]:
         ...
@@ -148,14 +162,233 @@
         self,
         task_name: str,
         input_hash: str,
     ) -> None:
         ...
 
 
+class ApiClientRecorder(EvalRecorder):
+    def __init__(self, api_key: str, api_url: Optional[str] = None) -> None:
+        self.api_key = api_key
+        if api_url is None:
+            self.url = "https://eyeball.tark.ai/"
+        else:
+            self.url = api_url
+        self.checkpoint_dicts: LruCache = LruCache(max_size=100)
+        self.pool = ThreadPoolExecutor(max_workers=1)
+
+    def _get_headers(self) -> dict[str, str]:
+        return {
+            "Authorization": f"Bearer {self.api_key}",
+        }
+
+    def _record_checkpoint(
+        self,
+        task_name: str,
+        checkpoint_id: str,
+        prefixes: list[str],
+        name: str,
+        value: Any,
+        flush: bool = False,
+    ) -> dict[str, Any]:
+        dict_key = f"{task_name},{checkpoint_id}"
+        if dict_key not in self.checkpoint_dicts:
+            checkpoint_dict: dict[str, Any] = {"checkpoint_id": checkpoint_id}
+        else:
+            checkpoint_dict = self.checkpoint_dicts[dict_key]
+
+        current_dict = checkpoint_dict
+        for prefix in prefixes:
+            if prefix not in current_dict:
+                current_dict[prefix] = {}
+            current_dict = current_dict[prefix]
+        current_dict[name] = value
+        self.checkpoint_dicts[dict_key] = dict(checkpoint_dict)
+
+        if flush:
+
+            def _record():
+                response = requests.post(
+                    f"{self.url}/record_checkpoint",
+                    json={
+                        "task_name": task_name,
+                        "checkpoint_id": checkpoint_id,
+                        **checkpoint_dict,
+                    },
+                    headers=self._get_headers(),
+                )
+                if response.status_code != 200:
+                    logger.error(
+                        f"Failed to record checkpoint {checkpoint_id} -- {response.status_code}, {response.text}"
+                    )
+                else:
+                    logger.debug(f"Recorded checkpoint {checkpoint_id}")
+
+            self.pool.submit(_record)
+        return checkpoint_dict
+
+    def record_input_variable(
+        self, task_name: str, checkpoint_id: str, variable_name: str, value: str
+    ) -> None:
+        self._record_checkpoint(
+            task_name=task_name,
+            checkpoint_id=checkpoint_id,
+            prefixes=["input_variables"],
+            name=variable_name,
+            value=value,
+        )
+
+    def record_output(self, task_name: str, checkpoint_id: str, output: str) -> None:
+        self._record_checkpoint(
+            task_name=task_name,
+            checkpoint_id=checkpoint_id,
+            prefixes=[],
+            name="output",
+            value=output,
+            flush=True,
+        )
+
+    def record_eval_params(
+        self,
+        task_name: str,
+        checkpoint_id: str,
+        eval_params: dict[str, Any],
+        rerun_metadata: dict[str, Any] | None = None,
+    ) -> None:
+        self._record_checkpoint(
+            task_name=task_name,
+            checkpoint_id=checkpoint_id,
+            prefixes=[],
+            name="eval_params",
+            value=eval_params,
+        )
+        if rerun_metadata is not None:
+            self._record_checkpoint(
+                task_name=task_name,
+                checkpoint_id=checkpoint_id,
+                prefixes=[],
+                name="rerun_metadata",
+                value=rerun_metadata,
+            )
+
+    def record_comparison_result(
+        self, task_name: str, input_hash: str, result: ComparisonResult
+    ) -> None:
+        requests.post(
+            f"{self.url}/record_comparison_result",
+            json={
+                "task_name": task_name,
+                "input_hash": input_hash,
+                "result": result.as_dict(),
+            },
+            headers=self._get_headers(),
+        )
+
+    def record_output_score(
+        self, task_name: str, checkpoint_id: str, score: OutputScore
+    ) -> None:
+        requests.post(
+            f"{self.url}/record_output_score",
+            json={
+                "task_name": task_name,
+                "checkpoint_id": checkpoint_id,
+                "score": score.as_dict(),
+            },
+            headers=self._get_headers(),
+        )
+
+    def record_output_feedback(
+        self, task_name: str, checkpoint_id: str, feedback: OutputFeedback
+    ) -> None:
+        requests.post(
+            f"{self.url}/record_output_feedback",
+            json={
+                "task_name": task_name,
+                "checkpoint_id": checkpoint_id,
+                "feedback": feedback.as_dict(),
+            },
+            headers=self._get_headers(),
+        )
+
+    def delete_checkpoints_for_input_hash(
+        self, task_name: str, input_hash: str
+    ) -> None:
+        ...
+
+    def get_checkpoint(self, task_name: str, checkpoint_id: str) -> Checkpoint | None:
+        dict_key = f"{task_name},{checkpoint_id}"
+        if dict_key in self.checkpoint_dicts:
+            return Checkpoint(**(self.checkpoint_dicts[dict_key]))
+
+        response = requests.get(
+            f"{self.url}/get_checkpoint",
+            json={
+                "task_name": task_name,
+                "checkpoint_id": checkpoint_id,
+            },
+            headers=self._get_headers(),
+        )
+        if response.status_code != 200:
+            logger.debug(
+                f"Failed to get checkpoint - {checkpoint_id}: {response.status_code}"
+            )
+            return None
+        return Checkpoint(**response.json())
+
+    def get_comparison_result(
+        self, task_name: str, older_checkpoint_id: str, newer_checkpoint_id: str
+    ) -> ComparisonResult | None:
+        ...
+
+    def get_comparison_results_for_input_hash(
+        self, task_name: str, input_hash: str, num_results: int = 3
+    ) -> list[ComparisonResult]:
+        return []
+
+    def get_input_hashes(self, task_name: str) -> list[str]:
+        response = requests.get(
+            f"{self.url}/get_input_hashes",
+            json={
+                "task_name": task_name,
+            },
+            headers=self._get_headers(),
+        )
+        if response.status_code != 200:
+            logger.debug(f"Failed to get input hashes: {response.status_code}")
+            return []
+        return response.json()["input_hashes"]
+
+    def get_latest_checkpoints(
+        self, task_name: str, input_hash: str, num_checkpoints: int = 2
+    ) -> list[Checkpoint]:
+        response = requests.get(
+            f"{self.url}/get_latest_checkpoints",
+            json={
+                "task_name": task_name,
+                "input_hash": input_hash,
+                "num_checkpoints": num_checkpoints,
+            },
+            headers=self._get_headers(),
+        )
+        if response.status_code != 200:
+            logger.debug(f"Failed to get latest checkpoints: {response.status_code}")
+            return []
+        return [Checkpoint(**data) for data in response.json()["checkpoints"]]
+
+    def get_task_names(self) -> list[str]:
+        response = requests.get(
+            f"{self.url}/get_task_names",
+            headers=self._get_headers(),
+        )
+        if response.status_code != 200:
+            logger.debug(f"Failed to get task names: {response.status_code}")
+            return []
+        return response.json()["task_names"]
+
+
 @dataclass
 class Task:
     name: str
     checkpoints: dict[str, Checkpoint] = dataclasses.field(default_factory=dict)
     input_hashes: dict[str, set[str]] = dataclasses.field(default_factory=dict)
     comparison_results: dict[str, ComparisonResult] = dataclasses.field(
         default_factory=dict
@@ -227,22 +460,27 @@
         checkpoint = self._fetch_or_create_checkpoint(
             task_name=task_name, checkpoint_id=checkpoint_id
         )
         checkpoint.output = output
 
     def get_latest_checkpoints(
         self, task_name: str, input_hash: str, num_checkpoints: int = 2
-    ) -> list[str]:
+    ) -> list[Checkpoint]:
         if task_name not in self.tasks:
             return []
         task = self.tasks[task_name]
         if input_hash not in task.input_hashes:
             return []
 
-        return sorted(task.input_hashes[input_hash])[-num_checkpoints:]
+        return [
+            task.checkpoints[checkpoint_id]
+            for checkpoint_id in sorted(task.input_hashes[input_hash])[
+                -num_checkpoints:
+            ]
+        ]
 
     def get_checkpoint(
         self, task_name: str, checkpoint_id: str
     ) -> Optional[Checkpoint]:
         if task_name not in self.tasks:
             return None
         task = self.tasks[task_name]
@@ -522,34 +760,35 @@
             OutputScore.from_dict(yaml_dict.get("output_score"))
             if "output_score" in yaml_dict
             else None
         )
         checkpoint.rerun_metadata = yaml_dict.get("rerun_metadata")
         return checkpoint
 
-    def _read_checkpoints(self, task_name: str) -> dict[str, list[str]]:
-        input_hashes_to_checkpoints: dict[str, list[str]] = {}
+    def _read_checkpoints(self, task_name: str) -> dict[str, list[Checkpoint]]:
+        input_hashes_to_checkpoints: dict[str, list[Checkpoint]] = {}
         dir_name = os.path.join(self.dir_path, task_name, "checkpoints")
         for file_name in os.listdir(dir_name):
             if file_name.endswith(".yaml"):
-                checkpoint_id = file_name[:-5]
                 file_path = os.path.join(dir_name, file_name)
                 yaml_dict = yaml.load(open(file_path, "r"), Loader=yaml.FullLoader)
                 if input_hash := yaml_dict.get("input_hash"):
                     if input_hash not in input_hashes_to_checkpoints:
                         input_hashes_to_checkpoints[input_hash] = []
-                    input_hashes_to_checkpoints[input_hash].append(checkpoint_id)
+                    input_hashes_to_checkpoints[input_hash].append(
+                        Checkpoint(**yaml_dict)
+                    )
 
         for input_hash in input_hashes_to_checkpoints:
             input_hashes_to_checkpoints[input_hash].sort(reverse=True)
         return input_hashes_to_checkpoints
 
     def get_latest_checkpoints(
         self, task_name: str, input_hash: str, num_checkpoints: int = 2
-    ) -> list[str]:
+    ) -> list[Checkpoint]:
         input_hashes_to_checkpoints = self._read_checkpoints(task_name)
         if input_hash not in input_hashes_to_checkpoints:
             return []
         return input_hashes_to_checkpoints[input_hash][:num_checkpoints]
 
     def get_input_hashes(self, task_name: str) -> list[str]:
         input_hashes = []
@@ -711,15 +950,15 @@
     ) -> Optional[Checkpoint]:
         return self.memory_recorder.get_checkpoint(
             task_name=task_name, checkpoint_id=checkpoint_id
         )
 
     def get_latest_checkpoints(
         self, task_name: str, input_hash: str, num_checkpoints: int = 2
-    ) -> list[str]:
+    ) -> list[Checkpoint]:
         return self.memory_recorder.get_latest_checkpoints(
             task_name=task_name, input_hash=input_hash, num_checkpoints=num_checkpoints
         )
 
     def get_input_hashes(self, task_name: str) -> list[str]:
         return self.memory_recorder.get_input_hashes(task_name)
```

### Comparing `eyeball_pp-0.0.2/eyeball_pp.egg-info/PKG-INFO` & `eyeball_pp-0.0.3/eyeball_pp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eyeball-pp
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for evaluating tasks which use llms
 Home-page: https://github.com/revantk/eyeball-plus-plus
 Author: Revant
 Author-email: revant.kapoor@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

