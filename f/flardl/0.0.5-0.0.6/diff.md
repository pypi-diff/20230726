# Comparing `tmp/flardl-0.0.5.tar.gz` & `tmp/flardl-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flardl-0.0.5.tar", max compression
+gzip compressed data, was "flardl-0.0.6.tar", max compression
```

## Comparing `flardl-0.0.5.tar` & `flardl-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1958 2023-07-24 22:21:35.793575 flardl-0.0.5/LICENSE
--rw-r--r--   0        0        0      243 2023-07-24 22:21:35.793575 flardl-0.0.5/LICENSE.logo.txt
--rw-r--r--   0        0        0     7841 2023-07-24 22:21:48.441846 flardl-0.0.5/README.md
--rw-r--r--   0        0        0     2781 2023-07-24 22:21:48.441846 flardl-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      673 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/__init__.py
--rw-r--r--   0        0        0     3380 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/common.py
--rw-r--r--   0        0        0     1581 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/dict_to_indexed_list.py
--rwxr-xr-x   0        0        0     8265 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/downloader.py
--rwxr-xr-x   0        0        0     4225 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/instrumented_streams.py
--rwxr-xr-x   0        0        0     7304 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/multidispatcher.py
--rw-r--r--   0        0        0        0 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/py.typed
--rw-r--r--   0        0        0      651 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/server_defs.py
--rwxr-xr-x   0        0        0    11622 2023-07-24 22:21:35.797575 flardl-0.0.5/src/flardl/stream_stats.py
--rw-r--r--   0        0        0     9181 1970-01-01 00:00:00.000000 flardl-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1958 2023-07-26 20:59:49.908917 flardl-0.0.6/LICENSE
+-rw-r--r--   0        0        0      243 2023-07-26 20:59:49.908917 flardl-0.0.6/LICENSE.logo.txt
+-rw-r--r--   0        0        0     7841 2023-07-26 20:59:49.908917 flardl-0.0.6/README.md
+-rw-r--r--   0        0        0     2780 2023-07-26 21:00:01.512897 flardl-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      673 2023-07-26 20:59:49.912917 flardl-0.0.6/src/flardl/__init__.py
+-rw-r--r--   0        0        0     3380 2023-07-26 20:59:49.912917 flardl-0.0.6/src/flardl/common.py
+-rw-r--r--   0        0        0     1581 2023-07-26 20:59:49.916917 flardl-0.0.6/src/flardl/dict_to_indexed_list.py
+-rwxr-xr-x   0        0        0     8243 2023-07-26 21:00:01.512897 flardl-0.0.6/src/flardl/downloader.py
+-rwxr-xr-x   0        0        0     4225 2023-07-26 20:59:49.916917 flardl-0.0.6/src/flardl/instrumented_streams.py
+-rwxr-xr-x   0        0        0     7663 2023-07-26 21:00:01.512897 flardl-0.0.6/src/flardl/multidispatcher.py
+-rw-r--r--   0        0        0        0 2023-07-26 20:59:49.916917 flardl-0.0.6/src/flardl/py.typed
+-rw-r--r--   0        0        0      651 2023-07-26 20:59:49.916917 flardl-0.0.6/src/flardl/server_defs.py
+-rwxr-xr-x   0        0        0    11622 2023-07-26 20:59:49.916917 flardl-0.0.6/src/flardl/stream_stats.py
+-rw-r--r--   0        0        0     9181 1970-01-01 00:00:00.000000 flardl-0.0.6/PKG-INFO
```

### Comparing `flardl-0.0.5/LICENSE` & `flardl-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flardl-0.0.5/README.md` & `flardl-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 work very well on the real-world power-law collections that are most
 important.
 
 **Modal values are a good statistic for power-law distributions**, unlike
 means. To put that another way, the average download time $\overline{t_{dl}}$
 varies a lot
 between runs, but the _most-common_ download time
-$\tilde{t_{dl}}$ can be pretty
+$\tilde{t}_{dl}$ can be pretty
 consistent. The mode of file lengths and the mode of download bit rate
 are both quantities that are easy to estimate for a
 collection and a collection and rarely change. If one happens to select
 the biggest files for downloading, or if one happens to try downloading
 a long collection at the same time that someone is watching a high-bit-rate
 video on the same shared connection, then it's easy to adjust a bit
 for just that time.
```

### Comparing `flardl-0.0.5/pyproject.toml` & `flardl-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flardl"
-version = "0.0.5"
+version = "0.0.6"
 description = "Flardl"
 authors = ["Joel Berendzen <joel@generisbio.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/hydrationdynamics/flardl"
 repository = "https://github.com/hydrationdynamics/flardl"
 documentation = "https://flardl.readthedocs.io"
@@ -40,15 +40,15 @@
 uvloop = { version = ">=0.17.0", markers = "sys_platform != 'win32'"}
 trio = "^0.22.0"
 
 
 [tool.poetry.group.dev.dependencies]
 Pygments = ">=2.10.0"
 bandit = ">=1.7.4"
-black = ">=21.10b0"
+black = ">=23.7.0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 flake8 = ">=4.0.1"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
```

### Comparing `flardl-0.0.5/src/flardl/__init__.py` & `flardl-0.0.6/src/flardl/__init__.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.5/src/flardl/common.py` & `flardl-0.0.6/src/flardl/common.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.5/src/flardl/dict_to_indexed_list.py` & `flardl-0.0.6/src/flardl/dict_to_indexed_list.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.5/src/flardl/downloader.py` & `flardl-0.0.6/src/flardl/downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,19 +216,17 @@
         queue_depth: int,
         timeout_s: float,
         **super_kwargs,
     ):
         """Init with id number."""
         super().__init__(*args, **super_kwargs)
         self.hard_exceptions: tuple[()] | tuple[type[BaseException]] = (
-            httpx.ConnectError,
-        )
-        self.soft_exceptions: tuple[()] | tuple[type[BaseException]] = (
-            ConnectionError,
+            httpx.HTTPStatusError,
         )
