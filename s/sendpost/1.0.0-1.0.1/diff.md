# Comparing `tmp/sendpost-1.0.0.tar.gz` & `tmp/sendpost-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sendpost-1.0.0.tar", last modified: Wed Jul 26 08:26:24 2023, max compression
+gzip compressed data, was "dist/sendpost-1.0.1.tar", last modified: Wed Jul 26 13:29:21 2023, max compression
```

## Comparing `sendpost-1.0.0.tar` & `sendpost-1.0.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:24.000000 sendpost-1.0.0/
--rw-r--r--   0 arseniy    (501) staff       (20)      540 2023-07-26 08:26:24.000000 sendpost-1.0.0/PKG-INFO
--rw-r--r--   0 arseniy    (501) staff       (20)     3149 2023-07-26 08:19:43.000000 sendpost-1.0.0/README.md
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:23.000000 sendpost-1.0.0/sendpost.egg-info/
--rw-r--r--   0 arseniy    (501) staff       (20)      540 2023-07-26 08:26:23.000000 sendpost-1.0.0/sendpost.egg-info/PKG-INFO
--rw-r--r--   0 arseniy    (501) staff       (20)     2331 2023-07-26 08:26:23.000000 sendpost-1.0.0/sendpost.egg-info/SOURCES.txt
--rw-r--r--   0 arseniy    (501) staff       (20)        1 2023-07-26 08:26:23.000000 sendpost-1.0.0/sendpost.egg-info/dependency_links.txt
--rw-r--r--   0 arseniy    (501) staff       (20)      118 2023-07-26 08:26:23.000000 sendpost-1.0.0/sendpost.egg-info/requires.txt
--rw-r--r--   0 arseniy    (501) staff       (20)       21 2023-07-26 08:26:23.000000 sendpost-1.0.0/sendpost.egg-info/top_level.txt
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:23.000000 sendpost-1.0.0/sendpost_py_sdk/
--rw-r--r--   0 arseniy    (501) staff       (20)      947 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)    58843 2023-07-26 08:21:39.000000 sendpost-1.0.0/sendpost_py_sdk/api_client.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:23.000000 sendpost-1.0.0/sendpost_py_sdk/apis/
--rw-r--r--   0 arseniy    (501) staff       (20)      214 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/apis/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      598 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/apis/path_to_api.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:23.000000 sendpost-1.0.0/sendpost_py_sdk/apis/paths/
--rw-r--r--   0 arseniy    (501) staff       (20)      242 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/apis/paths/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      121 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/apis/paths/subaccount_email_.py
--rw-r--r--   0 arseniy    (501) staff       (20)      137 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/apis/paths/subaccount_email_template.py
--rw-r--r--   0 arseniy    (501) staff       (20)      310 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/apis/tag_to_api.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:23.000000 sendpost-1.0.0/sendpost_py_sdk/apis/tags/
--rw-r--r--   0 arseniy    (501) staff       (20)      308 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/apis/tags/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      792 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/apis/tags/email_api.py
--rw-r--r--   0 arseniy    (501) staff       (20)    15560 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/configuration.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4702 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/exceptions.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:24.000000 sendpost-1.0.0/sendpost_py_sdk/model/
--rw-r--r--   0 arseniy    (501) staff       (20)      349 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/model/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3135 2023-07-26 08:15:56.000000 sendpost-1.0.0/sendpost_py_sdk/model/attachment.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4852 2023-07-26 08:15:57.000000 sendpost-1.0.0/sendpost_py_sdk/model/city.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3657 2023-07-26 08:15:57.000000 sendpost-1.0.0/sendpost_py_sdk/model/copy_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)     2583 2023-07-26 08:15:57.000000 sendpost-1.0.0/sendpost_py_sdk/model/device.py
--rw-r--r--   0 arseniy    (501) staff       (20)    12616 2023-07-26 08:15:58.000000 sendpost-1.0.0/sendpost_py_sdk/model/email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4757 2023-07-26 08:15:59.000000 sendpost-1.0.0/sendpost_py_sdk/model/email_response.py
--rw-r--r--   0 arseniy    (501) staff       (20)     6046 2023-07-26 08:15:59.000000 sendpost-1.0.0/sendpost_py_sdk/model/event_metadata.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3055 2023-07-26 08:15:59.000000 sendpost-1.0.0/sendpost_py_sdk/model/model_from.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4608 2023-07-26 08:15:59.000000 sendpost-1.0.0/sendpost_py_sdk/model/os.py
--rw-r--r--   0 arseniy    (501) staff       (20)    20157 2023-07-26 08:16:00.000000 sendpost-1.0.0/sendpost_py_sdk/model/q_email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)     9809 2023-07-26 08:16:00.000000 sendpost-1.0.0/sendpost_py_sdk/model/q_event.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3051 2023-07-26 08:16:01.000000 sendpost-1.0.0/sendpost_py_sdk/model/reply_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)     6311 2023-07-26 08:16:01.000000 sendpost-1.0.0/sendpost_py_sdk/model/to.py
--rw-r--r--   0 arseniy    (501) staff       (20)     4065 2023-07-26 08:16:01.000000 sendpost-1.0.0/sendpost_py_sdk/model/user_agent.py
--rw-r--r--   0 arseniy    (501) staff       (20)     3335 2023-07-26 08:16:01.000000 sendpost-1.0.0/sendpost_py_sdk/model/webhook_event.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:24.000000 sendpost-1.0.0/sendpost_py_sdk/models/
--rw-r--r--   0 arseniy    (501) staff       (20)     1188 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/models/__init__.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:24.000000 sendpost-1.0.0/sendpost_py_sdk/paths/
--rw-r--r--   0 arseniy    (501) staff       (20)      397 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/paths/__init__.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:24.000000 sendpost-1.0.0/sendpost_py_sdk/paths/subaccount_email_/
--rw-r--r--   0 arseniy    (501) staff       (20)      323 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/paths/subaccount_email_/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)    15432 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/paths/subaccount_email_/post.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:24.000000 sendpost-1.0.0/sendpost_py_sdk/paths/subaccount_email_template/
--rw-r--r--   0 arseniy    (501) staff       (20)      339 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/paths/subaccount_email_template/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)    15612 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/paths/subaccount_email_template/post.py
--rw-r--r--   0 arseniy    (501) staff       (20)    10856 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/rest.py
--rw-r--r--   0 arseniy    (501) staff       (20)    97840 2023-07-26 08:16:02.000000 sendpost-1.0.0/sendpost_py_sdk/schemas.py
--rw-r--r--   0 arseniy    (501) staff       (20)      110 2023-07-26 08:26:24.000000 sendpost-1.0.0/setup.cfg
--rw-r--r--   0 arseniy    (501) staff       (20)     1502 2023-07-26 08:16:02.000000 sendpost-1.0.0/setup.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:23.000000 sendpost-1.0.0/test/
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:24.000000 sendpost-1.0.0/test/test_models/
--rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 08:16:02.000000 sendpost-1.0.0/test/test_models/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      736 2023-07-26 08:15:56.000000 sendpost-1.0.0/test/test_models/test_attachment.py
--rw-r--r--   0 arseniy    (501) staff       (20)      712 2023-07-26 08:15:57.000000 sendpost-1.0.0/test/test_models/test_city.py
--rw-r--r--   0 arseniy    (501) staff       (20)      721 2023-07-26 08:15:57.000000 sendpost-1.0.0/test/test_models/test_copy_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)      720 2023-07-26 08:15:57.000000 sendpost-1.0.0/test/test_models/test_device.py
--rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 08:15:58.000000 sendpost-1.0.0/test/test_models/test_email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)      749 2023-07-26 08:15:59.000000 sendpost-1.0.0/test/test_models/test_email_response.py
--rw-r--r--   0 arseniy    (501) staff       (20)      749 2023-07-26 08:15:59.000000 sendpost-1.0.0/test/test_models/test_event_metadata.py
--rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 08:15:59.000000 sendpost-1.0.0/test/test_models/test_model_from.py
--rw-r--r--   0 arseniy    (501) staff       (20)      704 2023-07-26 08:15:59.000000 sendpost-1.0.0/test/test_models/test_os.py
--rw-r--r--   0 arseniy    (501) staff       (20)      750 2023-07-26 08:16:00.000000 sendpost-1.0.0/test/test_models/test_q_email_message.py
--rw-r--r--   0 arseniy    (501) staff       (20)      721 2023-07-26 08:16:01.000000 sendpost-1.0.0/test/test_models/test_q_event.py
--rw-r--r--   0 arseniy    (501) staff       (20)      725 2023-07-26 08:16:01.000000 sendpost-1.0.0/test/test_models/test_reply_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)      704 2023-07-26 08:16:01.000000 sendpost-1.0.0/test/test_models/test_to.py
--rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 08:16:01.000000 sendpost-1.0.0/test/test_models/test_user_agent.py
--rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 08:16:01.000000 sendpost-1.0.0/test/test_models/test_webhook_event.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:24.000000 sendpost-1.0.0/test/test_paths/
--rw-r--r--   0 arseniy    (501) staff       (20)     1995 2023-07-26 08:16:02.000000 sendpost-1.0.0/test/test_paths/__init__.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:24.000000 sendpost-1.0.0/test/test_paths/test_subaccount_email_/
--rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 08:16:02.000000 sendpost-1.0.0/test/test_paths/test_subaccount_email_/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      790 2023-07-26 08:16:02.000000 sendpost-1.0.0/test/test_paths/test_subaccount_email_/test_post.py
-drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 08:26:24.000000 sendpost-1.0.0/test/test_paths/test_subaccount_email_template/
--rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 08:16:02.000000 sendpost-1.0.0/test/test_paths/test_subaccount_email_template/__init__.py
--rw-r--r--   0 arseniy    (501) staff       (20)      814 2023-07-26 08:16:02.000000 sendpost-1.0.0/test/test_paths/test_subaccount_email_template/test_post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/
+-rw-r--r--   0 arseniy    (501) staff       (20)      652 2023-07-26 13:29:21.000000 sendpost-1.0.1/PKG-INFO
+-rw-r--r--   0 arseniy    (501) staff       (20)     3180 2023-07-26 12:36:30.000000 sendpost-1.0.1/README.md
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost.egg-info/
+-rw-r--r--   0 arseniy    (501) staff       (20)      652 2023-07-26 13:29:20.000000 sendpost-1.0.1/sendpost.egg-info/PKG-INFO
+-rw-r--r--   0 arseniy    (501) staff       (20)     2475 2023-07-26 13:29:20.000000 sendpost-1.0.1/sendpost.egg-info/SOURCES.txt
+-rw-r--r--   0 arseniy    (501) staff       (20)        1 2023-07-26 13:29:20.000000 sendpost-1.0.1/sendpost.egg-info/dependency_links.txt
+-rw-r--r--   0 arseniy    (501) staff       (20)      118 2023-07-26 13:29:20.000000 sendpost-1.0.1/sendpost.egg-info/requires.txt
+-rw-r--r--   0 arseniy    (501) staff       (20)       25 2023-07-26 13:29:20.000000 sendpost-1.0.1/sendpost.egg-info/top_level.txt
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/
+-rw-r--r--   0 arseniy    (501) staff       (20)      979 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    58859 2023-07-26 12:39:50.000000 sendpost-1.0.1/sendpost_python_sdk/api_client.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/apis/
+-rw-r--r--   0 arseniy    (501) staff       (20)      214 2023-07-26 12:34:02.000000 sendpost-1.0.1/sendpost_python_sdk/apis/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      610 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/path_to_api.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/apis/paths/
+-rw-r--r--   0 arseniy    (501) staff       (20)      246 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/paths/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      125 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/paths/subaccount_email_.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      141 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/paths/subaccount_email_template.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      318 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/tag_to_api.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/apis/tags/
+-rw-r--r--   0 arseniy    (501) staff       (20)      312 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/tags/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      800 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/apis/tags/email_api.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15568 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/configuration.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4702 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/exceptions.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/model/
+-rw-r--r--   0 arseniy    (501) staff       (20)      353 2023-07-26 12:34:02.000000 sendpost-1.0.1/sendpost_python_sdk/model/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3139 2023-07-26 12:33:55.000000 sendpost-1.0.1/sendpost_python_sdk/model/attachment.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4856 2023-07-26 12:33:56.000000 sendpost-1.0.1/sendpost_python_sdk/model/city.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3661 2023-07-26 12:33:56.000000 sendpost-1.0.1/sendpost_python_sdk/model/copy_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     2587 2023-07-26 12:33:57.000000 sendpost-1.0.1/sendpost_python_sdk/model/device.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    12636 2023-07-26 12:33:57.000000 sendpost-1.0.1/sendpost_python_sdk/model/email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4761 2023-07-26 12:33:58.000000 sendpost-1.0.1/sendpost_python_sdk/model/email_response.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     6066 2023-07-26 12:33:58.000000 sendpost-1.0.1/sendpost_python_sdk/model/event_metadata.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3059 2023-07-26 12:33:58.000000 sendpost-1.0.1/sendpost_python_sdk/model/model_from.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4612 2023-07-26 12:33:58.000000 sendpost-1.0.1/sendpost_python_sdk/model/os.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    20181 2023-07-26 12:33:59.000000 sendpost-1.0.1/sendpost_python_sdk/model/q_email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     9817 2023-07-26 12:33:59.000000 sendpost-1.0.1/sendpost_python_sdk/model/q_event.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3055 2023-07-26 12:34:00.000000 sendpost-1.0.1/sendpost_python_sdk/model/reply_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     6319 2023-07-26 12:34:00.000000 sendpost-1.0.1/sendpost_python_sdk/model/to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     4069 2023-07-26 12:34:00.000000 sendpost-1.0.1/sendpost_python_sdk/model/user_agent.py
+-rw-r--r--   0 arseniy    (501) staff       (20)     3347 2023-07-26 12:34:00.000000 sendpost-1.0.1/sendpost_python_sdk/model/webhook_event.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/models/
+-rw-r--r--   0 arseniy    (501) staff       (20)     1252 2023-07-26 12:34:02.000000 sendpost-1.0.1/sendpost_python_sdk/models/__init__.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/paths/
+-rw-r--r--   0 arseniy    (501) staff       (20)      401 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/paths/__init__.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_/
+-rw-r--r--   0 arseniy    (501) staff       (20)      331 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15448 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_/post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_template/
+-rw-r--r--   0 arseniy    (501) staff       (20)      347 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_template/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    15628 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_template/post.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    10860 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/rest.py
+-rw-r--r--   0 arseniy    (501) staff       (20)    97848 2023-07-26 12:34:01.000000 sendpost-1.0.1/sendpost_python_sdk/schemas.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      110 2023-07-26 13:29:21.000000 sendpost-1.0.1/setup.cfg
+-rw-r--r--   0 arseniy    (501) staff       (20)     1631 2023-07-26 13:24:19.000000 sendpost-1.0.1/setup.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/test/
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/test/test_models/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_models/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      748 2023-07-26 12:33:55.000000 sendpost-1.0.1/test/test_models/test_attachment.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      724 2023-07-26 12:33:56.000000 sendpost-1.0.1/test/test_models/test_city.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 12:33:56.000000 sendpost-1.0.1/test/test_models/test_copy_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      732 2023-07-26 12:33:57.000000 sendpost-1.0.1/test/test_models/test_device.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-07-26 12:33:57.000000 sendpost-1.0.1/test/test_models/test_email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-07-26 12:33:58.000000 sendpost-1.0.1/test/test_models/test_email_response.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      761 2023-07-26 12:33:58.000000 sendpost-1.0.1/test/test_models/test_event_metadata.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 12:33:58.000000 sendpost-1.0.1/test/test_models/test_model_from.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      716 2023-07-26 12:33:58.000000 sendpost-1.0.1/test/test_models/test_os.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      762 2023-07-26 12:33:59.000000 sendpost-1.0.1/test/test_models/test_q_email_message.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      733 2023-07-26 12:34:00.000000 sendpost-1.0.1/test/test_models/test_q_event.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      737 2023-07-26 12:34:00.000000 sendpost-1.0.1/test/test_models/test_reply_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      716 2023-07-26 12:34:00.000000 sendpost-1.0.1/test/test_models/test_to.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      745 2023-07-26 12:34:00.000000 sendpost-1.0.1/test/test_models/test_user_agent.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      757 2023-07-26 12:34:00.000000 sendpost-1.0.1/test/test_models/test_webhook_event.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/test/test_paths/
+-rw-r--r--   0 arseniy    (501) staff       (20)     1995 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_paths/__init__.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      802 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_/test_post.py
+drwxr-xr-x   0 arseniy    (501) staff       (20)        0 2023-07-26 13:29:21.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_template/
+-rw-r--r--   0 arseniy    (501) staff       (20)        0 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_template/__init__.py
+-rw-r--r--   0 arseniy    (501) staff       (20)      826 2023-07-26 12:34:01.000000 sendpost-1.0.1/test/test_paths/test_subaccount_email_template/test_post.py
```

### Comparing `sendpost-1.0.0/PKG-INFO` & `sendpost-1.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 1.2
 Name: sendpost
