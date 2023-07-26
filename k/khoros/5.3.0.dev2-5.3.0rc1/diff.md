# Comparing `tmp/khoros-5.3.0.dev2.tar.gz` & `tmp/khoros-5.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khoros-5.3.0.dev2.tar", last modified: Fri Jul  7 19:37:54 2023, max compression
+gzip compressed data, was "khoros-5.3.0rc1.tar", last modified: Wed Jul 26 20:46:34 2023, max compression
```

## Comparing `khoros-5.3.0.dev2.tar` & `khoros-5.3.0rc1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.508592 khoros-5.3.0.dev2/
--rw-r--r--   0 shurtj     (501) staff       (20)     1071 2020-05-20 04:19:02.000000 khoros-5.3.0.dev2/LICENSE
--rw-r--r--   0 shurtj     (501) staff       (20)    17352 2023-07-07 19:37:54.508036 khoros-5.3.0.dev2/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)    15696 2023-01-02 17:40:43.000000 khoros-5.3.0.dev2/README.md
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.450049 khoros-5.3.0.dev2/khoros/
--rw-r--r--   0 shurtj     (501) staff       (20)      799 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    73826 2023-06-14 20:24:00.000000 khoros-5.3.0.dev2/khoros/api.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11891 2023-06-14 19:57:43.000000 khoros-5.3.0.dev2/khoros/auth.py
--rw-r--r--   0 shurtj     (501) staff       (20)    14989 2023-06-14 19:56:42.000000 khoros-5.3.0.dev2/khoros/bulk_data.py
--rw-r--r--   0 shurtj     (501) staff       (20)   279262 2023-07-06 21:23:27.000000 khoros-5.3.0.dev2/khoros/core.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.455194 khoros-5.3.0.dev2/khoros/errors/
--rw-r--r--   0 shurtj     (501) staff       (20)      597 2020-07-07 04:29:45.000000 khoros-5.3.0.dev2/khoros/errors/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    30504 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/errors/exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11117 2023-06-14 20:26:29.000000 khoros-5.3.0.dev2/khoros/errors/handlers.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2631 2020-12-26 17:57:00.000000 khoros-5.3.0.dev2/khoros/errors/translations.py
--rw-r--r--   0 shurtj     (501) staff       (20)    23051 2023-06-06 21:11:32.000000 khoros-5.3.0.dev2/khoros/liql.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.465203 khoros-5.3.0.dev2/khoros/objects/
--rw-r--r--   0 shurtj     (501) staff       (20)      856 2021-10-11 04:30:21.000000 khoros-5.3.0.dev2/khoros/objects/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5999 2020-10-30 02:28:27.000000 khoros-5.3.0.dev2/khoros/objects/albums.py
--rw-r--r--   0 shurtj     (501) staff       (20)    15595 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/objects/archives.py
--rw-r--r--   0 shurtj     (501) staff       (20)     6697 2020-10-30 02:28:27.000000 khoros-5.3.0.dev2/khoros/objects/attachments.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3290 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/objects/base.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1508 2023-07-06 21:05:48.000000 khoros-5.3.0.dev2/khoros/objects/labels.py
--rw-r--r--   0 shurtj     (501) staff       (20)    60447 2022-09-28 20:40:19.000000 khoros-5.3.0.dev2/khoros/objects/messages.py
--rw-r--r--   0 shurtj     (501) staff       (20)    23431 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/objects/roles.py
--rw-r--r--   0 shurtj     (501) staff       (20)    10387 2022-10-28 20:28:53.000000 khoros-5.3.0.dev2/khoros/objects/settings.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12899 2021-05-20 22:43:31.000000 khoros-5.3.0.dev2/khoros/objects/subscriptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)     8692 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/objects/tags.py
--rw-r--r--   0 shurtj     (501) staff       (20)    61692 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/objects/users.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4106 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/saml.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.473961 khoros-5.3.0.dev2/khoros/structures/
--rw-r--r--   0 shurtj     (501) staff       (20)      566 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/structures/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    20187 2022-09-29 22:14:22.000000 khoros-5.3.0.dev2/khoros/structures/base.py
--rw-r--r--   0 shurtj     (501) staff       (20)    32351 2023-06-05 22:07:05.000000 khoros-5.3.0.dev2/khoros/structures/boards.py
--rw-r--r--   0 shurtj     (501) staff       (20)    24979 2022-09-28 20:40:19.000000 khoros-5.3.0.dev2/khoros/structures/categories.py
--rw-r--r--   0 shurtj     (501) staff       (20)    16669 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/structures/communities.py
--rw-r--r--   0 shurtj     (501) staff       (20)    27189 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/structures/grouphubs.py
--rw-r--r--   0 shurtj     (501) staff       (20)    27256 2021-03-26 08:19:55.000000 khoros-5.3.0.dev2/khoros/structures/nodes.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.477786 khoros-5.3.0.dev2/khoros/studio/
--rw-r--r--   0 shurtj     (501) staff       (20)      411 2020-05-21 02:08:38.000000 khoros-5.3.0.dev2/khoros/studio/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2845 2023-06-14 20:27:59.000000 khoros-5.3.0.dev2/khoros/studio/base.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.483737 khoros-5.3.0.dev2/khoros/utils/
--rw-r--r--   0 shurtj     (501) staff       (20)      280 2020-05-20 04:19:02.000000 khoros-5.3.0.dev2/khoros/utils/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    19423 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5939 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/environment.py
--rw-r--r--   0 shurtj     (501) staff       (20)    11243 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/helper.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12035 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/log_utils.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.506892 khoros-5.3.0.dev2/khoros/utils/tests/
--rw-r--r--   0 shurtj     (501) staff       (20)      229 2020-05-20 04:19:02.000000 khoros-5.3.0.dev2/khoros/utils/tests/__init__.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12107 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/utils/tests/resources.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1869 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_albums.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2775 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_archives.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5146 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_board_creation.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4453 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_bulk_data.py
--rw-r--r--   0 shurtj     (501) staff       (20)     6575 2022-10-28 20:28:53.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_categories.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3944 2022-09-29 22:14:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_communities.py
--rw-r--r--   0 shurtj     (501) staff       (20)     7147 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_core_utils.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2582 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_error_handling.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12531 2022-12-05 21:42:42.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_exceptions.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1916 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_grouphub_creation.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1425 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_helper_file.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2186 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_http_headers.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1035 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_library_import.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4704 2022-09-29 22:14:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_liql.py
--rw-r--r--   0 shurtj     (501) staff       (20)    12826 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_mentions.py
--rw-r--r--   0 shurtj     (501) staff       (20)    13752 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_messages.py
--rw-r--r--   0 shurtj     (501) staff       (20)     4640 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_node_id_extract.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5701 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_roles.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3621 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_settings.py
--rw-r--r--   0 shurtj     (501) staff       (20)     2281 2022-09-20 20:51:22.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_ssl_verify.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1419 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_studio.py
--rw-r--r--   0 shurtj     (501) staff       (20)     5829 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_tags.py
--rw-r--r--   0 shurtj     (501) staff       (20)     8450 2022-10-04 19:53:13.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_users.py
--rw-r--r--   0 shurtj     (501) staff       (20)     1517 2022-09-28 20:40:19.000000 khoros-5.3.0.dev2/khoros/utils/tests/test_version.py
--rw-r--r--   0 shurtj     (501) staff       (20)     3790 2023-07-07 14:06:27.000000 khoros-5.3.0.dev2/khoros/utils/version.py
-drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-07 19:37:54.452211 khoros-5.3.0.dev2/khoros.egg-info/
--rw-r--r--   0 shurtj     (501) staff       (20)    17352 2023-07-07 19:37:54.000000 khoros-5.3.0.dev2/khoros.egg-info/PKG-INFO
--rw-r--r--   0 shurtj     (501) staff       (20)     2096 2023-07-07 19:37:54.000000 khoros-5.3.0.dev2/khoros.egg-info/SOURCES.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-07-07 19:37:54.000000 khoros-5.3.0.dev2/khoros.egg-info/dependency_links.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      291 2023-07-07 19:37:54.000000 khoros-5.3.0.dev2/khoros.egg-info/requires.txt
--rw-r--r--   0 shurtj     (501) staff       (20)        7 2023-07-07 19:37:54.000000 khoros-5.3.0.dev2/khoros.egg-info/top_level.txt
--rw-r--r--   0 shurtj     (501) staff       (20)      917 2023-07-07 14:06:40.000000 khoros-5.3.0.dev2/pyproject.toml
--rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-07-07 19:37:54.508756 khoros-5.3.0.dev2/setup.cfg
--rw-r--r--   0 shurtj     (501) staff       (20)     3483 2022-09-27 22:19:00.000000 khoros-5.3.0.dev2/setup.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-26 20:46:34.372106 khoros-5.3.0rc1/
+-rw-r--r--   0 shurtj     (501) staff       (20)     1071 2020-05-20 04:19:02.000000 khoros-5.3.0rc1/LICENSE
+-rw-r--r--   0 shurtj     (501) staff       (20)    17351 2023-07-26 20:46:34.371676 khoros-5.3.0rc1/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)    15697 2023-07-07 19:40:33.000000 khoros-5.3.0rc1/README.md
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-26 20:46:34.288804 khoros-5.3.0rc1/khoros/
+-rw-r--r--   0 shurtj     (501) staff       (20)      799 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    73826 2023-07-07 19:40:22.000000 khoros-5.3.0rc1/khoros/api.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11891 2023-07-07 19:40:22.000000 khoros-5.3.0rc1/khoros/auth.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    14989 2023-07-07 19:40:22.000000 khoros-5.3.0rc1/khoros/bulk_data.py
+-rw-r--r--   0 shurtj     (501) staff       (20)   281009 2023-07-10 17:31:55.000000 khoros-5.3.0rc1/khoros/core.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-26 20:46:34.299030 khoros-5.3.0rc1/khoros/errors/
+-rw-r--r--   0 shurtj     (501) staff       (20)      597 2020-07-07 04:29:45.000000 khoros-5.3.0rc1/khoros/errors/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    30504 2022-12-05 21:42:42.000000 khoros-5.3.0rc1/khoros/errors/exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11117 2023-07-07 19:40:22.000000 khoros-5.3.0rc1/khoros/errors/handlers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2631 2020-12-26 17:57:00.000000 khoros-5.3.0rc1/khoros/errors/translations.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    23051 2023-07-07 19:40:22.000000 khoros-5.3.0rc1/khoros/liql.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-26 20:46:34.318142 khoros-5.3.0rc1/khoros/objects/
+-rw-r--r--   0 shurtj     (501) staff       (20)      856 2021-10-11 04:30:21.000000 khoros-5.3.0rc1/khoros/objects/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5999 2020-10-30 02:28:27.000000 khoros-5.3.0rc1/khoros/objects/albums.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    15595 2022-12-05 21:42:42.000000 khoros-5.3.0rc1/khoros/objects/archives.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     6697 2020-10-30 02:28:27.000000 khoros-5.3.0rc1/khoros/objects/attachments.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3290 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/objects/base.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1508 2023-07-07 19:40:22.000000 khoros-5.3.0rc1/khoros/objects/labels.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    60447 2022-09-28 20:40:19.000000 khoros-5.3.0rc1/khoros/objects/messages.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    23431 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/objects/roles.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    10387 2022-10-28 20:28:53.000000 khoros-5.3.0rc1/khoros/objects/settings.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12899 2021-05-20 22:43:31.000000 khoros-5.3.0rc1/khoros/objects/subscriptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     8692 2022-10-04 19:53:13.000000 khoros-5.3.0rc1/khoros/objects/tags.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    67189 2023-07-10 17:28:22.000000 khoros-5.3.0rc1/khoros/objects/users.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4106 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/saml.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-26 20:46:34.333366 khoros-5.3.0rc1/khoros/structures/
+-rw-r--r--   0 shurtj     (501) staff       (20)      566 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/structures/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    20187 2022-09-29 22:14:22.000000 khoros-5.3.0rc1/khoros/structures/base.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    32351 2023-07-07 19:40:22.000000 khoros-5.3.0rc1/khoros/structures/boards.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    24979 2022-09-28 20:40:19.000000 khoros-5.3.0rc1/khoros/structures/categories.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    16669 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/structures/communities.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    27189 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/structures/grouphubs.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    27256 2021-03-26 08:19:55.000000 khoros-5.3.0rc1/khoros/structures/nodes.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-26 20:46:34.336120 khoros-5.3.0rc1/khoros/studio/
+-rw-r--r--   0 shurtj     (501) staff       (20)      411 2020-05-21 02:08:38.000000 khoros-5.3.0rc1/khoros/studio/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2845 2023-07-07 19:40:22.000000 khoros-5.3.0rc1/khoros/studio/base.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-26 20:46:34.342122 khoros-5.3.0rc1/khoros/utils/
+-rw-r--r--   0 shurtj     (501) staff       (20)      280 2020-05-20 04:19:02.000000 khoros-5.3.0rc1/khoros/utils/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    19423 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5939 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/environment.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    11243 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/helper.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12035 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/log_utils.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-26 20:46:34.370379 khoros-5.3.0rc1/khoros/utils/tests/
+-rw-r--r--   0 shurtj     (501) staff       (20)      229 2020-05-20 04:19:02.000000 khoros-5.3.0rc1/khoros/utils/tests/__init__.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12107 2022-12-05 21:42:42.000000 khoros-5.3.0rc1/khoros/utils/tests/resources.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1869 2022-10-04 19:53:13.000000 khoros-5.3.0rc1/khoros/utils/tests/test_albums.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2775 2022-12-05 21:42:42.000000 khoros-5.3.0rc1/khoros/utils/tests/test_archives.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5146 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_board_creation.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4453 2022-12-05 21:42:42.000000 khoros-5.3.0rc1/khoros/utils/tests/test_bulk_data.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     6575 2022-10-28 20:28:53.000000 khoros-5.3.0rc1/khoros/utils/tests/test_categories.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3944 2022-09-29 22:14:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_communities.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     7147 2022-10-04 19:53:13.000000 khoros-5.3.0rc1/khoros/utils/tests/test_core_utils.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2582 2022-10-04 19:53:13.000000 khoros-5.3.0rc1/khoros/utils/tests/test_error_handling.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12531 2022-12-05 21:42:42.000000 khoros-5.3.0rc1/khoros/utils/tests/test_exceptions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1916 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_grouphub_creation.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1425 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_helper_file.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2186 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_http_headers.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1035 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_library_import.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4704 2022-09-29 22:14:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_liql.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    12826 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_mentions.py
+-rw-r--r--   0 shurtj     (501) staff       (20)    14200 2023-07-10 19:09:06.000000 khoros-5.3.0rc1/khoros/utils/tests/test_messages.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     4640 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_node_id_extract.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5701 2022-10-04 19:53:13.000000 khoros-5.3.0rc1/khoros/utils/tests/test_roles.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3621 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_settings.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     2281 2022-09-20 20:51:22.000000 khoros-5.3.0rc1/khoros/utils/tests/test_ssl_verify.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1419 2022-10-04 19:53:13.000000 khoros-5.3.0rc1/khoros/utils/tests/test_studio.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     5829 2022-10-04 19:53:13.000000 khoros-5.3.0rc1/khoros/utils/tests/test_tags.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     9113 2023-07-10 19:18:25.000000 khoros-5.3.0rc1/khoros/utils/tests/test_users.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     1517 2022-09-28 20:40:19.000000 khoros-5.3.0rc1/khoros/utils/tests/test_version.py
+-rw-r--r--   0 shurtj     (501) staff       (20)     3789 2023-07-26 20:45:56.000000 khoros-5.3.0rc1/khoros/utils/version.py
+drwxr-xr-x   0 shurtj     (501) staff       (20)        0 2023-07-26 20:46:34.292369 khoros-5.3.0rc1/khoros.egg-info/
+-rw-r--r--   0 shurtj     (501) staff       (20)    17351 2023-07-26 20:46:33.000000 khoros-5.3.0rc1/khoros.egg-info/PKG-INFO
+-rw-r--r--   0 shurtj     (501) staff       (20)     2096 2023-07-26 20:46:33.000000 khoros-5.3.0rc1/khoros.egg-info/SOURCES.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        1 2023-07-26 20:46:33.000000 khoros-5.3.0rc1/khoros.egg-info/dependency_links.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      291 2023-07-26 20:46:33.000000 khoros-5.3.0rc1/khoros.egg-info/requires.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)        7 2023-07-26 20:46:33.000000 khoros-5.3.0rc1/khoros.egg-info/top_level.txt
+-rw-r--r--   0 shurtj     (501) staff       (20)      916 2023-07-26 20:45:05.000000 khoros-5.3.0rc1/pyproject.toml
+-rw-r--r--   0 shurtj     (501) staff       (20)       38 2023-07-26 20:46:34.372257 khoros-5.3.0rc1/setup.cfg
+-rw-r--r--   0 shurtj     (501) staff       (20)     3483 2022-09-27 22:19:00.000000 khoros-5.3.0rc1/setup.py
```

### Comparing `khoros-5.3.0.dev2/LICENSE` & `khoros-5.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/PKG-INFO` & `khoros-5.3.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoros
-Version: 5.3.0.dev2
+Version: 5.3.0rc1
 Summary: Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment.
 Home-page: https://github.com/jeffshurtliff/khoros
 Author: Jeff Shurtliff
 Author-email: jeff.shurtliff@rsa.com
 Project-URL: Changelog, https://khoros.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://khoros.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/jeffshurtliff/khoros/issues
