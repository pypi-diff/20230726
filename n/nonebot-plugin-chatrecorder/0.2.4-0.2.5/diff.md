# Comparing `tmp/nonebot_plugin_chatrecorder-0.2.4.tar.gz` & `tmp/nonebot_plugin_chatrecorder-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_chatrecorder-0.2.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_chatrecorder-0.2.5.tar", max compression
```

## Comparing `nonebot_plugin_chatrecorder-0.2.4.tar` & `nonebot_plugin_chatrecorder-0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2979 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/README.md
--rw-r--r--   0        0        0      602 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/__init__.py
--rw-r--r--   0        0        0       37 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/adapters/__init__.py
--rw-r--r--   0        0        0     4631 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/adapters/onebot_v11.py
--rw-r--r--   0        0        0     3327 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/adapters/onebot_v12.py
--rw-r--r--   0        0        0      317 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/config.py
--rw-r--r--   0        0        0      483 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/consts.py
--rw-r--r--   0        0        0      402 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/exception.py
--rw-r--r--   0        0        0     1859 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/message.py
--rw-r--r--   0        0        0     1703 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py
--rw-r--r--   0        0        0     3732 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py
--rw-r--r--   0        0        0     1517 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py
--rw-r--r--   0        0        0     1731 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/model.py
--rw-r--r--   0        0        0     6206 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/record.py
--rw-r--r--   0        0        0     2587 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/record.pyi
--rw-r--r--   0        0        0      365 2023-06-28 02:43:20.338192 nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/utils.py
--rw-r--r--   0        0        0     1183 2023-06-28 02:43:20.342192 nonebot_plugin_chatrecorder-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3789 1970-01-01 00:00:00.000000 nonebot_plugin_chatrecorder-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2979 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/README.md
+-rw-r--r--   0        0        0      602 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/__init__.py
+-rw-r--r--   0        0        0       37 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/adapters/__init__.py
+-rw-r--r--   0        0        0     4855 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3327 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/adapters/onebot_v12.py
+-rw-r--r--   0        0        0      317 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/config.py
+-rw-r--r--   0        0        0      483 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/consts.py
+-rw-r--r--   0        0        0      402 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/exception.py
+-rw-r--r--   0        0        0     1859 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/message.py
+-rw-r--r--   0        0        0     1703 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py
+-rw-r--r--   0        0        0     3732 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py
+-rw-r--r--   0        0        0     1517 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py
+-rw-r--r--   0        0        0     1731 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/model.py
+-rw-r--r--   0        0        0     6206 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/record.py
+-rw-r--r--   0        0        0     2587 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/record.pyi
+-rw-r--r--   0        0        0      365 2023-07-26 15:06:50.802185 nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/utils.py
+-rw-r--r--   0        0        0     1183 2023-07-26 15:06:50.806185 nonebot_plugin_chatrecorder-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3789 1970-01-01 00:00:00.000000 nonebot_plugin_chatrecorder-0.2.5/PKG-INFO
```

### Comparing `nonebot_plugin_chatrecorder-0.2.4/README.md` & `nonebot_plugin_chatrecorder-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/__init__.py` & `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/adapters/onebot_v11.py` & `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/adapters/onebot_v11.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,25 +68,33 @@
             result: Optional[Dict[str, Any]],
         ):
             if e or not result:
                 return
             if api not in ["send_msg", "send_private_msg", "send_group_msg"]:
                 return
 
+            if api == "send_group_msg" or (
+                api == "send_msg"
+                and (
+                    data.get("message_type") == "group"
+                    or (data.get("message_type") == None and data.get("group_id"))
+                )
+            ):
+                detail_type = "group"
+            else:
+                detail_type = "private"
+
             message = Message(data["message"])
             record = MessageRecord(
                 bot_type=bot.type,
                 bot_id=bot.self_id,
                 platform="qq",
                 time=datetime.utcnow(),
                 type="message_sent",
-                detail_type="group"
-                if api == "send_group_msg"
-                or (api == "send_msg" and data["message_type"] == "group")
-                else "private",
+                detail_type=detail_type,
                 message_id=str(result["message_id"]),
                 message=serialize_message(bot, message),
                 plain_text=message.extract_plain_text(),
                 user_id=str(bot.self_id),
                 group_id=str(data.get("group_id", "")) or None,
             )
```

### Comparing `nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/adapters/onebot_v12.py` & `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/message.py` & `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py` & `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/2cad88d938f1_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py` & `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/7228a3a08576_ob12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py` & `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/migrations/9bca28bcb998_msg_type.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/model.py` & `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/record.py` & `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/record.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.4/nonebot_plugin_chatrecorder/record.pyi` & `nonebot_plugin_chatrecorder-0.2.5/nonebot_plugin_chatrecorder/record.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_chatrecorder-0.2.4/pyproject.toml` & `nonebot_plugin_chatrecorder-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_chatrecorder"
-version = "0.2.4"
+version = "0.2.5"
 description = "适用于 Nonebot2 的聊天记录插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-chatrecorder"
 repository = "https://github.com/noneplugin/nonebot-plugin-chatrecorder"
```

### Comparing `nonebot_plugin_chatrecorder-0.2.4/PKG-INFO` & `nonebot_plugin_chatrecorder-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-chatrecorder
-Version: 0.2.4
+Version: 0.2.5
 Summary: 适用于 Nonebot2 的聊天记录插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-chatrecorder
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

