# Comparing `tmp/databasez-0.4.0.tar.gz` & `tmp/databasez-0.5.0.tar.gz`

## Comparing `databasez-0.4.0.tar` & `databasez-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/__init__.py
--rw-r--r--   0        0        0    21730 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/core.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/importer.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/interfaces.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/py.typed
--rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/testclient.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/__init__.py
--rw-r--r--   0        0        0    11179 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/aiopg.py
--rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/asyncmy.py
--rw-r--r--   0        0        0    11987 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/mssql.py
--rw-r--r--   0        0        0    11054 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/mysql.py
--rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/postgres.py
--rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/sqlite.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/common/__init__.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/common/records.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/compilers/__init__.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/compilers/psycopg.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/dialects/__init__.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 databasez-0.4.0/databasez/backends/dialects/psycopg.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 databasez-0.4.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 databasez-0.4.0/LICENSE.md
--rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 databasez-0.4.0/README.md
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 databasez-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    10741 2020-02-02 00:00:00.000000 databasez-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/__init__.py
+-rw-r--r--   0        0        0    23433 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/core.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/importer.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/interfaces.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/py.typed
+-rw-r--r--   0        0        0     8783 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/testclient.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/__init__.py
+-rw-r--r--   0        0        0    11179 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/aiopg.py
+-rw-r--r--   0        0        0    11399 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/asyncmy.py
+-rw-r--r--   0        0        0    11987 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/mssql.py
+-rw-r--r--   0        0        0    11054 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/mysql.py
+-rw-r--r--   0        0        0     8427 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/postgres.py
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/sqlite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/common/__init__.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/common/records.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/compilers/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/compilers/psycopg.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/dialects/__init__.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 databasez-0.5.0/databasez/backends/dialects/psycopg.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 databasez-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 databasez-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 databasez-0.5.0/README.md
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 databasez-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 databasez-0.5.0/PKG-INFO
```

### Comparing `databasez-0.4.0/databasez/core.py` & `databasez-0.5.0/databasez/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import asyncio
 import contextlib
 import functools
 import logging
 import typing
+import weakref
 from contextvars import ContextVar
 from types import TracebackType
 from urllib.parse import SplitResult, parse_qsl, unquote, urlencode, urlsplit
 
 from sqlalchemy import text
 from sqlalchemy.sql import ClauseElement
-from sqlalchemy.util._concurrency_py3k import greenlet_spawn
 
 from databasez.importer import import_from_string
-from databasez.interfaces import DatabaseBackend, Record
+from databasez.interfaces import DatabaseBackend, Record, TransactionBackend
 
 if typing.TYPE_CHECKING:
     from databasez.types import DictAny
 
 try:  # pragma: no cover
     import click
 
@@ -31,14 +31,19 @@
     CONNECT_EXTRA = {}
     DISCONNECT_EXTRA = {}
 
 
 logger = logging.getLogger("databasez")
 
 
