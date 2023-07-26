# Comparing `tmp/pymino-1.2.4.2.tar.gz` & `tmp/pymino-1.2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymino-1.2.4.2.tar", last modified: Tue Jul 25 19:30:35 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\ggg\pymino\dist\.tmp-vhw6q6o2\pymino-1.2.4.3.tar", last modified: Wed Jul 26 00:07:44 2023, max compression
```

## Comparing `pymino-1.2.4.2.tar` & `pymino-1.2.4.3.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.486045 pymino-1.2.4.2/
--rw-rw-rw-   0        0        0     1085 2023-07-14 23:58:40.000000 pymino-1.2.4.2/LICENSE
--rw-rw-rw-   0        0        0     7373 2023-07-25 19:30:35.486045 pymino-1.2.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     6706 2023-07-25 19:30:17.000000 pymino-1.2.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.414048 pymino-1.2.4.2/pymino/
--rw-rw-rw-   0        0        0      952 2023-07-25 19:16:15.000000 pymino-1.2.4.2/pymino/__init__.py
--rw-rw-rw-   0        0        0    12297 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/async_bot.py
--rw-rw-rw-   0        0        0    38219 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/async_client.py
--rw-rw-rw-   0        0        0    32248 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/bot.py
--rw-rw-rw-   0        0        0    37736 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.439179 pymino-1.2.4.2/pymino/ext/
--rw-rw-rw-   0        0        0      638 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0      192 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/_global.py
--rw-rw-rw-   0        0        0    11300 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/account.py
--rw-rw-rw-   0        0        0    11529 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/async_account.py
--rw-rw-rw-   0        0        0   345197 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    21402 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    25878 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0    72111 2023-07-20 02:29:35.000000 pymino-1.2.4.2/pymino/ext/async_global_client.py
--rw-rw-rw-   0        0        0     7203 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   344131 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/community.py
--rw-rw-rw-   0        0        0     3040 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/console.py
--rw-rw-rw-   0        0        0    45520 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/context.py
--rw-rw-rw-   0        0        0     2052 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.470455 pymino-1.2.4.2/pymino/ext/entities/
--rw-rw-rw-   0        0        0      428 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0     8044 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/acm.py
--rw-rw-rw-   0        0        0     9014 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/admin_log.py
--rw-rw-rw-   0        0        0     1670 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/api_response.py
--rw-rw-rw-   0        0        0    17769 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/bubble.py
--rw-rw-rw-   0        0        0    20322 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/chat_threads.py
--rw-rw-rw-   0        0        0    13223 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/comments.py
--rw-rw-rw-   0        0        0      765 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    16021 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    43827 2023-07-20 01:14:10.000000 pymino-1.2.4.2/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     5516 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0     5127 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/link_info.py
--rw-rw-rw-   0        0        0     3831 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/member.py
--rw-rw-rw-   0        0        0    42520 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     1839 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/notification.py
--rw-rw-rw-   0        0        0    31711 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/sticker.py
--rw-rw-rw-   0        0        0     6185 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    32492 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0    75199 2023-07-25 19:15:48.000000 pymino-1.2.4.2/pymino/ext/global_client.py
--rw-rw-rw-   0        0        0      543 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     6609 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.470455 pymino-1.2.4.2/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      234 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11719 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0    11309 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/chat_console.py
--rw-rw-rw-   0        0        0     6280 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     2078 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/community_console.py
--rw-rw-rw-   0        0        0     1514 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0     2911 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/menu.py
--rw-rw-rw-   0        0        0     2106 2023-07-14 23:58:40.000000 pymino-1.2.4.2/pymino/ext/utilities/profile_console.py
--rw-rw-rw-   0        0        0    10853 2023-07-25 18:46:41.000000 pymino-1.2.4.2/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:30:35.423555 pymino-1.2.4.2/pymino.egg-info/
--rw-rw-rw-   0        0        0     7373 2023-07-25 19:30:35.000000 pymino-1.2.4.2/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1640 2023-07-25 19:30:35.000000 pymino-1.2.4.2/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 19:30:35.000000 pymino-1.2.4.2/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-07-25 19:30:35.000000 pymino-1.2.4.2/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-25 19:30:35.000000 pymino-1.2.4.2/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      833 2023-07-25 19:30:35.486045 pymino-1.2.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-07-25 18:46:41.000000 pymino-1.2.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.114213 pymino-1.2.4.3/
+-rw-rw-rw-   0        0        0     1085 2023-07-24 08:22:40.000000 pymino-1.2.4.3/LICENSE
+-rw-rw-rw-   0        0        0     7373 2023-07-26 00:07:44.114213 pymino-1.2.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6706 2023-07-26 00:07:16.000000 pymino-1.2.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.006580 pymino-1.2.4.3/pymino/
+-rw-rw-rw-   0        0        0      952 2023-07-26 00:01:40.000000 pymino-1.2.4.3/pymino/__init__.py
+-rw-rw-rw-   0        0        0    12297 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    38219 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/async_client.py
+-rw-rw-rw-   0        0        0    38038 2023-07-26 00:02:14.000000 pymino-1.2.4.3/pymino/bot.py
+-rw-rw-rw-   0        0        0    42332 2023-07-25 23:53:57.000000 pymino-1.2.4.3/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.058165 pymino-1.2.4.3/pymino/ext/
+-rw-rw-rw-   0        0        0      638 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11300 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/account.py
+-rw-rw-rw-   0        0        0    11529 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_account.py
+-rw-rw-rw-   0        0        0   345197 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    21402 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    25878 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0    72111 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_global_client.py
+-rw-rw-rw-   0        0        0     7203 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   344131 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/community.py
+-rw-rw-rw-   0        0        0     3040 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/console.py
+-rw-rw-rw-   0        0        0    46013 2023-07-25 22:08:36.000000 pymino-1.2.4.3/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     2052 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.093876 pymino-1.2.4.3/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      428 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0     8044 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/acm.py
+-rw-rw-rw-   0        0        0     9014 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/admin_log.py
+-rw-rw-rw-   0        0        0     1670 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/api_response.py
+-rw-rw-rw-   0        0        0    17769 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/bubble.py
+-rw-rw-rw-   0        0        0    20322 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/chat_threads.py
+-rw-rw-rw-   0        0        0    13223 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/comments.py
+-rw-rw-rw-   0        0        0      765 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    16021 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    43827 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     5516 2023-07-25 22:58:58.000000 pymino-1.2.4.3/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0     5127 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/link_info.py
+-rw-rw-rw-   0        0        0     3831 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/member.py
+-rw-rw-rw-   0        0        0    42520 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     1839 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/notification.py
+-rw-rw-rw-   0        0        0    31711 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/sticker.py
+-rw-rw-rw-   0        0        0     6185 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    32584 2023-07-25 02:40:08.000000 pymino-1.2.4.3/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0    74405 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/global_client.py
+-rw-rw-rw-   0        0        0      543 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     8182 2023-07-25 23:53:30.000000 pymino-1.2.4.3/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.111237 pymino-1.2.4.3/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      234 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11719 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0    11309 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/chat_console.py
+-rw-rw-rw-   0        0        0     6280 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     2078 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/community_console.py
+-rw-rw-rw-   0        0        0     1514 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0     2911 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/menu.py
+-rw-rw-rw-   0        0        0     2106 2023-07-24 08:22:40.000000 pymino-1.2.4.3/pymino/ext/utilities/profile_console.py
+-rw-rw-rw-   0        0        0    10918 2023-07-25 23:59:39.000000 pymino-1.2.4.3/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:07:44.027909 pymino-1.2.4.3/pymino.egg-info/
+-rw-rw-rw-   0        0        0     7373 2023-07-26 00:07:43.000000 pymino-1.2.4.3/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-07-26 00:07:43.000000 pymino-1.2.4.3/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 00:07:43.000000 pymino-1.2.4.3/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-07-26 00:07:43.000000 pymino-1.2.4.3/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 00:07:43.000000 pymino-1.2.4.3/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      833 2023-07-26 00:07:44.118180 pymino-1.2.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-07-24 08:22:40.000000 pymino-1.2.4.3/setup.py
```

### Comparing `pymino-1.2.4.2/LICENSE` & `pymino-1.2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/PKG-INFO` & `pymino-1.2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.4.2
+Version: 1.2.4.3
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
-Metadata-Version: 2.1 Name: pymino Version: 1.2.4.2 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.4.3 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `pymino-1.2.4.2/README.md` & `pymino-1.2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/__init__.py` & `pymino-1.2.4.3/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from requests import get
 from colorama import Fore, Style
 
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.2.4.2'
+__version__ = '1.2.4.3'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot
 from .async_bot import AsyncBot
 from .client import Client
 from .async_client import AsyncClient
```

### Comparing `pymino-1.2.4.2/pymino/async_bot.py` & `pymino-1.2.4.3/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/async_client.py` & `pymino-1.2.4.3/pymino/async_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/bot.py` & `pymino-1.2.4.3/pymino/bot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,100 @@
 from threading import Thread
 from typing import Optional, Union
 from time import perf_counter, time
+from logging import FileHandler, Logger, getLogger, Formatter, DEBUG
 
 from .ext.console import *
 from .ext.entities import *
-from .ext.socket import WSClient
-from .ext.global_client import Global
 from .ext.account import Account
+from .ext.socket import WSClient
 from .ext.community import Community
+from .ext.global_client import Global
 from .ext.utilities.generate import Generator
 from .ext.utilities.request_handler import RequestHandler
 
+__all__ = (
+    'Bot',
+)
+
 
 class Bot(WSClient, Global):
