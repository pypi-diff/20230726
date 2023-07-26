# Comparing `tmp/aioskd-0.0.4.tar.gz` & `tmp/aioskd-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioskd-0.0.4.tar", last modified: Tue Jul 25 20:33:50 2023, max compression
+gzip compressed data, was "aioskd-0.0.5.tar", last modified: Wed Jul 26 14:35:45 2023, max compression
```

## Comparing `aioskd-0.0.4.tar` & `aioskd-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-25 20:33:50.252434 aioskd-0.0.4/
--rw-r--r--   0 bigmag_    (502) staff       (20)     1062 2023-07-25 16:20:16.000000 aioskd-0.0.4/LICENSE
--rw-r--r--   0 bigmag_    (502) staff       (20)      394 2023-07-25 20:33:50.252696 aioskd-0.0.4/PKG-INFO
--rw-r--r--   0 bigmag_    (502) staff       (20)       55 2023-07-25 16:20:16.000000 aioskd-0.0.4/README.md
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-25 20:33:50.240600 aioskd-0.0.4/aioskd/
--rw-r--r--   0 bigmag_    (502) staff       (20)       48 2023-07-25 20:22:27.000000 aioskd-0.0.4/aioskd/__init__.py
--rwxr-xr-x   0 bigmag_    (502) staff       (20)     1381 2023-07-25 19:16:18.000000 aioskd-0.0.4/aioskd/cli.py
--rw-r--r--   0 bigmag_    (502) staff       (20)     4569 2023-07-25 20:13:53.000000 aioskd-0.0.4/aioskd/scheduler.py
-drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-25 20:33:50.251913 aioskd-0.0.4/aioskd.egg-info/
--rw-r--r--   0 bigmag_    (502) staff       (20)      394 2023-07-25 20:33:49.000000 aioskd-0.0.4/aioskd.egg-info/PKG-INFO
--rw-r--r--   0 bigmag_    (502) staff       (20)      271 2023-07-25 20:33:50.000000 aioskd-0.0.4/aioskd.egg-info/SOURCES.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-25 20:33:49.000000 aioskd-0.0.4/aioskd.egg-info/dependency_links.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)       52 2023-07-25 20:33:49.000000 aioskd-0.0.4/aioskd.egg-info/entry_points.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)       13 2023-07-25 20:33:49.000000 aioskd-0.0.4/aioskd.egg-info/requires.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)        7 2023-07-25 20:33:49.000000 aioskd-0.0.4/aioskd.egg-info/top_level.txt
--rw-r--r--   0 bigmag_    (502) staff       (20)       38 2023-07-25 20:33:50.254121 aioskd-0.0.4/setup.cfg
--rw-r--r--   0 bigmag_    (502) staff       (20)      681 2023-07-25 20:33:44.000000 aioskd-0.0.4/setup.py
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-26 14:35:45.979254 aioskd-0.0.5/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1062 2023-07-25 16:20:16.000000 aioskd-0.0.5/LICENSE
+-rw-r--r--   0 bigmag_    (502) staff       (20)     5897 2023-07-26 14:35:45.979448 aioskd-0.0.5/PKG-INFO
+-rw-r--r--   0 bigmag_    (502) staff       (20)     4696 2023-07-26 13:46:39.000000 aioskd-0.0.5/README.md
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-26 14:35:45.971891 aioskd-0.0.5/aioskd/
+-rw-r--r--   0 bigmag_    (502) staff       (20)       48 2023-07-25 20:22:27.000000 aioskd-0.0.5/aioskd/__init__.py
+-rwxr-xr-x   0 bigmag_    (502) staff       (20)     1550 2023-07-26 11:13:59.000000 aioskd-0.0.5/aioskd/cli.py
+-rw-r--r--   0 bigmag_    (502) staff       (20)     5212 2023-07-26 13:32:17.000000 aioskd-0.0.5/aioskd/scheduler.py
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-26 14:35:45.975687 aioskd-0.0.5/aioskd.egg-info/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     5897 2023-07-26 14:35:45.000000 aioskd-0.0.5/aioskd.egg-info/PKG-INFO
+-rw-r--r--   0 bigmag_    (502) staff       (20)      313 2023-07-26 14:35:45.000000 aioskd-0.0.5/aioskd.egg-info/SOURCES.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        1 2023-07-26 14:35:45.000000 aioskd-0.0.5/aioskd.egg-info/dependency_links.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)       39 2023-07-26 14:35:45.000000 aioskd-0.0.5/aioskd.egg-info/entry_points.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)       13 2023-07-26 14:35:45.000000 aioskd-0.0.5/aioskd.egg-info/requires.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)        7 2023-07-26 14:35:45.000000 aioskd-0.0.5/aioskd.egg-info/top_level.txt
+-rw-r--r--   0 bigmag_    (502) staff       (20)       38 2023-07-26 14:35:45.980432 aioskd-0.0.5/setup.cfg
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1529 2023-07-26 14:32:04.000000 aioskd-0.0.5/setup.py
+drwxr-xr-x   0 bigmag_    (502) staff       (20)        0 2023-07-26 14:35:45.978305 aioskd-0.0.5/tests/
+-rw-r--r--   0 bigmag_    (502) staff       (20)     1866 2023-07-26 12:38:24.000000 aioskd-0.0.5/tests/test_cli.py
+-rw-r--r--   0 bigmag_    (502) staff       (20)     3663 2023-07-26 12:38:04.000000 aioskd-0.0.5/tests/test_scheduler.py
```

### Comparing `aioskd-0.0.4/LICENSE` & `aioskd-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aioskd-0.0.4/aioskd/cli.py` & `aioskd-0.0.5/aioskd/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 import click
-from importlib.machinery import SourceFileLoader
+from importlib.util import spec_from_file_location, module_from_spec
 
 
 sys.path.append(".")
 
 class CustomPath(click.Path):
 
     def __init__(self, *args, **kwargs):
