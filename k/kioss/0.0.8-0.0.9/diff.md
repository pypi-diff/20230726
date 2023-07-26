# Comparing `tmp/kioss-0.0.8.tar.gz` & `tmp/kioss-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kioss-0.0.8.tar", last modified: Wed Jul 26 07:14:44 2023, max compression
+gzip compressed data, was "kioss-0.0.9.tar", last modified: Wed Jul 26 07:24:13 2023, max compression
```

## Comparing `kioss-0.0.8.tar` & `kioss-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:14:44.611529 kioss-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 07:14:21.000000 kioss-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:14:44.611529 kioss-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-26 07:14:21.000000 kioss-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:14:44.611529 kioss-0.0.8/kioss/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 07:14:21.000000 kioss-0.0.8/kioss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-26 07:14:21.000000 kioss-0.0.8/kioss/pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-26 07:14:21.000000 kioss-0.0.8/kioss/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:14:44.611529 kioss-0.0.8/kioss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:14:44.000000 kioss-0.0.8/kioss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-26 07:14:44.000000 kioss-0.0.8/kioss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 07:14:44.000000 kioss-0.0.8/kioss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 07:14:44.000000 kioss-0.0.8/kioss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 07:14:44.611529 kioss-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 07:14:21.000000 kioss-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:14:44.611529 kioss-0.0.8/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-26 07:14:21.000000 kioss-0.0.8/test/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-26 07:14:21.000000 kioss-0.0.8/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:24:13.961039 kioss-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 07:23:58.000000 kioss-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:24:13.961039 kioss-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-26 07:23:58.000000 kioss-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:24:13.957039 kioss-0.0.9/kioss/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-26 07:23:58.000000 kioss-0.0.9/kioss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-07-26 07:23:58.000000 kioss-0.0.9/kioss/pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-26 07:23:58.000000 kioss-0.0.9/kioss/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:24:13.957039 kioss-0.0.9/kioss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 07:24:13.000000 kioss-0.0.9/kioss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-26 07:24:13.000000 kioss-0.0.9/kioss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 07:24:13.000000 kioss-0.0.9/kioss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 07:24:13.000000 kioss-0.0.9/kioss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 07:24:13.961039 kioss-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-26 07:23:58.000000 kioss-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:24:13.961039 kioss-0.0.9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-07-26 07:23:58.000000 kioss-0.0.9/test/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-26 07:23:58.000000 kioss-0.0.9/test/test_util.py
```

### Comparing `kioss-0.0.8/LICENSE` & `kioss-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kioss-0.0.8/README.md` & `kioss-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `kioss-0.0.8/kioss/pipe.py` & `kioss-0.0.9/kioss/pipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,38 +324,51 @@
             if batch:
                 return batch
             else:
                 raise
 
 
 class _ConcurrentlyMergingPipe(Pipe[T]):
-    MAX_QUEUE_SIZE = 64
     MIN_SLEEP_TIME_MS = 0.005
+    MAX_NUM_WAITING_ELEMS_PER_THREAD = 16
 
     def __init__(self, iterators: List[Iterator[T]]) -> None:
         super().__init__(
-            iter(_ConcurrentlyMergingPipe._concurrently_merging_iterable(iterators))
+            iter(
+                _ConcurrentlyMergingPipe._concurrently_merging_iterable(
+                    iterators,
+                    max_queue_size=_ConcurrentlyMergingPipe.MAX_NUM_WAITING_ELEMS_PER_THREAD
+                    * len(iterators),
+                )
+            )
         )
 
     @staticmethod
-    def _pull_in_queue(iterator: Iterator[T], queue: Queue) -> None:
+    def _pull_in_queue(
+        iterator: Iterator[T], queue: Queue, max_queue_size: int
+    ) -> None:
         for elem in iterator:
             backoffed_sleep_time = _ConcurrentlyMergingPipe.MIN_SLEEP_TIME_MS
-            while queue.qsize() > _ConcurrentlyMergingPipe.MAX_QUEUE_SIZE:
+            while queue.qsize() > max_queue_size:
                 time.sleep(backoffed_sleep_time)
                 backoffed_sleep_time *= 2
             queue.put(elem)
 
     @staticmethod
-    def _concurrently_merging_iterable(iterators: List[Iterator[T]]) -> Iterator[T]:
+    def _concurrently_merging_iterable(
+        iterators: List[Iterator[T]], max_queue_size: int
+    ) -> Iterator[T]:
         queue = Queue()
         with ThreadPoolExecutor(max_workers=len(iterators)) as executor:
             futures = [
                 executor.submit(
-                    _ConcurrentlyMergingPipe._pull_in_queue, iterator, queue
+                    _ConcurrentlyMergingPipe._pull_in_queue,
+                    iterator,
+                    queue,
+                    max_queue_size,
                 )
                 for iterator in iterators
             ]
             while not queue.empty() or not all((future.done() for future in futures)):
                 try:
                     yield queue.get(block=False)
                 except Empty:
```

### Comparing `kioss-0.0.8/test/test_pipe.py` & `kioss-0.0.9/test/test_pipe.py`

 * *Files identical despite different names*

