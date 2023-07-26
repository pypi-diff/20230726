# Comparing `tmp/idefix_cli-2.3.1.tar.gz` & `tmp/idefix_cli-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idefix_cli-2.3.1.tar", last modified: Wed Jul 12 12:20:36 2023, max compression
+gzip compressed data, was "idefix_cli-2.3.2.tar", last modified: Wed Jul 26 17:12:39 2023, max compression
```

## Comparing `idefix_cli-2.3.1.tar` & `idefix_cli-2.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:36.469917 idefix_cli-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-12 12:20:36.469917 idefix_cli-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 12:20:36.469917 idefix_cli-2.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:36.465917 idefix_cli-2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:36.469917 idefix_cli-2.3.1/src/idefix_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_backports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:36.469917 idefix_cli-2.3.1/src/idefix_cli/_commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_commands/clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_commands/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_commands/stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_commands/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_commands/write.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/src/idefix_cli/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:36.469917 idefix_cli-2.3.1/src/idefix_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-12 12:20:36.000000 idefix_cli-2.3.1/src/idefix_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-12 12:20:36.000000 idefix_cli-2.3.1/src/idefix_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 12:20:36.000000 idefix_cli-2.3.1/src/idefix_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-12 12:20:36.000000 idefix_cli-2.3.1/src/idefix_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-12 12:20:36.000000 idefix_cli-2.3.1/src/idefix_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 12:20:36.000000 idefix_cli-2.3.1/src/idefix_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 12:20:36.469917 idefix_cli-2.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_app_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_stamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-12 12:20:26.000000 idefix_cli-2.3.1/tests/test_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.339352 idefix_cli-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-26 17:12:39.339352 idefix_cli-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:12:39.339352 idefix_cli-2.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.335352 idefix_cli-2.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.335352 idefix_cli-2.3.2/src/idefix_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_backports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.339352 idefix_cli-2.3.2/src/idefix_cli/_commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_commands/write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/src/idefix_cli/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.335352 idefix_cli-2.3.2/src/idefix_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-26 17:12:39.000000 idefix_cli-2.3.2/src/idefix_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:12:39.339352 idefix_cli-2.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_app_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-07-26 17:12:27.000000 idefix_cli-2.3.2/tests/test_write.py
```

### Comparing `idefix_cli-2.3.1/LICENSE` & `idefix_cli-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/PKG-INFO` & `idefix_cli-2.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: idefix_cli
-Version: 2.3.1
+Version: 2.3.2
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: isolated
 License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/idefix_cli.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/idefix-cli/)
