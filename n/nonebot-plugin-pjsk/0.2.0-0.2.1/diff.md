# Comparing `tmp/nonebot_plugin_pjsk-0.2.0.tar.gz` & `tmp/nonebot_plugin_pjsk-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_pjsk-0.2.0.tar", last modified: Tue Jul 25 16:07:35 2023, max compression
+gzip compressed data, was "nonebot_plugin_pjsk-0.2.1.tar", last modified: Wed Jul 26 16:22:00 2023, max compression
```

## Comparing `nonebot_plugin_pjsk-0.2.0.tar` & `nonebot_plugin_pjsk-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-07-25 16:07:15.896097 nonebot_plugin_pjsk-0.2.0/LICENSE
--rw-r--r--   0        0        0     3412 2023-07-25 16:07:15.896097 nonebot_plugin_pjsk-0.2.0/README.md
--rw-r--r--   0        0        0      765 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/__init__.py
--rw-r--r--   0        0        0     4607 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/__main__.py
--rw-r--r--   0        0        0      695 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/config.py
--rw-r--r--   0        0        0     6410 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/draw.py
--rw-r--r--   0        0        0     3553 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/resource.py
--rw-r--r--   0        0        0     2460 2023-07-25 16:07:15.964097 nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/utils.py
--rw-r--r--   0        0        0     1086 2023-07-25 16:07:35.972062 nonebot_plugin_pjsk-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-26 16:21:44.002201 nonebot_plugin_pjsk-0.2.1/LICENSE
+-rw-r--r--   0        0        0     3412 2023-07-26 16:21:44.002201 nonebot_plugin_pjsk-0.2.1/README.md
+-rw-r--r--   0        0        0      801 2023-07-26 16:21:44.062201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/__init__.py
+-rw-r--r--   0        0        0     6591 2023-07-26 16:21:44.062201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/__main__.py
+-rw-r--r--   0        0        0      695 2023-07-26 16:21:44.062201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/config.py
+-rw-r--r--   0        0        0     6407 2023-07-26 16:21:44.066201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/draw.py
+-rw-r--r--   0        0        0     3553 2023-07-26 16:21:44.066201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/resource.py
+-rw-r--r--   0        0        0     2423 2023-07-26 16:21:44.066201 nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/utils.py
+-rw-r--r--   0        0        0     1086 2023-07-26 16:22:00.370602 nonebot_plugin_pjsk-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4394 1970-01-01 00:00:00.000000 nonebot_plugin_pjsk-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_pjsk-0.2.0/LICENSE` & `nonebot_plugin_pjsk-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.0/README.md` & `nonebot_plugin_pjsk-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   <img src="https://img.shields.io/pypi/dm/nonebot-plugin-pjsk" alt="pypi download">
 </a>
 
 </div>
 
 ## 📖 介绍
 
-这里是插件的详细介绍部分
+![Wonderhoy](./readme/wonderhoy.png)
 
 ## 💿 安装
 
 以下提到的方法 任选**其一** 即可
 
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-PJSK _â¨ Project Sekai è¡¨æåå¶ä½ â¨_ [python] [pdm-
                            managed] [QQ_Chat_Group]
                        [license] [pypi] [pypi_download]
-## ð ä»ç» è¿éæ¯æä»¶çè¯¦ç»ä»ç»é¨å ## ð¿ å®è£
+## ð ä»ç» ![Wonderhoy](./readme/wonderhoy.png) ## ð¿ å®è£
 ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
 å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-pjsk
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-pjsk ```   pdm ```bash pdm add nonebot-
 plugin-pjsk ```   poetry ```bash poetry add nonebot-plugin-pjsk ```   conda
```

### Comparing `nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/__init__.py` & `nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from nonebot.plugin import PluginMetadata
 
 require("nonebot_plugin_saa")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __plugin_meta__ = PluginMetadata(
     name="Sekai Stickers",
     description="基于 NoneBot2 的 Project Sekai 表情包制作插件",
     usage="使用指令 `pjsk -h` 获取指令帮助",
     type="application",
     homepage="https://github.com/Agnes4m/nonebot_plugin_pjsk",
     config=ConfigModel,
@@ -19,10 +19,10 @@
         "~onebot.v12",
         "~kaiheila",
         "~qqguild",
         "~telegram",
     },
     extra={
         "version": __version__,
-        "author": "Agnes4m <Z735803792@163.com>",
+        "author": ["Agnes4m <Z735803792@163.com>", "student_2333 <lgc2333@126.com>"],
     },
 )
