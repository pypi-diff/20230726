# Comparing `tmp/nonebot_plugin_datastore-1.0.0.tar.gz` & `tmp/nonebot_plugin_datastore-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_datastore-1.0.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_datastore-1.1.0.tar", max compression
```

## Comparing `nonebot_plugin_datastore-1.0.0.tar` & `nonebot_plugin_datastore-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/LICENSE
--rw-r--r--   0        0        0     7564 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/README.md
--rw-r--r--   0        0        0      572 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/__init__.py
--rw-r--r--   0        0        0     1772 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/config.py
--rw-r--r--   0        0        0     4093 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/db.py
--rw-r--r--   0        0        0      804 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py
--rw-r--r--   0        0        0     8844 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/plugin.py
--rw-r--r--   0        0        0     1487 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/__init__.py
--rw-r--r--   0        0        0     1226 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/database.py
--rw-r--r--   0        0        0     1530 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/json.py
--rw-r--r--   0        0        0     1635 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/toml.py
--rw-r--r--   0        0        0     1816 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/yaml.py
--rw-r--r--   0        0        0        0 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/py.typed
--rw-r--r--   0        0        0        0 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/__init__.py
--rw-r--r--   0        0        0     6372 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/cli.py
--rw-r--r--   0        0        0    12170 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/command.py
--rw-r--r--   0        0        0      510 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/migration/script.py.mako
--rw-r--r--   0        0        0     3611 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/utils.py
--rw-r--r--   0        0        0     1889 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/utils.py
--rw-r--r--   0        0        0     2075 2023-06-06 15:04:46.726860 nonebot_plugin_datastore-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8989 1970-01-01 00:00:00.000000 nonebot_plugin_datastore-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/LICENSE
+-rw-r--r--   0        0        0     8721 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/README.md
+-rw-r--r--   0        0        0      572 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/__init__.py
+-rw-r--r--   0        0        0     1772 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/config.py
+-rw-r--r--   0        0        0     4093 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/db.py
+-rw-r--r--   0        0        0      804 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py
+-rw-r--r--   0        0        0    10051 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/plugin.py
+-rw-r--r--   0        0        0     1487 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/providers/__init__.py
+-rw-r--r--   0        0        0     1226 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/providers/database.py
+-rw-r--r--   0        0        0     1530 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/providers/json.py
+-rw-r--r--   0        0        0     1635 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/providers/toml.py
+-rw-r--r--   0        0        0     1816 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/providers/yaml.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/py.typed
+-rw-r--r--   0        0        0        0 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/script/__init__.py
+-rw-r--r--   0        0        0     6372 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/script/cli.py
+-rw-r--r--   0        0        0    12168 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/script/command.py
+-rw-r--r--   0        0        0      510 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/script/migration/script.py.mako
+-rw-r--r--   0        0        0     4046 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/script/utils.py
+-rw-r--r--   0        0        0     1889 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/utils.py
+-rw-r--r--   0        0        0     2054 2023-07-26 09:40:44.668606 nonebot_plugin_datastore-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10126 1970-01-01 00:00:00.000000 nonebot_plugin_datastore-1.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_datastore-1.0.0/LICENSE` & `nonebot_plugin_datastore-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/README.md` & `nonebot_plugin_datastore-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -177,14 +177,43 @@
 
 详细介绍可查看 `SQLAlchemy` 文档的 [dealing-with-disconnects](https://docs.sqlalchemy.org/en/20/core/pooling.html#dealing-with-disconnects) 章节。
 
 ### SQLite 数据库已锁定
 
 使用 `SQLite` 数据库时，如果在写入时遇到 `(sqlite3.OperationalError) database is locked` 错误。可尝试将 `poolclass` 设置为 `StaticPool`，保持有且仅有一个连接。不过这样设置之后，在程序运行期间，你的数据库文件都将被占用。
 
+### 不同插件间表的关联关系
+
+datastore 默认会给每个插件的 Base 模型提供独立的 registry，所以不同插件间的表无法建立关联关系。如果你需要与其他插件的表建立关联关系，请在需要关联的两个插件中都调用 use_global_registry 函数使用全局 registry。
+
+```python
+# 定义模型
+db = get_plugin_data()
+db.use_global_registry()
+
+class Example(db.Model):
+    """实例函数"""
+
+    id: Mapped[int] = mapped_column(primary_key=True)
+    message: Mapped[str]
+
+    tests: Mapped["Test"] = relationship(back_populates="example")
+
+
+class Test(db.Model):
+    id: Mapped[int] = mapped_column(primary_key=True)
+
+    example_id: Mapped[int] = mapped_column(ForeignKey("plugin_example.id"))
+    example: Mapped[Example] = relationship(back_populates="tests")
+
+# 注意，为了避免不同插件的模型同名而报错，请一定要加上这一行，避免如下报错
+# sqlalchemy.exc.InvalidRequestError: Multiple classes found for path "Test" in the registry of this declarative base. Please use a fully module-qualified path.
+Example.tests = relationship(Test, back_populates="example")
+```
+
 ## 配置项
 
 配置方式：直接在 `NoneBot` 全局配置文件中添加以下配置项即可。
 
 ### datastore_cache_dir
 
 - 类型: `Path`
```

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/__init__.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/config.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/db.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/migrations/0f8d23241fd7_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/plugin.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,25 +97,28 @@
 class PluginData(metaclass=Singleton):
     """插件数据管理
 
     将插件数据保存在 `data` 文件夹对应的目录下。
     提供保存和读取文件/数据的方法。
     """
 
+    global_registry = registry()
+
     def __init__(self, name: str) -> None:
         # 插件名，用来确定插件的文件夹位置
         self.name = name
 
         # 插件配置
         self._config = None
 
         # 数据库
         self._metadata = None
         self._model = None
         self._migration_path = None
+        self._use_global_registry = False
 
     @staticmethod
     def _ensure_dir(path: Path):
         """确保目录存在"""
         if not path.exists():
             path.mkdir(parents=True, exist_ok=True)
         elif not path.is_dir():
@@ -222,36 +225,51 @@
         return NetworkFile[T, R](url, filename, self, process_data, cache)
 
     @property
     def Model(self) -> Type[DeclarativeBase]:
         """数据库模型"""
         if self._model is None:
             self._metadata = MetaData(info={"name": self.name})
-
-            # 为每个插件创建一个独立的 registry
-            plugin_registry = registry(metadata=self._metadata)
+            if self._use_global_registry:
+                plugin_registry = self.global_registry
+            else:
+                # 为每个插件创建一个独立的 registry
+                plugin_registry = registry(metadata=self._metadata)
 
             class _Base(DeclarativeBase):
                 registry = plugin_registry
 
                 @declared_attr.directive
                 def __tablename__(cls) -> str:
                     """设置表名前缀，避免表名冲突
 
                     规则为：插件名_表名
                     https://docs.sqlalchemy.org/en/20/orm/declarative_mixins.html#augmenting-the-base
                     """
-                    return f"{self.name}_{cls.__name__.lower()}"
+                    table_name = f"{self.name}_{cls.__name__.lower()}"
+                    if self._use_global_registry:
+                        # 如果使用全局 registry，则需要在 metadata 中记录表名和插件名的对应关系
+                        # 因为所有插件共用一个 metadata，没法通过 metadata.name 指定插件名
+                        if plugin_name_map := cls.metadata.info.get("plugin_name_map"):
+                            plugin_name_map[table_name] = self.name
+                        else:
+                            cls.metadata.info["plugin_name_map"] = {
+                                table_name: self.name
+                            }
+
+                    return table_name
 
             self._model = _Base
         return self._model
 
     @property
     def metadata(self) -> Optional[MetaData]:
         """获取数据库元数据"""
+        if self._use_global_registry:
+            return self.global_registry.metadata
         return self._metadata
 
     @property
     def migration_dir(self) -> Optional[Path]:
         """数据库迁移文件夹"""
         if self._migration_path is None:
             plugin = get_plugin(self.name)
@@ -261,14 +279,22 @@
                 )
         return self._migration_path
 
     def set_migration_dir(self, path: Path) -> None:
         """设置数据库迁移文件夹"""
         self._migration_path = path
 
+    def use_global_registry(self):
+        """使用全局的 registry
+
+        请在获取 Model 之前调用此方法
+        用于解决多个插件模型互相关联时的问题，请谨慎启用
+        """
+        self._use_global_registry = True
+
 
 def get_plugin_data(name: Optional[str] = None) -> PluginData:
     """获取插件数据
 
     如果名称为空，则尝试自动获取调用者所在的插件名
     """
     name = name or get_caller_plugin_name()
```

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/__init__.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/database.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/providers/database.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/json.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/providers/json.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/toml.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/providers/toml.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/providers/yaml.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/providers/yaml.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/cli.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/script/cli.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/command.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/script/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,15 +145,15 @@
     if len(scripts) == 1:
         return scripts[0]
     else:
         return scripts
 
 
 async def check(
-    config: "Config",
+    config: Config,
 ) -> None:
     """Check if revision command with autogenerate has pending upgrade ops.
 
     :param config: a :class:`.Config` object.
 
     .. versionadded:: 1.9.0
```

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/script/utils.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/script/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,19 +78,33 @@
         if config.cmd_opts and config.cmd_opts.autogenerate:
             script = directives[0]
             if script.upgrade_ops.is_empty():
                 logger.info("模型未发生变化，已跳过生成迁移文件")
                 directives[:] = []
 
     def include_object(object, name, type_, reflected, compare_to):
-        if type_ == "table" and object.metadata.info.get("name") != plugin_name:
+        if type_ != "table":
             return False
-        else:
+
+        table_info_name = object.metadata.info.get("name")
+        # 因为所有插件共用一个 metadata
+        # 通过存放在 metadata.info 中的 plugin_name_map 判断是否为当前插件的表
+        if (
+            table_info_name is None
+            and target_metadata
+            and target_metadata.info.get("plugin_name_map", {}).get(object.fullname)
+            == plugin_name
+        ):
+            return True
+
+        if table_info_name == plugin_name:
             return True
 
+        return False
+
     context.configure(
         connection=connection,
         target_metadata=target_metadata,
         version_table=f"{plugin_name}_alembic_version",
         include_object=include_object,
         process_revision_directives=process_revision_directives,
         render_as_batch=True,
```

### Comparing `nonebot_plugin_datastore-1.0.0/nonebot_plugin_datastore/utils.py` & `nonebot_plugin_datastore-1.1.0/nonebot_plugin_datastore/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_datastore-1.0.0/pyproject.toml` & `nonebot_plugin_datastore-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "nonebot-plugin-datastore"
-version = "1.0.0"
+version = "1.1.0"
 description = "适用于 Nonebot2 的数据存储插件"
 authors = ["hemengyang <hmy0119@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/he0119/nonebot-plugin-datastore"
 repository = "https://github.com/he0119/nonebot-plugin-datastore"
 documentation = "https://github.com/he0119/nonebot-plugin-datastore#readme"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = { extras = ["httpx"], version = "^2.0.0" }
-nonebot-plugin-localstore = ">=0.2.0,!=0.3.0,!=0.4.0,<0.6.0"
+nonebot-plugin-localstore = ">=0.2.0,!=0.3.0,!=0.4.0"
 sqlalchemy = { extras = ["aiosqlite"], version = "^2.0.0" }
 alembic = "^1.9.1"
 
 anyio = { version = ">=3.6", optional = true }
 click = { version = ">=8.0", optional = true }
 typing-extensions = { version = ">=4.4", optional = true }
-rtoml = { version = "^0.9.0", optional = true }
-pyyaml = { version = "^6.0", optional = true }
+rtoml = { version = ">=0.9.0", optional = true }
+pyyaml = { version = ">=6.0", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
 pre-commit = "*"
 nonebug = "^0.3.1"
 pytest-cov = "^4.0.0"
@@ -67,12 +67,12 @@
 omit = ["*/script/command.py", "*/migrations/*"]
 
 [tool.poetry.plugins.nb_scripts]
 datastore = "nonebot_plugin_datastore.script.cli:main"
 
 [tool.nonebot]
 plugins = ["nonebot_plugin_datastore"]
-plugin_dirs = ["tests/registry"]
+plugin_dirs = []
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_datastore-1.0.0/PKG-INFO` & `nonebot_plugin_datastore-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-datastore
-Version: 1.0.0
+Version: 1.1.0
 Summary: 适用于 Nonebot2 的数据存储插件
 Home-page: https://github.com/he0119/nonebot-plugin-datastore
 License: MIT
 Author: hemengyang
 Author-email: hmy0119@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,18 +16,18 @@
 Provides-Extra: all
 Provides-Extra: cli
 Provides-Extra: toml
 Provides-Extra: yaml
 Requires-Dist: alembic (>=1.9.1,<2.0.0)
 Requires-Dist: anyio (>=3.6) ; extra == "cli" or extra == "all"
 Requires-Dist: click (>=8.0) ; extra == "cli" or extra == "all"
-Requires-Dist: nonebot-plugin-localstore (>=0.2.0,!=0.3.0,!=0.4.0,<0.6.0)
+Requires-Dist: nonebot-plugin-localstore (>=0.2.0,!=0.3.0,!=0.4.0)
 Requires-Dist: nonebot2[httpx] (>=2.0.0,<3.0.0)
-Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml" or extra == "all"
-Requires-Dist: rtoml (>=0.9.0,<0.10.0) ; extra == "toml" or extra == "all"
+Requires-Dist: pyyaml (>=6.0) ; extra == "yaml" or extra == "all"
+Requires-Dist: rtoml (>=0.9.0) ; extra == "toml" or extra == "all"
 Requires-Dist: sqlalchemy[aiosqlite] (>=2.0.0,<3.0.0)
 Requires-Dist: typing-extensions (>=4.4) ; extra == "cli" or extra == "all"
 Project-URL: Documentation, https://github.com/he0119/nonebot-plugin-datastore#readme
 Project-URL: Repository, https://github.com/he0119/nonebot-plugin-datastore
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD033 MD036 MD041 -->
@@ -209,14 +209,43 @@
 
 详细介绍可查看 `SQLAlchemy` 文档的 [dealing-with-disconnects](https://docs.sqlalchemy.org/en/20/core/pooling.html#dealing-with-disconnects) 章节。
 
 ### SQLite 数据库已锁定
 
 使用 `SQLite` 数据库时，如果在写入时遇到 `(sqlite3.OperationalError) database is locked` 错误。可尝试将 `poolclass` 设置为 `StaticPool`，保持有且仅有一个连接。不过这样设置之后，在程序运行期间，你的数据库文件都将被占用。
 
+### 不同插件间表的关联关系
+
+datastore 默认会给每个插件的 Base 模型提供独立的 registry，所以不同插件间的表无法建立关联关系。如果你需要与其他插件的表建立关联关系，请在需要关联的两个插件中都调用 use_global_registry 函数使用全局 registry。
+
+```python
+# 定义模型
+db = get_plugin_data()
+db.use_global_registry()
+
+class Example(db.Model):
+    """实例函数"""
+
+    id: Mapped[int] = mapped_column(primary_key=True)
+    message: Mapped[str]
+
+    tests: Mapped["Test"] = relationship(back_populates="example")
+
+
+class Test(db.Model):
+    id: Mapped[int] = mapped_column(primary_key=True)
+
+    example_id: Mapped[int] = mapped_column(ForeignKey("plugin_example.id"))
+    example: Mapped[Example] = relationship(back_populates="tests")
+
+# 注意，为了避免不同插件的模型同名而报错，请一定要加上这一行，避免如下报错
+# sqlalchemy.exc.InvalidRequestError: Multiple classes found for path "Test" in the registry of this declarative base. Please use a fully module-qualified path.
+Example.tests = relationship(Test, back_populates="example")
+```
+
 ## 配置项
 
 配置方式：直接在 `NoneBot` 全局配置文件中添加以下配置项即可。
 
 ### datastore_cache_dir
 
 - 类型: `Path`
```

