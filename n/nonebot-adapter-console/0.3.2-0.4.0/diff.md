# Comparing `tmp/nonebot_adapter_console-0.3.2.tar.gz` & `tmp/nonebot_adapter_console-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_console-0.3.2.tar", max compression
+gzip compressed data, was "nonebot_adapter_console-0.4.0.tar", last modified: Wed Jul 26 14:58:27 2023, max compression
```

## Comparing `nonebot_adapter_console-0.3.2.tar` & `nonebot_adapter_console-0.4.0.tar`

### file list

```diff
@@ -1,31 +1,13 @@
--rw-r--r--   0        0        0     1078 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/LICENSE
--rw-r--r--   0        0        0      282 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/README.md
--rw-r--r--   0        0        0      203 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/__init__.py
--rw-r--r--   0        0        0     1995 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/adapter.py
--rw-r--r--   0        0        0     1931 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/bot.py
--rw-r--r--   0        0        0       98 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/config.py
--rw-r--r--   0        0        0     2388 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/event.py
--rw-r--r--   0        0        0        0 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/exception.py
--rw-r--r--   0        0        0       38 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/__init__.py
--rw-r--r--   0        0        0     4321 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/app.py
--rw-r--r--   0        0        0      713 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/components/chatroom/__init__.py
--rw-r--r--   0        0        0     2023 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/components/chatroom/history.py
--rw-r--r--   0        0        0     1433 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/components/chatroom/input.py
--rw-r--r--   0        0        0     4096 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/components/chatroom/message.py
--rw-r--r--   0        0        0     2189 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/components/chatroom/toolbar.py
--rw-r--r--   0        0        0       45 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/components/footer.py
--rw-r--r--   0        0        0      982 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/components/general/action.py
--rw-r--r--   0        0        0      236 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/components/header.py
--rw-r--r--   0        0        0     1297 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/components/log/__init__.py
--rw-r--r--   0        0        0     1253 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/components/log/toolbar.py
--rw-r--r--   0        0        0     1143 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/log_redirect.py
--rw-r--r--   0        0        0       92 2023-02-02 06:48:37.609463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/router/__init__.py
--rw-r--r--   0        0        0     1242 2023-02-02 06:48:37.613463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/router/router.py
--rw-r--r--   0        0        0     2232 2023-02-02 06:48:37.613463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/storage/__init__.py
--rw-r--r--   0        0        0     1569 2023-02-02 06:48:37.613463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/views/horizontal.py
--rw-r--r--   0        0        0      295 2023-02-02 06:48:37.613463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/frontend/views/log_view.py
--rw-r--r--   0        0        0     7650 2023-02-02 06:48:37.613463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/message.py
--rw-r--r--   0        0        0      361 2023-02-02 06:48:37.613463 nonebot_adapter_console-0.3.2/nonebot/adapters/console/utils.py
--rw-r--r--   0        0        0      920 2023-02-02 06:48:37.613463 nonebot_adapter_console-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1379 1970-01-01 00:00:00.000000 nonebot_adapter_console-0.3.2/setup.py
--rw-r--r--   0        0        0      916 1970-01-01 00:00:00.000000 nonebot_adapter_console-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/LICENSE
+-rw-r--r--   0        0        0       18 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/README.md
+-rw-r--r--   0        0        0      264 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/nonebot/adapters/console/__init__.py
+-rw-r--r--   0        0        0     2201 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/nonebot/adapters/console/adapter.py
+-rw-r--r--   0        0        0     3232 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/nonebot/adapters/console/backend.py
+-rw-r--r--   0        0        0     2333 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/nonebot/adapters/console/bot.py
+-rw-r--r--   0        0        0       98 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/nonebot/adapters/console/config.py
+-rw-r--r--   0        0        0     2145 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/nonebot/adapters/console/event.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/nonebot/adapters/console/exception.py
+-rw-r--r--   0        0        0     4034 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/nonebot/adapters/console/message.py
+-rw-r--r--   0        0        0      361 2023-07-26 14:57:50.144151 nonebot_adapter_console-0.4.0/nonebot/adapters/console/utils.py
+-rw-r--r--   0        0        0     1286 2023-07-26 14:58:27.312023 nonebot_adapter_console-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 nonebot_adapter_console-0.4.0/PKG-INFO
```

### Comparing `nonebot_adapter_console-0.3.2/LICENSE` & `nonebot_adapter_console-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_console-0.3.2/nonebot/adapters/console/adapter.py` & `nonebot_adapter_console-0.4.0/nonebot/adapters/console/adapter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import sys
 import asyncio
-from typing import TYPE_CHECKING, Any, Dict, List, Callable, Optional, Awaitable
+from typing import Any, Dict, List, Callable, Optional, Awaitable
 
+from textual.color import Color
 from nonebot.drivers import Driver
 from nonebot.typing import overrides
+from nonechat import Frontend, ConsoleSetting
 
 from nonebot.adapters import Adapter as BaseAdapter
 
 from . import BOT_ID
 from .bot import Bot
 from .event import Event
 from .config import Config
-
-if TYPE_CHECKING:
-    from .frontend import Frontend
+from .backend import AdapterConsoleBackend
 
 
 class Adapter(BaseAdapter):
     @overrides(BaseAdapter)
     def __init__(self, driver: Driver, **kwargs: Any) -> None:
         super().__init__(driver, **kwargs)
         self.console_config = Config.parse_obj(self.config)
         self.bot = Bot(self, BOT_ID)
 
         self._task: Optional[asyncio.Task] = None
