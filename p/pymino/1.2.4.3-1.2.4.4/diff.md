# Comparing `tmp/pymino-1.2.4.3.tar.gz` & `tmp/pymino-1.2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\ggg\pymino\dist\.tmp-vhw6q6o2\pymino-1.2.4.3.tar", last modified: Wed Jul 26 00:07:44 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.2.4.3\dist\.tmp-r8pqdr8w\pymino-1.2.4.4.tar", last modified: Wed Jul 26 00:18:29 2023, max compression
```

## Comparing `pymino-1.2.4.3.tar` & `pymino-1.2.4.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.114213 pymino-1.2.4.3/
--rw-rw-rw-   0        0        0     1085 2023-07-24 08:22:40.000000 pymino-1.2.4.3/LICENSE
--rw-rw-rw-   0        0        0     7373 2023-07-26 00:07:44.114213 pymino-1.2.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-07-26 00:07:16.000000 pymino-1.2.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.006580 pymino-1.2.4.3/pymino/
--rw-rw-rw-   0        0        0      952 2023-07-26 00:01:40.000000 pymino-1.2.4.3/pymino/__init__.py
--rw-rw-rw-   0        0        0    12297 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/async_bot.py
--rw-rw-rw-   0        0        0    38219 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/async_client.py
--rw-rw-rw-   0        0        0    38038 2023-07-26 00:02:14.000000 pymino-1.2.4.3/pymino/bot.py
--rw-rw-rw-   0        0        0    42332 2023-07-25 23:53:57.000000 pymino-1.2.4.3/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.058165 pymino-1.2.4.3/pymino/ext/
--rw-rw-rw-   0        0        0      638 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    11300 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/account.py
--rw-rw-rw-   0        0        0    11529 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_account.py
--rw-rw-rw-   0        0        0   345197 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    21402 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    25878 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0    72111 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_global_client.py
--rw-rw-rw-   0        0        0     7203 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   344131 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/console.py
--rw-rw-rw-   0        0        0    46013 2023-07-25 22:08:36.000000 pymino-1.2.4.3/pymino/ext/context.py
--rw-rw-rw-   0        0        0     2052 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.093876 pymino-1.2.4.3/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43827 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     5516 2023-07-25 22:58:58.000000 pymino-1.2.4.3/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1839 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    32584 2023-07-25 02:40:08.000000 pymino-1.2.4.3/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0    74405 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/global_client.py
--rw-rw-rw-   0        0        0      543 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     8182 2023-07-25 23:53:30.000000 pymino-1.2.4.3/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.111237 pymino-1.2.4.3/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11719 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6280 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1514 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10918 2023-07-25 23:59:39.000000 pymino-1.2.4.3/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.027909 pymino-1.2.4.3/pymino.egg-info/
--rw-rw-rw-   0        0        0     7373 2023-07-26 00:07:43.000000 pymino-1.2.4.3/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1618 2023-07-26 00:07:43.000000 pymino-1.2.4.3/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 00:07:43.000000 pymino-1.2.4.3/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-07-26 00:07:43.000000 pymino-1.2.4.3/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-26 00:07:43.000000 pymino-1.2.4.3/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      833 2023-07-26 00:07:44.118180 pymino-1.2.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-07-24 08:22:40.000000 pymino-1.2.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:18:29.496518 pymino-1.2.4.4/
+-rw-rw-rw-   0        0        0     1085 2023-07-24 08:22:40.000000 pymino-1.2.4.4/LICENSE
+-rw-rw-rw-   0        0        0     7373 2023-07-26 00:18:29.497014 pymino-1.2.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-07-26 00:07:16.000000 pymino-1.2.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 00:18:29.421127 pymino-1.2.4.4/pymino/
+-rw-rw-rw-   0        0        0      952 2023-07-26 00:16:26.000000 pymino-1.2.4.4/pymino/__init__.py
+-rw-rw-rw-   0        0        0    12297 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    38219 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/async_client.py
+-rw-rw-rw-   0        0        0    38038 2023-07-26 00:02:14.000000 pymino-1.2.4.4/pymino/bot.py
+-rw-rw-rw-   0        0        0    42305 2023-07-26 00:16:39.000000 pymino-1.2.4.4/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:18:29.457831 pymino-1.2.4.4/pymino/ext/
+-rw-rw-rw-   0        0        0      638 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11300 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/account.py
+-rw-rw-rw-   0        0        0    11529 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/async_account.py
+-rw-rw-rw-   0        0        0   345197 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    21402 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25878 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0    72111 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/async_global_client.py
+-rw-rw-rw-   0        0        0     7203 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   344131 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    46013 2023-07-25 22:08:36.000000 pymino-1.2.4.4/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     2052 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:18:29.483622 pymino-1.2.4.4/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43827 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     5516 2023-07-25 22:58:58.000000 pymino-1.2.4.4/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1839 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    32520 2023-07-26 00:16:53.000000 pymino-1.2.4.4/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0    75189 2023-07-26 00:18:02.000000 pymino-1.2.4.4/pymino/ext/global_client.py
+-rw-rw-rw-   0        0        0      543 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     8182 2023-07-25 23:53:30.000000 pymino-1.2.4.4/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:18:29.495526 pymino-1.2.4.4/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11719 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1514 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-07-24 08:22:40.000000 pymino-1.2.4.4/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10918 2023-07-25 23:59:39.000000 pymino-1.2.4.4/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:18:29.435510 pymino-1.2.4.4/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7373 2023-07-26 00:18:29.000000 pymino-1.2.4.4/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-07-26 00:18:29.000000 pymino-1.2.4.4/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 00:18:29.000000 pymino-1.2.4.4/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-07-26 00:18:29.000000 pymino-1.2.4.4/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 00:18:29.000000 pymino-1.2.4.4/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      833 2023-07-26 00:18:29.502967 pymino-1.2.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-07-24 08:22:40.000000 pymino-1.2.4.4/setup.py
```

### Comparing `pymino-1.2.4.3/LICENSE` & `pymino-1.2.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/PKG-INFO` & `pymino-1.2.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.4.3
+Version: 1.2.4.4
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.4.3 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.4.4 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `pymino-1.2.4.3/README.md` & `pymino-1.2.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/__init__.py` & `pymino-1.2.4.4/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from requests import get
 from colorama import Fore, Style
 
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.4.3'
+__version__ = '1.2.4.4'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot
 from .async_bot import AsyncBot
 from .client import Client
 from .async_client import AsyncClient
```

