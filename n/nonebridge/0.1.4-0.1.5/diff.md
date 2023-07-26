# Comparing `tmp/nonebridge-0.1.4.tar.gz` & `tmp/nonebridge-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebridge-0.1.4.tar", max compression
+gzip compressed data, was "nonebridge-0.1.5.tar", max compression
```

## Comparing `nonebridge-0.1.4.tar` & `nonebridge-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1070 2023-01-17 13:24:41.053089 nonebridge-0.1.4/LICENSE
--rw-r--r--   0        0        0     2757 2023-01-17 13:24:41.053089 nonebridge-0.1.4/README.md
--rw-r--r--   0        0        0    18978 2023-01-17 13:24:41.053089 nonebridge-0.1.4/nonebridge/__init__.py
--rw-r--r--   0        0        0      769 2023-01-17 13:24:41.053089 nonebridge-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3647 1970-01-01 00:00:00.000000 nonebridge-0.1.4/setup.py
--rw-r--r--   0        0        0     3735 1970-01-01 00:00:00.000000 nonebridge-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-26 04:46:33.991526 nonebridge-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2869 2023-07-26 04:46:33.991526 nonebridge-0.1.5/README.md
+-rw-r--r--   0        0        0    20220 2023-07-26 04:46:33.995525 nonebridge-0.1.5/nonebridge/__init__.py
+-rw-r--r--   0        0        0      769 2023-07-26 04:46:33.995525 nonebridge-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3799 1970-01-01 00:00:00.000000 nonebridge-0.1.5/PKG-INFO
```

### Comparing `nonebridge-0.1.4/LICENSE` & `nonebridge-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebridge-0.1.4/README.md` & `nonebridge-0.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 | get_group_member_info | getChatMember                                                            |
 | send_group_msg        | ---                                                                      |
 ## 配置
 nonebridge所需的配置直接写入到nonebot2的.env文件内即可
 ```
 nonebridge_ob11_caption_ahead_photo: 将从telegram收到的带文字描述的图片消息中文字部分作为文字消息在ob11的消息段中前置以配合ob11中大部分插件的习惯写法，默认为True
 nonebridge_httpx_hook: 安装httpx钩子以拦截获取qq头像的http api，默认为False
+ob11_plugin_list: [] 需要强制处理为ob11消息的插件，该插件内的matcer将不会被tg消息触发
 ```
 
 ## 使用方法
 同时安装并两个adapter，在bot.py紧随nonebot之后导入nonebridge，必须在任何adapter导入之前导入nonebridge，需要同时注册两个Adapter才能正常运行   
 ### Example bot.py
 ```python
 import nonebot
```

### Comparing `nonebridge-0.1.4/nonebridge/__init__.py` & `nonebridge-0.1.5/nonebridge/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,20 @@
 
 
 import httpx
 
 async def httpx_async_client_get_func_hook(*a, **b):
     origin_func = b["origin_func"]
     b.pop("origin_func")
+    # try:
+    #     raise Exception("")
+    # except Exception as e:
+    #     print(e)
+    #     pass
+        
     # 寄，玩不明白怎么拿调用堆栈了，开摆
     # perform_hook = False
     # # limited hook for warped with asyncio, special for nonebot-plugin-petpet
     # asyncio_task = asyncio.current_task()
     # if "bot" in asyncio_task._coro.cr_frame.f_locals:
     #     bot : Ob11Bot = asyncio_task._coro.cr_frame.f_locals["bot"] #get bot
     #     if isinstance(bot,Ob11Bot) and bot.self_id == "0": # check is converted bot
@@ -113,14 +119,21 @@
     return await httpx_async_client_get_func_hook(*a, **b)
 orig_httpx_async_client_get_func = httpx.AsyncClient.get
 httpx.AsyncClient.get = httpx_async_client_get_func_async
 
 
 @run_preprocessor
 async def before_run_matcher(matcher: Matcher, bot: Bot, event: Event):
+    driver = nonebot.get_driver()
+    try:
+        ob11_plugin_list = driver.config.ob11_plugin_list
+    except:
+        ob11_plugin_list = []
+    if bot.adapter.get_name() == "Telegram" and matcher.plugin_name in ob11_plugin_list:
+        raise IgnoredException("Matcher target in ob11, ignore")
     if has_attr_in_bot(bot, "_alread_run_matcher") and isinstance(bot._alread_run_matcher, Dict):
         event_id = id(event) if not has_attr_in_bot(
             bot, "raw_event") else id(bot.raw_event)
         if not matcher.__class__ in bot._alread_run_matcher[event_id]:
             bot._alread_run_matcher[event_id].append(matcher.__class__)
         else:
             raise IgnoredException("Matcher has already been run")