@@ -45,15 +45,15 @@
             </a>
         </td>
     </tr>
     <tr>
         <td>Latest Beta/RC Release</td>
         <td>
             <a href='https://pypi.org/project/khoros/#history'>
-                <img alt="PyPI" src="https://img.shields.io/badge/pypi-5.2.0rc1-blue">
+                <img alt="PyPI" src="https://img.shields.io/badge/pypi-5.3.0dev2-blue">
             </a>
         </td>
     </tr>
     <tr>
         <td>Build Status</td>
         <td>
             <a href="https://github.com/jeffshurtliff/khoros/blob/master/.github/workflows/pythonpackage.yml">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: khoros Version: 5.3.0.dev2 Summary: Useful tools
-and utilities to assist in managing a Khoros Communities (formerly Lithium)
+Metadata-Version: 2.1 Name: khoros Version: 5.3.0rc1 Summary: Useful tools and
+utilities to assist in managing a Khoros Communities (formerly Lithium)
 environment. Home-page: https://github.com/jeffshurtliff/khoros Author: Jeff
 Shurtliff Author-email: jeff.shurtliff@rsa.com Project-URL: Changelog, https://
 khoros.readthedocs.io/en/latest/changelog.html Project-URL: Documentation,
 https://khoros.readthedocs.io/ Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/khoros/issues Project-URL: Khoros Dev Docs, https://
 developer.khoros.com/khoroscommunitydevdocs Classifier: Development Status :: 5
 - Production/Stable Classifier: Environment :: Web Environment Classifier:
```

### Comparing `khoros-5.3.0.dev2/README.md` & `khoros-5.3.0rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             </a>
         </td>
     </tr>
     <tr>
         <td>Latest Beta/RC Release</td>
         <td>
             <a href='https://pypi.org/project/khoros/#history'>
-                <img alt="PyPI" src="https://img.shields.io/badge/pypi-5.2.0rc1-blue">
+                <img alt="PyPI" src="https://img.shields.io/badge/pypi-5.3.0dev2-blue">
             </a>
         </td>
     </tr>
     <tr>
         <td>Build Status</td>
         <td>
             <a href="https://github.com/jeffshurtliff/khoros/blob/master/.github/workflows/pythonpackage.yml">
```

### Comparing `khoros-5.3.0.dev2/khoros/__init__.py` & `khoros-5.3.0rc1/khoros/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/api.py` & `khoros-5.3.0rc1/khoros/api.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/auth.py` & `khoros-5.3.0rc1/khoros/auth.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/bulk_data.py` & `khoros-5.3.0rc1/khoros/bulk_data.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/core.py` & `khoros-5.3.0rc1/khoros/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 :Module:            khoros.core
 :Synopsis:          Collection of core functions and tools to work with the Khoros Community APIs
 :Usage:             ``import khoros.core`` *(Imported by default in primary package)*
 :Example:           ``khoros = Khoros(helper='helper.yml')``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     06 Jul 2023