-        self._frontend: Optional["Frontend"] = None
+        self._frontend: Optional[Frontend[AdapterConsoleBackend]] = None
         self._stdout = sys.stdout
         self.clients: List[Callable[[Bot, str, Dict[str, Any]], Awaitable[Any]]] = []
 
         self.setup()
 
     @staticmethod
     @overrides(BaseAdapter)
@@ -37,29 +37,34 @@
 
     def setup(self):
         if not self.console_config.console_headless_mode:
             self.driver.on_startup(self._start)
             self.driver.on_shutdown(self._shutdown)
 
     async def _start(self) -> None:
-        from .frontend import Frontend
-
-        self._frontend = Frontend(self)
+        self._frontend = Frontend(
+            AdapterConsoleBackend,
+            ConsoleSetting(
+                title="Nonebot",
+                sub_title="welcome to Console",
+                toolbar_exit="❌",
+                toolbar_back="⬅",
+                icon_color=Color.parse("#EA5252"),
+            ),
+        )
+        self._frontend.backend.set_adapter(self)
         self._task = asyncio.create_task(self._frontend.run_async())
         self.bot_connect(self.bot)
 
     async def _shutdown(self) -> None:
         self.bot_disconnect(self.bot)
         if self._frontend:
             self._frontend.exit()
         if self._task:
             await self._task
 
-    def add_client(self, client: Callable[[Bot, str, Dict[str, Any]], Awaitable[Any]]):
-        self.clients.append(client)
-
     def post_event(self, event: Event) -> None:
         asyncio.create_task(self.bot.handle_event(event))
 
     @overrides(BaseAdapter)
     async def _call_api(self, bot: Bot, api: str, **data: Any) -> None:
-        await asyncio.gather(*(client(bot, api, data) for client in self.clients))
+        await self._frontend.call(api, data)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_adapter_console-0.3.2/nonebot/adapters/console/bot.py` & `nonebot_adapter_console-0.4.0/nonebot/adapters/console/bot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import re
 from typing import TYPE_CHECKING, Any, Union
 
 from nonebot.typing import overrides
 from nonebot.message import handle_event
+from nonechat.message import Text, Emoji, Markup, Markdown, ConsoleMessage
 
-from nonebot.adapters import Adapter
 from nonebot.adapters import Bot as BaseBot
 
 from .utils import log
+from .event import Event, MessageEvent
 from .message import Message, MessageSegment
-from .event import Event, Robot, MessageEvent
 
 
 def _check_nickname(bot: "Bot", event: MessageEvent) -> None:
     first_msg_seg = event.message[0]
     if first_msg_seg.type != "text":
         return
 
@@ -28,25 +28,17 @@
         log("DEBUG", f"User is calling me {m[1]}")
         first_msg_seg.data["text"] = first_text[m.end() :]
 
 
 class Bot(BaseBot):
     if TYPE_CHECKING:
 
-        async def send_msg(self, user_id: str, message: Message, **kwargs: Any) -> None:
-            ...
-
         async def bell(self) -> None:
             ...
 
-    @overrides(BaseBot)
-    def __init__(self, adapter: "Adapter", self_id: str):
-        super().__init__(adapter, self_id)
-        self.info = Robot(id=self_id)
-
     @property
     def type(self) -> str:
         return "Console"
 
     @overrides(BaseBot)
     async def send(
         self,
@@ -57,12 +49,27 @@
         full_message = Message()
         full_message += message
 
         return await self.send_msg(
             user_id=event.user.nickname, message=full_message, **kwargs
         )
 
+    async def send_msg(self, *, user_id: str, message: Message, **kwargs: Any) -> None:
+        elements = []
+        for seg in message:
+            if seg.type == "text":
+                elements.append(Text(seg.data["text"]))
+            elif seg.type == "emoji":
+                elements.append(Emoji(seg.data["name"]))
+            elif seg.type == "markdown":
+                elements.append(Markdown(**seg.data))
+            elif seg.type == "markup":
+                elements.append(Markup(**seg.data))
+        return await self.call_api(
+            "send_msg", user_id=user_id, message=ConsoleMessage(elements), **kwargs
+        )
+
     async def handle_event(self, event: Event) -> None:
         """处理收到的事件"""
         if isinstance(event, MessageEvent):
             _check_nickname(self, event)
         await handle_event(self, event)
```

### Comparing `nonebot_adapter_console-0.3.2/nonebot/adapters/console/event.py` & `nonebot_adapter_console-0.4.0/nonebot/adapters/console/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,19 @@
 from datetime import datetime
 from typing import List, Literal
 
-from pydantic import BaseModel
+from nonechat.info import User
 from nonebot.typing import overrides
 from nonebot.utils import escape_tag
 
 from nonebot.adapters import Event as BaseEvent
 
 from .message import Message
 
 
-class User(BaseModel, frozen=True):
-    """用户"""
-
-    id: str
-    avatar: str = "👤"
-    nickname: str = "User"
-
-
-class Robot(User, frozen=True):
-    """机器人"""
-
-    avatar: str = "🤖"
-    nickname: str = "Bot"
-
-
 class Event(BaseEvent):
     time: datetime
     self_id: str
     post_type: str
     user: User
 
     @overrides(BaseEvent)
@@ -93,8 +78,8 @@
                     (escape_tag("".join(texts)), f"<le>{escape_tag(str(seg))}</le>")
                 )
                 texts.clear()
         msg_string.append(escape_tag("".join(texts)))
         return f"Message from {self.user.nickname} {''.join(msg_string)!r}"
 
 
-__all__ = ["User", "Robot", "Event", "MessageEvent"]
+__all__ = ["Event", "MessageEvent"]
```

