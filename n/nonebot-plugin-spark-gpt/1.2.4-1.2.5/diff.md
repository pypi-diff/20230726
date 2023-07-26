# Comparing `tmp/nonebot_plugin_spark_gpt-1.2.4.tar.gz` & `tmp/nonebot_plugin_spark_gpt-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_spark_gpt-1.2.4.tar", max compression
+gzip compressed data, was "nonebot_plugin_spark_gpt-1.2.5.tar", max compression
```

## Comparing `nonebot_plugin_spark_gpt-1.2.4.tar` & `nonebot_plugin_spark_gpt-1.2.5.tar`

### file list

```diff
@@ -1,89 +1,84 @@
--rw-r--r--   0        0        0      219 2023-07-11 09:53:31.539890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/__init__.py
--rw-r--r--   0        0        0    17261 2023-07-11 09:53:31.540890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/adapter.py
--rw-r--r--   0        0        0      138 2023-07-11 09:53:31.541890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/__init__.py
--rw-r--r--   0        0        0       27 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/client.py
--rw-r--r--   0        0        0    51932 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/client.pyi
--rw-r--r--   0        0        0    98693 2023-07-11 09:53:31.543890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/handle.py
--rw-r--r--   0        0        0   115238 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/model.py
--rw-r--r--   0        0        0     1482 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/request.py
--rw-r--r--   0        0        0    34839 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/types.py
--rw-r--r--   0        0        0     2441 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/utils.py
--rw-r--r--   0        0        0     7255 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/bot.py
--rw-r--r--   0        0        0     2192 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/config.py
--rw-r--r--   0        0        0    28334 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/event.py
--rw-r--r--   0        0        0     2076 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/exception.py
--rw-r--r--   0        0        0    13603 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/message.py
--rw-r--r--   0        0        0     2874 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/payload.py
--rw-r--r--   0        0        0     1946 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/typing.py
--rw-r--r--   0        0        0      626 2023-07-11 09:53:31.548892 nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/utils.py
--rw-r--r--   0        0        0      836 2023-07-24 07:03:07.854838 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 07:03:07.854838 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/__init__.py
--rw-r--r--   0        0        0     2791 2023-07-24 07:03:07.855838 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/bard.py
--rw-r--r--   0        0        0     9823 2023-07-24 07:03:07.855838 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py
--rw-r--r--   0        0        0     9032 2023-07-24 07:03:07.855838 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/claude_ai.py
--rw-r--r--   0        0        0     4881 2023-07-24 07:15:39.854055 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/load_config.py
--rw-r--r--   0        0        0     6815 2023-07-24 07:29:17.601187 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/newbing.py
--rw-r--r--   0        0        0     6713 2023-07-24 07:15:39.851055 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/poe.py
--rw-r--r--   0        0        0     7619 2023-07-24 07:03:07.857837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/slack_claude.py
--rw-r--r--   0        0        0     8129 2023-07-24 07:03:07.858837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/spark_desk.py
--rw-r--r--   0        0        0     7490 2023-07-24 07:29:17.597189 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/sydneybing.py
--rw-r--r--   0        0        0     6802 2023-07-24 07:03:07.858837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py
--rw-r--r--   0        0        0        0 2023-07-24 07:03:07.859837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/__init__.py
--rw-r--r--   0        0        0    12575 2023-07-24 07:03:07.859837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/Bard.py
--rw-r--r--   0        0        0        0 2023-07-24 07:03:07.860837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/__init__.py
--rw-r--r--   0        0        0    17586 2023-07-24 07:03:07.860837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/BingImageCreator.py
--rw-r--r--   0        0        0    11837 2023-07-24 07:03:07.861837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/chathub.py
--rw-r--r--   0        0        0     2107 2023-07-24 07:03:07.861837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py
--rw-r--r--   0        0        0     4582 2023-07-24 07:03:07.861837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py
--rw-r--r--   0        0        0     1312 2023-07-24 07:03:07.862837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation_style.py
--rw-r--r--   0        0        0     8088 2023-07-24 07:03:07.862837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeGPT.py
--rw-r--r--   0        0        0    14626 2023-07-24 07:03:07.863837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py
--rw-r--r--   0        0        0       48 2023-07-24 07:03:07.863837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/exceptions.py
--rw-r--r--   0        0        0      278 2023-07-24 07:03:07.863837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/ImageGen.py
--rw-r--r--   0        0        0     2332 2023-07-24 07:03:07.864837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/locale.py
--rw-r--r--   0        0        0     7757 2023-07-24 07:03:07.864837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/main.py
--rw-r--r--   0        0        0     5948 2023-07-24 07:03:07.865837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/request.py
--rw-r--r--   0        0        0      992 2023-07-24 07:03:07.865837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/utilities.py
--rw-r--r--   0        0        0       83 2023-07-24 07:03:07.866837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/__init__.py
--rw-r--r--   0        0        0     1454 2023-07-24 07:03:07.866837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py
--rw-r--r--   0        0        0      127 2023-07-24 07:03:07.867836 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/main.py
--rw-r--r--   0        0        0     5878 2023-07-24 07:03:07.867836 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py
--rw-r--r--   0        0        0      719 2023-07-24 07:03:07.867836 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py
--rw-r--r--   0        0        0        0 2023-07-24 07:03:07.868837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/__init__.py
--rw-r--r--   0        0        0     5163 2023-07-24 07:15:39.840027 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/config.py
--rw-r--r--   0        0        0     1660 2023-07-24 07:03:07.869837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/load_config.py
--rw-r--r--   0        0        0     5024 2023-07-24 07:03:07.869837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/mytypes.py
--rw-r--r--   0        0        0     4634 2023-07-24 07:03:07.870837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/prefix_data.py
--rw-r--r--   0        0        0    30787 2023-07-24 07:03:07.870837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/prompt_data.py
--rw-r--r--   0        0        0     9955 2023-07-24 07:03:07.870837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/user_data.py
--rw-r--r--   0        0        0    15217 2023-07-24 07:15:39.844030 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/app.py
--rw-r--r--   0        0        0      547 2023-07-24 07:03:07.872837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json
--rw-r--r--   0        0        0        0 2023-07-24 07:03:07.872837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/templates/__init__.py
--rw-r--r--   0        0        0     4730 2023-07-24 07:03:07.872837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/templates/config.html
--rw-r--r--   0        0        0     2246 2023-07-24 07:03:07.873837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/templates/index.html
--rw-r--r--   0        0        0    10215 2023-07-24 07:03:07.873837 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/templates/prefix.html
--rw-r--r--   0        0        0    10211 2023-07-24 07:03:07.874842 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/templates/prompt.html
--rw-r--r--   0        0        0       23 2023-07-24 07:03:07.874842 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/__init__.py
--rw-r--r--   0        0        0       51 2023-07-24 07:03:07.874842 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/__init__.py
--rw-r--r--   0        0        0    20108 2023-07-24 07:15:39.848049 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py
--rw-r--r--   0        0        0    26287 2023-07-24 07:29:17.590679 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py
--rw-r--r--   0        0        0        0 2023-07-24 07:37:10.606615 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/HelpMsg.jpeg
--rw-r--r--   0        0        0   136085 2023-07-24 07:37:12.079792 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/PrefixMsg.jpeg
--rw-r--r--   0        0        0   580379 2023-07-24 07:37:11.423936 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/PromptMsg.jpeg
--rw-r--r--   0        0        0   925239 2023-07-24 07:37:10.070600 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/SourceMsg.jpeg
--rw-r--r--   0        0        0   614235 2023-07-24 07:37:10.606615 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/SuperMsg.jpeg
--rw-r--r--   0        0        0     2275 2023-07-24 07:03:07.887841 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py
--rw-r--r--   0        0        0    15735 2023-07-24 07:03:07.887841 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py
--rw-r--r--   0        0        0     6523 2023-07-24 07:03:07.889345 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/temp_bots.py
--rw-r--r--   0        0        0     2127 2023-07-24 07:03:07.889345 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/render.py
--rw-r--r--   0        0        0  1458204 2023-07-24 07:03:07.897348 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css
--rw-r--r--   0        0        0   270288 2023-07-24 07:03:07.899350 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js
--rw-r--r--   0        0        0     1290 2023-07-24 07:03:07.900349 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js
--rw-r--r--   0        0        0    19652 2023-07-24 07:03:07.900349 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/markdown.css
--rw-r--r--   0        0        0     1259 2023-07-24 07:03:07.901350 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/markdown.html
--rw-r--r--   0        0        0     4963 2023-07-24 07:03:07.901350 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css
--rw-r--r--   0        0        0      125 2023-07-24 07:03:07.902350 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/text.css
--rw-r--r--   0        0        0     1113 2023-07-24 07:03:07.902350 nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/utils.py
--rw-r--r--   0        0        0     1016 2023-07-24 06:58:18.377669 nonebot_plugin_spark_gpt-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     8478 2023-07-23 16:09:22.248830 nonebot_plugin_spark_gpt-1.2.4/README.md
--rw-r--r--   0        0        0     9698 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0      219 2023-07-11 09:53:31.539890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/__init__.py
+-rw-r--r--   0        0        0    17261 2023-07-11 09:53:31.540890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/adapter.py
+-rw-r--r--   0        0        0      138 2023-07-11 09:53:31.541890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/__init__.py
+-rw-r--r--   0        0        0       27 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/client.py
+-rw-r--r--   0        0        0    51932 2023-07-11 09:53:31.542890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/client.pyi
+-rw-r--r--   0        0        0    98693 2023-07-11 09:53:31.543890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/handle.py
+-rw-r--r--   0        0        0   115238 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/model.py
+-rw-r--r--   0        0        0     1482 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/request.py
+-rw-r--r--   0        0        0    34839 2023-07-11 09:53:31.544890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/types.py
+-rw-r--r--   0        0        0     2441 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/utils.py
+-rw-r--r--   0        0        0     7255 2023-07-11 09:53:31.545890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/bot.py
+-rw-r--r--   0        0        0     2192 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/config.py
+-rw-r--r--   0        0        0    28334 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/event.py
+-rw-r--r--   0        0        0     2076 2023-07-11 09:53:31.546890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/exception.py
+-rw-r--r--   0        0        0    13603 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/message.py
+-rw-r--r--   0        0        0     2874 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/payload.py
+-rw-r--r--   0        0        0     1946 2023-07-11 09:53:31.547890 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/typing.py
+-rw-r--r--   0        0        0      626 2023-07-11 09:53:31.548892 nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/utils.py
+-rw-r--r--   0        0        0      836 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/__init__.py
+-rw-r--r--   0        0        0     2791 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/bard.py
+-rw-r--r--   0        0        0     9823 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py
+-rw-r--r--   0        0        0     9032 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/claude_ai.py
+-rw-r--r--   0        0        0     4881 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/load_config.py
+-rw-r--r--   0        0        0     6815 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/newbing.py
+-rw-r--r--   0        0        0     6863 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/poe.py
+-rw-r--r--   0        0        0     7619 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/slack_claude.py
+-rw-r--r--   0        0        0     8129 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/spark_desk.py
+-rw-r--r--   0        0        0     7490 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/sydneybing.py
+-rw-r--r--   0        0        0     6802 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/__init__.py
+-rw-r--r--   0        0        0    12575 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/Bard.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/__init__.py
+-rw-r--r--   0        0        0    17586 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/BingImageCreator.py
+-rw-r--r--   0        0        0    11837 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/chathub.py
+-rw-r--r--   0        0        0     2107 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py
+-rw-r--r--   0        0        0     4582 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py
+-rw-r--r--   0        0        0     1312 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation_style.py
+-rw-r--r--   0        0        0     8088 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeGPT.py
+-rw-r--r--   0        0        0    14626 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py
+-rw-r--r--   0        0        0       48 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/exceptions.py
+-rw-r--r--   0        0        0      278 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/ImageGen.py
+-rw-r--r--   0        0        0     2332 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/locale.py
+-rw-r--r--   0        0        0     7757 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/main.py
+-rw-r--r--   0        0        0     5948 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/request.py
+-rw-r--r--   0        0        0      992 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/utilities.py
+-rw-r--r--   0        0        0       83 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/__init__.py
+-rw-r--r--   0        0        0     1454 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py
+-rw-r--r--   0        0        0      127 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/main.py
+-rw-r--r--   0        0        0     5878 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py
+-rw-r--r--   0        0        0      719 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/__init__.py
+-rw-r--r--   0        0        0     5163 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/config.py
+-rw-r--r--   0        0        0     1660 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/load_config.py
+-rw-r--r--   0        0        0     5024 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/mytypes.py
+-rw-r--r--   0        0        0     4634 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/prefix_data.py
+-rw-r--r--   0        0        0    30787 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/prompt_data.py
+-rw-r--r--   0        0        0     9955 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/user_data.py
+-rw-r--r--   0        0        0    15269 2023-07-26 07:45:54.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/app.py
+-rw-r--r--   0        0        0      547 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json
+-rw-r--r--   0        0        0        0 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/templates/__init__.py
+-rw-r--r--   0        0        0     4730 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/templates/config.html
+-rw-r--r--   0        0        0     2246 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/templates/index.html
+-rw-r--r--   0        0        0    10215 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/templates/prefix.html
+-rw-r--r--   0        0        0    10211 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/templates/prompt.html
+-rw-r--r--   0        0        0       23 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/__init__.py
+-rw-r--r--   0        0        0       51 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/nonebot/__init__.py
+-rw-r--r--   0        0        0    17766 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py
+-rw-r--r--   0        0        0    26080 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py
+-rw-r--r--   0        0        0     2275 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py
+-rw-r--r--   0        0        0    15735 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py
+-rw-r--r--   0        0        0     6623 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/temp_bots.py
+-rw-r--r--   0        0        0     2127 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/render.py
+-rw-r--r--   0        0        0  1458204 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css
+-rw-r--r--   0        0        0   270288 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js
+-rw-r--r--   0        0        0     1290 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js
+-rw-r--r--   0        0        0    19652 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/markdown.css
+-rw-r--r--   0        0        0     1259 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/markdown.html
+-rw-r--r--   0        0        0     4963 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css
+-rw-r--r--   0        0        0      125 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/text.css
+-rw-r--r--   0        0        0     1113 2023-07-26 07:39:48.000000 nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/utils.py
+-rw-r--r--   0        0        0     1016 2023-07-26 08:39:41.678201 nonebot_plugin_spark_gpt-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     8478 2023-07-23 16:09:22.248830 nonebot_plugin_spark_gpt-1.2.5/README.md
+-rw-r--r--   0        0        0     9698 1970-01-01 00:00:00.000000 nonebot_plugin_spark_gpt-1.2.5/PKG-INFO
```

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/adapter.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/client.pyi` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/handle.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/model.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/request.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/types.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/api/utils.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/api/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/bot.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/config.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/event.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/exception.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/message.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/payload.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/payload.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/typing.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/typing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot/adapters/discord/utils.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot/adapters/discord/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/__init__.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/bard.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/bard.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/chatgpt_web.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/claude_ai.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/claude_ai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/load_config.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/load_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/newbing.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/newbing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/poe.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/poe.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,19 @@
     except Exception as e:
         logger.info(f"加载Poe配置时warn:{str(e)},如果你已经配置了分流或全局代理,请无视此warn")
 
     try:
         P_B = config.get_config(source="Poe配置", config_name="p_b")
     except Exception as e:
         ABLE = False
