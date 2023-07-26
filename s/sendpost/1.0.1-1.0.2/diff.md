# Comparing `tmp/sendpost-1.0.1.tar.gz` & `tmp/sendpost-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sendpost-1.0.1.tar", last modified: Wed Jul 26 13:29:21 2023, max compression
+gzip compressed data, was "dist/sendpost-1.0.2.tar", last modified: Wed Jul 26 13:36:43 2023, max compression
```

## Comparing `sendpost-1.0.1.tar` & `sendpost-1.0.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/
--rw-r--r--   0 arseniy    (501) staff       (20)      652 2023-07-26 13:29:21.000000 sendpost-1.0.1/PKG-INFO
--rw-r--r--   0 arseniy    (501) staff       (20)     3180 2023-07-26 12:36:30.000000 sendpost-1.0.1/README.md
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost.egg-info/
--rw-r--r--   0 arseniy    (501) staff       (20)      652 2023-07-26 13:29:20.000000 sendpost-1.0.1/sendpost.egg-info/PKG-INFO
--rw-r--r--   0 arseniy    (501) staff       (20)     2475 2023-07-26 13:29:20.000000 sendpost-1.0.1/sendpost.egg-info/SOURCES.txt
--rw-r--r--   0 arseniy    (501) staff       (20)        1 2023-07-26 13:29:20.000000 sendpost-1.0.1/sendpost.egg-info/dependency_links.txt
--rw-r--r--   0 arseniy    (501) staff       (20)      118 2023-07-26 13:29:20.000000 sendpost-1.0.1/sendpost.egg-info/requires.txt
--rw-r--r--   0 arseniy    (501) staff       (20)       25 2023-07-26 13:29:20.000000 sendpost-1.0.1/sendpost.egg-info/top_level.txt
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/
--rw-r--r--   0 arseniy    (501) staff       (20)      979 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)    58859 2023-07-26 12:39:50.000000 sendpost-1.0.1/sendpost_python_sdk/api_client.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/apis/
--rw-r--r--   0 arseniy    (501) staff       (20)      214 2023-07-26 12:34:02.000000 sendpost-1.0.1/sendpost_python_sdk/apis/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      610 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/path_to_api.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/apis/paths/
--rw-r--r--   0 arseniy    (501) staff       (20)      246 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/paths/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      125 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/paths/subaccount_email_.py
--rw-r--r--   0 arseniy    (501) staff       (20)      141 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/paths/subaccount_email_template.py
--rw-r--r--   0 arseniy    (501) staff       (20)      318 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/tag_to_api.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/apis/tags/
--rw-r--r--   0 arseniy    (501) staff       (20)      312 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/tags/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      800 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/tags/email_api.py
--rw-r--r--   0 arseniy    (501) staff       (20)    15568 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/configuration.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4702 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/exceptions.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/model/
--rw-r--r--   0 arseniy    (501) staff       (20)      353 2023-07-26 12:34:02.000000 sendpost-1.0.1/sendpost_python_sdk/model/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3139 2023-07-26 12:33:55.000000 sendpost-1.0.1/sendpost_python_sdk/model/attachment.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4856 2023-07-26 12:33:56.000000 sendpost-1.0.1/sendpost_python_sdk/model/city.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3661 2023-07-26 12:33:56.000000 sendpost-1.0.1/sendpost_python_sdk/model/copy_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)     2587 2023-07-26 12:33:57.000000 sendpost-1.0.1/sendpost_python_sdk/model/device.py
--rw-r--r--   0 arseniy    (501) staff       (20)    12636 2023-07-26 12:33:57.000000 sendpost-1.0.1/sendpost_python_sdk/model/email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4761 2023-07-26 12:33:58.000000 sendpost-1.0.1/sendpost_python_sdk/model/email_response.py
--rw-r--r--   0 arseniy    (501) staff       (20)     6066 2023-07-26 12:33:58.000000 sendpost-1.0.1/sendpost_python_sdk/model/event_metadata.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3059 2023-07-26 12:33:58.000000 sendpost-1.0.1/sendpost_python_sdk/model/model_from.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4612 2023-07-26 12:33:58.000000 sendpost-1.0.1/sendpost_python_sdk/model/os.py
--rw-r--r--   0 arseniy    (501) staff       (20)    20181 2023-07-26 12:33:59.000000 sendpost-1.0.1/sendpost_python_sdk/model/q_email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)     9817 2023-07-26 12:33:59.000000 sendpost-1.0.1/sendpost_python_sdk/model/q_event.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3055 2023-07-26 12:34:00.000000 sendpost-1.0.1/sendpost_python_sdk/model/reply_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)     6319 2023-07-26 12:34:00.000000 sendpost-1.0.1/sendpost_python_sdk/model/to.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4069 2023-07-26 12:34:00.000000 sendpost-1.0.1/sendpost_python_sdk/model/user_agent.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3347 2023-07-26 12:34:00.000000 sendpost-1.0.1/sendpost_python_sdk/model/webhook_event.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/models/
--rw-r--r--   0 arseniy    (501) staff       (20)     1252 2023-07-26 12:34:02.000000 sendpost-1.0.1/sendpost_python_sdk/models/__init__.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/paths/
--rw-r--r--   0 arseniy    (501) staff       (20)      401 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/paths/__init__.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_/
--rw-r--r--   0 arseniy    (501) staff       (20)      331 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)    15448 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_/post.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_template/
--rw-r--r--   0 arseniy    (501) staff       (20)      347 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_template/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)    15628 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_template/post.py
--rw-r--r--   0 arseniy    (501) staff       (20)    10860 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/rest.py
--rw-r--r--   0 arseniy    (501) staff       (20)    97848 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/schemas.py
--rw-r--r--   0 arseniy    (501) staff       (20)      110 2023-07-26 13:29:21.000000 sendpost-1.0.1/setup.cfg
--rw-r--r--   0 arseniy    (501) staff       (20)     1631 2023-07-26 13:24:19.000000 sendpost-1.0.1/setup.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/test/
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/test/test_models/
--rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_models/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      748 2023-07-26 12:33:55.000000 sendpost-1.0.1/test/test_models/test_attachment.py
--rw-r--r--   0 arseniy    (501) staff       (20)      724 2023-07-26 12:33:56.000000 sendpost-1.0.1/test/test_models/test_city.py
--rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 12:33:56.000000 sendpost-1.0.1/test/test_models/test_copy_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)      732 2023-07-26 12:33:57.000000 sendpost-1.0.1/test/test_models/test_device.py
--rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-07-26 12:33:57.000000 sendpost-1.0.1/test/test_models/test_email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-07-26 12:33:58.000000 sendpost-1.0.1/test/test_models/test_email_response.py
--rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-07-26 12:33:58.000000 sendpost-1.0.1/test/test_models/test_event_metadata.py
--rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 12:33:58.000000 sendpost-1.0.1/test/test_models/test_model_from.py
--rw-r--r--   0 arseniy    (501) staff       (20)      716 2023-07-26 12:33:58.000000 sendpost-1.0.1/test/test_models/test_os.py
--rw-r--r--   0 arseniy    (501) staff       (20)      762 2023-07-26 12:33:59.000000 sendpost-1.0.1/test/test_models/test_q_email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 12:34:00.000000 sendpost-1.0.1/test/test_models/test_q_event.py
--rw-r--r--   0 arseniy    (501) staff       (20)      737 2023-07-26 12:34:00.000000 sendpost-1.0.1/test/test_models/test_reply_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)      716 2023-07-26 12:34:00.000000 sendpost-1.0.1/test/test_models/test_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 12:34:00.000000 sendpost-1.0.1/test/test_models/test_user_agent.py
--rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-07-26 12:34:00.000000 sendpost-1.0.1/test/test_models/test_webhook_event.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/test/test_paths/
--rw-r--r--   0 arseniy    (501) staff       (20)     1995 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_paths/__init__.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_/
--rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      802 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_/test_post.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_template/
--rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_template/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      826 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_template/test_post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/
+-rw-r--r--   0 arseniy    (501) staff       (20)      652 2023-07-26 13:36:43.000000 sendpost-1.0.2/PKG-INFO
+-rw-r--r--   0 arseniy    (501) staff       (20)     3180 2023-07-26 12:36:30.000000 sendpost-1.0.2/README.md
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost.egg-info/
+-rw-r--r--   0 arseniy    (501) staff       (20)      652 2023-07-26 13:36:42.000000 sendpost-1.0.2/sendpost.egg-info/PKG-INFO
+-rw-r--r--   0 arseniy    (501) staff       (20)     2475 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost.egg-info/SOURCES.txt
+-rw-r--r--   0 arseniy    (501) staff       (20)        1 2023-07-26 13:36:42.000000 sendpost-1.0.2/sendpost.egg-info/dependency_links.txt
+-rw-r--r--   0 arseniy    (501) staff       (20)      118 2023-07-26 13:36:42.000000 sendpost-1.0.2/sendpost.egg-info/requires.txt
+-rw-r--r--   0 arseniy    (501) staff       (20)       25 2023-07-26 13:36:42.000000 sendpost-1.0.2/sendpost.egg-info/top_level.txt
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost_python_sdk/
+-rw-r--r--   0 arseniy    (501) staff       (20)      979 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    58859 2023-07-26 12:39:50.000000 sendpost-1.0.2/sendpost_python_sdk/api_client.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost_python_sdk/apis/
+-rw-r--r--   0 arseniy    (501) staff       (20)      214 2023-07-26 12:34:02.000000 sendpost-1.0.2/sendpost_python_sdk/apis/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      610 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/apis/path_to_api.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost_python_sdk/apis/paths/
+-rw-r--r--   0 arseniy    (501) staff       (20)      246 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/apis/paths/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      125 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/apis/paths/subaccount_email_.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      141 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/apis/paths/subaccount_email_template.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      318 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/apis/tag_to_api.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost_python_sdk/apis/tags/
+-rw-r--r--   0 arseniy    (501) staff       (20)      312 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/apis/tags/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      800 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/apis/tags/email_api.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15568 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/configuration.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4702 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/exceptions.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost_python_sdk/model/
+-rw-r--r--   0 arseniy    (501) staff       (20)      353 2023-07-26 12:34:02.000000 sendpost-1.0.2/sendpost_python_sdk/model/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3139 2023-07-26 12:33:55.000000 sendpost-1.0.2/sendpost_python_sdk/model/attachment.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4856 2023-07-26 12:33:56.000000 sendpost-1.0.2/sendpost_python_sdk/model/city.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3661 2023-07-26 12:33:56.000000 sendpost-1.0.2/sendpost_python_sdk/model/copy_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     2587 2023-07-26 12:33:57.000000 sendpost-1.0.2/sendpost_python_sdk/model/device.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    12636 2023-07-26 12:33:57.000000 sendpost-1.0.2/sendpost_python_sdk/model/email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4761 2023-07-26 12:33:58.000000 sendpost-1.0.2/sendpost_python_sdk/model/email_response.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     6066 2023-07-26 12:33:58.000000 sendpost-1.0.2/sendpost_python_sdk/model/event_metadata.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3059 2023-07-26 12:33:58.000000 sendpost-1.0.2/sendpost_python_sdk/model/model_from.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4612 2023-07-26 12:33:58.000000 sendpost-1.0.2/sendpost_python_sdk/model/os.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    20181 2023-07-26 12:33:59.000000 sendpost-1.0.2/sendpost_python_sdk/model/q_email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     9817 2023-07-26 12:33:59.000000 sendpost-1.0.2/sendpost_python_sdk/model/q_event.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3055 2023-07-26 12:34:00.000000 sendpost-1.0.2/sendpost_python_sdk/model/reply_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     6319 2023-07-26 12:34:00.000000 sendpost-1.0.2/sendpost_python_sdk/model/to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4069 2023-07-26 12:34:00.000000 sendpost-1.0.2/sendpost_python_sdk/model/user_agent.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3347 2023-07-26 12:34:00.000000 sendpost-1.0.2/sendpost_python_sdk/model/webhook_event.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost_python_sdk/models/
+-rw-r--r--   0 arseniy    (501) staff       (20)     1252 2023-07-26 12:34:02.000000 sendpost-1.0.2/sendpost_python_sdk/models/__init__.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost_python_sdk/paths/
+-rw-r--r--   0 arseniy    (501) staff       (20)      401 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/paths/__init__.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost_python_sdk/paths/subaccount_email_/
+-rw-r--r--   0 arseniy    (501) staff       (20)      331 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/paths/subaccount_email_/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15448 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/paths/subaccount_email_/post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/sendpost_python_sdk/paths/subaccount_email_template/
+-rw-r--r--   0 arseniy    (501) staff       (20)      347 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/paths/subaccount_email_template/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15628 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/paths/subaccount_email_template/post.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    10860 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/rest.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    97848 2023-07-26 12:34:01.000000 sendpost-1.0.2/sendpost_python_sdk/schemas.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      110 2023-07-26 13:36:43.000000 sendpost-1.0.2/setup.cfg
+-rw-r--r--   0 arseniy    (501) staff       (20)     1631 2023-07-26 13:34:49.000000 sendpost-1.0.2/setup.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/test/
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/test/test_models/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost-1.0.2/test/test_models/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      748 2023-07-26 12:33:55.000000 sendpost-1.0.2/test/test_models/test_attachment.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      724 2023-07-26 12:33:56.000000 sendpost-1.0.2/test/test_models/test_city.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 12:33:56.000000 sendpost-1.0.2/test/test_models/test_copy_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      732 2023-07-26 12:33:57.000000 sendpost-1.0.2/test/test_models/test_device.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-07-26 12:33:57.000000 sendpost-1.0.2/test/test_models/test_email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-07-26 12:33:58.000000 sendpost-1.0.2/test/test_models/test_email_response.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-07-26 12:33:58.000000 sendpost-1.0.2/test/test_models/test_event_metadata.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 12:33:58.000000 sendpost-1.0.2/test/test_models/test_model_from.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      716 2023-07-26 12:33:58.000000 sendpost-1.0.2/test/test_models/test_os.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      762 2023-07-26 12:33:59.000000 sendpost-1.0.2/test/test_models/test_q_email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 12:34:00.000000 sendpost-1.0.2/test/test_models/test_q_event.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      737 2023-07-26 12:34:00.000000 sendpost-1.0.2/test/test_models/test_reply_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      716 2023-07-26 12:34:00.000000 sendpost-1.0.2/test/test_models/test_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 12:34:00.000000 sendpost-1.0.2/test/test_models/test_user_agent.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-07-26 12:34:00.000000 sendpost-1.0.2/test/test_models/test_webhook_event.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/test/test_paths/
+-rw-r--r--   0 arseniy    (501) staff       (20)     1995 2023-07-26 12:34:01.000000 sendpost-1.0.2/test/test_paths/__init__.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/test/test_paths/test_subaccount_email_/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost-1.0.2/test/test_paths/test_subaccount_email_/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      802 2023-07-26 12:34:01.000000 sendpost-1.0.2/test/test_paths/test_subaccount_email_/test_post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:36:43.000000 sendpost-1.0.2/test/test_paths/test_subaccount_email_template/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost-1.0.2/test/test_paths/test_subaccount_email_template/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      826 2023-07-26 12:34:01.000000 sendpost-1.0.2/test/test_paths/test_subaccount_email_template/test_post.py
```

### Comparing `sendpost-1.0.1/PKG-INFO` & `sendpost-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.2
 Name: sendpost