-Version: 1.0.0
+Version: 1.0.1
 Summary: SendPost API
-Home-page: UNKNOWN
-Author: OpenAPI Generator community
-Author-email: hello@sendpost.io
+Home-page: https://github.com/sednpost/sendpost_python_sdk
+Author: Sendpost
+Author-email: dev@sendpost.io
 License: UNKNOWN
+Download-URL: https://github.com/sednpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz
 Description:     Email API and SMTP relay to not just send and measure email sending, but also alert and optimise. We provide you with tools, expertise and support needed to reliably deliver emails to your customers inboxes on time, every time.  # noqa: E501
             
 Keywords: OpenAPI,OpenAPI-Generator,SendPost API
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `sendpost-1.0.0/README.md` & `sendpost-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,49 +8,49 @@
 
 ## Installation & Usage
 ### pip install
 
 If the python package is hosted on a repository, you can install directly using:
 
 ```sh
-pip install git+https://github.com/sendpost/sendpost_py_sdk.git
+pip install git+https://github.com/sendpost/sendpost_python_sdk.git
 ```
-(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/sendpost/sendpost_py_sdk.git`)
+(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/sendpost/sendpost_python_sdk.git`)
 
 Then import the package:
 ```python
-import sendpost_py_sdk
+import sendpost_python_sdk
 ```
 
 ### Setuptools
 
 Install via [Setuptools](http://pypi.python.org/pypi/setuptools).
 
 ```sh
 python setup.py install --user
 ```
 (or `sudo python setup.py install` to install the package for all users)
 
 Then import the package:
 ```python
-import sendpost_py_sdk
+import sendpost_python_sdk
 ```
 
 ## Getting Started
 
 Please follow the [installation procedure](#installation--usage) and then run the following:
 
 ```python
 
-import sendpost_py_sdk
+import sendpost_python_sdk
 from pprint import pprint
-from sendpost_py_sdk.apis.tags import email_api
+from sendpost_python_sdk.apis.tags import email_api
 
 # Enter a context with an instance of the API client
-with sendpost_py_sdk.ApiClient() as api_client:
+with sendpost_python_sdk.ApiClient() as api_client:
     # Create an instance of the API class
     api_instance = email_api.EmailApi(api_client)
     x_sub_account_api_key = "your_api_key" # str | Sub-Account API Key
     email = {
       "from": {
             "email": "richard@piedpiper.com",
       },
@@ -62,15 +62,15 @@
       "subject": "Hello World",
       "htmlBody": "<strong>it works!</strong>",
       "ippool": "PiedPiper",
     }
     try:
         api_response = api_instance.send_email(header_params={ 'X-SubAccount-ApiKey': x_sub_account_api_key}, body=email)
         pprint(api_response)
-    except sendpost_py_sdk.ApiException as e:
+    except sendpost_python_sdk.ApiException as e:
         print("Exception when calling EmailApi->send_email: %s\n" % e)
 ```
 
 ## Documentation for API Endpoints
 
 All URIs are relative to *https://api.sendpost.io/api/v1*
 
@@ -102,8 +102,8 @@
  Endpoints do not require authorization.
 
 
 ## Author
 
 dev@sendpost.io
 
-```
+```
```

### Comparing `sendpost-1.0.0/sendpost.egg-info/PKG-INFO` & `sendpost-1.0.1/sendpost.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 1.2
 Name: sendpost
-Version: 1.0.0
+Version: 1.0.1
 Summary: SendPost API
-Home-page: UNKNOWN
-Author: OpenAPI Generator community
-Author-email: hello@sendpost.io
+Home-page: https://github.com/sednpost/sendpost_python_sdk
+Author: Sendpost
+Author-email: dev@sendpost.io
 License: UNKNOWN
+Download-URL: https://github.com/sednpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz
 Description:     Email API and SMTP relay to not just send and measure email sending, but also alert and optimise. We provide you with tools, expertise and support needed to reliably deliver emails to your customers inboxes on time, every time.  # noqa: E501
             
 Keywords: OpenAPI,OpenAPI-Generator,SendPost API
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `sendpost-1.0.0/sendpost.egg-info/SOURCES.txt` & `sendpost-1.0.1/sendpost.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 setup.cfg
 setup.py
 sendpost.egg-info/PKG-INFO
 sendpost.egg-info/SOURCES.txt
 sendpost.egg-info/dependency_links.txt
 sendpost.egg-info/requires.txt
 sendpost.egg-info/top_level.txt
-sendpost_py_sdk/__init__.py
-sendpost_py_sdk/api_client.py
-sendpost_py_sdk/configuration.py
-sendpost_py_sdk/exceptions.py
-sendpost_py_sdk/rest.py
-sendpost_py_sdk/schemas.py
-sendpost_py_sdk/apis/__init__.py
-sendpost_py_sdk/apis/path_to_api.py
-sendpost_py_sdk/apis/tag_to_api.py
-sendpost_py_sdk/apis/paths/__init__.py
-sendpost_py_sdk/apis/paths/subaccount_email_.py
-sendpost_py_sdk/apis/paths/subaccount_email_template.py
-sendpost_py_sdk/apis/tags/__init__.py
-sendpost_py_sdk/apis/tags/email_api.py
-sendpost_py_sdk/model/__init__.py
-sendpost_py_sdk/model/attachment.py
-sendpost_py_sdk/model/city.py
-sendpost_py_sdk/model/copy_to.py
-sendpost_py_sdk/model/device.py
-sendpost_py_sdk/model/email_message.py
-sendpost_py_sdk/model/email_response.py
-sendpost_py_sdk/model/event_metadata.py
-sendpost_py_sdk/model/model_from.py
-sendpost_py_sdk/model/os.py
-sendpost_py_sdk/model/q_email_message.py
-sendpost_py_sdk/model/q_event.py
-sendpost_py_sdk/model/reply_to.py
-sendpost_py_sdk/model/to.py
-sendpost_py_sdk/model/user_agent.py
-sendpost_py_sdk/model/webhook_event.py
-sendpost_py_sdk/models/__init__.py
-sendpost_py_sdk/paths/__init__.py
-sendpost_py_sdk/paths/subaccount_email_/__init__.py
-sendpost_py_sdk/paths/subaccount_email_/post.py
-sendpost_py_sdk/paths/subaccount_email_template/__init__.py
-sendpost_py_sdk/paths/subaccount_email_template/post.py
+sendpost_python_sdk/__init__.py
+sendpost_python_sdk/api_client.py
+sendpost_python_sdk/configuration.py
+sendpost_python_sdk/exceptions.py
+sendpost_python_sdk/rest.py
+sendpost_python_sdk/schemas.py
+sendpost_python_sdk/apis/__init__.py
+sendpost_python_sdk/apis/path_to_api.py
+sendpost_python_sdk/apis/tag_to_api.py
+sendpost_python_sdk/apis/paths/__init__.py
+sendpost_python_sdk/apis/paths/subaccount_email_.py
+sendpost_python_sdk/apis/paths/subaccount_email_template.py
+sendpost_python_sdk/apis/tags/__init__.py
+sendpost_python_sdk/apis/tags/email_api.py
+sendpost_python_sdk/model/__init__.py
+sendpost_python_sdk/model/attachment.py
+sendpost_python_sdk/model/city.py
+sendpost_python_sdk/model/copy_to.py
+sendpost_python_sdk/model/device.py
+sendpost_python_sdk/model/email_message.py
+sendpost_python_sdk/model/email_response.py
+sendpost_python_sdk/model/event_metadata.py
+sendpost_python_sdk/model/model_from.py
+sendpost_python_sdk/model/os.py
+sendpost_python_sdk/model/q_email_message.py
+sendpost_python_sdk/model/q_event.py
+sendpost_python_sdk/model/reply_to.py
+sendpost_python_sdk/model/to.py
+sendpost_python_sdk/model/user_agent.py
+sendpost_python_sdk/model/webhook_event.py
+sendpost_python_sdk/models/__init__.py
+sendpost_python_sdk/paths/__init__.py
+sendpost_python_sdk/paths/subaccount_email_/__init__.py
+sendpost_python_sdk/paths/subaccount_email_/post.py
+sendpost_python_sdk/paths/subaccount_email_template/__init__.py
+sendpost_python_sdk/paths/subaccount_email_template/post.py
 test/test_models/__init__.py
 test/test_models/test_attachment.py
 test/test_models/test_city.py
 test/test_models/test_copy_to.py
 test/test_models/test_device.py
 test/test_models/test_email_message.py
 test/test_models/test_email_response.py
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/__init__.py` & `sendpost-1.0.1/sendpost_python_sdk/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,19 +11,19 @@
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 __version__ = "1.0.0"
 
 # import ApiClient
-from sendpost_py_sdk.api_client import ApiClient
+from sendpost_python_sdk.api_client import ApiClient
 
 # import Configuration
-from sendpost_py_sdk.configuration import Configuration
+from sendpost_python_sdk.configuration import Configuration
 
 # import exceptions
-from sendpost_py_sdk.exceptions import OpenApiException
-from sendpost_py_sdk.exceptions import ApiAttributeError
-from sendpost_py_sdk.exceptions import ApiTypeError
-from sendpost_py_sdk.exceptions import ApiValueError
-from sendpost_py_sdk.exceptions import ApiKeyError
-from sendpost_py_sdk.exceptions import ApiException
+from sendpost_python_sdk.exceptions import OpenApiException
+from sendpost_python_sdk.exceptions import ApiAttributeError
+from sendpost_python_sdk.exceptions import ApiTypeError
+from sendpost_python_sdk.exceptions import ApiValueError
+from sendpost_python_sdk.exceptions import ApiKeyError
+from sendpost_python_sdk.exceptions import ApiException
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/api_client.py` & `sendpost-1.0.1/sendpost_python_sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,18 @@
 import urllib3
 from urllib3._collections import HTTPHeaderDict
 from urllib.parse import urlparse, quote
 from urllib3.fields import RequestField as RequestFieldBase
 
 import frozendict
 
-from sendpost_py_sdk import rest
-from sendpost_py_sdk.configuration import Configuration
-from sendpost_py_sdk.exceptions import ApiTypeError, ApiValueError
-from sendpost_py_sdk.schemas import (
+from sendpost_python_sdk import rest
+from sendpost_python_sdk.configuration import Configuration
+from sendpost_python_sdk.exceptions import ApiTypeError, ApiValueError
+from sendpost_python_sdk.schemas import (
     NoneClass,
     BoolClass,
     Schema,
     FileIO,
     BinarySchema,
     date,
     datetime,
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/apis/path_to_api.py` & `sendpost-1.0.1/sendpost_python_sdk/apis/path_to_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typing_extensions
 
-from sendpost_py_sdk.paths import PathValues
-from sendpost_py_sdk.apis.paths.subaccount_email_ import SubaccountEmail
-from sendpost_py_sdk.apis.paths.subaccount_email_template import SubaccountEmailTemplate
+from sendpost_python_sdk.paths import PathValues
+from sendpost_python_sdk.apis.paths.subaccount_email_ import SubaccountEmail
+from sendpost_python_sdk.apis.paths.subaccount_email_template import SubaccountEmailTemplate
 
 PathToApi = typing_extensions.TypedDict(
     'PathToApi',
     {
         PathValues.SUBACCOUNT_EMAIL_: SubaccountEmail,
         PathValues.SUBACCOUNT_EMAIL_TEMPLATE: SubaccountEmailTemplate,
     }
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/apis/tags/email_api.py` & `sendpost-1.0.1/sendpost_python_sdk/apis/tags/email_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     Email API and SMTP relay to not just send and measure email sending, but also alert and optimise. We provide you with tools, expertise and support needed to reliably deliver emails to your customers inboxes on time, every time.  # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
-from sendpost_py_sdk.paths.subaccount_email_.post import SendEmail
-from sendpost_py_sdk.paths.subaccount_email_template.post import SendEmailWithTemplate
+from sendpost_python_sdk.paths.subaccount_email_.post import SendEmail
+from sendpost_python_sdk.paths.subaccount_email_template.post import SendEmailWithTemplate
 
 
 class EmailApi(
     SendEmail,
     SendEmailWithTemplate,
 ):
     """NOTE: This class is auto generated by OpenAPI Generator
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/configuration.py` & `sendpost-1.0.1/sendpost_python_sdk/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import copy
 import logging
 import multiprocessing
 import sys
 import urllib3
 
 from http import client as http_client
-from sendpost_py_sdk.exceptions import ApiValueError
+from sendpost_python_sdk.exceptions import ApiValueError
 
 
 JSON_SCHEMA_VALIDATION_KEYWORDS = {
     'multipleOf', 'maximum', 'exclusiveMaximum',
     'minimum', 'exclusiveMinimum', 'maxLength',
     'minLength', 'pattern', 'maxItems', 'minItems',
     'uniqueItems', 'maxProperties', 'minProperties',
@@ -108,15 +108,15 @@
         """Temp file folder for downloading files
         """
         # Authentication Settings
         self.disabled_client_side_validations = disabled_client_side_validations
         self.logger = {}
         """Logging Settings
         """
-        self.logger["package_logger"] = logging.getLogger("sendpost_py_sdk")
+        self.logger["package_logger"] = logging.getLogger("sendpost_python_sdk")
         self.logger["urllib3_logger"] = logging.getLogger("urllib3")
         self.logger_format = '%(asctime)s %(levelname)s %(message)s'
         """Log format
         """
         self.logger_stream_handler = None
         """Log stream handler
         """
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/exceptions.py` & `sendpost-1.0.1/sendpost_python_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/attachment.py` & `sendpost-1.0.1/sendpost_python_sdk/model/attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class Attachment(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/city.py` & `sendpost-1.0.1/sendpost_python_sdk/model/city.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class City(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/copy_to.py` & `sendpost-1.0.1/sendpost_python_sdk/model/copy_to.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class CopyTo(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/device.py` & `sendpost-1.0.1/sendpost_python_sdk/model/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class Device(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/email_message.py` & `sendpost-1.0.1/sendpost_python_sdk/model/email_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class EmailMessage(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -290,11 +290,11 @@
             trackOpens=trackOpens,
             headers=headers,
             ampBody=ampBody,
             _configuration=_configuration,
             **kwargs,
         )
 
-from sendpost_py_sdk.model.attachment import Attachment
-from sendpost_py_sdk.model.model_from import ModelFrom
-from sendpost_py_sdk.model.reply_to import ReplyTo
-from sendpost_py_sdk.model.to import To
+from sendpost_python_sdk.model.attachment import Attachment
+from sendpost_python_sdk.model.model_from import ModelFrom
+from sendpost_python_sdk.model.reply_to import ReplyTo
+from sendpost_python_sdk.model.to import To
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/email_response.py` & `sendpost-1.0.1/sendpost_python_sdk/model/email_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class EmailResponse(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/event_metadata.py` & `sendpost-1.0.1/sendpost_python_sdk/model/event_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class EventMetadata(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -146,11 +146,11 @@
             smtpCode=smtpCode,
             smtpDescription=smtpDescription,
             userAgent=userAgent,
             _configuration=_configuration,
             **kwargs,
         )
 
-from sendpost_py_sdk.model.city import City
-from sendpost_py_sdk.model.device import Device
-from sendpost_py_sdk.model.os import Os
-from sendpost_py_sdk.model.user_agent import UserAgent
+from sendpost_python_sdk.model.city import City
+from sendpost_python_sdk.model.device import Device
+from sendpost_python_sdk.model.os import Os
+from sendpost_python_sdk.model.user_agent import UserAgent
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/model_from.py` & `sendpost-1.0.1/sendpost_python_sdk/model/model_from.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class ModelFrom(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/os.py` & `sendpost-1.0.1/sendpost_python_sdk/model/os.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class Os(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/q_email_message.py` & `sendpost-1.0.1/sendpost_python_sdk/model/q_email_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class QEmailMessage(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -441,12 +441,12 @@
             to=to,
             trackClicks=trackClicks,
             trackOpens=trackOpens,
             _configuration=_configuration,
             **kwargs,
         )
 
-from sendpost_py_sdk.model.attachment import Attachment
-from sendpost_py_sdk.model.copy_to import CopyTo
-from sendpost_py_sdk.model.model_from import ModelFrom
-from sendpost_py_sdk.model.reply_to import ReplyTo
-from sendpost_py_sdk.model.to import To
+from sendpost_python_sdk.model.attachment import Attachment
+from sendpost_python_sdk.model.copy_to import CopyTo
+from sendpost_python_sdk.model.model_from import ModelFrom
+from sendpost_python_sdk.model.reply_to import ReplyTo
+from sendpost_python_sdk.model.to import To
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/q_event.py` & `sendpost-1.0.1/sendpost_python_sdk/model/q_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class QEvent(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -217,8 +217,8 @@
             to=to,
             tpspId=tpspId,
             type=type,
             _configuration=_configuration,
             **kwargs,
         )
 
-from sendpost_py_sdk.model.event_metadata import EventMetadata
+from sendpost_python_sdk.model.event_metadata import EventMetadata
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/reply_to.py` & `sendpost-1.0.1/sendpost_python_sdk/model/reply_to.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class ReplyTo(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/to.py` & `sendpost-1.0.1/sendpost_python_sdk/model/to.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class To(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -164,8 +164,8 @@
             cc=cc,
             bcc=bcc,
             customFields=customFields,
             _configuration=_configuration,
             **kwargs,
         )
 
-from sendpost_py_sdk.model.copy_to import CopyTo
+from sendpost_python_sdk.model.copy_to import CopyTo
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/user_agent.py` & `sendpost-1.0.1/sendpost_python_sdk/model/user_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class UserAgent(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/model/webhook_event.py` & `sendpost-1.0.1/sendpost_python_sdk/model/webhook_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
 
 class WebhookEvent(
     schemas.DictSchema
 ):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
@@ -90,9 +90,9 @@
             *_args,
             event=event,
             emailMessage=emailMessage,
             _configuration=_configuration,
             **kwargs,
         )
 
-from sendpost_py_sdk.model.q_email_message import QEmailMessage
-from sendpost_py_sdk.model.q_event import QEvent
+from sendpost_python_sdk.model.q_email_message import QEmailMessage
+from sendpost_python_sdk.model.q_event import QEvent
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/models/__init__.py` & `sendpost-1.0.1/sendpost_python_sdk/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 # flake8: noqa
 
 # import all models into this package
 # if you have many models here with many references from one model to another this may
 # raise a RecursionError
 # to avoid this, import only the models that you directly need like:
-# from sendpost_py_sdk.model.pet import Pet
+# from sendpost_python_sdk.model.pet import Pet
 # or import this package, but before doing it, use:
 # import sys
 # sys.setrecursionlimit(n)
 
-from sendpost_py_sdk.model.attachment import Attachment
-from sendpost_py_sdk.model.city import City
-from sendpost_py_sdk.model.copy_to import CopyTo
-from sendpost_py_sdk.model.device import Device
-from sendpost_py_sdk.model.email_message import EmailMessage
-from sendpost_py_sdk.model.email_response import EmailResponse
-from sendpost_py_sdk.model.event_metadata import EventMetadata
-from sendpost_py_sdk.model.model_from import ModelFrom
-from sendpost_py_sdk.model.os import Os
-from sendpost_py_sdk.model.q_email_message import QEmailMessage
-from sendpost_py_sdk.model.q_event import QEvent
-from sendpost_py_sdk.model.reply_to import ReplyTo
-from sendpost_py_sdk.model.to import To
-from sendpost_py_sdk.model.user_agent import UserAgent
-from sendpost_py_sdk.model.webhook_event import WebhookEvent
+from sendpost_python_sdk.model.attachment import Attachment
+from sendpost_python_sdk.model.city import City
+from sendpost_python_sdk.model.copy_to import CopyTo
+from sendpost_python_sdk.model.device import Device
+from sendpost_python_sdk.model.email_message import EmailMessage
+from sendpost_python_sdk.model.email_response import EmailResponse
+from sendpost_python_sdk.model.event_metadata import EventMetadata
+from sendpost_python_sdk.model.model_from import ModelFrom
+from sendpost_python_sdk.model.os import Os
+from sendpost_python_sdk.model.q_email_message import QEmailMessage
+from sendpost_python_sdk.model.q_event import QEvent
+from sendpost_python_sdk.model.reply_to import ReplyTo
+from sendpost_python_sdk.model.to import To
+from sendpost_python_sdk.model.user_agent import UserAgent
+from sendpost_python_sdk.model.webhook_event import WebhookEvent
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/paths/subaccount_email_/post.py` & `sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_/post.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 from urllib3._collections import HTTPHeaderDict
 
-from sendpost_py_sdk import api_client, exceptions
+from sendpost_python_sdk import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
-from sendpost_py_sdk.model.email_response import EmailResponse
-from sendpost_py_sdk.model.email_message import EmailMessage
+from sendpost_python_sdk.model.email_response import EmailResponse
+from sendpost_python_sdk.model.email_message import EmailMessage
 
 from . import path
 
 # Header params
 XSubAccountApiKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/paths/subaccount_email_template/post.py` & `sendpost-1.0.1/sendpost_python_sdk/paths/subaccount_email_template/post.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 """
 
 from dataclasses import dataclass
 import typing_extensions
 import urllib3
 from urllib3._collections import HTTPHeaderDict
 
-from sendpost_py_sdk import api_client, exceptions
+from sendpost_python_sdk import api_client, exceptions
 from datetime import date, datetime  # noqa: F401
 import decimal  # noqa: F401
 import functools  # noqa: F401
 import io  # noqa: F401
 import re  # noqa: F401
 import typing  # noqa: F401
 import typing_extensions  # noqa: F401
 import uuid  # noqa: F401
 
 import frozendict  # noqa: F401
 
-from sendpost_py_sdk import schemas  # noqa: F401
+from sendpost_python_sdk import schemas  # noqa: F401
 
-from sendpost_py_sdk.model.email_response import EmailResponse
-from sendpost_py_sdk.model.email_message import EmailMessage
+from sendpost_python_sdk.model.email_response import EmailResponse
+from sendpost_python_sdk.model.email_message import EmailMessage
 
 from . import path
 
 # Header params
 XSubAccountApiKeySchema = schemas.StrSchema
 RequestRequiredHeaderParams = typing_extensions.TypedDict(
     'RequestRequiredHeaderParams',
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/rest.py` & `sendpost-1.0.1/sendpost_python_sdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from urllib.parse import urlencode
 import typing
 
 import certifi
 import urllib3
 from urllib3._collections import HTTPHeaderDict
 
-from sendpost_py_sdk.exceptions import ApiException, ApiValueError
+from sendpost_python_sdk.exceptions import ApiException, ApiValueError
 
 
 logger = logging.getLogger(__name__)
 
 
 class RESTClientObject(object):
```

### Comparing `sendpost-1.0.0/sendpost_py_sdk/schemas.py` & `sendpost-1.0.1/sendpost_python_sdk/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 import types
 import typing
 import uuid
 
 from dateutil.parser.isoparser import isoparser, _takes_ascii
 import frozendict
 
-from sendpost_py_sdk.exceptions import (
+from sendpost_python_sdk.exceptions import (
     ApiTypeError,
     ApiValueError,
 )
-from sendpost_py_sdk.configuration import (
+from sendpost_python_sdk.configuration import (
     Configuration,
 )
 
 
 class Unset(object):
     """
     An instance of this class is set as the default value for object type(dict) properties that are optional
```

### Comparing `sendpost-1.0.0/setup.py` & `sendpost-1.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "sendpost"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -30,17 +30,18 @@
     "urllib3 ~= 1.26.7",
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="SendPost API",
-    author="OpenAPI Generator community",
-    author_email="hello@sendpost.io",
-    url="",
+    url = 'https://github.com/sednpost/sendpost_python_sdk',
+    download_url = 'https://github.com/sednpost/sendpost_python_sdk/archive/refs/tags/1.0.0.tar.gz',
+    author="Sendpost",
+    author_email="dev@sendpost.io",
     keywords=["OpenAPI", "OpenAPI-Generator", "SendPost API"],
     python_requires=">=3.7",
     install_requires=REQUIRES,
     packages=find_packages(exclude=["test", "tests"]),
     include_package_data=True,
     long_description="""\
     Email API and SMTP relay to not just send and measure email sending, but also alert and optimise. We provide you with tools, expertise and support needed to reliably deliver emails to your customers inboxes on time, every time.  # noqa: E501
```

### Comparing `sendpost-1.0.0/test/test_models/test_attachment.py` & `sendpost-1.0.1/test/test_models/test_email_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.attachment import Attachment
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.email_response import EmailResponse
+from sendpost_python_sdk import configuration
 
 
-class TestAttachment(unittest.TestCase):
-    """Attachment unit test stubs"""
+class TestEmailResponse(unittest.TestCase):
+    """EmailResponse unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sendpost-1.0.0/test/test_models/test_city.py` & `sendpost-1.0.1/test/test_models/test_city.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.city import City
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.city import City
+from sendpost_python_sdk import configuration
 
 
 class TestCity(unittest.TestCase):
     """City unit test stubs"""
     _configuration = configuration.Configuration()
```

### Comparing `sendpost-1.0.0/test/test_models/test_copy_to.py` & `sendpost-1.0.1/test/test_models/test_to.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.copy_to import CopyTo
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.to import To
+from sendpost_python_sdk import configuration
 
 
-class TestCopyTo(unittest.TestCase):
-    """CopyTo unit test stubs"""
+class TestTo(unittest.TestCase):
+    """To unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sendpost-1.0.0/test/test_models/test_device.py` & `sendpost-1.0.1/test/test_models/test_device.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.device import Device
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.device import Device
+from sendpost_python_sdk import configuration
 
 
 class TestDevice(unittest.TestCase):
     """Device unit test stubs"""
     _configuration = configuration.Configuration()
```

### Comparing `sendpost-1.0.0/test/test_models/test_email_message.py` & `sendpost-1.0.1/test/test_models/test_os.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.email_message import EmailMessage
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.os import Os
+from sendpost_python_sdk import configuration
 
 
-class TestEmailMessage(unittest.TestCase):
-    """EmailMessage unit test stubs"""
+class TestOs(unittest.TestCase):
+    """Os unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sendpost-1.0.0/test/test_models/test_email_response.py` & `sendpost-1.0.1/test/test_models/test_q_event.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.email_response import EmailResponse
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.q_event import QEvent
+from sendpost_python_sdk import configuration
 
 
-class TestEmailResponse(unittest.TestCase):
-    """EmailResponse unit test stubs"""
+class TestQEvent(unittest.TestCase):
+    """QEvent unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sendpost-1.0.0/test/test_models/test_event_metadata.py` & `sendpost-1.0.1/test/test_models/test_event_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.event_metadata import EventMetadata
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.event_metadata import EventMetadata
+from sendpost_python_sdk import configuration
 
 
 class TestEventMetadata(unittest.TestCase):
     """EventMetadata unit test stubs"""
     _configuration = configuration.Configuration()
```

### Comparing `sendpost-1.0.0/test/test_models/test_model_from.py` & `sendpost-1.0.1/test/test_models/test_copy_to.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.model_from import ModelFrom
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.copy_to import CopyTo
+from sendpost_python_sdk import configuration
 
 
-class TestModelFrom(unittest.TestCase):
-    """ModelFrom unit test stubs"""
+class TestCopyTo(unittest.TestCase):
+    """CopyTo unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sendpost-1.0.0/test/test_models/test_os.py` & `sendpost-1.0.1/test/test_models/test_model_from.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.os import Os
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.model_from import ModelFrom
+from sendpost_python_sdk import configuration
 
 
-class TestOs(unittest.TestCase):
-    """Os unit test stubs"""
+class TestModelFrom(unittest.TestCase):
+    """ModelFrom unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sendpost-1.0.0/test/test_models/test_q_email_message.py` & `sendpost-1.0.1/test/test_models/test_webhook_event.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.q_email_message import QEmailMessage
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.webhook_event import WebhookEvent
+from sendpost_python_sdk import configuration
 
 
-class TestQEmailMessage(unittest.TestCase):
-    """QEmailMessage unit test stubs"""
+class TestWebhookEvent(unittest.TestCase):
+    """WebhookEvent unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sendpost-1.0.0/test/test_models/test_q_event.py` & `sendpost-1.0.1/test/test_models/test_q_email_message.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.q_event import QEvent
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.q_email_message import QEmailMessage
+from sendpost_python_sdk import configuration
 
 
-class TestQEvent(unittest.TestCase):
-    """QEvent unit test stubs"""
+class TestQEmailMessage(unittest.TestCase):
+    """QEmailMessage unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sendpost-1.0.0/test/test_models/test_reply_to.py` & `sendpost-1.0.1/test/test_models/test_email_message.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.reply_to import ReplyTo
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.email_message import EmailMessage
+from sendpost_python_sdk import configuration
 
 
-class TestReplyTo(unittest.TestCase):
-    """ReplyTo unit test stubs"""
+class TestEmailMessage(unittest.TestCase):
+    """EmailMessage unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sendpost-1.0.0/test/test_models/test_to.py` & `sendpost-1.0.1/test/test_models/test_reply_to.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.to import To
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.reply_to import ReplyTo
+from sendpost_python_sdk import configuration
 
 
-class TestTo(unittest.TestCase):
-    """To unit test stubs"""
+class TestReplyTo(unittest.TestCase):
+    """ReplyTo unit test stubs"""
     _configuration = configuration.Configuration()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `sendpost-1.0.0/test/test_models/test_user_agent.py` & `sendpost-1.0.1/test/test_models/test_user_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     The version of the OpenAPI document: 1.0.0
     Contact: hello@sendpost.io
     Generated by: https://openapi-generator.tech
 """
 
 import unittest
 
-import sendpost_py_sdk
-from sendpost_py_sdk.model.user_agent import UserAgent
-from sendpost_py_sdk import configuration
+import sendpost_python_sdk
+from sendpost_python_sdk.model.user_agent import UserAgent
+from sendpost_python_sdk import configuration
 
 
 class TestUserAgent(unittest.TestCase):
     """UserAgent unit test stubs"""
     _configuration = configuration.Configuration()
```

### Comparing `sendpost-1.0.0/test/test_paths/__init__.py` & `sendpost-1.0.1/test/test_paths/__init__.py`

 * *Files identical despite different names*

### Comparing `sendpost-1.0.0/test/test_paths/test_subaccount_email_/test_post.py` & `sendpost-1.0.1/test/test_paths/test_subaccount_email_/test_post.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
-import sendpost_py_sdk
-from sendpost_py_sdk.paths.subaccount_email_ import post  # noqa: E501
-from sendpost_py_sdk import configuration, schemas, api_client
+import sendpost_python_sdk
+from sendpost_python_sdk.paths.subaccount_email_ import post  # noqa: E501
+from sendpost_python_sdk import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestSubaccountEmail(ApiTestMixin, unittest.TestCase):
     """
     SubaccountEmail unit test stubs
```

### Comparing `sendpost-1.0.0/test/test_paths/test_subaccount_email_template/test_post.py` & `sendpost-1.0.1/test/test_paths/test_subaccount_email_template/test_post.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 """
 
 import unittest
 from unittest.mock import patch
 
 import urllib3
 
-import sendpost_py_sdk
-from sendpost_py_sdk.paths.subaccount_email_template import post  # noqa: E501
-from sendpost_py_sdk import configuration, schemas, api_client
+import sendpost_python_sdk
+from sendpost_python_sdk.paths.subaccount_email_template import post  # noqa: E501
+from sendpost_python_sdk import configuration, schemas, api_client
 
 from .. import ApiTestMixin
 
 
 class TestSubaccountEmailTemplate(ApiTestMixin, unittest.TestCase):
     """
     SubaccountEmailTemplate unit test stubs
```