### Comparing `pymino-1.2.4.3/pymino/async_bot.py` & `pymino-1.2.4.4/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/async_client.py` & `pymino-1.2.4.4/pymino/async_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/bot.py` & `pymino-1.2.4.4/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/client.py` & `pymino-1.2.4.4/pymino/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -723,15 +723,14 @@
         self.request.userId: str = self.userId
         
         if hasattr(self.request, "email") and self._cached:
             cache_login(email=self.request.email, device=self.device_id, sid=self.sid)
 
         if not self.is_authenticated:
             self._is_authenticated = True
-            print("test")
             self._log(f"Logged in as {self.profile.username} ({self.profile.userId})")
         else:
             self._log(f"Reconnected as {self.profile.username} ({self.profile.userId})")
 
         if self.debug:
             print(f"{Fore.MAGENTA}Logged in as {self.profile.username} ({self.profile.userId}){Style.RESET_ALL}")
```

### Comparing `pymino-1.2.4.3/pymino/ext/__init__.py` & `pymino-1.2.4.4/pymino/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/account.py` & `pymino-1.2.4.4/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/async_account.py` & `pymino-1.2.4.4/pymino/ext/async_account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/async_community.py` & `pymino-1.2.4.4/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/async_context.py` & `pymino-1.2.4.4/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/async_event_handler.py` & `pymino-1.2.4.4/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/async_global_client.py` & `pymino-1.2.4.4/pymino/ext/async_global_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/async_socket.py` & `pymino-1.2.4.4/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/community.py` & `pymino-1.2.4.4/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/console.py` & `pymino-1.2.4.4/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/context.py` & `pymino-1.2.4.4/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/dispatcher.py` & `pymino-1.2.4.4/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/acm.py` & `pymino-1.2.4.4/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/admin_log.py` & `pymino-1.2.4.4/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/api_response.py` & `pymino-1.2.4.4/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/bubble.py` & `pymino-1.2.4.4/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/chat_threads.py` & `pymino-1.2.4.4/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/comments.py` & `pymino-1.2.4.4/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/enums.py` & `pymino-1.2.4.4/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/exceptions.py` & `pymino-1.2.4.4/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/general.py` & `pymino-1.2.4.4/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/handlers.py` & `pymino-1.2.4.4/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/link_info.py` & `pymino-1.2.4.4/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/member.py` & `pymino-1.2.4.4/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/messages.py` & `pymino-1.2.4.4/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/notification.py` & `pymino-1.2.4.4/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/sticker.py` & `pymino-1.2.4.4/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/threads.py` & `pymino-1.2.4.4/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/entities/userprofile.py` & `pymino-1.2.4.4/pymino/ext/entities/userprofile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1324,15 +1324,14 @@
 		self.ndcId:						List[int] = [x.ndcId for x in parser]
 		self.comId:						List[int] = self.ndcId
 		self.created_time:				List[str] = [x.created_time for x in parser]
 		#self.extensions:				List[UserExtensionsList] = [UserExtensionsList(self._data.get("extensions") for y in self._data) for x in parser]
 		self.visit_privacy:				List[int] = [x.visit_privacy for x in parser]
 		self.stories_count:				List[int] = [x.stories_count for x in parser]
 		self.blogs_count:				List[int] = [x.blogs_count for x in parser]