-Version: 1.0.1
+Version: 1.0.2
 Summary: SendPost API
-Home-page: https://github.com/sednpost/sendpost_python_sdk
+Home-page: https://github.com/sendpost/sendpost_python_sdk
 Author: Sendpost
 Author-email: dev@sendpost.io
 License: UNKNOWN
-Download-URL: https://github.com/sednpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/sendpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz
 Description:     Email API and SMTP relay to not just send and measure email sending, but also alert and optimise. We provide you with tools, expertise and support needed to reliably deliver emails to your customers inboxes on time, every time.  # noqa: E501
             
 Keywords: OpenAPI,OpenAPI-Generator,SendPost API
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `sendpost-1.0.1/README.md` & `sendpost-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost.egg-info/PKG-INFO` & `sendpost-1.0.2/sendpost.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 1.2
 Name: sendpost
-Version: 1.0.1
+Version: 1.0.2
 Summary: SendPost API
-Home-page: https://github.com/sednpost/sendpost_python_sdk
+Home-page: https://github.com/sendpost/sendpost_python_sdk
 Author: Sendpost
 Author-email: dev@sendpost.io
 License: UNKNOWN
-Download-URL: https://github.com/sednpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz
+Download-URL: https://github.com/sendpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz
 Description:     Email API and SMTP relay to not just send and measure email sending, but also alert and optimise. We provide you with tools, expertise and support needed to reliably deliver emails to your customers inboxes on time, every time.  # noqa: E501
             
 Keywords: OpenAPI,OpenAPI-Generator,SendPost API
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `sendpost-1.0.1/sendpost.egg-info/SOURCES.txt` & `sendpost-1.0.2/sendpost.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/__init__.py` & `sendpost-1.0.2/sendpost_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/api_client.py` & `sendpost-1.0.2/sendpost_python_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/apis/path_to_api.py` & `sendpost-1.0.2/sendpost_python_sdk/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/apis/tags/email_api.py` & `sendpost-1.0.2/sendpost_python_sdk/apis/tags/email_api.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/configuration.py` & `sendpost-1.0.2/sendpost_python_sdk/configuration.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/exceptions.py` & `sendpost-1.0.2/sendpost_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/attachment.py` & `sendpost-1.0.2/sendpost_python_sdk/model/attachment.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/city.py` & `sendpost-1.0.2/sendpost_python_sdk/model/city.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/copy_to.py` & `sendpost-1.0.2/sendpost_python_sdk/model/copy_to.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/device.py` & `sendpost-1.0.2/sendpost_python_sdk/model/device.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/email_message.py` & `sendpost-1.0.2/sendpost_python_sdk/model/email_message.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/email_response.py` & `sendpost-1.0.2/sendpost_python_sdk/model/email_response.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/event_metadata.py` & `sendpost-1.0.2/sendpost_python_sdk/model/event_metadata.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/model_from.py` & `sendpost-1.0.2/sendpost_python_sdk/model/model_from.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/os.py` & `sendpost-1.0.2/sendpost_python_sdk/model/os.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/q_email_message.py` & `sendpost-1.0.2/sendpost_python_sdk/model/q_email_message.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/q_event.py` & `sendpost-1.0.2/sendpost_python_sdk/model/q_event.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/reply_to.py` & `sendpost-1.0.2/sendpost_python_sdk/model/reply_to.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/to.py` & `sendpost-1.0.2/sendpost_python_sdk/model/to.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/user_agent.py` & `sendpost-1.0.2/sendpost_python_sdk/model/user_agent.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/model/webhook_event.py` & `sendpost-1.0.2/sendpost_python_sdk/model/webhook_event.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/models/__init__.py` & `sendpost-1.0.2/sendpost_python_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_/post.py` & `sendpost-1.0.2/sendpost_python_sdk/paths/subaccount_email_/post.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_template/post.py` & `sendpost-1.0.2/sendpost_python_sdk/paths/subaccount_email_template/post.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/rest.py` & `sendpost-1.0.2/sendpost_python_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/sendpost_python_sdk/schemas.py` & `sendpost-1.0.2/sendpost_python_sdk/schemas.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/setup.py` & `sendpost-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "sendpost"
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -30,16 +30,16 @@
     "urllib3 ~= 1.26.7",
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="SendPost API",
-    url = 'https://github.com/sednpost/sendpost_python_sdk',
-    download_url = 'https://github.com/sednpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz',
+    url = 'https://github.com/sendpost/sendpost_python_sdk',
+    download_url = 'https://github.com/sendpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz',
     author="Sendpost",
     author_email="dev@sendpost.io",
     keywords=["OpenAPI", "OpenAPI-Generator", "SendPost API"],
     python_requires=">=3.7",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
