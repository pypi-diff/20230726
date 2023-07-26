# Comparing `tmp/nonebot_plugin_templates-0.1.4.tar.gz` & `tmp/nonebot_plugin_templates-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_templates-0.1.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_templates-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_templates-0.1.4.tar` & `nonebot_plugin_templates-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      397 2023-07-18 03:49:45.298270 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/__init__.py
--rw-r--r--   0        0        0     5861 2023-07-18 02:38:35.241359 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/template_types.py
--rw-r--r--   0        0        0     4545 2023-07-18 02:38:35.327079 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/cards.html
--rw-r--r--   0        0        0     4336 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/colorlist.html
--rw-r--r--   0        0        0     3623 2023-07-24 06:56:16.187282 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/menus.html
--rw-r--r--   0        0        0 10968356 2023-07-18 02:38:35.327079 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/PingFang.ttf
--rw-r--r--   0        0        0     6543 2023-07-18 02:38:35.328078 nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates_render.py
--rw-r--r--   0        0        0      471 2023-07-24 06:56:16.183277 nonebot_plugin_templates-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3449 2023-07-18 04:01:13.672237 nonebot_plugin_templates-0.1.4/README.md
--rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 nonebot_plugin_templates-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      397 2023-07-24 07:00:05.108193 nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/__init__.py
+-rw-r--r--   0        0        0     5861 2023-07-24 07:00:05.108193 nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/template_types.py
+-rw-r--r--   0        0        0     4545 2023-07-24 07:00:05.109196 nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates/cards.html
+-rw-r--r--   0        0        0     4336 2023-07-24 07:00:05.109196 nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates/colorlist.html
+-rw-r--r--   0        0        0     2210 2023-07-26 06:36:50.774160 nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates/grid.html
+-rw-r--r--   0        0        0     3623 2023-07-24 07:00:05.110255 nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates/menus.html
+-rw-r--r--   0        0        0 10968356 2023-07-24 07:00:05.174372 nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates/PingFang.ttf
+-rw-r--r--   0        0        0     7621 2023-07-26 06:37:55.318591 nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates_render.py
+-rw-r--r--   0        0        0      471 2023-07-26 07:19:01.740454 nonebot_plugin_templates-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3449 2023-07-18 04:01:13.672237 nonebot_plugin_templates-0.1.5/README.md
+-rw-r--r--   0        0        0     4007 1970-01-01 00:00:00.000000 nonebot_plugin_templates-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/template_types.py` & `nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/template_types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/cards.html` & `nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates/cards.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/colorlist.html` & `nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates/colorlist.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/menus.html` & `nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates/menus.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates/PingFang.ttf` & `nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates/PingFang.ttf`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.4/nonebot_plugin_templates/templates_render.py` & `nonebot_plugin_templates-0.1.5/nonebot_plugin_templates/templates_render.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from pathlib import Path
 from typing import Optional
 
 from nonebot import require
 
 from nonebot_plugin_templates.template_types import *
 
@@ -17,56 +18,59 @@
     loader=FileSystemLoader(str(Path(__file__).parent / "templates")),
     enable_async=True,
 )
 
 COLORLIST_TEMPLATE = env.get_template("colorlist.html")
 MENUS_TEMPLATE = env.get_template("menus.html")
 CARD_TEMPLATE = env.get_template("cards.html")
+GRID_TEMPLATE = env.get_template("grid.html")
 
 Font_Path = (TEMPLATES_PATH / "PingFang.ttf").as_uri()
 
 
 async def colorlist_render(
-        _list: dict,
-        width: int,
-        headline: str = "列表",
-        description: str = "🌈列表",
-        font_size: int = 15,
-        font_path: str = Font_Path
+    _list: dict,
+    width: int,
+    headline: str = "列表",
+    description: str = "🌈列表",
+    font_size: int = 15,
+    font_path: str = Font_Path,
 ) -> bytes:
-    """ 函数名：colorlist_render
+    """函数名：colorlist_render
 
-        功能：该函数用于生成一张带有颜色列表的图片。
+    功能：该函数用于生成一张带有颜色列表的图片。
 
-        参数：
-            _list: 字典类型的列表，其中键为字符串，值为颜色代码。
-                {
-                "line1 name":"description of line1",
-                "line2 name":"description of line1"
-                }
-            width: 图片的宽度。
-            headline: 列表的标题，默认值为"列表"。
-            description: 列表的描述，默认值为"🌈列表"。
-            font_size: 字体大小，默认值为15。
-            font_path: 字体文件的路径，默认值为Font_Path。
-
-        返回值:
-            该函数返回彩色列表的图片bytes。
-        """
+    参数：
+        _list: 字典类型的列表，其中键为字符串，值为颜色代码。
+            {
+            "line1 name":"description of line1",
+            "line2 name":"description of line1"
+            }
+        width: 图片的宽度。
+        headline: 列表的标题，默认值为"列表"。
+        description: 列表的描述，默认值为"🌈列表"。
+        font_size: 字体大小，默认值为15。
+        font_path: 字体文件的路径，默认值为Font_Path。
+
+    返回值:
+        该函数返回彩色列表的图片bytes。
+    """
     html = await COLORLIST_TEMPLATE.render_async(
         headline=headline,
         list=_list,
         description=description,
         font_path=font_path,
         font_size=font_size,
     )
     return await html_to_pic(html, viewport={"width": width, "height": 10})
 
 
-async def menu_render(menus: Menus, width: int, colors: Optional[dict] = None, font_path: str = Font_Path) -> bytes:
+async def menu_render(
+    menus: Menus, width: int, colors: Optional[dict] = None, font_path: str = Font_Path
+) -> bytes:
     """
     函数：menu_render
 
     功能：该函数将菜单对象渲染成图片格式，以便于展示。
 
     参数：
     - menus: Menus对象，表示需要渲染的菜单对象。
@@ -96,16 +100,22 @@
         }
     html = await MENUS_TEMPLATE.render_async(
         menus=menus.to_dict(), colors=colors, font_path=font_path
     )
     return await html_to_pic(html, viewport={"width": width, "height": 10})
 
 
-async def cardlist_render(title: str, cards: Cards, subtitle: str = "", width: int = 500, colors: Optional[dict] = None,
-                          font_path: str = Font_Path) -> bytes:
+async def cardlist_render(
+    title: str,
+    cards: Cards,
+    subtitle: str = "",
+    width: int = 500,
+    colors: Optional[dict] = None,
+    font_path: str = Font_Path,
+) -> bytes:
     """
     函数：cardlist_render
 
     功能：渲染一个带有标题和可选子标题的卡片列表图片。
 
     参数：
 
@@ -126,17 +136,57 @@
     font_path (str)：用于渲染文本的字体文件的路径（默认为 Font_Path）。
 
     返回值：
 
     bytes：包含卡片列表渲染图像的 bytes 对象,可直接发送。
     """
     if colors is None:
-        colors = {"html": "#f3f3f3",  # 整体页面最底层的背景颜色
-                  "body_border": "#ffffff",  # 最外面的边框的的背景颜色
-                  "card_header": "#E5F3F9",  # 卡片的标题栏的背景颜色
-                  "card-body": "#ffffff",  # 卡片主体的颜色
-                  "index_text": "#FFFFFF",  # 数字索引的文本颜色
-                  "index_bg": "#8D3C1E",  # 数字索引的圆形背景颜色
-                  }
-    html = await CARD_TEMPLATE.render_async(title=title, cards=cards.to_dict(), subtitle=subtitle, colors=colors,
-                                            font_path=font_path)
+        colors = {
+            "html": "#f3f3f3",  # 整体页面最底层的背景颜色
+            "body_border": "#ffffff",  # 最外面的边框的的背景颜色
+            "card_header": "#E5F3F9",  # 卡片的标题栏的背景颜色
+            "card-body": "#ffffff",  # 卡片主体的颜色
+            "index_text": "#FFFFFF",  # 数字索引的文本颜色
+            "index_bg": "#8D3C1E",  # 数字索引的圆形背景颜色
+        }
+    html = await CARD_TEMPLATE.render_async(
+        title=title,
+        cards=cards.to_dict(),
+        subtitle=subtitle,
+        colors=colors,
+        font_path=font_path,
+    )
+    return await html_to_pic(html, viewport={"width": width, "height": 10})
+
+
+async def dict_render(
+    data: dict,
+    width: int = 400,
+    title: str = "表格",
+    font_path: str = Font_Path,
+    colors: dict = {},
+) -> bytes:
+    """函数名：colorlist_render
+
+    功能：该函数用于生成一张带有颜色列表的图片。
+
+    参数：
+        data:要转图片的dict
+        width:如片宽度
+        title:图片标题
+        key_tile:dict的键
+
+    返回值:
+        该函数返回彩色列表的图片bytes。
+    """
+    if not colors:
+        colors = {
+            "html_bg": "#d9d9d9",  # 整体背景颜色
+            "key": "#E5F3F9",  # 键所在的块的颜色
+            "value": "#ffffff",  # 值所在的块的背景颜色
+            "func_index_text": "#FFFFFF",  # 命令前的索引的数字的颜色
+            "func_index_bg": "#8D3C1E",  # 命令前的索引的数字的圆形背景颜色
+        }
+    html = await GRID_TEMPLATE.render_async(
+        title=title, font_path=font_path, data=data, colors=colors
+    )
     return await html_to_pic(html, viewport={"width": width, "height": 10})
```

### Comparing `nonebot_plugin_templates-0.1.4/README.md` & `nonebot_plugin_templates-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_templates-0.1.4/PKG-INFO` & `nonebot_plugin_templates-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-templates
-Version: 0.1.4
+Version: 0.1.5
 Summary: 为nonebot提供一系列jinja2 template模板,方便的生成图片
 Author: canxin
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-templates Version: 0.1.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-templates Version: 0.1.5 Summary:
 ä¸ºnonebotæä¾ä¸ç³»åjinja2 templateæ¨¡æ¿,æ¹ä¾¿ççæå¾ç Author:
 canxin Author-email: 1969730106@qq.com Requires-Python: >=3.8,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.1,<0.3.0)
 Requires-Dist: nonebot2 (>=2.0.0,<3.0.0) Description-Content-Type: text/
```