-        SUBSCRIBE_ABLE = False
         logger.warning(f"加载Poe配置时warn:{str(e)},无法使用Poe")
     try:
         FORMKEY = config.get_config(source="Poe配置", config_name="formkey")
     except Exception as e:
-        ABLE = False
-        SUBSCRIBE_ABLE = False
-        logger.warning(f"加载Poe配置时warn:{str(e)},无法使用Poe")
+        logger.warning(f"加载Poe配置时warn:{str(e)},必须安装node.js才可以自动提取formkey,否则报错无法使用")
     try:
         arg = config.get_config(source="Poe配置", config_name="suggest_able")
         if arg == "True":
             SUGGEST_ABLE = True
         else:
             SUGGEST_ABLE = False
     except Exception as e:
@@ -63,15 +60,18 @@
 
 
 load_config()
 
 
 class Poe_Bot:
     def __init__(
-            self, common_userinfo: CommonUserInfo, bot_info: BotInfo, bot_data: BotData,
+        self,
+        common_userinfo: CommonUserInfo,
+        bot_info: BotInfo,
+        bot_data: BotData,
     ):
         self.lock = asyncio.Lock()
         self.nickname = bot_info.nickname
         self.common_userinfo = common_userinfo
         self.botdata = bot_data
         self.source = bot_data.source
 
