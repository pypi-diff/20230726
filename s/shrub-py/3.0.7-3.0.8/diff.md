# Comparing `tmp/shrub_py-3.0.7.tar.gz` & `tmp/shrub_py-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shrub_py-3.0.7.tar", max compression
+gzip compressed data, was "shrub_py-3.0.8.tar", max compression
```

## Comparing `shrub_py-3.0.7.tar` & `shrub_py-3.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11536 2023-07-14 20:00:24.977757 shrub_py-3.0.7/LICENSE
--rw-r--r--   0        0        0     1285 2023-07-14 20:00:24.977757 shrub_py-3.0.7/README.md
--rw-r--r--   0        0        0      837 2023-07-14 20:00:24.981757 shrub_py-3.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/__init__.py
--rw-r--r--   0        0        0     1723 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/base.py
--rw-r--r--   0        0        0     6189 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/command.py
--rw-r--r--   0        0        0     7769 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/config.py
--rw-r--r--   0        0        0    28873 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/operations.py
--rw-r--r--   0        0        0        0 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/py.typed
--rw-r--r--   0        0        0     9305 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/task.py
--rw-r--r--   0        0        0      266 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/__init__.py
--rw-r--r--   0        0        0    22752 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/command.py
--rw-r--r--   0        0        0      992 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/dict_creation_util.py
--rw-r--r--   0        0        0     2386 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/project.py
--rw-r--r--   0        0        0     5561 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/task.py
--rw-r--r--   0        0        0     9669 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v2/variant.py
--rw-r--r--   0        0        0        0 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/__init__.py
--rw-r--r--   0        0        0     1535 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/evg_build_variant.py
--rw-r--r--   0        0        0    33152 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/evg_command.py
--rw-r--r--   0        0        0     3187 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/evg_project.py
--rw-r--r--   0        0        0     1663 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/evg_task.py
--rw-r--r--   0        0        0     1968 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/evg_task_group.py
--rw-r--r--   0        0        0      921 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/v3/shrub_service.py
--rw-r--r--   0        0        0    10210 2023-07-14 20:00:24.981757 shrub_py-3.0.7/src/shrub/variant.py
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 shrub_py-3.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11536 2023-07-26 14:12:12.436263 shrub_py-3.0.8/LICENSE
+-rw-r--r--   0        0        0     1285 2023-07-26 14:12:12.436263 shrub_py-3.0.8/README.md
+-rw-r--r--   0        0        0      850 2023-07-26 14:12:12.436263 shrub_py-3.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/__init__.py
+-rw-r--r--   0        0        0     1723 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/base.py
+-rw-r--r--   0        0        0     6189 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/command.py
+-rw-r--r--   0        0        0     7769 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/config.py
+-rw-r--r--   0        0        0    28873 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/operations.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/py.typed
+-rw-r--r--   0        0        0     9305 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/task.py
+-rw-r--r--   0        0        0      266 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/v2/__init__.py
+-rw-r--r--   0        0        0    22752 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/v2/command.py
+-rw-r--r--   0        0        0      992 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/v2/dict_creation_util.py
+-rw-r--r--   0        0        0     2386 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/v2/project.py
+-rw-r--r--   0        0        0     5561 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/v2/task.py
+-rw-r--r--   0        0        0     9669 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/v2/variant.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/v3/__init__.py
+-rw-r--r--   0        0        0     1535 2023-07-26 14:12:12.436263 shrub_py-3.0.8/src/shrub/v3/evg_build_variant.py
+-rw-r--r--   0        0        0    33152 2023-07-26 14:12:12.440263 shrub_py-3.0.8/src/shrub/v3/evg_command.py
+-rw-r--r--   0        0        0     3187 2023-07-26 14:12:12.440263 shrub_py-3.0.8/src/shrub/v3/evg_project.py
+-rw-r--r--   0        0        0     1663 2023-07-26 14:12:12.440263 shrub_py-3.0.8/src/shrub/v3/evg_task.py
+-rw-r--r--   0        0        0     1968 2023-07-26 14:12:12.440263 shrub_py-3.0.8/src/shrub/v3/evg_task_group.py
+-rw-r--r--   0        0        0      921 2023-07-26 14:12:12.440263 shrub_py-3.0.8/src/shrub/v3/shrub_service.py
+-rw-r--r--   0        0        0    10210 2023-07-26 14:12:12.440263 shrub_py-3.0.8/src/shrub/variant.py
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 shrub_py-3.0.8/PKG-INFO
```

### Comparing `shrub_py-3.0.7/LICENSE` & `shrub_py-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/README.md` & `shrub_py-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/pyproject.toml` & `shrub_py-3.0.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shrub.py"
-version = "3.0.7"
+version = "3.0.8"
 description = "Library for creating evergreen configurations"
 authors = [
     "David Bradford <david.bradford@mongodb.com>",
     "Lydia Stepanek <lydia.stepanek@mongodb.com>",
     "Tausif Rahman <tausif.rahman@mongodb.com>"
 ]
 license = "Apache-2.0"