@@ -357,14 +370,27 @@
                         "group_id": data["group_id"],
                         "user_id": member["user"]["id"],
                         "nickname": member["user"]["first_name"] if not "last_name" in member["user"] else member["user"]["first_name"] + member["user"]["last_name"],
                         "card": member["user"]["first_name"] if not "last_name" in member["user"] else member["user"]["first_name"] + member["user"]["last_name"],
                         "sex": "unknown",
                         "role": "member"
                     }))
+            # elif api == "get_stranger_info":
+            #     if adapter := get_adapter("Telegram"):
+            #         tg_bot = TgBot(adapter, "nonebridge")
+            #         member = await tg_bot.call_api("getChatMember", chat_id=data["group_id"], user_id=data["user_id"])
+            #         return json.loads(json.dumps({
+            #             "user_id": member["user"]["id"],
+            #             "nickname": member["user"]["first_name"] if not "last_name" in member["user"] else member["user"]["first_name"] + member["user"]["last_name"],
+            #             "sex": "unknown",
+            #             "age": 114514,
+            #             "qid": None,
+            #             "level": 114514,
+            #             "login_days": 114514
+            #         }))
         return await origin_func(self, api, **data)
 
     @staticmethod
     async def handle_event_hook(bot: "Bot", event: "Event", origin_func: Callable):
         return await origin_func(bot, event)
 
     @staticmethod
