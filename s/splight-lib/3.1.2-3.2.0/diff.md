# Comparing `tmp/splight-lib-3.1.2.tar.gz` & `tmp/splight-lib-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-3.1.2.tar", last modified: Fri Jul 14 18:09:35 2023, max compression
+gzip compressed data, was "splight-lib-3.2.0.tar", last modified: Wed Jul 26 12:52:49 2023, max compression
```

## Comparing `splight-lib-3.1.2.tar` & `splight-lib-3.2.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.575604 splight-lib-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.000000 splight-lib-3.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-14 18:09:35.575604 splight-lib-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-14 18:09:35.000000 splight-lib-3.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 18:09:35.575604 splight-lib-3.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-14 18:09:35.000000 splight-lib-3.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.567603 splight-lib-3.1.2/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.567603 splight-lib-3.1.2/splight_lib/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/abstract/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.567603 splight-lib-3.1.2/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.571603 splight-lib-3.1.2/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.571603 splight-lib-3.1.2/splight_lib/client/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/communication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/communication/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/communication/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.571603 splight-lib-3.1.2/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/database/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/database/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.571603 splight-lib-3.1.2/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/datalake/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/datalake/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.571603 splight-lib-3.1.2/splight_lib/client/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/grpc/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/grpc/reflector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.571603 splight-lib-3.1.2/splight_lib/client/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/hub/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/client/hub/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.575604 splight-lib-3.1.2/splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/communication/event_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.575604 splight-lib-3.1.2/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/component/log_streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/component/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.575604 splight-lib-3.1.2/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/logging/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.575604 splight-lib-3.1.2/splight_lib/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/communication.py
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/data_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/models/setpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.575604 splight-lib-3.1.2/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.575604 splight-lib-3.1.2/splight_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.575604 splight-lib-3.1.2/splight_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/utils/custom_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 18:09:35.567603 splight-lib-3.1.2/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 18:09:35.000000 splight-lib-3.1.2/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.020779 splight-lib-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:47.000000 splight-lib-3.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-26 12:52:49.020779 splight-lib-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-26 12:52:47.000000 splight-lib-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 12:52:49.020779 splight-lib-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-26 12:52:47.000000 splight-lib-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.004779 splight-lib-3.2.0/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.008779 splight-lib-3.2.0/splight_lib/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/abstract/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.008779 splight-lib-3.2.0/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.008779 splight-lib-3.2.0/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.012779 splight-lib-3.2.0/splight_lib/client/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/communication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/communication/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/communication/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.012779 splight-lib-3.2.0/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/database/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/database/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.012779 splight-lib-3.2.0/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/datalake/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/datalake/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.012779 splight-lib-3.2.0/splight_lib/client/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/grpc/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/grpc/reflector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.016779 splight-lib-3.2.0/splight_lib/client/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/hub/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/client/hub/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.016779 splight-lib-3.2.0/splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/communication/event_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.016779 splight-lib-3.2.0/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/component/log_streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/component/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.016779 splight-lib-3.2.0/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/logging/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.016779 splight-lib-3.2.0/splight_lib/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/communication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/data_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/models/setpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.016779 splight-lib-3.2.0/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.016779 splight-lib-3.2.0/splight_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.016779 splight-lib-3.2.0/splight_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/utils/custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-07-26 12:52:47.000000 splight-lib-3.2.0/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 12:52:49.004779 splight-lib-3.2.0/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-26 12:52:48.000000 splight-lib-3.2.0/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-26 12:52:48.000000 splight-lib-3.2.0/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:52:48.000000 splight-lib-3.2.0/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 12:52:48.000000 splight-lib-3.2.0/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-26 12:52:48.000000 splight-lib-3.2.0/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 12:52:48.000000 splight-lib-3.2.0/splight_lib.egg-info/top_level.txt
```

### Comparing `splight-lib-3.1.2/PKG-INFO` & `splight-lib-3.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.1.2
+Version: 3.2.0
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.1.2/setup.py` & `splight-lib-3.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="3.1.2",
+    version="3.2.0",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-3.1.2/splight_lib/abstract/client.py` & `splight-lib-3.2.0/splight_lib/abstract/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/auth/mac_auth.py` & `splight-lib-3.2.0/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/communication/abstract.py` & `splight-lib-3.2.0/splight_lib/client/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/communication/remote_client.py` & `splight-lib-3.2.0/splight_lib/client/communication/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/database/abstract.py` & `splight-lib-3.2.0/splight_lib/client/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/database/builder.py` & `splight-lib-3.2.0/splight_lib/client/database/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/database/classmap.py` & `splight-lib-3.2.0/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/database/local_client.py` & `splight-lib-3.2.0/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/database/remote_client.py` & `splight-lib-3.2.0/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/datalake/abstract.py` & `splight-lib-3.2.0/splight_lib/client/datalake/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/datalake/builder.py` & `splight-lib-3.2.0/splight_lib/client/datalake/builder.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/datalake/local_client.py` & `splight-lib-3.2.0/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/datalake/remote_client.py` & `splight-lib-3.2.0/splight_lib/client/datalake/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/exceptions.py` & `splight-lib-3.2.0/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/file_handler.py` & `splight-lib-3.2.0/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/filter.py` & `splight-lib-3.2.0/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/grpc/client.py` & `splight-lib-3.2.0/splight_lib/client/grpc/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from typing import Callable, Optional, Tuple
 
 import grpc
 from splight_lib.client.grpc.decorators import retry_streaming
 from splight_lib.client.grpc.reflector import GrpcReflectionClient
 
 