+:Modified Date:     10 Jul 2023
 """
 
 import sys
 import copy
 import logging
 import warnings
 
@@ -4817,14 +4817,29 @@
             :type email: str, None
             :returns: The number of kudos received by the user in integer format
             :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
             """
             return objects_module.users.get_kudos_received_count(self.khoros_object, user_settings, user_id,
                                                                  login, email)
 
+        def get_users_count(self, registered=False, online=False):
+            """This method returns the total number of users in an environment. (Filtering possible for registered and online)
+
+            .. versionadded:: 5.3.0
+
+            :param registered: Return a count of registered users (``False`` by default)
+            :type registered: bool
+            :param online: Return a count of online users (``False`` by default)
+            :type online: bool
+            :returns: An integer defining the total user count for the environment
+            :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`,
+                     :py:exc:`khoros.errors.exceptions.InvalidParameterError`
+            """
+            return objects_module.users.get_users_count(self.khoros_object, registered=registered, online=online)
+
         def get_online_user_count(self):
             """This method retrieves the number of users currently online.
 
             :returns: The user count for online users as an integer
             :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
             """
             return objects_module.users.get_online_user_count(self.khoros_object)
@@ -4835,14 +4850,39 @@
             .. versionadded:: 5.2.0
 
             :returns: The user count for total users as an integer
             :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
             """
             return objects_module.users.get_all_users_count(self.khoros_object)
 
+        def get_all_users(self, fields=None, order_by='last_visit_time', order_by_desc=True):
+            """This function retrieves data for all users.
+
+            .. versionadded:: 5.3.0
+
+            :param fields: Specific fields to query if not all fields are needed (comma-separated string or iterable)
+            :type fields: str, tuple, list, set, None
+            :param order_by: The order by which to sort the data (``last_visit_time`` by default)
+            :type order_by: str
+            :param order_by_desc: Indicates if the data should be sorted in descending (default) or ascending order
+            :type order_by_desc: bool
+            :returns: A list containing a dictionary of data for each user
+            :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
+            """
+            return objects_module.users.get_all_users(self.khoros_object, fields, order_by, order_by_desc)
+
+        def get_registered_users_count(self):
+            """This method returns the total count of registered users on the community.
+
+            .. versionadded:: 5.0.0
+
+            :returns: An integer of the total registered users count
+            """
+            return objects_module.users.get_registered_users_count(self.khoros_object)
+
         def get_registration_data(self, user_settings=None, user_id=None, login=None, email=None):
             """This method retrieves the registration data for a given user.
 
             :param user_settings: A dictionary containing all relevant user settings supplied in the parent function
             :type user_settings: dict, None
             :param user_id: The User ID associated with the user
             :type user_id: int, str, None