@@ -98,52 +98,67 @@
     def __hash__(self) -> int:
         return hash((self.common_userinfo.user_id, self.nickname))
 
     async def ask(self, question: str):
         global CLIENT
         if CLIENT is None:
             CLIENT = await Poe_Client(P_B, FORMKEY, PROXY).create()
-        if self.botdata.source == "poe chatgpt4" or self.botdata.source == "poe claude-2-100k":
+        if (
+            self.botdata.source == "poe chatgpt4"
+            or self.botdata.source == "poe claude-2-100k"
+        ):
             if not SUBSCRIBE_ABLE:
                 raise Exception("Poe账户未订阅,无法使用订阅功能")
             if self.common_userinfo.user_id not in WHITE_LIST:
                 raise Exception("你不在poe订阅功能白名单内,无法使用订阅功能")
         if question in ["1", "2", "3"] and (
-                self.botdata.handle in CLIENT.bots.keys() and "Suggestion" in CLIENT.bots[self.botdata.handle] and
-                CLIENT.bots[self.botdata.handle]["Suggestion"]):
+            self.botdata.handle in CLIENT.bots.keys()
+            and "Suggestion" in CLIENT.bots[self.botdata.handle]
+            and CLIENT.bots[self.botdata.handle]["Suggestion"]
+        ):
             question = CLIENT.bots[self.botdata.handle]["Suggestion"][int(question) - 1]
         if self.botdata.prefix:
             question += self.botdata.prefix + "\n" + question
         if not self.botdata.handle:
             await self.refresh()
         try:
