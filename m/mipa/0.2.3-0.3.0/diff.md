# Comparing `tmp/mipa-0.2.3.tar.gz` & `tmp/mipa-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mipa-0.2.3.tar", last modified: Sun Jun 18 02:35:22 2023, max compression
+gzip compressed data, was "mipa-0.3.0.tar", last modified: Wed Jul 26 01:05:17 2023, max compression
```

## Comparing `mipa-0.2.3.tar` & `mipa-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 02:35:08.000000 mipa-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-18 02:35:08.000000 mipa-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-18 02:35:22.596957 mipa-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-06-18 02:35:08.000000 mipa-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa/ext/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa/ext/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/cog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/commands/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa/ext/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/ext/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/router.py
--rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-18 02:35:08.000000 mipa-0.2.3/mipa/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:35:22.596957 mipa-0.2.3/mipa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-06-18 02:35:22.000000 mipa-0.2.3/mipa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-18 02:35:22.000000 mipa-0.2.3/mipa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:35:22.000000 mipa-0.2.3/mipa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-18 02:35:22.000000 mipa-0.2.3/mipa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-18 02:35:22.000000 mipa-0.2.3/mipa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-18 02:35:08.000000 mipa-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-18 02:35:08.000000 mipa-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-18 02:35:22.596957 mipa-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-18 02:35:08.000000 mipa-0.2.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-18 02:35:08.000000 mipa-0.2.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 01:05:17.665750 mipa-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-26 01:05:06.000000 mipa-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-26 01:05:06.000000 mipa-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-26 01:05:17.665750 mipa-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-07-26 01:05:06.000000 mipa-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 01:05:17.665750 mipa-0.3.0/mipa/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-26 01:05:17.665750 mipa-0.3.0/mipa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 01:05:17.661750 mipa-0.3.0/mipa/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 01:05:17.665750 mipa-0.3.0/mipa/ext/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/ext/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/ext/commands/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/ext/commands/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/ext/commands/cog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/ext/commands/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/ext/commands/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 01:05:17.665750 mipa-0.3.0/mipa/ext/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/ext/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-26 01:05:06.000000 mipa-0.3.0/mipa/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 01:05:17.661750 mipa-0.3.0/mipa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-26 01:05:17.000000 mipa-0.3.0/mipa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-26 01:05:17.000000 mipa-0.3.0/mipa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 01:05:17.000000 mipa-0.3.0/mipa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-26 01:05:17.000000 mipa-0.3.0/mipa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-26 01:05:17.000000 mipa-0.3.0/mipa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-26 01:05:06.000000 mipa-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-26 01:05:06.000000 mipa-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-26 01:05:17.665750 mipa-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-26 01:05:06.000000 mipa-0.3.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-26 01:05:06.000000 mipa-0.3.0/versioneer.py
```

### Comparing `mipa-0.2.3/LICENSE` & `mipa-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/PKG-INFO` & `mipa-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipa
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/MiPA
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `mipa-0.2.3/README.md` & `mipa-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/client.py` & `mipa-0.3.0/mipa/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,34 +202,40 @@
     async def __on_error(event_method: str) -> None:
         print(f'Ignoring exception in {event_method}', file=sys.stderr)
         traceback.print_exc()
 
     async def on_error(self, err):
         self.event_dispatch('error', err)
 
-    async def create_api_session(self, token: str, url: str) -> API:
-        self.core = API(url, token)
+    async def create_api_session(
+        self, token: str, url: str, log_level: LOGING_LEVEL_TYPE | None,
+    ) -> API:
+        self.core = API(url, token, log_level=log_level)
         return self.core
 
     async def setup_hook(self) -> None:
         ...
 
-    async def login(self, token: str, url: str):
+    async def login(
+        self, token: str, url: str, log_level: LOGING_LEVEL_TYPE | None
+    ):
         """
         ユーザーにログインし、ユーザー情報を取得します
 
         Parameters
         ----------
         token : str
             BOTにするユーザーのTOKEN
         url : str
             BOTにするユーザーがいるインスタンスのURL
+        log_level : LOGING_LEVEL_TYPE
+            The log level to use for logging. Defaults to ``INFO``.
         """
 
-        core = await self.create_api_session(token, url)
+        core = await self.create_api_session(token, url, log_level)
         await core.http.login()
         self.user = await core.api.get_me()
         await self.setup_hook()
 
     async def _connect(
         self, *, timeout: int = 60, event_name: str = 'ready',
     ) -> None:
@@ -274,15 +280,15 @@
         url: str,
         token: str,
         *,
         debug: bool = False,
         reconnect: bool = True,
         timeout: int = 60,
         is_ayuskey: bool = False,
-        log_level: LOGING_LEVEL_TYPE = 'INFO',
+        log_level: LOGING_LEVEL_TYPE | None = 'INFO',
     ):
         """
         Starting Bot
 
         Parameters
         ----------
         url: str
@@ -292,15 +298,16 @@
         debug: bool, default False
             debugging mode
         reconnect: bool, default True
             coming soon...
         timeout: int, default 60
             Time until websocket times out
         """
-        setup_logging(level=log_level)
+        if log_level is not None:
+            setup_logging(level=log_level)
         self.token = token
         url = url[:-1] if url[-1] == '/' else url
         split_url = url.split('/')
 
         if origin_url := re.search(r'wss?://(.*)', url):
             origin_url = (
                 origin_url.group(0)
@@ -311,9 +318,9 @@
         else:
             origin_url = url
         if 'streaming' not in split_url:
             split_url.append('streaming')
             url = '/'.join(split_url)
         self.url = url.replace('https', 'wss').replace('http', 'ws')
         self.origin_url = origin_url
-        await self.login(token, origin_url)
+        await self.login(token, origin_url, log_level)
         await self.connect(reconnect=reconnect, timeout=timeout)
```

### Comparing `mipa-0.2.3/mipa/exception.py` & `mipa-0.3.0/mipa/exception.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/ext/commands/_types.py` & `mipa-0.3.0/mipa/ext/commands/_types.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/ext/commands/bot.py` & `mipa-0.3.0/mipa/ext/commands/bot.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/ext/commands/cog.py` & `mipa-0.3.0/mipa/ext/commands/cog.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/ext/commands/context.py` & `mipa-0.3.0/mipa/ext/commands/context.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/ext/commands/core.py` & `mipa-0.3.0/mipa/ext/commands/core.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/ext/tasks/__init__.py` & `mipa-0.3.0/mipa/ext/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/gateway.py` & `mipa-0.3.0/mipa/gateway.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/http.py` & `mipa-0.3.0/mipa/http.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/router.py` & `mipa-0.3.0/mipa/router.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/state.py` & `mipa-0.3.0/mipa/state.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa/utils.py` & `mipa-0.3.0/mipa/utils.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/mipa.egg-info/PKG-INFO` & `mipa-0.3.0/mipa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipa
-Version: 0.2.3
+Version: 0.3.0
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/MiPA
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `mipa-0.2.3/mipa.egg-info/SOURCES.txt` & `mipa-0.3.0/mipa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/setup.py` & `mipa-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `mipa-0.2.3/versioneer.py` & `mipa-0.3.0/versioneer.py`

 * *Files identical despite different names*