@@ -4918,25 +4958,16 @@
             :param user_login: The username that identifies the user
             :type user_login: str, None
             :returns: The API response
             :raises: py:exc:`khoros.errors.exceptions.MissingRequiredDataError`
             """
             return objects_module.users.update_sso_id(self.khoros_object, new_sso_id, user_id, user_login)
 
-        def get_registered_users_count(self):
-            """This function returns the total count of registered users on the community.
-
-            .. versionadded:: 5.0.0
-
-            :returns: An integer of the total registered users count
-            """
-            return objects_module.users.get_registered_users_count(self.khoros_object)
-
         def get_online_users_count(self, anonymous=None, registered=None):
-            """This function returns the total count of users currently online.
+            """This method returns the total count of users currently online.
 
             .. versionadded:: 5.0.0
 
             :param anonymous: Filters the results to only anonymous (non-registered) users
             :type anonymous: bool, None
             :param registered: Filters the results to only registered users
             :type registered: bool, None
```

### Comparing `khoros-5.3.0.dev2/khoros/errors/__init__.py` & `khoros-5.3.0rc1/khoros/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/errors/exceptions.py` & `khoros-5.3.0rc1/khoros/errors/exceptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/errors/handlers.py` & `khoros-5.3.0rc1/khoros/errors/handlers.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/errors/translations.py` & `khoros-5.3.0rc1/khoros/errors/translations.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/liql.py` & `khoros-5.3.0rc1/khoros/liql.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/__init__.py` & `khoros-5.3.0rc1/khoros/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/albums.py` & `khoros-5.3.0rc1/khoros/objects/albums.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/archives.py` & `khoros-5.3.0rc1/khoros/objects/archives.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/attachments.py` & `khoros-5.3.0rc1/khoros/objects/attachments.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/base.py` & `khoros-5.3.0rc1/khoros/objects/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/labels.py` & `khoros-5.3.0rc1/khoros/objects/labels.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/messages.py` & `khoros-5.3.0rc1/khoros/objects/messages.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/roles.py` & `khoros-5.3.0rc1/khoros/objects/roles.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/settings.py` & `khoros-5.3.0rc1/khoros/objects/settings.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/subscriptions.py` & `khoros-5.3.0rc1/khoros/objects/subscriptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/tags.py` & `khoros-5.3.0rc1/khoros/objects/tags.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/objects/users.py` & `khoros-5.3.0rc1/khoros/objects/users.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 """
 :Module:            khoros.objects.users
 :Synopsis:          This module includes functions that handle user-related operations.
 :Usage:             ``from khoros.objects import users``
 :Example:           ``khoros.users.create(username='john_doe', email='john.doe@example.com')``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     24 May 2022
+:Modified Date:     10 Jul 2023
 """
 
 import warnings
+from operator import itemgetter
 
 from .. import api, auth, liql, errors
 from ..utils import core_utils, log_utils
 
 # Initialize the logger for this module
 logger = log_utils.initialize_logging(__name__)
 
@@ -1024,29 +1025,14 @@
     :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
     """
     liql_query = "select count(*) from users where online_status = 'online'"
     api_response = liql.perform_query(khoros_object, liql_query=liql_query, verify_success=True)
     return int(api_response['data']['count'])
 
 
