# Comparing `tmp/clean_ioc-0.2.1.tar.gz` & `tmp/clean_ioc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_ioc-0.2.1.tar", max compression
+gzip compressed data, was "clean_ioc-0.3.0.tar", max compression
```

## Comparing `clean_ioc-0.2.1.tar` & `clean_ioc-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-07-05 20:46:42.074594 clean_ioc-0.2.1/LICENSE
--rw-r--r--   0        0        0    16473 2023-07-05 20:46:42.074594 clean_ioc-0.2.1/README.md
--rw-r--r--   0        0        0    33608 2023-07-05 20:46:42.074594 clean_ioc-0.2.1/clean_ioc/__init__.py
--rw-r--r--   0        0        0      674 2023-07-05 20:46:42.074594 clean_ioc-0.2.1/clean_ioc/factories.py
--rw-r--r--   0        0        0     1320 2023-07-05 20:46:42.074594 clean_ioc-0.2.1/clean_ioc/functional_utils.py
--rw-r--r--   0        0        0     2228 2023-07-05 20:46:42.074594 clean_ioc-0.2.1/clean_ioc/registration_filters.py
--rw-r--r--   0        0        0      587 2023-07-05 20:46:42.074594 clean_ioc-0.2.1/clean_ioc/type_filters.py
--rw-r--r--   0        0        0     6569 2023-07-05 20:46:42.074594 clean_ioc-0.2.1/clean_ioc/typing_utils.py
--rw-r--r--   0        0        0     1125 2023-07-05 20:46:42.074594 clean_ioc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    17746 1970-01-01 00:00:00.000000 clean_ioc-0.2.1/setup.py
--rw-r--r--   0        0        0    17113 1970-01-01 00:00:00.000000 clean_ioc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-26 20:21:47.697404 clean_ioc-0.3.0/LICENSE
+-rw-r--r--   0        0        0    17673 2023-07-26 20:21:47.697404 clean_ioc-0.3.0/README.md
+-rw-r--r--   0        0        0    37928 2023-07-26 20:21:47.697404 clean_ioc-0.3.0/clean_ioc/__init__.py
+-rw-r--r--   0        0        0      674 2023-07-26 20:21:47.697404 clean_ioc-0.3.0/clean_ioc/factories.py
+-rw-r--r--   0        0        0     1320 2023-07-26 20:21:47.697404 clean_ioc-0.3.0/clean_ioc/functional_utils.py
+-rw-r--r--   0        0        0      558 2023-07-26 20:21:47.697404 clean_ioc-0.3.0/clean_ioc/list_reduction_filters.py
+-rw-r--r--   0        0        0      405 2023-07-26 20:21:47.697404 clean_ioc-0.3.0/clean_ioc/parent_context_filters.py
+-rw-r--r--   0        0        0     2228 2023-07-26 20:21:47.697404 clean_ioc-0.3.0/clean_ioc/registration_filters.py
+-rw-r--r--   0        0        0      587 2023-07-26 20:21:47.697404 clean_ioc-0.3.0/clean_ioc/type_filters.py
+-rw-r--r--   0        0        0     6555 2023-07-26 20:21:47.697404 clean_ioc-0.3.0/clean_ioc/typing_utils.py
+-rw-r--r--   0        0        0     1152 2023-07-26 20:21:47.701404 clean_ioc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    19003 1970-01-01 00:00:00.000000 clean_ioc-0.3.0/setup.py
+-rw-r--r--   0        0        0    18313 1970-01-01 00:00:00.000000 clean_ioc-0.3.0/PKG-INFO
```

### Comparing `clean_ioc-0.2.1/LICENSE` & `clean_ioc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.2.1/README.md` & `clean_ioc-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,16 @@
 
 client.get_number() # returns 10
 
 ```
 
 ## List resolving
 
+If you have multiple dependencues you can simply define a dependency as a list[T] and you can return all of the instances.
+
 ```python
 
 class ClientDependency
     def __init__(self, numbers: list[int]):
         self.numbers = numbers
 
     def get_numbers(self):
@@ -534,14 +536,57 @@
 ar1 = container.resolve(A, filter=has_tag("a", "a1")) # returns a1
 al1 = container.resolve(list[A], filter=has_tag("a"))  # returns [a2, a1]
 al2 = container.resolve(list[A], filter=has_tag("a", "a1")) # returns [a1]
 al3 = container.resolve(list[A], filter=fn_not(has_tag("a", "a1")))  # returns [a3, a2]
 al4 = container.resolve(list[A], filter=fn_not(has_tag("a"))) # returns [a3]
 al5 = container.resolve(list[A]) # returns [a3, a2, a1]
 ```
+
+
+
+## Parent Context Filters
+
+Registrations can also specify that should only apply to certain parents objects by setting the parent_context_filter
+
+```python
+def test_parent_context_filter():
+    class A:
+        pass
+
+    class B(A):
+        pass
+
+    class C(A):
+        pass
+
+    class D:
+        def __init__(self, a: A):
+            self.a = a
+
+    class E:
+        def __init__(self, a: A):
+            self.a = a
+
+    container = Container()
+
+    container.register(A, B, parent_context_filter=parent_implementation_is(E))
+    container.register(A, C, parent_context_filter=parent_implementation_is(D))
+    container.register(D)
+    container.register(E)
+
+    e = container.resolve(E)
+    d = container.resolve(D)
+
+    type(e.a) # returns B
+    type(d.a) # returns C
+
+```
+
+
+
 ## Accessing the Container, Scope and Resolver within dependencies
 
 Accessing container directly
 
 ```python
 class Client
     def __init__(self, container: Container)
@@ -596,14 +641,27 @@
 
 with container.get_scope() as scope:
     scope.register(int, instance=10)
     scoped_client = scope.resolve(Client)
     scoped_client.get_number() # returns 10
 ```
 
+Scopes can also be used as an async context manager
+
+```python
+class Client
+    async def get_number(self):
+        return 10
+
+container.register(Client)
+
+async with container.get_scope() as scope:
+    scoped_client = scope.resolve(Client)
+    await scoped_client.get_number() # returns 10
+```
 
 ## Modules
 
 
 A module is a just a function that accepts a container, it can be used to set up common elements on the container
 
 ```python
@@ -626,15 +684,14 @@
 
 client = container.resolve(Client)
 
 client.get_number() # returns 10
 ```
 
 
-
 ## DependencyContext (BETA feature)
 
 You can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing
 One example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context
 
 ```python
 class Logger
