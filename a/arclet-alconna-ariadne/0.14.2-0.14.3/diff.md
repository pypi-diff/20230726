# Comparing `tmp/arclet_alconna_ariadne-0.14.2.tar.gz` & `tmp/arclet_alconna_ariadne-0.14.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet_alconna_ariadne-0.14.2.tar", last modified: Mon Jul  3 14:11:54 2023, max compression
+gzip compressed data, was "arclet_alconna_ariadne-0.14.3.tar", last modified: Wed Jul 26 06:28:18 2023, max compression
```

## Comparing `arclet_alconna_ariadne-0.14.2.tar` & `arclet_alconna_ariadne-0.14.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet_alconna_ariadne-0.14.2/LICENSE
--rw-r--r--   0        0        0     7388 2023-05-26 09:21:34.997183 arclet_alconna_ariadne-0.14.2/README.md
--rw-r--r--   0        0        0     6208 2023-07-03 14:11:54.915409 arclet_alconna_ariadne-0.14.2/pyproject.toml
--rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet_alconna_ariadne-0.14.2/src/arclet/alconna/ariadne/__init__.py
--rw-r--r--   0        0        0     5488 2023-06-30 17:20:01.730941 arclet_alconna_ariadne-0.14.2/src/arclet/alconna/ariadne/adapter.py
--rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet_alconna_ariadne-0.14.2/src/arclet/alconna/ariadne/typings.py
--rw-r--r--   0        0        0     7922 1970-01-01 00:00:00.000000 arclet_alconna_ariadne-0.14.2/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-05-04 12:40:50.638175 arclet_alconna_ariadne-0.14.3/LICENSE
+-rw-r--r--   0        0        0     7388 2023-05-26 09:21:34.997183 arclet_alconna_ariadne-0.14.3/README.md
+-rw-r--r--   0        0        0     6154 2023-07-26 06:28:18.397951 arclet_alconna_ariadne-0.14.3/pyproject.toml
+-rw-r--r--   0        0        0       81 2023-02-20 07:51:15.898481 arclet_alconna_ariadne-0.14.3/src/arclet/alconna/ariadne/__init__.py
+-rw-r--r--   0        0        0     5502 2023-07-26 06:04:06.337391 arclet_alconna_ariadne-0.14.3/src/arclet/alconna/ariadne/adapter.py
+-rw-r--r--   0        0        0     1262 2023-05-08 17:03:36.101915 arclet_alconna_ariadne-0.14.3/src/arclet/alconna/ariadne/typings.py
+-rw-r--r--   0        0        0     7922 1970-01-01 00:00:00.000000 arclet_alconna_ariadne-0.14.3/PKG-INFO
```

### Comparing `arclet_alconna_ariadne-0.14.2/LICENSE` & `arclet_alconna_ariadne-0.14.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet_alconna_ariadne-0.14.2/README.md` & `arclet_alconna_ariadne-0.14.3/README.md`

 * *Files identical despite different names*

### Comparing `arclet_alconna_ariadne-0.14.2/pyproject.toml` & `arclet_alconna_ariadne-0.14.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arclet-alconna-ariadne"
-version = "0.14.2"
+version = "0.14.3"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "graia-ariadne<1.0.0,>=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -29,17 +29,17 @@
 
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
@@ -59,15 +59,15 @@
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
@@ -111,20 +111,20 @@
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
     "graia-ariadne<1.0.0,>=0.7.14",
 ]
 description = "Support Alconna to GraiaProject/Ariadne"
@@ -152,20 +152,20 @@
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
@@ -194,20 +194,20 @@
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

### Comparing `arclet_alconna_ariadne-0.14.2/src/arclet/alconna/ariadne/adapter.py` & `arclet_alconna_ariadne-0.14.3/src/arclet/alconna/ariadne/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 AlconnaDispatcher.default_send_handler = lambda _, x: MessageChain([Plain(x)])
 Sender = Union[Friend, Member, Stranger, Client]
 
 
 class AlconnaAriadneAdapter(AlconnaGraiaAdapter[MessageEvent]):
     def completion_waiter(self, source: MessageEvent, priority: int = 15) -> Waiter:
         async def waiter(m: MessageChain, sender: Sender):
-            if sender.id == source.sender.id:
+            if isinstance(sender, source.sender.__class__) and sender.id == source.sender.id:
                 return m
 
         return FunctionWaiter(waiter, [source.__class__], block_propagation=True, priority=priority)
 
     async def lookup_source(self, interface: DispatcherInterface[MessageEvent]) -> MessageChain:
         return await interface.lookup_param("__message_chain__", MessageChain, MessageChain("Unknown"))
 
@@ -93,16 +93,15 @@
     def handle_listen(
         self,
         func: Callable,
         buffer: dict[str, Any],
         dispatcher: BaseDispatcher | None,
         guild: bool,
         private: bool,
-        private_name: str,
-        guild_name: str
+        **kwargs,
     ) -> None:
         events = []
         if guild:
             events.append(GroupMessage)
         if private:
             events.append(FriendMessage)
         buffer.setdefault("dispatchers", [])
```

### Comparing `arclet_alconna_ariadne-0.14.2/src/arclet/alconna/ariadne/typings.py` & `arclet_alconna_ariadne-0.14.3/src/arclet/alconna/ariadne/typings.py`

 * *Files identical despite different names*

### Comparing `arclet_alconna_ariadne-0.14.2/PKG-INFO` & `arclet_alconna_ariadne-0.14.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arclet-alconna-ariadne
-Version: 0.14.2
+Version: 0.14.3
 Summary: Support Alconna to GraiaProject/Ariadne
 Keywords: alconna graia arclet
 Home-page: https://github.com/ArcletProject/Alconna-Graia
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: AGPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