-def get_all_users_count(khoros_object):
-    """This function retrieves the total number of users on the community.
-
-    .. versionadded:: 5.2.0
-
-    :param khoros_object: The core :py:class:`khoros.Khoros` object
-    :type khoros_object: class[khoros.Khoros]
-    :returns: The user count for total users as an integer
-    :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
-    """
-    liql_query = "select count(*) from users"
-    api_response = liql.perform_query(khoros_object, liql_query=liql_query, verify_success=True)
-    return int(api_response['data']['count'])
-
-
 def get_registration_data(khoros_object, user_settings=None, user_id=None, login=None, email=None):
     """This function retrieves the registration data for a given user.
 
     :param khoros_object: The core :py:class:`khoros.Khoros` object
     :type khoros_object: class[khoros.Khoros]
     :param user_settings: A dictionary containing all relevant user settings supplied in the parent function
     :type user_settings: dict, None
@@ -1191,14 +1177,55 @@
     for login in login_list:
         user_id = get_user_id(khoros_object, login=login)
         id_list.append(user_id)
         id_dict[login] = user_id
     return id_list if return_type == 'list' else id_dict
 
 
+def get_users_count(khoros_object, registered=False, online=False):
+    """This function returns the total number of users in an environment. (Filtering possible for registered and online)
+
+    .. versionadded:: 5.3.0
+
+    :param khoros_object: The core :py:class:`khoros.Khoros` object
+    :type khoros_object: class[khoros.Khoros]
+    :param registered: Return a count of registered users (``False`` by default)
+    :type registered: bool
+    :param online: Return a count of online users (``False`` by default)
+    :type online: bool
+    :returns: An integer defining the total user count for the environment
+    :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`,
+             :py:exc:`khoros.errors.exceptions.InvalidParameterError`
+    """
+    if all((registered, online)):
+        raise errors.exceptions.InvalidParameterError('You can only select registered or online users but not both.')
+    if registered:
+        user_count = get_registered_users_count(khoros_object)
+    elif online:
+        user_count = get_online_user_count(khoros_object)
+    else:
+        user_count = get_all_users_count(khoros_object)
+    return user_count
+
+
+def get_all_users_count(khoros_object):
+    """This function retrieves the total number of users on the community.
+
+    .. versionadded:: 5.2.0
+
+    :param khoros_object: The core :py:class:`khoros.Khoros` object
+    :type khoros_object: class[khoros.Khoros]
+    :returns: The user count for total users as an integer
+    :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
+    """
+    liql_query = 'SELECT count(*) FROM users'
+    api_response = liql.perform_query(khoros_object, liql_query=liql_query, verify_success=True)
+    return int(api_response['data']['count'])
+
+
 def get_registered_users_count(khoros_object):
     """This function returns the total count of registered users on the community.
 
     .. versionadded:: 5.0.0
 
     :param khoros_object: The core :py:class:`khoros.Khoros` object
     :type khoros_object: class[khoros.Khoros]
@@ -1226,7 +1253,117 @@
     if anonymous and not registered:
         response = api.make_v1_request(khoros_object, '/users/online/anonymous/count')
     elif registered and not anonymous:
         response = api.make_v1_request(khoros_object, '/users/online/registered/count')
     else:
         response = api.make_v1_request(khoros_object, '/users/online/count')
     return response['response']['value']['$']
+
+
+def get_all_users(khoros_object, fields=None, order_by='last_visit_time', order_by_desc=True):
+    """This function retrieves data for all users.
+
+    .. versionadded:: 5.3.0
+
+    :param khoros_object: The core :py:class:`khoros.Khoros` object
+    :type khoros_object: class[khoros.Khoros]
+    :param fields: Specific fields to query if not all fields are needed (comma-separated string or iterable)
+    :type fields: str, tuple, list, set, None
+    :param order_by: The order by which to sort the data (``last_visit_time`` by default)
+    :type order_by: str
+    :param order_by_desc: Indicates if the data should be sorted in descending (default) or ascending order
+    :type order_by_desc: bool
+    :returns: A list containing a dictionary of data for each user
+    :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
+    """
+    # Define the variable where the users will be stored
+    users = []
+
+    # Define the LiQL query to be performed
+    fields = '*' if not fields else fields
+    if not isinstance(fields, str):
+        fields = liql.parse_select_fields(fields)
+    order_direction = 'DESC' if order_by_desc else 'ASC'
+    order = f'ORDER BY {order_by} {order_direction}' if order_by else ''
+    query = f"SELECT {fields} FROM users {order} LIMIT 1000"
+
+    # Perform the first LiQL query and add to the master list
+    response, cursor = _perform_single_query(khoros_object, query, fields)
+    users.extend(response)
+
+    # Continue looping as long as a cursor is present
+    while cursor:
+        response, cursor = _perform_single_query(khoros_object, query, fields, cursor)
+        users.extend(response)
+
+    # Return the collected messages
+    return users
+
+
+def _perform_single_query(khoros_object, query, fields=None, cursor=None):
+    """This function performs a single LiQL query with or without a cursor.
+
+    .. versionadded:: 5.3.0
+
+    :param khoros_object: The core :py:class:`khoros.Khoros` object
+    :type khoros_object: class[khoros.Khoros]
+    :param query: The LiQL query to be performed
+    :type query: str
+    :param fields: Specific fields used in the LiQL SELECT statement
+    :type fields: str, tuple, list, set, None
+    :param cursor: The cursor from the LiQL response (when present)
+    :type cursor: str, None
+    :returns: The response to the LiQL query and the cursor when applicable
+    :raises: :py:exc:`khoros.errors.exceptions.GETRequestError`
+    """
+    # Construct the entire LiQL query
+    cursor = '' if not cursor else liql.structure_cursor_clause(cursor)
+    query = f"{query} {cursor}" if cursor else query
+
+    # Perform the API call and retrieve the data
+    response = liql.perform_query(khoros_object, liql_query=query)
+    data = liql.get_returned_items(response)
+
+    # Get the cursor when present
+    cursor = None
+    if response.get('data').get('next_cursor'):
+        cursor = response['data'].get('next_cursor')
+
+    # Add missing columns to message data as needed
+    data = _add_missing_cols(data, fields)
+    try:
+        data = sorted(data, key=itemgetter(*tuple(data[0].keys())))
+    except KeyError as missing_key:
+        logger.error(f'Could not sort the user data because the \'{missing_key}\' key was missing.')
+
+    # Return the user data and cursor
+    return data, cursor
+
+
+def _add_missing_cols(user_list, fields=None):
+    """This function adds columns (fields) that might be missing from a LiQL response containing users.
+
+    .. versionadded:: 5.3.0
+
+    :param user_list: The list of dictionaries containing user data
+    :type user_list: list
+    :param fields: Specific fields used in the LiQL SELECT statement
+    :type fields: str, tuple, list, set, None
+    :returns: The same Liql response data with the required columns included
+    """
+    new_list = []
+    required_cols = ['type', 'id', 'view_href', 'login']
+
+    # Add any defined fields to the list of required columns
+    if fields and fields != '*':
+        parsed_fields = fields.split(',')
+        for field in parsed_fields:
+            if field not in required_cols:
+                required_cols.append(field)
+
+    # Loop through the messages and add any missing columns
+    for user in user_list:
+        for col in required_cols:
+            if col not in user:
+                user[col] = ''
+        new_list.append(user)
+    return new_list
```

