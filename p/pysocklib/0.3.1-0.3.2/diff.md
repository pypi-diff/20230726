# Comparing `tmp/pysocklib-0.3.1.tar.gz` & `tmp/pysocklib-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysocklib-0.3.1.tar", last modified: Mon Jul 24 19:41:37 2023, max compression
+gzip compressed data, was "pysocklib-0.3.2.tar", last modified: Wed Jul 26 17:19:37 2023, max compression
```

## Comparing `pysocklib-0.3.1.tar` & `pysocklib-0.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-24 19:41:24.000000 pysocklib-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-24 19:41:37.398083 pysocklib-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-24 19:41:24.000000 pysocklib-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-24 19:41:24.000000 pysocklib-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 19:41:37.398083 pysocklib-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.394083 pysocklib-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.394083 pysocklib-0.3.1/src/pysocklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-24 19:41:37.000000 pysocklib-0.3.1/src/pysocklib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/basic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/basic/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/basic/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/basic/receive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/basic/send.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/services/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/services/abstract_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/services/samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:37.398083 pysocklib-0.3.1/src/socketlib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-24 19:41:24.000000 pysocklib-0.3.1/src/socketlib/utils/watch_dog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:37.749883 pysocklib-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-26 17:19:23.000000 pysocklib-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-26 17:19:37.749883 pysocklib-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-26 17:19:23.000000 pysocklib-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-26 17:19:23.000000 pysocklib-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:19:37.749883 pysocklib-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:37.745883 pysocklib-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:37.749883 pysocklib-0.3.2/src/pysocklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-07-26 17:19:37.000000 pysocklib-0.3.2/src/pysocklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-26 17:19:37.000000 pysocklib-0.3.2/src/pysocklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:19:37.000000 pysocklib-0.3.2/src/pysocklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 17:19:37.000000 pysocklib-0.3.2/src/pysocklib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 17:19:37.000000 pysocklib-0.3.2/src/pysocklib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 17:19:37.000000 pysocklib-0.3.2/src/pysocklib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:37.749883 pysocklib-0.3.2/src/socketlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:37.749883 pysocklib-0.3.2/src/socketlib/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/basic/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/basic/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/basic/receive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/basic/send.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:37.749883 pysocklib-0.3.2/src/socketlib/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:37.749883 pysocklib-0.3.2/src/socketlib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13521 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:37.749883 pysocklib-0.3.2/src/socketlib/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11591 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:37.749883 pysocklib-0.3.2/src/socketlib/services/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/services/abstract_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/services/samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:37.749883 pysocklib-0.3.2/src/socketlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-26 17:19:23.000000 pysocklib-0.3.2/src/socketlib/utils/watch_dog.py
```

### Comparing `pysocklib-0.3.1/LICENSE` & `pysocklib-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/PKG-INFO` & `pysocklib-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysocklib
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to work with socket clients and servers.
 Author-email: Daniel Ibarrola <daniel.ibarrola.sanchez@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Daniel Ibarrola Sánchez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysocklib-0.3.1/README.md` & `pysocklib-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/pyproject.toml` & `pysocklib-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=65.5.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysocklib"