```

### Comparing `sendpost-1.0.1/test/test_models/test_attachment.py` & `sendpost-1.0.2/test/test_models/test_attachment.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_city.py` & `sendpost-1.0.2/test/test_models/test_city.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_copy_to.py` & `sendpost-1.0.2/test/test_models/test_copy_to.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_device.py` & `sendpost-1.0.2/test/test_models/test_device.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_email_message.py` & `sendpost-1.0.2/test/test_models/test_email_message.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_email_response.py` & `sendpost-1.0.2/test/test_models/test_email_response.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_event_metadata.py` & `sendpost-1.0.2/test/test_models/test_event_metadata.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_model_from.py` & `sendpost-1.0.2/test/test_models/test_model_from.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_os.py` & `sendpost-1.0.2/test/test_models/test_os.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_q_email_message.py` & `sendpost-1.0.2/test/test_models/test_q_email_message.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_q_event.py` & `sendpost-1.0.2/test/test_models/test_q_event.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_reply_to.py` & `sendpost-1.0.2/test/test_models/test_reply_to.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_to.py` & `sendpost-1.0.2/test/test_models/test_to.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_user_agent.py` & `sendpost-1.0.2/test/test_models/test_user_agent.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_models/test_webhook_event.py` & `sendpost-1.0.2/test/test_models/test_webhook_event.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_paths/__init__.py` & `sendpost-1.0.2/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_paths/test_subaccount_email_/test_post.py` & `sendpost-1.0.2/test/test_paths/test_subaccount_email_/test_post.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.1/test/test_paths/test_subaccount_email_template/test_post.py` & `sendpost-1.0.2/test/test_paths/test_subaccount_email_template/test_post.py`

 * *Files identical despite different names*