+ACTIVE_TRANSACTIONS: ContextVar[
+    typing.Optional["weakref.WeakKeyDictionary['Transaction', 'TransactionBackend']"]
+] = ContextVar("databasez:active_transactions", default=None)
+
+
 class Database:
     """
     An abstraction on the top of the EncodeORM databases.Database object.
 
     This object allows to pass also a configuration dictionary in the format of
 
     DATABASEZ_CONFIG = {
@@ -68,14 +73,15 @@
         "mssql": "databasez.backends.mssql:MSSQLBackend",
         "mssql+pyodbc": "databasez.backends.mssql:MSSQLBackend",
         "mssql+aioodbc": "databasez.backends.mssql:MSSQLBackend",
         "sqlite": "databasez.backends.sqlite:SQLiteBackend",
     }
     DIRECT_URL_SCHEME = {"sqlite"}
     MANDATORY_FIELDS = ["host", "port", "user", "database"]
+    _connection_map: "weakref.WeakKeyDictionary[asyncio.Task, 'Connection']"
 
     def __init__(
         self,
         url: typing.Optional[typing.Union[str, "DatabaseURL"]] = None,
         *,
         force_rollback: bool = False,
         config: typing.Optional["DictAny"] = None,
@@ -88,25 +94,23 @@
             _url = url
         else:
             _url = self._build_url(config)
 
         self.url = DatabaseURL(_url)  # type: ignore
         self.options = options
         self.is_connected = False
+        self._connection_map = weakref.WeakKeyDictionary()
 
         self._force_rollback = force_rollback
 
         backend_str = self._get_backend()
         backend_cls = import_from_string(backend_str)
         assert issubclass(backend_cls, DatabaseBackend)
         self._backend = backend_cls(self.url, **self.options)
 
-        # Connections are stored as task-local state.
-        self._connection_context: ContextVar = ContextVar("connection_context")
-
         # When `force_rollback=True` is used, we use a single global
         # connection, within a transaction that always rolls back.
         self._global_connection: typing.Optional[Connection] = None
         self._global_transaction: typing.Optional[Transaction] = None
 
     @property
     def allowed_url_schemes(self) -> typing.Set[str]:
@@ -160,14 +164,38 @@
 
     def _build_url_for_direct_url_scheme(self, scheme: str, database: str) -> str:
         """Builds the URL for direct url schemes that do not support user, password and other
         parameters. Example: SQLite.
         """
         return f"{scheme}:///{database}"
 
+    @property
+    def _current_task(self) -> asyncio.Task:
+        task = asyncio.current_task()
+        if not task:
+            raise RuntimeError("No currently active asyncio.Task found")
+        return task
+
+    @property
+    def _connection(self) -> typing.Optional["Connection"]:
+        return self._connection_map.get(self._current_task)
+
+    @_connection.setter
+    def _connection(
+        self, connection: typing.Optional["Connection"]
+    ) -> typing.Optional["Connection"]:
+        task = self._current_task
+
+        if connection is None:
+            self._connection_map.pop(task, None)
+        else:
+            self._connection_map[task] = connection
+
+        return self._connection
+
     async def connect(self) -> None:
         """
         Establish the connection pool.
         """
         if self.is_connected:
             logger.debug("Already connected, skipping connection")
             return None
@@ -176,15 +204,15 @@
         logger.info("Connected to database %s", self.url.obscure_password, extra=CONNECT_EXTRA)
         self.is_connected = True
 
         if self._force_rollback:
             assert self._global_connection is None
             assert self._global_transaction is None
 
-            self._global_connection = Connection(self._backend)
+            self._global_connection = Connection(self, self._backend)
             self._global_transaction = self._global_connection.transaction(force_rollback=True)
 
             await self._global_transaction.__aenter__()
 
     async def disconnect(self) -> None:
         """
         Close all connections in the connection pool.
@@ -198,15 +226,15 @@
             assert self._global_transaction is not None
 
             await self._global_transaction.__aexit__()
 
             self._global_transaction = None
             self._global_connection = None
         else:
-            self._connection_context = ContextVar("connection_context")
+            self._connection = None
 
         await self._backend.disconnect()
         logger.info(
             "Disconnected from database %s",
             self.url.obscure_password,
             extra=DISCONNECT_EXTRA,
         )
@@ -270,20 +298,17 @@
             async for record in connection.iterate(query, values):
                 yield record
 
     def connection(self) -> "Connection":
         if self._global_connection is not None:
             return self._global_connection
 
-        try:
-            return self._connection_context.get()  # type: ignore
-        except LookupError:
-            connection = Connection(self._backend)
-            self._connection_context.set(connection)
-            return connection
+        if not self._connection:
+            self._connection = Connection(self, self._backend)
+        return self._connection
 
     def transaction(self, *, force_rollback: bool = False, **kwargs: typing.Any) -> "Transaction":
         return Transaction(self.connection, force_rollback=force_rollback, **kwargs)
 
     @contextlib.contextmanager
     def force_rollback(self) -> typing.Iterator[None]:
         initial = self._force_rollback
@@ -296,15 +321,16 @@
     def _get_backend(self) -> str:
         return self.SUPPORTED_BACKENDS.get(
             self.url.scheme, self.SUPPORTED_BACKENDS[self.url.dialect]
         )
 
 
 class Connection:
-    def __init__(self, backend: DatabaseBackend) -> None:
+    def __init__(self, database: Database, backend: DatabaseBackend) -> None:
+        self._database = database
         self._backend = backend
 
         self._connection_lock = asyncio.Lock()
         self._connection = self._backend.connection()
         self._connection_counter = 0
 
         self._transaction_lock = asyncio.Lock()