@@ -12,25 +12,25 @@
 repository = "https://github.com/evergreen-ci/shrub.py"
 packages = [
     { include = "shrub", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">3.7.0"
-PyYaml = "^5.1"
+PyYaml = "^5.1 || ^6.0"
 dataclasses = {version = "^0.7", python = "3.6.*"}
 pydantic = "^1.8"
 git-url-parse = "^1"
 typing-extensions = "^4"
 croniter = "^1.4.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.0"
 pytest-black = "^0.3"
 pytest-flake8 = "^1.0"
 pytest-mypy = "^0.8.0"
 black = "^23.3.0"
-types-PyYAML = "^5.4.10"
+types-PyYAML = "^5.1 || ^6.0"
 flake8 = "3.9.2"
 
 [tool.black]
 line-length = 100
```

### Comparing `shrub_py-3.0.7/src/shrub/base.py` & `shrub_py-3.0.8/src/shrub/base.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/command.py` & `shrub_py-3.0.8/src/shrub/command.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/config.py` & `shrub_py-3.0.8/src/shrub/config.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/operations.py` & `shrub_py-3.0.8/src/shrub/operations.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/task.py` & `shrub_py-3.0.8/src/shrub/task.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v2/command.py` & `shrub_py-3.0.8/src/shrub/v2/command.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v2/dict_creation_util.py` & `shrub_py-3.0.8/src/shrub/v2/dict_creation_util.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v2/project.py` & `shrub_py-3.0.8/src/shrub/v2/project.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v2/task.py` & `shrub_py-3.0.8/src/shrub/v2/task.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v2/variant.py` & `shrub_py-3.0.8/src/shrub/v2/variant.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v3/evg_build_variant.py` & `shrub_py-3.0.8/src/shrub/v3/evg_build_variant.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v3/evg_command.py` & `shrub_py-3.0.8/src/shrub/v3/evg_command.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v3/evg_project.py` & `shrub_py-3.0.8/src/shrub/v3/evg_project.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v3/evg_task.py` & `shrub_py-3.0.8/src/shrub/v3/evg_task.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v3/evg_task_group.py` & `shrub_py-3.0.8/src/shrub/v3/evg_task_group.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/v3/shrub_service.py` & `shrub_py-3.0.8/src/shrub/v3/shrub_service.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/src/shrub/variant.py` & `shrub_py-3.0.8/src/shrub/variant.py`

 * *Files identical despite different names*

### Comparing `shrub_py-3.0.7/PKG-INFO` & `shrub_py-3.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: shrub-py
-Version: 3.0.7
+Version: 3.0.8
 Summary: Library for creating evergreen configurations
 Home-page: https://github.com/evergreen-ci/shrub.py
 License: Apache-2.0
 Author: David Bradford
 Author-email: david.bradford@mongodb.com
 Requires-Python: >3.7.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYaml (>=5.1,<6.0)
+Requires-Dist: PyYaml (>=5.1,<7.0)
 Requires-Dist: croniter (>=1.4.1,<2.0.0)
 Requires-Dist: dataclasses (>=0.7,<0.8) ; python_version >= "3.6.dev0" and python_version < "3.7.dev0"
 Requires-Dist: git-url-parse (>=1,<2)
 Requires-Dist: pydantic (>=1.8,<2.0)
 Requires-Dist: typing-extensions (>=4,<5)
 Project-URL: Repository, https://github.com/evergreen-ci/shrub.py
 Description-Content-Type: text/markdown
```

