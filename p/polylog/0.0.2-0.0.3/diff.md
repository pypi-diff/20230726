# Comparing `tmp/polylog-0.0.2.tar.gz` & `tmp/polylog-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polylog-0.0.2.tar", last modified: Tue Jun 27 17:16:30 2023, max compression
+gzip compressed data, was "polylog-0.0.3.tar", last modified: Wed Jul 26 19:59:32 2023, max compression
```

## Comparing `polylog-0.0.2.tar` & `polylog-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:30.607716 polylog-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-27 17:16:30.607716 polylog-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-27 17:16:13.000000 polylog-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:30.603716 polylog-0.0.2/polylog/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-27 17:16:13.000000 polylog-0.0.2/polylog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-27 17:16:13.000000 polylog-0.0.2/polylog/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:16:30.607716 polylog-0.0.2/polylog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-27 17:16:30.000000 polylog-0.0.2/polylog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-27 17:16:30.000000 polylog-0.0.2/polylog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:16:30.000000 polylog-0.0.2/polylog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-27 17:16:30.000000 polylog-0.0.2/polylog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 17:16:30.000000 polylog-0.0.2/polylog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-27 17:16:21.000000 polylog-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:16:30.607716 polylog-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-27 17:16:13.000000 polylog-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:59:32.091702 polylog-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-26 19:59:32.087702 polylog-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-26 19:59:18.000000 polylog-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:59:32.087702 polylog-0.0.3/polylog/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-26 19:59:18.000000 polylog-0.0.3/polylog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-07-26 19:59:18.000000 polylog-0.0.3/polylog/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:59:32.087702 polylog-0.0.3/polylog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-07-26 19:59:32.000000 polylog-0.0.3/polylog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-26 19:59:32.000000 polylog-0.0.3/polylog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 19:59:32.000000 polylog-0.0.3/polylog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 19:59:32.000000 polylog-0.0.3/polylog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 19:59:32.000000 polylog-0.0.3/polylog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-26 19:59:24.000000 polylog-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 19:59:32.091702 polylog-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-26 19:59:18.000000 polylog-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 19:59:32.087702 polylog-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-07-26 19:59:18.000000 polylog-0.0.3/tests/logger_test.py
```

### Comparing `polylog-0.0.2/PKG-INFO` & `polylog-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylog
-Version: 0.0.2
+Version: 0.0.3
 Summary: A custom python logging package
 Home-page: https://github.com/lvlcn-t/PolyLog
 Author: lvlcn-t
 Author-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Maintainer-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/lvlcn-t/polylog
 Project-URL: Bug Reports, https://github.com/lvlcn-t/polylog/issues
```

### Comparing `polylog-0.0.2/README.md` & `polylog-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `polylog-0.0.2/polylog/logger.py` & `polylog-0.0.3/polylog/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import os
 import logging
 import logging.handlers
 import threading
 from contextvars import ContextVar
+from typing import Union
 
 # Define context variables for traceId and spanId
-trace_id_var = ContextVar("trace_id", default=None)
-span_id_var = ContextVar("span_id", default=None)
+TRACE_ID: ContextVar[Union[None, str, int]] = ContextVar("trace_id", default=None)
+SPAN_ID: ContextVar[Union[None, str, int]] = ContextVar("span_id", default=None)
 
 
 class CustomFormatter(logging.Formatter):
     LEVEL_COLORS = [
         (logging.DEBUG, "\x1b[40;1m"),
         (logging.INFO, "\x1b[34;1m"),
         (logging.WARNING, "\x1b[33;1m"),
         (logging.ERROR, "\x1b[31m"),
         (logging.CRITICAL, "\x1b[41m"),
     ]
     FORMATS = {
         level: logging.Formatter(
-            f"\x1b[30;1m%(asctime)s\x1b[0m {color}%(levelname)-8s\x1b[0m \x1b[35m%(name)s\x1b[0m (traceId=%(traceId)s, spanId=%(spanId)s) -> %(message)s",
+            f"\x1b[30;1m%(asctime)s\x1b[0m {color}%(levelname)-8s\x1b[0m \x1b[35m%(name)s\x1b[0m %(extra)s %(message)s",
             "%Y-%m-%d %H:%M:%S",
         )
         for level, color in LEVEL_COLORS
     }
 
     def format(self, record):
         formatter = self.FORMATS.get(record.levelno)
@@ -32,26 +33,35 @@
 
         # Override the traceback to always print in red
         if record.exc_info:
             text = formatter.formatException(record.exc_info)
             record.exc_text = f"\x1b[31m{text}\x1b[0m"
 
         # Adding context data to record
-        record.traceId = trace_id_var.get()
-        record.spanId = span_id_var.get()
+        trace_id = TRACE_ID.get()
+        span_id = SPAN_ID.get()
+        extra = ""
+        if trace_id is not None:
+            extra += f"traceId={trace_id}, "
+        if span_id is not None:
+            extra += f"spanId={span_id}"
+        if extra:
+            extra = f"({extra.strip(', ')}) ->"
+        record.extra = extra
 
         output = formatter.format(record)
         # Remove the cache layer
         record.exc_text = None
         return output
 
 
 # Define a lock for logger switching
 logger_lock = threading.Lock()
 
+
 def setup_logger(module_name: str) -> logging.Logger:
     with logger_lock:
         # create logger
         library, _, _ = module_name.partition(".py")
         logger = logging.getLogger(library)
 
         log_level = os.getenv("LOG_LEVEL", "INFO")
```

### Comparing `polylog-0.0.2/polylog.egg-info/PKG-INFO` & `polylog-0.0.3/polylog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polylog
-Version: 0.0.2
+Version: 0.0.3
 Summary: A custom python logging package
 Home-page: https://github.com/lvlcn-t/PolyLog
 Author: lvlcn-t
 Author-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Maintainer-email: lvlcn-t <75443136+lvlcn-t@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/lvlcn-t/polylog
 Project-URL: Bug Reports, https://github.com/lvlcn-t/polylog/issues
```

### Comparing `polylog-0.0.2/pyproject.toml` & `polylog-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "polylog"  # Required
-version = "0.0.2"
+version = "0.0.3"
 description = "A custom python logging package"  # Optional
 
 readme = "README.md" # Optional
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 
 keywords = []  # Optional
```

### Comparing `polylog-0.0.2/setup.py` & `polylog-0.0.3/setup.py`

 * *Files identical despite different names*

