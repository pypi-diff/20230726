# Comparing `tmp/nonebot_plugin_ncm-1.6.1.tar.gz` & `tmp/nonebot_plugin_ncm-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ncm-1.6.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_ncm-1.6.2.tar", max compression
```

## Comparing `nonebot_plugin_ncm-1.6.1.tar` & `nonebot_plugin_ncm-1.6.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-07-24 00:01:57.558888 nonebot_plugin_ncm-1.6.1/LICENSE
--rw-r--r--   0        0        0     4733 2023-07-24 00:01:57.558888 nonebot_plugin_ncm-1.6.1/README.md
--rw-r--r--   0        0        0    14194 2023-07-24 00:01:57.558888 nonebot_plugin_ncm-1.6.1/nonebot-plugin-ncm/__init__.py
--rw-r--r--   0        0        0      734 2023-07-24 00:01:57.558888 nonebot_plugin_ncm-1.6.1/nonebot-plugin-ncm/config.py
--rw-r--r--   0        0        0    12800 2023-07-24 00:01:57.558888 nonebot_plugin_ncm-1.6.1/nonebot-plugin-ncm/data_source.py
--rw-r--r--   0        0        0      859 2023-07-24 00:01:57.558888 nonebot_plugin_ncm-1.6.1/pyproject.toml
--rw-r--r--   0        0        0     5890 1970-01-01 00:00:00.000000 nonebot_plugin_ncm-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-25 23:54:28.856732 nonebot_plugin_ncm-1.6.2/LICENSE
+-rw-r--r--   0        0        0     4733 2023-07-25 23:54:28.856732 nonebot_plugin_ncm-1.6.2/README.md
+-rw-r--r--   0        0        0    13477 2023-07-25 23:54:28.856732 nonebot_plugin_ncm-1.6.2/nonebot-plugin-ncm/__init__.py
+-rw-r--r--   0        0        0      734 2023-07-25 23:54:28.856732 nonebot_plugin_ncm-1.6.2/nonebot-plugin-ncm/config.py
+-rw-r--r--   0        0        0    12800 2023-07-25 23:54:28.856732 nonebot_plugin_ncm-1.6.2/nonebot-plugin-ncm/data_source.py
+-rw-r--r--   0        0        0      859 2023-07-25 23:54:28.856732 nonebot_plugin_ncm-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5890 1970-01-01 00:00:00.000000 nonebot_plugin_ncm-1.6.2/PKG-INFO
```

### Comparing `nonebot_plugin_ncm-1.6.1/LICENSE` & `nonebot_plugin_ncm-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ncm-1.6.1/README.md` & `nonebot_plugin_ncm-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ncm-1.6.1/nonebot-plugin-ncm/__init__.py` & `nonebot_plugin_ncm-1.6.2/nonebot-plugin-ncm/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,49 +14,28 @@
 from nonebot.matcher import Matcher
 from nonebot.params import CommandArg, RegexGroup, Arg
 from nonebot.rule import Rule
 from pydantic.main import BaseModel
 
 from .data_source import nncm, ncm_config, setting, Q, cmd
 from .config import Config
+from nonebot.plugin import PluginMetadata
 
-# =======nonebot-plugin-help=======
-@dataclass(eq=False)
-class PluginMetadata:
-    """插件元信息，由插件编写者提供"""
-
-    name: str = "网易云无损音乐下载",
-    """插件名称"""
-    description: str = "✨ 基于go-cqhttp与nonebot2的 网易云 无损音乐下载 ✨",
-    """插件功能介绍"""
-    usage: str = (
+__plugin_meta__ = PluginMetadata(
+    name="网易云无损音乐下载",
+    description="基于go-cqhttp与nonebot2的 网易云无损音乐下载",
+    usage=(
         '将网易云歌曲/歌单分享到群聊即可自动解析\n'
-        '回复分享消息 + 文字`下载` 即可开始下载歌曲并上传到群文件(需要稍等一会)\n'
-        '指令：\n'
-        f'开启下载：{cmd}ncm t\n'
-        f'关闭下载：{cmd}ncm f\n'
-        f'点歌：{cmd}点歌 歌名'
-    )
-    """插件使用方法"""
-    type: Optional[str] = "application"
-    """插件类型，用于商店分类"""
-    homepage: Optional[str] = "https://github.com/kitUIN/nonebot-plugin-ncm"
-    """插件主页"""
-    config: Optional[Type[BaseModel]] = Config
-    """插件配置项"""
-    supported_adapters: Optional[Set[str]] = {"nonebot.adapters.onebot.v11"},
-    """插件支持的适配器模块路径
-
-    格式为 `<module>[:<Adapter>]`，`~` 为 `nonebot.adapters.` 的缩写。
-
-    `None` 表示支持**所有适配器**。
-    """
-
-
-__plugin_meta__ = PluginMetadata(...)
+        '回复分享消息 + 文字`下载` 即可开始下载歌曲并上传到群文件(需要稍等一会)'
+    ),
+    config=Config,
+    type="application",
+    homepage="https://github.com/kitUIN/nonebot-plugin-ncm",
+    supported_adapters={"~onebot.v11"},
+)
 # ========nonebot-plugin-ncm======
 # ===========Constant=============
 TRUE = ["True", "T", "true", "t"]
 FALSE = ["False", "F", "false", "f"]
 ADMIN = ["owner", "admin", "member"]
```

### Comparing `nonebot_plugin_ncm-1.6.1/nonebot-plugin-ncm/config.py` & `nonebot_plugin_ncm-1.6.2/nonebot-plugin-ncm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ncm-1.6.1/nonebot-plugin-ncm/data_source.py` & `nonebot_plugin_ncm-1.6.2/nonebot-plugin-ncm/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ncm-1.6.1/pyproject.toml` & `nonebot_plugin_ncm-1.6.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-ncm"
-version = "1.6.1"
+version = "1.6.2"
 description = "基于go-cqhttp与nonebot2的 网易云 无损音乐下载"
 license = "Apache License 2.0"
 authors = ["kitUIN <kulujun@gmail.com>"]
 maintainers = ["kitUIN <kulujun@gmail.com>", "Kurokitu"]
 readme = "README.md"
 packages = [
     { include = "nonebot-plugin-ncm" }
```

### Comparing `nonebot_plugin_ncm-1.6.1/PKG-INFO` & `nonebot_plugin_ncm-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ncm
-Version: 1.6.1
+Version: 1.6.2
 Summary: 基于go-cqhttp与nonebot2的 网易云 无损音乐下载
 Home-page: https://github.com/kitUIN/nonebot-plugin-ncm
 License: Apache-2.0
 Keywords: netease-cloud-music,netease,go-cqhttp,nonebot2
 Author: kitUIN
 Author-email: kulujun@gmail.com
 Maintainer: kitUIN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ncm Version: 1.6.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-ncm Version: 1.6.2 Summary:
 åºäºgo-cqhttpä¸nonebot2ç ç½æäº æ æé³ä¹ä¸è½½ Home-page: https://
 github.com/kitUIN/nonebot-plugin-ncm License: Apache-2.0 Keywords: netease-
 cloud-music,netease,go-cqhttp,nonebot2 Author: kitUIN Author-email:
 kulujun@gmail.com Maintainer: kitUIN Maintainer-email: kulujun@gmail.com
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