-            answer = ''
-            async for message in CLIENT.ask_stream(url_botname=self.botdata.handle, question=question,
-                                                   suggest_able=True):
+            answer = ""
+            async for message in CLIENT.ask_stream(
+                url_botname=self.botdata.handle,
+                question=question,
+                suggest_able=SUGGEST_ABLE,
+            ):
                 answer += message
             return answer
         except Exception as e:
             logger.error(f"Poe询问时出错:{str(e)}")
             raise Exception(f"Poe询问时出错:{str(e)}")
 
     async def refresh(self):
         global CLIENT
         if CLIENT is None:
             CLIENT = await Poe_Client(P_B, FORMKEY, PROXY).create()
-        if self.botdata.source == "poe chatgpt4" or self.botdata.source == "poe claude-2-100k":
+        if (
+            self.botdata.source == "poe chatgpt4"
+            or self.botdata.source == "poe claude-2-100k"
+        ):
             if not SUBSCRIBE_ABLE:
                 raise Exception("Poe账户未订阅,无法使用订阅功能")
             if self.common_userinfo.user_id not in WHITE_LIST:
                 raise Exception("你不在poe订阅功能白名单内,无法使用订阅功能")
         if not self.botdata.handle:
             try:
                 generated_uuid = uuid.uuid4()
                 self.botdata.handle = generated_uuid.hex.replace("-", "")[0:15]