+    """
+    Bot class that interacts with aminoapps API.
+
+    This class extends `WSClient` and `Global` classes, allowing the bot to use WebSocket functionality and global client features.
+
+    Special Attributes:
+    __slots__ : tuple
+        A tuple containing a fixed set of attributes to optimize memory usage.
+
+    Attributes:
+    _debug : bool
+        Whether or not debug mode is enabled.
+    _console_enabled : bool
+        Whether or not the CONSOLE is enabled.
+    _cooldown_message : str
+        The default cooldown message used when a command is on cooldown.
+    _intents : bool
+        Whether or not intents are enabled.
+    _is_ready : bool
+        Whether the bot is ready after successful login.
+    _userId : str
+        The ID of the user associated with the bot.
+    _sid : str
+        The session ID of the client.
+    _cached : bool
+        Whether the login credentials are cached.
+    logger : Logger
+        The logger object.
+    cache : Cache
+        An instance of the Cache class for caching data.
+    command_prefix : Optional[str]
+        The prefix used for bot commands.
+    community_id : Union[str, int]
+        The ID of the community associated with the bot.
+    generate : Generator
+        An instance of the Generator class for generating data.
+    online_status : bool
+        Whether the bot's online status is enabled.
+    device_id : Optional[str]
+        The device ID used for logging in. If not provided, it will be generated using the Generator class.
+    _is_authenticated : bool
+        Whether the bot is authenticated.
+    request : RequestHandler
+        An instance of the RequestHandler class for handling API requests.
+    community : Community
+        An instance of the Community class for community-related actions.
+    account : Account
+        An instance of the Account class for account-related actions.
+    profile : UserProfile
+        An instance of the UserProfile class representing the bot's user profile.
+    """
+    __slots__ = (
+        '_debug',
+        '_console_enabled',
+        '_cooldown_message',
+        '_intents',
+        '_is_ready',
+        '_userId',
+        '_sid',
+        '_cached',
+        'cache',
+        'logger',
+        'command_prefix',
+        'community_id',
+        'generate',
+        'online_status',
+        'device_id',
+        '_is_authenticated'
+        'request',
+        'community',
+        'account',
+        'profile',
+    )
     def __init__(
         self,
         command_prefix: Optional[str] = "!",
         community_id: Union[str, int] = None,
         console_enabled: bool = False,
         device_id: str = None,
         intents: bool = False,
@@ -223,28 +301,30 @@
                 ctx.send("Pong!")
 
             bot.run(email="email", password="password")
             ```
         """
         self._debug:            bool = check_debugger()
         self._console_enabled:  bool = console_enabled
-        self._cooldown_message  = None
+        self._cooldown_message: Optional[str] = None
+        self._is_authenticated: bool = False
         self._intents:          bool = intents
         self._is_ready:         bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
         self.cache:             Cache = Cache("cache")
 
         self.command_prefix:    Optional[str] = command_prefix
         if self.command_prefix == "":
             raise InvalidCommandPrefix()
         
+        self.logger:            Optional[Logger] = self._create_logger()
         self.community_id:      Union[str, int] = community_id
-        self.generate           = Generator(hash_prefix, device_key, signature_key)
+        self.generate:          Generator = Generator(hash_prefix, device_key, signature_key)
         self.online_status:     bool = online_status
         self.device_id:         Optional[str] = device_id or self.generate.device_id()
         self.request:           RequestHandler = RequestHandler(
                                 bot = self,
                                 proxy=proxy,
                                 generator=self.generate
                                 )
@@ -257,14 +337,40 @@
                                 session=self.request
                                 )
 
         if self.community_id:   self.set_community_id(community_id)
 
         super().__init__()
 
+    def __repr__(self):
+        """
+        Returns a string representation of the Bot object.
+
+        :return: A string representation of the Bot object.
+        :rtype: str
+        """
+        return f"Bot(command_prefix='{self.command_prefix}', community_id={self.community_id}, device_id='{self.device_id}')"
+
+    def __str__(self):
+        """
+        Returns a user-friendly string representation of the Bot object.
+
+        :return: A user-friendly string representation of the Bot object.
+        :rtype: str
+        """
+        return f"Bot: Prefix='{self.command_prefix}', Community ID={self.community_id}, Device ID='{self.device_id}'"
+
+    def __iter__(self) -> iter:
+        """
+        Allows iteration over the Bot object.
+
+        :return: An iterator for the Bot object.
+        :rtype: iter
+        """
+        return iter(self.__slots__)
 
     @property
     def debug(self) -> bool:
         """
         Whether or not debug mode is enabled.
 
         :return: True if debug mode is enabled, False otherwise.
@@ -273,15 +379,14 @@
         This property returns whether or not debug mode is enabled. Debug mode can be used to enable additional logging and
         debug information during development.
 
         **Note:** This property only returns the debug mode state and cannot be used to set the debug mode state. To set the
         debug mode state, use the `self._debug` attribute directly.
         """
         return self._debug
-    
 
     @debug.setter
     def debug(self, value: bool) -> None:
         """
         Sets the debug mode state.
 
         :param value: True to enable debug mode, False to disable it.
@@ -292,15 +397,14 @@
         during development.
 
         **Note:** This setter only sets the debug mode state and cannot be used to retrieve the debug mode state. To retrieve
         the debug mode state, use the `self.debug` property.
         """
         self._debug = value
 
-    
     @property
     def console_enabled(self) -> bool:
         """
         Whether or not the CONSOLE is enabled.
 
         :return: True if the CONSOLE is enabled, False otherwise.
         :rtype: bool
@@ -308,15 +412,14 @@
         This property returns whether or not the CONSOLE is enabled. The CONSOLE can be used to interact with the bot and access
         additional features such as the console.
 
         **Note:** This property only returns the CONSOLE state and cannot be used to set the CONSOLE state. To set the CONSOLE state, use
         the `self._console_enabled` attribute directly.
         """
         return self._console_enabled
-    
 
     @console_enabled.setter
     def console_enabled(self, value: bool) -> None:
         """
         Sets the CONSOLE state.
 
         :param value: True to enable the CONSOLE, False to disable it.
@@ -327,15 +430,14 @@
         the console.
 
         **Note:** This setter only sets the CONSOLE state and cannot be used to retrieve the CONSOLE state. To retrieve the CONSOLE state,
         use the `self.console_enabled` property.
         """
         self._console_enabled = value
 
-
     @property
     def intents(self) -> bool:
         """
         Whether or not intents are enabled.
 
         :return: True if intents are enabled, False otherwise.
         :rtype: bool
@@ -343,15 +445,14 @@
         This property returns whether or not intents are enabled. Intents allow the bot to use additional features such as
         `ctx.wait_for_message()`.
 
         **Note:** This property only returns the intents state and cannot be used to set the intents state. To set the intents
         state, use the `self._intents` attribute directly.
         """
         return self._intents
-    
 
     @intents.setter
     def intents(self, value: bool) -> None:
         """
         Sets the intents state.
 
         :param value: True to enable intents, False to disable them.
@@ -361,15 +462,14 @@
         This setter sets the intents state. Intents allow the bot to use additional features such as `ctx.wait_for_message()`.
 
         **Note:** This setter only sets the intents state and cannot be used to retrieve the intents state. To retrieve the
         intents state, use the `self.intents` property.
         """
         self._intents = value
 
-
     @property
     def is_ready(self) -> bool:
         """
         Whether or not the bot is ready.
 
         :return: True if the bot is ready, False otherwise.
         :rtype: bool
@@ -377,15 +477,14 @@
         This property returns whether or not the bot is ready. The bot is ready after logging in to
         Amino and receiving a valid session ID.
 
         **Note:** This property only returns the authentication state and cannot be used to set the authentication state. To
         set the authentication state, use the `self._is_ready` attribute directly.
         """
         return self._is_ready
-    
 
     @is_ready.setter
     def is_ready(self, value: bool) -> None:
         """
         Sets the `is_ready` state of the client.
 
         :param value: True to set the client as ready, False to set it as not ready.
@@ -396,15 +495,14 @@
         receiving a valid session ID.
 
         **Note:** This setter only sets the authentication state and cannot be used to retrieve the authentication state. To
         retrieve the authentication state, use the `self.is_ready` property.
         """
         self._is_ready = value
 
-
     @property
     def userId(self) -> str:
         """
         The ID of the user associated with the client.
 
         :return: The ID of the user.
         :rtype: str
@@ -413,15 +511,14 @@
         Amino, and can be used to make API calls related to the user, such as retrieving the user's profile or posts.
 
         **Note:** This property only returns the user ID and cannot be used to set the user ID. To set the user ID, use the
         `self._userId` attribute directly.
         """
         return self._userId
 
-
     @userId.setter
     def userId(self, value: str) -> None: # Human is gay.
         """
         Sets the ID of the user associated with the client.
 
         :param value: The ID of the user to set.
         :type value: str
@@ -431,15 +528,14 @@
         user, such as retrieving the user's profile or posts.
 
         **Note:** This setter only sets the user ID and cannot be used to retrieve the user ID. To retrieve the user ID, use
         the `self.userId` property.
         """
         self._userId = value
 
-        
     @property
     def sid(self) -> str:
         """
         The session ID of the client.
 
         :return: The session ID.
         :rtype: str
@@ -448,15 +544,14 @@
         used to make authenticated API calls, such as posting messages or retrieving user information.
 
         **Note:** This property only returns the session ID and cannot be used to set the session ID. To set the session ID,
         use the `self._sid` attribute directly.
         """
         return self._sid
 
-
     @sid.setter
     def sid(self, value: str) -> None:
         """
         Sets the session ID of the client.
 
         :param value: The session ID to set.
         :type value: str
@@ -466,29 +561,82 @@
         posting messages or retrieving user information.
 
         **Note:** This setter only sets the session ID and cannot be used to retrieve the session ID. To retrieve the session
         ID, use the `self.sid` property.
         """
         self._sid = value
 
-    
     def set_cooldown_message(self, message: str) -> None:
         """
         Changes the default cooldown message.
         
         :param message: The message to set as the default cooldown message.
         :type message: str
         :return: None
         
         This method changes the default cooldown message. The default cooldown message is used when a command is on cooldown
         
         **Note:** This method only sets the default cooldown message and cannot be used to retrieve the default cooldown message.
         """
         self._cooldown_message = message
 
+    @property
+    def is_authenticated(self) -> bool:
+        """
+        Whether or not the client is authenticated.
+
+        :return: True if the client is authenticated, False otherwise.
+        :rtype: bool
+
+        This property returns whether or not the client is authenticated. The client is authenticated after logging in to
+        Amino and receiving a valid session ID.
+
+        **Note:** This property only returns the authentication state and cannot be used to set the authentication state. To
+        set the authentication state, use the `self._is_authenticated` attribute directly.
+        """
+        return self._is_authenticated
+
+    @is_authenticated.setter
+    def is_authenticated(self, value: bool) -> None:
+        """
+        Sets the authentication state of the client.
+
+        :param value: True to authenticate the client, False to deauthenticate it.
+        :type value: bool
+        :return: None
+
+        This setter sets the authentication state of the client. The client is authenticated after logging in to Amino and
+        receiving a valid session ID.
+
+        **Note:** This setter only sets the authentication state and cannot be used to retrieve the authentication state. To
+        retrieve the authentication state, use the `self.is_authenticated` property.
+        """
+        self._is_authenticated = value
+
+    def _create_logger(self) -> Logger:
+        """
+        Creates a logger object.
+        
+        :return: A logger object.
+        :rtype: Logger
+        
+        This method creates a logger object. The logger object is used to log debug information to debug.log.
+        """
+        logger = getLogger("pymino")
+        logger.setLevel(DEBUG)
+
+        file_handler = FileHandler("debug.log")
+        file_handler.setLevel(DEBUG)
+
+        formatter = Formatter("%(asctime)s - %(levelname)s - %(message)s")
+        file_handler.setFormatter(formatter)
+
+        logger.addHandler(file_handler)
+
+        return logger
 
     def authenticate(self, email: str, password: str, device_id: str=None) -> dict:
         """
         Authenticates the bot with the provided email and password.
 
         :param email: The email to use to log in.
         :type email: str
@@ -518,15 +666,14 @@
                 "deviceID": self.device_id,
                 "email": email,
                 "v": 2,
                 "clientCallbackURL": "narviiapp://default"
                 }
             )).json()
 
-
     def _login_handler(self, email: str, password: str, device_id: str=None, use_cache: bool=True) -> dict:
         """
         Authenticates the user with the provided email and password.
 
         :param email: The email address associated with the account.
         :type email: str
         :param password: The password for the account.
@@ -575,15 +722,14 @@
                 )
 
         for key, value in {"email": email, "password": password}.items():
             setattr(self.request, key, value)            
 
         return response
 
-
     def run(
         self,
         email: Optional[str] = None,
         password: Optional[str] = None,
         sid: Optional[str] = None,
         device_id: Optional[str] = None,
         use_cache: bool = True
@@ -630,15 +776,14 @@
                 )
 
         if not response:
             raise LoginFailed
 
         return self._run(response)
 
-
     def _run(self, response: dict) -> dict:
         """
         Processes the response from a successful login attempt and sets up the authenticated client.
 
         :param response: The response from the login attempt.
         :type response: dict
         :return: The response from the login attempt.
@@ -666,36 +811,37 @@
         if not self.sid:
             self.sid: str = response["sid"]
 
         self.userId: str = self.profile.userId
         self.community.userId: str = self.userId
         self.request.sid: str = self.sid
         self.request.userId: str = self.userId
-        self.is_authenticated: bool = True
-
+        
         if hasattr(self.request, "email") and self._cached:
             cache_login(email=self.request.email, device=self.device_id, sid=self.sid)
 
         if not self.is_ready:
             self._is_ready = True
+            self._is_authenticated = True
+            self._log(f"Logged in as {self.profile.username} ({self.profile.userId})")
             self.connect()
+        else:
+            self._log(f"Reconnected as {self.profile.username} ({self.profile.userId})")
 
         if self.debug:
             print(f"{Fore.MAGENTA}Logged in as {self.profile.username} ({self.profile.userId}){Style.RESET_ALL}")
 
         Thread(target=self.__run_console__).start()
         return response
 
-    
     def __run_console__(self) -> None:
         if self.console_enabled:
             self._debug = False
             Console(self).fetch_menu()
 
-
     def fetch_account(self) -> dict:
         """
         Fetches the account information for the authenticated user.
 
         :return: A dictionary containing the user's account information.
         :rtype: dict
 
@@ -714,15 +860,14 @@
             self.request.handler(
                 method="GET",
                 url=f"/g/s/user-profile/{self.userId}"
                 ))
         
         return ApiResponse(self.request.handler(method="GET", url="/g/s/account")).json()
 
-
     def fetch_community_id(self, community_link: str, set_community_id: Optional[bool] = True) -> int:
         """
         Fetches the community ID associated with the provided community link.
 
         :param community_link: The community link for which to fetch the ID.
         :type community_link: str
         :param set_community_id: Whether or not to set the fetched community ID on the client instance. Defaults to True.
@@ -751,15 +896,14 @@
         community_id = self.cache.get(KEY)
 
         if set_community_id:
             self.set_community_id(community_id)
 
         return community_id
 
-
     def set_community_id(self, community_id: Union[str, int]) -> int:
         """
         Sets the community ID on the client instance and the Community object.
 
         :param community_id: The community ID to set.
         :type community_id: Union[str, int]
         :return: The community ID that was set.
@@ -783,15 +927,14 @@
             raise VerifyCommunityIdIsCorrect from e
 
         self.community_id = community_id
         self.community.community_id = community_id
 
         return community_id
 
-
     def ping(self) -> float:
         """
         Pings the server and returns the elapsed time in milliseconds.
         
         :return: The elapsed time in milliseconds.
         :rtype: float
```

### Comparing `pymino-1.2.4.2/pymino/client.py` & `pymino-1.2.4.3/pymino/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,136 +1,201 @@
 from time import time
 from typing import Any, Callable, Optional, TypeVar, Union
+from logging import FileHandler, Logger, getLogger, Formatter, DEBUG
 
 from .ext.entities import *
 from .ext.global_client import Global
 from .ext.utilities.generate import Generator
 from .ext import RequestHandler, Account, Community
 
-
 F = TypeVar("F", bound=Callable[..., Any])
 
+__all__ = (
+    "Client",
+)
+
+
 class Client(Global):
     """
-    `Client` - This is the main client.
+    Bot class that interacts with aminoapps API.
 
-    `**Parameters**``
-    - `**kwargs` - any other parameters to use for the client.
-    - `device_id` - device id to use for the client.
-    - `proxy` - proxy string to use for the client.
-    - `hash_prefix` - The hash prefix to use for the bot. `Defaults` to `19`.
-    - `device_key` - The device key to use for the bot. `Defaults` to `E7309ECC0953C6FA60005B2765F99DBBC965C8E9`.
-    - `signature_key` - The signature key to use for the bot. `Defaults` to `DFA5ED192DDA6E88A12FE12130DC6206B1251E44`.
-    
-    ----------------------------
-    Why use `Client` over `Bot`?
+    This class extends `Global` classes, allowing the client to access all global client features.
 
-    - Used for scripts rather than bots.
-    - Lightweight, does not utilize websocket.
+    Special Attributes:
+    __slots__ : tuple
+        A tuple containing a fixed set of attributes to optimize memory usage.
 
-    ----------------------------
-    Do I have to be logged in to use `Client`?
+    Attributes:
+    _debug : bool
+        Whether or not debug mode is enabled.
+    _userId : str
+        The ID of the user associated with the bot.
+    _sid : str
+        The session ID of the client.
+    _cached : bool
+        Whether the login credentials are cached.
+    _is_authenticated : bool
+        Whether or not the client is authenticated.
+    cache : Cache
+        An instance of the Cache class for caching data.
+    logger : Logger
+        An instance of the Logger class for logging.
+    is_logging : bool
+        Whether or not logging is enabled.
+    community_id : Union[str, int]
+        The ID of the community associated with the bot.
+    generate : Generator
+        An instance of the Generator class for generating data.
+    device_id : Optional[str]
+        The device ID used for logging in. If not provided, it will be generated using the Generator class.
+    request : RequestHandler
+        An instance of the RequestHandler class for handling API requests.
+    account : Account
+        An instance of the Account class for account-related actions.
+    community : Community
+        An instance of the Community class for community-related actions.
+    profile : UserProfile
+        An instance of the UserProfile class representing the bot's user profile.
+    """
+    __slots__ = (
+        '_debug',
+        '_userId',
+        '_sid',
+        '_cached',
+        '_is_authenticated',
+        'cache',
+        'logger',
+        'is_logging'
+        'community_id',
+        'generate',
+        'device_id',
+        'request',
+        'account',
+        'community',
+        'profile'
+    )
+    def __init__(
+        self,
+        community_id: Optional[Union[str, int]] = None,
+        hash_prefix: Union[str, int] = 19,
+        device_key: str = "E7309ECC0953C6FA60005B2765F99DBBC965C8E9",
+        signature_key: str  = "DFA5ED192DDA6E88A12FE12130DC6206B1251E44",
+        **kwargs
+        ) -> None:
+        """
+        `Client` - This is the main client.
 
-    - No, you do not have to be logged in to use `Client`.
-    - However, you will not be able to use any methods that require authentication.
+        `**Parameters**``
+        - `**kwargs` - any other parameters to use for the client.
+        - `device_id` - device id to use for the client.
+        - `proxy` - proxy string to use for the client.
+        - `hash_prefix` - The hash prefix to use for the bot. `Defaults` to `19`.
+        - `device_key` - The device key to use for the bot. `Defaults` to `E7309ECC0953C6FA60005B2765F99DBBC965C8E9`.
+        - `signature_key` - The signature key to use for the bot. `Defaults` to `DFA5ED192DDA6E88A12FE12130DC6206B1251E44`.
+        
+        ----------------------------
+        Why use `Client` over `Bot`?
 
-    `**NON-AUTH EXAMPLE**`
-    ```python
-    # This method does not require authentication, so it will work without logging in.    
+        - Used for scripts rather than bots.
+        - Lightweight, does not utilize websocket.
 
-    from pymino import Client
+        ----------------------------
+        Do I have to be logged in to use `Client`?
 
-    client = Client()
+        - No, you do not have to be logged in to use `Client`.
+        - However, you will not be able to use any methods that require authentication.
 
-    print(f"Logged in: {client.is_authenticated}")
+        `**NON-AUTH EXAMPLE**`
+        ```python
+        # This method does not require authentication, so it will work without logging in.    
 
-    chat_id = client.community.fetch_object_id(link="https://aminoapps.com/p/123456789")
+        from pymino import Client
 
-    print(f"Chat ID: {chat_id}")
-    ```
-    ----------------------------
+        client = Client()
 
-    How do I login with `Client`?
-        - You can login with `Client` by using the `login` method.
-        
-    `**Login Example**`
+        print(f"Logged in: {client.is_authenticated}")
 
-    ```python
-    from pymino import Client
+        chat_id = client.community.fetch_object_id(link="https://aminoapps.com/p/123456789")
 
-    client = Client()
+        print(f"Chat ID: {chat_id}")
+        ```
+        ----------------------------
 
-    client.login(email="email", password="password")
+        How do I login with `Client`?
+            - You can login with `Client` by using the `login` method.
+            
+        `**Login Example**`
 
-    print(f"Logged in: {client.is_authenticated}")
+        ```python
+        from pymino import Client
 
-    # Output: Logged in: True
-    ```
-    ----------------------------
-    How can I utilize community methods with `Client`?
-        - First, you must set the community id.
-        - You can set the community id by using the `set_community_id` method
-        - Or the `fetch_community_id` method if you do not know the community id.
+        client = Client()
 
-    `**Community Example**`
-    ```python
-    from pymino import Client
+        client.login(email="email", password="password")
 
-    client = Client()
+        print(f"Logged in: {client.is_authenticated}")
 
-    client.login(email="email", password="password")
+        # Output: Logged in: True
+        ```
+        ----------------------------
+        How can I utilize community methods with `Client`?
+            - First, you must set the community id.
+            - You can set the community id by using the `set_community_id` method
+            - Or the `fetch_community_id` method if you do not know the community id.
 
-    print(f"Logged in: {client.is_authenticated}")
+        `**Community Example**`
+        ```python
+        from pymino import Client
 
-    client.fetch_community_id("http://aminoapps.com/c/CommunityName")
-    # Or
-    client.set_community_id(123456789)
+        client = Client()
 
-    print(f"Community ID has been set: {client.community_id}")
-    ```
-    ----------------------------
-    `**Community Methods**`
-    ```python
-    from pymino import Client
+        client.login(email="email", password="password")
 
-    client = Client()
+        print(f"Logged in: {client.is_authenticated}")
 
-    client.login(email="email", password="password")
+        client.fetch_community_id("http://aminoapps.com/c/CommunityName")
+        # Or
+        client.set_community_id(123456789)
 
-    client.fetch_community_id("http://aminoapps.com/c/CommunityName")
+        print(f"Community ID has been set: {client.community_id}")
+        ```
+        ----------------------------
+        `**Community Methods**`
+        ```python
+        from pymino import Client
 
-    client.community.send_message(
-        chatId = "000000-0000-0000-0000-000000",
-        content = "Hello, world!"
-    ) # This will send in the community you set the community id for.
+        client = Client()
 
-    #Alternatively, you can use the community id as a parameter.
-    comId = client.fetch_community_id("http://aminoapps.com/c/CommunityName")
-    client.community.send_message(
-        chatId = "000000-0000-0000-0000-000000",
-        content = "Hello, world!",
-        comId = comId
-    )
-    ```
+        client.login(email="email", password="password")
 
-    """
-    def __init__(
-        self,
-        community_id: Optional[Union[str, int]] = None,
-        hash_prefix: Union[str, int] = 19,
-        device_key: str = "E7309ECC0953C6FA60005B2765F99DBBC965C8E9",
-        signature_key: str  = "DFA5ED192DDA6E88A12FE12130DC6206B1251E44",
-        **kwargs
-        ) -> None:
+        client.fetch_community_id("http://aminoapps.com/c/CommunityName")
+
+        client.community.send_message(
+            chatId = "000000-0000-0000-0000-000000",
+            content = "Hello, world!"
+        ) # This will send in the community you set the community id for.
+
+        #Alternatively, you can use the community id as a parameter.
+        comId = client.fetch_community_id("http://aminoapps.com/c/CommunityName")
+        client.community.send_message(
+            chatId = "000000-0000-0000-0000-000000",
+            content = "Hello, world!",
+            comId = comId
+        )
+        ```
+
+        """
         self._debug:            bool = check_debugger()
         self._is_authenticated: bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
         self.cache:             Cache = Cache("cache")
+        self.logger:            Logger = self._create_logger()
+        self.is_logging:        bool = True
         self.community_id:      Optional[str] = community_id or kwargs.get("comId")
         self.generate:          Generator = Generator(
                                 prefix=hash_prefix,
                                 device_key=device_key,
                                 signature_key=signature_key
                                 )
         self.device_id:         Optional[str] = kwargs.get("device_id") or self.generate.device_id()
@@ -146,14 +211,40 @@
                                 bot=self,
                                 session=self.request,
                                 community_id=self.community_id
                                 )
         
         super().__init__()
 
+    def __repr__(self):
+        """
+        Returns a string representation of the Client object.
+
+        :return: A string representation of the Client object.
+        :rtype: str
+        """
+        return f"Client(community_id={self.community_id}, device_id={self.device_id})"
+
+    def __str__(self):
+        """
+        Returns a user-friendly string representation of the Client object.
+
+        :return: A user-friendly string representation of the Client object.
+        :rtype: str
+        """
+        return f"Client(community_id={self.community_id}, device_id={self.device_id})"
+
+    def __iter__(self) -> iter:
+        """
+        Allows iteration over the Client object.
+
+        :return: An iterator for the Client object.
+        :rtype: iter
+        """
+        return iter(self.__slots__)
 
     @property
     def debug(self) -> bool:
         """
         Whether or not debug mode is enabled.
 
         :return: True if debug mode is enabled, False otherwise.
@@ -162,15 +253,14 @@
         This property returns whether or not debug mode is enabled. Debug mode can be used to enable additional logging and
         debug information during development.
 
         **Note:** This property only returns the debug mode state and cannot be used to set the debug mode state. To set the
         debug mode state, use the `self._debug` attribute directly.
         """
         return self._debug
-    
 
     @debug.setter
     def debug(self, value: bool) -> None:
         """
         Sets the debug mode state.
 
         :param value: True to enable debug mode, False to disable it.
@@ -181,15 +271,14 @@
         during development.
 
         **Note:** This setter only sets the debug mode state and cannot be used to retrieve the debug mode state. To retrieve
         the debug mode state, use the `self.debug` property.
         """
         self._debug = value
 
-
     @property
     def is_authenticated(self) -> bool:
         """
         Whether or not the client is authenticated.
 
         :return: True if the client is authenticated, False otherwise.
         :rtype: bool
@@ -197,15 +286,14 @@
         This property returns whether or not the client is authenticated. The client is authenticated after logging in to
         Amino and receiving a valid session ID.
 
         **Note:** This property only returns the authentication state and cannot be used to set the authentication state. To
         set the authentication state, use the `self._is_authenticated` attribute directly.
         """
         return self._is_authenticated
-    
 
     @is_authenticated.setter
     def is_authenticated(self, value: bool) -> None:
         """
         Sets the authentication state of the client.
 
         :param value: True to authenticate the client, False to deauthenticate it.
@@ -216,15 +304,14 @@
         receiving a valid session ID.
 
         **Note:** This setter only sets the authentication state and cannot be used to retrieve the authentication state. To
         retrieve the authentication state, use the `self.is_authenticated` property.
         """
         self._is_authenticated = value
 
-
     @property
     def userId(self) -> str:
         """
         The ID of the user associated with the client.
 
         :return: The ID of the user.
         :rtype: str
@@ -233,15 +320,14 @@
         Amino, and can be used to make API calls related to the user, such as retrieving the user's profile or posts.
 
         **Note:** This property only returns the user ID and cannot be used to set the user ID. To set the user ID, use the
         `self._userId` attribute directly.
         """
         return self._userId
 
-
     @userId.setter
     def userId(self, value: str) -> None:
         """
         Sets the ID of the user associated with the client.
 
         :param value: The ID of the user to set.
         :type value: str
@@ -251,15 +337,14 @@
         user, such as retrieving the user's profile or posts.
 
         **Note:** This setter only sets the user ID and cannot be used to retrieve the user ID. To retrieve the user ID, use
         the `self.userId` property.
         """
         self._userId = value
 
-        
     @property
     def sid(self) -> str:
         """
         The session ID of the client.
 
         :return: The session ID.
         :rtype: str
@@ -268,15 +353,14 @@
         used to make authenticated API calls, such as posting messages or retrieving user information.
 
         **Note:** This property only returns the session ID and cannot be used to set the session ID. To set the session ID,
         use the `self._sid` attribute directly.
         """
         return self._sid
 
-
     @sid.setter
     def sid(self, value: str) -> None:
         """
         Sets the session ID of the client.
 
         :param value: The session ID to set.
         :type value: str
@@ -286,14 +370,50 @@
         posting messages or retrieving user information.
 
         **Note:** This setter only sets the session ID and cannot be used to retrieve the session ID. To retrieve the session
         ID, use the `self.sid` property.
         """
         self._sid = value
 
+    def _log(self, message: str) -> None:
+        """
+        Logs a message to debug.log
+
+        :param message: The message to log.
+        :type message: str
+        :return: None
+
+        """
+        if self.is_logging:
+            try:
+                self.logger.debug(message)
+            except Exception:
+                self.is_logging = False
+
+    def _create_logger(self) -> Logger:
+        """
+        Creates a logger object.
+        
+        :return: A logger object.
+        :rtype: Logger
+        
+        This method creates a logger object. The logger object is used to log debug information to debug.log.
+        """
+        logger = getLogger("pymino")
+        logger.setLevel(DEBUG)
+
+        file_handler = FileHandler("debug.log")
+        file_handler.setLevel(DEBUG)
+
+        formatter = Formatter("%(asctime)s - %(levelname)s - %(message)s")
+        file_handler.setFormatter(formatter)
+
+        logger.addHandler(file_handler)
+
+        return logger
 
     def authenticated(func: F) -> F:
         """
         A decorator that ensures the user is authenticated before running the decorated function.
 
         :param func: The function to be decorated.
         :type func: Callable
@@ -315,15 +435,14 @@
                 if not args[0].is_authenticated:
                     raise LoginRequired
                 return func(*args, **kwargs)
             except AttributeError:
                 raise LoginRequired
         return wrapper
 
-
     def fetch_community_id(self, community_link: str, set_community_id: Optional[bool] = True) -> int:
         """
         Fetches the community ID associated with the provided community link.
 
         :param community_link: The community link for which to fetch the ID.
         :type community_link: str
         :param set_community_id: Whether or not to set the fetched community ID on the client instance. Defaults to True.
@@ -352,15 +471,14 @@
         community_id = self.cache.get(KEY)
 
         if set_community_id:
             self.set_community_id(community_id)
 
         return community_id
 
-
     def set_community_id(self, community_id: Union[str, int]) -> int:
         """
         Sets the community ID on the client instance and the Community object.
 
         :param community_id: The community ID to set.
         :type community_id: Union[str, int]
         :return: The community ID that was set.
@@ -384,15 +502,14 @@
             raise VerifyCommunityIdIsCorrect from e
 
         self.community_id = community_id
         self.community.community_id = community_id
 
         return community_id
 
-
     def authenticate(self, email: str, password: str, device_id: str=None) -> dict:
         """
         Authenticates the bot with the provided email and password.
 
         :param email: The email to use to log in.
         :type email: str
         :param password: The password to use to log in.
@@ -402,33 +519,34 @@
         :return: A dictionary representing the server response.
         :rtype: dict
         :raises: `APIError` if the API response code is not 200.
         """
         if device_id:
             self.device_id = device_id
 
-        return ApiResponse(self.request.handler(
-            method="POST",
-            url = "/g/s/auth/login",
-            data = {
-                "secret": f"0 {password}",
-                "clientType": 100,
-                "systemPushEnabled": 0,
-                "timestamp": int(time() * 1000),
-                "locale": "en_US",
-                "action": "normal",
-                "bundleID": "com.narvii.master",
-                "timezone": -480,
-                "deviceID": self.device_id,
-                "email": email,
-                "v": 2,
-                "clientCallbackURL": "narviiapp://default"
-                }
-            )).json()
-
+        return ApiResponse(
+            self.request.handler(
+                method="POST",
+                url = "/g/s/auth/login",
+                data = {
+                    "secret": f"0 {password}",
+                    "clientType": 100,
+                    "systemPushEnabled": 0,
+                    "timestamp": int(time() * 1000),
+                    "locale": "en_US",
+                    "action": "normal",
+                    "bundleID": "com.narvii.master",
+                    "timezone": -480,
+                    "deviceID": self.device_id,
+                    "email": email,
+                    "v": 2,
+                    "clientCallbackURL": "narviiapp://default"
+                    }
+                )
+            ).json()
 
     def _login_handler(self, email: str, password: str, device_id: str=None, use_cache: bool=True) -> dict:
         """
         Authenticates the user with the provided email and password.
 
         :param email: The email address associated with the account.
         :type email: str
@@ -478,15 +596,14 @@
                 )
 
         for key, value in {"email": email, "password": password}.items():
             setattr(self.request, key, value)            
 
         return response
 
-
     def login(
         self,
         email: Optional[str] = None,
         password: Optional[str] = None,
         sid: Optional[str] = None,
         device_id: Optional[str] = None,
         use_cache: bool = True
@@ -531,15 +648,14 @@
                 )
 
         if not response:
             raise LoginFailed
 
         return self._run(response)
 
-
     def run(
         self,
         email: Optional[str] = None,
         password: Optional[str] = None,
         sid: Optional[str] = None,
         device_id: Optional[str] = None,
         use_cache: bool = True
@@ -567,15 +683,14 @@
         **Example usage:**
 
         >>> client = Client()
         >>> client.run(email="example@example.com", password="password")
         """
         return self.login(email=email, password=password, sid=sid, device_id=device_id, use_cache=use_cache)
 
-
     def _run(self, response: dict) -> dict:
         """
         Processes the response from a successful login attempt and sets up the authenticated client.
 
         :param response: The response from the login attempt.
         :type response: dict
         :return: The response from the login attempt.
@@ -593,34 +708,39 @@
         >>> client = Client()
         >>> response = client.authenticate(email="example@example.com", password="password")
         >>> client._run(response)
         """
         if response["api:statuscode"] != 0: input(response), exit()
 
         if not hasattr(self, "profile"): 
-            self.profile: UserProfile = UserProfile(response) # Human is gay.
+            self.profile: UserProfile = UserProfile(response) 
 
         if not self.sid:
             self.sid: str = response["sid"]
 
         self.userId: str = self.profile.userId
         self.community.userId: str = self.userId
         self.request.sid: str = self.sid
         self.request.userId: str = self.userId
-        self.is_authenticated: bool = True
-
+        
         if hasattr(self.request, "email") and self._cached:
             cache_login(email=self.request.email, device=self.device_id, sid=self.sid)
 
+        if not self.is_authenticated:
+            self._is_authenticated = True
+            print("test")
+            self._log(f"Logged in as {self.profile.username} ({self.profile.userId})")
+        else:
+            self._log(f"Reconnected as {self.profile.username} ({self.profile.userId})")
+
         if self.debug:
             print(f"{Fore.MAGENTA}Logged in as {self.profile.username} ({self.profile.userId}){Style.RESET_ALL}")
 
         return response
 
-
     @authenticated
     def disconnect_google(self, password: str) -> dict:
         """
         Disconnects the user's Google account from their account on Amino.
 
         :param password: The user's account password.
         :type password: str
@@ -642,15 +762,14 @@
                 "deviceID": self.device_id,
                 "secret": f"0 {password}",
                 "type": 30,
                 "timestamp": int(time() * 1000),
                 }
             )
 
-
     @authenticated
     def logout(self) -> None:
         """
         Logs out the user by clearing the session ID and user ID on the client instance.
 
         :return: None
         :rtype: None
@@ -667,15 +786,14 @@
         **Note:** After calling this function, the client will no longer be authenticated and will need to log in again to
         make authenticated API calls.
         """
         for key in ["sid", "userId", "community.userId", "request.sid", "request.userId", "is_authenticated"]:
             setattr(self, key, None)
         return None
 
-
     def register(self, email: str, password: str, username: str, verificationCode: str) -> Authenticate:
         """
         Registers a new account with the provided email, password, username, and verification code.
 
         :param email: The email address to register the account with.
         :type email: str
         :param password: The password to use for the account.
@@ -694,15 +812,14 @@
         return self.account.register(
             email=email, 
             password=password,
             username=username,
             verificationCode=verificationCode
             )
 
-
     @authenticated
     def delete_request(self, email: str, password: str) -> ApiResponse:
         """
         Sends a request to delete the authenticated user's account.
 
         :param email: The email address associated with the account.
         :type email: str
@@ -713,15 +830,14 @@
 
         This method sends a request to delete the authenticated user's account. The email and password parameters are used to
         authenticate the request. The method returns an `ApiResponse` object containing the server's response to the delete
         request.
         """
         return self.account.delete_request(email=email, password=password)
 
-
     @authenticated
     def delete_request_cancel(self, email: str, password: str) -> ApiResponse:
         """
         Cancels a previously requested account deletion for the authenticated user.
 
         :param email: The email address associated with the account.
         :type email: str
@@ -732,15 +848,14 @@
 
         This method cancels a previously requested account deletion for the authenticated user. The email and password
         parameters are used to authenticate the request. The method returns an `ApiResponse` object containing the server's
         response to the delete request cancellation request.
         """
         return self.account.delete_request_cancel(email=email, password=password)
 
-
     def check_device(self, device_id: str) -> ApiResponse:
         """
         Checks if the given device ID is valid.
 
         :param device_id: The ID of the device to check.
         :type device_id: str
         :return: An `ApiResponse` object containing the server's response to the device check request.
@@ -752,15 +867,14 @@
         response to the device check request.
 
         The method returns the `ApiResponse` object obtained from calling the `check_device` method of the `account`
         object. The response will return a `0` status code if the device ID is valid.
         """
         return self.account.check_device(deviceId=device_id)
 
-
     def fetch_account(self) -> dict:
         """
         Fetches the account information for the authenticated user.
 
         :return: A dictionary containing the user's account information.
         :rtype: dict
 
@@ -779,15 +893,14 @@
             self.request.handler(
                 method="GET",
                 url=f"/g/s/user-profile/{self.userId}"
                 ))
         
         return ApiResponse(self.request.handler(method="GET", url="/g/s/account")).json()
 
-
     @authenticated
     def upload_image(self, image: str) -> str:
         """
         Uploads an image to amino servers.
 
         :param image: The base64-encoded image data.
         :type image: str
@@ -798,15 +911,14 @@
         `upload_image` method of the `account` object with the `image` parameter set to the given image data. The result is
         a `mediaValue` object that contains the URL of the uploaded image.
 
         The method returns the URL of the uploaded image.
         """
         return self.account.upload_image(image=image)
 
-
     @authenticated
     def fetch_profile(self) -> UserProfile:
         """
         Fetches the user profile of the authenticated user.
 
         :return: A `UserProfile` object containing the user's profile information.
         :rtype: UserProfile
@@ -815,15 +927,14 @@
         `account` object to get the profile information. The result is a `UserProfile` object that contains the user's profile
         information.
 
         The method returns the `UserProfile` object.
         """
         return self.account.fetch_profile(self.userId)
 
-
     @authenticated
     def set_amino_id(self, aminoId: str) -> ApiResponse:
         """
         Sets the Amino ID of the authenticated user.
 
         :param aminoId: The Amino ID to set for the user.
         :type aminoId: str
@@ -835,15 +946,14 @@
         is an `ApiResponse` object that contains the server's response to the set Amino ID request.
 
         The method returns the `ApiResponse` object obtained from calling the `set_amino_id` method of the `account` object.
         The response will return a `0` status code if the Amino ID is set successfully.
         """
         return self.account.set_amino_id(aminoId=aminoId)
 
-
     @authenticated
     def fetch_wallet(self) -> Wallet:
         """
         Fetches the wallet information for the authenticated user.
 
         :return: A `Wallet` object containing the user's wallet information.
         :rtype: Wallet
@@ -852,15 +962,14 @@
         total number of coins, the number of business coins, and other relevant details. The method calls the `fetch_wallet`
         method of the `account` object. The result is a `Wallet` object that contains the user's wallet information.
 
         The method returns a `Wallet` object containing the user's wallet information.
         """
         return self.account.fetch_wallet()
 
-
     def request_security_validation(self, email: str, resetPassword: bool = False) -> ApiResponse:
         """
         Requests security validation for the provided email address.
 
         :param email: The email address to request security validation for.
         :type email: str
         :param resetPassword: Optional flag to indicate if the user is requesting password reset. Default is False.
@@ -874,15 +983,14 @@
         parameter set to the provided email address and `resetPassword` parameter set to the provided flag. The result is
         an `ApiResponse` object that contains the server's response to the security validation request.
 
         The method returns an `ApiResponse` object containing the server's response to the security validation request.
         """
         return self.account.request_security_validation(email=email, resetPassword=resetPassword)
 
-
     def activate_email(self, email: str, code: str) -> ApiResponse:
         """
         Activates the user's email using the provided verification code.
 
         :param email: The email address to activate.
         :type email: str
         :param code: The verification code sent to the email address for activation.
@@ -892,15 +1000,14 @@
 
         This method activates the user's email using the provided verification code. The email and verification code
         parameters are used to authenticate the request. The method returns an `ApiResponse` object containing the server's
         response to the activation request.
         """
         return self.account.activate_email(email=email, code=code)
 
-
     @authenticated
     def reset_password(self, email: str, newPassword: str, code: str) -> ResetPassword:
         """
         Resets the user's password using the provided email, verification code, and new password.
 
         :param email: The email address associated with the account.
         :type email: str
```

### Comparing `pymino-1.2.4.2/pymino/ext/__init__.py` & `pymino-1.2.4.3/pymino/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/account.py` & `pymino-1.2.4.3/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/async_account.py` & `pymino-1.2.4.3/pymino/ext/async_account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/async_community.py` & `pymino-1.2.4.3/pymino/ext/async_community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/async_context.py` & `pymino-1.2.4.3/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/async_event_handler.py` & `pymino-1.2.4.3/pymino/ext/async_event_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/async_global_client.py` & `pymino-1.2.4.3/pymino/ext/async_global_client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/async_socket.py` & `pymino-1.2.4.3/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/community.py` & `pymino-1.2.4.3/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/console.py` & `pymino-1.2.4.3/pymino/ext/console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/context.py` & `pymino-1.2.4.3/pymino/ext/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,23 +8,50 @@
 from time import sleep as delay, time
 from inspect import signature as inspect_signature
 from typing import BinaryIO, Callable, List, Union
 
 from .entities import *
 from .utilities.commands import Command, Commands
 
-class Context():
-    """
-    `Context` - This handles the event context.
+__all__ = (
+    "Context",
+    "EventHandler"
+    )
 
-    `**Parameters**``
-    - `message` - The message which triggered the event.
-    - `session` - The session we will use to send requests.
 
+class Context:
     """
+    Context class that handles context.
+
+    This class is used to handle context for commands.
+
+    Special Attributes:
+    __slots__ : tuple
+        A tuple containing a fixed set of attributes to optimize memory usage.
+
+    Attributes:
+    message : Message
+        The message object.
+    bot : Bot
+        The bot object.
+    request : RequestHandler
+        The request handler object.
+    userId : str
+        The user ID.
+    intents : bool
+        Whether or not intents are enabled.
+
+"""
+    __slots__ = (
+        "message",
+        "bot",
+        "request",
+        "userId",
+        "intents"
+    )
     def __init__(self, message: Message, bot):
         self.message:   Message = message 
         self.bot        = bot
         self.request    = self.bot.request
         self.userId:    str = self.request.userId
         self.intents:   bool = self.bot.intents
```

### Comparing `pymino-1.2.4.2/pymino/ext/dispatcher.py` & `pymino-1.2.4.3/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/acm.py` & `pymino-1.2.4.3/pymino/ext/entities/acm.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/admin_log.py` & `pymino-1.2.4.3/pymino/ext/entities/admin_log.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/api_response.py` & `pymino-1.2.4.3/pymino/ext/entities/api_response.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/bubble.py` & `pymino-1.2.4.3/pymino/ext/entities/bubble.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/chat_threads.py` & `pymino-1.2.4.3/pymino/ext/entities/chat_threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/comments.py` & `pymino-1.2.4.3/pymino/ext/entities/comments.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/enums.py` & `pymino-1.2.4.3/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/exceptions.py` & `pymino-1.2.4.3/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/general.py` & `pymino-1.2.4.3/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/handlers.py` & `pymino-1.2.4.3/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/link_info.py` & `pymino-1.2.4.3/pymino/ext/entities/link_info.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/member.py` & `pymino-1.2.4.3/pymino/ext/entities/member.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/messages.py` & `pymino-1.2.4.3/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/notification.py` & `pymino-1.2.4.3/pymino/ext/entities/notification.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/sticker.py` & `pymino-1.2.4.3/pymino/ext/entities/sticker.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/threads.py` & `pymino-1.2.4.3/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/entities/userprofile.py` & `pymino-1.2.4.3/pymino/ext/entities/userprofile.py`

 * *Files 18% similar despite different names*

```diff
@@ -422,15 +422,15 @@
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.status)
 		```
 		"""
-		return self._data.get('status', None)
+		return self._data.get('status')
 
 	@property
 	def mood_sticker(self) -> Union[MoodSticker, MoodStickerNotFound]:
 		"""
 		`mood_sticker` - Mood sticker the user has set.
 
 		`Returns:` MoodSticker | MoodStickerNotFound
@@ -456,45 +456,45 @@
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.wiki_count)
 		```
 		"""
-		return self._data.get('itemsCount', None)
+		return self._data.get('itemsCount')
 
 	@property
 	def consecutive_check_in_days(self) -> int:
 		"""
 		`consecutiveCheckInDays` - The amount of consecutive days the user has checked in.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.consecutive_check_in_days)
 		```
 		"""
-		return self._data.get('consecutiveCheckInDays', None)
+		return self._data.get('consecutiveCheckInDays')
 
 	@property
 	def uid(self) -> str:
 		"""
 		`uid` - The user's uid.
 
 		`Returns:` str | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.uid)
 		```
 		"""
-		return self._data.get('uid', None)
+		return self._data.get('uid')
 
 	@property
 	def userId(self) -> str:
 		"""
 		`userId` - The user's uid.
 
 		`Returns:` str | None
@@ -516,150 +516,150 @@
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.aminoId)
 		```
 		"""
-		return self._data.get('aminoId', None)
+		return self._data.get('aminoId')
 
 	@property
 	def modified_time(self) -> str:
 		"""
 		`modifiedTime` - The time the user's profile was last modified.
 
 		`Returns:` str | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.modified_time)
 		```
 		"""
-		return self._data.get('modifiedTime', None)
+		return self._data.get('modifiedTime')
 
 	@property
 	def following_status(self) -> int:
 		"""
 		`followingStatus` - Whether the user is following the current user.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.following_status)
 		```
 		"""
-		return self._data.get('followingStatus', None)
+		return self._data.get('followingStatus')
 
 	@property
 	def online_status(self) -> int:
 		"""
 		`onlineStatus` - The user's online status.
 		
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.online_status)
 		```
 		"""
-		return self._data.get('onlineStatus', None)
+		return self._data.get('onlineStatus')
 
 	@property
 	def account_membership_status(self) -> int:
 		"""
 		`account_membership_status` - The user's account membership status.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.account_membership_status)
 		```
 		"""
-		return self._data.get('accountMembershipStatus', None)
+		return self._data.get('accountMembershipStatus')
 
 	@property
 	def is_global(self) -> bool:
 		"""
 		`is_global` - Whether the user is a global user.
 
 		`Returns:` bool | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.is_global)
 		```
 		"""
-		return self._data.get('isGlobal', None)
+		return self._data.get('isGlobal')
 
 	@property
 	def avatar_frame_id(self) -> str:
 		"""
 		`avatar_frame_id` - The user's avatar frame id.
 
 		`Returns:` str | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.avatar_frame_id)
 		```
 		"""
-		return self._data.get('avatarFrameId', None)
+		return self._data.get('avatarFrameId')
 
 	@property
 	def fan_club_list(self) -> list:
 		"""
 		`fan_club_list` - The user's fan club list.
 
 		`Returns:` list | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.fan_club_list)
 		```
 		"""
-		return self._data.get('fanClubList', None)
+		return self._data.get('fanClubList')
 
 	@property
 	def reputation(self) -> int:
 		"""
 		`reputation` - The user's reputation.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.reputation)
 		```
 		"""
-		return self._data.get('reputation', None)
+		return self._data.get('reputation')
 
 	@property
 	def posts_count(self) -> int:
 		"""
 		`posts_count` - The amount of posts the user has created.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.posts_count)
 		```
 		"""
-		return self._data.get('postsCount', None)
+		return self._data.get('postsCount')
 
 	@property
 	def avatar_frame(self) -> Union[AvatarFrame, AvatarFrameNotFound]:
 		"""
 		`avatar_frame` - The user's avatar frame.
 		
 		`Returns:` dict | None
@@ -669,45 +669,45 @@
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> if isinstance(user.avatar_frame, AvatarFrame):
 		...     print(user.avatar_frame.name)
 		... else:
 		...     print('Avatar frame not found.')
 		```
 		"""
-		return AvatarFrame(self._data.get('avatarFrame', None))
+		return AvatarFrame(self._data.get('avatarFrame'))
 
 	@property
 	def follower_count(self) -> int:
 		"""
 		`follower_count` - The amount of followers the user has.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.follower_count)
 		```
 		"""
-		return self._data.get('membersCount', None)	
+		return self._data.get('membersCount')	
 
 	@property
 	def nickname(self) -> str:
 		"""
 		`nickname` - The user's nickname.
 
 		`Returns:` str | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.nickname)
 		```
 		"""
-		return self._data.get('nickname', None)
+		return self._data.get('nickname')
 
 	@property
 	def username(self) -> str:
 		"""
 		`username` - The user's username.
 		
 		`Returns:` str | None
@@ -729,30 +729,30 @@
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.media_list)
 		```
 		"""
-		return self._data.get('mediaList', None)
+		return self._data.get('mediaList')
 
 	@property
 	def icon(self) -> str:
 		"""
 		`icon` - The user's icon.
 
 		`Returns:` str | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.icon)
 		```
 		"""
-		return self._data.get('icon', None)
+		return self._data.get('icon')
 
 	@property
 	def avatar(self) -> str:
 		"""
 		`avatar` - The user's avatar.
 
 		`Returns:` str | None
@@ -774,75 +774,75 @@
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.is_nickname_verified)
 		```
 		"""
-		return self._data.get('isNicknameVerified', None)
+		return self._data.get('isNicknameVerified')
 
 	@property
 	def mood(self) -> str:
 		"""
 		`mood` - The user's mood.
 
 		`Returns:` str | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.mood)
 		```
 		"""
-		return self._data.get('mood', None)
+		return self._data.get('mood')
 
 	@property
 	def level(self) -> int:
 		"""
 		`level` - The user's level.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.level)
 		```
 		"""
-		return self._data.get('level', None)
+		return self._data.get('level')
 
 	@property
 	def push_enabled(self) -> bool:
 		"""
 		`pushEnabled` - The user's push notification status.
 
 		`Returns:` bool | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.push_enabled)
 		```
 		"""
-		return self._data.get('pushEnabled', None)
+		return self._data.get('pushEnabled')
 
 	@property
 	def membership_status(self) -> int:
 		"""
 		`membershipStatus` - The user's membership status.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.membership_status)
 		```
 		"""
-		return self._data.get('membershipStatus', None)
+		return self._data.get('membershipStatus')
 
 	@property
 	def influencer_info(self) -> Union[InfluencerInfo, InfluencerInfoNotFound]:
 		"""
 		`influencerInfo` - The user's influencer info.
 
 		`Returns:` dict | None
@@ -852,120 +852,120 @@
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> if isinstance(user.influencer_info, InfluencerInfo):
 		...     print(user.influencer_info)
 		... else:
 		...     print("User influencer info not found.")
 		```
 		"""
-		return InfluencerInfo(self._data.get('influencerInfo', None))
+		return InfluencerInfo(self._data.get('influencerInfo'))
 
 	@property
 	def content(self) -> str:
 		"""
 		`content` - The user's profile content.
 
 		`Returns:` str | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.content)
 		```
 		"""
-		return self._data.get('content', None)
+		return self._data.get('content')
 
 	@property
 	def following_count(self) -> int:
 		"""
 		`followingCount` - The amount of users the user is following.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.following_count)
 		```
 		"""
-		return self._data.get('joinedCount', None)
+		return self._data.get('joinedCount')
 
 	@property
 	def role(self) -> int:
 		"""
 		`role` - The user's role.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.role)
 		```
 		"""
-		return self._data.get('role', None)
+		return self._data.get('role')
 
 	@property
 	def comments_count(self) -> int:
 		"""
 		`commentsCount` - The amount of comments the user has on their wall.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.comments_count)
 		```
 		"""
-		return self._data.get('commentsCount', None)
+		return self._data.get('commentsCount')
 
 	@property
 	def ndcId(self) -> int:
 		"""
 		`ndcId` - The community the user is in.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.ndcId)
 		```
 		"""
-		return self._data.get('ndcId', None)
+		return self._data.get('ndcId')
 
 	@property
 	def comId(self) -> int:
 		"""
 		`comId` - The community the user is in.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.comId)
 		```
 		"""
-		return self._data.get('ndcId', None)
+		return self._data.get('ndcId')
 
 	@property
 	def created_time(self) -> str:
 		"""
 		`createdTime` - The time the user was created.
 
 		`Returns:` str | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.created_time)
 		```
 		"""
-		return self._data.get('createdTime', None)
+		return self._data.get('createdTime')
 
 	@property
 	def extensions(self) -> Union[UserExtensions, UserExtensionsNotFound]:
 		"""
 		`extensions` - The user's extensions.
 
 		`Returns:` dict | None
@@ -975,60 +975,60 @@
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> if isinstance(user.extensions, UserExtensions):
 		...     print(user.extensions)
 		... else:
 		...     print("No extensions found.")
 		```
 		"""
-		return UserExtensions(self._data.get('extensions', None))
+		return UserExtensions(self._data.get('extensions'))
 
 	@property
 	def visit_privacy(self) -> int:
 		"""
 		`visitPrivacy` - The user's visit privacy.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.visit_privacy)
 		```
 		"""
-		return self._data.get('visitPrivacy', None)
+		return self._data.get('visitPrivacy')
 
 	@property
 	def stories_count(self) -> int:
 		"""
 		`storiesCount` - The amount of stories the user has.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.stories_count)
 		```
 		"""
-		return self._data.get('storiesCount', None)
+		return self._data.get('storiesCount')
 
 	@property
 	def blogs_count(self) -> int:
 		"""
 		`blogsCount` - The amount of blogs the user has.
 
 		`Returns:` int | None
 
 		`Example`:
 		```py
 		>>> user = bot.community.fetch_user(0000-0000-0000-0000)
 		>>> print(user.blogs_count)
 		```
 		"""
-		return self._data.get('blogsCount', None)
+		return self._data.get('blogsCount')
 
 	def json(self) -> dict:
 		"""
 		`json` - The json response from the api.
 		
 		`Returns:` dict
 
@@ -1069,33 +1069,33 @@
 	- `avatar_frame_id` - The user's avatar frame id.
 	- `avatar_frame` - The user's avatar frame.
 	- `is_nickname_verified` - If the user's nickname is verified.
 	- `json` - The json response from the api.
 	"""
 	def __init__(self, data: dict):
 		self._data = data.get('o', data)
-		self._user: dict = self._data.get('userProfileList', None)[0]
+		self._user: dict = self._data.get('userProfileList')[0]
 
 	@property
 	def topic(self) -> str:
 		"""
 		`topic` - The community's topic.
 		
 		`Returns:` str | None
 		"""
-		return self._data.get('topic', None)
+		return self._data.get('topic')
 	
 	@property
 	def ndcId(self) -> str:
 		"""
 		`ndcId` - The community's id.
 
 		`Returns:` str | None
 		"""
-		return self._data.get('ndcId', None)
+		return self._data.get('ndcId')
 
 	@property
 	def comId(self) -> str:
 		"""
 		`comId` - The community's id.
 		
 		`Returns:` str | None
@@ -1105,33 +1105,33 @@
 	@property
 	def users_online(self) -> int:
 		"""
 		`usersOnline` - The amount of users online.
 		
 		`Returns:` int | None
 		"""
-		return self._data.get('userProfileCount', None)
+		return self._data.get('userProfileCount')
 
 	@property
 	def is_guest(self) -> bool:
 		"""
 		`isGuest` - If the user is a guest.
 		
 		`Returns:` bool | None
 		"""
-		return self._user.get('isGuest', None)
+		return self._user.get('isGuest')
 
 	@property
 	def uid(self) -> str:
 		"""
 		`uid` - The user's id.
 		
 		`Returns:` str | None
 		"""
-		return self._user.get('uid', None)
+		return self._user.get('uid')
 
 	@property
 	def userId(self) -> str:
 		"""
 		`userId` - The user's id.
 		
 		`Returns:` str | None
@@ -1141,24 +1141,24 @@
 	@property
 	def status(self) -> str:
 		"""
 		`status` - The user's status.
 		
 		`Returns:` str | None
 		"""
-		return self._user.get('status', None)
+		return self._user.get('status')
 
 	@property
 	def icon(self) -> str:
 		"""
 		`icon` - The user's icon.
 		
 		`Returns:` str | None
 		"""
-		return self._user.get('icon', None)
+		return self._user.get('icon')
 
 	@property
 	def avatar(self) -> str:
 		"""
 		`avatar` - The user's icon.
 		
 		`Returns:` str | None
@@ -1168,33 +1168,33 @@
 	@property
 	def reputation(self) -> int:
 		"""
 		`reputation` - The user's reputation.
 		
 		`Returns:` int | None
 		"""
-		return self._user.get('reputation', None)
+		return self._user.get('reputation')
 
 	@property
 	def role(self) -> str:
 		"""
 		`role` - The user's role.
 		
 		`Returns:` str | None
 		"""
-		return self._user.get('role', None)
+		return self._user.get('role')
 
 	@property
 	def nickname(self) -> str:
 		"""
 		`nickname` - The user's nickname.
 		
 		`Returns:` str | None
 		"""
-		return self._user.get('nickname', None)
+		return self._user.get('nickname')
 
 	@property
 	def username(self) -> str:
 		"""
 		`username` - The user's nickname.
 		
 		`Returns:` str | None
@@ -1204,15 +1204,15 @@
 	@property
 	def level(self) -> int:
 		"""
 		`level` - The user's level.
 		
 		`Returns:` int | None
 		"""
-		return self._user.get('level', None)
+		return self._user.get('level')
 
 	@property
 	def extensions(self) -> UserExtensions:
 		"""
 		`extensions` - The user's extensions.
 		
 		`Returns:` UserExtensions | None
@@ -1222,33 +1222,33 @@
 		>>> user = OnlineUser(...)
 		>>> if isinstance(user.extensions, UserExtensions):
 		...     print(user.extensions.(...))
 		... else:
 		...     print('No extensions')
 		```
 		"""
-		return UserExtensions(self._user.get('extensions', None))
+		return UserExtensions(self._user.get('extensions'))
 
 	@property
 	def account_membership_status(self) -> str:
 		"""
 		`accountMembershipStatus` - The user's account membership status.
 
 		`Returns:` str | None
 		"""
-		return self._user.get('accountMembershipStatus', None)
+		return self._user.get('accountMembershipStatus')
 
 	@property
 	def avatar_frame_id(self) -> str:
 		"""
 		`avatarFrameId` - The user's avatar frame id.
 
 		`Returns:` str | None
 		"""
-		return self._user.get('avatarFrameId', None)
+		return self._user.get('avatarFrameId')
 
 	@property
 	def avatar_frame(self) -> AvatarFrame:
 		"""
 		`avatarFrame` - The user's avatar frame.
 
 		`Returns:` AvatarFrame | None
@@ -1258,77 +1258,81 @@
 		>>> user = OnlineUser(...)
 		>>> if isinstance(user.avatar_frame, AvatarFrame):
 		...     print(user.avatar_frame.(...))
 		... else:
 		...     print('No avatar frame')
 		```
 		"""
-		return AvatarFrame(self._user.get('avatarFrame', None))
+		return AvatarFrame(self._user.get('avatarFrame'))
 
 	@property
 	def is_nickname_verified(self) -> bool:
 		"""
 		`isNicknameVerified` - If the user's nickname is verified.
 
 		`Returns:` bool | None
 		"""
-		return self._user.get('isNicknameVerified', None)
+		return self._user.get('isNicknameVerified')
 
 	def json(self):
 		"""
 		`Returns:`
 		- Api response in json format.
 		"""
 		return self._data
 
 class UserProfileList:
-	def __init__(self, data: dict):
-		self._data = data.get("userProfileList", data) if isinstance(data, dict) else data
+	def __init__(self, data: Union[dict, list]) -> None:
 
-		parser:							list = [UserProfile(x) for x in self._data]
-		self.status:					list = [x.status for x in parser]
-		self.mood_sticker:				list = [x.mood_sticker for x in parser]
-		self.wiki_count:				list = [x.wiki_count for x in parser]
-		self.consecutive_check_in_days:	list = [x.consecutive_check_in_days for x in parser]
-		self.uid:						list = [x.uid for x in parser]
-		self.userId:					list = self.uid
-		self.modified_time:				list = [x.modified_time for x in parser]
-		self.following_status:			list = [x.following_status for x in parser]
-		self.online_status:				list = [x.online_status for x in parser]
-		self.account_membership_status:	list = [x.account_membership_status for x in parser]
-		self.is_global:					list = [x.is_global for x in parser]
-		self.avatar_frame_id:			list = [x.avatar_frame_id for x in parser]
-		self.fan_club_list:				list = [x.fan_club_list for x in parser]
-		self.reputation:				list = [x.reputation for x in parser]
-		self.posts_count:				list = [x.posts_count for x in parser]
-		#self.avatar_frame:				list = [x.avatar_frame for x in parser]
-		self.follower_count:			list = [x.follower_count for x in parser]
-		self.nickname:					list = [x.nickname for x in parser]
-		self.username:					list = self.nickname
-		self.media_list:				list = [x.media_list for x in parser]
-		self.icon:						list = [x.icon for x in parser]
-		self.avatar:					list = self.icon
-		self.is_nickname_verified:		list = [x.is_nickname_verified for x in parser]
-		self.mood:						list = [x.mood for x in parser]
-		self.level:						list = [x.level for x in parser]
-		self.pushEnabled:				list = [x.push_enabled for x in parser]
-		self.membership_status:			list = [x.membership_status for x in parser]
+		if isinstance(data, dict):
+			self._data: List[dict] = data.get("userProfileList", data)
+		else:
+			self._data: List[dict] = data
+
+		parser:							List[UserProfile] = [UserProfile(x) for x in self._data]
+		self.status:					List[int] = [x.status for x in parser]
+		self.mood_sticker:				List[MoodSticker] = [x.mood_sticker for x in parser]
+		self.wiki_count:				List[int] = [x.wiki_count for x in parser]
+		self.consecutive_check_in_days:	List[int] = [x.consecutive_check_in_days for x in parser]
+		self.uid:						List[str] = [x.uid for x in parser]
+		self.userId:					List[str] = self.uid
+		self.modified_time:				List[str] = [x.modified_time for x in parser]
+		self.following_status:			List[int] = [x.following_status for x in parser]
+		self.online_status:				List[int] = [x.online_status for x in parser]
+		self.account_membership_status:	List[int] = [x.account_membership_status for x in parser]
+		self.is_global:					List[bool] = [x.is_global for x in parser]
+		self.avatar_frame_id:			List[str] = [x.avatar_frame_id for x in parser]
+		self.fan_club_list:				List[list] = [x.fan_club_list for x in parser]
+		self.reputation:				List[int] = [x.reputation for x in parser]
+		self.posts_count:				List[int] = [x.posts_count for x in parser]
+		#self.avatar_frame:				List[AvatarFrameList] = [AvatarFrameList(x.avatar_frame.json()) for x in parser]	
+		self.follower_count:			List[int] = [x.follower_count for x in parser]
+		self.nickname:					List[str] = [x.nickname for x in parser]
+		self.username:					List[str] = self.nickname
+		self.media_list:				List[list] = [x.media_list for x in parser]
+		self.icon:						List[str] = [x.icon for x in parser]
+		self.avatar:					List[str] = self.icon
+		self.is_nickname_verified:		List[bool] = [x.is_nickname_verified for x in parser]
+		self.mood:						List[str] = [x.mood for x in parser]
+		self.level:						List[int] = [x.level for x in parser]
+		self.pushEnabled:				List[bool] = [x.push_enabled for x in parser]
+		self.membership_status:			List[int] = [x.membership_status for x in parser]
 		#self.influencer_info:			list = [x.influencer_info for x in parser]
-		self.content:					list = [x.content for x in parser]
-		self.following_count:			list = [x.following_count for x in parser]
-		self.role:						list = [x.role for x in parser]
-		self.comments_count:			list = [x.comments_count for x in parser]
-		self.ndcId:						list = [x.ndcId for x in parser]
-		self.comId:						list = self.ndcId
-		self.created_time:				list = [x.created_time for x in parser]
-		#self.extensions:				list = [x.extensions for x in parser]
-		self.visit_privacy:				list = [x.visit_privacy for x in parser]
-		self.stories_count:				list = [x.stories_count for x in parser]
-		self.blogs_count:				list = [x.blogs_count for x in parser]
-		self.user_profile_count:		int = len(self._data)
+		self.content:					List[str] = [x.content for x in parser]
+		self.following_count:			List[int] = [x.following_count for x in parser]
+		self.role:						List[int] = [x.role for x in parser]
+		self.comments_count:			List[int] = [x.comments_count for x in parser]
+		self.ndcId:						List[int] = [x.ndcId for x in parser]
+		self.comId:						List[int] = self.ndcId
+		self.created_time:				List[str] = [x.created_time for x in parser]
+		#self.extensions:				List[UserExtensionsList] = [UserExtensionsList(self._data.get("extensions") for y in self._data) for x in parser]
+		self.visit_privacy:				List[int] = [x.visit_privacy for x in parser]
+		self.stories_count:				List[int] = [x.stories_count for x in parser]
+		self.blogs_count:				List[int] = [x.blogs_count for x in parser]
+		self.user_profile_count:		int = data.get("userProfileCount")
 
 class Pagging:
     def __init__(self, data: dict):
         self._data = data.get("paging") if isinstance(data, dict) else data
         self.prev_page_token = None
         self.next_page_token = None
```

### Comparing `pymino-1.2.4.2/pymino/ext/entities/wsevents.py` & `pymino-1.2.4.3/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/global_client.py` & `pymino-1.2.4.3/pymino/ext/global_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1922,30 +1922,8 @@
         >>> community_list = client.community.fetch_available_communities(start=0, size=10, language="en")
         >>> for name, comId in zip(community_list.name, community_list.comId):
         >>>     print(name, comId])
         """
         return CCommunityList(self.make_request(
             method = "GET",
             url = f"/g/s/topic/0/feed/community?language={language}&type=web-explore&categoryKey=recommendation&start={start}&size={size}&pagingType=t"
-        ))
-    
-    def unfollow(self, userId: str) -> ApiResponse:
-        """
-        Unfollows a user.
-
-        :param userId: The ID of the user to unfollow.
-        :type userId: str
-        :return: An ApiResponse object containing the response data from the API.
-        :rtype: ApiResponse
-
-        This function allows the logged-in user to unfollow another user specified by their ID.
-        After successful execution, the user will no longer be following the specified user.
-
-        **Example usage:**
-
-        >>> response = client.unfollow(userId="user123")
-        >>> print(response.status_code)
-        """
-        return ApiResponse(self.make_request(
-            method = "DELETE",
-            url = f"/g/s/user-profile/{userId}/member/{self.userId}"
         ))
```

### Comparing `pymino-1.2.4.2/pymino/ext/handle_queue.py` & `pymino-1.2.4.3/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/socket.py` & `pymino-1.2.4.3/pymino/ext/socket.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,164 +21,202 @@
     pipmain(["uninstall", "websocket", "-y"])
     pipmain(["install", "websocket-client==1.6.1"])
     raise WrongWebSocketPackage from e
 
 
 class WSClient(EventHandler):
     """
