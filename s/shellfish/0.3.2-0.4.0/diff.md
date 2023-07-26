# Comparing `tmp/shellfish-0.3.2.tar.gz` & `tmp/shellfish-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellfish-0.3.2.tar", max compression
+gzip compressed data, was "shellfish-0.4.0.tar", max compression
```

## Comparing `shellfish-0.3.2.tar` & `shellfish-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     2275 2023-04-21 00:18:13.195085 shellfish-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1003 2022-09-19 18:35:16.987296 shellfish-0.3.2/README.md
--rw-r--r--   0        0        0      295 2023-04-21 00:18:13.195085 shellfish-0.3.2/shellfish/__about__.py
--rw-r--r--   0        0        0     1148 2023-04-21 00:04:53.526032 shellfish-0.3.2/shellfish/__init__.py
--rw-r--r--   0        0        0      483 2023-04-21 00:04:53.526032 shellfish-0.3.2/shellfish/__main__.py
--rw-r--r--   0        0        0      358 2023-04-21 00:04:53.526032 shellfish-0.3.2/shellfish/_meta.py
--rw-r--r--   0        0        0      866 2023-04-19 19:17:33.733686 shellfish-0.3.2/shellfish/_types.py
--rw-r--r--   0        0        0     3278 2023-04-19 19:17:33.734686 shellfish-0.3.2/shellfish/aios/__init__.py
--rw-r--r--   0        0        0      640 2023-04-19 19:16:52.950595 shellfish-0.3.2/shellfish/aios/_path.py
--rw-r--r--   0        0        0     7251 2023-04-19 19:17:33.734686 shellfish-0.3.2/shellfish/batman.py
--rw-r--r--   0        0        0      295 2022-02-17 22:17:07.429546 shellfish-0.3.2/shellfish/const.py
--rw-r--r--   0        0        0       49 2022-02-04 21:32:32.211842 shellfish-0.3.2/shellfish/dev/__init__.py
--rw-r--r--   0        0        0     1439 2023-04-19 19:17:33.735685 shellfish-0.3.2/shellfish/dev/do.py
--rw-r--r--   0        0        0     3456 2023-04-19 19:17:33.735685 shellfish-0.3.2/shellfish/dev/popen_gen.py
--rw-r--r--   0        0        0     7941 2023-04-19 19:17:33.736685 shellfish-0.3.2/shellfish/dev/run_async.py
--rw-r--r--   0        0        0     4265 2023-04-11 22:29:27.086800 shellfish-0.3.2/shellfish/dotenv.py
--rw-r--r--   0        0        0      664 2023-03-31 17:46:06.868732 shellfish-0.3.2/shellfish/echo.py
--rw-r--r--   0        0        0     7924 2023-04-19 19:17:33.736685 shellfish-0.3.2/shellfish/exe.py
--rw-r--r--   0        0        0    54196 2023-04-21 00:18:13.196068 shellfish-0.3.2/shellfish/fs/__init__.py
--rw-r--r--   0        0        0    15169 2023-04-19 19:17:33.738722 shellfish-0.3.2/shellfish/fs/_async.py
--rw-r--r--   0        0        0     1534 2023-02-24 22:45:12.450622 shellfish-0.3.2/shellfish/fs/promises.py
--rw-r--r--   0        0        0     1917 2023-04-19 19:17:33.738722 shellfish-0.3.2/shellfish/libhash.py
--rw-r--r--   0        0        0       50 2023-02-09 22:42:06.315587 shellfish-0.3.2/shellfish/libsh/__init__.py
--rw-r--r--   0        0        0     3655 2023-04-19 19:17:33.739722 shellfish-0.3.2/shellfish/libsh/_dirtree.py
--rw-r--r--   0        0        0     1872 2023-04-19 19:17:33.739722 shellfish-0.3.2/shellfish/libsh/args.py
--rw-r--r--   0        0        0    10653 2023-04-19 19:17:33.739722 shellfish-0.3.2/shellfish/osfs.py
--rw-r--r--   0        0        0     7266 2023-04-19 19:17:33.740721 shellfish-0.3.2/shellfish/process.py
--rw-r--r--   0        0        0      308 2023-03-24 22:14:11.926875 shellfish-0.3.2/shellfish/psu.py
--rw-r--r--   0        0        0        0 2022-02-01 22:06:04.844951 shellfish-0.3.2/shellfish/py.typed
--rw-r--r--   0        0        0    63208 2023-04-21 00:04:53.526032 shellfish-0.3.2/shellfish/sh.py
--rw-r--r--   0        0        0     8275 2023-04-19 19:17:33.741721 shellfish-0.3.2/shellfish/sp.py
--rw-r--r--   0        0        0      228 2023-04-19 19:17:33.741721 shellfish-0.3.2/shellfish/stdio.py
--rw-r--r--   0        0        0     2617 2023-04-11 22:29:27.086800 shellfish-0.3.2/shellfish/testing.py
--rw-r--r--   0        0        0       27 2023-04-19 19:17:33.742721 shellfish-0.3.2/shellfish/tests/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-19 19:17:33.742721 shellfish-0.3.2/shellfish/tests/test_fs.py
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 shellfish-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2300 2023-07-26 14:37:12.145796 shellfish-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1029 2023-06-15 16:25:20.011325 shellfish-0.4.0/README.md
+-rw-r--r--   0        0        0      295 2023-07-20 15:55:15.334103 shellfish-0.4.0/shellfish/__about__.py
+-rw-r--r--   0        0        0     1200 2023-04-21 22:10:02.240905 shellfish-0.4.0/shellfish/__init__.py
+-rw-r--r--   0        0        0      483 2023-04-21 00:04:53.526032 shellfish-0.4.0/shellfish/__main__.py
+-rw-r--r--   0        0        0      358 2023-04-21 00:04:53.526032 shellfish-0.4.0/shellfish/_meta.py
+-rw-r--r--   0        0        0      866 2023-04-19 19:17:33.733686 shellfish-0.4.0/shellfish/_types.py
+-rw-r--r--   0        0        0     3278 2023-04-19 19:17:33.734686 shellfish-0.4.0/shellfish/aios/__init__.py
+-rw-r--r--   0        0        0      640 2023-04-19 19:16:52.950595 shellfish-0.4.0/shellfish/aios/_path.py
+-rw-r--r--   0        0        0      538 2023-04-21 22:10:02.240905 shellfish-0.4.0/shellfish/aioshutil.py
+-rw-r--r--   0        0        0     7251 2023-04-19 19:17:33.734686 shellfish-0.4.0/shellfish/batman.py
+-rw-r--r--   0        0        0      295 2022-02-17 22:17:07.429546 shellfish-0.4.0/shellfish/const.py
+-rw-r--r--   0        0        0       49 2022-02-04 21:32:32.211842 shellfish-0.4.0/shellfish/dev/__init__.py
+-rw-r--r--   0        0        0     1439 2023-04-19 19:17:33.735685 shellfish-0.4.0/shellfish/dev/do.py
+-rw-r--r--   0        0        0     3456 2023-04-19 19:17:33.735685 shellfish-0.4.0/shellfish/dev/popen_gen.py
+-rw-r--r--   0        0        0     8019 2023-06-15 16:25:20.011325 shellfish-0.4.0/shellfish/dev/run_async.py
+-rw-r--r--   0        0        0     4265 2023-04-11 22:29:27.086800 shellfish-0.4.0/shellfish/dotenv.py
+-rw-r--r--   0        0        0      664 2023-03-31 17:46:06.868732 shellfish-0.4.0/shellfish/echo.py
+-rw-r--r--   0        0        0     8039 2023-06-15 16:25:20.011325 shellfish-0.4.0/shellfish/exe.py
+-rw-r--r--   0        0        0    54204 2023-06-15 16:25:20.027510 shellfish-0.4.0/shellfish/fs/__init__.py
+-rw-r--r--   0        0        0    15169 2023-04-19 19:17:33.738722 shellfish-0.4.0/shellfish/fs/_async.py
+-rw-r--r--   0        0        0     1534 2023-02-24 22:45:12.450622 shellfish-0.4.0/shellfish/fs/promises.py
+-rw-r--r--   0        0        0     1927 2023-05-03 19:53:18.637683 shellfish-0.4.0/shellfish/libhash.py
+-rw-r--r--   0        0        0       50 2023-02-09 22:42:06.315587 shellfish-0.4.0/shellfish/libsh/__init__.py
+-rw-r--r--   0        0        0     3655 2023-04-19 19:17:33.739722 shellfish-0.4.0/shellfish/libsh/_dirtree.py
+-rw-r--r--   0        0        0     1872 2023-04-19 19:17:33.739722 shellfish-0.4.0/shellfish/libsh/args.py
+-rw-r--r--   0        0        0    10653 2023-04-19 19:17:33.739722 shellfish-0.4.0/shellfish/osfs.py
+-rw-r--r--   0        0        0     7292 2023-05-23 19:01:12.699434 shellfish-0.4.0/shellfish/process.py
+-rw-r--r--   0        0        0      308 2023-03-24 22:14:11.926875 shellfish-0.4.0/shellfish/psu.py
+-rw-r--r--   0        0        0        0 2022-02-01 22:06:04.844951 shellfish-0.4.0/shellfish/py.typed
+-rw-r--r--   0        0        0    63493 2023-07-20 15:55:15.334103 shellfish-0.4.0/shellfish/sh.py
+-rw-r--r--   0        0        0     8275 2023-04-19 19:17:33.741721 shellfish-0.4.0/shellfish/sp.py
+-rw-r--r--   0        0        0      228 2023-04-19 19:17:33.741721 shellfish-0.4.0/shellfish/stdio.py
+-rw-r--r--   0        0        0     2617 2023-04-11 22:29:27.086800 shellfish-0.4.0/shellfish/testing.py
+-rw-r--r--   0        0        0       27 2023-04-19 19:17:33.742721 shellfish-0.4.0/shellfish/tests/__init__.py
+-rw-r--r--   0        0        0     3368 2023-04-21 22:10:02.240905 shellfish-0.4.0/shellfish/tests/test_fs.py
+-rw-r--r--   0        0        0     2222 1970-01-01 00:00:00.000000 shellfish-0.4.0/PKG-INFO
```

### Comparing `shellfish-0.3.2/pyproject.toml` & `shellfish-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shellfish"
-version = "0.3.2"
+version = "0.4.0"
 description = "shellfish ~ shell & file-system utils"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/shellfish"
 readme = 'README.md'
 packages = [
@@ -27,26 +27,26 @@
   "fs",
   "filesystem",
   "typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pydantic = "^1.9.0"
+pydantic = ">=2.0.3"
 aiopen = "^0.5.0"
 asyncify = ">=0.9.1"
 funkify = ">=0.4.0"
-jsonbourne = ">=0.24.0"
+jsonbourne = ">=0.27.0"
 listless = ">=0.1.0"
 xtyping = ">=0.6.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.3.1"
-pytest-asyncio = "^0.21.0"
-pytest-cov = "^4.0.0"
+pytest = "^7.4.0"
+pytest-asyncio = "^0.21.1"
+pytest-cov = "^4.1.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
@@ -92,7 +92,8 @@
   '\(Protocol\):$',
   'if 0:',
   'if False:',
 ]
 
 [tool.ruff]
 extend = "../../pyproject.toml"