### Comparing `khoros-5.3.0.dev2/khoros/saml.py` & `khoros-5.3.0rc1/khoros/saml.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/structures/__init__.py` & `khoros-5.3.0rc1/khoros/structures/__init__.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/structures/base.py` & `khoros-5.3.0rc1/khoros/structures/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/structures/boards.py` & `khoros-5.3.0rc1/khoros/structures/boards.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/structures/categories.py` & `khoros-5.3.0rc1/khoros/structures/categories.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/structures/communities.py` & `khoros-5.3.0rc1/khoros/structures/communities.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/structures/grouphubs.py` & `khoros-5.3.0rc1/khoros/structures/grouphubs.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/structures/nodes.py` & `khoros-5.3.0rc1/khoros/structures/nodes.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/studio/base.py` & `khoros-5.3.0rc1/khoros/studio/base.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/core_utils.py` & `khoros-5.3.0rc1/khoros/utils/core_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/environment.py` & `khoros-5.3.0rc1/khoros/utils/environment.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/helper.py` & `khoros-5.3.0rc1/khoros/utils/helper.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/log_utils.py` & `khoros-5.3.0rc1/khoros/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/resources.py` & `khoros-5.3.0rc1/khoros/utils/tests/resources.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_albums.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_albums.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_archives.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_archives.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_board_creation.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_board_creation.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_bulk_data.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_bulk_data.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_categories.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_categories.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_communities.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_communities.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_core_utils.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_core_utils.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_error_handling.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_exceptions.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_grouphub_creation.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_grouphub_creation.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_helper_file.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_helper_file.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_http_headers.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_library_import.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_library_import.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_liql.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_liql.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_mentions.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_mentions.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_messages.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 :Module:            khoros.utils.tests.test_messages
 :Synopsis:          This module is used by pytest to verify that messages function properly
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     30 Sep 2022
+:Modified Date:     10 Jul 2023
 """
 
 import os
 import sys
 
 import pytest
 import requests
@@ -73,14 +73,28 @@
     tags_found = []
     for tag_dict in payload['data']['tags']:
         tags_found.append(tag_dict.get('text'))
     for tag in tags_to_find:
         assert tag in tags_found        # nosec
 
 
+def test_count_messages():
+    """This function tests the ability to retrieve a messages count for a specific board.
+
+    .. versionadded:: 5.3.0
+    """
+    # Instantiate the Khoros object
+    set_package_path()
+    khoros_object = resources.get_core_object()
+
+    # Test retrieving the message count for a given board
+    messages_count = khoros_object.boards.get_message_count('support-information')
+    assert isinstance(messages_count, int)
+
+
 def test_construct_only_subject():
     """This function tests to ensure that a :py:exc:`khoros.errors.exceptions.MissingRequiredDataError` exception
     gets raised when only a subject is passed to the :py:func:`khoros.objects.messages.construct_payload` function.
 
     .. versionchanged:: 5.0.0
        Removed the redundant return statement.
     """
```

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_node_id_extract.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_node_id_extract.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_roles.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_roles.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_settings.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_ssl_verify.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_ssl_verify.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_studio.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_studio.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_tags.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_users.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 :Module:            khoros.utils.tests.test_users
 :Synopsis:          This module is used by pytest to verify that the ``users`` module functions properly
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     03 Oct 2022
+:Modified Date:     10 Jul 2023
 """
 
 import os
 import sys
 
 import pytest
 import requests