@@ -330,14 +356,15 @@
         traceback: typing.Optional[TracebackType] = None,
     ) -> None:
         async with self._connection_lock:
             assert self._connection is not None
             self._connection_counter -= 1
             if self._connection_counter == 0:
                 await self._connection.release()
+                self._database._connection = None
 
     async def fetch_all(
         self,
         query: typing.Union[ClauseElement, str],
         values: typing.Optional[dict] = None,
     ) -> typing.List[Record]:
         built_query = self._build_query(query, values)
@@ -394,19 +421,14 @@
 
         return Transaction(connection_callable, force_rollback, **kwargs)
 
     @property
     def raw_connection(self) -> typing.Any:
         return self._connection.raw_connection
 
-    async def run_sync(
-        self, fn: typing.Callable[..., typing.Any], *arg: typing.Any, **kw: typing.Any
-    ) -> typing.Any:
-        return await greenlet_spawn(fn, self._connection.raw_connection, *arg, **kw)
-
     @staticmethod
     def _build_query(
         query: typing.Union[ClauseElement, str], values: typing.Optional[dict] = None
     ) -> ClauseElement:
         if isinstance(query, str):
             query = text(query)
 
@@ -427,14 +449,45 @@
         force_rollback: bool,
         **kwargs: typing.Any,
     ) -> None:
         self._connection_callable = connection_callable
         self._force_rollback = force_rollback
         self._extra_options = kwargs
 
+    @property
+    def _connection(self) -> "Connection":
+        # Returns the same connection if called multiple times
+        return self._connection_callable()
+
+    @property
+    def _transaction(self) -> typing.Optional["TransactionBackend"]:
+        transactions = ACTIVE_TRANSACTIONS.get()
+        if transactions is None:
+            return None
+
+        return transactions.get(self, None)
+
+    @_transaction.setter
+    def _transaction(
+        self, transaction: typing.Optional["TransactionBackend"]
+    ) -> typing.Optional["TransactionBackend"]:
+        transactions = ACTIVE_TRANSACTIONS.get()
+        if transactions is None:
+            transactions = weakref.WeakKeyDictionary()
+        else:
+            transactions = transactions.copy()
+
+        if transaction is None:
+            transactions.pop(self, None)
+        else:
+            transactions[self] = transaction
+
+        ACTIVE_TRANSACTIONS.set(transactions)
+        return transactions.get(self, None)
+
     async def __aenter__(self) -> "Transaction":
         """
         Called when entering `async with database.transaction()`
         """
         await self.start()
         return self
 
@@ -467,37 +520,40 @@
         async def wrapper(*args: typing.Any, **kwargs: typing.Any) -> typing.Any:
             async with self:
                 return await func(*args, **kwargs)
 
         return wrapper  # type: ignore
 
     async def start(self) -> "Transaction":
-        self._connection = self._connection_callable()
         self._transaction = self._connection._connection.transaction()
 
         async with self._connection._transaction_lock:
             is_root = not self._connection._transaction_stack
             await self._connection.__aenter__()
             await self._transaction.start(is_root=is_root, extra_options=self._extra_options)
             self._connection._transaction_stack.append(self)
         return self
 
     async def commit(self) -> None:
         async with self._connection._transaction_lock:
             assert self._connection._transaction_stack[-1] is self
             self._connection._transaction_stack.pop()
+            assert self._transaction is not None
             await self._transaction.commit()
             await self._connection.__aexit__()
+            self._transaction = None
 
     async def rollback(self) -> None:
         async with self._connection._transaction_lock:
             assert self._connection._transaction_stack[-1] is self
             self._connection._transaction_stack.pop()
+            assert self._transaction is not None
             await self._transaction.rollback()
             await self._connection.__aexit__()
+            self._transaction = None
 
 
 class _EmptyNetloc(str):
     def __bool__(self) -> bool:
         return True
