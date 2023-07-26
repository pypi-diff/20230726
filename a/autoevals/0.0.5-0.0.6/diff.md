# Comparing `tmp/autoevals-0.0.5.tar.gz` & `tmp/autoevals-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoevals-0.0.5.tar", last modified: Mon Jul 24 22:07:36 2023, max compression
+gzip compressed data, was "autoevals-0.0.6.tar", last modified: Wed Jul 26 00:11:50 2023, max compression
```

## Comparing `autoevals-0.0.5.tar` & `autoevals-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-24 22:07:36.246872 autoevals-0.0.5/
--rw-r--r--   0 ankur      (501) staff       (20)     1072 2023-07-11 17:08:28.000000 autoevals-0.0.5/LICENSE
--rw-r--r--   0 ankur      (501) staff       (20)     5639 2023-07-24 22:07:36.246072 autoevals-0.0.5/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)     5122 2023-07-11 21:46:08.000000 autoevals-0.0.5/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       31 2023-07-11 06:26:06.000000 autoevals-0.0.5/pyproject.toml
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-07-24 22:07:36.246980 autoevals-0.0.5/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1611 2023-07-12 04:49:11.000000 autoevals-0.0.5/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-24 22:07:36.229387 autoevals-0.0.5/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-24 22:07:36.234019 autoevals-0.0.5/src/autoevals/
--rw-r--r--   0 ankur      (501) staff       (20)       61 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     1528 2023-07-24 08:40:40.000000 autoevals-0.0.5/src/autoevals/base.py
--rw-r--r--   0 ankur      (501) staff       (20)     6191 2023-07-24 08:40:40.000000 autoevals-0.0.5/src/autoevals/llm.py
--rw-r--r--   0 ankur      (501) staff       (20)      673 2023-07-24 08:40:40.000000 autoevals-0.0.5/src/autoevals/string.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-24 22:07:36.245757 autoevals-0.0.5/src/autoevals/templates/
--rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/battle.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/closed_q_a.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/factuality.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/humor.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/possible.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/security.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/sql.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-11 17:44:18.000000 autoevals-0.0.5/src/autoevals/templates/summary.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/templates/translation.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     4780 2023-07-11 20:58:26.000000 autoevals-0.0.5/src/autoevals/test_llm.py
--rw-r--r--   0 ankur      (501) staff       (20)      552 2023-07-24 08:40:40.000000 autoevals-0.0.5/src/autoevals/test_string.py
--rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-11 06:26:29.000000 autoevals-0.0.5/src/autoevals/util.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-07-24 22:07:19.000000 autoevals-0.0.5/src/autoevals/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-24 22:07:36.242717 autoevals-0.0.5/src/autoevals.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)     5639 2023-07-24 22:07:36.000000 autoevals-0.0.5/src/autoevals.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      758 2023-07-24 22:07:36.000000 autoevals-0.0.5/src/autoevals.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-07-24 22:07:36.000000 autoevals-0.0.5/src/autoevals.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)      268 2023-07-24 22:07:36.000000 autoevals-0.0.5/src/autoevals.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       10 2023-07-24 22:07:36.000000 autoevals-0.0.5/src/autoevals.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:11:50.881888 autoevals-0.0.6/
+-rw-r--r--   0 ankur      (501) staff       (20)     1072 2023-07-24 12:02:52.000000 autoevals-0.0.6/LICENSE
+-rw-r--r--   0 ankur      (501) staff       (20)       30 2023-07-25 10:30:28.000000 autoevals-0.0.6/MANIFEST.in
+-rw-r--r--   0 ankur      (501) staff       (20)     5426 2023-07-26 00:11:50.881772 autoevals-0.0.6/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)     4908 2023-07-26 00:11:49.000000 autoevals-0.0.6/README.md
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:11:50.878142 autoevals-0.0.6/py/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:11:50.880043 autoevals-0.0.6/py/autoevals/
+-rw-r--r--   0 ankur      (501) staff       (20)       61 2023-07-25 10:30:28.000000 autoevals-0.0.6/py/autoevals/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1506 2023-07-25 12:23:28.000000 autoevals-0.0.6/py/autoevals/base.py
+-rw-r--r--   0 ankur      (501) staff       (20)     7383 2023-07-25 12:33:25.000000 autoevals-0.0.6/py/autoevals/llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1866 2023-07-25 10:30:28.000000 autoevals-0.0.6/py/autoevals/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)      612 2023-07-25 12:23:44.000000 autoevals-0.0.6/py/autoevals/string.py
+-rw-r--r--   0 ankur      (501) staff       (20)     5132 2023-07-25 12:28:11.000000 autoevals-0.0.6/py/autoevals/test_llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)      546 2023-07-25 10:30:28.000000 autoevals-0.0.6/py/autoevals/test_string.py
+-rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-25 10:30:28.000000 autoevals-0.0.6/py/autoevals/util.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-07-25 10:30:45.000000 autoevals-0.0.6/py/autoevals/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:11:50.880599 autoevals-0.0.6/py/autoevals.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)     5426 2023-07-26 00:11:50.000000 autoevals-0.0.6/py/autoevals.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      651 2023-07-26 00:11:50.000000 autoevals-0.0.6/py/autoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-07-26 00:11:50.000000 autoevals-0.0.6/py/autoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      259 2023-07-26 00:11:50.000000 autoevals-0.0.6/py/autoevals.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       10 2023-07-26 00:11:50.000000 autoevals-0.0.6/py/autoevals.egg-info/top_level.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       31 2023-07-24 12:02:52.000000 autoevals-0.0.6/pyproject.toml
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-07-26 00:11:50.881926 autoevals-0.0.6/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1575 2023-07-25 10:30:28.000000 autoevals-0.0.6/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:11:50.881622 autoevals-0.0.6/templates/
+-rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/battle.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/closed_q_a.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/factuality.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/humor.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/possible.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/security.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/sql.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/summary.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/translation.yaml
```

### Comparing `autoevals-0.0.5/LICENSE` & `autoevals-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.5/PKG-INFO` & `autoevals-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoevals
-Version: 0.0.5
+Version: 0.0.6
 Summary: Universal library for evaluating AI models
 Home-page: https://www.braintrustdata.com
 Author: BrainTrust
 Author-email: info@braintrustdata.com
 Project-URL: Bug Tracker, https://github.com/braintrustdata/autoevals
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -33,15 +33,16 @@
 their outputs.
 
 You can also create your own model-graded evaluations with AutoEvals. It's easy to add custom prompts, parse outputs,
 and manage exceptions.
 
 ## Installation
 
