# Comparing `tmp/auto_click_auto-0.1.0a3.tar.gz` & `tmp/auto_click_auto-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_click_auto-0.1.0a3.tar", max compression
+gzip compressed data, was "auto_click_auto-0.1.0a4.tar", max compression
```

## Comparing `auto_click_auto-0.1.0a3.tar` & `auto_click_auto-0.1.0a4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1082 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/LICENSE
--rw-r--r--   0        0        0     5252 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/README.md
--rw-r--r--   0        0        0       99 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/__init__.py
--rw-r--r--   0        0        0      532 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/constants.py
--rw-r--r--   0        0        0     5271 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/core.py
--rw-r--r--   0        0        0      460 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/py.typed
--rw-r--r--   0        0        0     2823 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/auto_click_auto/utils.py
--rw-r--r--   0        0        0     1476 2023-07-17 20:18:43.651763 auto_click_auto-0.1.0a3/pyproject.toml
--rw-r--r--   0        0        0     6553 1970-01-01 00:00:00.000000 auto_click_auto-0.1.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-07-25 22:18:09.700163 auto_click_auto-0.1.0a4/LICENSE
+-rw-r--r--   0        0        0     5252 2023-07-25 22:18:09.700163 auto_click_auto-0.1.0a4/README.md
+-rw-r--r--   0        0        0       99 2023-07-25 22:18:09.700163 auto_click_auto-0.1.0a4/auto_click_auto/__init__.py
+-rw-r--r--   0        0        0      532 2023-07-25 22:18:09.700163 auto_click_auto-0.1.0a4/auto_click_auto/constants.py
+-rw-r--r--   0        0        0     5325 2023-07-25 22:18:09.704163 auto_click_auto-0.1.0a4/auto_click_auto/core.py
+-rw-r--r--   0        0        0      643 2023-07-25 22:18:09.704163 auto_click_auto-0.1.0a4/auto_click_auto/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-25 22:18:09.704163 auto_click_auto-0.1.0a4/auto_click_auto/py.typed
+-rw-r--r--   0        0        0     3037 2023-07-25 22:18:09.704163 auto_click_auto-0.1.0a4/auto_click_auto/utils.py
+-rw-r--r--   0        0        0     1476 2023-07-25 22:18:09.704163 auto_click_auto-0.1.0a4/pyproject.toml
+-rw-r--r--   0        0        0     6553 1970-01-01 00:00:00.000000 auto_click_auto-0.1.0a4/PKG-INFO
```

### Comparing `auto_click_auto-0.1.0a3/LICENSE` & `auto_click_auto-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a3/README.md` & `auto_click_auto-0.1.0a4/README.md`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a3/auto_click_auto/constants.py` & `auto_click_auto-0.1.0a4/auto_click_auto/constants.py`

 * *Files identical despite different names*

### Comparing `auto_click_auto-0.1.0a3/auto_click_auto/core.py` & `auto_click_auto-0.1.0a4/auto_click_auto/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import platform
 from typing import TYPE_CHECKING, Any, Callable, Optional, Set, TypeVar, Union
 
 from click import Command, Context, Parameter, option
 
 from .constants import ShellType
-from .exceptions import ShellTypeNotSupportedError
+from .exceptions import ShellEnvVarNotFoundError, ShellTypeNotSupportedError
 from .utils import add_shell_configuration, detect_shell
 
 if TYPE_CHECKING:
     import typing_extensions as te
 
 R = TypeVar("R")
 T = TypeVar("T")
@@ -56,15 +56,15 @@
 
     click_env_var = f"_{program_name.upper()}_COMPLETE"
 
     if shells is None:
         try:
             shells = {detect_shell()}
 
-        except ShellTypeNotSupportedError as err:
+        except (ShellTypeNotSupportedError, ShellEnvVarNotFoundError) as err:
             if verbose is True:
                 print(err)
 
             return None
 
     for shell in shells:
```

### Comparing `auto_click_auto-0.1.0a3/auto_click_auto/utils.py` & `auto_click_auto-0.1.0a4/auto_click_auto/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from typing import List, Optional
 
 from auto_click_auto.constants import ShellType
 from auto_click_auto.exceptions import (
     ShellConfigurationFileNotFoundError,
+    ShellEnvVarNotFoundError,
     ShellTypeNotSupportedError,
 )
 
 
 def check_strings_in_file(file_path: str, search_strings: List[str]) -> bool:
     """
     Check if the given search strings are in the specified file.
@@ -78,15 +79,22 @@
         print(
             "Tab autocomplete configuration already setup in "
             f"{shell_config_file}."
         )
 
 
 def detect_shell() -> ShellType:
-    shell_env_var = os.environ["SHELL"]
+    try:
+        shell_env_var = os.environ["SHELL"]
+
+    except KeyError:
+        raise ShellEnvVarNotFoundError(
+            "Could not infer the shell type from the 'SHELL' environment "
+            "variable."
+        )
 
     try:
         shell_value = shell_env_var.split("/")[-1]
         return ShellType(shell_value)
 
     except ValueError:
         raise ShellTypeNotSupportedError(
```

### Comparing `auto_click_auto-0.1.0a3/pyproject.toml` & `auto_click_auto-0.1.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "auto-click-auto"
-version = "0.1.0-alpha.3"
+version = "0.1.0-alpha.4"
 description = "Automatically enable tab autocompletion for shells in Click CLI applications."
 authors = ["Konstantinos Papadopoulos <konpap1996@yahoo.com>"]
 maintainers = ["Konstantinos Papadopoulos <konpap1996@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/KAUTH/auto-click-auto"
 repository = "https://github.com/KAUTH/auto-click-auto"
```

### Comparing `auto_click_auto-0.1.0a3/PKG-INFO` & `auto_click_auto-0.1.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-click-auto
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: Automatically enable tab autocompletion for shells in Click CLI applications.
 Home-page: https://github.com/KAUTH/auto-click-auto
 License: MIT
 Keywords: click,autocomplete,shell
 Author: Konstantinos Papadopoulos
 Author-email: konpap1996@yahoo.com
 Maintainer: Konstantinos Papadopoulos
```