-    `WSClient` is a class that handles the websocket.
+    WSClient class that handles websocket events.
+
+    This class extends `EventHandler` class, allowing the bot to use event handler features.
+
+    Special Attributes:
+    __slots__ : tuple
+        A tuple containing a fixed set of attributes to optimize memory usage.
+
+    Attributes:
+    ws : WebSocketApp
+        The websocket object.
+    _communities : set
+        A set containing the communities the bot is in.
+    event_types : dict
+        A dictionary containing the event types.
+    notif_types : dict
+        A dictionary containing the notification types.
+    dispatcher : MessageDispatcher
+        The message dispatcher object.
+    channel : Optional[Channel] 
+        The agora channel.
+    orjson : bool
+        Whether or not orjson is installed.
+
     """
+    __slots__ = (
+        "ws",
+        "_communities",
+        "event_types",
+        "is_logging",
+        "notif_types",
+        "dispatcher",
+        "channel",
+        "orjson"
+    )
     def __init__(self):
-        self.ws:            WebSocketApp = None      
+        self.ws:            WebSocketApp = None
         self._communities:  set = set()
         self.event_types:   dict =  EventTypes().events
+        self.is_logging:    bool = True
         self.notif_types:   dict =  NotifTypes().notifs
         self.dispatcher:    MessageDispatcher = MessageDispatcher()
         self.channel:       Optional[Channel] = None
         self.orjson:        bool = orjson_exists()
         
         self.dispatcher.register(10, self._handle_notification)
         self.dispatcher.register(201, self._handle_agora_channel)
         self.dispatcher.register(400, self._handle_user_online)
         self.dispatcher.register(1000, self._handle_message)
 
         EventHandler.__init__(self)
 
-
     def fetch_ws_url(self) -> str:
         return f"wss://ws{randint(1, 4)}.aminoapps.com"
-
+    
+    def _log(self, message: str) -> None:
+        """
+        Logs a message to debug.log
+
+        :param message: The message to log.
+        :type message: str
+        :return: None
+
+        """
+        if self.is_logging:
+            try:
+                self.logger.debug(message)
+            except Exception:
+                self.is_logging = False
 
     def connect(self) -> None:
         """Connects to the websocket."""
         self.run_forever()
         return self.emit("ready")
 
-
     def run_forever(self) -> None:
         """Runs the websocket forever."""
+        self._log("Initializing websocket.")
         ws_data = f"{self.generate.device_id()}|{int(time() * 1000)}"
         self.ws = WebSocketApp(
             url = f"{self.fetch_ws_url()}/?{urlencode({'signbody': ws_data})}",
             on_open=self.on_websocket_open,
             on_message=self.on_websocket_message,
             on_error=self.on_websocket_error,
             on_close=self.on_websocket_close,
             header={
             "NDCDEVICEID": self.generate.device_id(),
             "NDCAUTH": f"sid={self.sid}",
             "NDC-MSG-SIG": self.generate.signature(ws_data)
             })
-        return self.start_processes()
-
+        
+        self.start_processes()
+        return self._log("Websocket connected.")
 
     def start_processes(self) -> None:
         """Starts the websocket processes."""
         websocket_thread = Thread(target=self.ws.run_forever)
         websocket_thread.start()
 
         aalive_thread = Thread(target=run_alive_loop, args=(self,))
         aalive_thread.start()
 
-
     def on_websocket_error(self, ws: WebSocket, error: Exception) -> None:
         """Handles websocket errors."""
         with suppress(KeyError):
             self._events["error"](error)
 
+        return self._log(f"Websocket error: {error}")
 
     def on_websocket_message(self, ws: WebSocket, message: dict) -> None:
         """Handles websocket messages."""
         try:
             raw_message = orjson_loads(message) if self.orjson else loads(message)
         except JSONDecodeError:
             raw_message = loads(message)
 
         self.dispatcher.handle(raw_message)
 
-
     def _handle_message(self, message: dict) -> None:
         """Sends the message to the event handler."""
         _message: Message = Message(message)
 
         if self.userId == _message.userId: return None
         None if any(
             [_message.ndcId is None, _message.ndcId == 0]
         ) else self._communities.add(_message.ndcId)
 
         key = self.event_types.get(f"{_message.type}:{_message.mediaType}")
         if key != None:
             return self._handle_event(key, _message)
 
-
     def _handle_notification(self, message: dict) -> None:
         """Handles notifications."""
         notification: Notification = Notification(message)
         key = self.notif_types.get(notification.notification_type)
         return self._handle_event(key, notification) if key else None
 
-
     def _handle_agora_channel(self, message: dict) -> None:
         """Sets the agora channel."""
         self.channel: Channel = Channel(message)
 
-
     def _handle_user_online(self, message: dict) -> None:
         """Handles user online events."""
         return self._handle_event("user_online", OnlineMembers(message))
 
-
     def on_websocket_close(self, ws: WebSocket, close_status_code: int, close_msg: str) -> None:
         """Handles websocket close events."""
         if [close_status_code, close_msg] == [None, None]:
-            return self.run_forever() 
-
+            self._log("Websocket closed unexpectedly.")
+            return self.run_forever()
 
     def send_websocket_message(self, message: dict) -> None:
         """Sends a websocket message."""
         return self.ws.send(orjson_dumps(message).decode() if self.orjson else dumps(message))
 
-
     def stop_websocket(self) -> None:
         """Stops the websocket."""
+        self._log("Websocket received stop signal.")
         return self.ws.close()
 
-
     def on_websocket_open(self, ws: WebSocket) -> None:
         """Handles websocket open events."""
         if all([self.community_id != None, "user_online" in self._events]):
             return self.send_websocket_message({
                 "t": 300,
                 "o": {
                     "ndcId": self.community_id,
                     "topic": f"ndtopic:x{self.community_id}:online-members",
                     "id": int(time() * 1000)
                 }})
 
-
     def _last_active(self, last_activity_time: float) -> bool:
         """Returns True if the last activity was 5 minutes ago."""""
         return time() - last_activity_time >= 300
 
-
     def _last_message(self, last_message_time: float) -> bool:
         """Returns True if the last message was 30 seconds ago."""
         return time() - last_message_time >= 30
 
-
     def _send_message(self) -> None:
         """Sends a message to the websocket."""
         self.send_websocket_message({
             "o":{
                 "threadChannelUserInfoList": [],
                 "id": randint(1, 100)},
                 "t": 116
                 })
 
-
     def _activity_status(self) -> None:
         """Sets the user's activity status to online."""
         for comId in self._communities:
 
             if self.online_status:
                 try:
                     self.community.send_active(comId=comId,
```

### Comparing `pymino-1.2.4.2/pymino/ext/utilities/async_request_handler.py` & `pymino-1.2.4.3/pymino/ext/utilities/async_request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/utilities/chat_console.py` & `pymino-1.2.4.3/pymino/ext/utilities/chat_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/utilities/commands.py` & `pymino-1.2.4.3/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/utilities/community_console.py` & `pymino-1.2.4.3/pymino/ext/utilities/community_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/utilities/generate.py` & `pymino-1.2.4.3/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/utilities/menu.py` & `pymino-1.2.4.3/pymino/ext/utilities/menu.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/utilities/profile_console.py` & `pymino-1.2.4.3/pymino/ext/utilities/profile_console.py`

 * *Files identical despite different names*

### Comparing `pymino-1.2.4.2/pymino/ext/utilities/request_handler.py` & `pymino-1.2.4.3/pymino/ext/utilities/request_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from time import sleep
 from uuid import uuid4
 from ujson import loads, dumps
 from colorama import Fore, Style
 from typing import Optional, Union, Tuple, Callable
 
 from .generate import Generator
 from ..entities.handlers import orjson_exists
@@ -136,16 +135,16 @@
             return response.status_code, response.text
         except (
             ConnectionError,
             ReadTimeout,
             SSLError,
             ProxyError,
             ConnectTimeout,
-        ):
-            sleep(1.5)
+        ) as e:
+            self.bot._log(f"Failed to send request: {e}")
             return self.handler(method, url, data, content_type)
 
     def handler(
         self,
         method: str,
         url: str,
         data: Union[dict, bytes, None] = None,
@@ -289,14 +288,15 @@
                 hasattr(self, "email"),
                 hasattr(self, "password"),
             ]
         ):
             self.bot.run(self.email, self.password, use_cache=False)
             return 404      
       
