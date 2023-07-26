# Comparing `tmp/asyncz-0.4.0.tar.gz` & `tmp/asyncz-0.5.0.tar.gz`

## Comparing `asyncz-0.4.0.tar` & `asyncz-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/__init__.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/_mapping.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/datastructures.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/enums.py
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/py.typed
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/state.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/typing.py
--rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/contrib/esmerald/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/contrib/esmerald/decorator.py
--rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/contrib/esmerald/scheduler.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/events/__init__.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/events/base.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/events/constants.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/__init__.py
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/asyncio.py
--rw-r--r--   0        0        0     7796 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/base.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/debug.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/pool.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/executors/types.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/__init__.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/asyncio.py
--rw-r--r--   0        0        0    39886 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/base.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/datastructures.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/types.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/schedulers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/__init__.py
--rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/base.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/memory.py
--rw-r--r--   0        0        0     5116 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/mongo.py
--rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/redis.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/stores/types.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/tasks/__init__.py
--rw-r--r--   0        0        0    10428 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/tasks/base.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/tasks/types.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/__init__.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/base.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/combination.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/date.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/interval.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/types.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/__init__.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/constants.py
--rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/expressions.py
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/fields.py
--rw-r--r--   0        0        0     9942 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/trigger.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 asyncz-0.4.0/asyncz/triggers/cron/types.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 asyncz-0.4.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 asyncz-0.4.0/LICENSE
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 asyncz-0.4.0/README.md
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 asyncz-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 asyncz-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/__init__.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/_mapping.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/datastructures.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/enums.py
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/py.typed
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/state.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/typing.py
+-rw-r--r--   0        0        0    11409 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/contrib/esmerald/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/contrib/esmerald/decorator.py
+-rw-r--r--   0        0        0     7890 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/contrib/esmerald/scheduler.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/events/__init__.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/events/base.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/events/constants.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/asyncio.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/base.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/debug.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/pool.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/executors/types.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/__init__.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/asyncio.py
+-rw-r--r--   0        0        0    39885 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/base.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/datastructures.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/types.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/schedulers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/__init__.py
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/base.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/memory.py
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/mongo.py
+-rw-r--r--   0        0        0     5490 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/redis.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/stores/types.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/tasks/__init__.py
+-rw-r--r--   0        0        0    10622 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/tasks/base.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/tasks/types.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/__init__.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/base.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/combination.py
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/date.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/interval.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/types.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/__init__.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/constants.py
+-rw-r--r--   0        0        0    10433 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/expressions.py
+-rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/fields.py
+-rw-r--r--   0        0        0     9942 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/trigger.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 asyncz-0.5.0/asyncz/triggers/cron/types.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 asyncz-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 asyncz-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 asyncz-0.5.0/README.md
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 asyncz-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    10874 2020-02-02 00:00:00.000000 asyncz-0.5.0/PKG-INFO
```

### Comparing `asyncz-0.4.0/asyncz/_mapping.py` & `asyncz-0.5.0/asyncz/_mapping.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/datastructures.py` & `asyncz-0.5.0/asyncz/datastructures.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/exceptions.py` & `asyncz-0.5.0/asyncz/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/utils.py` & `asyncz-0.5.0/asyncz/utils.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/contrib/esmerald/decorator.py` & `asyncz-0.5.0/asyncz/contrib/esmerald/decorator.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/contrib/esmerald/scheduler.py` & `asyncz-0.5.0/asyncz/contrib/esmerald/scheduler.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/events/base.py` & `asyncz-0.5.0/asyncz/events/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/events/constants.py` & `asyncz-0.5.0/asyncz/events/constants.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/executors/asyncio.py` & `asyncz-0.5.0/asyncz/executors/asyncio.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/executors/base.py` & `asyncz-0.5.0/asyncz/executors/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         Sends the task for execution.
 
         Args:
             task: A Task instanceyo execute.
             run_times: A list of datetimes specifying when the task should have been run.
         """
         assert self.lock is not None, "This executor has not been started yet."
-
         with self.lock:
             if self.instances[task.id] >= task.max_instances:
                 raise MaximumInstancesError(task.id, task.max_instances)
 
             self.do_send_task(task, run_times)
             self.instances[task.id] += 1
```

### Comparing `asyncz-0.4.0/asyncz/executors/debug.py` & `asyncz-0.5.0/asyncz/executors/debug.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/executors/pool.py` & `asyncz-0.5.0/asyncz/executors/pool.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/schedulers/asyncio.py` & `asyncz-0.5.0/asyncz/schedulers/asyncio.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/schedulers/base.py` & `asyncz-0.5.0/asyncz/schedulers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,14 @@
                 self.executors[alias] = executor = self.create_plugin_instance(
                     PluginInstance.EXECUTOR, executor, executor_options
                 )
             else:
                 raise TypeError(
                     f"Expected an executor instance or a string, got {executor.__class__.__name__} instead."
                 )
-
             if self.state != SchedulerState.STATE_STOPPED:
                 executor.start(self, alias)
 
         self.dispatch_event(SchedulerEvent(code=EXECUTOR_ADDED, alias=alias))
 
     def remove_executor(self, alias: str, shutdown: bool = True):
         """