+target-version = "py37"
```

### Comparing `shellfish-0.3.2/README.md` & `shellfish-0.4.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,14 @@
 **Install:** `pip install shellfish` OR `poetry add shellfish`
 
 **What:** shellfish = shell & file-system utils; async & sync
 
 **Features:**
 
 - Pydantic models
-- Asyncio
+- Async(io) shell/file-system utils
 - Type annotated
 
 **TODO:**
 
-- [ ] Add support for acceptable return codes
+- [x] Add support for acceptable return codes
 - [ ] Look into breaking down shellfish.sh into smaller modules
```

#### html2text {}

```diff
@@ -2,10 +2,10 @@
 shellfish.svg)](https://img.shields.io/pypi/wheel/shellfish.svg) [![Version]
 (https://img.shields.io/pypi/v/shellfish.svg)](https://img.shields.io/pypi/v/
 shellfish.svg) [![py_versions](https://img.shields.io/pypi/pyversions/
 shellfish.svg)](https://img.shields.io/pypi/pyversions/shellfish.svg) [![Code
 style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
 (https://github.com/psf/black) **Install:** `pip install shellfish` OR `poetry
 add shellfish` **What:** shellfish = shell & file-system utils; async & sync
-**Features:** - Pydantic models - Asyncio - Type annotated **TODO:** - [ ] Add
-support for acceptable return codes - [ ] Look into breaking down shellfish.sh
-into smaller modules
+**Features:** - Pydantic models - Async(io) shell/file-system utils - Type
+annotated **TODO:** - [x] Add support for acceptable return codes - [ ] Look
+into breaking down shellfish.sh into smaller modules
```

### Comparing `shellfish-0.3.2/shellfish/__init__.py` & `shellfish-0.4.0/shellfish/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 """shellfish ~ shell and file-system utils"""
 from __future__ import annotations
 
+from asyncify import aiorun as aiorun
 from funkify import funkify as _funkify
 from shellfish import dotenv as dotenv, fs as fs, process as process, sh as sh
 from shellfish.__about__ import __version__ as __version__
 from shellfish._types import (
     FsPath as FsPath,
     PathLikeBytes as PathLikeBytes,
     PathLikeStr as PathLikeStr,
@@ -38,14 +39,15 @@
     "PathLikeStrBytes",
     "PopenArg",
     "PopenArgs",
     "PopenArgv",
     "PopenEnv",
     "SymlinkType",
     "__version__",
+    "aiorun",
     "do",
     "do_async",
     "dotenv",
     "env",
     "fs",
     "process",
     "ps",
```

### Comparing `shellfish-0.3.2/shellfish/_types.py` & `shellfish-0.4.0/shellfish/_types.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/aios/__init__.py` & `shellfish-0.4.0/shellfish/aios/__init__.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/aios/_path.py` & `shellfish-0.4.0/shellfish/aios/_path.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/batman.py` & `shellfish-0.4.0/shellfish/batman.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/dev/do.py` & `shellfish-0.4.0/shellfish/dev/do.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/dev/popen_gen.py` & `shellfish-0.4.0/shellfish/dev/popen_gen.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/dev/run_async.py` & `shellfish-0.4.0/shellfish/dev/run_async.py`

 * *Files 12% similar despite different names*

```diff
@@ -89,14 +89,16 @@
             env=env,
             limit=2**23,
             cwd=_cwd,
         )
 
     _out_buf = BytesIO()
     _err_buf = BytesIO()
+    _stdout = b""
+    _stderr = b""
 
     def _tee_bytes(line: bytes, sink: BytesIO, pipe: IO[bytes]) -> None:
         sink.write(line)
         pipe.write(line)
 
     def _tee_string(line: bytes, sink: BytesIO, pipe: IO[str]) -> None:
         sink.write(line)
@@ -131,34 +133,34 @@
                 await asyncio.wait_for(
                     asyncio.gather(
                         *_bg,
                     ),
                     timeout=timeout,
                 )
                 tf = time()
-            except ValueError:
+            except ValueError as ve:
                 tf = time()
                 _proc.terminate()
                 raise TimeoutExpired(
                     cmd=_args,
                     timeout=timeout,
                     output=_out_buf.getvalue(),
                     stderr=_err_buf.getvalue(),
-                )
-            except TimeoutError:
+                ) from ve
+            except TimeoutError as te:
                 tf = time()
                 for task in _bg:
                     task.cancel()
                 _proc.terminate()
                 raise TimeoutExpired(
                     cmd=_args,
                     timeout=timeout,
                     output=_out_buf.getvalue(),
                     stderr=_err_buf.getvalue(),
-                )
+                ) from te
         else:
             await asyncio.gather(
                 *_bg,
             )
             tf = time()
     else:
         if timeout:
@@ -173,22 +175,22 @@
                 else:
                     (_stdout, _stderr) = await asyncio.wait_for(
                         _proc.communicate(),  # wait for subprocess to finish
                         timeout=timeout,
                     )
 
                 tf = time()
-            except TimeoutError:
+            except TimeoutError as te:
                 _proc.terminate()
                 raise TimeoutExpired(
                     cmd=_args,
                     timeout=timeout,
                     output=_out_buf.getvalue(),
                     stderr=_err_buf.getvalue(),
-                )
+                ) from te
         else:
             (_stdout, _stderr) = await _proc.communicate(input=_input_bytes)
             tf = time()
     if tee:
         _stdout = _out_buf.getvalue()
         _stderr = _err_buf.getvalue()
     if universal_newlines:
