# Comparing `tmp/arclet_alconna_ichika-0.14.2.tar.gz` & `tmp/arclet_alconna_ichika-0.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_alconna_ichika-0.14.2.tar", last modified: Mon Jul  3 14:11:59 2023, max compression
+gzip compressed data, was "arclet_alconna_ichika-0.14.3.tar", last modified: Wed Jul 26 06:28:22 2023, max compression
```

## Comparing `arclet_alconna_ichika-0.14.2.tar` & `arclet_alconna_ichika-0.14.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet_alconna_ichika-0.14.2/LICENSE
--rw-r--r--   0        0        0     7388 2023-05-26 09:21:34.997183 arclet_alconna_ichika-0.14.2/README.md
--rw-r--r--   0        0        0     6207 2023-07-03 14:11:59.241833 arclet_alconna_ichika-0.14.2/pyproject.toml
--rw-r--r--   0        0        0       80 2023-05-09 04:08:01.631055 arclet_alconna_ichika-0.14.2/src/arclet/alconna/ichika/__init__.py
--rw-r--r--   0        0        0     5822 2023-06-30 17:20:01.758718 arclet_alconna_ichika-0.14.2/src/arclet/alconna/ichika/adapter.py
--rw-r--r--   0        0        0     1256 2023-05-09 04:21:37.796354 arclet_alconna_ichika-0.14.2/src/arclet/alconna/ichika/typings.py
--rw-r--r--   0        0        0     7914 1970-01-01 00:00:00.000000 arclet_alconna_ichika-0.14.2/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet_alconna_ichika-0.14.3/LICENSE
+-rw-r--r--   0        0        0     7388 2023-05-26 09:21:34.997183 arclet_alconna_ichika-0.14.3/README.md
+-rw-r--r--   0        0        0     6153 2023-07-26 06:28:22.031997 arclet_alconna_ichika-0.14.3/pyproject.toml
+-rw-r--r--   0        0        0       80 2023-05-09 04:08:01.631055 arclet_alconna_ichika-0.14.3/src/arclet/alconna/ichika/__init__.py
+-rw-r--r--   0        0        0     5835 2023-07-26 06:04:06.357591 arclet_alconna_ichika-0.14.3/src/arclet/alconna/ichika/adapter.py
+-rw-r--r--   0        0        0     1256 2023-05-09 04:21:37.796354 arclet_alconna_ichika-0.14.3/src/arclet/alconna/ichika/typings.py
+-rw-r--r--   0        0        0     7914 1970-01-01 00:00:00.000000 arclet_alconna_ichika-0.14.3/PKG-INFO
```

### Comparing `arclet_alconna_ichika-0.14.2/LICENSE` & `arclet_alconna_ichika-0.14.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet_alconna_ichika-0.14.2/README.md` & `arclet_alconna_ichika-0.14.3/README.md`

 * *Files identical despite different names*

### Comparing `arclet_alconna_ichika-0.14.2/pyproject.toml` & `arclet_alconna_ichika-0.14.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-alconna-ichika"
-version = "0.14.2"
+version = "0.14.3"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "ichika>=0.0.5",
 ]
 description = "Support Alconna to BlueGlassBlock/Ichika"
@@ -30,17 +30,17 @@
 
 [project.urls]
 homepage = "https://github.com/ArcletProject/Alconna-Graia"
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.pdm.dev-dependencies]
 dev = [
+    "editables>=0.3.0",
     "fix-future-annotations>=0.5.0",
-    "textual~=0.11.1",
-    "avilla-console @ file:///${PROJECT_ROOT}/avilla_console-0.1.1-py3-none-any.whl",
+    "textual<1.0.0, >=0.29.0",
 ]
 
 [tool.pdm.scripts]
 buildall = "pdm mina build -a"
 pub = "pdm publish --no-build"
 
 [tool.pdm.scripts.puball]
