# Comparing `tmp/mipac-0.4.99.tar.gz` & `tmp/mipac-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mipac-0.4.99.tar", last modified: Sun Jun 18 02:31:40 2023, max compression
+gzip compressed data, was "mipac-0.5.0.tar", last modified: Wed Jul 26 00:56:27 2023, max compression
```

## Comparing `mipac-0.4.99.tar` & `mipac-0.5.0.tar`

### file list

```diff
@@ -1,151 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.727592 mipac-0.4.99/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-18 02:31:31.000000 mipac-0.4.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-18 02:31:31.000000 mipac-0.4.99/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-18 02:31:40.727592 mipac-0.4.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-18 02:31:31.000000 mipac-0.4.99/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.727592 mipac-0.4.99/mipac/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-18 02:31:40.727592 mipac-0.4.99/mipac/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.715592 mipac-0.4.99/mipac/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/abstract/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/abstract/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/abstract/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.715592 mipac-0.4.99/mipac/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.719592 mipac-0.4.99/mipac/actions/admins/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/moderator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/admins/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/antenna.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/favorite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/federation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/my.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/actions/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.719592 mipac-0.4.99/mipac/errors/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/errors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/errors/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/http.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.719592 mipac-0.4.99/mipac/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.719592 mipac-0.4.99/mipac/manager/admins/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/moderator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/admins/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/antenna.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/favorite.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/federation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/my.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/note.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/page.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/manager/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.723592 mipac-0.4.99/mipac/models/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/ad.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/antenna.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.723592 mipac-0.4.99/mipac/models/lite/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/lite/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/models/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.727592 mipac-0.4.99/mipac/types/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/achievement.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/ads.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/announcement.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/antenna.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/follow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/mute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/note.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/page.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/reaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/roles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/types/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.727592 mipac-0.4.99/mipac/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-18 02:31:31.000000 mipac-0.4.99/mipac/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 02:31:40.715592 mipac-0.4.99/mipac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-18 02:31:40.000000 mipac-0.4.99/mipac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-18 02:31:40.000000 mipac-0.4.99/mipac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 02:31:40.000000 mipac-0.4.99/mipac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-18 02:31:40.000000 mipac-0.4.99/mipac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-18 02:31:40.000000 mipac-0.4.99/mipac.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-18 02:31:31.000000 mipac-0.4.99/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-18 02:31:31.000000 mipac-0.4.99/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-18 02:31:40.727592 mipac-0.4.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-18 02:31:31.000000 mipac-0.4.99/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-06-18 02:31:31.000000 mipac-0.4.99/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.477675 mipac-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-26 00:56:15.000000 mipac-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-26 00:56:15.000000 mipac-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-26 00:56:27.477675 mipac-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-07-26 00:56:15.000000 mipac-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.461675 mipac-0.5.0/mipac/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-26 00:56:27.477675 mipac-0.5.0/mipac/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.461675 mipac-0.5.0/mipac/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/abstract/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/abstract/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/abstract/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.465675 mipac-0.5.0/mipac/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.465675 mipac-0.5.0/mipac/actions/admins/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/admins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/admins/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9086 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/admins/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/admins/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/admins/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/admins/moderator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10575 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/admins/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/admins/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/antenna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5259 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/favorite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/my.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19610 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/actions/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.465675 mipac-0.5.0/mipac/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/errors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8878 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/errors/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/http.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.469675 mipac-0.5.0/mipac/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.469675 mipac-0.5.0/mipac/manager/admins/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/admins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/admins/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/admins/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/admins/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/admins/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/admins/moderator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/admins/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/admins/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/antenna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/favorite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/my.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/manager/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.469675 mipac-0.5.0/mipac/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/ad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/antenna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.473675 mipac-0.5.0/mipac/models/lite/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/lite/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/lite/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/lite/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/lite/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/lite/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/lite/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/models/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.473675 mipac-0.5.0/mipac/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/achievement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/ads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/announcement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/antenna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10807 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/follow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/mute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/reaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/types/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11528 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.477675 mipac-0.5.0/mipac/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/utils/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/utils/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-26 00:56:15.000000 mipac-0.5.0/mipac/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:56:27.461675 mipac-0.5.0/mipac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-07-26 00:56:27.000000 mipac-0.5.0/mipac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-26 00:56:27.000000 mipac-0.5.0/mipac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:56:27.000000 mipac-0.5.0/mipac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-26 00:56:27.000000 mipac-0.5.0/mipac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 00:56:27.000000 mipac-0.5.0/mipac.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-26 00:56:15.000000 mipac-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-26 00:56:15.000000 mipac-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-26 00:56:27.477675 mipac-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-26 00:56:15.000000 mipac-0.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-07-26 00:56:15.000000 mipac-0.5.0/versioneer.py
```

### Comparing `mipac-0.4.99/LICENSE` & `mipac-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/PKG-INFO` & `mipac-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipac
-Version: 0.4.99
+Version: 0.5.0
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/mipac
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
@@ -57,47 +57,32 @@
     note = await api.note.action.send('Hello World')
     print(note.author.name, note.content)
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
-### Migration from v0.3.0 to v0.4.0
-
-#### configの属性が変更されました
-
-- `is_official` が削除されました
-
-##### **重要** `use_version` が追加されました
-
-Misskeyではv11,v12,v13とバージョンがあり、バージョンによっては使用できないAPIがあったりします。MiPACでは`use_version`を指定することで事前に使用できるかどうかを確認し、使用できない場合は`NotSupportVersion`という例外を返します。このようにご自分のインスタンスのバージョンを書いていただくだけで、よくわからないエラーを事前に防ぐことが出来ます。（issue等にエラーを報告場合は必ず適切に設定されているか確認してください）
-
-v13はまだリリースされて日が浅く、全てのインスタンスがアップデートしたとは考えにくいため、現在のデフォルト値は`12`となっています。
+### 注意事項
 
-#### `Client` のオプションから `config`が削除されました
+### Python3.12.0 final がリリースされ、3カ月経過後に最低バージョンを 3.12.0 に変更します
 
-今後configを参照する際は `Client.config` を使用してください。
-また、値を更新する場合はClient.config.from_dict()を用いることをお勧めします。
-通常の変更方法との違いは以下の通りです。
+これは主にMiPACの開発を行う上で、新規構文の使用などによってDXがより良くなり開発ペースが向上する為です。
+また、使用者の皆様においてはPythonの高速化や新規構文の使用などが使用できるといった恩恵を得ることができます。
 
-```python
-Client.config.is_ayuskey = True
-Client.config.use_version = 13
-Client.config.from_dict(is_ayuskey=True, use_version=13)
-```
+現在Python3.12.0のリリースは以下のように記載されているため、早くて **2024年01月02日** に変更を実施する予定です。
 
-上記のように複数の値を同時に更新する場合特に`from_dict`は有効な方法になります。
+ > `3.12.0 final: Monday, 2023-10-02`
 
-### 注意事項
+ これについて意見がある場合はDiscussionを作成することができます。
 
 ### 一部サーバー(インスタンス)のバージョンによっては正常に動作しない可能性があります
 
 MiPACの特徴として、v11,v12,v13のバージョンごとに生じる変更点をなるべく気にしなくてよいように作成していますが、現状の最新版であるv13でもv13の中で削除されたり、増えたりした物があります。結果的に追従しきれていない箇所があることがあります。そのため、そのような物を見つけた場合は、使用しているサーバーのバージョンと使用できないエンドポイント名をIssueに送信してください。
 
