# Comparing `tmp/kioss-0.0.7.tar.gz` & `tmp/kioss-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.0.7.tar", last modified: Wed Jul 26 07:05:56 2023, max compression
+gzip compressed data, was "kioss-0.0.8.tar", last modified: Wed Jul 26 07:14:44 2023, max compression
```

## Comparing `kioss-0.0.7.tar` & `kioss-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:05:56.440790 kioss-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 07:05:39.000000 kioss-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:05:56.440790 kioss-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-26 07:05:39.000000 kioss-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:05:56.440790 kioss-0.0.7/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 07:05:39.000000 kioss-0.0.7/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-07-26 07:05:39.000000 kioss-0.0.7/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-26 07:05:39.000000 kioss-0.0.7/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:05:56.440790 kioss-0.0.7/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:05:56.000000 kioss-0.0.7/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-26 07:05:56.000000 kioss-0.0.7/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 07:05:56.000000 kioss-0.0.7/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 07:05:56.000000 kioss-0.0.7/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 07:05:56.440790 kioss-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 07:05:39.000000 kioss-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:05:56.440790 kioss-0.0.7/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-26 07:05:39.000000 kioss-0.0.7/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-26 07:05:39.000000 kioss-0.0.7/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:14:44.611529 kioss-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 07:14:21.000000 kioss-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:14:44.611529 kioss-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-26 07:14:21.000000 kioss-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:14:44.611529 kioss-0.0.8/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 07:14:21.000000 kioss-0.0.8/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-26 07:14:21.000000 kioss-0.0.8/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-26 07:14:21.000000 kioss-0.0.8/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:14:44.611529 kioss-0.0.8/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:14:44.000000 kioss-0.0.8/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-26 07:14:44.000000 kioss-0.0.8/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 07:14:44.000000 kioss-0.0.8/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 07:14:44.000000 kioss-0.0.8/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 07:14:44.611529 kioss-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 07:14:21.000000 kioss-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:14:44.611529 kioss-0.0.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-26 07:14:21.000000 kioss-0.0.8/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-26 07:14:21.000000 kioss-0.0.8/test/test_util.py
```

### Comparing `kioss-0.0.7/LICENSE` & `kioss-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.0.7/README.md` & `kioss-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 
 ```python
 from kioss import Pipe
 
 words_count: int = (
     Pipe(open("...", "r"))
     .map(str.split)
+    .map(iter)
     .flatten()
     .map(lambda _: 1)
     .reduce(int.__add__, initial=0)
 )
 ```
 
 ## Features
 - mutate
     - `.merge` several pipes to form a new one that yields elements using multiple threads
     - `.chain` several pipes to form a new one that yields elements of one pipe after the previous one is exhausted.
     - `.map` over pipe's elements uing multiple threads
-    - `.flatten` a pipeline that yields iterable elements to make it separately yield each object contained in the element
+    - `.flatten` a pipe, whose elements are assumed to be iterators, creating a new pipe with individual elements
     - `.filter` a pipe
     - `.batch` pipe's elements and yield them as lists of a given max size or spanning over a given max period.
 - manage
     - `.log` a pipe's iteration status
     - `.catch` any pipe's error to treat it after iteration
     - `.slow` a pipe to limit the iteration's speed over it
 - consume
```

### Comparing `kioss-0.0.7/kioss/pipe.py` & `kioss-0.0.8/kioss/pipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,17 @@
                 executor = ThreadPoolExecutor(max_workers=num_threads)
                 # non consumed map results block the worker that produced them, hence it makes it compatible with self.slow()
                 yield from executor.map(func, self)
                 executor.shutdown()
 
             return Pipe[R](iter(iterable()))
 
-    def flatten(self: "Pipe[List[R]]") -> "Pipe[R]":
+    def flatten(self: "Pipe[Iterator[R]]") -> "Pipe[R]":
         """
-        Flatten the elements of the Pipe, which are assumed to be iterables, creating a new Pipe with individual elements.
+        Flatten the elements of the Pipe, which are assumed to be iterators, creating a new Pipe with individual elements.
 
         Returns:
             Pipe[R]: A new Pipe instance with individual elements obtained by flattening the original elements.
         """
         return _FlatteningPipe[R](self)
 
     def filter(self, predicate: Callable[[T], bool]) -> "Pipe[T]":
@@ -220,15 +220,15 @@
             .map(repr)
             .collect(limit=num_error_samples)
         ):
             raise RuntimeError(errors)
 
 
 class _FlatteningPipe(Pipe[R]):
-    def __init__(self, iterator: Iterator[List[R]]) -> None:
+    def __init__(self, iterator: Iterator[Iterator[R]]) -> None:
         super().__init__(iterator)
         self.current_iterator_elem = iter(super().__next__())
 
     def __next__(self) -> R:
         try:
             return next(self.current_iterator_elem)
         except StopIteration:
```

### Comparing `kioss-0.0.7/test/test_pipe.py` & `kioss-0.0.8/test/test_pipe.py`

 * *Files identical despite different names*

