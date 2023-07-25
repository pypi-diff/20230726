# Comparing `tmp/dearprudence-1.0.0.tar.gz` & `tmp/dearprudence-1.1.0.tar.gz`

## Comparing `dearprudence-1.0.0.tar` & `dearprudence-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dearprudence-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dearprudence-1.0.0/requirements-dev.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dearprudence-1.0.0/setup.cfg
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 dearprudence-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 dearprudence-1.0.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 dearprudence-1.0.0/.github/workflows/python-publish.yaml
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 dearprudence-1.0.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 dearprudence-1.0.0/src/dearprudence/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 dearprudence-1.0.0/src/dearprudence/_version.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 dearprudence-1.0.0/src/dearprudence/core.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 dearprudence-1.0.0/src/dearprudence/errors.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 dearprudence-1.0.0/src/dearprudence/io.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 dearprudence-1.0.0/src/dearprudence/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dearprudence-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 dearprudence-1.0.0/tests/test_io.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 dearprudence-1.0.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dearprudence-1.0.0/LICENSE
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 dearprudence-1.0.0/README.md
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 dearprudence-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 dearprudence-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 dearprudence-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 dearprudence-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 dearprudence-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 dearprudence-1.1.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 dearprudence-1.1.0/.github/workflows/python-publish.yaml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 dearprudence-1.1.0/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 dearprudence-1.1.0/src/dearprudence/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 dearprudence-1.1.0/src/dearprudence/_version.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 dearprudence-1.1.0/src/dearprudence/core.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 dearprudence-1.1.0/src/dearprudence/errors.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 dearprudence-1.1.0/src/dearprudence/io.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 dearprudence-1.1.0/src/dearprudence/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dearprudence-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 dearprudence-1.1.0/tests/test_io.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 dearprudence-1.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 dearprudence-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 dearprudence-1.1.0/README.md
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 dearprudence-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 dearprudence-1.1.0/PKG-INFO
```

### Comparing `dearprudence-1.0.0/.github/dependabot.yml` & `dearprudence-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dearprudence-1.0.0/.github/workflows/codeql-analysis.yml` & `dearprudence-1.1.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `dearprudence-1.0.0/src/dearprudence/io.py` & `dearprudence-1.1.0/src/dearprudence/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import dataclasses
 import json
 from os import PathLike
-from typing import Union, TextIO, BinaryIO, Any, TypedDict, Sequence
+from typing import Union, TextIO, BinaryIO, Any, TypedDict
+from collections.abc import Sequence
 
 from dearprudence.core import Cmip6Record, SimpleRun
 
 
 __all__ = ["read_params", "write_params"]
 
 
@@ -32,15 +33,15 @@
 def _load_paramfile(
     urlpath: Union[str, Union[TextIO, BinaryIO]]
 ) -> Sequence[SimpleRunMapping]:
     # First readline() to pop-off and discard the first yaml bit of
     # the file, then load as JSON str. Keeps us from depending
     # on pyyaml.
     if isinstance(urlpath, str):
-        with open(urlpath, "r") as fl:
+        with open(urlpath) as fl:
             # Pop off and discard the first "yaml" bit.
             _ = fl.readline()
             return json.load(fl)
     else:
         # Pop off and discard the first "yaml" bit.
         _ = urlpath.readline()
         return json.load(urlpath)
```

### Comparing `dearprudence-1.0.0/src/dearprudence/utils.py` & `dearprudence-1.1.0/src/dearprudence/utils.py`

 * *Files identical despite different names*

### Comparing `dearprudence-1.0.0/tests/test_io.py` & `dearprudence-1.1.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `dearprudence-1.0.0/.gitignore` & `dearprudence-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dearprudence-1.0.0/LICENSE` & `dearprudence-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dearprudence-1.0.0/README.md` & `dearprudence-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dearprudence-1.0.0/pyproject.toml` & `dearprudence-1.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -25,23 +25,20 @@
 "Homepage" = "https://github.com/brews/dearprudence"
 "Bug Tracker" = "https://github.com/brews/dearprudence/issues"
 
 [project.optional-dependencies]
 catalog = [
     "intake_esm",
 ]
-dev = [
+test = [
     "black",
-    "build",
-    "flake8",
-    "intake_esm",
     "mypy",
     "pytest",
     "pytest-cov",
-    "twine",
+    "ruff",
 ]
 
 [tool.hatch.version]
 source = "vcs"
 fallback-version = "999"
 
 [tool.hatch.build.hooks.vcs]
@@ -50,7 +47,27 @@
 [tool.mypy]
 python_version = "3.10"
 warn_unused_configs = true
 
 [[tool.mypy.overrides]]
 module = "intake"
 ignore_missing_imports = true
+
+[tool.ruff]
+exclude = [
+    ".eggs",
+]
+# E402: module level import not at top of file
+# E501: line too long - let black worry about that
+ignore = [
+    "E402",
+    "E501",
+]
+select = [
+    # Pyflakes
+    "F",
+    # Pycodestyle
+    "E",
+    "W",
+    # Pyupgrade
+    "UP",
+]
```

### Comparing `dearprudence-1.0.0/PKG-INFO` & `dearprudence-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dearprudence
-Version: 1.0.0
+Version: 1.1.0
 Summary: Internal Python library filled with sugar for swallowing downscalingCMIP6 parameter files
 Project-URL: Homepage, https://github.com/brews/dearprudence
 Project-URL: Bug Tracker, https://github.com/brews/dearprudence/issues
 Author-email: Brewster Malevich <bmalevich@rhg.com>
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -12,23 +12,20 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.9
 Provides-Extra: catalog
 Requires-Dist: intake-esm; extra == 'catalog'
-Provides-Extra: dev
-Requires-Dist: black; extra == 'dev'
-Requires-Dist: build; extra == 'dev'
-Requires-Dist: flake8; extra == 'dev'
-Requires-Dist: intake-esm; extra == 'dev'
-Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: pytest; extra == 'dev'
-Requires-Dist: pytest-cov; extra == 'dev'
-Requires-Dist: twine; extra == 'dev'
+Provides-Extra: test
+Requires-Dist: black; extra == 'test'
+Requires-Dist: mypy; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-cov; extra == 'test'
+Requires-Dist: ruff; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![Test](https://github.com/brews/dearprudence/actions/workflows/test.yaml/badge.svg)](https://github.com/brews/dearprudence/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/brews/dearprudence/branch/main/graph/badge.svg?token=FZD8KX4RC1)](https://codecov.io/gh/brews/dearprudence)
 
 # dearprudence
 Internal Python library filled with sugar for swallowing downscalingCMIP6 parameter files.
```