```

### Comparing `shellfish-0.3.2/shellfish/dotenv.py` & `shellfish-0.4.0/shellfish/dotenv.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/echo.py` & `shellfish-0.4.0/shellfish/echo.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/exe.py` & `shellfish-0.4.0/shellfish/exe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # -*- coding: utf-8 -*-
 """Exes/commands"""
 from __future__ import annotations
 
+from dataclasses import dataclass, field
 from shlex import split as _shplit
 from typing import Any, Dict, List, Optional, Set, Tuple, Type, TypeVar, Union
 
-from jsonbourne.pydantic import JsonBaseModel
 from shellfish import sh
 from shellfish._types import PopenArgs, PopenArgv
 from shellfish.sh import Done, flatten_args
 from xtyping import STDIN, FsPath
 
 __all__ = (
     "Exe",
     "ExeAsync",
 )
 
 TExe = TypeVar("TExe", bound="ExeABC")
 
 
-class ExeConfig(JsonBaseModel):
+@dataclass
+class ExeConfig:
     cmd: str
     subcmd: Optional[Tuple[str, ...]] = None
     abspath: Optional[str] = None
     env: Optional[Dict[str, str]] = None
     cwd: Optional[str] = None
     shell: bool = False
     verbose: bool = False
     timeout: Optional[int] = None