+        self.soft_exceptions: tuple[()] | tuple[type[BaseException]] = (ValueError,)
         self.launch_rate = self.LAUNCH_RATE_MAX
         self.base_url = transport + "://" + server + "/"
         if dir != "":
             self.base_url += dir + "/"
         if transport_ver == "2":
             self.http2 = True
         else:
@@ -243,14 +241,14 @@
         worker_count: int,
         /,
         idx: int,
         path: str,
         out_filename: str,
     ):
         """Download a file."""
-        if not self.quiet:
-            self._logger.info(
-                f"Downloading {self.base_url}{path} to file {out_filename}"
-            )
         response = await self.client.get(path)
+        if response.status_code != httpx.codes.OK:
+            response.raise_for_status()
         dl_data = response.content
+        if not self.quiet:
+            print(out_filename)
         await self.add_result(dl_data, out_filename, idx, worker_count, result_q)
```

### Comparing `flardl-0.0.5/src/flardl/instrumented_streams.py` & `flardl-0.0.6/src/flardl/instrumented_streams.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.5/src/flardl/multidispatcher.py` & `flardl-0.0.6/src/flardl/multidispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from __future__ import annotations
 
 import sys
 from typing import Any
 
 # third-party imports
 import anyio
+import httpx
 import loguru
 from loguru import logger as mylogger
 
 from .common import DEFAULT_MAX_RETRIES
 from .common import INDEX_KEY
 from .common import SIMPLE_TYPES
 from .common import MillisecondTimer
@@ -139,25 +140,25 @@
         """Dispatch tasks to worker functions and handle exceptions."""
         while True:
             try:
                 # Get a set of arguments from the queue.
                 kwargs, worker_count = await arg_q.get(worker_name=worker.name)
             except anyio.WouldBlock:
                 return
-            # Do rate limiting, if a limiter is found in worker.
-            try:
-                await worker.limiter()
-            except AttributeError:
-                pass  # it's okay if worker didn't have a limiter
+            if worker_count > 0:
+                # Do rate limiting, if a limiter is found in worker.
+                try:
+                    await worker.limiter()
+                except AttributeError:
+                    pass  # it's okay if worker didn't have a limiter
             # Do the work and handle any exceptions encountered.
             try:
                 await worker.worker(result_q, worker_count, **kwargs)
             except worker.soft_exceptions as e:
                 # Errors to be requeued by worker, unless too many
-                idx = kwargs[INDEX_KEY]
                 async with self._lock:
                     idx = kwargs[INDEX_KEY]
                     self.n_exceptions += 1
                     if idx not in self.exception_counter:
                         self.exception_counter[idx] = 1
                     else:
                         self.exception_counter[idx] += 1
@@ -171,14 +172,23 @@
                         kwargs, worker.name, worker_count, e, arg_q
                     )
             except worker.hard_exceptions as e:
                 idx = kwargs[INDEX_KEY]
                 await worker.hard_exception_handler(
                     idx, worker.name, worker_count, e, failure_q
                 )
+            except httpx.ConnectError:
+                await worker.soft_exception_handler(
+                    kwargs,
+                    worker.name,
+                    worker_count,
+                    f"Server '{worker.name!r}' shutdown due to ConnectError",
+                    arg_q,
+                )
+                return
             except Exception as e:
                 # unhandled errors go to unhandled exception handler
                 idx = kwargs[INDEX_KEY]
                 await worker.unhandled_exception_handler(idx, e)
 
     def main(
         self,
```

### Comparing `flardl-0.0.5/src/flardl/server_defs.py` & `flardl-0.0.6/src/flardl/server_defs.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.5/src/flardl/stream_stats.py` & `flardl-0.0.6/src/flardl/stream_stats.py`

 * *Files identical despite different names*

### Comparing `flardl-0.0.5/PKG-INFO` & `flardl-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flardl
-Version: 0.0.5
+Version: 0.0.6
 Summary: Flardl
 Home-page: https://github.com/hydrationdynamics/flardl
 License: BSD-3-Clause
 Keywords: downloads,adaptive,federated
 Author: Joel Berendzen
 Author-email: joel@generisbio.com
 Requires-Python: >=3.9,<4
@@ -103,15 +103,15 @@
 work very well on the real-world power-law collections that are most
 important.
 
 **Modal values are a good statistic for power-law distributions**, unlike
 means. To put that another way, the average download time $\overline{t_{dl}}$
 varies a lot
 between runs, but the _most-common_ download time
-$\tilde{t_{dl}}$ can be pretty
+$\tilde{t}_{dl}$ can be pretty
 consistent. The mode of file lengths and the mode of download bit rate
 are both quantities that are easy to estimate for a
 collection and a collection and rarely change. If one happens to select
 the biggest files for downloading, or if one happens to try downloading
 a long collection at the same time that someone is watching a high-bit-rate
 video on the same shared connection, then it's easy to adjust a bit
 for just that time.
```

