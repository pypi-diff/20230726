# Comparing `tmp/nonebot_plugin_session-0.0.6.tar.gz` & `tmp/nonebot_plugin_session-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_session-0.0.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_session-0.0.7.tar", max compression
```

## Comparing `nonebot_plugin_session-0.0.6.tar` & `nonebot_plugin_session-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1063 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/LICENSE
--rw-r--r--   0        0        0     4337 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/README.md
--rw-r--r--   0        0        0      601 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/__init__.py
--rw-r--r--   0        0        0       75 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/__init__.py
--rw-r--r--   0        0        0      585 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/console.py
--rw-r--r--   0        0        0     1190 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/kaiheila.py
--rw-r--r--   0        0        0     2719 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/onebot_v11.py
--rw-r--r--   0        0        0     3537 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/onebot_v12.py
--rw-r--r--   0        0        0     1565 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/qqguild.py
--rw-r--r--   0        0        0     2616 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/telegram.py
--rw-r--r--   0        0        0      398 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/const.py
--rw-r--r--   0        0        0     2700 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/extractor.py
--rw-r--r--   0        0        0     1525 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/migrations/36de70108aeb_init_db.py
--rw-r--r--   0        0        0     1264 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/migrations/7d0575ba4608_enum_type.py
--rw-r--r--   0        0        0     2825 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/model.py
--rw-r--r--   0        0        0     2228 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/saa.py
--rw-r--r--   0        0        0     2106 2023-07-22 14:15:10.073833 nonebot_plugin_session-0.0.6/nonebot_plugin_session/session.py
--rw-r--r--   0        0        0     1874 2023-07-22 14:15:10.077833 nonebot_plugin_session-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5388 1970-01-01 00:00:00.000000 nonebot_plugin_session-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4337 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/README.md
+-rw-r--r--   0        0        0      601 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/__init__.py
+-rw-r--r--   0        0        0       75 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/__init__.py
+-rw-r--r--   0        0        0      585 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/console.py
+-rw-r--r--   0        0        0     1190 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/kaiheila.py
+-rw-r--r--   0        0        0     2719 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3537 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/onebot_v12.py
+-rw-r--r--   0        0        0     1565 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/qqguild.py
+-rw-r--r--   0        0        0     2616 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/telegram.py
+-rw-r--r--   0        0        0      398 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/const.py
+-rw-r--r--   0        0        0     2700 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/extractor.py
+-rw-r--r--   0        0        0     1525 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/migrations/36de70108aeb_init_db.py
+-rw-r--r--   0        0        0     1264 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/migrations/7d0575ba4608_enum_type.py
+-rw-r--r--   0        0        0     2893 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/model.py
+-rw-r--r--   0        0        0     2228 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/saa.py
+-rw-r--r--   0        0        0     2106 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/nonebot_plugin_session/session.py
+-rw-r--r--   0        0        0     1874 2023-07-26 10:14:44.709208 nonebot_plugin_session-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5388 1970-01-01 00:00:00.000000 nonebot_plugin_session-0.0.7/PKG-INFO
```

### Comparing `nonebot_plugin_session-0.0.6/LICENSE` & `nonebot_plugin_session-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/README.md` & `nonebot_plugin_session-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/__init__.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/console.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/kaiheila.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/kaiheila.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/onebot_v11.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/onebot_v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/onebot_v12.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/onebot_v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/qqguild.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/adapters/telegram.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/extractor.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/extractor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/migrations/36de70108aeb_init_db.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/migrations/36de70108aeb_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/migrations/7d0575ba4608_enum_type.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/migrations/7d0575ba4608_enum_type.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/model.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,17 @@
     require("nonebot_plugin_datastore")
 
     from nonebot_plugin_datastore import get_plugin_data
     from sqlalchemy import String, UniqueConstraint, select
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Mapped, mapped_column
 
-    Model = get_plugin_data().Model
+    plugin_data = get_plugin_data()
+    plugin_data.use_global_registry()
+    Model = plugin_data.Model
 
     class SessionModel(Model):
         __table_args__ = (
             UniqueConstraint(
                 "bot_id",
                 "bot_type",
                 "platform",
```

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/saa.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/saa.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/nonebot_plugin_session/session.py` & `nonebot_plugin_session-0.0.7/nonebot_plugin_session/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_session-0.0.6/pyproject.toml` & `nonebot_plugin_session-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot_plugin_session"
-version = "0.0.6"
+version = "0.0.7"
 description = "Nonebot2 会话信息提取与会话id定义"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-session"
 repository = "https://github.com/noneplugin/nonebot-plugin-session"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nonebot2 = { version = "^2.0.0", extras = ["fastapi"] }
 strenum = "^0.4.8"
-nonebot-plugin-datastore = { version = "^1.0.0", optional = true }
+nonebot-plugin-datastore = { version = "^1.1.0", optional = true }
 nonebot-plugin-send-anything-anywhere = { version = "^0.2.7", optional = true }
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 
 [tool.poetry.group.test.dependencies]
 pytest-cov = "^4.0.0"
```

### Comparing `nonebot_plugin_session-0.0.6/PKG-INFO` & `nonebot_plugin_session-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-session
-Version: 0.0.6
+Version: 0.0.7
 Summary: Nonebot2 会话信息提取与会话id定义
 Home-page: https://github.com/noneplugin/nonebot-plugin-session
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: datastore
 Provides-Extra: saa
-Requires-Dist: nonebot-plugin-datastore (>=1.0.0,<2.0.0) ; extra == "datastore" or extra == "all"
+Requires-Dist: nonebot-plugin-datastore (>=1.1.0,<2.0.0) ; extra == "datastore" or extra == "all"
 Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0) ; extra == "saa" or extra == "all"
 Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0)
 Requires-Dist: strenum (>=0.4.8,<0.5.0)
 Project-URL: Repository, https://github.com/noneplugin/nonebot-plugin-session
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-session Version: 0.0.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-session Version: 0.0.7 Summary:
 Nonebot2 ä¼è¯ä¿¡æ¯æåä¸ä¼è¯idå®ä¹ Home-page: https://github.com/
 noneplugin/nonebot-plugin-session License: MIT Author: meetwq Author-email:
 meetwq@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Provides-Extra: all
 Provides-Extra: datastore Provides-Extra: saa Requires-Dist: nonebot-plugin-
-datastore (>=1.0.0,<2.0.0) ; extra == "datastore" or extra == "all" Requires-
+datastore (>=1.1.0,<2.0.0) ; extra == "datastore" or extra == "all" Requires-
 Dist: nonebot-plugin-send-anything-anywhere (>=0.2.7,<0.3.0) ; extra == "saa"
 or extra == "all" Requires-Dist: nonebot2[fastapi] (>=2.0.0,<3.0.0) Requires-
 Dist: strenum (>=0.4.8,<0.5.0) Project-URL: Repository, https://github.com/
 noneplugin/nonebot-plugin-session Description-Content-Type: text/markdown
 [nonebot] # nonebot-plugin-session _â¨ [Nonebot2](https://github.com/nonebot/
           nonebot2) ä¼è¯ä¿¡æ¯æåä¸ä¼è¯ id å®ä¹æä»¶ â¨_
                       [license] [Python] [NoneBot] [pypi]
```

