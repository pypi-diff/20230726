# Comparing `tmp/clickloader-0.1.2.tar.gz` & `tmp/clickloader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickloader-0.1.2.tar", max compression
+gzip compressed data, was "clickloader-0.1.3.tar", max compression
```

## Comparing `clickloader-0.1.2.tar` & `clickloader-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-07-25 09:48:19.501883 clickloader-0.1.2/LICENSE
--rw-r--r--   0        0        0     2066 2023-07-25 09:48:19.501883 clickloader-0.1.2/README.md
--rw-r--r--   0        0        0     1077 2023-07-25 09:48:19.501883 clickloader-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2226 2023-07-25 09:48:19.501883 clickloader-0.1.2/src/ccl/__init__.py
--rw-r--r--   0        0        0     2733 2023-07-25 09:48:19.501883 clickloader-0.1.2/src/ccl/finder.py
--rw-r--r--   0        0        0        0 2023-07-25 09:48:19.501883 clickloader-0.1.2/src/ccl/py.typed
--rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 clickloader-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-26 00:32:17.505986 clickloader-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2066 2023-07-26 00:32:17.505986 clickloader-0.1.3/README.md
+-rw-r--r--   0        0        0     1077 2023-07-26 00:32:17.505986 clickloader-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2242 2023-07-26 00:32:17.505986 clickloader-0.1.3/src/ccl/__init__.py
+-rw-r--r--   0        0        0     2733 2023-07-26 00:32:17.505986 clickloader-0.1.3/src/ccl/finder.py
+-rw-r--r--   0        0        0        0 2023-07-26 00:32:17.505986 clickloader-0.1.3/src/ccl/py.typed
+-rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 clickloader-0.1.3/PKG-INFO
```

### Comparing `clickloader-0.1.2/LICENSE` & `clickloader-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clickloader-0.1.2/README.md` & `clickloader-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `clickloader-0.1.2/pyproject.toml` & `clickloader-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clickloader"
-version = "0.1.2"
+version = "0.1.3"
 description = "Click Command Loader, permit to load Click command from a given folder."
 authors = ["Julien Mauroy <pro.julien.mauroy@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ccl", from = "src"}]
 repository = "https://github.com/madebylydia/CCL"
 
 [tool.poetry.dependencies]
```

### Comparing `clickloader-0.1.2/src/ccl/__init__.py` & `clickloader-0.1.3/src/ccl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import pathlib
-from importlib.metadata import distribution as __dist
 import typing
+from importlib.metadata import distribution as __dist
 
 import click
 
 from ccl import finder
 
 __version__ = __dist("clickloader").version
 __author__ = __dist("clickloader").metadata["Author"]
@@ -13,29 +13,31 @@
 _log = logging.getLogger("ccl")
 
 
 def register_commands(
     group: click.Group,
     source: typing.Union[str, pathlib.Path],
 ) -> None:
-    path = pathlib.Path(source)
+    path = pathlib.Path(source).resolve()
     _log.debug(f"Started registering commands in {path.resolve()}")
 
     commands = fetch_commands_for_group(path)
 
     for command in commands:
         _log.info(
             f"Adding commands from group {command.name}"
             if isinstance(command, click.Group)
             else f"Adding command {command.name}"
         )
         group.add_command(command)
 
 
-def fetch_commands_for_group(source: pathlib.Path) -> typing.List[typing.Union[click.Command, click.Group]]:
+def fetch_commands_for_group(
+    source: pathlib.Path,
+) -> typing.List[typing.Union[click.Command, click.Group]]:
     """Return a list of click's commands or groups.
 
     Parameters
     ----------
     source : pathlib.Path
         Path to the source that should be read.
     """
@@ -49,15 +51,14 @@
             _log.debug(f"Found {file.name}")
             function_name = finder.find_cmd_func_name(file)
             command = finder.fetch_cmd_func(file, function_name, "command")
 
             entities.append(command)
 
         if file.is_dir():
-
             _log.debug(f"Found directory {file.resolve()}, looping inside...")
 
             if (file / "__init__.py").exists():
                 _log.debug("Found __init__.py, trying to extract group")
                 func_name = finder.find_cmd_func_name(file / "__init__.py")
                 group = finder.fetch_cmd_func(file / "__init__.py", func_name, "group")
                 group.name = file.name
```

### Comparing `clickloader-0.1.2/src/ccl/finder.py` & `clickloader-0.1.3/src/ccl/finder.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import importlib.util
 import logging
 import pathlib
+import typing
 from shutil import ExecError
 from typing import Literal, overload
-import typing
 
 import click
 
 _log = logging.getLogger("ccl")
 
 
 def find_cmd_func_name(path: pathlib.Path) -> str:
```

### Comparing `clickloader-0.1.2/PKG-INFO` & `clickloader-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickloader
-Version: 0.1.2
+Version: 0.1.3
 Summary: Click Command Loader, permit to load Click command from a given folder.
 Home-page: https://github.com/madebylydia/CCL
 Author: Julien Mauroy
 Author-email: pro.julien.mauroy@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