-    ok_code: Union[int, Set[int]] = {0}
+    ok_code: Union[int, Set[int]] = field(default_factory=lambda: {0})
     check: bool = False
 
 
 class ExeABC:
     cmd: str
     subcmd: Optional[Tuple[str, ...]] = None
 
     abspath: Optional[str] = None
     env: Optional[Dict[str, str]] = None
     cwd: Optional[FsPath] = None
     shell: bool = False
     verbose: bool = False
     timeout: Optional[int] = None
-    ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = (0,)
+    ok_code: Union[int, Set[int]] = 0  # List[int], Tuple[int, ...], Set[int]] = (0,)
     check: bool = False
 
     def __init__(
         self,
         cmd: str,
         subcmd: Optional[Union[Tuple[str, ...], List[str], str]] = None,
         abspath: Optional[str] = None,
@@ -63,15 +64,21 @@
             self.subcmd = (subcmd,) if isinstance(subcmd, str) else tuple(subcmd)
         self.abspath = abspath
         self.env = env
         self.cwd = cwd
         self.shell = shell
         self.verbose = verbose
         self.timeout = timeout
-        self.ok_code = (ok_code,) if isinstance(ok_code, int) else tuple(ok_code)
+        self.ok_code = (
+            {
+                ok_code,
+            }
+            if isinstance(ok_code, int)
+            else set(ok_code)
+        )
         self.check = check
         self.__post_init__()
 
     def __post_init__(self) -> None:
         """Post-initialization"""
         ...
```

### Comparing `shellfish-0.3.2/shellfish/fs/__init__.py` & `shellfish-0.4.0/shellfish/fs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1447,15 +1447,15 @@
 
     """
     return iglob(pattern, recursive=recursive or r)
 
 
 def rename(src: FsPath, dest: FsPath, *, dryrun: bool = False) -> Tuple[FsPath, FsPath]:
     if not dryrun:
-        _move(src, dest)
+        _move(fspath(src), dest)
     return (src, dest)
 
 
 def move(src: FsPath, dest: FsPath) -> None:
     """Move file(s) like on the command line
 
     Args:
```

### Comparing `shellfish-0.3.2/shellfish/fs/_async.py` & `shellfish-0.4.0/shellfish/fs/_async.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/fs/promises.py` & `shellfish-0.4.0/shellfish/fs/promises.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/libhash.py` & `shellfish-0.4.0/shellfish/libhash.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     """
     try:
         return _HASHERS[string]()
     except KeyError:
         raise ValueError(
             f"Invalid hash algorithm: {string} (valid: {list(_HASHERS.keys())})"
-        )
+        ) from None
 
 
 def hasher(obj: HashLike) -> "_Hash":
     """Return a hash object from a string or a hash object
 
     Args:
         obj (Union[str, hash]): String or hash object
```

### Comparing `shellfish-0.3.2/shellfish/libsh/_dirtree.py` & `shellfish-0.4.0/shellfish/libsh/_dirtree.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/libsh/args.py` & `shellfish-0.4.0/shellfish/libsh/args.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/osfs.py` & `shellfish-0.4.0/shellfish/osfs.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/process.py` & `shellfish-0.4.0/shellfish/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 """Current running process info"""
 from __future__ import annotations
 
-import os
 import platform
 import sys
 
 from contextlib import contextmanager
-from os import environ
+from os import environ, name as os_name, pathsep
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     ItemsView,
     Iterator,
@@ -20,17 +19,17 @@
     Optional,
     Type,
     Union,
     ValuesView,
     cast,
 )
 
