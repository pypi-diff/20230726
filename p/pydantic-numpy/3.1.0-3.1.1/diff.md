# Comparing `tmp/pydantic_numpy-3.1.0.tar.gz` & `tmp/pydantic_numpy-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_numpy-3.1.0.tar", max compression
+gzip compressed data, was "pydantic_numpy-3.1.1.tar", max compression
```

## Comparing `pydantic_numpy-3.1.0.tar` & `pydantic_numpy-3.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-3.1.0/LICENSE
--rw-r--r--   0        0        0     2703 2023-07-25 16:31:55.726059 pydantic_numpy-3.1.0/README.md
--rw-r--r--   0        0        0      138 2023-07-25 15:36:47.472916 pydantic_numpy-3.1.0/pydantic_numpy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 10:48:54.840721 pydantic_numpy-3.1.0/pydantic_numpy/helper/__init__.py
--rw-r--r--   0        0        0     5565 2023-07-25 15:51:56.951261 pydantic_numpy-3.1.0/pydantic_numpy/helper/annotation.py
--rw-r--r--   0        0        0     3891 2023-07-25 15:34:13.657876 pydantic_numpy-3.1.0/pydantic_numpy/helper/validation.py
--rw-r--r--   0        0        0      118 2023-07-25 10:48:54.840721 pydantic_numpy-3.1.0/pydantic_numpy/model/__init__.py
--rw-r--r--   0        0        0     1116 2023-07-25 15:40:17.968604 pydantic_numpy-3.1.0/pydantic_numpy/model/multi_array.py
--rw-r--r--   0        0        0     8605 2023-07-25 15:45:03.591827 pydantic_numpy-3.1.0/pydantic_numpy/model/np_model.py
--rw-r--r--   0        0        0      474 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/i_dimensional.py
--rw-r--r--   0        0        0     2285 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/ii_dimensional.py
--rw-r--r--   0        0        0     2284 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/iii_dimensional.py
--rw-r--r--   0        0        0     2036 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/n_dimensional.py
--rw-r--r--   0        0        0        0 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/__init__.py
--rw-r--r--   0        0        0     2860 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/i_dimensional.py
--rw-r--r--   0        0        0     2860 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
--rw-r--r--   0        0        0     2859 2023-07-25 10:48:54.841721 pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
--rw-r--r--   0        0        0     2578 2023-07-25 10:48:54.842721 pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/n_dimensional.py
--rw-r--r--   0        0        0      868 2023-07-25 16:29:51.865761 pydantic_numpy-3.1.0/pydantic_numpy/util.py
--rw-r--r--   0        0        0     1181 2023-07-25 11:13:47.189996 pydantic_numpy-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     3651 1970-01-01 00:00:00.000000 pydantic_numpy-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-03-01 05:05:36.172059 pydantic_numpy-3.1.1/LICENSE
+-rw-r--r--   0        0        0     2703 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.1/README.md
+-rw-r--r--   0        0        0      138 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.1/pydantic_numpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 16:46:39.932073 pydantic_numpy-3.1.1/pydantic_numpy/helper/__init__.py
+-rw-r--r--   0        0        0     5502 2023-07-25 16:46:48.615024 pydantic_numpy-3.1.1/pydantic_numpy/helper/annotation.py
+-rw-r--r--   0        0        0     3891 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/helper/validation.py
+-rw-r--r--   0        0        0      118 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/model/__init__.py
+-rw-r--r--   0        0        0     1116 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/model/multi_array.py
+-rw-r--r--   0        0        0     8605 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/model/np_model.py
+-rw-r--r--   0        0        0      474 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/i_dimensional.py
+-rw-r--r--   0        0        0     2285 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/ii_dimensional.py
+-rw-r--r--   0        0        0     2284 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/iii_dimensional.py
+-rw-r--r--   0        0        0     2036 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/n_dimensional.py
+-rw-r--r--   0        0        0        0 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/__init__.py
+-rw-r--r--   0        0        0     2860 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/i_dimensional.py
+-rw-r--r--   0        0        0     2860 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/ii_dimensional.py
+-rw-r--r--   0        0        0     2859 2023-07-25 16:46:39.933073 pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/iii_dimensional.py
+-rw-r--r--   0        0        0     2578 2023-07-25 16:46:39.934073 pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/n_dimensional.py
+-rw-r--r--   0        0        0     1621 2023-07-26 10:42:16.751707 pydantic_numpy-3.1.1/pydantic_numpy/util.py
+-rw-r--r--   0        0        0     1206 2023-07-26 10:44:36.410938 pydantic_numpy-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 pydantic_numpy-3.1.1/PKG-INFO
```

### Comparing `pydantic_numpy-3.1.0/LICENSE` & `pydantic_numpy-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/README.md` & `pydantic_numpy-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/helper/annotation.py` & `pydantic_numpy-3.1.1/pydantic_numpy/helper/annotation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from collections.abc import Sequence
 from pathlib import Path
 from typing import Any, Callable, ClassVar, Optional, Union
 
 import numpy as np