-                await CLIENT.create_bot(self.botdata.handle, "无", base_model=self.botdata.model,
-                                        suggested_replies=SUGGEST_ABLE)
+                await CLIENT.create_bot(
+                    self.botdata.handle,
+                    "无",
+                    base_model=self.botdata.model,
+                    suggested_replies=True,
+                )
                 if self.botdata.prompt:
                     await CLIENT.send_message(self.botdata.handle, self.botdata.prompt)
                 common_users.save_userdata(self.common_userinfo)
             except Exception as e:
                 logger.error(f"Poe刷新对话时出错:{str(e)}")
                 raise Exception(f"Poe刷新对话时出错:{str(e)}")
         else:
```

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/slack_claude.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/slack_claude.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/spark_desk.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/spark_desk.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/sydneybing.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/sydneybing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/tongyiqianwen.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/Bard.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/Bard.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/BingImageCreator.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/BingImageCreator.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/chathub.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/chathub.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/constants.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation_style.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/conversation_style.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeGPT.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeGPT.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/EdgeUtils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/locale.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/locale.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/main.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/main.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/request.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/utilities.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/EdgeGPT/utilities.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/conversation_style.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPT.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/chatbot/utils/SydneyGPT/SydneyGPTUtils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/config.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/load_config.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/load_config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/mytypes.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/mytypes.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/prefix_data.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/prefix_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/prompt_data.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/prompt_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/user_data.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/user_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/app.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             "pic_able": PICABLE,
             "url_able": URLABLE,
             "wait_msg_able": '是否发送"正在思考\刷新,请稍等",默认True为发送,False为不发送',
             "num_limit": NUM_LIMIT,
             "private_command": "私人的bot的控制和使用前缀,默认‘/’",
             "public_command": "公用的bot的控制和使用前缀,默认‘.’",
             "pic_width": "文字转图片的宽度",
-            "show_name": "预设展示图和前缀展示图右侧显示的数字的多少"
+            "show_num": "预设列表和前缀列表展示的字数",
         },
         "Newbing配置": {
             "cookie": "Newbing的cookie json,获取方法为登录微软账号并打开到bing聊天界面,使用浏览器扩展 cookie editor将cookie导出为json格式并粘贴到此处",
             "proxy": "EdgeGPT的代理地址,请按照协议://地址:端口的格式填写",
             "wss_link": "EdgeGPT的wss_link地址,如果无法使用,可以自建cf代理,详细教程https://canxin121.github.io/docs/docs/Spark_GPT.html#QA中的第一个",
         },
         "Spark Desk配置": {
@@ -63,19 +63,19 @@
         "Claude Ai配置": {
             "cookie": "获取方式为打开https://claude.ai和开发者工具中的网络,和claude进行对话,并在append_message的请求中获取请求头中的cookie",
             "organization_uuid": "获取方式为登陆后打开https://claude.ai/api/organizations,并复制uuid一项的值,填写在此处",
             "proxy": "访问POE官网时使用的代理链接,请按照协议://地址:端口的格式填写",
         },
         "Poe配置": {
             "p_b": "获取方式为打开https://poe.com/,登录后F12打开开发者工具,在应用程序->cookie中复制p-b项的值,如l_recO0QgugqEyfgMbBc-g%3D%3D",
-            "formkey": "获取方式为打开https://poe.com/,登录后F12打开开发者工具,打开网络,然后向一个bot发消息,提取请求头中的formkey",
+            "formkey": "如果你没有安装node.js,请填写此项:获取方式为打开https://poe.com/,登录后F12打开开发者工具,打开网络,然后向一个bot发消息,提取请求头中的formkey",
             "suggest_able": "是否开启建议回复",
             "proxy": "访问POE官网时使用的代理链接,请按照协议://地址:端口的格式填写",
             "whitelist": "允许使用gpt4和claude2 100k的用户的列表,注意填写的是通用用户id,不是qq号或某平台id",
-            "subscribed": "账号是否为订阅账户,只有订阅账户才可使用gpt4 和 claude2 100k,否则将报错"
+            "subscribed": "账号是否为订阅账户,只有订阅账户才可使用gpt4 和 claude2 100k,否则将报错,True为是,任意值为否",
         },
         "Bard配置": {
             "__Secure-1PSID": "获取方式:打开Bard网页,打开开发者工具中的应用程序,选择其中的cookie,并且复制其中的__Secure-1PSID一项的值复制到这里",
             "__Secure-1PSIDTS": "获取方式:打开Bard网页,打开开发者工具中的应用程序,选择其中的cookie,并且复制其中的__Secure-1PSIDTS一项的值复制到这里",
             "proxy": "访问Bard官网时使用的代理链接,请按照协议://地址:端口的格式填写",
         },
         "通义千问配置": {
```

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/data/spark_gpt/common/config.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/templates/config.html` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/templates/config.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/templates/index.html` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/templates/prefix.html` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/templates/prefix.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/common/web/templates/prompt.html` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/common/web/templates/prompt.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/nonebot/bot_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from nonebot.exception import MatcherException
 from nonebot.matcher import Matcher
 from nonebot.params import ArgStr
 from nonebot.plugin import on_message
 from nonebot.typing import T_State
 
 require("nonebot_plugin_templates")
