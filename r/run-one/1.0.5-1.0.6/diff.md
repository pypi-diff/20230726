# Comparing `tmp/run_one-1.0.5.tar.gz` & `tmp/run_one-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_one-1.0.5.tar", max compression
+gzip compressed data, was "run_one-1.0.6.tar", max compression
```

## Comparing `run_one-1.0.5.tar` & `run_one-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-07-25 14:52:21.056223 run_one-1.0.5/LICENSE
--rw-r--r--   0        0        0     1708 2023-07-25 14:52:21.056223 run_one-1.0.5/README.md
--rw-r--r--   0        0        0      741 2023-07-25 14:52:21.056223 run_one-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      345 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/__init__.py
--rw-r--r--   0        0        0      282 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/action_handlers/SleepHandler.py
--rw-r--r--   0        0        0     1916 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/action_handlers/TH2ActHandler.py
--rw-r--r--   0        0        0     1182 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/action_handlers/TH2ActSSHHandler.py
--rw-r--r--   0        0        0     3391 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/action_handlers/TH2Check1Handler.py
--rw-r--r--   0        0        0        0 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/action_handlers/__init__.py
--rw-r--r--   0        0        0      325 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/action_handlers/abstract_action_handler.py
--rw-r--r--   0        0        0      304 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/action_handlers/context.py
--rw-r--r--   0        0        0        0 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/processors/__init__.py
--rw-r--r--   0        0        0     1339 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/processors/abstract_processor.py
--rw-r--r--   0        0        0     5608 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/processors/th2_processor.py
--rw-r--r--   0        0        0        0 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/util/__init__.py
--rw-r--r--   0        0        0     1501 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/util/config.py
--rw-r--r--   0        0        0     3225 2023-07-25 14:52:21.056223 run_one-1.0.5/run_one/util/util.py
--rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 run_one-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-26 12:59:01.279157 run_one-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1708 2023-07-26 12:59:01.279157 run_one-1.0.6/README.md
+-rw-r--r--   0        0        0      740 2023-07-26 12:59:01.279157 run_one-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      345 2023-07-26 12:59:01.279157 run_one-1.0.6/run_one/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-26 12:59:01.279157 run_one-1.0.6/run_one/action_handlers/SleepHandler.py
+-rw-r--r--   0        0        0     1916 2023-07-26 12:59:01.279157 run_one-1.0.6/run_one/action_handlers/TH2ActHandler.py
+-rw-r--r--   0        0        0     1182 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/action_handlers/TH2ActSSHHandler.py
+-rw-r--r--   0        0        0     3391 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/action_handlers/TH2Check1Handler.py
+-rw-r--r--   0        0        0        0 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/action_handlers/__init__.py
+-rw-r--r--   0        0        0      325 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/action_handlers/abstract_action_handler.py
+-rw-r--r--   0        0        0      304 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/action_handlers/context.py
+-rw-r--r--   0        0        0        0 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/processors/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/processors/abstract_processor.py
+-rw-r--r--   0        0        0     5608 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/processors/th2_processor.py
+-rw-r--r--   0        0        0        0 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/util/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/util/config.py
+-rw-r--r--   0        0        0     3225 2023-07-26 12:59:01.283157 run_one-1.0.6/run_one/util/util.py
+-rw-r--r--   0        0        0     2649 1970-01-01 00:00:00.000000 run_one-1.0.6/PKG-INFO
```

### Comparing `run_one-1.0.5/LICENSE` & `run_one-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `run_one-1.0.5/README.md` & `run_one-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `run_one-1.0.5/pyproject.toml` & `run_one-1.0.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "run-one"
-version = "1.0.5"
+version = "1.0.6"
 description = "Tool for parsing matrix files, extracting actions and processing them according to user defined logic"
 authors = ["TH2-devs <th2-devs@exactprosystems.com>"]
 readme = "README.md"
 license = "Apache License 2.0"
 homepage = "https://github.com/th2-net/run-one"
 repository = "https://github.com/th2-net/run-one"
 packages = [
     {include = 'run_one'},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 pandas = "^2.0.3"
 pyyaml = "^6.0"
 th2-common = "^4"
 th2-grpc-act-template = "^4.0.1"
 th2-grpc-check1 = "^4.1.1"
 th2-grpc-act-ssh = "^2.0.0"
```

### Comparing `run_one-1.0.5/run_one/action_handlers/TH2ActHandler.py` & `run_one-1.0.6/run_one/action_handlers/TH2ActHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.5/run_one/action_handlers/TH2ActSSHHandler.py` & `run_one-1.0.6/run_one/action_handlers/TH2ActSSHHandler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.5/run_one/action_handlers/TH2Check1Handler.py` & `run_one-1.0.6/run_one/action_handlers/TH2Check1Handler.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.5/run_one/processors/abstract_processor.py` & `run_one-1.0.6/run_one/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.5/run_one/processors/th2_processor.py` & `run_one-1.0.6/run_one/processors/th2_processor.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.5/run_one/util/config.py` & `run_one-1.0.6/run_one/util/config.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.5/run_one/util/util.py` & `run_one-1.0.6/run_one/util/util.py`

 * *Files identical despite different names*

### Comparing `run_one-1.0.5/PKG-INFO` & `run_one-1.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: run-one
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tool for parsing matrix files, extracting actions and processing them according to user defined logic
 Home-page: https://github.com/th2-net/run-one
 License: Apache-2.0
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: th2-common (>=4,<5)
 Requires-Dist: th2-grpc-act-ssh (>=2.0.0,<3.0.0)
 Requires-Dist: th2-grpc-act-template (>=4.0.1,<5.0.0)
```