```

### Comparing `asyncz-0.4.0/asyncz/schedulers/datastructures.py` & `asyncz-0.5.0/asyncz/schedulers/datastructures.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/stores/base.py` & `asyncz-0.5.0/asyncz/stores/base.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/stores/memory.py` & `asyncz-0.5.0/asyncz/stores/memory.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/stores/mongo.py` & `asyncz-0.5.0/asyncz/stores/mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     def lookup_task(self, task_id: Union[str, int]) -> "TaskType":
         document = self.collection.find_one(task_id, ["state"])
         return self.rebuild_task(document["state"]) if document else None
 
     def rebuild_task(self, state: Any) -> "TaskType":
         state = pickle.loads(state)
-        task = Task.__new__(TaskType)
+        task = Task.__new__(Task)
         task.__setstate__(state)
         task.scheduler = self.scheduler
         task.store_alias = self.alias
         return task
 
     def get_due_tasks(self, now: datetime) -> List["Task"]:
         timestamp = datetime_to_utc_timestamp(now)
```

### Comparing `asyncz-0.4.0/asyncz/stores/redis.py` & `asyncz-0.5.0/asyncz/stores/redis.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/tasks/base.py` & `asyncz-0.5.0/asyncz/tasks/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
     name: Optional[str] = None
     fn: Optional[Union[Callable[..., Any], str]] = None
     fn_reference: Optional[str] = None
     args: Optional[Any] = None
     kwargs: Optional[Any] = None
     next_run_time: Optional[datetime] = None