-from nonebot_plugin_templates.templates_render import colorlist_render
+from nonebot_plugin_templates.templates_render import dict_render
 
 from .utils import get_question_chatbot
 from .utils import (
     if_super_user,
     set_common_userinfo,
     set_public_common_userinfo,
     delete_messages,
@@ -124,16 +124,15 @@
             msg,
             matcher,
             bot,
             event,
         )
     )
     if not Generated_Source_Pic:
-        pic_bytes = await colorlist_render(source_des_dict, width=700, headline="来源列表", description="",
-                                           font_size=20)
+        pic_bytes = await dict_render(source_des_dict, width=450, title="来源列表")
         get_source_pic()
         with open(Source_Msg_Path, "wb") as f:
             f.write(pic_bytes)
     else:
         with open(Source_Msg_Path, "rb") as f:
             pic_bytes = f.read()
 
@@ -179,16 +178,15 @@
         state["replys"].append(
             await send_message(
                 msg, matcher, bot, event,
             )
         )
 
         if not prompts.Generated:
-            pic_bytes = await colorlist_render(prompts_dict, headline="预设列表", width=800,
-                                               description="")
+            pic_bytes = await dict_render(prompts_dict, title="预设列表", width=600)
             prompts.generate_pic()
             with open(Prompt_Msg_Path, "wb") as f:
                 f.write(pic_bytes)
         else:
             with open(Prompt_Msg_Path, "rb") as f:
                 pic_bytes = f.read()
 
@@ -245,16 +243,15 @@
 
         state["replys"].append(
             await send_message(
                 msg, matcher, bot, event
             )
         )
         if not prefixes.Generated:
-            pic_bytes = await colorlist_render(prefixes_dict, headline="前缀列表", width=800,
-                                               description="")
+            pic_bytes = await dict_render(prefixes_dict, title="前缀列表", width=600)
             prefixes.generate_pic()
             with open(Prefix_Msg_Path, "wb") as f:
                 f.write(pic_bytes)
         else:
             with open(Prefix_Msg_Path, "rb") as f:
                 pic_bytes = f.read()
         state["replys"].append(
@@ -349,74 +346,14 @@
         except MatcherException:
             await delete_messages(bot, event, state["replys"])
             raise
         except Exception as e:
             await send_message(str(e), matcher, bot, event)
             await matcher.finish()
 
-
-delete_bot = on_message(priority=1, block=False)
-
-
-@delete_bot.handle()
-async def delete_bot_(matcher: Matcher, event: MessageEvent, bot: Bot, state: T_State):
-    from ...common.load_config import PRIVATE_COMMAND, PUBLIC_COMMAND
-
-    if not event.get_plaintext().startswith(
-            (f"{PRIVATE_COMMAND}删除bot", f"{PUBLIC_COMMAND}删除bot")
-    ):
-        await matcher.finish()
-    if event.get_plaintext().startswith(PRIVATE_COMMAND):
-        state["common_userinfo"] = set_common_userinfo(event, bot)
-        plain_message = (
-            event.get_plaintext()
-            .replace(f"{PRIVATE_COMMAND}删除bot", "")
-            .replace(" ", "")
-        )
-    else:
-        await if_super_user(event, bot, matcher)
-        state["common_userinfo"] = set_public_common_userinfo(bot)
-        plain_message = (
-            event.get_plaintext().replace(f"{PUBLIC_COMMAND}删除bot", "").replace(" ", "")
-        )
-    state["replys"] = []
-    if not plain_message:
-        msg = "请输入bot的昵称,区分大小写\n输入'取消'或'算了'可以结束当前操作"
-        state["replys"].append(await send_message(msg, matcher, bot, event))
-
-    else:
-        matcher.set_arg("bot", plain_message)
-
-
-@delete_bot.got("bot")
-async def delete_bot__(
-        matcher: Matcher,
-        state: T_State,
-        bot: Bot,
-        event: MessageEvent,
-        args: str = ArgStr("bot"),
-):
-    await if_close(event, matcher, bot, state["replys"])
-    bot_name = str(args).replace("\n", "")
-    common_userinfo = state["common_userinfo"]
-    try:
-        common_users.delete_bot(
-            common_userinfo=common_userinfo,
-            botinfo=BotInfo(nickname=bot_name, owner=common_userinfo),
-        )
-        await send_message("成功删除了该bot", matcher, bot, event)
-        await matcher.finish()
-    except MatcherException:
-        await delete_messages(bot, event, state["replys"])
-        raise
-    except Exception as e:
-        await send_message(str(e), matcher, bot, event)
-        await matcher.finish()
-
-
 delete_bot = on_message(priority=1, block=False)
 
 
 @delete_bot.handle()
 async def delete_bot_(matcher: Matcher, event: MessageEvent, bot: Bot, state: T_State):
     from ...common.load_config import PRIVATE_COMMAND, PUBLIC_COMMAND
 
@@ -462,15 +399,14 @@
             common_userinfo=common_userinfo,
             botinfo=BotInfo(nickname=bot_name, owner=common_userinfo),
         )
         await send_message("成功删除了该bot", matcher, bot, event)
         await matcher.finish()
     except MatcherException:
         await delete_messages(bot, event, state["replys"])