-version = "0.3.1"
+version = "0.3.2"
 description = "Library to work with socket clients and servers."
 readme = "README.md"
 authors = [{ name = "Daniel Ibarrola", email = "daniel.ibarrola.sanchez@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -25,15 +25,15 @@
 [project.urls]
 Homepage = "https://github.com/Daniel-Ibarrola/SocketLib.git"
 
 [project.scripts]
 socketlib = "socketlib.__main__:main"
 
 [tool.bumpver]
-current_version = "0.3.1"
+current_version = "0.3.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `pysocklib-0.3.1/src/pysocklib.egg-info/PKG-INFO` & `pysocklib-0.3.2/src/pysocklib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysocklib
-Version: 0.3.1
+Version: 0.3.2
 Summary: Library to work with socket clients and servers.
 Author-email: Daniel Ibarrola <daniel.ibarrola.sanchez@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Daniel Ibarrola Sánchez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysocklib-0.3.1/src/pysocklib.egg-info/SOURCES.txt` & `pysocklib-0.3.2/src/pysocklib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/src/socketlib/basic/buffer.py` & `pysocklib-0.3.2/src/socketlib/basic/buffer.py`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/src/socketlib/basic/queues.py` & `pysocklib-0.3.2/src/socketlib/basic/queues.py`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/src/socketlib/basic/receive.py` & `pysocklib-0.3.2/src/socketlib/basic/receive.py`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/src/socketlib/basic/send.py` & `pysocklib-0.3.2/src/socketlib/basic/send.py`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/src/socketlib/cli/cli.py` & `pysocklib-0.3.2/src/socketlib/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/src/socketlib/client/client.py` & `pysocklib-0.3.2/src/socketlib/client/client.py`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/src/socketlib/server/server.py` & `pysocklib-0.3.2/src/socketlib/server/server.py`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/src/socketlib/services/abstract_service.py` & `pysocklib-0.3.2/src/socketlib/services/abstract_service.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,29 +18,29 @@
         main thread. However, a custom function to terminate the service when needed
         can be used, and the service can also run in the main thread if necessary.
     """
     def __init__(
             self,
             in_queue: Optional[queue.Queue] = None,
             out_queue: Optional[queue.Queue] = None,
-            stop: Callable[[], bool] = lambda: False,
+            stop: Optional[Callable[[], bool]] = None,
             events: Optional[dict[str, threading.Event]] = None,
             logger: Optional[logging.Logger] = None,
     ):
-        # Main thread of this service
         self._in = in_queue if in_queue is not None else queue.Queue()
         self._out = out_queue if out_queue is not None else queue.Queue()
         self._events = events if events is not None else dict()
         self._logger = logger
 
         self._process_thread = threading.Thread(
             target=self._handle_message,
             daemon=True
         )
-        self._stop = stop
+        self._stop_event = threading.Event()
+        self._stop = self._get_stop_function(stop, self._stop_event)
 
     @property
     def process_thread(self) -> threading.Thread:
         return self._process_thread
 
     @property
     def in_queue(self) -> queue.Queue:
@@ -62,12 +62,21 @@
         self._process_thread.start()
         if self._logger is not None:
             self._logger.debug(f"Started {self.__class__.__name__}")
 
     def join(self) -> None:
         self._process_thread.join()
 
+    @staticmethod
+    def _get_stop_function(
+            stop: Optional[Callable[[], bool]],
+            stop_event: threading.Event
+    ) -> Callable[[], bool]:
+        if stop is None:
+            return lambda: stop_event.is_set()
+        return stop
+
     def shutdown(self) -> None:
-        self._stop = lambda: True
+        self._stop_event.set()
         self.join()
         if self._logger is not None:
             self._logger.debug(f"Shutting down {self.__class__.__name__}")
```

### Comparing `pysocklib-0.3.1/src/socketlib/services/samples.py` & `pysocklib-0.3.2/src/socketlib/services/samples.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 class ToUpper(AbstractService):
 
     def __init__(
             self,
             msg_in: Optional[queue.Queue[str]] = None,
             msg_out: Optional[queue.Queue[str]] = None,
-            stop: Optional[Callable[[], bool]] = lambda: False,
+            stop: Optional[Callable[[], bool]] = None,
     ):
         super().__init__(msg_in, msg_out, stop)
 
     @property
     def msg_in(self) -> queue.Queue[str]:
         return self.in_queue
```

### Comparing `pysocklib-0.3.1/src/socketlib/utils/logger.py` & `pysocklib-0.3.2/src/socketlib/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pysocklib-0.3.1/src/socketlib/utils/watch_dog.py` & `pysocklib-0.3.2/src/socketlib/utils/watch_dog.py`

 * *Files identical despite different names*

