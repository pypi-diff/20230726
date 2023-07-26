# Comparing `tmp/pybotx-0.55.8.tar.gz` & `tmp/pybotx-0.56.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotx-0.55.8.tar", max compression
+gzip compressed data, was "pybotx-0.56.0.tar", max compression
```

## Comparing `pybotx-0.55.8.tar` & `pybotx-0.56.0.tar`

### file list

```diff
@@ -1,131 +1,132 @@
--rw-r--r--   0        0        0     6078 2023-07-25 10:36:06.358456 pybotx-0.55.8/LICENSE
--rw-r--r--   0        0        0    21491 2023-07-25 10:36:06.358456 pybotx-0.55.8/README.md
--rw-r--r--   0        0        0     6519 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/__init__.py
--rw-r--r--   0        0        0      976 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/async_buffer.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/__init__.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/api/__init__.py
--rw-r--r--   0        0        0      560 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/api/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/api/responses/__init__.py
--rw-r--r--   0        0        0     1048 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/api/responses/bot_disabled.py
--rw-r--r--   0        0        0      275 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/api/responses/command_accepted.py
--rw-r--r--   0        0        0    54140 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/bot.py
--rw-r--r--   0        0        0     1558 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/bot_accounts_storage.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/callbacks/__init__.py
--rw-r--r--   0        0        0     3101 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/callbacks/callback_manager.py
--rw-r--r--   0        0        0     2176 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/callbacks/callback_memory_repo.py
--rw-r--r--   0        0        0      983 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/callbacks/callback_repo_proto.py
--rw-r--r--   0        0        0      330 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/contextvars.py
--rw-r--r--   0        0        0      966 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/exceptions.py
--rw-r--r--   0        0        0     2701 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/handler.py
--rw-r--r--   0        0        0    14503 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/handler_collector.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/middlewares/__init__.py
--rw-r--r--   0        0        0     1749 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/middlewares/exception_middleware.py
--rw-r--r--   0        0        0      293 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/bot/testing.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/client/__init__.py
--rw-r--r--   0        0        0     1617 2023-07-25 10:36:06.358456 pybotx-0.55.8/pybotx/client/authorized_botx_method.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/bots_api/__init__.py
--rw-r--r--   0        0        0     1235 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/bots_api/get_token.py
--rw-r--r--   0        0        0     6815 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/botx_method.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/__init__.py
--rw-r--r--   0        0        0     2201 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/add_admin.py
--rw-r--r--   0        0        0     1443 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/add_user.py
--rw-r--r--   0        0        0     2975 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/chat_info.py
--rw-r--r--   0        0        0     2177 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/create_chat.py
--rw-r--r--   0        0        0     1415 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/disable_stealth.py
--rw-r--r--   0        0        0     2004 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/list_chats.py
--rw-r--r--   0        0        0     1398 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/pin_message.py
--rw-r--r--   0        0        0     1430 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/remove_user.py
--rw-r--r--   0        0        0     1699 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/set_stealth.py
--rw-r--r--   0        0        0     1354 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/chats_api/unpin_message.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/events_api/__init__.py
--rw-r--r--   0        0        0     3295 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/events_api/edit_event.py
--rw-r--r--   0        0        0     2324 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/events_api/message_status_event.py
--rw-r--r--   0        0        0     3770 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/events_api/reply_event.py
--rw-r--r--   0        0        0     1019 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/events_api/stop_typing_event.py
--rw-r--r--   0        0        0      955 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/events_api/typing_event.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/exceptions/__init__.py
--rw-r--r--   0        0        0     1301 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/exceptions/base.py
--rw-r--r--   0        0        0      889 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/exceptions/callbacks.py
--rw-r--r--   0        0        0      424 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/exceptions/chats.py
--rw-r--r--   0        0        0      429 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/exceptions/common.py
--rw-r--r--   0        0        0      130 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/exceptions/event.py
--rw-r--r--   0        0        0      289 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/exceptions/files.py
--rw-r--r--   0        0        0      750 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/exceptions/http.py
--rw-r--r--   0        0        0      378 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/exceptions/notifications.py
--rw-r--r--   0        0        0      293 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/exceptions/users.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/files_api/__init__.py
--rw-r--r--   0        0        0     2093 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/files_api/download_file.py
--rw-r--r--   0        0        0     2448 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/files_api/upload_file.py
--rw-r--r--   0        0        0      812 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/get_token.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/notifications_api/__init__.py
--rw-r--r--   0        0        0     5567 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/notifications_api/direct_notification.py
--rw-r--r--   0        0        0     2925 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/notifications_api/internal_bot_notification.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/openid_api/__init__.py
--rw-r--r--   0        0        0     1245 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/openid_api/refresh_access_token.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/smartapps_api/__init__.py
--rw-r--r--   0        0        0     2259 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/smartapps_api/smartapp_event.py
--rw-r--r--   0        0        0     1836 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/smartapps_api/smartapp_notification.py
--rw-r--r--   0        0        0     2195 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/smartapps_api/smartapps_list.py
--rw-r--r--   0        0        0     1652 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/smartapps_api/upload_file.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/__init__.py
--rw-r--r--   0        0        0     2883 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/add_sticker.py
--rw-r--r--   0        0        0     1689 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/create_sticker_pack.py
--rw-r--r--   0        0        0     1506 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/delete_sticker.py
--rw-r--r--   0        0        0     1426 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/delete_sticker_pack.py
--rw-r--r--   0        0        0     1793 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/edit_sticker_pack.py
--rw-r--r--   0        0        0      311 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/exceptions.py
--rw-r--r--   0        0        0     1984 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/get_sticker.py
--rw-r--r--   0        0        0     1397 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/get_sticker_pack.py
--rw-r--r--   0        0        0     2352 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/get_sticker_packs.py
--rw-r--r--   0        0        0     1321 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/stickers_api/sticker_pack.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/users_api/__init__.py
--rw-r--r--   0        0        0     1231 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/users_api/search_user_by_email.py
--rw-r--r--   0        0        0     1257 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/users_api/search_user_by_huid.py
--rw-r--r--   0        0        0     1330 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/users_api/search_user_by_login.py
--rw-r--r--   0        0        0     1254 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/users_api/search_user_by_other_id.py
--rw-r--r--   0        0        0     3020 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/users_api/update_user_profile.py
--rw-r--r--   0        0        0     1737 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/users_api/user_from_csv.py
--rw-r--r--   0        0        0     1353 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/users_api/user_from_search.py
--rw-r--r--   0        0        0     1659 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/client/users_api/users_as_csv.py
--rw-r--r--   0        0        0      421 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/constants.py
--rw-r--r--   0        0        0      221 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/converters.py
--rw-r--r--   0        0        0      789 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/image_validators.py
--rw-r--r--   0        0        0     1341 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/logger.py
--rw-r--r--   0        0        0      648 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/missing.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/__init__.py
--rw-r--r--   0        0        0     2079 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/api_base.py
--rw-r--r--   0        0        0     7256 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/async_files.py
--rw-r--r--   0        0        0    13052 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/attachments.py
--rw-r--r--   0        0        0     2480 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/base_command.py
--rw-r--r--   0        0        0      187 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/bot_account.py
--rw-r--r--   0        0        0      199 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/bot_sender.py
--rw-r--r--   0        0        0     1625 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/chats.py
--rw-r--r--   0        0        0     1595 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/commands.py
--rw-r--r--   0        0        0     8751 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/enums.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/message/__init__.py
--rw-r--r--   0        0        0      670 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/message/edit_message.py
--rw-r--r--   0        0        0      524 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/message/forward.py
--rw-r--r--   0        0        0    10253 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/message/incoming_message.py
--rw-r--r--   0        0        0     4714 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/message/markup.py
--rw-r--r--   0        0        0     9106 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/message/mentions.py
--rw-r--r--   0        0        0      270 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/message/message_status.py
--rw-r--r--   0        0        0      882 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/message/outgoing_message.py
--rw-r--r--   0        0        0      696 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/message/reply.py
--rw-r--r--   0        0        0      825 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/message/reply_message.py
--rw-r--r--   0        0        0      538 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/method_callbacks.py
--rw-r--r--   0        0        0      547 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/smartapps.py
--rw-r--r--   0        0        0     2691 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/status.py
--rw-r--r--   0        0        0     1744 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/stickers.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/system_events/__init__.py
--rw-r--r--   0        0        0     1591 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/system_events/added_to_chat.py
--rw-r--r--   0        0        0     2964 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/system_events/chat_created.py
--rw-r--r--   0        0        0     1267 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/system_events/cts_login.py
--rw-r--r--   0        0        0     1277 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/system_events/cts_logout.py
--rw-r--r--   0        0        0     1746 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/system_events/deleted_from_chat.py
--rw-r--r--   0        0        0     2144 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/system_events/internal_bot_notification.py
--rw-r--r--   0        0        0     1600 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/system_events/left_from_chat.py
--rw-r--r--   0        0        0     3744 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/system_events/smartapp_event.py
--rw-r--r--   0        0        0     1571 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/models/users.py
--rw-r--r--   0        0        0        0 2023-07-25 10:36:06.362456 pybotx-0.55.8/pybotx/py.typed
--rw-r--r--   0        0        0     1247 2023-07-25 10:36:06.362456 pybotx-0.55.8/pyproject.toml
--rw-r--r--   0        0        0    22448 1970-01-01 00:00:00.000000 pybotx-0.55.8/PKG-INFO
+-rw-r--r--   0        0        0     6078 2023-07-26 09:14:44.641203 pybotx-0.56.0/LICENSE
+-rw-r--r--   0        0        0    21491 2023-07-26 09:14:44.641203 pybotx-0.56.0/README.md
+-rw-r--r--   0        0        0     6519 2023-07-26 09:14:44.641203 pybotx-0.56.0/pybotx/__init__.py
+-rw-r--r--   0        0        0      976 2023-07-26 09:14:44.641203 pybotx-0.56.0/pybotx/async_buffer.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.641203 pybotx-0.56.0/pybotx/bot/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.641203 pybotx-0.56.0/pybotx/bot/api/__init__.py
+-rw-r--r--   0        0        0      560 2023-07-26 09:14:44.641203 pybotx-0.56.0/pybotx/bot/api/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.641203 pybotx-0.56.0/pybotx/bot/api/responses/__init__.py
+-rw-r--r--   0        0        0     1048 2023-07-26 09:14:44.641203 pybotx-0.56.0/pybotx/bot/api/responses/bot_disabled.py
+-rw-r--r--   0        0        0      275 2023-07-26 09:14:44.641203 pybotx-0.56.0/pybotx/bot/api/responses/command_accepted.py
+-rw-r--r--   0        0        0    55005 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/bot.py
+-rw-r--r--   0        0        0     1558 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/bot_accounts_storage.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/callbacks/__init__.py
+-rw-r--r--   0        0        0     3101 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/callbacks/callback_manager.py
+-rw-r--r--   0        0        0     2176 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/callbacks/callback_memory_repo.py
+-rw-r--r--   0        0        0      983 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/callbacks/callback_repo_proto.py
+-rw-r--r--   0        0        0      330 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/contextvars.py
+-rw-r--r--   0        0        0      966 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/exceptions.py
+-rw-r--r--   0        0        0     2701 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/handler.py
+-rw-r--r--   0        0        0    14503 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/handler_collector.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/middlewares/__init__.py
+-rw-r--r--   0        0        0     1749 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/middlewares/exception_middleware.py
+-rw-r--r--   0        0        0      293 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/bot/testing.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/__init__.py
+-rw-r--r--   0        0        0     1617 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/authorized_botx_method.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/bots_api/__init__.py
+-rw-r--r--   0        0        0     1235 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/bots_api/get_token.py
+-rw-r--r--   0        0        0     6815 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/botx_method.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/__init__.py
+-rw-r--r--   0        0        0     2201 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/add_admin.py
+-rw-r--r--   0        0        0     1443 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/add_user.py
+-rw-r--r--   0        0        0     2975 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/chat_info.py
+-rw-r--r--   0        0        0     2177 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/create_chat.py
+-rw-r--r--   0        0        0     1415 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/disable_stealth.py
+-rw-r--r--   0        0        0     2004 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/list_chats.py
+-rw-r--r--   0        0        0     1398 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/pin_message.py
+-rw-r--r--   0        0        0     1430 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/remove_user.py
+-rw-r--r--   0        0        0     1699 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/set_stealth.py
+-rw-r--r--   0        0        0     1354 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/chats_api/unpin_message.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/events_api/__init__.py
+-rw-r--r--   0        0        0     3295 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/events_api/edit_event.py
+-rw-r--r--   0        0        0     2324 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/events_api/message_status_event.py
+-rw-r--r--   0        0        0     3770 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/events_api/reply_event.py
+-rw-r--r--   0        0        0     1019 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/events_api/stop_typing_event.py
+-rw-r--r--   0        0        0      955 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/events_api/typing_event.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/exceptions/__init__.py
+-rw-r--r--   0        0        0     1301 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/exceptions/base.py
+-rw-r--r--   0        0        0      889 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/exceptions/callbacks.py
+-rw-r--r--   0        0        0      424 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/exceptions/chats.py
+-rw-r--r--   0        0        0      429 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/exceptions/common.py
+-rw-r--r--   0        0        0      130 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/exceptions/event.py
+-rw-r--r--   0        0        0      289 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/exceptions/files.py
+-rw-r--r--   0        0        0      750 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/exceptions/http.py
+-rw-r--r--   0        0        0      378 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/exceptions/notifications.py
+-rw-r--r--   0        0        0      293 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/exceptions/users.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/files_api/__init__.py
+-rw-r--r--   0        0        0     2093 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/files_api/download_file.py
+-rw-r--r--   0        0        0     2448 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/files_api/upload_file.py
+-rw-r--r--   0        0        0      812 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/get_token.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/notifications_api/__init__.py
+-rw-r--r--   0        0        0     5567 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/notifications_api/direct_notification.py
+-rw-r--r--   0        0        0     2925 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/notifications_api/internal_bot_notification.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/openid_api/__init__.py
+-rw-r--r--   0        0        0     1245 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/openid_api/refresh_access_token.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/smartapps_api/__init__.py
+-rw-r--r--   0        0        0     2259 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/smartapps_api/smartapp_event.py
+-rw-r--r--   0        0        0     1836 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/smartapps_api/smartapp_notification.py
+-rw-r--r--   0        0        0     2195 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/smartapps_api/smartapps_list.py
+-rw-r--r--   0        0        0     1652 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/smartapps_api/upload_file.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.645203 pybotx-0.56.0/pybotx/client/stickers_api/__init__.py
+-rw-r--r--   0        0        0     2883 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/stickers_api/add_sticker.py
+-rw-r--r--   0        0        0     1689 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/stickers_api/create_sticker_pack.py
+-rw-r--r--   0        0        0     1506 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/stickers_api/delete_sticker.py
+-rw-r--r--   0        0        0     1426 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/stickers_api/delete_sticker_pack.py
+-rw-r--r--   0        0        0     1793 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/stickers_api/edit_sticker_pack.py
+-rw-r--r--   0        0        0      311 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/stickers_api/exceptions.py
+-rw-r--r--   0        0        0     1984 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/stickers_api/get_sticker.py
+-rw-r--r--   0        0        0     1397 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/stickers_api/get_sticker_pack.py
+-rw-r--r--   0        0        0     2352 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/stickers_api/get_sticker_packs.py
+-rw-r--r--   0        0        0     1321 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/stickers_api/sticker_pack.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/users_api/__init__.py
+-rw-r--r--   0        0        0     1231 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/users_api/search_user_by_email.py
+-rw-r--r--   0        0        0     1066 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/users_api/search_user_by_emails.py
+-rw-r--r--   0        0        0     1257 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/users_api/search_user_by_huid.py
+-rw-r--r--   0        0        0     1330 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/users_api/search_user_by_login.py
+-rw-r--r--   0        0        0     1254 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/users_api/search_user_by_other_id.py
+-rw-r--r--   0        0        0     3020 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/users_api/update_user_profile.py
+-rw-r--r--   0        0        0     1737 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/users_api/user_from_csv.py
+-rw-r--r--   0        0        0     2092 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/users_api/user_from_search.py
+-rw-r--r--   0        0        0     1659 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/client/users_api/users_as_csv.py
+-rw-r--r--   0        0        0      421 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/constants.py
+-rw-r--r--   0        0        0      221 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/converters.py
+-rw-r--r--   0        0        0      789 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/image_validators.py
+-rw-r--r--   0        0        0     1341 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/logger.py
+-rw-r--r--   0        0        0      648 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/missing.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/__init__.py
+-rw-r--r--   0        0        0     2079 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/api_base.py
+-rw-r--r--   0        0        0     7256 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/async_files.py
+-rw-r--r--   0        0        0    13052 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/attachments.py
+-rw-r--r--   0        0        0     2480 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/base_command.py
+-rw-r--r--   0        0        0      187 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/bot_account.py
+-rw-r--r--   0        0        0      199 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/bot_sender.py
+-rw-r--r--   0        0        0     1625 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/chats.py
+-rw-r--r--   0        0        0     1595 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/commands.py
+-rw-r--r--   0        0        0     8751 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/enums.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/message/__init__.py
+-rw-r--r--   0        0        0      670 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/message/edit_message.py
+-rw-r--r--   0        0        0      524 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/message/forward.py
+-rw-r--r--   0        0        0    10253 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/message/incoming_message.py
+-rw-r--r--   0        0        0     4714 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/message/markup.py
+-rw-r--r--   0        0        0     9106 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/message/mentions.py
+-rw-r--r--   0        0        0      270 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/message/message_status.py
+-rw-r--r--   0        0        0      882 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/message/outgoing_message.py
+-rw-r--r--   0        0        0      696 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/message/reply.py
+-rw-r--r--   0        0        0      825 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/message/reply_message.py
+-rw-r--r--   0        0        0      538 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/method_callbacks.py
+-rw-r--r--   0        0        0      547 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/smartapps.py
+-rw-r--r--   0        0        0     2691 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/status.py
+-rw-r--r--   0        0        0     1744 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/stickers.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/system_events/__init__.py
+-rw-r--r--   0        0        0     1591 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/system_events/added_to_chat.py
+-rw-r--r--   0        0        0     2964 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/system_events/chat_created.py
+-rw-r--r--   0        0        0     1267 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/system_events/cts_login.py
+-rw-r--r--   0        0        0     1277 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/system_events/cts_logout.py
+-rw-r--r--   0        0        0     1746 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/system_events/deleted_from_chat.py
+-rw-r--r--   0        0        0     2144 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/system_events/internal_bot_notification.py
+-rw-r--r--   0        0        0     1600 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/system_events/left_from_chat.py
+-rw-r--r--   0        0        0     3744 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/system_events/smartapp_event.py
+-rw-r--r--   0        0        0     1571 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/models/users.py
+-rw-r--r--   0        0        0        0 2023-07-26 09:14:44.649203 pybotx-0.56.0/pybotx/py.typed
+-rw-r--r--   0        0        0     1247 2023-07-26 09:14:44.649203 pybotx-0.56.0/pyproject.toml
+-rw-r--r--   0        0        0    22448 1970-01-01 00:00:00.000000 pybotx-0.56.0/PKG-INFO
```

### Comparing `pybotx-0.55.8/LICENSE` & `pybotx-0.56.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/README.md` & `pybotx-0.56.0/README.md`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/__init__.py` & `pybotx-0.56.0/pybotx/__init__.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/async_buffer.py` & `pybotx-0.56.0/pybotx/async_buffer.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/bot/api/exceptions.py` & `pybotx-0.56.0/pybotx/bot/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/bot/api/responses/bot_disabled.py` & `pybotx-0.56.0/pybotx/bot/api/responses/bot_disabled.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/bot/bot.py` & `pybotx-0.56.0/pybotx/bot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,18 @@
     BotXAPIGetStickerPacksRequestPayload,
     GetStickerPacksMethod,
 )
 from pybotx.client.users_api.search_user_by_email import (
     BotXAPISearchUserByEmailRequestPayload,
     SearchUserByEmailMethod,
 )
+from pybotx.client.users_api.search_user_by_emails import (
+    BotXAPISearchUserByEmailsRequestPayload,
+    SearchUserByEmailsMethod,
+)
 from pybotx.client.users_api.search_user_by_huid import (
     BotXAPISearchUserByHUIDRequestPayload,
     SearchUserByHUIDMethod,
 )
 from pybotx.client.users_api.search_user_by_login import (
     BotXAPISearchUserByLoginRequestPayload,
     SearchUserByLoginMethod,
@@ -1059,23 +1063,50 @@
             self._httpx_client,
             self._bot_accounts_storage,
         )
         payload = BotXAPIUnpinMessageRequestPayload.from_domain(chat_id=chat_id)
 
         await method.execute(payload)
 
+    async def search_user_by_emails(
+        self,
+        *,
+        bot_id: UUID,
+        emails: List[str],
+    ) -> List[UserFromSearch]:
+        """Search user by emails for search.
+
+        :param bot_id: Bot which should perform the request.
+        :param emails: User emails.
+
+        :return: Search result with user information.
+        """
+
+        method = SearchUserByEmailsMethod(
+            bot_id,
+            self._httpx_client,
+            self._bot_accounts_storage,
+        )
+        payload = BotXAPISearchUserByEmailsRequestPayload.from_domain(emails=emails)
+
+        botx_api_users_from_search = await method.execute(payload)
+
+        return botx_api_users_from_search.to_domain()
+
     # - Users API -
     async def search_user_by_email(
         self,
         *,
         bot_id: UUID,
         email: str,
     ) -> UserFromSearch:
         """Search user by email for search.
 
+        DEPRECATED.
+
         :param bot_id: Bot which should perform the request.
         :param email: User email.
 
         :return: User information.
         """
 
         method = SearchUserByEmailMethod(
```