+        self.bot._log(f"Exception: {response}")
         raise APIException(response)
         
     def handle_response(self, status_code: int, response: str) -> dict:
         """
         `handle_response` - Handles the response and returns the response as a dict
         
         `**Parameters**``
```

### Comparing `pymino-1.2.4.2/pymino.egg-info/PKG-INFO` & `pymino-1.2.4.3/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.2.4.2
+Version: 1.2.4.3
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
-Metadata-Version: 2.1 Name: pymino Version: 1.2.4.2 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.2.4.3 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Requires-Python: >=3.8 Description-Content-Type:
```

### Comparing `pymino-1.2.4.2/pymino.egg-info/SOURCES.txt` & `pymino-1.2.4.3/pymino.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 pymino/client.py
 pymino.egg-info/PKG-INFO
 pymino.egg-info/SOURCES.txt
 pymino.egg-info/dependency_links.txt
 pymino.egg-info/requires.txt
 pymino.egg-info/top_level.txt
 pymino/ext/__init__.py
-pymino/ext/_global.py
 pymino/ext/account.py
 pymino/ext/async_account.py
 pymino/ext/async_community.py
 pymino/ext/async_context.py
 pymino/ext/async_event_handler.py
 pymino/ext/async_global_client.py
 pymino/ext/async_socket.py
```

### Comparing `pymino-1.2.4.2/setup.cfg` & `pymino-1.2.4.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e32 2e34 2e32 0d0a 6175  on = 1.2.4.2..au
+00000020: 6f6e 203d 2031 2e32 2e34 2e33 0d0a 6175  on = 1.2.4.3..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.2.4.2/setup.py` & `pymino-1.2.4.3/setup.py`

 * *Files identical despite different names*