```

### Comparing `nonebridge-0.1.4/pyproject.toml` & `nonebridge-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebridge"
-version = "0.1.4"
+version = "0.1.5"
 description = "A adapter event bridge for nonebot2 makes plugins run on different adapters without any modify"
 authors = ["ColdThunder11 <lslyj27761@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ColdThunder11/nonebot-adapter-telegram"
 packages = [
   { include = "nonebridge" }
```

### Comparing `nonebridge-0.1.4/setup.py` & `nonebridge-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,71 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['nonebridge']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['nonebot-adapter-antelegram>=0.2.0-dev10,<0.3.0',
- 'nonebot-adapter-onebot>=2.2.0,<3.0.0',
- 'nonebot2>=2.0.0rc2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebridge',
-    'version': '0.1.4',
-    'description': 'A adapter event bridge for nonebot2 makes plugins run on different adapters without any modify',
-    'long_description': '# nonebridge\nA adapter event bridge for nonebot2 makes plugins running on different adapters without any modify   \n一个让你能够在不修改插件的情况下使其运行在不同adapter中的魔法bridge，开发目的是为了给[Yuki Clanbattle](https://github.com/ColdThunder11/yuki_clanbattle)提供Telegram支持\n## 还在开发中请勿生产环境使用\n女生自用插件，目前仅支持让为onebotv11编写的插件运行在自己写的[nonebot-adapter-telegram](https://github.com/ColdThunder11/nonebot-adapter-telegram)上，仅会支持有限的消息类型和API模拟   \n目前不支持~~主动发送消息和~~向非事件触发的聊天发送消息，支持主动向群聊使用send_group_msg发送群组消息了(必须在tg端收到任意消息后虚假的obv11 bot连接才会被注册)\n## 支持的接收类型\n- [x] 纯文字(MessageSegment.text)\n- [x] 图片(MessageSegment.image)\n\n## 支持的发送类型\n- [x] 文字(MessageSegment.text)\n- [x] 图片(MessageSegment.image)\n- [x] AT(MessageSegment.at)\n- [x] 语音(MessageSegment.record)\n\n## 支持的额外API\n| Onebot v11 API        | 对应的Telegarm API                                                       |\n| --------------------- | ------------------------------------------------------------------------ |\n| get_group_info        | getChat和getChatMemberCount                                              |\n| get_group_member_list | getChatAdministrators(由于tg并没有提供相关API，仅能够直接获取管理员信息) |\n| get_group_member_info | getChatMember                                                            |\n| send_group_msg        | ---                                                                      |\n## 配置\nnonebridge所需的配置直接写入到nonebot2的.env文件内即可\n```\nnonebridge_ob11_caption_ahead_photo: 将从telegram收到的带文字描述的图片消息中文字部分作为文字消息在ob11的消息段中前置以配合ob11中大部分插件的习惯写法，默认为True\nnonebridge_httpx_hook: 安装httpx钩子以拦截获取qq头像的http api，默认为False\n```\n\n## 使用方法\n同时安装并两个adapter，在bot.py紧随nonebot之后导入nonebridge，必须在任何adapter导入之前导入nonebridge，需要同时注册两个Adapter才能正常运行   \n### Example bot.py\n```python\nimport nonebot\nimport nonebridge\nfrom nonebot.adapters.onebot.v11 import Adapter as OneBot_V11_Adapter\nfrom nonebot.adapters.telegram.adapter import Adapter as Telegram_Adapter\n\nnonebot.init()\ndriver = nonebot.get_driver()\ndriver.register_adapter(OneBot_V11_Adapter)\ndriver.register_adapter(Telegram_Adapter)\nnonebot.load_plugin("your_onebotv11_plugin")\n\nif __name__ == "__main__":\n    nonebot.run()   \n```',
-    'author': 'ColdThunder11',
-    'author_email': 'lslyj27761@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ColdThunder11/nonebot-adapter-telegram',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8.1,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: nonebridge
+Version: 0.1.5
+Summary: A adapter event bridge for nonebot2 makes plugins run on different adapters without any modify
+Home-page: https://github.com/ColdThunder11/nonebot-adapter-telegram
+License: MIT
+Keywords: bot
+Author: ColdThunder11
+Author-email: lslyj27761@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot-adapter-antelegram (>=0.2.0-dev10,<0.3.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.2.0,<3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0rc2,<3.0.0)
+Project-URL: Repository, https://github.com/ColdThunder11/nonebot-adapter-telegram
+Description-Content-Type: text/markdown
+
+# nonebridge
+A adapter event bridge for nonebot2 makes plugins running on different adapters without any modify   
+一个让你能够在不修改插件的情况下使其运行在不同adapter中的魔法bridge，开发目的是为了给[Yuki Clanbattle](https://github.com/ColdThunder11/yuki_clanbattle)提供Telegram支持
+## 还在开发中请勿生产环境使用
+女生自用插件，目前仅支持让为onebotv11编写的插件运行在自己写的[nonebot-adapter-telegram](https://github.com/ColdThunder11/nonebot-adapter-telegram)上，仅会支持有限的消息类型和API模拟   
+目前不支持~~主动发送消息和~~向非事件触发的聊天发送消息，支持主动向群聊使用send_group_msg发送群组消息了(必须在tg端收到任意消息后虚假的obv11 bot连接才会被注册)
+## 支持的接收类型
+- [x] 纯文字(MessageSegment.text)
+- [x] 图片(MessageSegment.image)
+
+## 支持的发送类型
+- [x] 文字(MessageSegment.text)
+- [x] 图片(MessageSegment.image)
+- [x] AT(MessageSegment.at)
+- [x] 语音(MessageSegment.record)
+
+## 支持的额外API
+| Onebot v11 API        | 对应的Telegarm API                                                       |
+| --------------------- | ------------------------------------------------------------------------ |
+| get_group_info        | getChat和getChatMemberCount                                              |
+| get_group_member_list | getChatAdministrators(由于tg并没有提供相关API，仅能够直接获取管理员信息) |
+| get_group_member_info | getChatMember                                                            |
+| send_group_msg        | ---                                                                      |
+## 配置
+nonebridge所需的配置直接写入到nonebot2的.env文件内即可
+```
+nonebridge_ob11_caption_ahead_photo: 将从telegram收到的带文字描述的图片消息中文字部分作为文字消息在ob11的消息段中前置以配合ob11中大部分插件的习惯写法，默认为True
+nonebridge_httpx_hook: 安装httpx钩子以拦截获取qq头像的http api，默认为False
+ob11_plugin_list: [] 需要强制处理为ob11消息的插件，该插件内的matcer将不会被tg消息触发
+```
+
+## 使用方法
+同时安装并两个adapter，在bot.py紧随nonebot之后导入nonebridge，必须在任何adapter导入之前导入nonebridge，需要同时注册两个Adapter才能正常运行   
+### Example bot.py
+```python
+import nonebot
+import nonebridge
+from nonebot.adapters.onebot.v11 import Adapter as OneBot_V11_Adapter
+from nonebot.adapters.telegram.adapter import Adapter as Telegram_Adapter
+
+nonebot.init()
+driver = nonebot.get_driver()
+driver.register_adapter(OneBot_V11_Adapter)
+driver.register_adapter(Telegram_Adapter)
+nonebot.load_plugin("your_onebotv11_plugin")
+
+if __name__ == "__main__":
+    nonebot.run()   
+```
```