-import numpy.typing as npt
-from numpy.lib.npyio import NpzFile
 from numpy.typing import DTypeLike
 from pydantic import FilePath, GetJsonSchemaHandler, PositiveInt
 from pydantic.json_schema import JsonSchemaValue
 from pydantic_core import core_schema
 from typing_extensions import Annotated
 
 from pydantic_numpy.helper.validation import (
```

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/helper/validation.py` & `pydantic_numpy-3.1.1/pydantic_numpy/helper/validation.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/model/multi_array.py` & `pydantic_numpy-3.1.1/pydantic_numpy/model/multi_array.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/model/np_model.py` & `pydantic_numpy-3.1.1/pydantic_numpy/model/np_model.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/typing/i_dimensional.py` & `pydantic_numpy-3.1.1/pydantic_numpy/typing/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/typing/ii_dimensional.py` & `pydantic_numpy-3.1.1/pydantic_numpy/typing/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/typing/iii_dimensional.py` & `pydantic_numpy-3.1.1/pydantic_numpy/typing/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/typing/n_dimensional.py` & `pydantic_numpy-3.1.1/pydantic_numpy/typing/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/i_dimensional.py` & `pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/i_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/ii_dimensional.py` & `pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/ii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/iii_dimensional.py` & `pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/iii_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pydantic_numpy/typing/strict_data_type/n_dimensional.py` & `pydantic_numpy-3.1.1/pydantic_numpy/typing/strict_data_type/n_dimensional.py`

 * *Files identical despite different names*

### Comparing `pydantic_numpy-3.1.0/pyproject.toml` & `pydantic_numpy-3.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic_numpy"
-version = "3.1.0"
+version = "3.1.1"
 description = "Pydantic Model integration of the NumPy array"
 authors = ["Can H. Tartanoglu", "Christoph Heindl"]
 maintainers = ["Can H. Tartanoglu <python@rotas.mozmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/caniko/pydantic-numpy"
 license = "BSD-4"
 
@@ -18,16 +18,17 @@
 packages = [{include = "pydantic_numpy"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 compress-pickle = { version = "*", extras = ["lz4"] }
 ruamel-yaml = "^0.17.21"
 
-numpy = "*"
+numpy = ">=1.23.0"
 pydantic = "^2.0"
+semver = "^3.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 parameterized = "^0.9.0"
 hypothesis = "^6.82.0"
 setuptools = "^68.0.0"
```

### Comparing `pydantic_numpy-3.1.0/PKG-INFO` & `pydantic_numpy-3.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-numpy
-Version: 3.1.0
+Version: 3.1.1
 Summary: Pydantic Model integration of the NumPy array
 Home-page: https://github.com/caniko/pydantic-numpy
 License: BSD-4
 Keywords: pydantic,numpy,typing
 Author: Can H. Tartanoglu
 Maintainer: Can H. Tartanoglu
 Maintainer-email: python@rotas.mozmail.com
@@ -14,17 +14,18 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: compress-pickle[lz4]
-Requires-Dist: numpy
+Requires-Dist: numpy (>=1.23.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
+Requires-Dist: semver (>=3.0.1,<4.0.0)
 Description-Content-Type: text/markdown
 
 # pydantic-numpy
 
 Package that integrates NumPy Arrays into Pydantic!
 
 - `NumpyModel` make it possible to dump and load `np.ndarray` within model fields alongside other fields that are not instances of `np.ndarray`!
```