```

### Comparing `clean_ioc-0.2.1/clean_ioc/__init__.py` & `clean_ioc-0.3.0/clean_ioc/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Simple IOC container.
 """
 from __future__ import annotations
 import abc
 from collections import defaultdict, deque
 from dataclasses import dataclass
+from functools import reduce
 import types
 from enum import IntEnum
-from typing import Any, Type, get_type_hints
+from typing import Any, Sequence, Type, TypeVar, get_type_hints
 from collections.abc import Callable
 from typing import _GenericAlias  # type: ignore
 from uuid import uuid4
 from .functional_utils import constant, fn_and, fn_not
 from .type_filters import is_abstract
 from .typing_utils import (
     get_generic_bases,
@@ -19,14 +20,17 @@
     get_typevar_to_type_mapping,
     is_open_generic_type,
     try_to_complete_generic,
 )
 import inspect
 
 
+TService = TypeVar("TService")
+
+
 class _empty:
     def __bool__(self):
         return False
 
 
 class ArgInfo:
     def __init__(self, name: str, arg_type: type, default_value: Any):
@@ -51,14 +55,18 @@
     return d
 
 
 def _default_registration_filter(r: Registration) -> bool:
     return not r.is_named
 
 
+_default_registration_list_reducing_filter = constant(True)
+_default_parent_context_filter = constant(True)
+
+
 @dataclass
 class Tag:
     name: str
     value: str | None = None
 
 
 class Lifespan(IntEnum):
@@ -117,15 +125,15 @@
     def add_child(self, child_node: DependencyNode):
         self.children.append(child_node)
         child_node.parent = self
 
     def add_decorator(self, decorator_node: DependencyNode):
         self.decorator = decorator_node
         decorator_node.decorated = self
-        self.parent = decorator_node
+        decorator_node.parent = self.parent
 
     def add_pre_configuration(self, pre_configuration_node: DependencyNode):
         self.pre_configured_by = pre_configuration_node
         pre_configuration_node.pre_configures = self
 
 
 class DependencyContext:
@@ -133,14 +141,20 @@
         self.name = name
         self.service_type = dependency_node.service_type
         self.implementation = dependency_node.implementation
         self.parent = dependency_node.parent
         self.decorated = dependency_node.decorated
 
 
+class ParentContext:
+    def __init__(self, paramater_name: str, parent: DependencyNode):
+        self.parameter_name = paramater_name
+        self.parent = parent
+
+
 class DependencyGraph:
     def __init__(self, root_node: DependencyNode, resolved_object: Any):
         self.root_node = root_node
         self.resolved_instance = resolved_object
         self.children: list[DependencyGraph] = []
 
     def add_child(self, child_graph: DependencyGraph):
@@ -201,59 +215,70 @@
         else:
             self.service_type = service_type
         self.settings = settings
         self.is_dependency_context = service_type == DependencyContext
         self.is_generic_list = getattr(self.service_type, "__origin__", None) == list
         self.default_value = default_value
 
-    def resolve(self, context: ResolvingContext, depedency_node: DependencyNode):
+    def resolve(self, context: ResolvingContext, dependency_node: DependencyNode):
         if not self.settings.value == _empty:
             return self.settings.value
 
         if not self.default_value == _empty and self.settings.use_default_paramater:
             return self.default_value
 
+        parent_context = ParentContext(paramater_name=self.name, parent=dependency_node)
+
         if self.is_dependency_context:
-            return DependencyContext(name=self.name, dependency_node=depedency_node)
+            return DependencyContext(name=self.name, dependency_node=dependency_node)
 
         if self.is_generic_list:
-            regs = context.find_registrations(self.service_type.__args__[0], self.settings.filter)  # type: ignore
-            return [r.build(context, depedency_node) for r in regs]
+            regs = context.find_registrations(
+                service_type=self.service_type.__args__[0],  # type: ignore
+                registration_filter=self.settings.filter,
+                registration_list_reducing_filter=self.settings.list_reducing_filter,
+                parent_context=parent_context,
+            )
+            return [r.build(context, dependency_node) for r in regs]
         else:
             try:
-                reg = context.find_registration(self.service_type, self.settings.filter)
-                return reg.build(context, depedency_node)
+                reg = context.find_registration(
+                    service_type=self.service_type,
+                    registration_filter=self.settings.filter,
+                    parent_context=parent_context,
+                )
+                return reg.build(context, dependency_node)
             except CannotResolveException as ex:
                 ex.append(self)
                 raise ex
 
 
 class RootDependency(Dependency):
     @staticmethod
     def __PARENT_ROOT__():
         pass
 
-    def __init__(self, service_type: Any, settings: DependencySettings):
+    def __init__(self, service_type: type, settings: DependencySettings):
         super().__init__(
             name="__ROOT__",
             parent_implementation=RootDependency.__PARENT_ROOT__,
             service_type=service_type,
             settings=settings,
             default_value=_empty,
         )
 
-    def resolve_instance(self, context: ResolvingContext) -> DependencyGraph:
+    def resolve_instance(self, context: ResolvingContext) -> Any:
         graph = self.resolve_dependency_graph(context)
         return graph.resolved_instance
 
     def resolve_dependency_graph(self, context: ResolvingContext) -> DependencyGraph:
         root_node = DependencyNode(
             RootDependency, self.parent_implementation, lifespan=Lifespan.transient
         )
-        resolved_object = self.resolve(context=context, depedency_node=root_node)
+        resolved_object = self.resolve(context=context, dependency_node=root_node)
         return DependencyGraph(root_node=root_node, resolved_object=resolved_object)
 
 
 class ImplementationCreator:
     def __init__(
         self,
         creator_function: Callable,
@@ -397,26 +422,28 @@
     def __init__(
         self,
         service_type: type,
         implementation: Callable,
         lifespan: Lifespan,
         name: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
+        parent_context_filter: ParentContextFilter = _default_parent_context_filter,
         tags: list[Tag] | None = None,
     ):
         self.service_type = service_type
         self.implementation = implementation
         self.creator = ImplementationCreator(
             creator_function=implementation, dependency_config=dependency_config
         )
         self.lifespan = lifespan
         self.name = name
         self.tags = tuple(tags) if tags else tuple()
-        self._id = str(uuid4())
+        self.id = str(uuid4())
         self.generic_mapping = get_typevar_to_type_mapping(self.service_type)
+        self.parent_context_filter = parent_context_filter
 
     @property
     def is_named(self):
         return self.name is not None
 
     def has_tag(self, name: str, value: str | None):
         if value is not None:
@@ -441,30 +468,30 @@
                 pre_configuration.configuration_fn,
                 lifespan=Lifespan.singleton,
             )
             my_node.add_pre_configuration(pre_configuration_node)
 
             pre_configuration.run(context, pre_configuration_node)
 
-        cached_instance = context.get_cached(self._id)
+        cached_instance = context.get_cached(self.id)
         if not cached_instance == _empty:
             return cached_instance
         built_instance = self.creator.create(context, my_node)
         decorated_node = my_node
         for dec in context.find_decorators_that_apply(self):
             next_dec_node = DependencyNode(
                 service_type=self.service_type,
                 implementation=dec.decorator_type,
                 lifespan=self.lifespan,
             )
             decorated_node.add_decorator(next_dec_node)
             built_instance = dec.decorate(built_instance, context, next_dec_node)
             decorated_node = next_dec_node
 
-        context.new_instance_created(self._id, built_instance, self.lifespan)
+        context.new_instance_created(self, built_instance)
         return built_instance
 
 
 class Registry:
     def __init__(self):
         self._registrations: dict[type, deque[Registration]] = defaultdict(deque)
         self._decorators: dict[type, deque[Decorator]] = defaultdict(deque)
@@ -533,63 +560,92 @@
 
         instance = self.registry.singletons.get(registration_id, _empty)
         if instance is not _empty:
             self._current_items[registration_id] = instance
 
         return instance
 
-    def put(self, registration_id: str, instance: Any, lifespan: Lifespan):
-        if lifespan == Lifespan.singleton:
-            self.registry.add_singleton_instance(registration_id, instance)
-        elif lifespan == Lifespan.scoped:
-            self.scope.add_scoped_instance(registration_id, instance)
+    def put(self, registration: Registration, instance: Any):
+        if registration.lifespan == Lifespan.singleton:
+            self.registry.add_singleton_instance(registration.id, instance)
+        elif registration.lifespan == Lifespan.scoped:
+            self.scope.add_scoped_instance(
+                registration.id, registration.service_type, instance
+            )
 
-        if lifespan >= Lifespan.once_per_graph:
-            self._current_items[registration_id] = instance
+        if registration.lifespan >= Lifespan.once_per_graph:
+            self._current_items[registration.id] = instance
 
 
 class ResolvingContext:
     def __init__(self, registry: Registry, scope: Scope):
         self.registry = registry
         self.scope = scope
         self._cache = DependencyCache(registry=registry, scope=scope)
 
-    def try_generic_fallback(self, service_type: _GenericAlias):
+    def try_generic_fallback(
+        self, service_type: _GenericAlias, dependency_context: ParentContext
+    ):
         return self.find_registration(
-            service_type.__origin__, _default_registration_filter
+            service_type=service_type.__origin__,
+            registration_filter=_default_registration_filter,
+            parent_context=dependency_context,
         )
 
     def find_registration(
-        self, service_type: type, registration_finder: Callable
+        self,
+        service_type: type,
+        registration_filter: Callable,
+        parent_context: ParentContext,
     ) -> Registration:
-        regs = self.find_registrations(service_type, registration_finder)
+        regs = self.find_registrations(
+            service_type=service_type,
+            registration_filter=registration_filter,
+            registration_list_reducing_filter=constant(True),
+            parent_context=parent_context,
+        )
         reg = next(iter(regs), None)
 
         if reg is None:
             if type(service_type) == _GenericAlias:
-                reg = self.try_generic_fallback(service_type)
+                reg = self.try_generic_fallback(service_type, parent_context)
             if reg is None:
                 print(f"{service_type} is None")
                 raise CannotResolveException()
         return reg
 
     def find_registrations(
-        self, service_type: type, registration_filter: Callable[[Registration], bool]
+        self,
+        service_type: type,
+        registration_filter: Callable[[Registration], bool],
+        registration_list_reducing_filter: Callable[
+            [Registration, Sequence[Registration]], bool
+        ],
+        parent_context: ParentContext,
     ) -> list[Registration]:
         scoped_registrations = [
             r
             for r in self.scope.get_registrations(service_type)
-            if registration_filter(r)
+            if registration_filter(r) and r.parent_context_filter(parent_context)
         ]
         container_registrations = [
             r
             for r in self.registry.get_registrations(service_type)
-            if registration_filter(r)
+            if registration_filter(r) and r.parent_context_filter(parent_context)
         ]
-        return scoped_registrations + container_registrations
+        combined_registrations = scoped_registrations + container_registrations
+
+        def reducer(
+            accumulator: list[Registration], registration: Registration
+        ) -> list[Registration]:
+            if registration_list_reducing_filter(registration, accumulator):
+                accumulator.append(registration)
+            return accumulator
+
+        return reduce(reducer, combined_registrations, [])
 
     def find_decorators_that_apply(self, registration: Registration):
         return [
             d
             for d in self.registry.get_decorators(registration.service_type)
             if d.registration_filter(registration)
         ]
@@ -601,175 +657,194 @@
             if c.id not in self.registry.run_pre_configurations
             and c.filter(registration)
         ]
 
     def get_cached(self, reg_id: str):
         return self._cache.get(reg_id)
 
-    def new_instance_created(self, reg_id: str, instance: Any, lifespan: Lifespan):
-        self._cache.put(registration_id=reg_id, instance=instance, lifespan=lifespan)
+    def new_instance_created(self, registration: Registration, instance: Any):
+        self._cache.put(registration=registration, instance=instance)
 
     def mark_pre_configuration_as_ran(self, preconfiguration_id: str):
         self.registry.mark_pre_configuration_as_run(preconfiguration_id)
 
 
 class Resolver(abc.ABC):
     @abc.abstractmethod
     def resolve(
         self,
-        cls: type,
+        service_type: type[TService],
         filter: RegistrationFilter = _default_registration_filter,
         *args,
         **kwargs,
-    ) -> Any:
+    ) -> TService:
         pass
 
 
 class Scope(Resolver):
     def __init__(
         self,
     ):
-        self._registrations = defaultdict(deque)
-        self._scoped_instances = {}
+        self._registrations: dict[type, deque[Registration]] = defaultdict(deque)
+        self._scoped_instances: dict[str, Any] = {}
+        self._resolved_instances: dict[type, deque[Any]] = defaultdict(deque)
+
+    async def __aenter__(self):
+        await self.before_start_async()
+        return self
+
+    async def __aexit__(self, *args, **kwargs):
+        await self.after_finish_async()
 
     def __enter__(self):
+        self.before_start()
         return self
 
     def __exit__(self, *args, **kwargs):
+        self.after_finish()
+
+    def before_start(self):
         pass
 
-    @abc.abstractmethod
-    def add_scoped_instance(self, *args):
+    def after_finish(self):
         pass
 
+    async def before_start_async(self):
+        pass
+
+    async def after_finish_async(self):
+        pass
+
+    def add_scoped_instance(
+        self, registration_id: str, service_type: type, instance: Any
+    ):
+        self._scoped_instances[registration_id] = instance
+        self._resolved_instances[service_type].appendleft(instance)
+
     @abc.abstractmethod
     def register(
         self,
         service_type: type,
         impl_type: type | None = None,
         factory: Callable | None = None,
         instance: Any | None = None,
         name: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
+        parent_context_filter: ParentContextFilter = _default_parent_context_filter,
     ):
         pass
 
     def get_registrations(self, service_tyep):
         return self._registrations[service_tyep]
 
     @property
     def scoped_instances(self):
         return self._scoped_instances
 
+    def get_resolved_instances(
+        self, service_type: type[TService]
+    ) -> Sequence[TService]:
+        return self._resolved_instances[service_type]
+
 
 class ContainerScope(Scope):
     def __init__(self, container: Container):
+        super().__init__()
         self._container = container
-        self._registrations = defaultdict(deque)
-        self._scoped_instances = {}
-
         self.register(ContainerScope, instance=self)
         self.register(Resolver, instance=self)
 
     def register(
         self,
         service_type: type,
         impl_type: type | None = None,
         factory: Callable | None = None,
         instance: Any | None = None,
         name: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
         tags: list[Tag] | None = None,
+        parent_context_filter: ParentContextFilter = _default_parent_context_filter,
     ):
         if instance is not None:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=lambda: instance,
                     lifespan=Lifespan.scoped,
                     name=name,
                     tags=tags,
+                    parent_context_filter=parent_context_filter,
                 )
             )
         elif factory is not None:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=factory,
                     lifespan=Lifespan.scoped,
                     name=name,
                     dependency_config=dependency_config,
                     tags=tags,
+                    parent_context_filter=parent_context_filter,
                 )
             )
         elif impl_type is not None:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=impl_type,
                     lifespan=Lifespan.scoped,
                     name=name,
                     dependency_config=dependency_config,
                     tags=tags,
+                    parent_context_filter=parent_context_filter,
                 )
             )
         else:
             self._registrations[service_type].appendleft(
                 Registration(
                     service_type=service_type,
                     implementation=service_type,
                     lifespan=Lifespan.scoped,
                     name=name,
                     dependency_config=dependency_config,
                     tags=tags,
+                    parent_context_filter=parent_context_filter,
                 )
             )
 
-    def _before_start(self):
-        pass
-
-    def _after_finish(self):
-        pass
-
-    def __enter__(self):
-        self._before_start()
-        return self
-
-    def __exit__(self, *args, **kwargs):
-        self._after_finish()
-
-    def get_registrations(self, service_tyep):
-        return self._registrations[service_tyep]
-
-    def add_scoped_instance(self, registration_id: str, instance: Any):
-        self._scoped_instances[registration_id] = instance
-
     def resolve(
         self,
-        service_type: type,
+        service_type: type[TService],
         filter: RegistrationFilter = _default_registration_filter,
-    ):
+    ) -> TService:
         return self._container.resolve(
             service_type=service_type, filter=filter, scope=self
         )
 
 
 class EmptyContainerScope(Scope):
     def __init__(self):
         super().__init__()
 
-    def add_scoped_instance(self, *args):
-        pass
-
     def register(self, *args):
         pass
 
     def resolve(self, *args):
         pass
 
+    def get_resolved_instances(
+        self, service_type: type[TService]
+    ) -> Sequence[TService]:
+        return []
+
+    @property
+    def scoped_instances(self):
+        return {}
+
 
 class NeedsScopedRegistrationError(Exception):
     def __init__(self, service_type, name):
         self.service_type = service_type
         self.name = name
 
     def __str__(self):
@@ -812,74 +887,92 @@
         impl_type: type | None = None,
         factory: Callable | None = None,
         instance: Any | None = None,
         lifespan: Lifespan = Lifespan.once_per_graph,
         name: str | None = None,
         dependency_config: dict[str, DependencySettings] = {},
         tags: list[Tag] | None = None,
+        parent_context_filter: ParentContextFilter = _default_parent_context_filter,
     ):
         if instance is not None:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=lambda: instance,
                     dependency_config=dependency_config,
                     lifespan=Lifespan.singleton,
                     name=name,
                     tags=tags,
+                    parent_context_filter=parent_context_filter,
                 )
             )
         elif factory is not None:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=factory,
                     dependency_config=dependency_config,
                     lifespan=lifespan,
                     name=name,
                     tags=tags,
+                    parent_context_filter=parent_context_filter,
                 )
             )
         elif impl_type is not None:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=impl_type,
                     dependency_config=dependency_config,
                     lifespan=lifespan,
                     name=name,
                     tags=tags,
+                    parent_context_filter=parent_context_filter,
                 )
             )
         else:
             self.registry.add_registration(
                 Registration(
                     service_type=service_type,
                     implementation=service_type,
                     dependency_config=dependency_config,
                     lifespan=lifespan,
                     name=name,
                     tags=tags,
+                    parent_context_filter=parent_context_filter,
                 )
             )
 
     def register_subclasses(
         self,
         base_type: type,
         lifespan: Lifespan = Lifespan.once_per_graph,
         subclass_type_filter: Callable[[type], bool] = constant(True),
         get_registration_name: Callable[[type], str | None] = constant(None),
         tags: list[Tag] | None = None,
+        parent_context_filter: ParentContextFilter = _default_parent_context_filter,
     ):
         full_type_filter = fn_and(fn_not(is_abstract), subclass_type_filter)
         subclasses = get_subclasses(base_type, full_type_filter)
         for sc in subclasses:
             name = get_registration_name(sc)
-            self.register(base_type, sc, lifespan=lifespan, name=name, tags=tags)
-            self.register(sc, lifespan=lifespan, tags=tags)
+            self.register(
+                base_type,
+                sc,
+                lifespan=lifespan,
+                name=name,
+                tags=tags,
+                parent_context_filter=parent_context_filter,
+            )
+            self.register(
+                sc,
+                lifespan=lifespan,
+                tags=tags,
+                parent_context_filter=parent_context_filter,
+            )
 
     def register_decorator(
         self,
         service_type: type,
         decorator_type: type,
         registration_filter: Callable[
             [Registration], bool
@@ -915,14 +1008,15 @@
         generic_service_type: type,
         fallback_type: type | None = None,
         fallback_name: str | None = None,
         lifespan: Lifespan = Lifespan.once_per_graph,
         subclass_type_filter: Callable[[type], bool] = constant(True),
         get_registration_name: Callable[[type], str | None] = constant(None),
         tags: list[Tag] | None = None,
+        parent_context_filter: ParentContextFilter = _default_parent_context_filter,
     ):
         full_type_filter = fn_and(fn_not(is_abstract), subclass_type_filter)
         subclasses = get_subclasses(generic_service_type, full_type_filter)
         for subclass in subclasses:
             name = get_registration_name(subclass)
             target_generic_base = self._get_target_generic_base(
                 generic_service_type, subclass
@@ -930,23 +1024,25 @@
             if target_generic_base:
                 self.register(
                     target_generic_base,
                     subclass,
                     lifespan=lifespan,
                     name=name,
                     tags=tags,
+                    parent_context_filter=parent_context_filter,
                 )
 
         if fallback_type:
             self.register(
                 generic_service_type,
                 fallback_type,
                 lifespan=lifespan,
                 name=fallback_name,
                 tags=tags,
+                parent_context_filter=parent_context_filter,
             )
 
     def register_open_generic_decorator(
         self,
         generic_service_type: type,
         generic_decorator_type: type,
         subclass_type_filter: Callable[[type], bool] = constant(True),
@@ -984,18 +1080,18 @@
                         generic_decorator_type,
                         decorated_arg=decorated_arg,
                         dependency_config=dependency_config,
                     )
 
     def resolve(
         self,
-        service_type,
+        service_type: type[TService],
         filter: RegistrationFilter = _default_registration_filter,
         scope: Scope = EmptyContainerScope(),
-    ) -> Any:
+    ) -> TService:
         d = RootDependency(service_type, DependencySettings(filter=filter))
         context = ResolvingContext(self.registry, scope)
         return d.resolve_instance(context)
 
     def new_scope(
         self, ScopeClass: Type[ContainerScope] = ContainerScope, *args, **kwargs
     ) -> Scope:
@@ -1007,19 +1103,29 @@
             factory=type_expected_to_be_scoped(service_type, name),
             name=name,
         )
 
     def apply_module(self, module_fn: Callable[[Container], None]):
         module_fn(self)
 
-    def has_registration(self, service_type):
-        return len(self.registry.get_registrations(service_type)) > 0
+    def has_registration(
+        self, service_type, filter: RegistrationFilter = _default_registration_filter
+    ):
+        found_registrations = [
+            r for r in self.registry.get_registrations(service_type) if filter(r)
+        ]
+        return len(found_registrations) > 0
 
 
 @dataclass(kw_only=True)
 class DependencySettings:
     value: Any = _empty
     use_default_paramater: bool = True
     filter: RegistrationFilter = _default_registration_filter
+    list_reducing_filter: RegistrationListReducingFilter = (
+        _default_registration_list_reducing_filter
+    )
 
 
 RegistrationFilter = Callable[[Registration], bool]
+RegistrationListReducingFilter = Callable[[Registration, Sequence[Registration]], bool]
+ParentContextFilter = Callable[[ParentContext], bool]
```

### Comparing `clean_ioc-0.2.1/clean_ioc/factories.py` & `clean_ioc-0.3.0/clean_ioc/factories.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.2.1/clean_ioc/functional_utils.py` & `clean_ioc-0.3.0/clean_ioc/functional_utils.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.2.1/clean_ioc/registration_filters.py` & `clean_ioc-0.3.0/clean_ioc/registration_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.2.1/clean_ioc/type_filters.py` & `clean_ioc-0.3.0/clean_ioc/type_filters.py`

 * *Files identical despite different names*

### Comparing `clean_ioc-0.2.1/clean_ioc/typing_utils.py` & `clean_ioc-0.3.0/clean_ioc/typing_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import _GenericAlias, _SpecialGenericAlias, Protocol  # type: ignore
 from typing import Generic, TypeVar
 from collections.abc import Callable
 from typing import get_type_hints
 import types
 from queue import Queue
-import inspect
+
 
 typingGenericAlias = (_GenericAlias, _SpecialGenericAlias, types.GenericAlias)
 
 
 def get_subclasses(cls: type, filter: Callable[[type], bool] = lambda t: True):
     queue = Queue()
     queue.put(cls)
```

### Comparing `clean_ioc-0.2.1/pyproject.toml` & `clean_ioc-0.3.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clean_ioc"
-version = "0.2.1"
+version = "0.3.0"
 description = "An IOC Container for Python 3.10+"
 authors = ["Peter Daly"]
 license = "MIT"
 homepage = "https://github.com/peter-daly/clean_ioc"
 repository = "https://github.com/peter-daly/clean_ioc"
 documentation = "https://github.com/peter-daly/clean_ioc"
 readme = "README.md"
@@ -12,16 +12,17 @@
     "Development Status :: 5 - Production/Stable",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^6.2.5"
+pytest = "^7.0.0"
 pytest-cov = "^4.0.0"
+pytest-asyncio = "^0.21.1"
 black = "^22.3.0"
 flakeheaven = "^3.2.1"
 isort = "^5.10.1"
 mkdocs-material = "^8.5.11"
 wily = "^1.24.0"
 mkdocstrings-python = "^0.8.3"
 expects = "^0.9.0"
```

### Comparing `clean_ioc-0.2.1/setup.py` & `clean_ioc-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['clean_ioc']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'clean-ioc',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': 'An IOC Container for Python 3.10+',
-    'long_description': '# Clean IoC\nA simple dependency injection library for python that requires nothing of your application code (except that you use typing).\n\n\n## Basic Registering and resolving\n\nThere are 4 basic modes of registering a new set of classes\n\n### Implementation\n\n```python\n\nclass UserRepository(abc.ABC)\n    @abc.abstractmethod\n    def add(self, user):\n        pass\n\nclass InMemoryUserRepository(UserRepository)\n\n    def __init__(self):\n        self.users = []\n\n    def add(self, user):\n        # This is obviously terrible, but it\'s for demo purposes\n        self.users.append(user)\n\nclass SqlAlchemyUserRepository(UserRepository)\n\n    def __init__(self):\n        # Do some db stuff here\n        pass\n\n    def add(self, user):\n        # Do some db stuff here\n        pass\n\ncontainer = Container()\ncontainer.register(UserRepository, InMemoryUserRepository)\n\n\nrepository = container.resolve(UserRepository) # This will return an InMemoryUserRepository\n\n```\n\n### Concrete Class\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n### Factory\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_factory(dep: ClientDependency):\n    return Client(dep=dep)\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client, factory=client_factory)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n\n### Instance\n\n```python\n\nclass ClientDependency\n    def __init__(self, num):\n        self.num = num\n\n    def get_int(self):\n        return self.num\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\nclient_dependency = ClientDependency(num=10)\n\ncontainer = Container()\ncontainer.register(ClientDependency, instance=client_dependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n## List resolving\n\n```python\n\nclass ClientDependency\n    def __init__(self, numbers: list[int]):\n        self.numbers = numbers\n\n    def get_numbers(self):\n        return self.numbers\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_numbers(self):\n        return self.dep.get_numbers()\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nclient = container.resolve(Client)\n\nclient.get_numbers() # returns [3, 2, 1]\n```\n\n\n## Decorators\n\nFollows a object orientated decoration pattern, rather than a decoration annotation.\nThe main reason for this was to allow decotation of registered instances\n\n```python\nclass Client\n    def __init__(self, number: int)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\n\nclass DoubleClientDecorator(Client):\n    def __init__(self, client: Client):\n        self.client = client\n    def get_number(self):\n        return self.client.get_number() * 2\n\ncontainer = Container()\n\ncontainer.register(Client)\ncontainer.register_decorator(Client, DoubleClientDecorator)\ncontainer.register(int, instance=10)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 20\n```\n\n\nDecorators are resolved in order of when first registered. So the first registered decorator is the highest in the class tree\n\n\n```python\n    class Concrete:\n        pass\n\n    class DecoratorOne(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    class DecoratorTwo(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    container = Container()\n\n    container.register(Concrete)\n    container.register_decorator(Concrete, DecoratorOne)\n    container.register_decorator(Concrete, DecoratorTwo)\n\n    root = container.resolve(Concrete)\n\n    type(root) # returns DecoratorOne\n    type(root.child) # returns DecoratorTwo\n    type(root.child.child) # returns Concrete\n```\n\n\n## Subclasses registration\n\nThis feature allows registration of all subclasses of a giveb type\n\n```python\nclass Client(abc.ABC)\n    @abc.abstractmethod\n    def get_number(self):\n        pass\n\n\nclass TenClient(Client)\n    def get_number(self):\n        return 10\n\nclass TwentyClient(Client)\n    def get_number(self):\n        return 20\n\ncontainer = Container()\n\ncontainer.register_subclasses(Client)\n\nten_client = container.resolve(TenClient)\nten_client.get_number() # returns 10\n\ntwenty_client = container.resolve(TwentyClient)\ntwenty_client.get_number() # returns 20\n\n# Resolve all subsclasses of Client\nclient = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]\n```\n\n\n## Lifespans\nLifespans configure how long and resolved object says alive for\nThere are 4 lifespan types\n\n### transient\nAlways create a new instance\n\n```python\ncontainer.register(Client, lifespan=Lifespan.transient)\n```\n\n\n### once_per_graph (Default behaviour)\nOnly create one instance throughout the resolve call\n\n```python\ncontainer.register(Client, lifespan=Lifespan.once_per_graph)\n```\n\n### scoped\nOnly create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**\n\n```python\ncontainer.register(Client, lifespan=Lifespan.scoped)\n```\n\n### singleton\nOnly one instance of the object is created throughout the lifespan of the container\n\n```python\ncontainer.register(Client, lifespan=Lifespan.singleton)\n```\n\n*Note:*\nWhen registering an instance, then the behaviour is always singleton\n\n```python\ncontainer.register(int, instance=10)\n```\n\n## Open Generics\n\nRegisters all generic subclasses of the service type and allows you to resolve with the generic alias\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\n\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'HELLO\'\nh2.handle(GoodbyeCommand()) # prints \'GOODBYE\'\n\n```\n\n## Open Generic Decorators\n\n\nAllows you to add decorators to your open generic registrations\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\nclass AVeryBigCommandHandlerDecorator(Generic[T]):\n    def __init__(self, handler: CommandHandler[T]):\n        self.handler = handler\n\n    def handle(self, command: T):\n        print(\'A VERY BIG\')\n        self.handler.handle(command=command)\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\ncontainer.register_open_generic_decorator(CommandHandler, AVeryBigCommandHandlerDecorator)\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'A VERY BIG\\nHELLO\'\nh2.handle(GoodbyeCommand()) # prints \'A VERY BIG\\nGOODBYE\'\n\n```\n\n## Scopes\n\nScopes are a way to create a sub container that will live for a certain lifespan.\nSome good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system\n\n\n```python\nclass Client\n    def __init__(self, number: int)\n        return number\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n## Named registrations & Registration filters\n\nBy default the last unnamed registration is what the container will return when resolve is called as below.\n\n```python\n\ncontainer = Container()\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nnumber = container.resolve(int) # returns 3\n\n```\nTo be more selective of what we return we can add a name to the registration and apply a registration filter when we resolve.\n\nA registration filter is simply function that receives a **Registration** and returns a **bool**\n\nFor example if we wanted to get the int named **"One"** we do the following\n\n```python\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=lambda r: r.name == "One") # returns 1\n```\n\nClean IOC comes with a set of in built registration filters that can be found [here](./clean_ioc/registration_filters.py)\n\nWe can get the desired behaviour as above\n```python\nfrom clean_ioc.registration_filters import with_name\n\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=with_name("One")) # returns 1\n```\n\n## Dependency Settings\n\nDependency settings are defined at registration and allow you to define the selection or setting dependencies\n\n\n```python\nclass Client\n    def __init__(self, number=10)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\ncontainer = Container()\n\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2)\n\ncontainer.register(\n    Client,\n    name="SetsValue",\n    dependency_config={"number": DependencySettings(value=50)}\n)\ncontainer.register(\n    Client,\n    name="UsesDefaultValue"\n)\ncontainer.register(\n    Client,\n    name="IgnoresDefaultParameterValue",\n    dependency_config={"number": DependencySettings(use_default_paramater=False)}\n)\ncontainer.register(\n    Client,\n    name="UsesRegistrationFilter",\n    dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}\n)\n\nclient1 = container.resolve(Client, filter=with_name("SetsValue"))\nclient2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))\nclient3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))\nclient4 = container.resolve(Client, filter=with_name("UsesRegistrationFilter"))\n\n\nclient1.get_number() # returns 50\nclient2.get_number() # returns 10\nclient3.get_number() # returns 2\nclient4.get_number() # returns 1\n```\n\nThe order of a dependant value is as follows\n1. Setting the dependency value explicitly\n    ```python\n    DependencySettings(value=50)\n    ```\n2. Using the default parameter value if it exisis the dependency value explicitly\n    ```python\n    class Client\n    def __init__(self, number=10)\n        self.number = number\n    ```\n    If you don\'t want to use the default parameter value you can set it to false in the dependency setting\n    ```python\n    DependencySettings(use_default_paramater=False)\n    ```\n3. Going to the container registry to find a registration using the registration filter if, if there is a default value on the dependant paramater you must explicity set.\n\n\n## Tags\n\nTags can be added to registrations in order to support filtering. This can be useful as a means to filter registrations when resolving lists of a particular type\n\n```python\nclass A:\n    pass\n\na1 = A()\na2 = A()\na3 = A()\n\ncontainer = Container()\n\ncontainer.register(A, instance=a1, tags=[Tag("a", "a1")])\ncontainer.register(A, instance=a2, tags=[Tag("a")])\ncontainer.register(A, instance=a3)\n\nar1 = container.resolve(A, filter=has_tag("a", "a1")) # returns a1\nal1 = container.resolve(list[A], filter=has_tag("a"))  # returns [a2, a1]\nal2 = container.resolve(list[A], filter=has_tag("a", "a1")) # returns [a1]\nal3 = container.resolve(list[A], filter=fn_not(has_tag("a", "a1")))  # returns [a3, a2]\nal4 = container.resolve(list[A], filter=fn_not(has_tag("a"))) # returns [a3]\nal5 = container.resolve(list[A]) # returns [a3, a2, a1]\n```\n## Accessing the Container, Scope and Resolver within dependencies\n\nAccessing container directly\n\n```python\nclass Client\n    def __init__(self, container: Container)\n        self.container = container\n\n    def get_number(self):\n        return self.container.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nAccessing Resolver also returns the container\n\n```python\n\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nWhen within a scope, Resolver returns the current scope rather than the container\n\n```python\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n\n## Modules\n\n\nA module is a just a function that accepts a container, it can be used to set up common elements on the container\n\n```python\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_module(c: Container):\n    c.register(ClientDependency)\n    c.register(Client)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n```\n\n\n\n## DependencyContext (BETA feature)\n\nYou can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing\nOne example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context\n\n```python\nclass Logger\n    def __init__(self, module):\n        self.module = module\n\nclass Client\n    def __init__(self, logger: Logger)\n        self.logger = logger\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return Logger(module)\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(Logger, factory=logger_fac)\n\nclient = container.resolve(Client)\n\n\n```\n\n\n## Pre-configurations\n\nPre configurations run a side-effect for a type before the type gets resolved.\nThis is useful if some python modules have some sort of module level functions that need to be called before the object get created\n\n```python\nimport logging\n\nclass Client\n    def __init__(self, logger: logging.Logger)\n        self.logger = logger\n\n    def do_a_thing(self):\n        self.logger.info(\'Doing a thing\')\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return logging.getLogger(module)\n\ndef configuring_logging():\n    logging.basicConfig()\n\n\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(logging.Logger, factory=logger_fac)\ncontainer.pre_configure(logging.Logger, configuring_logging)\n\nclient = container.resolve(Client)\n\n\n```',
+    'long_description': '# Clean IoC\nA simple dependency injection library for python that requires nothing of your application code (except that you use typing).\n\n\n## Basic Registering and resolving\n\nThere are 4 basic modes of registering a new set of classes\n\n### Implementation\n\n```python\n\nclass UserRepository(abc.ABC)\n    @abc.abstractmethod\n    def add(self, user):\n        pass\n\nclass InMemoryUserRepository(UserRepository)\n\n    def __init__(self):\n        self.users = []\n\n    def add(self, user):\n        # This is obviously terrible, but it\'s for demo purposes\n        self.users.append(user)\n\nclass SqlAlchemyUserRepository(UserRepository)\n\n    def __init__(self):\n        # Do some db stuff here\n        pass\n\n    def add(self, user):\n        # Do some db stuff here\n        pass\n\ncontainer = Container()\ncontainer.register(UserRepository, InMemoryUserRepository)\n\n\nrepository = container.resolve(UserRepository) # This will return an InMemoryUserRepository\n\n```\n\n### Concrete Class\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n### Factory\n\n```python\n\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_factory(dep: ClientDependency):\n    return Client(dep=dep)\n\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client, factory=client_factory)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n\n### Instance\n\n```python\n\nclass ClientDependency\n    def __init__(self, num):\n        self.num = num\n\n    def get_int(self):\n        return self.num\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\nclient_dependency = ClientDependency(num=10)\n\ncontainer = Container()\ncontainer.register(ClientDependency, instance=client_dependency)\ncontainer.register(Client)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n\n```\n\n## List resolving\n\nIf you have multiple dependencues you can simply define a dependency as a list[T] and you can return all of the instances.\n\n```python\n\nclass ClientDependency\n    def __init__(self, numbers: list[int]):\n        self.numbers = numbers\n\n    def get_numbers(self):\n        return self.numbers\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_numbers(self):\n        return self.dep.get_numbers()\n\ncontainer = Container()\ncontainer.register(ClientDependency)\ncontainer.register(Client)\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nclient = container.resolve(Client)\n\nclient.get_numbers() # returns [3, 2, 1]\n```\n\n\n## Decorators\n\nFollows a object orientated decoration pattern, rather than a decoration annotation.\nThe main reason for this was to allow decotation of registered instances\n\n```python\nclass Client\n    def __init__(self, number: int)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\n\nclass DoubleClientDecorator(Client):\n    def __init__(self, client: Client):\n        self.client = client\n    def get_number(self):\n        return self.client.get_number() * 2\n\ncontainer = Container()\n\ncontainer.register(Client)\ncontainer.register_decorator(Client, DoubleClientDecorator)\ncontainer.register(int, instance=10)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 20\n```\n\n\nDecorators are resolved in order of when first registered. So the first registered decorator is the highest in the class tree\n\n\n```python\n    class Concrete:\n        pass\n\n    class DecoratorOne(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    class DecoratorTwo(Concrete):\n        def __init__(self, child: Concrete):\n            self.child = child\n\n    container = Container()\n\n    container.register(Concrete)\n    container.register_decorator(Concrete, DecoratorOne)\n    container.register_decorator(Concrete, DecoratorTwo)\n\n    root = container.resolve(Concrete)\n\n    type(root) # returns DecoratorOne\n    type(root.child) # returns DecoratorTwo\n    type(root.child.child) # returns Concrete\n```\n\n\n## Subclasses registration\n\nThis feature allows registration of all subclasses of a giveb type\n\n```python\nclass Client(abc.ABC)\n    @abc.abstractmethod\n    def get_number(self):\n        pass\n\n\nclass TenClient(Client)\n    def get_number(self):\n        return 10\n\nclass TwentyClient(Client)\n    def get_number(self):\n        return 20\n\ncontainer = Container()\n\ncontainer.register_subclasses(Client)\n\nten_client = container.resolve(TenClient)\nten_client.get_number() # returns 10\n\ntwenty_client = container.resolve(TwentyClient)\ntwenty_client.get_number() # returns 20\n\n# Resolve all subsclasses of Client\nclient = container.resolve(list[Client]) ## [TwentyClient(), TenClient()]\n```\n\n\n## Lifespans\nLifespans configure how long and resolved object says alive for\nThere are 4 lifespan types\n\n### transient\nAlways create a new instance\n\n```python\ncontainer.register(Client, lifespan=Lifespan.transient)\n```\n\n\n### once_per_graph (Default behaviour)\nOnly create one instance throughout the resolve call\n\n```python\ncontainer.register(Client, lifespan=Lifespan.once_per_graph)\n```\n\n### scoped\nOnly create a new instance through the life a scope. When not in a scope the behaviour is the same as **once_per_graph**\n\n```python\ncontainer.register(Client, lifespan=Lifespan.scoped)\n```\n\n### singleton\nOnly one instance of the object is created throughout the lifespan of the container\n\n```python\ncontainer.register(Client, lifespan=Lifespan.singleton)\n```\n\n*Note:*\nWhen registering an instance, then the behaviour is always singleton\n\n```python\ncontainer.register(int, instance=10)\n```\n\n## Open Generics\n\nRegisters all generic subclasses of the service type and allows you to resolve with the generic alias\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\n\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'HELLO\'\nh2.handle(GoodbyeCommand()) # prints \'GOODBYE\'\n\n```\n\n## Open Generic Decorators\n\n\nAllows you to add decorators to your open generic registrations\n\n```python\nT = TypeVar("T")\n\nclass HelloCommand:\n    pass\n\nclass GoodbyeCommand:\n    pass\n\nclass CommandHandler(Generic[T]):\n    def handle(self, command: T):\n        pass\n\nclass HelloCommandHandler(CommandHandler[HelloCommand]):\n    def handle(self, command: HelloCommand):\n        print(\'HELLO\')\n\nclass GoodbyeCommandHandler(CommandHandler[GoodbyeCommand]):\n    def handle(self, command: GoodbyeCommand):\n        print(\'GOODBYE\')\n\nclass AVeryBigCommandHandlerDecorator(Generic[T]):\n    def __init__(self, handler: CommandHandler[T]):\n        self.handler = handler\n\n    def handle(self, command: T):\n        print(\'A VERY BIG\')\n        self.handler.handle(command=command)\n\ncontainer = Container()\ncontainer.register_open_generic(CommandHandler)\ncontainer.register_open_generic_decorator(CommandHandler, AVeryBigCommandHandlerDecorator)\nh1 = container.resolve(CommandHandler[HelloCommand])\nh2 = container.resolve(CommandHandler[GoodbyeCommand])\n\nh1.handle(HelloCommand()) # prints \'A VERY BIG\\nHELLO\'\nh2.handle(GoodbyeCommand()) # prints \'A VERY BIG\\nGOODBYE\'\n\n```\n\n## Scopes\n\nScopes are a way to create a sub container that will live for a certain lifespan.\nSome good use cases for scope would be for the lifespan of handling a http request with a web server or a message/event if working on a message based system\n\n\n```python\nclass Client\n    def __init__(self, number: int)\n        return number\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\n## Named registrations & Registration filters\n\nBy default the last unnamed registration is what the container will return when resolve is called as below.\n\n```python\n\ncontainer = Container()\ncontainer.register(int, instance=1)\ncontainer.register(int, instance=2)\ncontainer.register(int, instance=3)\n\nnumber = container.resolve(int) # returns 3\n\n```\nTo be more selective of what we return we can add a name to the registration and apply a registration filter when we resolve.\n\nA registration filter is simply function that receives a **Registration** and returns a **bool**\n\nFor example if we wanted to get the int named **"One"** we do the following\n\n```python\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=lambda r: r.name == "One") # returns 1\n```\n\nClean IOC comes with a set of in built registration filters that can be found [here](./clean_ioc/registration_filters.py)\n\nWe can get the desired behaviour as above\n```python\nfrom clean_ioc.registration_filters import with_name\n\ncontainer = Container()\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2, name="Two")\ncontainer.register(int, instance=3, name="Three")\n\nnumber = container.resolve(int, filter=with_name("One")) # returns 1\n```\n\n## Dependency Settings\n\nDependency settings are defined at registration and allow you to define the selection or setting dependencies\n\n\n```python\nclass Client\n    def __init__(self, number=10)\n        self.number = number\n\n    def get_number(self):\n        return self.number\n\ncontainer = Container()\n\ncontainer.register(int, instance=1, name="One")\ncontainer.register(int, instance=2)\n\ncontainer.register(\n    Client,\n    name="SetsValue",\n    dependency_config={"number": DependencySettings(value=50)}\n)\ncontainer.register(\n    Client,\n    name="UsesDefaultValue"\n)\ncontainer.register(\n    Client,\n    name="IgnoresDefaultParameterValue",\n    dependency_config={"number": DependencySettings(use_default_paramater=False)}\n)\ncontainer.register(\n    Client,\n    name="UsesRegistrationFilter",\n    dependency_config={"number": DependencySettings(use_default_paramater=False, filter=with_name("One"))}\n)\n\nclient1 = container.resolve(Client, filter=with_name("SetsValue"))\nclient2 = container.resolve(Client, filter=with_name("UsesDefaultValue"))\nclient3 = container.resolve(Client, filter=with_name("IgnoresDefaultParameterValue"))\nclient4 = container.resolve(Client, filter=with_name("UsesRegistrationFilter"))\n\n\nclient1.get_number() # returns 50\nclient2.get_number() # returns 10\nclient3.get_number() # returns 2\nclient4.get_number() # returns 1\n```\n\nThe order of a dependant value is as follows\n1. Setting the dependency value explicitly\n    ```python\n    DependencySettings(value=50)\n    ```\n2. Using the default parameter value if it exisis the dependency value explicitly\n    ```python\n    class Client\n    def __init__(self, number=10)\n        self.number = number\n    ```\n    If you don\'t want to use the default parameter value you can set it to false in the dependency setting\n    ```python\n    DependencySettings(use_default_paramater=False)\n    ```\n3. Going to the container registry to find a registration using the registration filter if, if there is a default value on the dependant paramater you must explicity set.\n\n\n## Tags\n\nTags can be added to registrations in order to support filtering. This can be useful as a means to filter registrations when resolving lists of a particular type\n\n```python\nclass A:\n    pass\n\na1 = A()\na2 = A()\na3 = A()\n\ncontainer = Container()\n\ncontainer.register(A, instance=a1, tags=[Tag("a", "a1")])\ncontainer.register(A, instance=a2, tags=[Tag("a")])\ncontainer.register(A, instance=a3)\n\nar1 = container.resolve(A, filter=has_tag("a", "a1")) # returns a1\nal1 = container.resolve(list[A], filter=has_tag("a"))  # returns [a2, a1]\nal2 = container.resolve(list[A], filter=has_tag("a", "a1")) # returns [a1]\nal3 = container.resolve(list[A], filter=fn_not(has_tag("a", "a1")))  # returns [a3, a2]\nal4 = container.resolve(list[A], filter=fn_not(has_tag("a"))) # returns [a3]\nal5 = container.resolve(list[A]) # returns [a3, a2, a1]\n```\n\n\n\n## Parent Context Filters\n\nRegistrations can also specify that should only apply to certain parents objects by setting the parent_context_filter\n\n```python\ndef test_parent_context_filter():\n    class A:\n        pass\n\n    class B(A):\n        pass\n\n    class C(A):\n        pass\n\n    class D:\n        def __init__(self, a: A):\n            self.a = a\n\n    class E:\n        def __init__(self, a: A):\n            self.a = a\n\n    container = Container()\n\n    container.register(A, B, parent_context_filter=parent_implementation_is(E))\n    container.register(A, C, parent_context_filter=parent_implementation_is(D))\n    container.register(D)\n    container.register(E)\n\n    e = container.resolve(E)\n    d = container.resolve(D)\n\n    type(e.a) # returns B\n    type(d.a) # returns C\n\n```\n\n\n\n## Accessing the Container, Scope and Resolver within dependencies\n\nAccessing container directly\n\n```python\nclass Client\n    def __init__(self, container: Container)\n        self.container = container\n\n    def get_number(self):\n        return self.container.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nAccessing Resolver also returns the container\n\n```python\n\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n```\n\nWhen within a scope, Resolver returns the current scope rather than the container\n\n```python\nclass Client\n    def __init__(self, resolver: Resolver)\n        self.resolver = resolver\n\n    def get_number(self):\n        return self.resolver.resolve(int)\n\ncontainer.register(int, instance=2)\n\ncontainer.register(Client)\n\nclient = container.resolve(Client)\nclient.get_number() # returns 2\n\nwith container.get_scope() as scope:\n    scope.register(int, instance=10)\n    scoped_client = scope.resolve(Client)\n    scoped_client.get_number() # returns 10\n```\n\nScopes can also be used as an async context manager\n\n```python\nclass Client\n    async def get_number(self):\n        return 10\n\ncontainer.register(Client)\n\nasync with container.get_scope() as scope:\n    scoped_client = scope.resolve(Client)\n    await scoped_client.get_number() # returns 10\n```\n\n## Modules\n\n\nA module is a just a function that accepts a container, it can be used to set up common elements on the container\n\n```python\nclass ClientDependency\n    def get_int(self):\n        return 10\n\nclass Client\n    def __init__(self, dep: ClientDependency)\n        self.dep = dep\n\n    def get_number(self):\n        return self.dep.get_int()\n\ndef client_module(c: Container):\n    c.register(ClientDependency)\n    c.register(Client)\n\ncontainer.apply_module(client_module)\n\nclient = container.resolve(Client)\n\nclient.get_number() # returns 10\n```\n\n\n## DependencyContext (BETA feature)\n\nYou can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing\nOne example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context\n\n```python\nclass Logger\n    def __init__(self, module):\n        self.module = module\n\nclass Client\n    def __init__(self, logger: Logger)\n        self.logger = logger\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return Logger(module)\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(Logger, factory=logger_fac)\n\nclient = container.resolve(Client)\n\n\n```\n\n\n## Pre-configurations\n\nPre configurations run a side-effect for a type before the type gets resolved.\nThis is useful if some python modules have some sort of module level functions that need to be called before the object get created\n\n```python\nimport logging\n\nclass Client\n    def __init__(self, logger: logging.Logger)\n        self.logger = logger\n\n    def do_a_thing(self):\n        self.logger.info(\'Doing a thing\')\n\ndef logger_fac(context: DependencyContext):\n    module = context.parent.implementation.__module__\n    return logging.getLogger(module)\n\ndef configuring_logging():\n    logging.basicConfig()\n\n\n\n\ncontainer = Container()\ncontainer.register(Client)\ncontainer.register(logging.Logger, factory=logger_fac)\ncontainer.pre_configure(logging.Logger, configuring_logging)\n\nclient = container.resolve(Client)\n\n\n```',
     'author': 'Peter Daly',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/peter-daly/clean_ioc',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `clean_ioc-0.2.1/PKG-INFO` & `clean_ioc-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean-ioc
-Version: 0.2.1
+Version: 0.3.0
 Summary: An IOC Container for Python 3.10+
 Home-page: https://github.com/peter-daly/clean_ioc
 License: MIT
 Author: Peter Daly
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -143,14 +143,16 @@
 
 client.get_number() # returns 10
 
 ```
 
 ## List resolving
 
+If you have multiple dependencues you can simply define a dependency as a list[T] and you can return all of the instances.
+
 ```python
 
 class ClientDependency
     def __init__(self, numbers: list[int]):
         self.numbers = numbers
 
     def get_numbers(self):
@@ -551,14 +553,57 @@
 ar1 = container.resolve(A, filter=has_tag("a", "a1")) # returns a1
 al1 = container.resolve(list[A], filter=has_tag("a"))  # returns [a2, a1]
 al2 = container.resolve(list[A], filter=has_tag("a", "a1")) # returns [a1]
 al3 = container.resolve(list[A], filter=fn_not(has_tag("a", "a1")))  # returns [a3, a2]
 al4 = container.resolve(list[A], filter=fn_not(has_tag("a"))) # returns [a3]
 al5 = container.resolve(list[A]) # returns [a3, a2, a1]
 ```
+
+
+
+## Parent Context Filters
+
+Registrations can also specify that should only apply to certain parents objects by setting the parent_context_filter
+
+```python
+def test_parent_context_filter():
+    class A:
+        pass
+
+    class B(A):
+        pass
+
+    class C(A):
+        pass
+
+    class D:
+        def __init__(self, a: A):
+            self.a = a
+
+    class E:
+        def __init__(self, a: A):
+            self.a = a
+
+    container = Container()
+
+    container.register(A, B, parent_context_filter=parent_implementation_is(E))
+    container.register(A, C, parent_context_filter=parent_implementation_is(D))
+    container.register(D)
+    container.register(E)
+
+    e = container.resolve(E)
+    d = container.resolve(D)
+
+    type(e.a) # returns B
+    type(d.a) # returns C
+
+```
+
+
+
 ## Accessing the Container, Scope and Resolver within dependencies
 
 Accessing container directly
 
 ```python
 class Client
     def __init__(self, container: Container)
@@ -613,14 +658,27 @@
 
 with container.get_scope() as scope:
     scope.register(int, instance=10)
     scoped_client = scope.resolve(Client)
     scoped_client.get_number() # returns 10
 ```
 
+Scopes can also be used as an async context manager
+
+```python
+class Client
+    async def get_number(self):
+        return 10
+
+container.register(Client)
+
+async with container.get_scope() as scope:
+    scoped_client = scope.resolve(Client)
+    await scoped_client.get_number() # returns 10
+```
 
 ## Modules
 
 
 A module is a just a function that accepts a container, it can be used to set up common elements on the container
 
 ```python
@@ -643,15 +701,14 @@
 
 client = container.resolve(Client)
 
 client.get_number() # returns 10
 ```
 
 
-
 ## DependencyContext (BETA feature)
 
 You can inject a special type into your dependants that allows you to inspect the current dependency tree. For instances you can check the parent of the current class you are constructing
 One example of where this becomes useful is if injecting a logger, you can get information about the loggers parent to add extra context
 
 ```python
 class Logger
```