-        raise
     except Exception as e:
         await send_message(str(e), matcher, bot, event)
         await matcher.finish()
 
 
 rename_bot = on_message(priority=1, block=False)
```

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/nonebot/config_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from nonebot.params import CommandStart
 from nonebot.plugin import on_command
 from nonebot.typing import T_State
 
 require("nonebot_plugin_templates")
 
 from nonebot_plugin_templates.template_types import *
-from nonebot_plugin_templates.templates_render import menu_render, colorlist_render
+from nonebot_plugin_templates.templates_render import menu_render, dict_render
 
 from .userlinks import users
 from .utils import (
     send_img,
     set_common_userinfo,
     set_userinfo,
     delete_messages,
@@ -253,16 +253,15 @@
 Prompt_Msg_Path.touch()
 
 
 @all_prompts.handle()
 async def all_prompts_(bot: Bot, matcher: Matcher, event: MessageEvent):
     prompts_dict = prompts.show_list()
     if not prompts.Generated:
-        pic_bytes = await colorlist_render(prompts_dict, headline="预设列表", width=800,
-                                           description="下面只展示了前200个字符")
+        pic_bytes = await dict_render(prompts_dict, title="预设列表", width=600)
         prompts.generate_pic()
         with open(Prompt_Msg_Path, "wb") as f:
             f.write(pic_bytes)
     else:
         with open(Prompt_Msg_Path, "rb") as f:
             pic_bytes = f.read()
     await send_img(
@@ -459,16 +458,15 @@
 Prefix_Msg_Path.touch()
 
 
 @all_prefixes.handle()
 async def all_prefixes_(bot: Bot, matcher: Matcher, event: MessageEvent):
     prefixes_dict = prefixes.show_list()
     if not prefixes.Generated:
-        pic_bytes = await colorlist_render(prefixes_dict, headline="前缀列表", width=800,
-                                           description="下面只展示了前200个字符")
+        pic_bytes = await dict_render(prefixes_dict, title="前缀列表", width=600)
         prefixes.generate_pic()
         with open(Prefix_Msg_Path, "wb") as f:
             f.write(pic_bytes)
     else:
         with open(Prefix_Msg_Path, "rb") as f:
             pic_bytes = f.read()
     await send_img(
```

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/nonebot/userlinks.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/nonebot/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/platforms/temp_bots.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/platforms/temp_bots.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,21 +125,22 @@
         else:
             raise Exception("没有这个messageid对应的bot")
 
     def get_bot_by_text(
             self, common_userinfo: CommonUserInfo, text: str
     ) -> tuple[str, CHATBOT]:
         """由原始的命令加bot名加问题得到问题和可调用的chatbot"""
+        from ..common.load_config import PRIVATE_COMMAND, PUBLIC_COMMAND
         try:
             botinfo, botdata = common_users.get_bot_by_text(common_userinfo, text)
-        except Exception as e:
+        except Exception:
             raise
 
-        question = text.replace(f"/{botinfo.nickname}", "").replace(
-            f".{botinfo.nickname}", ""
+        question = text.replace(f"{PRIVATE_COMMAND}{botinfo.nickname}", "").replace(
+            f"{PUBLIC_COMMAND}{botinfo.nickname}", ""
         )
         try:
             bot = self.get_bot_by_botinfo(
                 common_userinfo=common_userinfo, bot_info=botinfo
             )
         except:
             self.load_user_bot(
```

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/render.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/render.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.b64_fonts.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/katex/mathtex-script-type.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/markdown.css` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/markdown.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/markdown.html` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/markdown.html`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                 font-family: "Custom Font";
                 padding: 8px !important;
             }
         }
 
         .markdown-body::after {
             font-family: "Custom Font";
-            content: "Spark GPT 1.2.4";
+            content: "Spark GPT 1.2.5";
             font-size: 10px !important;
             font-weight: bold;
             color: black;
         }
     </style>
 </head>
