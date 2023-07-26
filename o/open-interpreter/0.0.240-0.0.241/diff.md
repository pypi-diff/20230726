# Comparing `tmp/open_interpreter-0.0.240.tar.gz` & `tmp/open_interpreter-0.0.241.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_interpreter-0.0.240.tar", max compression
+gzip compressed data, was "open_interpreter-0.0.241.tar", max compression
```

## Comparing `open_interpreter-0.0.240.tar` & `open_interpreter-0.0.241.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.240/LICENSE
--rw-r--r--   0        0        0     6298 2023-07-26 02:40:39.627654 open_interpreter-0.0.240/README.md
--rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.240/interpreter/__init__.py
--rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.240/interpreter/exec.py
--rw-r--r--   0        0        0     9021 2023-07-26 02:25:34.682450 open_interpreter-0.0.240/interpreter/interpreter.py
--rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.240/interpreter/json_utils.py
--rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.240/interpreter/openai_utils.py
--rw-r--r--   0        0        0     2415 2023-07-25 06:33:34.228431 open_interpreter-0.0.240/interpreter/system_message.txt
--rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.240/interpreter/view.py
--rw-r--r--   0        0        0      556 2023-07-26 02:40:51.532696 open_interpreter-0.0.240/pyproject.toml
--rw-r--r--   0        0        0     6922 1970-01-01 00:00:00.000000 open_interpreter-0.0.240/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-14 08:56:39.307343 open_interpreter-0.0.241/LICENSE
+-rw-r--r--   0        0        0     6298 2023-07-26 02:40:39.627654 open_interpreter-0.0.241/README.md
+-rw-r--r--   0        0        0      588 2023-07-26 18:16:13.669608 open_interpreter-0.0.241/cli/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-19 07:01:13.263887 open_interpreter-0.0.241/interpreter/__init__.py
+-rw-r--r--   0        0        0     7192 2023-07-24 03:01:01.276835 open_interpreter-0.0.241/interpreter/exec.py
+-rw-r--r--   0        0        0     9021 2023-07-26 02:25:34.682450 open_interpreter-0.0.241/interpreter/interpreter.py
+-rw-r--r--   0        0        0     3665 2023-07-19 04:08:44.789294 open_interpreter-0.0.241/interpreter/json_utils.py
+-rw-r--r--   0        0        0     6047 2023-07-24 02:40:53.069287 open_interpreter-0.0.241/interpreter/openai_utils.py
+-rw-r--r--   0        0        0     2415 2023-07-25 06:33:34.228431 open_interpreter-0.0.241/interpreter/system_message.txt
+-rw-r--r--   0        0        0     3243 2023-07-24 05:09:39.175621 open_interpreter-0.0.241/interpreter/view.py
+-rw-r--r--   0        0        0      578 2023-07-26 18:16:41.247290 open_interpreter-0.0.241/pyproject.toml
+-rw-r--r--   0        0        0     6922 1970-01-01 00:00:00.000000 open_interpreter-0.0.241/PKG-INFO
```

### Comparing `open_interpreter-0.0.240/LICENSE` & `open_interpreter-0.0.241/LICENSE`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.240/README.md` & `open_interpreter-0.0.241/README.md`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.240/interpreter/exec.py` & `open_interpreter-0.0.241/interpreter/exec.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.240/interpreter/interpreter.py` & `open_interpreter-0.0.241/interpreter/interpreter.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.240/interpreter/json_utils.py` & `open_interpreter-0.0.241/interpreter/json_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.240/interpreter/openai_utils.py` & `open_interpreter-0.0.241/interpreter/openai_utils.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.240/interpreter/system_message.txt` & `open_interpreter-0.0.241/interpreter/system_message.txt`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.240/interpreter/view.py` & `open_interpreter-0.0.241/interpreter/view.py`

 * *Files identical despite different names*

### Comparing `open_interpreter-0.0.240/pyproject.toml` & `open_interpreter-0.0.241/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "open-interpreter"
 packages = [
-    {include = "interpreter"}
+    {include = "interpreter"},
+    {include = "cli"}
 ]
-version = "0.0.240"
+version = "0.0.241"
 description = "Ask GPT-4 to run code locally."
 authors = ["Killian Lucas <killian@drinkwater.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
@@ -20,8 +21,8 @@
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-interpreter = "cli:main"
+interpreter = "cli:cli"
```

### Comparing `open_interpreter-0.0.240/PKG-INFO` & `open_interpreter-0.0.241/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-interpreter
-Version: 0.0.240
+Version: 0.0.241
 Summary: Ask GPT-4 to run code locally.
 Author: Killian Lucas
 Author-email: killian@drinkwater.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