```

### Comparing `databasez-0.4.0/databasez/importer.py` & `databasez-0.5.0/databasez/importer.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/databasez/interfaces.py` & `databasez-0.5.0/databasez/interfaces.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/databasez/testclient.py` & `databasez-0.5.0/databasez/testclient.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/databasez/backends/aiopg.py` & `databasez-0.5.0/databasez/backends/aiopg.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/databasez/backends/asyncmy.py` & `databasez-0.5.0/databasez/backends/asyncmy.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/databasez/backends/mssql.py` & `databasez-0.5.0/databasez/backends/mssql.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/databasez/backends/mysql.py` & `databasez-0.5.0/databasez/backends/mysql.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/databasez/backends/postgres.py` & `databasez-0.5.0/databasez/backends/postgres.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/databasez/backends/sqlite.py` & `databasez-0.5.0/databasez/backends/sqlite.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/databasez/backends/common/records.py` & `databasez-0.5.0/databasez/backends/common/records.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/databasez/backends/dialects/psycopg.py` & `databasez-0.5.0/databasez/backends/dialects/psycopg.py`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/LICENSE.md` & `databasez-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/README.md` & `databasez-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `databasez-0.4.0/pyproject.toml` & `databasez-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
-dependencies = ["nest_asyncio>=1.5.6,<2.0.0", "sqlalchemy>=2.0.16,<2.1"]
+dependencies = ["nest_asyncio>=1.5.6,<2.0.0", "sqlalchemy>=2.0.19,<2.1"]
 keywords = [
     "mysql",
     "postgres",
     "sqlalchemy",
     "sqlite",
     "asyncio",
     "esmerald",
@@ -74,14 +74,15 @@
 dev = [
     "asyncmy>=0.2.7,<0.3.0",
     "aiopg>=1.4.0,<2.0.0",
     "aiomysql>=0.1.1,<0.2.0",
     "aiosqlite>=0.18.0,<0.20.0",
     "asyncpg>=0.27.0,<0.30.0",
     "aioodbc>=0.4.0,<0.5.0",
+    "ipdb>=0.13.13",
     "pre-commit>=2.17.0,<4.0.0",
     "psycopg2-binary>=2.9.6,<3.0.0",
     "pymysql>=1.0.3,<2.0.0",
     "pyodbc>=4.0.35,<5.0.0",
 ]
 
 doc = [
```

### Comparing `databasez-0.4.0/PKG-INFO` & `databasez-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databasez
-Version: 0.4.0
+Version: 0.5.0
 Summary: Async database support for Python.
 Project-URL: Homepage, https://github.com/tarsil/databasez
 Project-URL: Documentation, https://databasez.tarsild/
 Project-URL: Changelog, https://databasez.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/databasez
 Author-email: Tiago Silva <tiago.arasilva@gmail.com>
@@ -33,15 +33,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: nest-asyncio<2.0.0,>=1.5.6
-Requires-Dist: sqlalchemy<2.1,>=2.0.16
+Requires-Dist: sqlalchemy<2.1,>=2.0.19
 Provides-Extra: aiomysql
 Requires-Dist: aiomysql; extra == 'aiomysql'
 Provides-Extra: aioodbc
 Requires-Dist: aioodbc; extra == 'aioodbc'
 Provides-Extra: aiopg
 Requires-Dist: aiopg; extra == 'aiopg'
 Provides-Extra: aiosqlite
@@ -53,14 +53,15 @@
 Provides-Extra: dev
 Requires-Dist: aiomysql<0.2.0,>=0.1.1; extra == 'dev'
 Requires-Dist: aioodbc<0.5.0,>=0.4.0; extra == 'dev'
 Requires-Dist: aiopg<2.0.0,>=1.4.0; extra == 'dev'
 Requires-Dist: aiosqlite<0.20.0,>=0.18.0; extra == 'dev'
 Requires-Dist: asyncmy<0.3.0,>=0.2.7; extra == 'dev'
 Requires-Dist: asyncpg<0.30.0,>=0.27.0; extra == 'dev'
+Requires-Dist: ipdb>=0.13.13; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=2.17.0; extra == 'dev'
 Requires-Dist: psycopg2-binary<3.0.0,>=2.9.6; extra == 'dev'
 Requires-Dist: pymysql<2.0.0,>=1.0.3; extra == 'dev'
 Requires-Dist: pyodbc<5.0.0,>=4.0.35; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
```