-![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)
 [![Documentation Status](https://readthedocs.org/projects/idefix-cli/badge/?version=latest)](https://idefix-cli.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 # `idefix_cli`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `idefix_cli-2.3.1/README.md` & `idefix_cli-2.3.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 [![PyPI](https://img.shields.io/pypi/v/idefix_cli.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/idefix-cli/)
-![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)
 [![Documentation Status](https://readthedocs.org/projects/idefix-cli/badge/?version=latest)](https://idefix-cli.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 # `idefix_cli`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `idefix_cli-2.3.1/pyproject.toml` & `idefix_cli-2.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 description = "A CLI to automate mundane tasks with Idefix"
 authors = [
     { name = "C.M.T. Robert" },
 ]
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
     "Typing :: Typed",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "gitpython>=3.1.18",
     "inifix>=3.0.0",
     "packaging>=21.0",
     "rich>=10.7.0",
     "typing-extensions>=4.1.0;python_version < '3.11'",
 ]
@@ -79,15 +78,15 @@
 ]
 
 [tool.ruff.isort]
 combine-as-imports = true
 known-first-party = ["idefix_cli"]
 
 [tool.mypy]
-python_version = 3.8
+python_version = 3.9
 show_error_codes = true
 ignore_missing_imports = true
 warn_unused_configs = true
 warn_unused_ignores = true
 warn_unreachable = true
 show_error_context = true
```

### Comparing `idefix_cli-2.3.1/src/idefix_cli/__main__.py` & `idefix_cli-2.3.2/src/idefix_cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import inspect
 import os
 import sys
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 from types import FunctionType, ModuleType
-from typing import Any, Dict, Final, List, Optional, Tuple
+from typing import Any, Final, Optional
 
 from rich.console import Console
 
 from idefix_cli import __version__
 from idefix_cli._theme import set_theme
 from idefix_cli.lib import get_config_file, get_option, print_err, print_warning
 
-CommandMap = Dict[str, Tuple[FunctionType, bool]]
+CommandMap = dict[str, tuple[FunctionType, bool]]
 
 
 BASE_COMMAND_PATH: Final[str] = str(Path(__file__).parent / "_commands")
 
 
-def _get_command_paths() -> List[str]:
+def _get_command_paths() -> list[str]:
     dirs = [BASE_COMMAND_PATH]
 
     if ext_dir_v1 := get_option("idefix_cli", "extension_dir"):
         print_warning(
             "The 'extension_dir' option is deprecated. Use 'plugins_directory' instead."
         )
 
@@ -116,15 +116,15 @@
             param.kind is param.VAR_POSITIONAL for param in sig.parameters.values()
         )
         cmddict.update({command_name: (module.command, accepts_unknown_args)})
     return cmddict
 
 
 def main(
-    argv: "List[str] | None" = None, parser: "ArgumentParser | None" = None
+    argv: "list[str] | None" = None, parser: "ArgumentParser | None" = None
 ) -> Any:
     # the return value is deleguated to sub commands so its type is arbitrary
     # In practice it should be either 'int' or 'typing.NoReturn'
     if parser is None:
         parser = ArgumentParser(prog="idfx", allow_abbrev=False)
     parser.add_argument("-v", "--version", action="version", version=__version__)
     commands = _setup_commands(parser)
@@ -144,15 +144,15 @@
     if unknown_args and not accepts_unknown_args:
         print_err(f"received unknown arguments {tuple(unknown_args)!r}")
         return 1
 
     return cmd(*unknown_args, **vars(known_args))
 
 
-def alt_main(argv: "List[str] | None" = None) -> Any:
+def alt_main(argv: "list[str] | None" = None) -> Any:
     console = Console(width=500, highlight=False)
     console.print(":tennis: :arrow_forward:")
 
     set_theme("baballe")
     try:
         retv = main(argv, parser=ArgumentParser(prog="baballe", allow_abbrev=False))
     finally:
```

### Comparing `idefix_cli-2.3.1/src/idefix_cli/_backports.py` & `idefix_cli-2.3.2/src/idefix_cli/_backports.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/src/idefix_cli/_commands/clean.py` & `idefix_cli-2.3.2/src/idefix_cli/_commands/clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/src/idefix_cli/_commands/clone.py` & `idefix_cli-2.3.2/src/idefix_cli/_commands/clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/src/idefix_cli/_commands/conf.py` & `idefix_cli-2.3.2/src/idefix_cli/_commands/conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/src/idefix_cli/_commands/read.py` & `idefix_cli-2.3.2/src/idefix_cli/_commands/read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/src/idefix_cli/_commands/run.py` & `idefix_cli-2.3.2/src/idefix_cli/_commands/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 from copy import deepcopy
 from enum import auto
 from math import prod
 from multiprocessing import cpu_count
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from time import sleep, time
+from time import sleep, time, time_ns
 from typing import Final
 
 import inifix
 from packaging.version import Version
 from rich.prompt import Confirm
 
 from idefix_cli.lib import (
@@ -429,28 +429,36 @@
         inputfile = tmp_inifile.name
     else:
         inputfile = str(pinifile.relative_to(d.resolve()))
 
     cmd = get_command(inputfile, nproc=nproc, idefix_args=unknown_args)
 
     print_subcommand(cmd, loc=d)
+
     if get_idefix_version() >= Version("1.0.0"):
+        tstart = time_ns()
         with chdir(d):
             ret = subprocess.call(cmd)
 
-        if ret == 0:
+        logfile = d / MAIN_LOG_FILE
+        if ret == 0 and logfile.is_file() and logfile.stat().st_mtime_ns > tstart:
             # Idefix >= 1.0 intentionally always returns 0, even on failure
             with open(d / MAIN_LOG_FILE) as fh:
                 last_line = fh.read().strip().split("\n")[-1].strip()
             if last_line in KNOWN_FAIL:
                 ret = 1
             elif last_line not in KNOWN_SUCCESS:
                 print_warning(
                     "Command completed with an unknown status. Please check log files."
                 )
+        else:
+            # Either the retcode is !=0 or no log files were produced, which may be
+            # perfectly legit (-nolog and -nowrite exist). In any case, resist the
+            # temptation to guess what happened.
+            pass
 
     else:
         with chdir(d):
             ret = _spawn_idefix_lt_1(cmd, ncycles=ncycles)
 
         if ret < 0:
             # special retcodes from spawn_idefix
```

### Comparing `idefix_cli-2.3.1/src/idefix_cli/_commands/stamp.py` & `idefix_cli-2.3.2/src/idefix_cli/_commands/stamp.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/src/idefix_cli/_commands/switch.py` & `idefix_cli-2.3.2/src/idefix_cli/_commands/switch.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/src/idefix_cli/_commands/write.py` & `idefix_cli-2.3.2/src/idefix_cli/_commands/write.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/src/idefix_cli/lib.py` & `idefix_cli-2.3.2/src/idefix_cli/lib.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/src/idefix_cli.egg-info/PKG-INFO` & `idefix_cli-2.3.2/src/idefix_cli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: idefix-cli
-Version: 2.3.1
+Version: 2.3.2
 Summary: A CLI to automate mundane tasks with Idefix
 Author: C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/neutrinoceros/idefix_cli
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: isolated
 License-File: LICENSE
 
 [![PyPI](https://img.shields.io/pypi/v/idefix_cli.svg?logo=pypi&logoColor=white&label=PyPI)](https://pypi.org/project/idefix-cli/)
-![PyPI](https://img.shields.io/badge/requires-Python%20≥%203.8-blue?logo=python&logoColor=white)
 [![Documentation Status](https://readthedocs.org/projects/idefix-cli/badge/?version=latest)](https://idefix-cli.readthedocs.io/en/latest/?badge=latest)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)](https://results.pre-commit.ci/badge/github/neutrinoceros/idefix_cli/main.svg)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 # `idefix_cli`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `idefix_cli-2.3.1/src/idefix_cli.egg-info/SOURCES.txt` & `idefix_cli-2.3.2/src/idefix_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/tests/test_app_structure.py` & `idefix_cli-2.3.2/tests/test_app_structure.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/tests/test_clean.py` & `idefix_cli-2.3.2/tests/test_clean.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/tests/test_clone.py` & `idefix_cli-2.3.2/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/tests/test_commons.py` & `idefix_cli-2.3.2/tests/test_commons.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/tests/test_conf.py` & `idefix_cli-2.3.2/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/tests/test_read.py` & `idefix_cli-2.3.2/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/tests/test_run.py` & `idefix_cli-2.3.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/tests/test_stamp.py` & `idefix_cli-2.3.2/tests/test_stamp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 from dataclasses import dataclass
 from getpass import getuser
 from socket import gethostname
-from typing import Tuple
 
 import pytest
 from pytest_check import check
 
 from idefix_cli.__main__ import main
 
 mock_data = {
@@ -29,15 +28,15 @@
 
 @dataclass
 class MockRepo:
     # I'm adding a meaningless "slot" attr here because pytest silently replaces my first attribute
     # with the test id. This is likely a bug on their side but for now I'll just work around it.
     slot: str
     head: MockHead = MockHead()
-    tags: Tuple[str] = (mock_data["latest ancestor version"],)
+    tags: tuple[str] = (mock_data["latest ancestor version"],)
 
 
 @pytest.mark.parametrize("flag", ["", "-d", "--json"])
 def test_stamp_no_idefix(flag, capsys, monkeypatch):
     monkeypatch.delenv("IDEFIX_DIR", raising=False)
 
     argv = ["stamp"]
```

### Comparing `idefix_cli-2.3.1/tests/test_ux.py` & `idefix_cli-2.3.2/tests/test_ux.py`

 * *Files identical despite different names*

### Comparing `idefix_cli-2.3.1/tests/test_write.py` & `idefix_cli-2.3.2/tests/test_write.py`

 * *Files identical despite different names*