-		self.user_profile_count:		int = data.get("userProfileCount")
 
 class Pagging:
     def __init__(self, data: dict):
         self._data = data.get("paging") if isinstance(data, dict) else data
         self.prev_page_token = None
         self.next_page_token = None
```

### Comparing `pymino-1.2.4.3/pymino/ext/entities/wsevents.py` & `pymino-1.2.4.4/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/global_client.py` & `pymino-1.2.4.4/pymino/ext/global_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1922,8 +1922,27 @@
         >>> community_list = client.community.fetch_available_communities(start=0, size=10, language="en")
         >>> for name, comId in zip(community_list.name, community_list.comId):
         >>>     print(name, comId])
         """
         return CCommunityList(self.make_request(
             method = "GET",
             url = f"/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&start={start}&size={size}&pagingType=t"
+        ))
+
+
+    def unfollow(self, userId: str) -> ApiResponse:
+        """
+        Unfollows a user.
+        :param userId: The ID of the user to unfollow.
+        :type userId: str
+        :return: An ApiResponse object containing the response data from the API.
+        :rtype: ApiResponse
+        This function allows the logged-in user to unfollow another user specified by their ID.
+        After successful execution, the user will no longer be following the specified user.
+        **Example usage:**
+        >>> response = client.unfollow(userId="user123")
+        >>> print(response.status_code)
+        """
+        return ApiResponse(self.make_request(
+            method = "DELETE",
+            url = f"/g/s/user-profile/{userId}/member/{self.userId}"
         ))
```

### Comparing `pymino-1.2.4.3/pymino/ext/handle_queue.py` & `pymino-1.2.4.4/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/socket.py` & `pymino-1.2.4.4/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.4.4/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/utilities/chat_console.py` & `pymino-1.2.4.4/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/utilities/commands.py` & `pymino-1.2.4.4/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/utilities/community_console.py` & `pymino-1.2.4.4/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/utilities/generate.py` & `pymino-1.2.4.4/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/utilities/menu.py` & `pymino-1.2.4.4/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/utilities/profile_console.py` & `pymino-1.2.4.4/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino/ext/utilities/request_handler.py` & `pymino-1.2.4.4/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/pymino.egg-info/PKG-INFO` & `pymino-1.2.4.4/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.4.3
+Version: 1.2.4.4
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.2.4.3 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.4.4 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `pymino-1.2.4.3/pymino.egg-info/SOURCES.txt` & `pymino-1.2.4.4/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.3/setup.cfg` & `pymino-1.2.4.4/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e34 2e33 0d0a 6175  on = 1.2.4.3..au
+00000020: 6f6e 203d 2031 2e32 2e34 2e34 0d0a 6175  on = 1.2.4.4..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.4.3/setup.py` & `pymino-1.2.4.4/setup.py`

 * *Files identical despite different names*