@@ -60,15 +60,15 @@
 [tool.mina.packages.core]
 includes = [
     "src/arclet/alconna/graia",
 ]
 
 [tool.mina.packages.core.project]
 name = "arclet-alconna-graia"
-version = "0.14.2"
+version = "0.14.3"
 description = "Support Alconna to GraiaProject"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -112,20 +112,20 @@
 alconna_behavior = "arclet.alconna.graia.create:AlconnaBehaviorCreator"
 
 [tool.mina.packages.ariadne]
 includes = [
     "src/arclet/alconna/ariadne",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.15.0, >= 0.14.2",
+    "arclet-alconna-graia<0.15.0, >= 0.14.3",
 ]
 
 [tool.mina.packages.ariadne.project]
 name = "arclet-alconna-ariadne"
-version = "0.14.2"
+version = "0.14.3"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0, >=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -153,20 +153,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.avilla]
 includes = [
     "src/arclet/alconna/avilla",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.15.0, >= 0.14.2",
+    "arclet-alconna-graia<0.15.0, >= 0.14.3",
 ]
 
 [tool.mina.packages.avilla.project]
 name = "arclet-alconna-avilla"
-version = "0.14.2"
+version = "0.14.3"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "avilla-core>=1.0.0a5",
 ]
 description = "Support Alconna to GraiaProject/Avilla"
@@ -195,20 +195,20 @@
 repository = "https://github.com/ArcletProject/Alconna-Graia"
 
 [tool.mina.packages.ichika]
 includes = [
     "src/arclet/alconna/ichika",
 ]
 raw-dependencies = [
-    "arclet-alconna-graia<0.15.0, >= 0.14.2",
+    "arclet-alconna-graia<0.15.0, >= 0.14.3",
 ]
 
 [tool.mina.packages.ichika.project]
 name = "arclet-alconna-ichika"
-version = "0.14.2"
+version = "0.14.3"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "ichika>=0.0.5",
 ]
 description = "Support Alconna to BlueGlassBlock/Ichika"
```

### Comparing `arclet_alconna_ichika-0.14.2/src/arclet/alconna/ichika/adapter.py` & `arclet_alconna_ichika-0.14.3/src/arclet/alconna/ichika/adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     def completion_waiter(self, source: MessageEvent, priority: int = 15) -> Waiter:
         @Waiter.create_using_function(
             [source.__class__],
             block_propagation=True,
             priority=priority,
         )
         async def waiter(m: MessageChain, sender: Friend | Member):
-            if source.sender.uin == sender.uid:
+            if isinstance(sender, source.sender.__class__) and source.sender.uin == sender.uid:
                 return m
 
         return waiter  # type: ignore
 
     async def lookup_source(self, interface: DispatcherInterface[MessageEvent]) -> MessageChain:
         return await interface.lookup_param("__message_chain__", MessageChain, MessageChain([Text("Unknown")]))
 
@@ -116,16 +116,15 @@
     def handle_listen(
         self,
         func: Callable,
         buffer: dict[str, Any],
         dispatcher: BaseDispatcher | None,
         guild: bool,
         private: bool,
-        private_name: str,
-        guild_name: str
+        **kwargs
     ) -> None:
         events = []
         if guild:
             events.append(GroupMessage)
         if private:
             events.append(FriendMessage)
         buffer.setdefault("dispatchers", [])
```

### Comparing `arclet_alconna_ichika-0.14.2/src/arclet/alconna/ichika/typings.py` & `arclet_alconna_ichika-0.14.3/src/arclet/alconna/ichika/typings.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_ichika-0.14.2/PKG-INFO` & `arclet_alconna_ichika-0.14.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ichika
-Version: 0.14.2
+Version: 0.14.3
 Summary: Support Alconna to BlueGlassBlock/Ichika
 Keywords: alconna graia arclet ichika
 Home-page: https://github.com/ArcletProject/Alconna-Graia
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: AGPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