### Comparing `pybotx-0.55.8/pybotx/bot/bot_accounts_storage.py` & `pybotx-0.56.0/pybotx/bot/bot_accounts_storage.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/bot/callbacks/callback_manager.py` & `pybotx-0.56.0/pybotx/bot/callbacks/callback_manager.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/bot/callbacks/callback_memory_repo.py` & `pybotx-0.56.0/pybotx/bot/callbacks/callback_memory_repo.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/bot/callbacks/callback_repo_proto.py` & `pybotx-0.56.0/pybotx/bot/callbacks/callback_repo_proto.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/bot/exceptions.py` & `pybotx-0.56.0/pybotx/bot/exceptions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/bot/handler.py` & `pybotx-0.56.0/pybotx/bot/handler.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/bot/handler_collector.py` & `pybotx-0.56.0/pybotx/bot/handler_collector.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/bot/middlewares/exception_middleware.py` & `pybotx-0.56.0/pybotx/bot/middlewares/exception_middleware.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/authorized_botx_method.py` & `pybotx-0.56.0/pybotx/client/authorized_botx_method.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/bots_api/get_token.py` & `pybotx-0.56.0/pybotx/client/bots_api/get_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/botx_method.py` & `pybotx-0.56.0/pybotx/client/botx_method.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/chats_api/add_admin.py` & `pybotx-0.56.0/pybotx/client/chats_api/add_admin.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/chats_api/add_user.py` & `pybotx-0.56.0/pybotx/client/chats_api/add_user.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/chats_api/chat_info.py` & `pybotx-0.56.0/pybotx/client/chats_api/chat_info.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/chats_api/create_chat.py` & `pybotx-0.56.0/pybotx/client/chats_api/create_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/chats_api/disable_stealth.py` & `pybotx-0.56.0/pybotx/client/chats_api/disable_stealth.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/chats_api/list_chats.py` & `pybotx-0.56.0/pybotx/client/chats_api/list_chats.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/chats_api/pin_message.py` & `pybotx-0.56.0/pybotx/client/chats_api/pin_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/chats_api/remove_user.py` & `pybotx-0.56.0/pybotx/client/chats_api/remove_user.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/chats_api/set_stealth.py` & `pybotx-0.56.0/pybotx/client/chats_api/set_stealth.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/chats_api/unpin_message.py` & `pybotx-0.56.0/pybotx/client/chats_api/unpin_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/events_api/edit_event.py` & `pybotx-0.56.0/pybotx/client/events_api/edit_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/events_api/message_status_event.py` & `pybotx-0.56.0/pybotx/client/events_api/message_status_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/events_api/reply_event.py` & `pybotx-0.56.0/pybotx/client/events_api/reply_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/events_api/stop_typing_event.py` & `pybotx-0.56.0/pybotx/client/events_api/stop_typing_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/events_api/typing_event.py` & `pybotx-0.56.0/pybotx/client/events_api/typing_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/exceptions/base.py` & `pybotx-0.56.0/pybotx/client/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/exceptions/callbacks.py` & `pybotx-0.56.0/pybotx/client/exceptions/callbacks.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/exceptions/http.py` & `pybotx-0.56.0/pybotx/client/exceptions/http.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/files_api/download_file.py` & `pybotx-0.56.0/pybotx/client/files_api/download_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/files_api/upload_file.py` & `pybotx-0.56.0/pybotx/client/files_api/upload_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/get_token.py` & `pybotx-0.56.0/pybotx/client/get_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/notifications_api/direct_notification.py` & `pybotx-0.56.0/pybotx/client/notifications_api/direct_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/notifications_api/internal_bot_notification.py` & `pybotx-0.56.0/pybotx/client/notifications_api/internal_bot_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/openid_api/refresh_access_token.py` & `pybotx-0.56.0/pybotx/client/openid_api/refresh_access_token.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/smartapps_api/smartapp_event.py` & `pybotx-0.56.0/pybotx/client/smartapps_api/smartapp_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/smartapps_api/smartapp_notification.py` & `pybotx-0.56.0/pybotx/client/smartapps_api/smartapp_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/smartapps_api/smartapps_list.py` & `pybotx-0.56.0/pybotx/client/smartapps_api/smartapps_list.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/smartapps_api/upload_file.py` & `pybotx-0.56.0/pybotx/client/smartapps_api/upload_file.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/stickers_api/add_sticker.py` & `pybotx-0.56.0/pybotx/client/stickers_api/add_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/stickers_api/create_sticker_pack.py` & `pybotx-0.56.0/pybotx/client/stickers_api/create_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/stickers_api/delete_sticker.py` & `pybotx-0.56.0/pybotx/client/stickers_api/delete_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/stickers_api/delete_sticker_pack.py` & `pybotx-0.56.0/pybotx/client/stickers_api/delete_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/stickers_api/edit_sticker_pack.py` & `pybotx-0.56.0/pybotx/client/stickers_api/edit_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/stickers_api/get_sticker.py` & `pybotx-0.56.0/pybotx/client/stickers_api/get_sticker.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/stickers_api/get_sticker_pack.py` & `pybotx-0.56.0/pybotx/client/stickers_api/get_sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/stickers_api/get_sticker_packs.py` & `pybotx-0.56.0/pybotx/client/stickers_api/get_sticker_packs.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/stickers_api/sticker_pack.py` & `pybotx-0.56.0/pybotx/client/stickers_api/sticker_pack.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/users_api/search_user_by_email.py` & `pybotx-0.56.0/pybotx/client/users_api/search_user_by_email.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/users_api/search_user_by_huid.py` & `pybotx-0.56.0/pybotx/client/users_api/search_user_by_huid.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/users_api/search_user_by_login.py` & `pybotx-0.56.0/pybotx/client/users_api/search_user_by_login.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/users_api/search_user_by_other_id.py` & `pybotx-0.56.0/pybotx/client/users_api/search_user_by_other_id.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/users_api/update_user_profile.py` & `pybotx-0.56.0/pybotx/client/users_api/update_user_profile.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/users_api/user_from_csv.py` & `pybotx-0.56.0/pybotx/client/users_api/user_from_csv.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/client/users_api/user_from_search.py` & `pybotx-0.56.0/pybotx/client/users_api/user_from_search.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,7 +34,29 @@
             company=self.result.company,
             company_position=self.result.company_position,
             department=self.result.department,
             emails=self.result.emails,
             other_id=self.result.other_id,
             user_kind=convert_user_kind_to_domain(self.result.user_kind),
         )