+    scheduler: Any = None
+    store_alias: Optional[str] = None
 
     def __init__(
         self,
         scheduler: Any,
         id: Optional[str] = None,
         store_alias: Optional[str] = None,
         **kwargs: Any,
@@ -216,14 +218,16 @@
 
         for key, value in approved.items():
             setattr(self, key, value)
 
     def __setstate__(self, state):
         object_setattr(self, "__dict__", state.__dict__)
         object_setattr(self, "__pydantic_fields_set__", state.__pydantic_fields_set__)
+        object_setattr(self, "__pydantic_extra__", state.__pydantic_extra__)
+        state.model_config.update(self.model_config)
 
         for name, value in self.__dict__.items():
             if name == "fn":
                 self.__dict__[name] = ref_to_obj(value)
 
         for name, value in state.__private_attributes__.items():
             if name == "fn":
```

### Comparing `asyncz-0.4.0/asyncz/triggers/base.py` & `asyncz-0.5.0/asyncz/triggers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     Base combination for the triggers.
 
     Args:
         triggers: A list of triggers.
         jitter: he maximum number of second to add to the next_trigger_time.
     """
 
+    triggers: Any = []
+
     def __init__(
         self,
         triggers: List["TriggerType"],
         jitter: Optional[int] = None,
         **kwargs: Any,
     ):
         super().__init__(**kwargs)
```

### Comparing `asyncz-0.4.0/asyncz/triggers/combination.py` & `asyncz-0.5.0/asyncz/triggers/combination.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/triggers/date.py` & `asyncz-0.5.0/asyncz/triggers/date.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/triggers/interval.py` & `asyncz-0.5.0/asyncz/triggers/interval.py`

 * *Files 9% similar despite different names*

```diff
@@ -90,18 +90,14 @@
             start_at=self.start_at,
             end_at=self.end_at,
             interval=self.interval,
             jitter=self.jitter,
         )
         return state
 
-    def __setstate__(self, state: Any) -> None:
-        trigger = super().__setstate__(state)
-        trigger.interval_size = timedelta_seconds(self.interval)
-
     def __str__(self) -> str:
         return f"interval[{self.interval}]"
 
     def __repr__(self) -> str:
         options = ["interval=%r" % self.interval, "start_at=%r" % datetime_repr(self.start_at)]
         if self.end_at:
             options.append("end_at=%r" % datetime_repr(self.end_at))
```

### Comparing `asyncz-0.4.0/asyncz/triggers/cron/constants.py` & `asyncz-0.5.0/asyncz/triggers/cron/constants.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/triggers/cron/expressions.py` & `asyncz-0.5.0/asyncz/triggers/cron/expressions.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/triggers/cron/fields.py` & `asyncz-0.5.0/asyncz/triggers/cron/fields.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/asyncz/triggers/cron/trigger.py` & `asyncz-0.5.0/asyncz/triggers/cron/trigger.py`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/LICENSE` & `asyncz-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/README.md` & `asyncz-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `asyncz-0.4.0/pyproject.toml` & `asyncz-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,21 +30,22 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 dependencies = [
     "asyncio>=3.4.3,<4.0.0",
     "loguru>=0.7.0,<0.8.0",
-    "pydantic>=2.0.0,<3.0.0",
+    "pydantic>=2.1.1,<3.0.0",
     "pytz>=2022.6",
     "tzlocal>=4.2,<5.0",
 ]
 keywords = [
     "api",
     "rest",
     "http",
@@ -85,14 +86,15 @@
     "ruff>=0.0.256,<1.0.0",
 ]
 
 dev = [
     "autoflake >=1.4.0,<3.0.0",
     "black>=22.10.0,<23.0.0",
     "flake8>=3.8.3,<7.0.0",
+    "ipdb>=0.13.13",
     "isort>=5.0.6,<6.0.0",
     "mypy>=0.982,<2.0.0",
     "pre-commit>=2.17.0,<3.0.0",
     "watchfiles>=0.16.1,<0.20.0",
 ]
 
 doc = [
```

### Comparing `asyncz-0.4.0/PKG-INFO` & `asyncz-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncz
-Version: 0.4.0
+Version: 0.5.0
 Summary: The scheduler that nobody wants but every application needs.
 Project-URL: Homepage, https://github.com/tarsil/asyncz
 Project-URL: Documentation, https://asyncz.tarsild.io/
 Project-URL: Changelog, https://asyncz.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/asyncz
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -23,36 +23,38 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: asyncio<4.0.0,>=3.4.3
 Requires-Dist: loguru<0.8.0,>=0.7.0
-Requires-Dist: pydantic<3.0.0,>=2.0.0
+Requires-Dist: pydantic<3.0.0,>=2.1.1
 Requires-Dist: pytz>=2022.6
 Requires-Dist: tzlocal<5.0,>=4.2
 Provides-Extra: all
 Requires-Dist: asyncio<4.0.0,>=3.4.3; extra == 'all'
 Requires-Dist: pytz>=2022.6; extra == 'all'
 Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: autoflake<3.0.0,>=1.4.0; extra == 'dev'
 Requires-Dist: black<23.0.0,>=22.10.0; extra == 'dev'
 Requires-Dist: flake8<7.0.0,>=3.8.3; extra == 'dev'
+Requires-Dist: ipdb>=0.13.13; extra == 'dev'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'dev'
 Requires-Dist: mypy<2.0.0,>=0.982; extra == 'dev'
 Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: watchfiles<0.20.0,>=0.16.1; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.2; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asyncz Version: 0.4.0 Summary: The scheduler that
+Metadata-Version: 2.1 Name: asyncz Version: 0.5.0 Summary: The scheduler that
 nobody wants but every application needs. Project-URL: Homepage, https://
 github.com/tarsil/asyncz Project-URL: Documentation, https://asyncz.tarsild.io/
 Project-URL: Changelog, https://asyncz.tarsild.io/release-notes/ Project-URL:
 Funding, https://github.com/sponsors/tarsil Project-URL: Source, https://
 github.com/tarsil/asyncz Author-email: Tiago Silva
 arasilva@gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 api,apscheduler,asgi,asyncz,cron,fastapi,framework,http,machine
@@ -12,30 +12,31 @@
 Intended Audience :: Developers Classifier: Intended Audience :: Information
 Technology Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
-Internet Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
-Internet :: WWW/HTTP :: HTTP Servers Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Application Frameworks Classifier: Topic
-:: Software Development :: Libraries :: Python Modules Classifier: Typing ::
-Typed Requires-Python: >=3.8 Requires-Dist: asyncio<4.0.0,>=3.4.3 Requires-
-Dist: loguru<0.8.0,>=0.7.0 Requires-Dist: pydantic<3.0.0,>=2.0.0 Requires-Dist:
-pytz>=2022.6 Requires-Dist: tzlocal<5.0,>=4.2 Provides-Extra: all Requires-
-Dist: asyncio<4.0.0,>=3.4.3; extra == 'all' Requires-Dist: pytz>=2022.6; extra
-== 'all' Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all' Provides-Extra: dev
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic ::
+Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
+Classifier: Topic :: Software Development Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Application Frameworks Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python: >=3.8
+Requires-Dist: asyncio<4.0.0,>=3.4.3 Requires-Dist: loguru<0.8.0,>=0.7.0
+Requires-Dist: pydantic<3.0.0,>=2.1.1 Requires-Dist: pytz>=2022.6 Requires-
+Dist: tzlocal<5.0,>=4.2 Provides-Extra: all Requires-Dist:
+asyncio<4.0.0,>=3.4.3; extra == 'all' Requires-Dist: pytz>=2022.6; extra ==
+'all' Requires-Dist: tzlocal<5.0,>=4.2; extra == 'all' Provides-Extra: dev
 Requires-Dist: autoflake<3.0.0,>=1.4.0; extra == 'dev' Requires-Dist:
 black<23.0.0,>=22.10.0; extra == 'dev' Requires-Dist: flake8<7.0.0,>=3.8.3;
-extra == 'dev' Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'dev' Requires-
-Dist: mypy<2.0.0,>=0.982; extra == 'dev' Requires-Dist: pre-
-commit<3.0.0,>=2.17.0; extra == 'dev' Requires-Dist:
+extra == 'dev' Requires-Dist: ipdb>=0.13.13; extra == 'dev' Requires-Dist:
+isort<6.0.0,>=5.0.6; extra == 'dev' Requires-Dist: mypy<2.0.0,>=0.982; extra ==
+'dev' Requires-Dist: pre-commit<3.0.0,>=2.17.0; extra == 'dev' Requires-Dist:
 watchfiles<0.20.0,>=0.16.1; extra == 'dev' Provides-Extra: doc Requires-Dist:
 mdx-include<2.0.0,>=1.4.2; extra == 'doc' Requires-Dist:
 mkautodoc<0.3.0,>=0.2.0; extra == 'doc' Requires-Dist: mkdocs-
 markdownextradata-plugin<0.3.0,>=0.2.5; extra == 'doc' Requires-Dist: mkdocs-
 material<10.0.0,>=9.0.13; extra == 'doc' Requires-Dist: mkdocs<2.0.0,>=1.1.2;
 extra == 'doc' Requires-Dist: mkdocstrings<0.30.0,>=0.20.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=6.0; extra == 'doc' Provides-Extra: test
```

