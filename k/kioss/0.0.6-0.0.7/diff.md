# Comparing `tmp/kioss-0.0.6.tar.gz` & `tmp/kioss-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.0.6.tar", last modified: Tue Jul 25 20:15:04 2023, max compression
+gzip compressed data, was "kioss-0.0.7.tar", last modified: Wed Jul 26 07:05:56 2023, max compression
```

## Comparing `kioss-0.0.6.tar` & `kioss-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:04.289058 kioss-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 20:14:51.000000 kioss-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 20:15:04.289058 kioss-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-25 20:14:51.000000 kioss-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:04.289058 kioss-0.0.6/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-25 20:14:51.000000 kioss-0.0.6/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-25 20:14:51.000000 kioss-0.0.6/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 20:14:51.000000 kioss-0.0.6/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:04.289058 kioss-0.0.6/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 20:15:04.000000 kioss-0.0.6/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-25 20:15:04.000000 kioss-0.0.6/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:15:04.000000 kioss-0.0.6/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 20:15:04.000000 kioss-0.0.6/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:15:04.289058 kioss-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-25 20:14:51.000000 kioss-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:15:04.289058 kioss-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-07-25 20:14:51.000000 kioss-0.0.6/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 20:14:51.000000 kioss-0.0.6/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:05:56.440790 kioss-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 07:05:39.000000 kioss-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:05:56.440790 kioss-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-26 07:05:39.000000 kioss-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:05:56.440790 kioss-0.0.7/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 07:05:39.000000 kioss-0.0.7/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-07-26 07:05:39.000000 kioss-0.0.7/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-26 07:05:39.000000 kioss-0.0.7/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:05:56.440790 kioss-0.0.7/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:05:56.000000 kioss-0.0.7/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-26 07:05:56.000000 kioss-0.0.7/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 07:05:56.000000 kioss-0.0.7/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 07:05:56.000000 kioss-0.0.7/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 07:05:56.440790 kioss-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 07:05:39.000000 kioss-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:05:56.440790 kioss-0.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-26 07:05:39.000000 kioss-0.0.7/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-26 07:05:39.000000 kioss-0.0.7/test/test_util.py
```

### Comparing `kioss-0.0.6/LICENSE` & `kioss-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.0.6/README.md` & `kioss-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ```python
 from kioss import Pipe
 
 words_count: int = (
     Pipe(open("...", "r"))
     .map(str.split)
-    .explode()
+    .flatten()
     .map(lambda _: 1)
     .reduce(int.__add__, initial=0)
 )
 ```
 
 ## Features
 - mutate
```

### Comparing `kioss-0.0.6/kioss/pipe.py` & `kioss-0.0.7/kioss/pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                 executor = ThreadPoolExecutor(max_workers=num_threads)
                 # non consumed map results block the worker that produced them, hence it makes it compatible with self.slow()
                 yield from executor.map(func, self)
                 executor.shutdown()
 
             return Pipe[R](iter(iterable()))
 
-    def flatten(self: "Pipe[Iterable[R]]") -> "Pipe[R]":
+    def flatten(self: "Pipe[List[R]]") -> "Pipe[R]":
         """
         Flatten the elements of the Pipe, which are assumed to be iterables, creating a new Pipe with individual elements.
 
         Returns:
             Pipe[R]: A new Pipe instance with individual elements obtained by flattening the original elements.
         """
         return _FlatteningPipe[R](self)
@@ -220,15 +220,15 @@
             .map(repr)
             .collect(limit=num_error_samples)
         ):
             raise RuntimeError(errors)
 
 
 class _FlatteningPipe(Pipe[R]):
-    def __init__(self, iterator: Iterator[Iterable[R]]) -> None:
+    def __init__(self, iterator: Iterator[List[R]]) -> None:
         super().__init__(iterator)
         self.current_iterator_elem = iter(super().__next__())
 
     def __next__(self) -> R:
         try:
             return next(self.current_iterator_elem)
         except StopIteration:
```

### Comparing `kioss-0.0.6/test/test_pipe.py` & `kioss-0.0.7/test/test_pipe.py`

 * *Files 8% similar despite different names*

```diff
@@ -150,15 +150,13 @@
 
     def test_catch(self):
         self.assertListEqual(
             list(Pipe(["1", "r", "2"]).map(int).catch().map(type)),
             [int, ValueError, int],
         )
 
-    def test_log(self):
-        list(
-            Pipe(range(8))
-            .map(lambda elem: ("_" if elem % 2 else "") + str(elem))
-            .map(int)
-            .catch()
-            .log()
+    def test_superintend(self):
+        Pipe("123").map(int).superintend()
+        self.assertRaises(
+            RuntimeError,
+            lambda: Pipe("12-3").map(int).superintend(),
         )
```