```

### Comparing `nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/config.py` & `nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/draw.py` & `nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
     text_lines = text.splitlines()
     padding = stoke_width
 
     actual_size = text_size_multiline(text_lines, font_size, font, line_spacing)
     size = (
         actual_size[0] + padding * 2,
-        actual_size[1] + padding * 2 + font_size // 2,  # 更多纵向 padding 防止文字被裁切
+        actual_size[1] + padding * 2 + font_size // 2,  # 更多纵向 padding 防止文字被裁
     )
 
     canvas = Canvas(*size, Color(255, 255, 255, 0))
     draw_text_multiline(
         canvas,
         text_lines,  # type: ignore 这里是源代码有问题
         size[0] // 2,
```

### Comparing `nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/resource.py` & `nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/resource.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_pjsk-0.2.0/nonebot_plugin_pjsk/utils.py` & `nonebot_plugin_pjsk-0.2.1/nonebot_plugin_pjsk/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,11 @@
 import math
 from asyncio import Semaphore
 from enum import Enum, auto
-from typing import (
-    Any,
-    Iterable,
-    List,
-    Literal,
-    Optional,
-    Type,
-    TypeVar,
-    overload,
-)
+from typing import Any, Iterable, List, Literal, Optional, Type, TypeVar, overload
 
 from httpx import AsyncClient
 
 from .config import config
 
 T = TypeVar("T")
 TN = TypeVar("TN", int, float)
```

### Comparing `nonebot_plugin_pjsk-0.2.0/pyproject.toml` & `nonebot_plugin_pjsk-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-pjsk"
-version = "0.2.0"
+version = "0.2.1"
 description = "Project Sekai Sticker Creator for NoneBot2."
 authors = [
     { name = "Agnes_Digital", email = "Z735803792@163.com" },
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0",
```

### Comparing `nonebot_plugin_pjsk-0.2.0/PKG-INFO` & `nonebot_plugin_pjsk-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-pjsk
-Version: 0.2.0
+Version: 0.2.1
 Summary: Project Sekai Sticker Creator for NoneBot2.
 Keywords: pjsk nonebot2 plugin
 Home-page: https://github.com/Agnes4m/nonebot_plugin_pjsk
 Author-Email: Agnes_Digital <Z735803792@163.com>, student_2333 <lgc2333@126.com>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -58,15 +58,15 @@
   <img src="https://img.shields.io/pypi/dm/nonebot-plugin-pjsk" alt="pypi download">
 </a>
 
 </div>
 
 ## 📖 介绍
 
-这里是插件的详细介绍部分
+![Wonderhoy](./readme/wonderhoy.png)
 
 ## 💿 安装
 
 以下提到的方法 任选**其一** 即可
 
 <details open>
 <summary>[推荐] 使用 nb-cli 安装</summary>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.0 Summary: Project
+Metadata-Version: 2.1 Name: nonebot-plugin-pjsk Version: 0.2.1 Summary: Project
 Sekai Sticker Creator for NoneBot2. Keywords: pjsk nonebot2 plugin Home-page:
 https://github.com/Agnes4m/nonebot_plugin_pjsk Author-Email: Agnes_Digital
 163.com>, student_2333
 126.com> License: MIT Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
@@ -13,15 +13,15 @@
 Requires-Dist: imagetext-py>=1.0.2 Requires-Dist: pil-utils>=0.1.7 Description-
 Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
  # NoneBot-Plugin-PJSK _â¨ Project Sekai è¡¨æåå¶ä½ â¨_ [python] [pdm-
                            managed] [QQ_Chat_Group]
                        [license] [pypi] [pypi_download]
-## ð ä»ç» è¿éæ¯æä»¶çè¯¦ç»ä»ç»é¨å ## ð¿ å®è£
+## ð ä»ç» ![Wonderhoy](./readme/wonderhoy.png) ## ð¿ å®è£
 ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£
 å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
 è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb plugin install nonebot-plugin-pjsk
 ```   ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-pjsk ```   pdm ```bash pdm add nonebot-
 plugin-pjsk ```   poetry ```bash poetry add nonebot-plugin-pjsk ```   conda
```