-IS_WIN = os.name == "nt"
+IS_WIN = os_name == "nt"
 PYTHON_IMPLEMENTATION = platform.python_implementation()
-SYS_PATH_SEP: str = os.pathsep
+SYS_PATH_SEP: str = pathsep
 
 __all__ = (
     "ENV",
     "Env",
     "PYTHON_IMPLEMENTATION",
     "SYS_PATH_SEP",
     "env",
@@ -43,15 +42,15 @@
     "is_wsl",
     "ismac",
     "iswin",
     "iswsl",
     "opsys",
     "sys_path_sep",
 )
-_OS_ENVIRON_ATTRS = set(dir(os.environ))
+_OS_ENVIRON_ATTRS = set(dir(environ))
 
 
 @contextmanager
 def tmpenv(**kwargs: str) -> Generator[Type[Env], Any, None]:
     """Context manager for Env"""
     old_env = dict(environ)
     if kwargs:
@@ -271,22 +270,23 @@
     return platform.node()
 
 
 def sys_path_sep() -> str:
     """Return the system path separator string (; on windows -- : otherwise)
 
     Examples:
+        >>> import os
         >>> sep = sys_path_sep()
         >>> isinstance(sep, str)
         True
         >>> os.pathsep == sep
         True
 
     """
-    return os.pathsep
+    return pathsep
 
 
 def syspath_paths(syspath: Optional[str] = None) -> List[str]:
     """Return the current sys.path as a list
 
     Examples:
         >>> sys_paths = syspath_paths()
@@ -298,8 +298,8 @@
         True
         >>> sys_paths_w_args == ['path1', 'path2', 'path3']
         True
 
     """
     if syspath is None:
         return list(filter(None, sys.path))