@@ -21,16 +21,16 @@
         filename = path.split("/")[-1]
         converted_path = super().convert(path + ".py", param, ctx)
         
         return converted_path, filename, obj
 
 
 @click.command()
-@click.option("--app", "-A", help="path to file with tasks in simple format", type=CustomPath(exists=True))
-def schedule(app):
+@click.argument("app", type=CustomPath(exists=True))
+def skd(app):
  
     """Start work task's scheduler
 
         \b
         Example:
             my_project/src/run:app
         \b
@@ -38,16 +38,22 @@
             my_project/src - path to module,
             run.py - your module,
             app - object of Scheduler class"
             
     """
     path, name, obj = app
     
-    # Find import and execute module with tasks
-    module = SourceFileLoader(name, path).load_module()
+
+    # Create a spec for the module from the given file path
+    spec = spec_from_file_location(name, path)
+    # Create the module from the spec
+    module = module_from_spec(spec)
+    # Load and execute the module
+    spec.loader.exec_module(module)
 
     # Start Scheduler
     scheduler = getattr(module, obj)
     scheduler.run()
+    click.echo("Tasks completed successfully")
 
-if __name__ == "__main__":
-    schedule()
+if __name__ == "__main__": # pragma: no cover
+    skd()
```

### Comparing `aioskd-0.0.4/aioskd/scheduler.py` & `aioskd-0.0.5/aioskd/scheduler.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,35 +7,47 @@
 class SchedulerTask:
     """
         A class that displays the task of the scheduler
         :param task: Asynchronous function to be executed
         :param interval: The interval between which the asynchronous function should be executed
         :param repeat: Indicates whether the asynchronous function should be repeated or executed once
         :param immediate: If yes, the scheduler will not wait for the interval when starting the task for the FIRST TIME
+        :param iter_count: necessary number of repeats
+
     """
-    def __init__(self, task: Callable, interval: datetime.timedelta, repeat: bool = True, immediate: bool = False) -> None:
+    def __init__(self, task: Callable, interval: datetime.timedelta, immediate: bool = False, repeat: bool = True, iter_count: int | None = None) -> None:
         self.task = task
         self.interval = interval
+        self.count = 0
         self.repeat = repeat
-        self.immediate = immediate
+        self.iter_count = iter_count
+        if self.iter_count and not self.repeat:
+            raise ValueError("If you want to repeat set arg repeat=True")
 
+        self.immediate = immediate
         if self.immediate:
             self.time_to = datetime.datetime.now()
         else:
             self.time_to = None
 
-    def set_time(self) -> None:
+    def next_iter(self):
+        self.count += 1
+        self.set_time()
+
+    def set_time(self) -> datetime.datetime:
         """
             Sets the time at which the self.task should be executed
         """
         self.time_to = datetime.datetime.now() + self.interval
+        return self.time_to
 
     async def wait_for_interval(self) -> None:
+        if not self.time_to:
+            raise RuntimeError("set_time() must be called")
         amount_of_time = self.time_to - datetime.datetime.now()
-
         await asyncio.sleep(amount_of_time.total_seconds())
 
     def time_to_do(self) -> bool:
         """
             Returns True if it is time to execute self.task
         """
         if self.time_to and datetime.datetime.now() >= self.time_to:
@@ -69,17 +81,17 @@
         """
             A coroutine that checks if it is time to execute the task, if so, executes it, if the task needs to be executed once (repeat), interrupts it, if not, sets a new time
             :param task: The task to be executed
         """
         while True:
             if task.time_to_do():
                 await task.task()
-                if not task.repeat:
+                if not task.repeat or task.count == task.iter_count:
                     break
-                task.set_time()
+                task.next_iter()
 
             await task.wait_for_interval()
 
     def _init_tasks(self) -> None:
         """
            A method that sets the execution time for all tasks that require it
         """
@@ -89,27 +101,29 @@
         """
             Coroutine that creates tasks in which the scheduler tasks will be performed
         """
         self._init_tasks()
         tasks = [asyncio.create_task(self._execute_task(task)) for task in self.tasks]
         await asyncio.gather(*tasks)
 
-    def schedule(self, interval: datetime.timedelta, repeat: bool = True, immediate: bool = False) -> Callable:
+    def schedule(self, interval: datetime.timedelta, immediate: bool = False, repeat: bool = True, iter_count: int | None = None) -> Callable:
         """
             Decorator that collects all the coroutines that need to be executed with time scheduling
             :param interval: The interval between which the asynchronous function should be executed
             :param repeat: Indicates whether the asynchronous function should be repeated or executed once
             :param immediate: If yes, the scheduler will not wait for the interval when starting the task for the FIRST TIME
+            :param iter_count: necessary number of repeats
         """
         def wrapper(func) -> None:
             """
                 :param func: Asynchronous function to be performed
             """
             if not iscoroutinefunction(func):
                 raise ValueError("Function under decorator must be await. Use 'async def' syntax")
-            task = SchedulerTask(task=func, interval=interval, repeat=repeat, immediate=immediate)
+            task = SchedulerTask(task=func, interval=interval, repeat=repeat, immediate=immediate, iter_count=iter_count)
             self.tasks.append(task)
+            return task
 
         return wrapper
 
     def run(self) -> None:
         asyncio.run(self._run_with_interval())
```