+
+
+class BotXAPISearchUserByEmailsResponsePayload(VerifiedPayloadBaseModel):
+    status: Literal["ok"]
+    result: List[BotXAPISearchUserResult]
+
+    def to_domain(self) -> List[UserFromSearch]:
+        return [
+            UserFromSearch(
+                huid=user.user_huid,
+                ad_login=user.ad_login,
+                ad_domain=user.ad_domain,
+                username=user.name,
+                company=user.company,
+                company_position=user.company_position,
+                department=user.department,
+                emails=user.emails,
+                other_id=user.other_id,
+                user_kind=convert_user_kind_to_domain(user.user_kind),
+            )
+            for user in self.result
+        ]
```

### Comparing `pybotx-0.55.8/pybotx/client/users_api/users_as_csv.py` & `pybotx-0.56.0/pybotx/client/users_api/users_as_csv.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/image_validators.py` & `pybotx-0.56.0/pybotx/image_validators.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/logger.py` & `pybotx-0.56.0/pybotx/logger.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/missing.py` & `pybotx-0.56.0/pybotx/missing.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/api_base.py` & `pybotx-0.56.0/pybotx/models/api_base.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/async_files.py` & `pybotx-0.56.0/pybotx/models/async_files.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/attachments.py` & `pybotx-0.56.0/pybotx/models/attachments.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/base_command.py` & `pybotx-0.56.0/pybotx/models/base_command.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/chats.py` & `pybotx-0.56.0/pybotx/models/chats.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/commands.py` & `pybotx-0.56.0/pybotx/models/commands.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/enums.py` & `pybotx-0.56.0/pybotx/models/enums.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/message/edit_message.py` & `pybotx-0.56.0/pybotx/models/message/edit_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/message/forward.py` & `pybotx-0.56.0/pybotx/models/message/forward.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/message/incoming_message.py` & `pybotx-0.56.0/pybotx/models/message/incoming_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/message/markup.py` & `pybotx-0.56.0/pybotx/models/message/markup.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/message/mentions.py` & `pybotx-0.56.0/pybotx/models/message/mentions.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/message/outgoing_message.py` & `pybotx-0.56.0/pybotx/models/message/outgoing_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/message/reply.py` & `pybotx-0.56.0/pybotx/models/message/reply.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/message/reply_message.py` & `pybotx-0.56.0/pybotx/models/message/reply_message.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/method_callbacks.py` & `pybotx-0.56.0/pybotx/models/method_callbacks.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/smartapps.py` & `pybotx-0.56.0/pybotx/models/smartapps.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/status.py` & `pybotx-0.56.0/pybotx/models/status.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/stickers.py` & `pybotx-0.56.0/pybotx/models/stickers.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/system_events/added_to_chat.py` & `pybotx-0.56.0/pybotx/models/system_events/added_to_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/system_events/chat_created.py` & `pybotx-0.56.0/pybotx/models/system_events/chat_created.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/system_events/cts_login.py` & `pybotx-0.56.0/pybotx/models/system_events/cts_login.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/system_events/cts_logout.py` & `pybotx-0.56.0/pybotx/models/system_events/cts_logout.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/system_events/deleted_from_chat.py` & `pybotx-0.56.0/pybotx/models/system_events/deleted_from_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/system_events/internal_bot_notification.py` & `pybotx-0.56.0/pybotx/models/system_events/internal_bot_notification.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/system_events/left_from_chat.py` & `pybotx-0.56.0/pybotx/models/system_events/left_from_chat.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/system_events/smartapp_event.py` & `pybotx-0.56.0/pybotx/models/system_events/smartapp_event.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pybotx/models/users.py` & `pybotx-0.56.0/pybotx/models/users.py`

 * *Files identical despite different names*

### Comparing `pybotx-0.55.8/pyproject.toml` & `pybotx-0.56.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pybotx"
-version = "0.55.8"
+version = "0.56.0"
 description = "A python library for interacting with eXpress BotX API"
 authors = [
     "Sidnev Nikolay <nsidnev@ccsteam.ru>",
     "Maxim Gorbachev <mgorbachev@ccsteam.ru>",
     "Alexander Samoylenko <alexandr.samojlenko@ccsteam.ru>",
     "Arseniy Zhiltsov <arseniy.zhiltsov@ccsteam.ru>"
 ]
```

### Comparing `pybotx-0.55.8/PKG-INFO` & `pybotx-0.56.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybotx
-Version: 0.55.8
+Version: 0.56.0
 Summary: A python library for interacting with eXpress BotX API
 Home-page: https://github.com/ExpressApp/pybotx
 Author: Sidnev Nikolay
 Author-email: nsidnev@ccsteam.ru
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