-    return list(filter(None, syspath.split(os.pathsep)))
+    return list(filter(None, syspath.split(pathsep)))
```

### Comparing `shellfish-0.3.2/shellfish/sh.py` & `shellfish-0.4.0/shellfish/sh.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,19 @@
 
 from asyncify import asyncify
 from jsonbourne import JSON
 from jsonbourne.pydantic import JsonBaseModel
 from listless import flatten_strings as _flatten_strings
 from shellfish import fs, sp
 from shellfish.__about__ import __version__
-from shellfish._types import FsPath as FsPath, PopenArgs as PopenArgs
+from shellfish._types import (
+    FsPath as FsPath,
+    PopenArg as PopenArg,
+    PopenArgs as PopenArgs,
+)
 from shellfish.dev import run_async as __run_async
 from shellfish.echo import echo as echo
 from shellfish.fs import (
     SymlinkType as SymlinkType,
     chmod as chmod,
     copy_file as copy_file,
     cp as cp,
@@ -421,15 +425,19 @@
 
 
 class DoneError(SubprocessError):
     """Raised when run() is called with check=True and the process
     returns a non-zero exit status.
 
     Attributes:
-      cmd, returncode, stdout, stderr, output
+        cmd (str): command that was run
+        returncode (int): exit status of the process
+        stdout (str): standard output (stdout) of the process
+        stderr (str): standard error (stderr) of the process
+
     """
 
     done: Done
     returncode: int
     stdout: str
     stderr: str
     cmd: List[str]
@@ -451,14 +459,22 @@
         return (
             f"Command '{self.cmd}' returned non-zero exit status {self.returncode:d}."
         )
 
     def __str__(self) -> str:
         return f"{self.error_msg()}\n{self.done}"
 
+    @property
+    def output(self) -> str:
+        return self.stdout
+
+    @output.setter
+    def output(self, value: str) -> None:
+        self.stdout = value
+
 
 class DoneDict(TypedDict):
     args: List[str]
     returncode: int
     stdout: str
     stderr: str
     ti: float
@@ -806,32 +822,28 @@
         _args = args[0]
         if isinstance(_args, str):
             return shplit(_args)
         return flatten_args(_args)
     return flatten_args(args)
 
 
-def popen_has_pipe_character(args: Union[List[str], Tuple[str, ...]]) -> bool:
+def popen_has_pipe_character(args: Union[List[PopenArg], Tuple[PopenArg, ...]]) -> bool:
     return any(arg == "|" for arg in args)
 
 
 def validate_popen_args_windows(
     args: PopenArgs, env: Optional[Dict[str, str]] = None
 ) -> PopenArgs:
     args = validate_popen_args(args)
     _path = None
     if env and "PATH" in env:
         _path = env["PATH"]
     fspath = which_lru(args[0], path=_path)
-    if fspath:
-        fspath_obj = Path(fspath)
-        if fspath.lower().endswith(".cmd"):
-            args[0] = str(fspath_obj.absolute())
-        elif fspath.lower().endswith(".bat"):
-            args[0] = str(fspath_obj.absolute())
+    if fspath and fspath.lower() in {".cmd", ".bat"}:
+        args[0] = str(Path(fspath).absolute())
     return args
 
 
 def _do_tee(
     args: PopenArgs,
     input: Optional[STDIN],
     cwd: Optional[FsPath],
@@ -971,14 +983,15 @@
     *popenargs: PopenArgs,
     args: Optional[PopenArgs] = None,
     env: Optional[Dict[str, str]] = None,
     extenv: bool = True,
     cwd: Optional[FsPath] = None,
     shell: bool = False,
     check: bool = False,
+    tee: bool = False,
     verbose: bool = False,
     input: STDIN = None,
     timeout: Optional[int] = None,
     ok_code: Union[int, List[int], Tuple[int, ...], Set[int]] = 0,
     dryrun: bool = False,
 ) -> Done:
     """Run a subprocess synchronously
@@ -1020,14 +1033,15 @@
         shell=shell,
         check=check,
         verbose=verbose,
         input=_input,
         timeout=timeout,
         ok_code=ok_code,
         dryrun=dryrun,
+        tee=tee,
     )
 
 
 def shell(
     *popenargs: PopenArgs,
     args: Optional[PopenArgs] = None,
     env: Optional[Dict[str, str]] = None,
```

### Comparing `shellfish-0.3.2/shellfish/sp.py` & `shellfish-0.4.0/shellfish/sp.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/testing.py` & `shellfish-0.4.0/shellfish/testing.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.2/shellfish/tests/test_fs.py` & `shellfish-0.4.0/shellfish/tests/test_fs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Testing shelfish.fs"""
+from collections import Counter
 from os import path
 from pathlib import Path
+from typing import Callable, Iterable
 
 import pytest
 
 from shellfish import sh
 
 
 def test_is_file_dir_link(tmp_path: Path) -> None:
@@ -87,7 +89,22 @@
     sh.mkdir("a-dir")
     for i in range(3):
         sh.touch(
             path.join("a-dir", f"file{i}.txt"),
         )
     items = await sh.listdir_async("a-dir")
     assert sorted(items) == ["file0.txt", "file1.txt", "file2.txt"]
+
+
+@pytest.mark.parametrize(
+    "gen",
+    [
+        pytest.param(sh.dirs_gen, id="dirs_gen"),
+        pytest.param(sh.files_gen, id="files_gen"),
+        pytest.param(sh.walk_gen, id="walk_gen"),
+    ],
+)
+def test_fs_generator_duplicates(gen: Callable[..., Iterable[str]]) -> None:
+    pkg_root = Path(__file__).parent.parent
+    gen_count = Counter(gen(pkg_root))
+    duplicates = {k: v for k, v in gen_count.items() if v > 1}
+    assert not duplicates, f"duplicates: {duplicates}"
```

### Comparing `shellfish-0.3.2/PKG-INFO` & `shellfish-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellfish
-Version: 0.3.2
+Version: 0.4.0
 Summary: shellfish ~ shell & file-system utils
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/shellfish
 License: MIT
 Keywords: dgpy,shell,fs,filesystem,typed
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0
@@ -14,25 +14,21 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Requires-Dist: aiopen (>=0.5.0,<0.6.0)
 Requires-Dist: asyncify (>=0.9.1)
 Requires-Dist: funkify (>=0.4.0)
-Requires-Dist: jsonbourne (>=0.24.0)
+Requires-Dist: jsonbourne (>=0.27.0)
 Requires-Dist: listless (>=0.1.0)
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: pydantic (>=2.0.3)
 Requires-Dist: xtyping (>=0.6.0)
 Project-URL: Repository, https://github.com/dynamic-graphics-inc/dgpy-libs
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/dynamic-graphics-inc/dgpy-libs">
 <img align="right" src="https://github.com/dynamic-graphics-inc/dgpy-libs/blob/main/docs/images/dgpy_banner.svg?raw=true" alt="drawing" height="120" width="300"/>
 </a>
@@ -47,15 +43,15 @@
 **Install:** `pip install shellfish` OR `poetry add shellfish`
 
 **What:** shellfish = shell & file-system utils; async & sync
 
 **Features:**
 
 - Pydantic models
-- Asyncio
+- Async(io) shell/file-system utils
 - Type annotated
 
 **TODO:**
 
-- [ ] Add support for acceptable return codes
+- [x] Add support for acceptable return codes
 - [ ] Look into breaking down shellfish.sh into smaller modules
```

#### html2text {}

```diff
@@ -1,29 +1,27 @@
-Metadata-Version: 2.1 Name: shellfish Version: 0.3.2 Summary: shellfish ~ shell
+Metadata-Version: 2.1 Name: shellfish Version: 0.4.0 Summary: shellfish ~ shell
 & file-system utils Home-page: https://github.com/dynamic-graphics-inc/dgpy-
 libs/tree/main/libs/shellfish License: MIT Keywords:
 dgpy,shell,fs,filesystem,typed Author: jesse Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Typing :: Typed Requires-
-Dist: aiopen (>=0.5.0,<0.6.0) Requires-Dist: asyncify (>=0.9.1) Requires-Dist:
-funkify (>=0.4.0) Requires-Dist: jsonbourne (>=0.24.0) Requires-Dist: listless
-(>=0.1.0) Requires-Dist: pydantic (>=1.9.0,<2.0.0) Requires-Dist: xtyping
-(>=0.6.0) Project-URL: Repository, https://github.com/dynamic-graphics-inc/
-dgpy-libs Description-Content-Type: text/markdown [drawing] # shellfish [!
-[Wheel](https://img.shields.io/pypi/wheel/shellfish.svg)](https://
+Typing :: Typed Requires-Dist: aiopen (>=0.5.0,<0.6.0) Requires-Dist: asyncify
+(>=0.9.1) Requires-Dist: funkify (>=0.4.0) Requires-Dist: jsonbourne (>=0.27.0)
+Requires-Dist: listless (>=0.1.0) Requires-Dist: pydantic (>=2.0.3) Requires-
+Dist: xtyping (>=0.6.0) Project-URL: Repository, https://github.com/dynamic-
+graphics-inc/dgpy-libs Description-Content-Type: text/markdown [drawing] #
+shellfish [![Wheel](https://img.shields.io/pypi/wheel/shellfish.svg)](https://
 img.shields.io/pypi/wheel/shellfish.svg) [![Version](https://img.shields.io/
 pypi/v/shellfish.svg)](https://img.shields.io/pypi/v/shellfish.svg) [!
 [py_versions](https://img.shields.io/pypi/pyversions/shellfish.svg)](https://
 img.shields.io/pypi/pyversions/shellfish.svg) [![Code style: black](https://
 img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
 black) **Install:** `pip install shellfish` OR `poetry add shellfish` **What:**
 shellfish = shell & file-system utils; async & sync **Features:** - Pydantic
-models - Asyncio - Type annotated **TODO:** - [ ] Add support for acceptable
-return codes - [ ] Look into breaking down shellfish.sh into smaller modules
+models - Async(io) shell/file-system utils - Type annotated **TODO:** - [x] Add
+support for acceptable return codes - [ ] Look into breaking down shellfish.sh
+into smaller modules
```