-To install AutoEvals, run the following command:
+AutoEvals is distributed as a [Python library on PyPI](https://pypi.org/project/autoevals/) and
+[Node.js library on NPM](https://www.npmjs.com/package/autoevals).
 
 ```bash
 pip install autoevals
 ```
 
 ## Example
 
@@ -178,13 +179,7 @@
 expected = "Standardize Error Responses across APIs"
 
 response = evaluator(output, expected, input=page_content)
 
 print(f"Score: {response.score}")
 print(f"Metadata: {response.metadata}")
 ```
-
-## Typescript / Node Support
-
-Since AutoEvals has a very simple prompt template format, it is easy to support in other languages, like
-Typescript (and eventually others). We'll support an npm package soon, but in the meantime, feel free to
-grab model templates from the [prompt templates](/src/autoevals/templates) directory.
```

### Comparing `autoevals-0.0.5/README.md` & `autoevals-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 their outputs.
 
 You can also create your own model-graded evaluations with AutoEvals. It's easy to add custom prompts, parse outputs,
 and manage exceptions.
 
 ## Installation
 
-To install AutoEvals, run the following command:
+AutoEvals is distributed as a [Python library on PyPI](https://pypi.org/project/autoevals/) and
+[Node.js library on NPM](https://www.npmjs.com/package/autoevals).
 
 ```bash
 pip install autoevals
 ```
 
 ## Example
 
@@ -160,14 +161,8 @@
 )
 expected = "Standardize Error Responses across APIs"
 
 response = evaluator(output, expected, input=page_content)
 
 print(f"Score: {response.score}")
 print(f"Metadata: {response.metadata}")
-```
-
-## Typescript / Node Support
-
-Since AutoEvals has a very simple prompt template format, it is easy to support in other languages, like
-Typescript (and eventually others). We'll support an npm package soon, but in the meantime, feel free to
-grab model templates from the [prompt templates](/src/autoevals/templates) directory.
+```
```

### Comparing `autoevals-0.0.5/setup.py` & `autoevals-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import setuptools
 
 
 dir_name = os.path.abspath(os.path.dirname(__file__))
 
 version_contents = {}
-with open(os.path.join(dir_name, "src", "autoevals", "version.py"), encoding="utf-8") as f:
+with open(os.path.join(dir_name, "py", "autoevals", "version.py"), encoding="utf-8") as f:
     exec(f.read(), version_contents)
 
 with open(os.path.join(dir_name, "README.md"), "r", encoding="utf-8") as f:
     long_description = f.read()
 
-install_requires = ["chevron", "guidance", "openai", "levenshtein", "pyyaml"]
+install_requires = ["chevron", "openai", "levenshtein", "pyyaml"]
 
 extras_require = {
     "dev": [
         "black",
         "build",
         "flake8",
         "flake8-isort",
@@ -43,17 +43,15 @@
     project_urls={
         "Bug Tracker": "https://github.com/braintrustdata/autoevals",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
-    package_dir={"": "src"},
-    package_data={
-        '': ['**/*.yaml']
-    },
-    packages=setuptools.find_packages(where="src"),
+    package_dir={"": "py"},
+    include_package_data=True,
+    packages=setuptools.find_packages(where="py"),
     python_requires=">=3.9.0",
     entry_points={},
     install_requires=install_requires,
     extras_require=extras_require,
 )
```

### Comparing `autoevals-0.0.5/src/autoevals/base.py` & `autoevals-0.0.6/py/autoevals/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import dataclasses
 from abc import ABC, abstractmethod
 
 from .util import SerializableDataClass
 
 
 @dataclasses.dataclass
-class Evaluation(SerializableDataClass):
+class Score(SerializableDataClass):
+    name: str
     score: float
     metadata: dict[str, any] = dataclasses.field(default_factory=dict)
     error: Exception = None
 
     def as_dict(self):
         return {
             "score": self.score,
@@ -18,33 +19,33 @@
         }
 
     def __post_init__(self):
         if self.score < 0 or self.score > 1:
             raise ValueError("score must be between 0 and 1")
 
 
-class Evaluator(ABC):
+class Scorer(ABC):
     async def eval_async(self, output, expected=None, **kwargs):
         try:
             return await self._run_eval_async(output, expected, **kwargs)
         except Exception as e:
-            return Evaluation(0, error=e)
+            return Score(0, error=e)
 
     def eval(self, output, expected=None, **kwargs):
         try:
             return self._run_eval_sync(output, expected, **kwargs)
         except Exception as e:
-            return Evaluation(0, error=e)
+            return Score(0, error=e)
 
     def __call__(self, output, expected=None, **kwargs):
         return self.eval(output, expected, **kwargs)
 
-    async def _run_eval_async(self, output, expected=None, **kwargs) -> Evaluation:
+    async def _run_eval_async(self, output, expected=None, **kwargs) -> Score:
         # By default we just run the sync version in a thread
         return self._run_eval_sync(output, expected, **kwargs)
 
     @abstractmethod
-    def _run_eval_sync(self, output, expected=None, **kwargs) -> Evaluation:
+    def _run_eval_sync(self, output, expected=None, **kwargs) -> Score:
         ...
 
 
-__all__ = ["Evaluation", "Evaluator"]
+__all__ = ["Score", "Scorer"]
```

### Comparing `autoevals-0.0.5/src/autoevals/llm.py` & `autoevals-0.0.6/py/autoevals/llm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 import re
 from dataclasses import dataclass
-from typing import Any, Union
+from typing import List, Optional
 
-import guidance
+import chevron
+import openai
 import yaml
 
-from .base import Evaluation, Evaluator
+from .base import Score, Scorer
+from .oai import arun_cached_request, run_cached_request
 
 
 SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
-MODEL_TEMPLATES = set(["Battle", "ClosedQA", "Humor", "Factuality", "Possible", "Security", "Summary", "Translation"])
-
 
 NO_COT_SUFFIX = """\
 Answer the question by printing only a single choice from {{__choices}} (without quotes or punctuation)
 corresponding to the correct answer with no other text.
 """.strip().replace(
     "\n", " "
 )
@@ -31,134 +31,176 @@
 
 SUPPORTED_MODELS = [
     "gpt-3.5-turbo",
     "gpt-4",
 ]
 
 
-class GuidanceLLMClassifier(Evaluator):
-    def __init__(self, program: Union[str, guidance.Program], parse_score_fn, choice_scores):
-        if isinstance(program, str):
-            program = guidance.Program(program)
-
-        if program.llm is None:
-            raise ValueError("GuidanceLLMClassifier requires an LLM")
+class OpenAILLMClassifier(Scorer):
+    def __init__(
+        self,
+        name: str,
+        messages: List,
+        model,
+        parse_score_fn,
+        choice_scores,
+        render_args=None,
+        max_tokens=None,
+        temperature=None,
+    ):
+        found = False
+        for m in SUPPORTED_MODELS:
+            # Prefixes are ok, because they are just time snapshots
+            if model.startswith(m):
+                found = True
+                break
+        if not found:
+            raise ValueError(f"Unsupported model: {model}. Currently only supports OpenAI chat models.")
 
-        self.program = program
+        self.name = name
+        self.model = model
+        self.messages = messages
         self.parse_score_fn = parse_score_fn
         self.choice_scores = choice_scores
 
+        self.extra_args = {"temperature": temperature or 0}
+        if max_tokens:
+            self.extra_args["max_tokens"] = max(max_tokens, 5)
+
+        self.render_args = {}
+        if render_args:
+            self.render_args.update(render_args)
+
     def _process_response(self, resp):
         metadata = {}
         try:
             metadata["rationale"] = str(resp)
             metadata["choice"] = self.parse_score_fn(resp)
             score = self.choice_scores[metadata["choice"]]
             error = None
         except Exception as e:
             score = 0
             error = e
 
-        return Evaluation(score=score, metadata=metadata, error=error)
+        return Score(name=self.name, score=score, metadata=metadata, error=error)
+
+    def _render_messages(self, **kwargs):
+        kwargs.update(self.render_args)
+        return [
+            {
+                **m,
+                "content": chevron.render(m["content"].strip(), kwargs, warn=True),
+            }
+            for m in self.messages
+        ]
 
     async def _run_eval_async(self, output, expected, **kwargs):
         try:
-            resp = await self.program(output=output, expected=expected, async_mode=True, **kwargs)
-            return self._process_response(resp)
+            resp = await arun_cached_request(
+                openai.ChatCompletion,
+                model=self.model,
+                messages=self._render_messages(output=output, expected=expected, **kwargs),
+                **self.extra_args,
+            )
+            if len(resp["choices"]) > 0:
+                return self._process_response(resp["choices"][0]["message"]["content"])
+            else:
+                raise ValueError("Empty response from OpenAI")
         except Exception as e:
-            return Evaluation(score=0, error=e)
+            return Score(name=self.name, score=0, error=e)
 
     def _run_eval_sync(self, output, expected, **kwargs):
         try:
-            resp = self.program(output=output, expected=expected, async_mode=False, **kwargs)
-            return self._process_response(resp)
+            resp = run_cached_request(
+                openai.ChatCompletion,
+                model=self.model,
+                messages=self._render_messages(output=output, expected=expected, **kwargs),
+                **self.extra_args,
+            )
+            if len(resp["choices"]) > 0:
+                return self._process_response(resp["choices"][0]["message"]["content"])
+            else:
+                raise ValueError("Empty response from OpenAI")
         except Exception as e:
-            return Evaluation(score=0, error=e)
+            return Score(name=self.name, score=0, error=e)
 
 
 @dataclass
 class ModelGradedSpec:
     prompt: str
     choice_scores: dict[str, float]
+    model: Optional[str] = None
+    use_cot: Optional[bool] = None
+    temperature: Optional[float] = None
 
 
 # XXX: Document that prompts are expected to be mustache templates
-class LLMClassifier(GuidanceLLMClassifier):
+class LLMClassifier(OpenAILLMClassifier):
     def __init__(
         self,
+        name,
         prompt_template,
         choice_scores,
         model="gpt-3.5-turbo",
         use_cot=True,
         max_tokens=512,
         temperature=0,
     ):
-        found = False
-        for m in SUPPORTED_MODELS:
-            # Prefixes are ok, because they are just time snapshots
-            if model.startswith(m):
-                found = True
-                break
-        if not found:
-            raise ValueError(f"Unsupported model: {model}. Currently only supports OpenAI chat models.")
-
         choice_strings = list(choice_scores.keys())
 
-        # XXX we should parse the prompt and make sure it has the right variables, and track the
-        # required inputs (so we can validate them when running the prompt)
         prompt = prompt_template + "\n" + (COT_SUFFIX if use_cot else NO_COT_SUFFIX)
         if use_cot:
 
             def parse_score_fn(resp):
                 answer = None
 
-                answers = re.findall(r"Answer\s*=\s*(.*)", resp["answer"], re.MULTILINE)
+                answers = re.findall(r"Answer\s*=\s*(.*)", resp, re.MULTILINE)
                 if len(answers) > 0:
                     answer = answers[-1].strip()
-                elif resp["answer"].strip() in choice_strings:
-                    answer = resp["answer"].strip()
+                elif resp.strip() in choice_strings:
+                    answer = resp.strip()
 
                 if answer is None:
                     raise ValueError("No answer found in response")
 
                 return answer
 
         else:
             max_tokens = max(len(c) for c in choice_strings)
 
             def parse_score_fn(resp):
-                return resp["answer"].strip()
+                return resp.strip()
 
-        program = guidance(
-            "{{#user~}}\n"
-            + prompt
-            + "{{~/user}}"
-            + """
-
-{{#assistant~}}
-{{gen 'answer' max_tokens=__max_tokens temperature=__temperature}}
-{{~/assistant}}''')
-""".strip(),
-            llm=guidance.llms.OpenAI(model),
-            __max_tokens=max_tokens,
-            __temperature=temperature,
-            __choices=choice_strings,
+        messages = [
+            {
+                "role": "user",
+                "content": prompt,
+            }
+        ]
+
+        super().__init__(
+            name,
+            messages,
+            model,
+            parse_score_fn,
+            choice_scores,
+            max_tokens=max_tokens,
+            temperature=temperature,
+            render_args={"__choices": choice_strings},
         )
 
-        super().__init__(program, parse_score_fn, choice_scores)
-
     @classmethod
-    def from_spec(cls, spec: ModelGradedSpec, **kwargs):
-        return cls(spec.prompt, spec.choice_scores, **kwargs)
+    def from_spec(cls, name: str, spec: ModelGradedSpec, **kwargs):
+        return cls(name, spec.prompt, spec.choice_scores, **kwargs)
 
     @classmethod
-    def from_spec_file(cls, path: str, **kwargs):
+    def from_spec_file(cls, name: str, path: str, **kwargs):
         with open(path) as f:
             spec = yaml.safe_load(f)
-        return cls.from_spec(ModelGradedSpec(**spec), **kwargs)
+        return cls.from_spec(name, ModelGradedSpec(**spec), **kwargs)
 
 
 def _build_template_class(name: str):
     class C(LLMClassifier):
         def __new__(cls, model=None, use_cot=None, max_tokens=None, temperature=None):
             kwargs = {}
             if model is not None:
@@ -167,24 +209,27 @@
                 kwargs["use_cot"] = use_cot
             if max_tokens is not None:
                 kwargs["max_tokens"] = max_tokens
             if temperature is not None:
                 kwargs["temperature"] = temperature
 
             # convert FooBar to foo_bar
-            template_name = re.sub(r"(?<!^)(?=[A-Z])", "_", name).lower() + ".yaml"
+            template_name = re.sub(r"(?<!^)(?=[A-Z])", "_", name).lower()
 
-            if not os.path.exists(os.path.join(SCRIPT_DIR, "templates", template_name)):
+            template_path = os.path.join(SCRIPT_DIR, "..", "..", "templates", template_name + ".yaml")
+            if not os.path.exists(template_path):
                 raise AttributeError(f"Model template {name} not found")
 
-            return LLMClassifier.from_spec_file(os.path.join(SCRIPT_DIR, "templates", template_name), **kwargs)
+            return LLMClassifier.from_spec_file(template_name, template_path, **kwargs)
 
     return C
 
 
-def _init_model_templates():
-    for model_template in MODEL_TEMPLATES:
-        globals()[model_template] = _build_template_class(model_template)
-
-
-_init_model_templates()
-__all__ = ["GuidanceLLMClassifier", "LLMClassifier"] + list(MODEL_TEMPLATES)
+# This makes static analysis tools happier
+Battle = _build_template_class("Battle")
+ClosedQA = _build_template_class("ClosedQA")
+Humor = _build_template_class("Humor")
+Factuality = _build_template_class("Factuality")
+Possible = _build_template_class("Possible")
+Security = _build_template_class("Security")
+Summary = _build_template_class("Summary")
+Translation = _build_template_class("Translation")
```

### Comparing `autoevals-0.0.5/src/autoevals/templates/factuality.yaml` & `autoevals-0.0.6/templates/factuality.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.5/src/autoevals/templates/possible.yaml` & `autoevals-0.0.6/templates/possible.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.5/src/autoevals/templates/sql.yaml` & `autoevals-0.0.6/templates/sql.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.5/src/autoevals/templates/translation.yaml` & `autoevals-0.0.6/templates/translation.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.5/src/autoevals/test_llm.py` & `autoevals-0.0.6/py/autoevals/test_llm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,130 +1,135 @@
 import os
 
-import diskcache
-from guidance.llms.caches import DiskCache
+from autoevals.oai import set_cache_dir
 
 
-# By default, guidance uses the user's cache directory (e.g. in the Library/Caches dir on macOS)
+# By default, we use the user's tmp cache directory (e.g. in the Library/Caches dir on macOS)
 # However, we'd like to cache (and commit) the results of our tests, so we monkey patch the library
 # to use a cache directory in the project root.
 _SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
-CACHE_DIR = os.path.join(_SCRIPT_DIR, "../../.testcache")
-os.makedirs(CACHE_DIR, exist_ok=True)
-
-
-def diskcache_init(self, llm_name: str):
-    self._diskcache = diskcache.Cache(os.path.join(CACHE_DIR, f"_{llm_name}.diskcache"))
-
-
-DiskCache.__init__ = diskcache_init
+set_cache_dir(os.path.join(_SCRIPT_DIR, "../../.testcache"))
 
 
 import asyncio
 import re
 
-import guidance
-
 from autoevals.llm import *
 
 
-def test_guidance():
+def test_openai():
     def parse_best_title(grade):
-        return int(re.findall(r"Winner: (\d+)", grade["summary"])[0])
+        return int(re.findall(r"Winner: (\d+)", grade)[0])
 
-    e = GuidanceLLMClassifier(
-        guidance(
-            """
-  {{#system~}}
-  You are a technical project manager who helps software engineers generate better titles for their GitHub issues.
-  You will look at the issue description, and pick which of two titles better describes it.
-  {{~/system}}
-
-  {{#user~}}
-  I'm going to provide you with the issue description, and two possible titles.
-
-  Issue Description: {{page_content}}
-
-  Title 1: {{output}}
-  Title 2: {{expected}}
-
-  Please discuss each title briefly (one line for pros, one for cons), and then pick which one you think more accurately
-  summarizes the issue by writing "Winner: 1" or "Winner: 2", and then a short rationale for your choice.
-  {{~/user}}
-
-  {{#assistant~}}
-  {{gen 'summary' max_tokens=__max_tokens temperature=0}}
-  {{~/assistant}}""",
-            llm=guidance.llms.OpenAI("gpt-3.5-turbo"),
-        ),
-        parse_best_title,
-        {1: 1, 2: 0},
+    e = OpenAILLMClassifier(
+        "title",
+        messages=[
+            {
+                "role": "system",
+                "content": """\
+You are a technical project manager who helps software engineers generate better titles for their GitHub issues.
+You will look at the issue description, and pick which of two titles better describes it.""",
+            },
+            {
+                "role": "user",
+                "content": """\
+I'm going to provide you with the issue description, and two possible titles.
+
+Issue Description: {{page_content}}
+
+Title 1: {{output}}
+Title 2: {{expected}}
+
+Please discuss each title briefly (one line for pros, one for cons), and then pick which one you think more accurately
+summarizes the issue by writing "Winner: 1" or "Winner: 2", and then a short rationale for your choice.""",
+            },
+        ],
+        model="gpt-3.5-turbo",
+        parse_score_fn=parse_best_title,
+        choice_scores={1: 1, 2: 0},
+        max_tokens=500,
     )
 
     page_content = """
-    As suggested by Nicolo, we should standardize the error responses coming from GoTrue, postgres, and realtime (and any other/future APIs) so that it's better DX when writing a client,
+As suggested by Nicolo, we should standardize the error responses coming from GoTrue, postgres, and realtime (and any other/future APIs) so that it's better DX when writing a client,
 
-    We can make this change on the servers themselves, but since postgrest and gotrue are fully/partially external may be harder to change, it might be an option to transform the errors within the client libraries/supabase-js, could be messy?
+We can make this change on the servers themselves, but since postgrest and gotrue are fully/partially external may be harder to change, it might be an option to transform the errors within the client libraries/supabase-js, could be messy?
 
-    Nicolo also dropped this as a reference: http://spec.openapis.org/oas/v3.0.3#openapi-specification"""
+Nicolo also dropped this as a reference: http://spec.openapis.org/oas/v3.0.3#openapi-specification"""
 
     gen_title = "Standardize error responses from GoTrue, Postgres, and Realtime APIs for better DX"
-    original_title = "Standardize Error Responses across APIs"
+    original_title = "This title has nothing to do with the content"
 
-    response = e(gen_title, original_title, page_content=page_content, __max_tokens=500)
+    response = e(gen_title, original_title, page_content=page_content)
     print(response.as_json(indent=2))
     assert response.score == 1
     assert response.error is None
 
 
 def test_llm_classifier():
     for use_cot in [True, False]:
         e = LLMClassifier(
+            "title",
             """
-    You are a technical project manager who helps software engineers generate better titles for their GitHub issues.
-    You will look at the issue description, and pick which of two titles better describes it.
-
-    I'm going to provide you with the issue description, and two possible titles.
+You are a technical project manager who helps software engineers generate better titles for their GitHub issues.
+You will look at the issue description, and pick which of two titles better describes it.
 
-    Issue Description: {{page_content}}
+I'm going to provide you with the issue description, and two possible titles.
 
-    1: {{output}}
-    2: {{expected}}
+Issue Description: {{page_content}}
 
-    Please discuss each title briefly (one line for pros, one for cons).
-    """,
+1: {{output}}
+2: {{expected}}""",
             {"1": 1, "2": 0},
             use_cot=use_cot,
         )
 
         page_content = """
-        As suggested by Nicolo, we should standardize the error responses coming from GoTrue, postgres, and realtime (and any other/future APIs) so that it's better DX when writing a client,
+As suggested by Nicolo, we should standardize the error responses coming from GoTrue, postgres, and realtime (and any other/future APIs) so that it's better DX when writing a client,
 
-        We can make this change on the servers themselves, but since postgrest and gotrue are fully/partially external may be harder to change, it might be an option to transform the errors within the client libraries/supabase-js, could be messy?
+We can make this change on the servers themselves, but since postgrest and gotrue are fully/partially external may be harder to change, it might be an option to transform the errors within the client libraries/supabase-js, could be messy?
 
-        Nicolo also dropped this as a reference: http://spec.openapis.org/oas/v3.0.3#openapi-specification"""
+Nicolo also dropped this as a reference: http://spec.openapis.org/oas/v3.0.3#openapi-specification"""
 
         gen_title = "Standardize error responses from GoTrue, Postgres, and Realtime APIs for better DX"
-        original_title = "Standardize Error Responses across APIs"
+        original_title = "This title has nothing to do with the content"
 
         response = e(gen_title, original_title, page_content=page_content)
         print(response.as_json(indent=2))
         assert response.score == 1
         assert response.error is None
 
+        response = e(original_title, gen_title, page_content=page_content)
+        print(response.as_json(indent=2))
+        assert response.score == 0
+        assert response.error is None
+
 
 def test_nested_async():
     async def nested_async():
         e = Battle()
-        e(instructions="Add the following numbers: 1, 2, 3", output="7", expected="6")
+        e(instructions="Add the following numbers: 1, 2, 3", output="600", expected="6")
 
     asyncio.run(nested_async())
 
 
 def test_battle():
     for use_cot in [True, False]:
+        print("use_cot", use_cot)
         e = Battle(use_cot=use_cot)
-        response = e(instructions="Add the following numbers: 1, 2, 3", output="7", expected="6")
+        response = e(instructions="Add the following numbers: 1, 2, 3", output="600", expected="6")
+
+        print(response.as_json(indent=2))
+        assert response.score == 0
+        assert response.error is None
+
+        response = e(instructions="Add the following numbers: 1, 2, 3", output="6", expected="600")
+
+        print(response.as_json(indent=2))
+        assert response.score == (1 if use_cot else 0)
+        assert response.error is None
+
+        response = e(instructions="Add the following numbers: 1, 2, 3", output="6", expected="6")
 
         print(response.as_json(indent=2))
         assert response.score == 0
         assert response.error is None
```

### Comparing `autoevals-0.0.5/src/autoevals/test_string.py` & `autoevals-0.0.6/py/autoevals/test_string.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from autoevals.string import LevenshteinEvaluator
+from autoevals.string import LevenshteinScorer
 
 
 def test_levenshtein():
     cases = [
         ("", "", 1),
         ("", "a", 0),
         ("a", "", 0),
@@ -10,11 +10,11 @@
         ("a", "b", 0),
         ("ab", "ac", 0.5),
         ("ac", "bc", 0.5),
         ("abc", "axc", 0.6666666666666667),
         ("xabxcdxxefxgx", "1ab2cd34ef5g6", 0.5384615384615384),
     ]
 
-    evaluator = LevenshteinEvaluator()
+    evaluator = LevenshteinScorer()
     for a, b, expected in cases:
         print(f"[{a}]", f"[{b}]", expected, evaluator(a, b))
         assert evaluator(a, b).score == expected
```

### Comparing `autoevals-0.0.5/src/autoevals.egg-info/PKG-INFO` & `autoevals-0.0.6/py/autoevals.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoevals
-Version: 0.0.5
+Version: 0.0.6
 Summary: Universal library for evaluating AI models
 Home-page: https://www.braintrustdata.com
 Author: BrainTrust
 Author-email: info@braintrustdata.com
 Project-URL: Bug Tracker, https://github.com/braintrustdata/autoevals
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -33,15 +33,16 @@
 their outputs.
 
 You can also create your own model-graded evaluations with AutoEvals. It's easy to add custom prompts, parse outputs,
 and manage exceptions.
 
 ## Installation
 
-To install AutoEvals, run the following command:
+AutoEvals is distributed as a [Python library on PyPI](https://pypi.org/project/autoevals/) and
+[Node.js library on NPM](https://www.npmjs.com/package/autoevals).
 
 ```bash
 pip install autoevals
 ```
 
 ## Example
 
@@ -178,13 +179,7 @@
 expected = "Standardize Error Responses across APIs"
 
 response = evaluator(output, expected, input=page_content)
 
 print(f"Score: {response.score}")
 print(f"Metadata: {response.metadata}")
 ```
-
-## Typescript / Node Support
-
-Since AutoEvals has a very simple prompt template format, it is easy to support in other languages, like
-Typescript (and eventually others). We'll support an npm package soon, but in the meantime, feel free to
-grab model templates from the [prompt templates](/src/autoevals/templates) directory.
```

