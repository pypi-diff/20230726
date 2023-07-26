# Comparing `tmp/svcs-23.4.0.tar.gz` & `tmp/svcs-23.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jul 24 16:58:40 2023, max compression
+gzip compressed data, last modified: Wed Jul 26 13:05:49 2023, max compression
```

## Comparing `svcs-23.4.0.tar` & `svcs-23.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      125 2023-07-24 16:58:40.000000 svcs-23.4.0/.git_archival.txt
--rw-r--r--   0        0        0      131 2023-07-24 16:58:40.000000 svcs-23.4.0/.gitattributes
--rw-r--r--   0        0        0      472 2023-07-24 16:58:40.000000 svcs-23.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2023-07-24 16:58:40.000000 svcs-23.4.0/.python-version-default
--rw-r--r--   0        0        0     2349 2023-07-24 16:58:40.000000 svcs-23.4.0/CHANGELOG.md
--rw-r--r--   0        0        0    13703 2023-07-24 16:58:40.000000 svcs-23.4.0/README.md
--rw-r--r--   0        0        0      591 2023-07-24 16:58:40.000000 svcs-23.4.0/conftest.py
--rw-r--r--   0        0        0      840 2023-07-24 16:58:40.000000 svcs-23.4.0/tox.ini
--rw-r--r--   0        0        0     5482 2023-07-24 16:58:40.000000 svcs-23.4.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      285 2023-07-24 16:58:40.000000 svcs-23.4.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       18 2023-07-24 16:58:40.000000 svcs-23.4.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      865 2023-07-24 16:58:40.000000 svcs-23.4.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2023-07-24 16:58:40.000000 svcs-23.4.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4136 2023-07-24 16:58:40.000000 svcs-23.4.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      749 2023-07-24 16:58:40.000000 svcs-23.4.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1642 2023-07-24 16:58:40.000000 svcs-23.4.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0     1094 2023-07-24 16:58:40.000000 svcs-23.4.0/docs/_static/logo.svg
--rw-r--r--   0        0        0      476 2023-07-24 16:58:40.000000 svcs-23.4.0/src/svcs/__init__.py
--rw-r--r--   0        0        0     6879 2023-07-24 16:58:40.000000 svcs-23.4.0/src/svcs/_core.py
--rw-r--r--   0        0        0      234 2023-07-24 16:58:40.000000 svcs-23.4.0/src/svcs/exceptions.py
--rw-r--r--   0        0        0     2365 2023-07-24 16:58:40.000000 svcs-23.4.0/src/svcs/flask.py
--rw-r--r--   0        0        0        0 2023-07-24 16:58:40.000000 svcs-23.4.0/src/svcs/py.typed
--rw-r--r--   0        0        0       91 2023-07-24 16:58:40.000000 svcs-23.4.0/tests/__init__.py
--rw-r--r--   0        0        0     4324 2023-07-24 16:58:40.000000 svcs-23.4.0/tests/test_async.py
--rw-r--r--   0        0        0     6987 2023-07-24 16:58:40.000000 svcs-23.4.0/tests/test_core.py
--rw-r--r--   0        0        0     5899 2023-07-24 16:58:40.000000 svcs-23.4.0/tests/test_flask.py
--rw-r--r--   0        0        0     1135 2023-07-24 16:58:40.000000 svcs-23.4.0/tests/typing/core.py
--rw-r--r--   0        0        0      903 2023-07-24 16:58:40.000000 svcs-23.4.0/tests/typing/flask_.py
--rw-r--r--   0        0        0      108 2023-07-24 16:58:40.000000 svcs-23.4.0/.gitignore
--rw-r--r--   0        0        0     1072 2023-07-24 16:58:40.000000 svcs-23.4.0/LICENSE
--rw-r--r--   0        0        0     4182 2023-07-24 16:58:40.000000 svcs-23.4.0/pyproject.toml
--rw-r--r--   0        0        0     5328 2023-07-24 16:58:40.000000 svcs-23.4.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-07-26 13:05:49.000000 svcs-23.5.0/.git_archival.txt
+-rw-r--r--   0        0        0      131 2023-07-26 13:05:49.000000 svcs-23.5.0/.gitattributes
+-rw-r--r--   0        0        0      596 2023-07-26 13:05:49.000000 svcs-23.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-07-26 13:05:49.000000 svcs-23.5.0/.python-version-default
+-rw-r--r--   0        0        0     2609 2023-07-26 13:05:49.000000 svcs-23.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    15836 2023-07-26 13:05:49.000000 svcs-23.5.0/README.md
+-rw-r--r--   0        0        0      841 2023-07-26 13:05:49.000000 svcs-23.5.0/conftest.py
+-rw-r--r--   0        0        0      840 2023-07-26 13:05:49.000000 svcs-23.5.0/tox.ini
+-rw-r--r--   0        0        0     5482 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      285 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       18 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      865 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     4136 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      749 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1642 2023-07-26 13:05:49.000000 svcs-23.5.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0     1094 2023-07-26 13:05:49.000000 svcs-23.5.0/docs/_static/logo.svg
+-rw-r--r--   0        0        0      476 2023-07-26 13:05:49.000000 svcs-23.5.0/src/svcs/__init__.py
+-rw-r--r--   0        0        0     9492 2023-07-26 13:05:49.000000 svcs-23.5.0/src/svcs/_core.py
+-rw-r--r--   0        0        0      234 2023-07-26 13:05:49.000000 svcs-23.5.0/src/svcs/exceptions.py
+-rw-r--r--   0        0        0     3458 2023-07-26 13:05:49.000000 svcs-23.5.0/src/svcs/flask.py
+-rw-r--r--   0        0        0        0 2023-07-26 13:05:49.000000 svcs-23.5.0/src/svcs/py.typed
+-rw-r--r--   0        0        0       91 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     4555 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/test_async.py
+-rw-r--r--   0        0        0    10959 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/test_core.py
+-rw-r--r--   0        0        0     6426 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/test_flask.py
+-rw-r--r--   0        0        0     1366 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/typing/core.py
+-rw-r--r--   0        0        0      935 2023-07-26 13:05:49.000000 svcs-23.5.0/tests/typing/flask_.py
+-rw-r--r--   0        0        0      112 2023-07-26 13:05:49.000000 svcs-23.5.0/.gitignore
+-rw-r--r--   0        0        0     1072 2023-07-26 13:05:49.000000 svcs-23.5.0/LICENSE
+-rw-r--r--   0        0        0     4274 2023-07-26 13:05:49.000000 svcs-23.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6743 2023-07-26 13:05:49.000000 svcs-23.5.0/PKG-INFO
```

### Comparing `svcs-23.4.0/CHANGELOG.md` & `svcs-23.5.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,27 @@
 The **third number** is for emergencies when we need to start branches for older releases.
 
 You can find our backwards-compatibility policy [here](https://github.com/hynek/svcs/blob/main/.github/SECURITY.md).
 
 <!-- changelog follows -->
 
 
+## [23.5.0](https://github.com/hynek/svcs/compare/23.4.0...23.5.0) - 2023-07-26
+
+### Added
+
+- Registered factory/value clean up!
+  It is now possible to register an `on_registry_close` hook that is called once the `Registry`'s `(a)close()` method is called.
+
+
 ## [23.4.0](https://github.com/hynek/svcs/compare/23.3.0...23.4.0) - 2023-07-24
 
 ### Changed
 
-- Renamed from *reg-svc* to *svcs*.
+- Renamed from *svc-reg* to *svcs*.
   Sadly the more obvious names are all taken.
 
 
 ## [23.3.0](https://github.com/hynek/svcs/compare/23.2.0...23.3.0) - 2023-07-20
 
 ### Added
```

### Comparing `svcs-23.4.0/README.md` & `svcs-23.5.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 <!-- begin-pypi -->
 
 
 <p align="center">
   <a href="https://github.com/hynek/svcs/">
-    <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo.svg" width="25%" alt="svcs" />
+    <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo.svg" width="20%" alt="svcs" />
   </a>
 </p>
 
 
-# *svcs*: A Service Locator for Python
+# *svcs*: A Lightweight Service Locator for Python
 
 > **Warning**
 > ☠️ Not ready yet! ☠️
 >
 > This project is only public to [gather feedback](https://github.com/hynek/svcs/discussions), and everything can and will change until the project is proclaimed stable.
 >
 > Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
 >
 > At this point, it's unclear whether this project will become a "proper Hynek project".
 > I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
 
 *svcs* (pronounced *services*) is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python.
 It provides you with a central place to register factories for types/interfaces and then imperatively request instances of those types with **automatic cleanup** and **health checks**.
 
-**This allows you to configure and manage resources in *one central place* and access them all in a *consistent* way.**
+---
+
+**This allows you to configure and manage all your resources in *one central place* and access them in a *consistent* way.**
 
 ---
 
 In practice that means that at runtime, you say "*Give me a database connection*!", and *svcs* will give you whatever you've configured it to return when asked for a database connection.
 This can be an actual database connection or it can be a mock object for testing.
+All of this happens *within* your application – service locators are **not** related to service discovery.
 
 If you like the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [Abstract Base Class](https://docs.python.org/3.11/library/abc.html).
 
 That:
 
 - unifies **acquisition** and **cleanups** of resources,
 - simplifies **testing**,
@@ -56,35 +59,73 @@
     api = services.get(WebAPIClient)
 ```
 
 The latter already works with [Flask](#flask).
 
 You set it up like this:
 
+<!--
+; skip: next
+-->
+
 ```python
+import atexit
+
 from sqlalchemy import Connection, create_engine
 
 ...
 
 engine = create_engine("postgresql://localhost")
 
 def engine_factory():
     with engine.connect() as conn:
         yield conn
 
 registry = svcs.Registry()
-registry.register_factory(Connection, engine_factory)
+registry.register_factory(
+    Connection, engine_factory, on_registry_close=engine.dispose
+)
+
+@atexit.register
+def cleanup():
+    registry.close()  # calls engine.dispose()
 ```
 
 The generator-based setup and cleanup may remind you of [Pytest fixtures](https://docs.pytest.org/en/stable/explanation/fixtures.html).
-
-Unlike typical dependency injection that passes your dependencies as arguments, the active obtainment of resources by calling `get()` when you *know* you're going to need it avoids the conundrum of either having to pass a factory (e.g., a connection pool -- which also puts the onus of cleanup on you), or eagerly creating resources that are never used.
+The hooks that are defined as `on_registry_close` are called when you call `Registry.close()` – e.g. when your application is shutting down.
 
 *svcs* comes with **full async** support via a-prefixed methods (i.e. `aget()` instead of `get()`, et cetera).
 
+
+## Is this Dependency Injection!?
+
+No.
+
+Unlike [dependency injection](https://en.wikipedia.org/wiki/Dependency_injection), which passes your dependencies as arguments, you actively ask a service locator for them. This usually requires less opaque magic since nothing meddles with your function/method definitions. But you can use, e.g., your web framework's injection capabilities to inject the locator object into your views and benefit from *svcs*'s upsides without giving up some of DI's ones.
+
+The active acquisition of resources by calling `get()` when you *know* for sure you're going to need it avoids the conundrum of either having to pass a factory (e.g., a connection pool – which also puts the onus of cleanup on you) or eagerly creating resources that you never use:
+
+<!--
+; skip: next
+-->
+```python
+def view(request):
+    if request.form.valid():
+        # Form is valid; only NOW get a DB connection
+        # and pass it into your business logic.
+        return handle_form_data(
+            request.services.get(Database),
+            form.data,
+        )
+
+    raise InvalidFormError()
+```
+
+The main downside is that it's impossible to verify whether all required dependencies have been configured without running the code.
+
 <!-- end-pypi -->
 
 
 ## Low-Level Core API
 
 You're unlikely to use the core API directly, but knowing what's happening underneath is good to dispel any concerns about magic.
 
@@ -103,20 +144,35 @@
 >>> import svcs
 >>> import uuid
 
 >>> reg = svcs.Registry()
 
 >>> reg.register_factory(uuid.UUID, uuid.uuid4)
 >>> reg.register_value(str, "Hello World")
-
 ```
 
 The values and return values of the factories don't have to be actual instances of the type they're registered for.
 But the types must be *hashable* because they're used as keys in a lookup dictionary.
 
+It's possible to register a callback that is called when the *registry* is closed:
+
+<!--
+; skip: next
+-->
+
+```python
+registry.register_factory(
+    Connection, engine_factory, on_registry_close=engine.dispose
+)
+```
+
+If this callback fails, it's logged at warning level but otherwise ignored.
+For instance, you could free a database connection pool in an [`atexit` handler](https://docs.python.org/3/library/atexit.html).
+This frees you from keeping track of registered resources yourself.
+
 
 ### Containers
 
 A **`Container`** belongs to a Registry and allows to create instances of the registered types, taking care of their life-cycle:
 
 ```python
 >>> container = svcs.Container(reg)
@@ -126,20 +182,19 @@
 UUID('...')
 >>> # Calling get() again returns the SAME UUID instance!
 >>> # Good for DB connections, bad for UUIDs.
 >>> u is container.get(uuid.UUID)
 True
 >>> container.get(str)
 'Hello World'
-
 ```
 
-A container lives as long as you want the instances to live -- e.g., as long as a request lives.
+A container lives as long as you want the instances to live – e.g., as long as a request lives.
 
-Importantly: It is possible to overwrite registered service factories later -- e.g., for testing -- **without monkey-patching**.
+Importantly: It is possible to overwrite registered service factories later – e.g., for testing – **without monkey-patching**.
 You have to remove possibly cached instances from the container though (`Container.forget_service_type()`).
 The Flask integration takes care of this for you.
 
 How to achieve this in other frameworks elegantly is TBD.
 
 
 #### Cleanup
@@ -155,15 +210,15 @@
 **The key idea is that your business code doesn't have to care about cleaning up resources it has requested.**
 
 That makes it even easier to test it because the business codes makes fewer assumptions about the object it's getting.
 
 
 #### Health Checks
 
-Additionally, each registered service may have a `ping` callable that you can use for health checks.
+Each registered service may have a `ping` callable that you can use for health checks.
 You can request all pingable registered services with `container.get_pings()`.
 This returns a list of `ServicePing` objects that currently have a name property to identify the ping and a `ping` method that instantiates the service, adds it to the cleanup list, and runs the ping.
 If you have async resources (either factory or ping callable), you can use `aping()` instead.
 `aping()` works with sync resources too, so you can use it universally in async code.
 You can look at the `is_async` property to check whether you *need* to use `aget()`, though.
 
 
@@ -181,25 +236,32 @@
 ## Flask
 
 *svcs* has grown from my frustration with the repetitiveness of using the `get_x` that creates an `x` and then stores it on the `g` object [pattern](https://flask.palletsprojects.com/en/latest/appcontext/#storing-data).
 
 Therefore it comes with Flask support out of the box in the form of the `svcs.flask` module.
 It:
 
-- puts the registry into `app.config["svcsistry"]`,
-- unifies the putting and caching of services on the `g` object by putting a container into `g.svc_container`,
+- puts the registry into `app.config["svcs_registry"]`,
+- unifies the putting and caching of services on the `g` object by putting a container into `g.svcs_container`,
 - transparently retrieves them from there for you,
 - and installs a [`teardown_appcontext()`](http://flask.pocoo.org/docs/latest/api#flask.Flask.teardown_appcontext) handler that calls `close()` on the container when a request is done.
 
 ---
 
 You can add support for *svcs* by calling `svcs.flask.init_app(app)` in your [*application factory*](https://flask.palletsprojects.com/en/latest/patterns/appfactories/).
 For instance, to create a factory that uses a SQLAlchemy engine to produce connections, you could do this:
 
+
+<!--
+; skip: start
+-->
+
 ```python
+import atexit
+
 from flask import Flask
 from sqlalchemy import Connection, create_engine
 from sqlalchemy.sql import text
 
 import svcs
 
 
@@ -224,26 +286,36 @@
 
     ping = text("SELECT 1")
     svcs_flask.register_factory(
         # The app argument makes it good for custom init_app() functions.
         app,
         Connection,
         engine_factory,
-        ping=lambda conn: conn.execute(ping)
+        ping=lambda conn: conn.execute(ping),
+        on_registry_close=engine.dispose,
     )
 
     # You also use svcs WITHIN factories:
     svcs_flask.register_factory(
         app, # <---
         AbstractRepository,
         # No cleanup, so we just return an object using a lambda
         lambda: Repository.from_connection(
             svcs.flask.get(Connection)
         ),
     )
+
+    @atexit.register
+    def cleanup() -> None:
+        """
+        Clean up all pools when the application shuts down.
+        """
+        log.info("app.cleanup.start")
+        svcs.flask.close_registry(app)
+        log.info("app.cleanup.done")
     ##########################################################################
 
     ...
 
     return app
 ```
```

### Comparing `svcs-23.4.0/conftest.py` & `svcs-23.5.0/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,37 @@
 # SPDX-License-Identifier: MIT
 
 from doctest import ELLIPSIS
 
 import pytest
 
 from sybil import Sybil
-from sybil.parsers.rest import DocTestParser, PythonCodeBlockParser
+from sybil.parsers import myst, rest
 
 import svcs
 
 
-pytest_collect_file = Sybil(
+markdown_examples = Sybil(
     parsers=[
-        DocTestParser(optionflags=ELLIPSIS),
-        PythonCodeBlockParser(),
+        myst.DocTestDirectiveParser(optionflags=ELLIPSIS),
+        myst.PythonCodeBlockParser(doctest_optionflags=ELLIPSIS),
+        myst.SkipParser(),
     ],
-    patterns=["*.md", "*.py"],
-).pytest()
+    patterns=["*.md"],
+)
+
+rest_examples = Sybil(
+    parsers=[
+        rest.DocTestParser(optionflags=ELLIPSIS),
+        rest.PythonCodeBlockParser(),
+    ],
+    patterns=["*.py"],
+)
+
+pytest_collect_file = (markdown_examples + rest_examples).pytest()
 
 
 @pytest.fixture(name="registry")
 def _registry():
     return svcs.Registry()
```

### Comparing `svcs-23.4.0/tox.ini` & `svcs-23.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `svcs-23.4.0/.github/CODE_OF_CONDUCT.md` & `svcs-23.5.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `svcs-23.4.0/.github/SECURITY.md` & `svcs-23.5.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `svcs-23.4.0/.github/workflows/ci.yml` & `svcs-23.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.4.0/.github/workflows/codeql-analysis.yml` & `svcs-23.5.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.4.0/.github/workflows/pypi-package.yml` & `svcs-23.5.0/.github/workflows/pypi-package.yml`

 * *Files identical despite different names*

### Comparing `svcs-23.4.0/docs/_static/logo.svg` & `svcs-23.5.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `svcs-23.4.0/src/svcs/_core.py` & `svcs-23.5.0/src/svcs/_core.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,162 +29,170 @@
 @attrs.define
 class Container:
     """
     A per-context container for instantiated services & cleanups.
     """
 
     registry: Registry
-    instantiated: dict[type, object] = attrs.Factory(dict)
-    cleanups: list[
+    _instantiated: dict[type, object] = attrs.Factory(dict)
+    _cleanups: list[
         tuple[RegisteredService, Generator | AsyncGenerator]
     ] = attrs.Factory(list)
 
     def __repr__(self) -> str:
         return (
-            f"<Container(instantiated={len(self.instantiated)}, "
-            f"cleanups={len(self.cleanups)})>"
+            f"<Container(instantiated={len(self._instantiated)}, "
+            f"cleanups={len(self._cleanups)})>"
         )
 
     def get(self, svc_type: type) -> Any:
         """
         Get an instance of *svc_type*.
 
         Instantiate it if necessary and register its cleanup.
 
         Returns:
              Any until https://github.com/python/mypy/issues/4717 is fixed.
         """
-        if (svc := self.instantiated.get(svc_type)) is not None:
+        if (svc := self._instantiated.get(svc_type)) is not None:
             return svc
 
         rs = self.registry.get_registered_service_for(svc_type)
         svc = rs.factory()
 
         if isinstance(svc, Generator):
-            self.cleanups.append((rs, svc))
+            self._cleanups.append((rs, svc))
             svc = next(svc)
 
-        self.instantiated[rs.svc_type] = svc
+        self._instantiated[rs.svc_type] = svc
 
         return svc
 
     async def aget(self, svc_type: type) -> Any:
         """
         Get an instance of *svc_type*.
 
         Instantiate it asynchronously if necessary and register its cleanup.
 
         Returns:
              Any until https://github.com/python/mypy/issues/4717 is fixed.
         """
-        if (svc := self.instantiated.get(svc_type)) is not None:
+        if (svc := self._instantiated.get(svc_type)) is not None:
             return svc
 
         rs = self.registry.get_registered_service_for(svc_type)
         svc = rs.factory()
 
         if isinstance(svc, AsyncGenerator):
-            self.cleanups.append((rs, svc))
+            self._cleanups.append((rs, svc))
             svc = await anext(svc)
         elif isawaitable(svc):
             svc = await svc
 
-        self.instantiated[rs.svc_type] = svc
+        self._instantiated[rs.svc_type] = svc
 
         return svc
 
     def forget_service_type(self, svc_type: type) -> None:
         """
-        Remove all traces of *svc_type*.
+        Remove all traces of *svc_type* in ourselves.
         """
         with suppress(KeyError):
-            del self.instantiated[svc_type]
+            del self._instantiated[svc_type]
 
     def close(self) -> None:
         """
-        Run all synchronous registered cleanups.
+        Run all registered *synchronous* cleanups.
 
         Async closes are *not* awaited.
         """
-        while self.cleanups:
-            rs, gen = self.cleanups.pop()
+        for rs, gen in reversed(self._cleanups):
             try:
                 if isinstance(gen, AsyncGenerator):
                     warnings.warn(
-                        f"Skipped async cleanup for {rs!r}. "
+                        f"Skipped async cleanup for {rs.name!r}. "
                         "Use aclose() instead.",
                         # stacklevel doesn't matter here; it's coming from a framework.
                         stacklevel=1,
                     )
                     continue
 
                 next(gen)
 
                 warnings.warn(
-                    f"clean up for {rs!r} didn't stop iterating", stacklevel=1
+                    f"Container clean up for {rs.name!r} didn't stop iterating.",
+                    stacklevel=1,
                 )
             except StopIteration:  # noqa: PERF203
                 pass
             except Exception:  # noqa: BLE001
                 log.warning(
-                    "clean up failed",
+                    "Container clean up failed for %r.",
+                    rs.name,
                     exc_info=True,
-                    extra={"service": rs.name},
+                    extra={"svcs_service_name": rs.name},
                 )
 
+        self._cleanups.clear()
+        self._instantiated.clear()
+
     async def aclose(self) -> None:
         """
         Run *all* registered cleanups -- synchronous **and** asynchronous.
         """
-        while self.cleanups:
-            rs, gen = self.cleanups.pop()
+        for rs, gen in reversed(self._cleanups):
             try:
                 if isinstance(gen, AsyncGenerator):
                     await anext(gen)
                 else:
                     next(gen)
 
                 warnings.warn(
-                    f"clean up for {rs!r} didn't stop iterating", stacklevel=1
+                    f"Container clean up for {rs.name!r} didn't stop iterating.",
+                    stacklevel=1,
                 )
 
             except (StopAsyncIteration, StopIteration):  # noqa: PERF203
                 pass
             except Exception:  # noqa: BLE001
                 log.warning(
-                    "clean up failed",
+                    "Container clean up failed for %r.",
+                    rs.name,
                     exc_info=True,
-                    extra={"service": rs.name},
+                    extra={"svcs_service_name": rs.name},
                 )
 
+        self._cleanups.clear()
+        self._instantiated.clear()
+
     def get_pings(self) -> list[ServicePing]:
         """
         Get all pingable services and bind them to ourselves for cleanups.
         """
         return [
             ServicePing(self, rs)
-            for rs in self.registry.services.values()
+            for rs in self.registry._services.values()
             if rs.ping is not None
         ]
 
 
 @attrs.frozen
 class RegisteredService:
     svc_type: type
     factory: Callable = attrs.field(hash=False)
     ping: Callable | None = attrs.field(hash=False)
 
     @property
     def name(self) -> str:
-        return self.svc_type.__qualname__
+        return f"{ self.svc_type.__module__ }.{self.svc_type.__qualname__}"
 
     def __repr__(self) -> str:
         return (
-            f"<RegisteredService(svc_type={ self.svc_type.__module__ }."
-            f"{ self.svc_type.__qualname__ }, "
+            f"<RegisteredService(svc_type="
+            f"{ self.name}, "
             f"has_ping={ self.ping is not None})>"
         )
 
     @property
     def is_async(self) -> bool:
         return iscoroutinefunction(self.factory) or isasyncgenfunction(
             self.factory
@@ -217,32 +225,99 @@
         Return True if you have to use `aping` instead of `ping`.
         """
         return self._rs.is_async or iscoroutinefunction(self._rs.ping)
 
 
 @attrs.define
 class Registry:
-    services: dict[type, RegisteredService] = attrs.Factory(dict)
+    _services: dict[type, RegisteredService] = attrs.Factory(dict)
+    _on_close: list[tuple[str, Callable]] = attrs.Factory(list)
 
     def register_factory(
         self,
         svc_type: type,
         factory: Callable,
         *,
         ping: Callable | None = None,
+        on_registry_close: Callable | None = None,
     ) -> None:
-        self.services[svc_type] = RegisteredService(svc_type, factory, ping)
+        rs = RegisteredService(svc_type, factory, ping)
+        self._services[svc_type] = rs
+
+        if on_registry_close is not None:
+            self._on_close.append((rs.name, on_registry_close))
 
     def register_value(
         self,
         svc_type: type,
         instance: object,
         *,
         ping: Callable | None = None,
+        on_registry_close: Callable | None = None,
     ) -> None:
-        self.register_factory(svc_type, lambda: instance, ping=ping)
+        self.register_factory(
+            svc_type,
+            lambda: instance,
+            ping=ping,
+            on_registry_close=on_registry_close,
+        )
 
     def get_registered_service_for(self, svc_type: type) -> RegisteredService:
         try:
-            return self.services[svc_type]
+            return self._services[svc_type]
         except KeyError:
             raise ServiceNotFoundError(svc_type) from None
+
+    def close(self) -> None:
+        """
+        Clear registrations & run synchronous ``on_registry_close`` callbacks.
+        """
+        for name, oc in reversed(self._on_close):
+            if iscoroutinefunction(oc):
+                warnings.warn(
+                    f"Skipped async cleanup for {name!r}. "
+                    "Use aclose() instead.",
+                    # stacklevel doesn't matter here; it's coming from a
+                    # framework.
+                    stacklevel=1,
+                )
+                continue
+
+            try:
+                log.debug("closing %r", name)
+                oc()
+                log.debug("closed %r", name)
+            except Exception:  # noqa: BLE001, PERF203
+                log.warning(
+                    "Registry's on_registry_close hook failed for %r.",
+                    name,
+                    exc_info=True,
+                    extra={"svcs_service_name": name},
+                )
+
+        self._services.clear()
+        self._on_close.clear()
+
+    async def aclose(self) -> None:
+        """
+        Clear registrations & run all ``on_registry_close`` callbacks.
+        """
+        for name, oc in reversed(self._on_close):
+            try:
+                if iscoroutinefunction(oc) or isawaitable(oc):
+                    log.debug("async closing %r", name)
+                    await oc()
+                    log.debug("async closed %r", name)
+                else:
+                    log.debug("closing %r", name)
+                    oc()
+                    log.debug("closed %r", name)
+            except Exception:  # noqa: BLE001, PERF203
+                log.warning(
+                    "Registry's on_registry_close hook failed for %r.",
+                    name,
+                    exc_info=True,
+                    extra={"svcs_service_name": name},
+                )
+
+        self._services.clear()
+        self._on_close.clear()
```

### Comparing `svcs-23.4.0/tests/test_async.py` & `svcs-23.5.0/tests/test_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,21 +73,23 @@
             await asyncio.sleep(0)
             cleaned_up = True
 
         registry.register_factory(Service, factory)
 
         svc = await container.aget(Service)
 
-        assert 1 == len(container.cleanups)
+        assert 1 == len(container._cleanups)
         assert Service() == svc
         assert not cleaned_up
 
         await container.aclose()
 
         assert cleaned_up
+        assert not container._instantiated
+        assert not container._cleanups
 
     @pytest.mark.asyncio()
     async def test_aclose_resilient(self, container, registry, caplog):
         """
         Failing cleanups are logged and ignored. They do not break the
         cleanup process.
         """
@@ -118,17 +120,24 @@
         assert 3 == await container.aget(YetAnotherService)
 
         assert not cleaned_up
 
         await container.aclose()
 
         # Inverse order
-        assert "AnotherService" == caplog.records[0].service
-        assert "Service" == caplog.records[1].service
+        assert (
+            "tests.test_async.AnotherService"
+            == caplog.records[0].svcs_service_name
+        )
+        assert (
+            "tests.test_async.Service" == caplog.records[1].svcs_service_name
+        )
         assert cleaned_up
+        assert not container._instantiated
+        assert not container._cleanups
 
     async def test_warns_if_generator_does_not_stop_after_cleanup(
         self, registry, container
     ):
         """
         If a generator doesn't stop after cleanup, a warning is emitted.
         """
@@ -141,17 +150,16 @@
 
         await container.aget(Service)
 
         with pytest.warns(UserWarning) as wi:
             await container.aclose()
 
         assert (
-            "clean up for <RegisteredService("
-            "svc_type=tests.test_async.Service, has_ping=False)> "
-            "didn't stop iterating" == wi.pop().message.args[0]
+            "Container clean up for 'tests.test_async.Service' "
+            "didn't stop iterating." == wi.pop().message.args[0]
         )
 
     async def test_aping(self, registry, container):
         """
         Async and sync pings work.
         """
         apinged = pinged = False
```

### Comparing `svcs-23.4.0/tests/test_core.py` & `svcs-23.5.0/tests/test_core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 # SPDX-FileCopyrightText: 2023 Hynek Schlawack <hs@ox.cx>
 #
 # SPDX-License-Identifier: MIT
 
 import asyncio
+import contextlib
+import inspect
 
-from unittest.mock import Mock
+from unittest.mock import AsyncMock, Mock
 
 import pytest
 
 import svcs
 
 
+needs_working_async_mock = pytest.mark.skipif(
+    not inspect.iscoroutinefunction(AsyncMock()),
+    reason="AsyncMock not working",
+)
+
+
 class Service:
     pass
 
 
 class AnotherService:
     pass
 
@@ -88,20 +96,20 @@
         """
         container.forget_service_type(Service)
 
     def test_forget_service_type_no_cleanup(self, container, rs, svc):
         """
         forget_service_type removes the registered service from the container.
         """
-        container.instantiated[rs.svc_type] = (rs, svc)
+        container._instantiated[rs.svc_type] = (rs, svc)
 
         container.forget_service_type(Service)
 
-        assert {} == container.instantiated
-        assert [] == container.cleanups
+        assert {} == container._instantiated
+        assert [] == container._cleanups
 
     @pytest.mark.asyncio()
     async def test_repr(self, registry, container):
         """
         The repr counts correctly.
         """
 
@@ -135,14 +143,16 @@
         container.get(Service)
 
         assert not cleaned_up
 
         container.close()
 
         assert cleaned_up
+        assert not container._instantiated
+        assert not container._cleanups
 
     def test_close_resilient(self, container, registry, caplog):
         """
         Failing cleanups are logged and ignored. They do not break the
         cleanup process.
         """
 
@@ -165,15 +175,15 @@
         assert 1 == container.get(Service)
         assert 3 == container.get(YetAnotherService)
 
         assert not cleaned_up
 
         container.close()
 
-        assert "Service" == caplog.records[0].service
+        assert "tests.test_core.Service" == caplog.records[0].svcs_service_name
         assert cleaned_up
 
     def test_warns_if_generator_does_not_stop_after_cleanup(
         self, registry, container
     ):
         """
         If a generator doesn't stop after cleanup, a warning is emitted.
@@ -187,17 +197,16 @@
 
         container.get(Service)
 
         with pytest.warns(UserWarning) as wi:
             container.close()
 
         assert (
-            "clean up for <RegisteredService("
-            "svc_type=tests.test_core.Service, has_ping=False)> "
-            "didn't stop iterating" == wi.pop().message.args[0]
+            "Container clean up for 'tests.test_core.Service' "
+            "didn't stop iterating." == wi.pop().message.args[0]
         )
 
 
 class TestRegisteredService:
     def test_repr(self, rs):
         """
         repr uses the fully-qualified name of a svc type.
@@ -208,15 +217,15 @@
         ) == repr(rs)
 
     def test_name(self, rs):
         """
         The name property deducts the correct class name.
         """
 
-        assert "Service" == rs.name
+        assert "tests.test_core.Service" == rs.name
 
     def test_is_async_yep(self):
         """
         The is_async property returns True if the factory needs to be awaited.
         """
 
         async def factory():
@@ -248,15 +257,15 @@
 
 class TestServicePing:
     def test_name(self, rs):
         """
         The name property proxies the correct class name.
         """
 
-        assert "Service" == svcs.ServicePing(None, rs).name
+        assert "tests.test_core.Service" == svcs.ServicePing(None, rs).name
 
     def test_ping(self, registry, container):
         """
         Calling ping instantiates the service using its factory, appends it to
         the cleanup list, and calls the service's ping method.
         """
 
@@ -277,7 +286,140 @@
         ping.assert_called_once()
 
         assert not cleaned_up
 
         container.close()
 
         assert cleaned_up
+        assert not container._instantiated
+        assert not container._cleanups
+
+
+class TestRegistry:
+    def test_empty_close(self):
+        """
+        Closing an empty registry does nothing.
+        """
+        svcs.Registry().close()
+
+        with contextlib.closing(svcs.Registry()):
+            ...
+
+    def test_close_closes(self, registry):
+        """
+        Calling close on Registry runs all on_close callbacks.
+        """
+        close_1 = Mock()
+        close_2 = Mock()
+
+        registry.register_factory(Service, Service, on_registry_close=close_1)
+        registry.register_value(
+            AnotherService, AnotherService, on_registry_close=close_2
+        )
+
+        registry.close()
+
+        assert close_1.called
+        assert close_2.called
+        assert not registry._services
+        assert not registry._on_close
+
+    def test_overwritten_factories_are_not_forgotten(self, registry):
+        """
+        If a factory is overwritten, it's close callback is still called.
+        """
+        close_1 = Mock()
+        close_2 = Mock()
+
+        registry.register_factory(Service, Service, on_registry_close=close_1)
+        registry.register_value(
+            Service, AnotherService, on_registry_close=close_2
+        )
+
+        registry.close()
+
+        assert close_1.called
+        assert close_2.called
+
+    def test_close_warns_about_async(self, registry):
+        """
+        Calling close raises a warning if there are async cleanups.
+        """
+
+        async def hook():
+            ...
+
+        registry.register_factory(Service, Service, on_registry_close=hook)
+
+        with pytest.warns(
+            UserWarning,
+            match="Skipped async cleanup for 'tests.test_core.Service'.",
+        ):
+            registry.close()
+
+    def test_close_logs_failures(self, registry, caplog):
+        """
+        Closing failures are logged but ignored.
+        """
+        registry.register_factory(
+            Service, Service, on_registry_close=Mock(side_effect=ValueError())
+        )
+
+        with contextlib.closing(registry):
+            ...
+
+        assert "tests.test_core.Service" == caplog.records[0].svcs_service_name
+
+    @pytest.mark.skipif(
+        not hasattr(contextlib, "aclosing"),
+        reason="Hasn't contextlib.aclosing()",
+    )
+    @pytest.mark.asyncio()
+    async def test_async_empty_close(self, registry):
+        """
+        Asynchronously closing an empty registry does nothing.
+        """
+        await registry.aclose()
+
+        async with contextlib.aclosing(svcs.Registry()):
+            ...
+
+    @pytest.mark.asyncio()
+    @needs_working_async_mock
+    async def test_aclose_mixed(self, registry):
+        """
+        aclose() closes all services, including async ones.
+        """
+        sync_close = Mock()
+        async_close = AsyncMock()
+
+        registry.register_factory(
+            Service, Service, on_registry_close=sync_close
+        )
+        registry.register_factory(
+            AnotherService, AnotherService, on_registry_close=async_close
+        )
+
+        await registry.aclose()
+
+        assert sync_close.called
+
+        async_close.assert_awaited_once()
+
+    @pytest.mark.asyncio()
+    @needs_working_async_mock
+    async def test_aclose_logs_failures(self, registry, caplog):
+        """
+        Async closing failures are logged but ignored.
+        """
+        close_mock = AsyncMock(side_effect=ValueError())
+
+        registry.register_factory(
+            Service,
+            Service,
+            on_registry_close=close_mock,
+        )
+
+        await registry.aclose()
+
+        close_mock.assert_awaited_once()
+        assert "tests.test_core.Service" == caplog.records[0].svcs_service_name
```

### Comparing `svcs-23.4.0/tests/test_flask.py` & `svcs-23.5.0/tests/test_flask.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         svcs.flask.replace_factory(Service2, factory2)
 
         svc1 = svcs.flask.get(Service1)
         svc2 = svcs.flask.get(Service2)
 
         assert isinstance(svc1, Service1)
         assert isinstance(svc2, Service2)
-        assert 2 == len(flask.g.svc_container.cleanups)
+        assert 2 == len(flask.g.svcs_container._cleanups)
 
         teardown(None)
 
         cleanup1.assert_called_once_with()
         cleanup2.assert_called_once_with()
 
     def test_overwrite_value(self, registry):
@@ -147,22 +147,22 @@
 
         svcs.flask.replace_factory(Service1, factory1)
         svcs.flask.replace_factory(Service2, factory2)
 
         svcs.flask.get(Service1)
         svcs.flask.get(Service2)
 
-        assert 2 == len(container.cleanups)
+        assert 2 == len(container._cleanups)
 
         svcs.flask.replace_factory(Service1, Interface)
 
         svcs.flask.get(Service1)
         svcs.flask.get(Service2)
 
-        assert 2 == len(container.cleanups)
+        assert 2 == len(container._cleanups)
 
     @pytest.mark.asyncio()
     async def test_teardown_warns_on_async_cleanups(self, container):
         """
         teardown() warns if there are async cleanups.
         """
 
@@ -176,54 +176,78 @@
         with pytest.warns(UserWarning) as wi:
             teardown(None)
 
         w = wi.pop()
 
         assert 0 == len(wi.list)
         assert (
-            "Skipped async cleanup for "
-            "<RegisteredService(svc_type=tests.test_flask.Service1, "
-            "has_ping=False)>. Use aclose() instead." == w.message.args[0]
+            "Skipped async cleanup for 'tests.test_flask.Service1'. "
+            "Use aclose() instead." == w.message.args[0]
         )
 
 
 class TestNonContextHelpers:
     def test_register_factory_helper(self, registry, app):
         """
         register_factory() registers a factory to the app that is passed.
         """
         svcs.flask.init_app(app, registry)
 
         svcs.flask.register_factory(app, Interface, Service1)
 
-        assert Interface in registry.services
+        assert Interface in registry._services
 
     def test_register_value_helper(self, registry, app):
         """
         register_value() registers a value to the app that is passed.
         """
         svcs.flask.init_app(app, registry)
 
         svcs.flask.register_value(app, Interface, 42)
 
-        assert Interface in registry.services
+        assert Interface in registry._services
 
 
 class TestInitApp:
     def test_implicit_registry(self):
         """
         init_app() creates a registry if one isn't provided.
         """
         app = flask.Flask("tests")
         svcs.flask.init_app(app)
 
-        assert isinstance(app.config["svcsistry"], svcs.Registry)
+        assert isinstance(app.config["svcs_registry"], svcs.Registry)
 
     def test_explicit_registry(self):
         """
         If a registry is passsed to init_app(), it's used.
         """
         registry = svcs.Registry()
         app = flask.Flask("tests")
         svcs.flask.init_app(app, registry)
 
-        assert registry is app.config["svcsistry"]
+        assert registry is app.config["svcs_registry"]
+
+
+class TestCloseRegistry:
+    def test_nop(self):
+        """
+        close_registry() does nothing if there's no registry in app.
+        """
+        app = flask.Flask("tests")
+        svcs.flask.close_registry(app)
+
+    def test_closes(self, app):
+        """
+        close_registry() runs the registry's close() method.
+        """
+        close = Mock()
+
+        svcs.flask.init_app(app)
+
+        svcs.flask.register_factory(
+            app, Interface, Service1, on_registry_close=close
+        )
+
+        svcs.flask.close_registry(app)
+
+        assert close.called
```

### Comparing `svcs-23.4.0/tests/typing/core.py` & `svcs-23.5.0/tests/typing/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,24 @@
 
 from typing import AsyncGenerator, Generator
 
 import svcs
 
 
 reg = svcs.Registry()
+con = svcs.Container(reg)
+
+reg.close()
+with contextlib.closing(reg) as reg:
+    ...
+
+
+async def f() -> None:
+    await reg.aclose()
+    await con.aclose()
 
 
 def gen() -> Generator:
     yield 42
 
 
 async def async_gen() -> AsyncGenerator:
@@ -49,10 +59,13 @@
 con.close()
 
 with contextlib.closing(svcs.Container(reg)) as con:
     ...
 
 if sys.version_info >= (3, 10):
 
-    async def f() -> None:
+    async def ctx() -> None:
         async with contextlib.aclosing(svcs.Container(reg)):
             ...
+
+        async with contextlib.aclosing(svcs.Registry()):
+            ...
```

### Comparing `svcs-23.4.0/tests/typing/flask_.py` & `svcs-23.5.0/tests/typing/flask_.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,7 +31,9 @@
 svcs.flask.register_factory(app, str, str)
 svcs.flask.register_factory(app, int, factory_with_cleanup)
 svcs.flask.register_value(app, str, str, ping=lambda: None)
 
 # The type checker believes whatever we tell it.
 o1: object = svcs.flask.get(object)
 o2: int = svcs.flask.get(object)
+
+svcs.flask.close_registry(app)
```

### Comparing `svcs-23.4.0/LICENSE` & `svcs-23.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svcs-23.4.0/pyproject.toml` & `svcs-23.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 
 [project]
 dynamic = ["version", "readme"]
 name = "svcs"
-description = "A Service Locator for Python"
+description = "A Lightweight Service Locator for Python"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["dependency injection"]
 authors = [{ name = "Hynek Schlawack", email = "hs@ox.cx" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
@@ -100,14 +100,20 @@
   "if __name__ == .__main__.:",
   # Typing-related
   "if TYPE_CHECKING:",
   "^ +\\.\\.\\.$",
 ]
 
 
+[tool.interrogate]
+verbose = 2
+fail-under = 100
+whitelist-regex = ["test_.*"]
+
+
 [tool.mypy]
 strict = true
 
 show_error_codes = true
 enable_error_code = ["ignore-without-code"]
 
 allow_any_generics = true
```

### Comparing `svcs-23.4.0/PKG-INFO` & `svcs-23.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: svcs
-Version: 23.4.0
-Summary: A Service Locator for Python
+Version: 23.5.0
+Summary: A Lightweight Service Locator for Python
 Project-URL: Changelog, https://github.com/hynek/svcs/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/hynek/svcs/blob/main/README.md
 Project-URL: Source, https://github.com/hynek/svcs
 Project-URL: Funding, https://github.com/sponsors/hynek
 Author-email: Hynek Schlawack <hs@ox.cx>
 License-Expression: MIT
 License-File: LICENSE
@@ -33,40 +33,43 @@
 Requires-Dist: mypy>=1.4; extra == 'typing'
 Description-Content-Type: text/markdown
 
 
 
 <p align="center">
   <a href="https://github.com/hynek/svcs/">
-    <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo.svg" width="25%" alt="svcs" />
+    <img src="https://raw.githubusercontent.com/hynek/svcs/main/docs/_static/logo.svg" width="20%" alt="svcs" />
   </a>
 </p>
 
 
-# *svcs*: A Service Locator for Python
+# *svcs*: A Lightweight Service Locator for Python
 
 > **Warning**
 > ☠️ Not ready yet! ☠️
 >
 > This project is only public to [gather feedback](https://github.com/hynek/svcs/discussions), and everything can and will change until the project is proclaimed stable.
 >
 > Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
 >
 > At this point, it's unclear whether this project will become a "proper Hynek project".
 > I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
 
 *svcs* (pronounced *services*) is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python.
 It provides you with a central place to register factories for types/interfaces and then imperatively request instances of those types with **automatic cleanup** and **health checks**.
 
-**This allows you to configure and manage resources in *one central place* and access them all in a *consistent* way.**
+---
+
+**This allows you to configure and manage all your resources in *one central place* and access them in a *consistent* way.**
 
 ---
 
 In practice that means that at runtime, you say "*Give me a database connection*!", and *svcs* will give you whatever you've configured it to return when asked for a database connection.
 This can be an actual database connection or it can be a mock object for testing.
+All of this happens *within* your application – service locators are **not** related to service discovery.
 
 If you like the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces; in Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [Abstract Base Class](https://docs.python.org/3.11/library/abc.html).
 
 That:
 
 - unifies **acquisition** and **cleanups** of resources,
 - simplifies **testing**,
@@ -90,46 +93,84 @@
     api = services.get(WebAPIClient)
 ```
 
 The latter already works with [Flask](#flask).
 
 You set it up like this:
 
+<!--
+; skip: next
+-->
+
 ```python
+import atexit
+
 from sqlalchemy import Connection, create_engine
 
 ...
 
 engine = create_engine("postgresql://localhost")
 
 def engine_factory():
     with engine.connect() as conn:
         yield conn
 
 registry = svcs.Registry()
-registry.register_factory(Connection, engine_factory)
+registry.register_factory(
+    Connection, engine_factory, on_registry_close=engine.dispose
+)
+
+@atexit.register
+def cleanup():
+    registry.close()  # calls engine.dispose()
 ```
 
 The generator-based setup and cleanup may remind you of [Pytest fixtures](https://docs.pytest.org/en/stable/explanation/fixtures.html).
-
-Unlike typical dependency injection that passes your dependencies as arguments, the active obtainment of resources by calling `get()` when you *know* you're going to need it avoids the conundrum of either having to pass a factory (e.g., a connection pool -- which also puts the onus of cleanup on you), or eagerly creating resources that are never used.
+The hooks that are defined as `on_registry_close` are called when you call `Registry.close()` – e.g. when your application is shutting down.
 
 *svcs* comes with **full async** support via a-prefixed methods (i.e. `aget()` instead of `get()`, et cetera).
 
+
+## Is this Dependency Injection!?
+
+No.
+
+Unlike [dependency injection](https://en.wikipedia.org/wiki/Dependency_injection), which passes your dependencies as arguments, you actively ask a service locator for them. This usually requires less opaque magic since nothing meddles with your function/method definitions. But you can use, e.g., your web framework's injection capabilities to inject the locator object into your views and benefit from *svcs*'s upsides without giving up some of DI's ones.
+
+The active acquisition of resources by calling `get()` when you *know* for sure you're going to need it avoids the conundrum of either having to pass a factory (e.g., a connection pool – which also puts the onus of cleanup on you) or eagerly creating resources that you never use:
+
+<!--
+; skip: next
+-->
+```python
+def view(request):
+    if request.form.valid():
+        # Form is valid; only NOW get a DB connection
+        # and pass it into your business logic.
+        return handle_form_data(
+            request.services.get(Database),
+            form.data,
+        )
+
+    raise InvalidFormError()
+```
+
+The main downside is that it's impossible to verify whether all required dependencies have been configured without running the code.
+
 ---
 
 For now, please refer to the [GitHub README](https://github.com/hynek/svcs/blob/main/README.md) for latest documentation.
 
 
 ## Release Information
 
-### Changed
+### Added
 
-- Renamed from *reg-svc* to *svcs*.
-  Sadly the more obvious names are all taken.
+- Registered factory/value clean up!
+  It is now possible to register an `on_registry_close` hook that is called once the `Registry`'s `(a)close()` method is called.
 
 
 ---
 
 [→ Full Changelog](https://github.com/hynek/svcs/blob/main/CHANGELOG.md)
```