@@ -150,14 +150,17 @@
     response = khoros_object.users.query_users_table_by_id(['login', 'email'], USER_ID)
     assert response.get('status') == 'success'
 
 
 def test_get_counts():
     """This function tests the various functions that involve retrieving user-related counts.
 
+    .. versionchanged:: 5.3.0
+       Added assertions for the :py:meth:`khoros.core.Khoros.User.get_users_count` method.
+
     .. versionadded:: 5.1.2
     """
     # Instantiate the core object
     khoros_object = resources.get_core_object()
 
     # Test retrieving the album count and verifying the response
     album_count = khoros_object.users.get_album_count(user_id=USER_ID)
@@ -210,10 +213,20 @@
     kudos_received_count = khoros_object.users.get_kudos_received_count(user_id=USER_ID)
     assert isinstance(kudos_received_count, int) and kudos_received_count >= 0
 
     # Test retrieving the online users count
     online_users_count = khoros_object.users.get_online_user_count()
     assert isinstance(online_users_count, int)
 
+    # Test the variations of the get_users_count() method
+    users_count = khoros_object.users.get_users_count()
+    registered_users_count = khoros_object.users.get_users_count(registered=True)
+    online_users_count = khoros_object.users.get_users_count(online=True)
+    assert isinstance(users_count, int)
+    assert isinstance(registered_users_count, int)
+    assert isinstance(online_users_count, int)
+    with pytest.raises(exceptions.InvalidParameterError):
+        khoros_object.users.get_users_count(registered=True, online=True)
+
 
 # Import the exceptions modules
 exceptions = resources.import_modules('khoros.errors.exceptions')
```

### Comparing `khoros-5.3.0.dev2/khoros/utils/tests/test_version.py` & `khoros-5.3.0rc1/khoros/utils/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/khoros/utils/version.py` & `khoros-5.3.0rc1/khoros/utils/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 """
 :Module:            khoros.utils.version
 :Synopsis:          This simple script contains the package version
 :Usage:             ``from .utils import version``
 :Example:           ``__version__ = version.get_full_version()``
 :Created By:        Jeff Shurtliff
 :Last Modified:     Jeff Shurtliff
-:Modified Date:     07 Jul 2023
+:Modified Date:     26 Jul 2023
 """
 
 import json
 import urllib.request
 
 from . import log_utils
 
 # Define special and global variables
-__version__ = "5.3.0dev2"
+__version__ = "5.3.0rc1"
 latest_version_reported = False
 logger = log_utils.initialize_logging(__name__)
 
 
 def get_full_version():
     """This function returns the current full version of the khoros package."""
     return __version__
```

### Comparing `khoros-5.3.0.dev2/khoros.egg-info/PKG-INFO` & `khoros-5.3.0rc1/khoros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoros
-Version: 5.3.0.dev2
+Version: 5.3.0rc1
 Summary: Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment.
 Home-page: https://github.com/jeffshurtliff/khoros
 Author: Jeff Shurtliff
 Author-email: jeff.shurtliff@rsa.com
 Project-URL: Changelog, https://khoros.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://khoros.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/jeffshurtliff/khoros/issues
@@ -45,15 +45,15 @@
             </a>
         </td>
     </tr>
     <tr>
         <td>Latest Beta/RC Release</td>
         <td>
             <a href='https://pypi.org/project/khoros/#history'>
-                <img alt="PyPI" src="https://img.shields.io/badge/pypi-5.2.0rc1-blue">
+                <img alt="PyPI" src="https://img.shields.io/badge/pypi-5.3.0dev2-blue">
             </a>
         </td>
     </tr>
     <tr>
         <td>Build Status</td>
         <td>
             <a href="https://github.com/jeffshurtliff/khoros/blob/master/.github/workflows/pythonpackage.yml">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: khoros Version: 5.3.0.dev2 Summary: Useful tools
-and utilities to assist in managing a Khoros Communities (formerly Lithium)
+Metadata-Version: 2.1 Name: khoros Version: 5.3.0rc1 Summary: Useful tools and
+utilities to assist in managing a Khoros Communities (formerly Lithium)
 environment. Home-page: https://github.com/jeffshurtliff/khoros Author: Jeff
 Shurtliff Author-email: jeff.shurtliff@rsa.com Project-URL: Changelog, https://
 khoros.readthedocs.io/en/latest/changelog.html Project-URL: Documentation,
 https://khoros.readthedocs.io/ Project-URL: Issue Tracker, https://github.com/
 jeffshurtliff/khoros/issues Project-URL: Khoros Dev Docs, https://
 developer.khoros.com/khoroscommunitydevdocs Classifier: Development Status :: 5
 - Production/Stable Classifier: Environment :: Web Environment Classifier:
```

### Comparing `khoros-5.3.0.dev2/khoros.egg-info/SOURCES.txt` & `khoros-5.3.0rc1/khoros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khoros-5.3.0.dev2/pyproject.toml` & `khoros-5.3.0rc1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "khoros"
-version = "5.3.0dev2"
+version = "5.3.0rc1"
 description = "Useful tools and utilities to assist in managing a Khoros Communities (formerly Lithium) environment."
 authors = ["Jeff Shurtliff <jeff.shurtliff@rsa.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
```

### Comparing `khoros-5.3.0.dev2/setup.py` & `khoros-5.3.0rc1/setup.py`

 * *Files identical despite different names*