```

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/templates/pygments-default.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/nonebot_plugin_spark_gpt/utils/utils.py` & `nonebot_plugin_spark_gpt-1.2.5/nonebot_plugin_spark_gpt/utils/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/pyproject.toml` & `nonebot_plugin_spark_gpt-1.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "nonebot_plugin_spark_gpt"
-version = "1.2.4"
+version = "1.2.5"
 description = "Spark-GPT,将多种来源的gpt接入qq,TG,Kook,Discord及更多平台,提供webui进行实时配置热更新,效率高超,使用便捷,管理完善,功能强大"
 authors = ["canxin121 <1969730106@qq.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_spark_gpt"},{ include = "nonebot"}]
 
 [tool.poetry.dependencies]
 nonebot-adapter-onebot = "^2.2.1"
 nonebot-adapter-telegram = "^0.1.0b6"
 nonebot-adapter-kaiheila = "^0.2.7"
 nonebot-plugin-htmlrender = "^0.2.1"
-nonebot-plugin-templates = "^0.1.4"
+nonebot-plugin-templates = "^0.1.5"
 python = "^3.10"
 aiohttp = "^3.8.4"
 bidict = "^0.22.1"
 edgegpt = "0.12.1"
 Sydneygpt = "0.11.8"
 fastapi = "^0.100.0"
 httpx = "^0.24.1"
-async-poe-client = "^0.1.6"
+async-poe-client = "^0.2.5"
 pydantic = "^1.10.9"
 slack-sdk = "^3.21.3"
 uvicorn = "^0.22.0"
 python-multipart = "^0.0.6"
 charset_normalizer = "^3.1.0"
 googlebard = "^1.4.0"
```

### Comparing `nonebot_plugin_spark_gpt-1.2.4/README.md` & `nonebot_plugin_spark_gpt-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_spark_gpt-1.2.4/PKG-INFO` & `nonebot_plugin_spark_gpt-1.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-spark-gpt
-Version: 1.2.4
+Version: 1.2.5
 Summary: Spark-GPT,将多种来源的gpt接入qq,TG,Kook,Discord及更多平台,提供webui进行实时配置热更新,效率高超,使用便捷,管理完善,功能强大
 Author: canxin121
 Author-email: 1969730106@qq.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Sydneygpt (==0.11.8)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: async-poe-client (>=0.1.6,<0.2.0)
+Requires-Dist: async-poe-client (>=0.2.5,<0.3.0)
 Requires-Dist: bidict (>=0.22.1,<0.23.0)
 Requires-Dist: charset_normalizer (>=3.1.0,<4.0.0)
 Requires-Dist: edgegpt (==0.12.1)
 Requires-Dist: fastapi (>=0.100.0,<0.101.0)
 Requires-Dist: googlebard (>=1.4.0,<2.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: nonebot-adapter-kaiheila (>=0.2.7,<0.3.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.1,<3.0.0)
 Requires-Dist: nonebot-adapter-telegram (>=0.1.0b6,<0.2.0)
 Requires-Dist: nonebot-plugin-htmlrender (>=0.2.1,<0.3.0)
-Requires-Dist: nonebot-plugin-templates (>=0.1.4,<0.2.0)
+Requires-Dist: nonebot-plugin-templates (>=0.1.5,<0.2.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: slack-sdk (>=3.21.3,<4.0.0)
 Requires-Dist: uvicorn (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 1.2.4 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-spark-gpt Version: 1.2.5 Summary:
 Spark-
 GPT,å°å¤ç§æ¥æºçgptæ¥å¥qq,TG,Kook,Discordåæ´å¤å¹³å°,æä¾webuiè¿è¡å®æ¶éç½®ç­æ´æ°,æçé«è¶,ä½¿ç¨ä¾¿æ·,ç®¡çå®å,åè½å¼ºå¤§
 Author: canxin121 Author-email: 1969730106@qq.com Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Sydneygpt (==0.11.8) Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: async-poe-client (>=0.1.6,<0.2.0) Requires-Dist: bidict
+Requires-Dist: async-poe-client (>=0.2.5,<0.3.0) Requires-Dist: bidict
 (>=0.22.1,<0.23.0) Requires-Dist: charset_normalizer (>=3.1.0,<4.0.0) Requires-
 Dist: edgegpt (==0.12.1) Requires-Dist: fastapi (>=0.100.0,<0.101.0) Requires-
 Dist: googlebard (>=1.4.0,<2.0.0) Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: nonebot-adapter-kaiheila (>=0.2.7,<0.3.0) Requires-Dist:
 nonebot-adapter-onebot (>=2.2.1,<3.0.0) Requires-Dist: nonebot-adapter-telegram
 (>=0.1.0b6,<0.2.0) Requires-Dist: nonebot-plugin-htmlrender (>=0.2.1,<0.3.0)
-Requires-Dist: nonebot-plugin-templates (>=0.1.4,<0.2.0) Requires-Dist:
+Requires-Dist: nonebot-plugin-templates (>=0.1.5,<0.2.0) Requires-Dist:
 pydantic (>=1.10.9,<2.0.0) Requires-Dist: python-multipart (>=0.0.6,<0.0.7)
 Requires-Dist: slack-sdk (>=3.21.3,<4.0.0) Requires-Dist: uvicorn
 (>=0.22.0,<0.23.0) Description-Content-Type: text/markdown
                 [https://socialify.git.ci/canxin121/Spark-GPT/
 image?font=Raleway&forks=1&issues=1&language=1&logo=https%3A%2F%2Fcanxin121.github.io%2Fdocs%2Flogo.png&name=1&owner=1&pattern=Charlie%20Brown&pulls=1&stargazers=1&theme=Auto]
                          ****** Spark-GPTä»åº ******
                                    Spark-GPT
```