+class LogsGRPCError(Exception):
+    pass
+
+
 class MissingGRPCService(Exception):
     pass
 
 
 class SplightGRPCClient:
     AUTHORIZATION: str = "authorization"
     _SERVICE_NAME: str = None
@@ -46,18 +50,21 @@
 
     def __init__(self, grpc_host: str, secure_channel: bool = True):
         super().__init__(grpc_host, secure_channel=secure_channel)
         self._log_entry = self._reflector.message_class(self._LOG_ENTRY)
 
     @retry_streaming(times=5)
     def stream_logs(self, log_generator: Callable, component_id: str):
-        self._stub.stash_log_entry(
-            self._parse_log_message(log_generator(), component_id),
-            metadata=[self._auth_header],
-        )
+        try:
+            self._stub.stash_log_entry(
+                self._parse_log_message(log_generator(), component_id),
+                metadata=[self._auth_header],
+            )
+        except grpc.RpcError as exc:
+            raise LogsGRPCError("Unable to stream component logs") from exc
 
     def _parse_log_message(self, message_iterator: str, component_id: str):
         for message in message_iterator:
             yield self._log_entry(
                 message=message,
                 component_id=component_id,
             )
```

### Comparing `splight-lib-3.1.2/splight_lib/client/grpc/decorators.py` & `splight-lib-3.2.0/splight_lib/client/grpc/decorators.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/grpc/reflector.py` & `splight-lib-3.2.0/splight_lib/client/grpc/reflector.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/hub/abstract.py` & `splight-lib-3.2.0/splight_lib/client/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/client/hub/client.py` & `splight-lib-3.2.0/splight_lib/client/hub/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/communication/event_handler.py` & `splight-lib-3.2.0/splight_lib/communication/event_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/component/abstract.py` & `splight-lib-3.2.0/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/component/exceptions.py` & `splight-lib-3.2.0/splight_lib/component/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,7 +36,11 @@
         super().__init__(msg)
 
 
 class MissingCommandCallback(Exception):
     def __init__(self, method_name: str):
         msg = f"Missing method {method_name} associated with a Command"
         super().__init__(msg)
+
+
+class LogsStreamerError(Exception):
+    pass
```

### Comparing `splight-lib-3.1.2/splight_lib/component/log_streamer.py` & `splight-lib-3.2.0/splight_lib/component/log_streamer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,66 +1,102 @@
 import re
 import sys
+from queue import Empty, Queue
 from subprocess import Popen
+from threading import Thread
 from typing import Generator, Optional
 
-from splight_lib.client.grpc.client import LogsGRPCClient
+from splight_lib.client.grpc.client import LogsGRPCClient, LogsGRPCError
+from splight_lib.component.exceptions import LogsStreamerError
 from splight_lib.settings import settings
 
 LOG_FORMAT = r"^.* \| .* \| .*:\d{2,} \| .* "
 LOG_PATTERN = re.compile(LOG_FORMAT)
 
 
 class ComponentLogsStreamer:
     def __init__(self, process: Popen, component_id: str):
         self._process = process
         self._component_id = component_id
 