-### モデルを基本的に自分でインスタンス化することは推奨しません
+### モデルを自分でインスタンス化することは推奨されません
 
 MiPACのモデルでは多くの場合、キーワード引数に `client`を受け取り、それを用いて`api` プロパティを生成します。しかし、サポート途中の機能なのではそこが省かれ、リリース後にモデルのインスタンス化に必要な引数として `client` が追加されることがあります。また、他にもモデルの更新のために引数が変更される可能性があります。そのため、引数の変更に関することをCHANGELOG等で通知することはありません。
 
 ### 開発者向け情報
 
 このプロジェクトでは [black](https://github.com/psf/black)のforkである、[axblack](https://github.com/axiros/axblack)を利用しています。主な違いはダブルクォートがデフォルトではなく、シングルクォートになっている点です
```

### Comparing `mipac-0.4.99/README.md` & `mipac-0.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -37,47 +37,32 @@
     note = await api.note.action.send('Hello World')
     print(note.author.name, note.content)
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
-### Migration from v0.3.0 to v0.4.0
-
-#### configの属性が変更されました
-
-- `is_official` が削除されました
-
-##### **重要** `use_version` が追加されました
-
-Misskeyではv11,v12,v13とバージョンがあり、バージョンによっては使用できないAPIがあったりします。MiPACでは`use_version`を指定することで事前に使用できるかどうかを確認し、使用できない場合は`NotSupportVersion`という例外を返します。このようにご自分のインスタンスのバージョンを書いていただくだけで、よくわからないエラーを事前に防ぐことが出来ます。（issue等にエラーを報告場合は必ず適切に設定されているか確認してください）
-
-v13はまだリリースされて日が浅く、全てのインスタンスがアップデートしたとは考えにくいため、現在のデフォルト値は`12`となっています。
+### 注意事項
 
-#### `Client` のオプションから `config`が削除されました
+### Python3.12.0 final がリリースされ、3カ月経過後に最低バージョンを 3.12.0 に変更します
 
-今後configを参照する際は `Client.config` を使用してください。
-また、値を更新する場合はClient.config.from_dict()を用いることをお勧めします。
-通常の変更方法との違いは以下の通りです。
+これは主にMiPACの開発を行う上で、新規構文の使用などによってDXがより良くなり開発ペースが向上する為です。
+また、使用者の皆様においてはPythonの高速化や新規構文の使用などが使用できるといった恩恵を得ることができます。
 
-```python
-Client.config.is_ayuskey = True
-Client.config.use_version = 13
-Client.config.from_dict(is_ayuskey=True, use_version=13)
-```
+現在Python3.12.0のリリースは以下のように記載されているため、早くて **2024年01月02日** に変更を実施する予定です。
 
-上記のように複数の値を同時に更新する場合特に`from_dict`は有効な方法になります。
+ > `3.12.0 final: Monday, 2023-10-02`
 
-### 注意事項
+ これについて意見がある場合はDiscussionを作成することができます。
 
 ### 一部サーバー(インスタンス)のバージョンによっては正常に動作しない可能性があります
 
 MiPACの特徴として、v11,v12,v13のバージョンごとに生じる変更点をなるべく気にしなくてよいように作成していますが、現状の最新版であるv13でもv13の中で削除されたり、増えたりした物があります。結果的に追従しきれていない箇所があることがあります。そのため、そのような物を見つけた場合は、使用しているサーバーのバージョンと使用できないエンドポイント名をIssueに送信してください。
 
-### モデルを基本的に自分でインスタンス化することは推奨しません
+### モデルを自分でインスタンス化することは推奨されません
 
 MiPACのモデルでは多くの場合、キーワード引数に `client`を受け取り、それを用いて`api` プロパティを生成します。しかし、サポート途中の機能なのではそこが省かれ、リリース後にモデルのインスタンス化に必要な引数として `client` が追加されることがあります。また、他にもモデルの更新のために引数が変更される可能性があります。そのため、引数の変更に関することをCHANGELOG等で通知することはありません。
 
 ### 開発者向け情報
 
 このプロジェクトでは [black](https://github.com/psf/black)のforkである、[axblack](https://github.com/axiros/axblack)を利用しています。主な違いはダブルクォートがデフォルトではなく、シングルクォートになっている点です
```

### Comparing `mipac-0.4.99/mipac/__init__.py` & `mipac-0.5.0/mipac/__init__.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/admins/ad.py` & `mipac-0.5.0/mipac/actions/admins/ad.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/admins/admin.py` & `mipac-0.5.0/mipac/actions/admins/admin.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/admins/announcement.py` & `mipac-0.5.0/mipac/actions/admins/announcement.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/admins/emoji.py` & `mipac-0.5.0/mipac/actions/admins/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/admins/moderator.py` & `mipac-0.5.0/mipac/actions/admins/moderator.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/admins/roles.py` & `mipac-0.5.0/mipac/actions/admins/roles.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/admins/user.py` & `mipac-0.5.0/mipac/actions/admins/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/antenna.py` & `mipac-0.5.0/mipac/actions/antenna.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/blocking.py` & `mipac-0.5.0/mipac/actions/blocking.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/chart.py` & `mipac-0.5.0/mipac/actions/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/chat.py` & `mipac-0.5.0/mipac/actions/chat.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,20 @@
             Message id
 
         Returns
         -------
         bool
             Success or Failure.
         """
+        if (
+            self.__client._config.use_version >= 13
+            and self.__client._config.features.chat is False
+        ):
+            raise NotSupportVersion(NotSupportVersionText)
+
         if check_multi_arg(message_id, self.__message_id) is False:
             raise ParameterError('message_idがありません')
         message_id = message_id or self.__message_id
         body = {'messageId': message_id}
         res: bool = await self.__session.request(
             Route('POST', '/api/messaging/messages/read'), json=body, auth=True, lower=True,
         )
@@ -60,14 +66,19 @@
             Message id
 
         Returns
         -------
         bool
             Success or Failure.
         """
+        if (
+            self.__client._config.use_version >= 13
+            and self.__client._config.features.chat is False
+        ):
+            raise NotSupportVersion(NotSupportVersionText)
 
         if check_multi_arg(message_id, self.__message_id) is False:
             raise ParameterError('message_idがありません')
 
         message_id = message_id or self.__message_id
         body = {'messageId': f'{message_id}'}
         res: bool = await self.__session.request(
```

### Comparing `mipac-0.4.99/mipac/actions/client.py` & `mipac-0.5.0/mipac/actions/client.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/drive.py` & `mipac-0.5.0/mipac/actions/drive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, AsyncGenerator
+import io
+from http.client import HTTPException
+from os import PathLike
+from typing import TYPE_CHECKING, Any, AsyncGenerator
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import ParameterError
 from mipac.http import HTTPClient, Route
 from mipac.models.drive import File, Folder
 from mipac.types.drive import FolderPayload, IDriveFile
 from mipac.utils.format import bool_to_string, remove_dict_empty
@@ -18,22 +21,24 @@
 
 
 class ClientFileActions(AbstractAction):
     def __init__(
         self,
         file_id: str | None = None,
         folder_id: str | None = None,
+        url: str | None = None,
         *,
         session: HTTPClient,
         client: ClientManager
     ) -> None:
         self._session: HTTPClient = session
         self._client: ClientManager = client
         self._file_id = file_id
         self._folder_id = folder_id
+        self._url = url
 
     async def remove(self, file_id: str | None = None) -> bool:
         """
         指定したIDのファイルを削除します
 
         Parameters
         ----------
@@ -43,20 +48,48 @@
         Returns
         -------
         bool
             削除に成功したかどうか
         """
 
         file_id = file_id or self._file_id
+        if file_id is None:
+            raise ParameterError('file_id is required')
+
         return bool(
             await self._session.request(
                 Route('POST', '/api/drive/files/delete'), json={'fileId': file_id}, auth=True,
             )
         )
 
+    async def save(
+        self,
+        fp: io.BufferedIOBase | PathLike[Any],
+        file_id: str | None = None,
+        url: str | None = None,
+    ):
+        file_id = file_id or self._file_id
+        url = url or self._url
+        if any([file_id, url]) is False:
+            raise ParameterError('file_id is required')
+
+        if url is None:
+            result = await self._client.drive.file.action.show_file(file_id=file_id)
+            url = result.url
+
+        async with self._session.session.get(url) as resp:
+            if resp.status == 200:
+                content = await resp.read()
+                with open(fp, 'wb') as f:
+                    return f.write(content)
+            elif resp.status == 400:
+                raise FileNotFoundError('File not found')
+            else:
+                raise HTTPException(resp, 'Failed to get file')
+
     @deprecated
     async def remove_file(self, file_id: str | None = None) -> bool:
         """
         指定したIDのファイルを削除します
 
         Parameters
         ----------
@@ -78,19 +111,22 @@
 
 
 class FileActions(ClientFileActions):
     def __init__(
         self,
         file_id: str | None = None,
         folder_id: str | None = None,
+        url: str | None = None,
         *,
         session: HTTPClient,
         client: ClientManager
     ) -> None:
-        super().__init__(file_id=file_id, folder_id=folder_id, session=session, client=client)
+        super().__init__(
+            file_id=file_id, folder_id=folder_id, url=url, session=session, client=client
+        )
 
     async def show_file(self, file_id: str | None = None, url: str | None = None) -> File:
         """
         ファイルの情報を取得します。
 
         Parameters
         ----------
```

### Comparing `mipac-0.4.99/mipac/actions/emoji.py` & `mipac-0.5.0/mipac/actions/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/favorite.py` & `mipac-0.5.0/mipac/actions/favorite.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/federation.py` & `mipac-0.5.0/mipac/actions/federation.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/follow.py` & `mipac-0.5.0/mipac/actions/follow.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/mute.py` & `mipac-0.5.0/mipac/actions/mute.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/my.py` & `mipac-0.5.0/mipac/actions/my.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/note.py` & `mipac-0.5.0/mipac/actions/note.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, AsyncGenerator, Literal
+from typing import TYPE_CHECKING, AsyncGenerator
 
 from mipac.abstract.action import AbstractAction
 from mipac.errors.base import APIError, ParameterError
 from mipac.file import MiFile
 from mipac.http import HTTPClient, Route
+from mipac.models.clip import Clip
 from mipac.models.drive import File
 from mipac.models.note import Note, NoteReaction, NoteState, NoteTranslateResult
 from mipac.models.poll import MiPoll, Poll
-from mipac.types.note import ICreatedNote, INote, INoteState, INoteTranslateResult
+from mipac.types.clip import IClip
+from mipac.types.note import ICreatedNote, INote, INoteState, INoteTranslateResult, INoteVisibility
 from mipac.utils.cache import cache
 from mipac.utils.format import remove_dict_empty
 from mipac.utils.pagination import Pagination
 from mipac.utils.util import check_multi_arg
 
 if TYPE_CHECKING:
     from mipac.client import ClientManager
 
 __all__ = ['NoteActions']
 
 
 def create_note_body(
     content: str | None = None,
-    visibility: Literal['public', 'home', 'followers', 'specified'] = 'public',
+    visibility: INoteVisibility = 'public',
     visible_user_ids: list[str] | None = None,
     cw: str | None = None,
     local_only: bool = False,
     extract_mentions: bool = True,
     extract_hashtags: bool = True,
     extract_emojis: bool = True,
     reply_id: str | None = None,
@@ -97,14 +99,18 @@
             Target note Id., by default None
 
         Returns
         -------
         bool
             Whether the release was successful
         """
+        note_id = note_id or self._note_id
+
+        if note_id is None:
+            raise ParameterError('note_id is required')
 
         body = {'noteId': note_id}
         res: bool = await self._session.request(
             Route('POST', '/api/notes/unrenote'), auth=True, json=body
         )
         return res
 
@@ -112,22 +118,25 @@
         self,
         limit: int = 100,
         since_id: str | None = None,
         untilId: str | None = None,
         note_id: str | None = None,
         get_all: bool = True,
     ) -> AsyncGenerator[Note, None]:
-
         if limit > 100:
             raise ParameterError('limit は100以下である必要があります')
 
         if get_all:
             limit = 100
 
         note_id = note_id or self._note_id
+
+        if note_id is None:
+            raise ParameterError('note_id is required')
+
         data = {
             'noteId': note_id,
             'limit': limit,
             'sinceId': since_id,
             'untilId': untilId,
         }
 
@@ -141,14 +150,18 @@
                 yield Note(note, self._client)
 
             if get_all is False or pagination.is_final:
                 break
 
     async def get_state(self, note_id: str | None = None) -> NoteState:
         note_id = note_id or self._note_id
+
+        if note_id is None:
+            raise ParameterError('note_id is required')
+
         data = {'noteId': note_id}
         res: INoteState = await self._session.request(
             Route('POST', '/api/notes/state'), auth=True, json=data
         )
         return NoteState(res)
 
     async def add_clips(self, clip_id: str, note_id: str | None = None) -> bool:
@@ -168,19 +181,48 @@
         -------
         bool
             成功したか否か
         """
 
         note_id = note_id or self._note_id
 
+        if note_id is None:
+            raise ParameterError('note_id is required')
+
         data = {'noteId': note_id, 'clipId': clip_id}
         return bool(
             await self._session.request(Route('POST', '/api/clips/add-note'), json=data, auth=True)
         )
 
+    async def get_clips(self, note_id: str | None = None) -> list[Clip]:
+        """
+        クリップを取得します
+
+        Parameters
+        ----------
+        note_id : str | None, default=None
+            取得したいノートのID
+
+        Returns
+        -------
+        list[Clip]
+            クリップのリスト
+        """
+
+        note_id = note_id or self._note_id
+
+        if note_id is None:
+            raise ParameterError('note_id is required')
+
+        data = {'noteId': note_id}
+        res: list[IClip] = await self._session.request(
+            Route('POST', '/api/notes/clips'), json=data, auth=True
+        )
+        return [Clip(clip, client=self._client) for clip in res]
+
     async def delete(self, note_id: str | None = None) -> bool:
         """
         Delete a note
 
         Parameters
         ----------
         note_id : str | None, default=None
@@ -190,14 +232,17 @@
         -------
         bool
             success or not
         """
 
         note_id = note_id or self._note_id
 
+        if note_id is None:
+            raise ParameterError('note_id is required')
+
         data = {'noteId': note_id}
         res = await self._session.request(Route('POST', '/api/notes/delete'), json=data, auth=True)
         return bool(res)
 
     async def create_renote(self, note_id: str | None = None) -> Note:
         """
         Renote a note
@@ -208,43 +253,51 @@
             note id
 
         Returns
         -------
         Note
             Renoted note
         """
-        body = create_note_body(renote_id=note_id,)
+
+        note_id = self._note_id or note_id
+
+        if note_id is None:
+            raise ParameterError('note_id is required')
+
+        body = create_note_body(renote_id=note_id)
         res: ICreatedNote = await self._session.request(
             Route('POST', '/api/notes/create'), json=body, auth=True, lower=True,
         )
         return Note(res['created_note'], client=self._client)
 
     async def get_reaction(self, reaction: str, note_id: str | None = None) -> list[NoteReaction]:
         note_id = note_id or self._note_id
         return await self._client.note.reaction.action.get_reaction(
             reaction
         )  # TODO: note.reactionのインタンスを新規作成出来るように
 
     async def reply(
         self,
         content: str | None = None,
-        visibility: Literal['public', 'home', 'followers', 'specified'] = 'public',
+        visibility: INoteVisibility = 'public',
         visible_user_ids: list[str] | None = None,
         cw: str | None = None,
         local_only: bool = False,
         extract_mentions: bool = True,
         extract_hashtags: bool = True,
         extract_emojis: bool = True,
         files: list[MiFile | File | str] | None = None,
         poll: MiPoll | None = None,
         reply_id: str | None = None,
     ) -> Note:
-
         reply_id = reply_id or self._note_id
 
+        if reply_id is None:
+            raise ParameterError('reply_id is required')
+
         body = create_note_body(
             content=content,
             cw=cw,
             visibility=visibility,
             visible_user_ids=visible_user_ids,
             extract_emojis=extract_emojis,
             extract_hashtags=extract_hashtags,
@@ -258,15 +311,15 @@
             Route('POST', '/api/notes/create'), json=body, lower=True, auth=True,
         )
         return Note(res['created_note'], client=self._client)
 
     async def create_quote(
         self,
         content: str | None = None,
-        visibility: Literal['public', 'home', 'followers', 'specified'] = 'public',
+        visibility: INoteVisibility = 'public',
         visible_user_ids: list[str] | None = None,
         cw: str | None = None,
         local_only: bool = False,
         extract_mentions: bool = True,
         extract_hashtags: bool = True,
         extract_emojis: bool = True,
         files: list[MiFile | File | str] | None = None,
@@ -276,15 +329,15 @@
         """
         Create a note quote.
 
         Parameters
         ----------
         content: str | None, default=None
             text
-        visibility: Literal['public', 'home', 'followers', 'specified'], default='public'
+        visibility: INoteVisibility, default='public'
             Disclosure range
         visible_user_ids: list[str] | None, default=None
             List of users to be published
         cw: str | None, default=None
             Text to be displayed when warning is given
         local_only: bool, default=False
             Whether to show only locally or not
@@ -300,14 +353,17 @@
             Questionnaire to be created
         note_id: str | None, default=None
             Note IDs to target for renote and citations
         """
 
         note_id = note_id or self._note_id
 
+        if note_id is None:
+            raise ParameterError('note_id is required')
+
         body = create_note_body(
             content=content,
             cw=cw,
             visibility=visibility,
             visible_user_ids=visible_user_ids,
             extract_emojis=extract_emojis,
             extract_hashtags=extract_hashtags,
@@ -340,34 +396,86 @@
         Returns
         -------
         NoteTranslateResult
             Translated result
         """
         note_id = note_id or self._note_id
 
+        if note_id is None:
+            raise ParameterError('note_id is required')
+
         data = {'noteId': note_id, 'targetLang': target_lang}
         res: INoteTranslateResult = await self._session.request(
             Route('POST', '/api/notes/translate'), json=data, auth=True
         )
         if isinstance(res, dict):
             return NoteTranslateResult(res)
         APIError(f'Translate Error: {res}', res if isinstance(res, int) else 204).raise_error()
 
+    async def get_replies(
+        self,
+        since_id: str | None = None,
+        until_id: str | None = None,
+        limit: int = 10,
+        note_id: str | None = None,
+        get_all: bool = False,
+    ) -> AsyncGenerator[Note, None]:
+        """
+        ノートに対する返信を取得します
+
+        Parameters
+        ---------
+        since_id : str | None, default=None
+            指定すると、その投稿を投稿を起点としてより新しい投稿を取得します
+        until_id : str | None, default=None
+            指定すると、その投稿を投稿を起点としてより古い投稿を取得します
+        limit : int, default=10
+            取得する上限
+        note_id: str | None, default=None
+            返信を取得したいノートのID
+
+        Returns
+        -------
+        AsyncGenerator[Note, None]
+            返信
+        """
+
+        if limit > 100:
+            raise ParameterError('limitは100以下である必要があります')
+        if get_all:
+            limit = 100
+
+        note_id = note_id or self._note_id
+
+        if note_id is None:
+            raise ParameterError('note_id is required')
+
+        body = {'noteId': note_id, 'sinceId': since_id, 'untilId': until_id, 'limit': limit}
+
+        pagination = Pagination[INote](self._session, Route('POST', '/api/notes'), json=body)
+
+        while True:
+            res_notes = await pagination.next()
+            for res_note in res_notes:
+                yield Note(res_note, client=self._client)
+
+            if get_all is False or pagination.is_final:
+                break
+
 
 class NoteActions(ClientNoteActions):
     def __init__(
         self, note_id: str | None = None, *, session: HTTPClient, client: ClientManager,
     ):
-
         super().__init__(note_id=note_id, session=session, client=client)
 
     async def send(
         self,
         content: str | None = None,
-        visibility: Literal['public', 'home', 'followers', 'specified'] = 'public',
+        visibility: INoteVisibility = 'public',
         visible_user_ids: list[str] | None = None,
         cw: str | None = None,
         local_only: bool = False,
         extract_mentions: bool = True,
         extract_hashtags: bool = True,
         extract_emojis: bool = True,
         reply_id: str | None = None,
@@ -379,15 +487,15 @@
         """
         ノートを投稿します。
 
         Parameters
         ----------
         content : str | None, default=None
             投稿する内容
-        visibility : Literal['public', 'home', 'followers', 'specified'], optional
+        visibility : INoteVisibility, optional
             公開範囲, by default "public"
             Enum: "public" "home" "followers" "specified"
         visible_user_ids : list[str] | None, optional
             公開するユーザー, by default None
         cw : str | None, optional
             閲覧注意の文字, by default None
         local_only : bool, optional
@@ -436,88 +544,40 @@
         )
         res: ICreatedNote = await self._session.request(
             Route('POST', '/api/notes/create'), json=body, auth=True, lower=True,
         )
         return Note(res['created_note'], client=self._client)
 
     @cache(group='get_note')
-    async def get(self, note_id: str | None = None) -> Note:
+    async def get(self, note_id: str) -> Note:
         """
         ノートを取得します
 
         Parameters
         ----------
-        note_id : str | None, default=None
+        note_id : str
             ノートのID
 
         Returns
         -------
         Note
             取得したノートID
         """
-        note_id = note_id or self._note_id
         res = await self._session.request(
             Route('POST', '/api/notes/show'), json={'noteId': note_id}, auth=True, lower=True,
         )
         return Note(res, client=self._client)
 
     @cache(group='get_note', override=True)
-    async def fetch(self, note_id: str | None = None) -> Note:
-        note_id = note_id or self._note_id
+    async def fetch(self, note_id: str) -> Note:
         res = await self._session.request(
             Route('POST', '/api/notes/show'), json={'noteId': note_id}, auth=True, lower=True,
         )
         return Note(res, client=self._client)
 
-    async def get_replies(
-        self,
-        since_id: str | None = None,
-        until_id: str | None = None,
-        limit: int = 10,
-        note_id: str | None = None,
-        get_all: bool = False,
-    ) -> AsyncGenerator[Note, None]:
-        """
-        ノートに対する返信を取得します
-
-        Parameters
-        ---------
-        since_id : str | None, default=None
-            指定すると、その投稿を投稿を起点としてより新しい投稿を取得します
-        until_id : str | None, default=None
-            指定すると、その投稿を投稿を起点としてより古い投稿を取得します
-        limit : int, default=10
-            取得する上限
-        note_id: str | None, default=None
-            返信を取得したいノートのID
-
-        Returns
-        -------
-        AsyncGenerator[Note, None]
-            返信
-        """
-
-        if limit > 100:
-            raise ParameterError('limitは100以下である必要があります')
-        if get_all:
-            limit = 100
-
-        note_id = note_id or self._note_id
-        body = {'noteId': note_id, 'sinceId': since_id, 'untilId': until_id, 'limit': limit}
-
-        pagination = Pagination[INote](self._session, Route('POST', '/api/notes'), json=body)
-
-        while True:
-            res_notes = await pagination.next()
-            for res_note in res_notes:
-                yield Note(res_note, client=self._client)
-
-            if get_all is False or pagination.is_final:
-                break
-
     async def gets(
         self,
         local: bool = False,
         reply: bool = False,
         renote: bool = False,
         with_files: bool = False,
         poll: bool = False,
```

### Comparing `mipac-0.4.99/mipac/actions/poll.py` & `mipac-0.5.0/mipac/actions/poll.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/reaction.py` & `mipac-0.5.0/mipac/actions/reaction.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/actions/user.py` & `mipac-0.5.0/mipac/actions/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, AsyncGenerator, Literal, Optional
 
 from mipac.config import config
 from mipac.errors.base import NotExistRequiredData, NotSupportVersion, ParameterError
 from mipac.http import HTTPClient, Route
+from mipac.models.clip import Clip
 from mipac.models.note import Note
 from mipac.models.user import Achievement, LiteUser, UserDetailed
+from mipac.types.clip import IClip
 from mipac.types.note import INote
 from mipac.utils.cache import cache
 from mipac.utils.format import remove_dict_empty
 from mipac.utils.pagination import Pagination
 from mipac.utils.util import check_multi_arg
 
 if TYPE_CHECKING:
@@ -116,15 +118,14 @@
         until_date: int = 0,
         include_my_renotes: bool = True,
         with_files: bool = False,
         file_type: Optional[list[str]] = None,
         exclude_nsfw: bool = True,
         get_all: bool = False,
     ) -> AsyncGenerator[Note, None]:
-
         if check_multi_arg(user_id, self.__user) is False:
             raise ParameterError('user_idがありません', user_id, self.__user)
 
         user_id = user_id or self.__user and self.__user.id
         data = {
             'userId': user_id,
             'includeReplies': include_replies,
@@ -222,15 +223,17 @@
         pagination = Pagination[UserDetailed | LiteUser](
             self.__session, Route('POST', '/api/users/search'), json=body, pagination_type='count'
         )
 
         while True:
             res_users = await pagination.next()
             for user in res_users:
-                yield UserDetailed(user, client=self.__client) if detail else LiteUser(user, client=self.__client)  # type: ignore
+                if detail:
+                    yield UserDetailed(user, client=self.__client)
+                yield LiteUser(user, client=self.__client)
             if get_all is False or pagination.is_final:
                 break
 
     async def search_by_username_and_host(
         self, username: str, host: str, limit: int = 100, detail: bool = True,
     ) -> list[UserDetailed | LiteUser]:
         """
@@ -269,15 +272,15 @@
             UserDetailed(user, client=self.__client)
             if detail
             else LiteUser(user, client=self.__client)
             for user in res
         ]
 
     async def get_achievements(self, user_id: str | None = None) -> list[Achievement]:
-        """ Get achievements of user. """
+        """Get achievements of user."""
 
         if config.use_version < 13:
             raise NotSupportVersion('ご利用のインスタンスのバージョンではサポートされていない機能です')
 
         user_id = user_id or self.__user and self.__user.id
 
         if not user_id:
@@ -286,7 +289,39 @@
         data = {
             'userId': user_id,
         }
         res = await self.__session.request(
             Route('POST', '/api/users/achievements'), json=data, auth=True, lower=True,
         )
         return [Achievement(i) for i in res]
+
+    async def get_clips(
+        self,
+        user_id: str | None = None,
+        limit: int = 10,
+        since_id: str | None = None,
+        until_id: str | None = None,
+        get_all: bool = False,
+    ):
+        user_id = user_id or self.__user and self.__user.id
+
+        if not user_id:
+            raise ParameterError('user_id is required')
+
+        if limit > 100:
+            raise ParameterError('limit must be less than 100')
+
+        if get_all:
+            limit = 100
+
+        body = {'userId': user_id, 'limit': limit, 'sinceId': since_id, 'untilId': until_id}
+
+        pagination = Pagination[IClip](
+            self.__session, Route('POST', '/api/users/clips'), json=body, auth=True
+        )
+
+        while True:
+            clips: list[IClip] = await pagination.next()
+            for clip in clips:
+                yield Clip(clip, client=self.__client)
+            if get_all is False or pagination.is_final:
+                break
```

### Comparing `mipac-0.4.99/mipac/client.py` & `mipac-0.5.0/mipac/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,37 @@
+from typing import Self
+
 from mipac.config import Config, IMisskeyVersions, config
 from mipac.http import HTTPClient
 from mipac.manager.client import ClientManager
 from mipac.utils.log import LOGING_LEVEL_TYPE, setup_logging
 
 
 class Client:
     def __init__(
         self,
         url: str,
         token: str | None = None,
         *,
-        log_level: LOGING_LEVEL_TYPE = 'INFO',
+        log_level: LOGING_LEVEL_TYPE | None = 'INFO',
         use_version: IMisskeyVersions = 12,
         use_version_autodetect: bool = True
     ) -> None:
-        setup_logging(level=log_level)
-        self.__url: str = url
-        self.__token: str | None = token
+        if log_level is not None:
+            setup_logging(level=log_level)
         config.from_dict(use_version=use_version, use_version_autodetect=use_version_autodetect)
         self.config: Config = config
         self.http: HTTPClient = HTTPClient(url, token)
 
+    async def __aenter__(self) -> Self:
+        await self.http.login()
+        return self
+
+    async def __aexit__(self, exc_type, exc, tb) -> None:
+        await self.close_session()
+
     @property
     def api(self) -> ClientManager:
         return ClientManager(self.http, self.config)
 
     async def close_session(self) -> None:
         await self.http.close_session()
```

### Comparing `mipac-0.4.99/mipac/config.py` & `mipac-0.5.0/mipac/config.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/errors/base.py` & `mipac-0.5.0/mipac/errors/base.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/errors/errors.py` & `mipac-0.5.0/mipac/errors/errors.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/file.py` & `mipac-0.5.0/mipac/file.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/http.py` & `mipac-0.5.0/mipac/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import json
 import logging
 import re
 import sys
 from typing import Any, Literal, TypeVar
 
 import aiohttp
-
-from mipac import __version__
 from mipac.config import config
 from mipac.errors.base import APIError
 from mipac.types.endpoints import ENDPOINTS
 from mipac.types.meta import IMeta
 from mipac.types.user import IUserDetailed
 from mipac.utils.format import remove_dict_empty, upper_to_lower
 from mipac.utils.util import COLORS, _from_json
 
+from mipac import __version__
+
 _log = logging.getLogger(__name__)
 
 
 class _MissingSentinel:
     def __eq__(self, other):
         return False
 
@@ -124,15 +124,15 @@
     async def close_session(self) -> None:
         await self._session.close()
 
     async def login(self) -> IUserDetailed | None:
         match_domain = re.search(r'https?:\/\/([^\/]+)', self._url)
         match_protocol = re.search(r'^(http|https)', self._url)
         if match_domain is None or match_protocol is None:
-            raise Exception()
+            raise Exception('Server URL cannot be retrieved or protocol (http / https) is missing')
         protocol = True if match_protocol.group(1) == 'https' else False
         config.from_dict(
             host=match_domain.group(1), is_ssl=protocol,
         )
         self._session = aiohttp.ClientSession(ws_response_class=MisskeyClientWebSocketResponse)
         if self._token:
             data: IUserDetailed = await self.request(Route('POST', '/api/i'), auth=True)
```

### Comparing `mipac-0.4.99/mipac/manager/admins/ad.py` & `mipac-0.5.0/mipac/manager/admins/ad.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/admins/admin.py` & `mipac-0.5.0/mipac/manager/admins/admin.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/admins/announcement.py` & `mipac-0.5.0/mipac/manager/admins/announcement.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/admins/emoji.py` & `mipac-0.5.0/mipac/manager/admins/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/admins/moderator.py` & `mipac-0.5.0/mipac/manager/admins/moderator.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/admins/roles.py` & `mipac-0.5.0/mipac/manager/admins/roles.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/admins/user.py` & `mipac-0.5.0/mipac/manager/admins/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/antenna.py` & `mipac-0.5.0/mipac/manager/antenna.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 from mipac.abstract.manager import AbstractManager
-from mipac.http import HTTPClient
 from mipac.actions.antenna import AntennaActions, ClientAntennaActions
+from mipac.http import HTTPClient
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
 
 class ClientAntennaManager(AbstractManager):
     def __init__(self, *, antenna_id: str, session: HTTPClient, client: ClientManager):
```

### Comparing `mipac-0.4.99/mipac/manager/blocking.py` & `mipac-0.5.0/mipac/manager/blocking.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/channel.py` & `mipac-0.5.0/mipac/manager/channel.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/chart.py` & `mipac-0.5.0/mipac/manager/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/chat.py` & `mipac-0.5.0/mipac/manager/chat.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/client.py` & `mipac-0.5.0/mipac/manager/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from mipac.actions.client import ClientActions
 from mipac.http import HTTPClient
 from mipac.manager.admins.admin import AdminManager
 from mipac.manager.antenna import AntennaManager
 from mipac.manager.channel import ChannelManager
 from mipac.manager.chart import ChartManager
 from mipac.manager.chat import ChatManager
+from mipac.manager.clip import ClipManager
 from mipac.manager.drive import DriveManager
 from mipac.manager.emoji import EmojiManager
 from mipac.manager.follow import FollowManager, FollowRequestManager
 from mipac.manager.my import MyManager
 from mipac.manager.note import NoteManager
 from mipac.manager.user import UserManager
 
@@ -38,14 +39,15 @@
         self.channel: ChannelManager = ChannelManager(session=session, client=self)
         self.follow: FollowManager = FollowManager(
             session=session, client=self,
         )
         self.follow_request: FollowRequestManager = FollowRequestManager(
             session=session, client=self,
         )
+        self.clip: ClipManager = ClipManager(session=session, client=self)
         self.emoji: EmojiManager = EmojiManager(session=session, client=self)
         self.antenna: AntennaManager = AntennaManager(session=session, client=self)
         self._config: Config = config
 
     @property
     def action(self) -> ClientActions:
         return ClientActions(session=self.__session, client=self)
```

### Comparing `mipac-0.4.99/mipac/manager/drive.py` & `mipac-0.5.0/mipac/manager/drive.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,60 +19,66 @@
 
 
 class ClientFileManager(AbstractManager):
     def __init__(
         self,
         file_id: str | None = None,
         folder_id: str | None = None,
+        url: str | None = None,
         *,
         session: HTTPClient,
         client: ClientManager
     ):
         self.__session: HTTPClient = session
         self.__client: ClientManager = client
         self.__file_id: str | None = file_id
         self.__folder_id: str | None = folder_id
+        self.__url: str | None = url
 
     @property
     def action(self) -> ClientFileActions:
         return ClientFileActions(
             file_id=self.__file_id,
             folder_id=self.__folder_id,
+            url=self.__url,
             client=self.__client,
             session=self.__session,
         )
 
 
 class FileManager(AbstractManager):
     def __init__(
         self,
         file_id: str | None = None,
         folder_id: str | None = None,
+        url: str | None = None,
         *,
         session: HTTPClient,
         client: ClientManager
     ):
         self.__session: HTTPClient = session
         self.__client: ClientManager = client
         self.__file_id = file_id
         self.__folder_id: str | None = folder_id
+        self.__url: str | None = url
 
     @property
     def action(self) -> FileActions:
         """
         ファイルの操作を行うインスタンスを返します
 
         Return
         ------
         FileActions
             ファイルに対するアクション
         """
         return FileActions(
             file_id=self.__file_id,
             folder_id=self.__folder_id,
+            url=self.__url,
             client=self.__client,
             session=self.__session,
         )
 
 
 class ClientFolderManager(AbstractManager):
     def __init__(
@@ -154,12 +160,16 @@
 
     def _get_client_folder_instance(self, folder_id: str) -> ClientFolderManager:
         return ClientFolderManager(
             folder_id=folder_id, session=self.__session, client=self.__client
         )
 
     def _get_client_file_instance(
-        self, file_id: str, folder_id: str | None = None
+        self, *, file_id: str, url: str, folder_id: str | None = None
     ) -> ClientFileManager:
         return ClientFileManager(
-            file_id=file_id, folder_id=folder_id, session=self.__session, client=self.__client
+            file_id=file_id,
+            folder_id=folder_id,
+            url=url,
+            session=self.__session,
+            client=self.__client,
         )
```

### Comparing `mipac-0.4.99/mipac/manager/emoji.py` & `mipac-0.5.0/mipac/manager/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/favorite.py` & `mipac-0.5.0/mipac/manager/favorite.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/federation.py` & `mipac-0.5.0/mipac/manager/federation.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/follow.py` & `mipac-0.5.0/mipac/manager/follow.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/mute.py` & `mipac-0.5.0/mipac/manager/mute.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/my.py` & `mipac-0.5.0/mipac/manager/my.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/note.py` & `mipac-0.5.0/mipac/manager/note.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from mipac.abstract.manager import AbstractManager
 from mipac.actions.note import ClientNoteActions, NoteActions
-from mipac.http import HTTPClient, Route
+from mipac.http import HTTPClient
 from mipac.manager.favorite import FavoriteManager
 from mipac.manager.poll import PollManager
 from mipac.manager.reaction import ReactionManager
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
```

### Comparing `mipac-0.4.99/mipac/manager/page.py` & `mipac-0.5.0/mipac/manager/page.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/poll.py` & `mipac-0.5.0/mipac/manager/poll.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/reaction.py` & `mipac-0.5.0/mipac/manager/reaction.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/manager/user.py` & `mipac-0.5.0/mipac/manager/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 class UserManager(AbstractManager):
     def __init__(
         self, user: LiteUser | None = None, *, session: HTTPClient, client: ClientManager
     ):
         user_id: str | None = user.id if user else None
         self.__session: HTTPClient = session
         self.__client: ClientManager = client
-        self.user: LiteUser | None = user
+        self.__user: LiteUser | None = user
         self.follow: FollowManager = FollowManager(user_id=user_id, session=session, client=client)
         self.mute: MuteManager = MuteManager(user_id=user_id, session=session, client=client)
         self.block = BlockingManager(user_id=user_id, session=session, client=client)
 
     @property
     def action(self) -> UserActions:
         """ユーザーに対するアクション
 
         Returns
         -------
         UserActions
             ユーザーに対するアクションを行うクラス
         """
-        return UserActions(session=self.__session, client=self.__client, user=self.user)
+        return UserActions(session=self.__session, client=self.__client, user=self.__user)
```

### Comparing `mipac-0.4.99/mipac/models/ad.py` & `mipac-0.5.0/mipac/models/ad.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,7 +55,13 @@
     @property
     def memo(self) -> str | None:
         return self.__ad_data['memo']
 
     @property
     def api(self) -> AdminAdvertisingModelManager:
         return self.__client.admin.create_ad_model_manager(ad_id=self.id)
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, Ad) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/admin.py` & `mipac-0.5.0/mipac/models/admin.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,20 @@
     def ip(self) -> str:
         return self.__user_ip['ip']
 
     @property
     def created_at(self) -> datetime:
         return str_to_datetime(self.__user_ip['created_at'])
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, UserIP) and self.ip == __value.ip
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
+
 
 class IndexStat:
     def __init__(self, index_stat: IIndexStat) -> None:
         self.__index_stat: IIndexStat = index_stat
 
     @property
     def schemaname(self) -> str:
@@ -83,14 +89,20 @@
     def user_id(self) -> str:
         return self.__moderation_log['user_id']
 
     @property
     def user(self) -> UserDetailed:
         return UserDetailed(self.__moderation_log['user'], client=self.__client)
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, ModerationLog) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
+
 
 class ServerInfoCpu:
     def __init__(self, server_info_cpu: IServerInfoCpu) -> None:
         self.__server_info_cpu = server_info_cpu
 
     @property
     def models(self) -> str:
```

### Comparing `mipac-0.4.99/mipac/models/announcement.py` & `mipac-0.5.0/mipac/models/announcement.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,20 @@
 
     @property
     def action(self) -> AdminAnnouncementClientActions:
         return self.__client.admin.announcement._create_client_announcement_instance(
             announce_id=self.id
         )
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, Announcement) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
+
 
 class Announcement(AnnouncementCommon):
     def __init__(self, announcement: IAnnouncement, *, client: ClientManager) -> None:
         super().__init__(announcement, client=client)
         self.__announcement: IAnnouncement
 
     @property
```

### Comparing `mipac-0.4.99/mipac/models/antenna.py` & `mipac-0.5.0/mipac/models/antenna.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
-from datetime import datetime
 
+from datetime import datetime
 from typing import TYPE_CHECKING
+
 from mipac.types.antenna import IAntenna, IAntennaReceiveSource
 from mipac.utils.format import str_to_datetime
 
-
 if TYPE_CHECKING:
-    from mipac.manager.client import ClientManager
     from mipac.manager.antenna import ClientAntennaManager
+    from mipac.manager.client import ClientManager
 
 
 class Antenna:
     def __init__(self, antenna: IAntenna, *, client: ClientManager) -> None:
         self.__antenna: IAntenna = antenna
         self.__client: ClientManager = client
 
@@ -71,7 +71,13 @@
     @property
     def with_replies(self) -> bool:
         return self.__antenna['with_replies']
 
     @property
     def api(self) -> ClientAntennaManager:
         return self.__client.antenna._create_client_antenna_manager(antenna_id=self.id)
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, Antenna) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/channel.py` & `mipac-0.5.0/mipac/models/channel.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/models/chart.py` & `mipac-0.5.0/mipac/models/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/models/chat.py` & `mipac-0.5.0/mipac/models/chat.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,14 +38,20 @@
         """グループのオーナーのID"""
         return self.__group['owner_id']
 
     @property
     def user_ids(self) -> list[str]:
         return self.__group['user_ids']
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, ChatGroup) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
+
 
 class ChatMessage:
     """
     チャットオブジェクト
     """
 
     def __init__(self, chat: IChatMessage, *, client: ClientManager):
@@ -116,7 +122,13 @@
             if self.__chat.get('group')
             else None
         )
 
     @property
     def api(self) -> BaseChatAction:
         return self.__client.chat.custom_base_chat_action(user_id=self.user.id, message_id=self.id)
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, ChatMessage) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/drive.py` & `mipac-0.5.0/mipac/models/drive.py`

 * *Files 12% similar despite different names*

```diff
@@ -65,14 +65,20 @@
     def parent(self) -> dict[str, Any]:
         return self.__folder['parent']
 
     @property
     def api(self) -> ClientFolderManager:
         return self.__client.drive._get_client_folder_instance(folder_id=self.id)
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, Folder) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
+
 
 class File:
     def __init__(self, file: IDriveFile, *, client: ClientManager):
         self.__file: IDriveFile = file
         self.__client: ClientManager = client
 
     @property
@@ -117,8 +123,14 @@
 
     @property
     def properties(self) -> FileProperties:
         return FileProperties(self.__file['properties'])
 
     @property
     def api(self) -> ClientFileManager:
-        return self.__client.drive._get_client_file_instance(file_id=self.id)
+        return self.__client.drive._get_client_file_instance(file_id=self.id, url=self.url)
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, File) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/emoji.py` & `mipac-0.5.0/mipac/models/emoji.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,7 +31,13 @@
     @property
     def license(self) -> str | None:
         return self.__emoji['license']
 
     @property
     def host(self) -> str | None:
         return self.__emoji['host']
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, CustomEmoji) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/follow.py` & `mipac-0.5.0/mipac/models/follow.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,7 +26,13 @@
     @property
     def followee(self) -> LiteUser:
         return LiteUser(self.__follow_request['followee'], client=self.__client)
 
     @property
     def api(self) -> FollowRequestManager:
         return self.__client._create_user_instance(user=self.follower).follow.request
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, FollowRequest) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/instance.py` & `mipac-0.5.0/mipac/models/instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,7 +104,13 @@
     @property
     def latest_request_sent_at(self) -> str | None:
         return self.__instance.get('latest_request_sent_at')
 
     @property
     def last_communicated_at(self) -> str | None:
         return self.__instance.get('last_communicated_at')
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, FederationInstance) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/lite/channel.py` & `mipac-0.5.0/mipac/models/lite/channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,7 +59,13 @@
     @property
     def pinned_note_ids(self) -> list:
         return self._channel.get('pinned_note_ids', [])
 
     @property
     def api(self) -> ChannelManager:
         return self.__client._create_channel_instance(channel_id=self.id)
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, ChannelLite) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/lite/emoji.py` & `mipac-0.5.0/mipac/models/lite/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/models/lite/instance.py` & `mipac-0.5.0/mipac/models/lite/instance.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/models/lite/meta.py` & `mipac-0.5.0/mipac/models/lite/meta.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/models/lite/note.py` & `mipac-0.5.0/mipac/models/lite/note.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from datetime import datetime
-from typing import TYPE_CHECKING, Generic, Literal, TypeVar
+from typing import TYPE_CHECKING, Generic, TypeVar
 
+from mipac.models.drive import File
 from mipac.models.lite.user import LiteUser
-from mipac.types.drive import IDriveFile
-from mipac.types.note import IPartialNote
+from mipac.types.note import INoteVisibility, IPartialNote
+from mipac.types.reaction import IReactionAcceptance
 from mipac.utils.format import str_to_datetime
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
     from mipac.manager.note import ClientNoteManager
 
 
@@ -30,36 +31,36 @@
         return self._note.get('cw')
 
     @property
     def file_ids(self) -> list[str]:
         return self._note['file_ids']
 
     @property
-    def files(self) -> list[IDriveFile]:  # TODO: モデルに
-        return self._note['files']
+    def files(self) -> list[File]:
+        return [File(file, client=self._client) for file in self._note['files']]
 
     @property
     def id(self) -> str:
         """
         ノートのID
 
         Returns
         -------
         str
             ユーザーのID
         """
         return self._note['id']
 
     @property
-    def reaction_acceptance(self) -> Literal['likeOnly', 'likeOnlyForRemote'] | None:
+    def reaction_acceptance(self) -> IReactionAcceptance | None:
         """リアクションを受け入れ
 
         Returns
         -------
-        Literal['likeOnly', 'likeOnlyForRemote'] | None
+        IReactionAcceptance | None
         """
         return self._note.get('reaction_acceptance')
 
     @property
     def reaction_emojis(self) -> dict[str, str] | None:
         """リアクション一覧です
 
@@ -103,20 +104,26 @@
         return LiteUser(self._note['user'], client=self._client)
 
     @property
     def user_id(self) -> str:
         return self._note['user_id']
 
     @property
-    def visibility(self,) -> Literal['public', 'home', 'followers', 'specified']:
+    def visibility(self,) -> INoteVisibility:
         return self._note['visibility']
 
     @property
     def api(self) -> ClientNoteManager:
         """
         ノートに対するアクション
 
         Returns
         -------
         NoteActions
         """
         return self._client.note.create_client_note_manager(self.id)
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, PartialNote) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/lite/user.py` & `mipac-0.5.0/mipac/models/lite/user.py`

 * *Files 8% similar despite different names*

```diff
@@ -78,7 +78,13 @@
     @property
     def instance(self) -> LiteInstance | None:
         return LiteInstance(self.__user['instance']) if 'instance' in self.__user else None
 
     @property
     def api(self) -> UserManager:
         return self.__client._create_user_instance(self)
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, LiteUser) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/meta.py` & `mipac-0.5.0/mipac/models/meta.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/models/mute.py` & `mipac-0.5.0/mipac/models/mute.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,7 +25,13 @@
     @property
     def mutee_id(self) -> str:
         return self.__data['mutee_id']
 
     @property
     def mutee(self) -> UserDetailed:
         return UserDetailed(self.__data['mutee'], client=self.__client)
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, IMuteUser) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/note.py` & `mipac-0.5.0/mipac/models/note.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,22 @@
     def note_id(self) -> str:
         return self.__data['body']['id']
 
     @property
     def deleted_at(self) -> datetime:
         return str_to_datetime(self.__data['body']['body']['deleted_at'])
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, NoteDeleted) and self.note_id == __value.note_id
 
-class Follow:
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
+
+
+class Follow:  # TODO: 消す
     def __init__(self, data):
         self.id: str | None = data.get('id')
         self.created_at: Optional[datetime] = datetime.strptime(
             data['created_at'], '%Y-%m-%dT%H:%M:%S.%fZ'
         ) if data.get('created_at') else None
         self.type: str | None = data.get('type')
         self.user: Optional[UserDetailed] = data.get('user')
@@ -136,14 +142,20 @@
     def type(self) -> str | None:
         return self.__reaction['type']
 
     @property
     def user(self) -> LiteUser:
         return LiteUser(self.__reaction['user'], client=self.__client)
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, NoteReaction) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
+
 
 class Note(PartialNote[INote]):
     """
     Noteモデル
 
     Parameters
     ----------
```

### Comparing `mipac-0.4.99/mipac/models/notification.py` & `mipac-0.5.0/mipac/models/notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,20 @@
     def created_at(self) -> datetime:
         return datetime.strptime(self.__notification['created_at'], '%Y-%m-%dT%H:%M:%S.%fZ')
 
     @property
     def is_read(self) -> bool:
         return self.__notification['is_read']
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, Notification) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
+
 
 class NotificationFollow(Notification):
     def __init__(self, notification: IUserNf, *, client: ClientManager,) -> None:
         super().__init__(notification, client=client)
         self.__notification: IUserNf = notification
         self.__client: ClientManager = client
```

### Comparing `mipac-0.4.99/mipac/models/poll.py` & `mipac-0.5.0/mipac/models/poll.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/models/reaction.py` & `mipac-0.5.0/mipac/models/reaction.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/models/roles.py` & `mipac-0.5.0/mipac/models/roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,20 @@
             else None
         )
 
     @property
     def action(self) -> UserManager:
         return self.__client._create_user_instance(self.user)
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, RoleUser) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
+
 
 class RolePolicyValue:
     def __init__(self, policiy_value_data: IRolePolicieValue) -> None:
         self.__policy_value_data = policiy_value_data
 
     @property
     def value(self) -> int:
@@ -193,7 +199,13 @@
     @property
     def users_count(self) -> int:
         return self.__role_data.get('users_count')
 
     @property
     def api(self) -> AdminRolesModelManager:
         return self.__client.admin.create_roles_model_manager(self.id)
+
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, Role) and self.id == __value.id
+
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
```

### Comparing `mipac-0.4.99/mipac/models/user.py` & `mipac-0.5.0/mipac/models/user.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,21 @@
 
 from datetime import datetime
 from typing import TYPE_CHECKING, Literal
 
 from mipac.models.lite.user import LiteUser
 from mipac.models.note import Note
 from mipac.types.page import IPage
-from mipac.types.user import (
-    IAchievement,
-    IBlockingUser,
-    IFollowRequest,
-    IUserDetailed,
-    IUserDetailedField,
-)
+from mipac.types.user import IAchievement, IBlockingUser, IUserDetailed, IUserDetailedField
 from mipac.utils.format import str_to_datetime
 
 if TYPE_CHECKING:
     from mipac.manager.client import ClientManager
 
-__all__ = ('UserDetailed', 'FollowRequest', 'LiteUser', 'Achievement', 'BlockingUser')
+__all__ = ('UserDetailed', 'LiteUser', 'Achievement', 'BlockingUser')
 
 
 class BlockingUser:
     def __init__(self, blocking_user_data: IBlockingUser, *, client: ClientManager) -> None:
         self.__blocking_user_data: IBlockingUser = blocking_user_data
         self.__client: ClientManager = client
 
@@ -38,31 +32,19 @@
     def blockee_id(self) -> str:
         return self.__blocking_user_data['blockee_id']
 
     @property
     def blockee(self) -> UserDetailed:
         return UserDetailed(self.__blocking_user_data['blockee'], client=self.__client)
 
+    def __eq__(self, __value: object) -> bool:
+        return isinstance(__value, BlockingUser) and self.id == __value.id
 
-class FollowRequest:
-    def __init__(self, request: IFollowRequest, *, client: ClientManager):
-        self.__request: IFollowRequest = request
-        self.__client: ClientManager = client
-
-    @property
-    def id(self) -> str:
-        return self.__request['id']
-
-    @property
-    def follower(self) -> LiteUser:
-        return LiteUser(self.__request['follower'], client=self.__client)
-
-    @property
-    def followee(self) -> LiteUser:
-        return LiteUser(self.__request['followee'], client=self.__client)
+    def __ne__(self, __value: object) -> bool:
+        return not self.__eq__(__value)
 
 
 class Achievement:
     def __init__(self, detail: IAchievement):
         self.__detail: IAchievement = detail
 
     @property
```

### Comparing `mipac-0.4.99/mipac/types/achievement.py` & `mipac-0.5.0/mipac/types/achievement.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/admin.py` & `mipac-0.5.0/mipac/types/admin.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/channel.py` & `mipac-0.5.0/mipac/types/channel.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/chart.py` & `mipac-0.5.0/mipac/types/chart.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/chat.py` & `mipac-0.5.0/mipac/types/chat.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/drive.py` & `mipac-0.5.0/mipac/types/drive.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/emoji.py` & `mipac-0.5.0/mipac/types/emoji.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/endpoints.py` & `mipac-0.5.0/mipac/types/endpoints.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/instance.py` & `mipac-0.5.0/mipac/types/instance.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/meta.py` & `mipac-0.5.0/mipac/types/meta.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/note.py` & `mipac-0.5.0/mipac/types/note.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import Any, Generic, Literal, NotRequired, Optional, TypedDict, TypeVar
 
-from .drive import IDriveFile
-from .emoji import ICustomEmojiLite
-from .poll import IPoll
-from .user import ILiteUser
+from mipac.types.drive import IDriveFile
+from mipac.types.emoji import ICustomEmojiLite
+from mipac.types.poll import IPoll
+from mipac.types.reaction import IReactionAcceptance
+from mipac.types.user import ILiteUser
 
 T = TypeVar('T')
 
+INoteVisibility = Literal['public', 'home', 'followers', 'specified']
+
 
 class INoteState(TypedDict):
     is_favorited: bool
     is_watching: bool
     is_muted_thread: NotRequired[bool]
 
 
@@ -56,25 +59,25 @@
 
 class IPartialNote(TypedDict):
     created_at: str
     cw: str | None
     file_ids: list[str]
     files: list[IDriveFile]
     id: str
-    reaction_acceptance: NotRequired[Literal['likeOnly', 'likeOnlyForRemote']]  # v13 only
+    reaction_acceptance: NotRequired[IReactionAcceptance]  # v13 only
     reaction_emojis: NotRequired[dict[str, str]]  # v13 only
     renote_id: str | None
     renote_count: int
     reactions: dict[str, int]
     replies_count: int
     reply_id: str | None
     text: str | None
     user: ILiteUser
     user_id: str
-    visibility: Literal['public', 'home', 'followers', 'specified']
+    visibility: INoteVisibility
     tags: NotRequired[list[str]]  # タグがついてないとbodyに存在しない
 
 
 class INote(IPartialNote, total=False):
     """
     note object
     """
```

### Comparing `mipac-0.4.99/mipac/types/notification.py` & `mipac-0.5.0/mipac/types/notification.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/page.py` & `mipac-0.5.0/mipac/types/page.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/roles.py` & `mipac-0.5.0/mipac/types/roles.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/types/user.py` & `mipac-0.5.0/mipac/types/user.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/util.py` & `mipac-0.5.0/mipac/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import uuid
 import warnings
 from datetime import datetime, timedelta
 from typing import Any, Mapping, Optional
 from urllib.parse import urlencode
 
 import aiohttp
-
 from mipac.utils.util import deprecated as new_deprecated
 
 try:
     import orjson  # type: ignore
 except ModuleNotFoundError:
     HAS_ORJSON = False
 else:
```

### Comparing `mipac-0.4.99/mipac/utils/auth.py` & `mipac-0.5.0/mipac/utils/auth.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/utils/cache.py` & `mipac-0.5.0/mipac/utils/cache.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/utils/format.py` & `mipac-0.5.0/mipac/utils/format.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/utils/log.py` & `mipac-0.5.0/mipac/utils/log.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac/utils/pagination.py` & `mipac-0.5.0/mipac/utils/pagination.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
             auth=self.auth,
             remove_none=self.remove_none,
             lower=self.lower,
             json=self.json,
         )
         if self.pagination_type == 'until':
             self.previous_id = self.json.get('untilId', '')  # 前のIDを保存しておく
-            self.next_id = res[-1]['id']  # type: ignore
+            if len(res) > 0:
+                self.next_id = res[-1]['id']  # type: ignore
             self.json['untilId'] = self.next_id
         self.latest_res_count = len(res)
         return res
 
     @property
     def is_final(self) -> bool:
         if (
```

### Comparing `mipac-0.4.99/mipac/utils/util.py` & `mipac-0.5.0/mipac/utils/util.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/mipac.egg-info/PKG-INFO` & `mipac-0.5.0/mipac.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mipac
-Version: 0.4.99
+Version: 0.5.0
 Summary: A Python wrapper for the Misskey API
 Home-page: https://github.com/yupix/mipac
 Author: yupix
 Author-email: yupi0982@outlook.jp
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
@@ -57,47 +57,32 @@
     note = await api.note.action.send('Hello World')
     print(note.author.name, note.content)
 
 if __name__ == '__main__':
     asyncio.run(main())
 ```
 
-### Migration from v0.3.0 to v0.4.0
-
-#### configの属性が変更されました
-
-- `is_official` が削除されました
-
-##### **重要** `use_version` が追加されました
-
-Misskeyではv11,v12,v13とバージョンがあり、バージョンによっては使用できないAPIがあったりします。MiPACでは`use_version`を指定することで事前に使用できるかどうかを確認し、使用できない場合は`NotSupportVersion`という例外を返します。このようにご自分のインスタンスのバージョンを書いていただくだけで、よくわからないエラーを事前に防ぐことが出来ます。（issue等にエラーを報告場合は必ず適切に設定されているか確認してください）
-
-v13はまだリリースされて日が浅く、全てのインスタンスがアップデートしたとは考えにくいため、現在のデフォルト値は`12`となっています。
+### 注意事項
 
-#### `Client` のオプションから `config`が削除されました
+### Python3.12.0 final がリリースされ、3カ月経過後に最低バージョンを 3.12.0 に変更します
 
-今後configを参照する際は `Client.config` を使用してください。
-また、値を更新する場合はClient.config.from_dict()を用いることをお勧めします。
-通常の変更方法との違いは以下の通りです。
+これは主にMiPACの開発を行う上で、新規構文の使用などによってDXがより良くなり開発ペースが向上する為です。
+また、使用者の皆様においてはPythonの高速化や新規構文の使用などが使用できるといった恩恵を得ることができます。
 
-```python
-Client.config.is_ayuskey = True
-Client.config.use_version = 13
-Client.config.from_dict(is_ayuskey=True, use_version=13)
-```
+現在Python3.12.0のリリースは以下のように記載されているため、早くて **2024年01月02日** に変更を実施する予定です。
 
-上記のように複数の値を同時に更新する場合特に`from_dict`は有効な方法になります。
+ > `3.12.0 final: Monday, 2023-10-02`
 
-### 注意事項
+ これについて意見がある場合はDiscussionを作成することができます。
 
 ### 一部サーバー(インスタンス)のバージョンによっては正常に動作しない可能性があります
 
 MiPACの特徴として、v11,v12,v13のバージョンごとに生じる変更点をなるべく気にしなくてよいように作成していますが、現状の最新版であるv13でもv13の中で削除されたり、増えたりした物があります。結果的に追従しきれていない箇所があることがあります。そのため、そのような物を見つけた場合は、使用しているサーバーのバージョンと使用できないエンドポイント名をIssueに送信してください。
 
-### モデルを基本的に自分でインスタンス化することは推奨しません
+### モデルを自分でインスタンス化することは推奨されません
 
 MiPACのモデルでは多くの場合、キーワード引数に `client`を受け取り、それを用いて`api` プロパティを生成します。しかし、サポート途中の機能なのではそこが省かれ、リリース後にモデルのインスタンス化に必要な引数として `client` が追加されることがあります。また、他にもモデルの更新のために引数が変更される可能性があります。そのため、引数の変更に関することをCHANGELOG等で通知することはありません。
 
 ### 開発者向け情報
 
 このプロジェクトでは [black](https://github.com/psf/black)のforkである、[axblack](https://github.com/axiros/axblack)を利用しています。主な違いはダブルクォートがデフォルトではなく、シングルクォートになっている点です
```

### Comparing `mipac-0.4.99/mipac.egg-info/SOURCES.txt` & `mipac-0.5.0/mipac.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 mipac/actions/__init__.py
 mipac/actions/antenna.py
 mipac/actions/blocking.py
 mipac/actions/channel.py
 mipac/actions/chart.py
 mipac/actions/chat.py
 mipac/actions/client.py
+mipac/actions/clip.py
 mipac/actions/drive.py
 mipac/actions/emoji.py
 mipac/actions/favorite.py
 mipac/actions/federation.py
 mipac/actions/follow.py
 mipac/actions/mute.py
 mipac/actions/my.py
@@ -54,14 +55,15 @@
 mipac/manager/__init__.py
 mipac/manager/antenna.py
 mipac/manager/blocking.py
 mipac/manager/channel.py
 mipac/manager/chart.py
 mipac/manager/chat.py
 mipac/manager/client.py
+mipac/manager/clip.py
 mipac/manager/drive.py
 mipac/manager/emoji.py
 mipac/manager/favorite.py
 mipac/manager/federation.py
 mipac/manager/follow.py
 mipac/manager/mute.py
 mipac/manager/my.py
@@ -82,14 +84,15 @@
 mipac/models/ad.py
 mipac/models/admin.py
 mipac/models/announcement.py
 mipac/models/antenna.py
 mipac/models/channel.py
 mipac/models/chart.py
 mipac/models/chat.py
+mipac/models/clip.py
 mipac/models/drive.py
 mipac/models/emoji.py
 mipac/models/follow.py
 mipac/models/instance.py
 mipac/models/meta.py
 mipac/models/mute.py
 mipac/models/note.py
@@ -110,14 +113,15 @@
 mipac/types/admin.py
 mipac/types/ads.py
 mipac/types/announcement.py
 mipac/types/antenna.py
 mipac/types/channel.py
 mipac/types/chart.py
 mipac/types/chat.py
+mipac/types/clip.py
 mipac/types/drive.py
 mipac/types/emoji.py
 mipac/types/endpoints.py
 mipac/types/follow.py
 mipac/types/instance.py
 mipac/types/meta.py
 mipac/types/mute.py
```

### Comparing `mipac-0.4.99/setup.py` & `mipac-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `mipac-0.4.99/versioneer.py` & `mipac-0.5.0/versioneer.py`

 * *Files identical despite different names*