-        self._client = LogsGRPCClient(
+        try:
+            self._client = self._create_client()
+        except Exception as exc:
+            raise LogsStreamerError(
+                "Unable to connect to gRPC server"
+            ) from exc
+        self._logs_entry = self._client._log_entry
+        self._thread: Optional[Thread] = None
+        self._queue: Optional[Queue] = None
+        self._running: bool = False
+
+    def _create_client(self):
+        client = LogsGRPCClient(
             grpc_host=settings.SPLIGHT_GRPC_HOST, secure_channel=True
         )
-        self._client.set_authorization_header(
+        client.set_authorization_header(
             access_id=settings.SPLIGHT_ACCESS_ID,
             secret_key=settings.SPLIGHT_SECRET_KEY,
         )
-        self._logs_entry = self._client._log_entry
+        return client
 
     def start(self):
+        self._thread = Thread(target=self._consume_logs, daemon=True)
+        self._queue = Queue()
+        self._running = True
+        self._thread.start()
         self._run()
 
     def stop(self):
-        self._thread.stop()
+        self._running = False
+        self._thread.join(timeout=10)
+        self._queue = None
+        self._thread = None
 
     def _run(self):
-        self._client.stream_logs(self.logs_iterator, self._component_id)
+        while self._running:
+            try:
+                self._client.stream_logs(
+                    self.logs_iterator, self._component_id
+                )
+            except LogsGRPCError as exc:
+                raise LogsStreamerError(
+                    "Component Logs stream stopped"
+                ) from exc
 
-    def logs_iterator(self) -> Generator:
-        self._message_buffer = []
+    def _consume_logs(self):
         reader = iter(self._process.stdout.readline, "")
         for new_line in reader:
             if self._process.poll() is not None:
-                msg = "".join(self._message_buffer)
-                sys.stdout.write(msg)
-                yield msg
                 output, error = self._process.communicate()
                 output_msg = output.decode("utf-8")
                 error_msg = error.decode("utf-8")
-                sys.stdout.write(output_msg)
-                yield output_msg
-                sys.stdout.write(error_msg)
-                yield error_msg
+                self._queue.put(output_msg)
+                self._queue.put(error_msg)
+                self._running = False
                 break
+            self._queue.put(new_line.decode("utf-8"))
 
-            line_msg = new_line.decode("utf-8")
-            sys.stdout.write(line_msg)
+    def logs_iterator(self) -> Generator:
+        self._message_buffer = []
+        while True:
+            try:
+                message = self._queue.get(timeout=10)
+            except Empty:
+                msg = "".join(self._message_buffer)
+                if msg:
+                    sys.stdout.write(msg)
+                    yield msg
+                return
 
-            full_msg = self._generate_message(line_msg)
+            full_msg = self._generate_message(message)
             if not full_msg:
                 continue
             yield full_msg
+            sys.stdout.write(full_msg)
 
     def _generate_message(self, raw_msg: str) -> Optional[str]:
         if self._is_log(raw_msg):
             msg = "".join(self._message_buffer)
             self._message_buffer = [raw_msg]
             return msg
         self._message_buffer.append(raw_msg)
```

### Comparing `splight-lib-3.1.2/splight_lib/component/spec.py` & `splight-lib-3.2.0/splight_lib/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/encryption.py` & `splight-lib-3.2.0/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/execution.py` & `splight-lib-3.2.0/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/logging/_internal.py` & `splight-lib-3.2.0/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/logging/component.py` & `splight-lib-3.2.0/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/logging/logging.py` & `splight-lib-3.2.0/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/__init__.py` & `splight-lib-3.2.0/splight_lib/models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/alert.py` & `splight-lib-3.2.0/splight_lib/models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/asset.py` & `splight-lib-3.2.0/splight_lib/models/asset.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/base.py` & `splight-lib-3.2.0/splight_lib/models/base.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/communication.py` & `splight-lib-3.2.0/splight_lib/models/communication.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/component.py` & `splight-lib-3.2.0/splight_lib/models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/dashboard.py` & `splight-lib-3.2.0/splight_lib/models/dashboard.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/data_address.py` & `splight-lib-3.2.0/splight_lib/models/data_address.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/event.py` & `splight-lib-3.2.0/splight_lib/models/event.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/file.py` & `splight-lib-3.2.0/splight_lib/models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/hub.py` & `splight-lib-3.2.0/splight_lib/models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/native.py` & `splight-lib-3.2.0/splight_lib/models/native.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/query.py` & `splight-lib-3.2.0/splight_lib/models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/models/setpoint.py` & `splight-lib-3.2.0/splight_lib/models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/restclient/client.py` & `splight-lib-3.2.0/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/restclient/exceptions.py` & `splight-lib-3.2.0/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/restclient/types.py` & `splight-lib-3.2.0/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/settings.py` & `splight-lib-3.2.0/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/testing/__init__.py` & `splight-lib-3.2.0/splight_lib/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/utils/custom_model.py` & `splight-lib-3.2.0/splight_lib/utils/custom_model.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/utils/hub.py` & `splight-lib-3.2.0/splight_lib/utils/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib/webhook.py` & `splight-lib-3.2.0/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib.egg-info/PKG-INFO` & `splight-lib-3.2.0/splight_lib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 3.1.2
+Version: 3.2.0
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-3.1.2/splight_lib.egg-info/SOURCES.txt` & `splight-lib-3.2.0/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-3.1.2/splight_lib.egg-info/requires.txt` & `splight-lib-3.2.0/splight_lib.egg-info/requires.txt`

 * *Files identical despite different names*

