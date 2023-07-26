# Comparing `tmp/tracim_daemon_sdk-1.0.0.tar.gz` & `tmp/tracim_daemon_sdk-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracim_daemon_sdk-1.0.0.tar", last modified: Sun Jul 23 19:07:11 2023, max compression
+gzip compressed data, was "tracim_daemon_sdk-1.0.1.tar", last modified: Wed Jul 26 15:31:10 2023, max compression
```

## Comparing `tracim_daemon_sdk-1.0.0.tar` & `tracim_daemon_sdk-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 millefeuille   (501) staff       (20)        0 2023-07-23 19:07:11.659625 tracim_daemon_sdk-1.0.0/
--rw-r--r--   0 millefeuille   (501) staff       (20)     1069 2023-07-23 18:59:43.000000 tracim_daemon_sdk-1.0.0/LICENCE
--rw-r--r--   0 millefeuille   (501) staff       (20)     7701 2023-07-23 19:07:11.659493 tracim_daemon_sdk-1.0.0/PKG-INFO
--rw-r--r--   0 millefeuille   (501) staff       (20)     7142 2023-07-23 19:00:11.000000 tracim_daemon_sdk-1.0.0/README.md
--rw-r--r--   0 millefeuille   (501) staff       (20)      633 2023-07-23 19:06:32.000000 tracim_daemon_sdk-1.0.0/pyproject.toml
--rw-r--r--   0 millefeuille   (501) staff       (20)       38 2023-07-23 19:07:11.659672 tracim_daemon_sdk-1.0.0/setup.cfg
-drwxr-xr-x   0 millefeuille   (501) staff       (20)        0 2023-07-23 19:07:11.655814 tracim_daemon_sdk-1.0.0/src/
-drwxr-xr-x   0 millefeuille   (501) staff       (20)        0 2023-07-23 19:07:11.658536 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/
--rw-r--r--   0 millefeuille   (501) staff       (20)       35 2023-07-23 15:49:03.000000 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/__init__.py
--rw-r--r--   0 millefeuille   (501) staff       (20)      515 2023-07-23 15:53:19.000000 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/daemon_event.py
--rw-r--r--   0 millefeuille   (501) staff       (20)     2034 2023-07-23 15:49:03.000000 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/data.py
--rw-r--r--   0 millefeuille   (501) staff       (20)      779 2023-07-23 15:49:03.000000 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/event.py
--rw-r--r--   0 millefeuille   (501) staff       (20)      350 2023-07-23 15:51:24.000000 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/helper.py
--rw-r--r--   0 millefeuille   (501) staff       (20)     4168 2023-07-23 18:56:39.000000 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/sdk.py
-drwxr-xr-x   0 millefeuille   (501) staff       (20)        0 2023-07-23 19:07:11.659299 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk.egg-info/
--rw-r--r--   0 millefeuille   (501) staff       (20)     7701 2023-07-23 19:07:11.000000 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk.egg-info/PKG-INFO
--rw-r--r--   0 millefeuille   (501) staff       (20)      406 2023-07-23 19:07:11.000000 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 millefeuille   (501) staff       (20)        1 2023-07-23 19:07:11.000000 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 millefeuille   (501) staff       (20)       18 2023-07-23 19:07:11.000000 tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2023-07-26 15:31:10.204312 tracim_daemon_sdk-1.0.1/
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     1069 2023-07-25 15:44:18.000000 tracim_daemon_sdk-1.0.1/LICENCE
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     2712 2023-07-26 15:31:10.204312 tracim_daemon_sdk-1.0.1/PKG-INFO
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     2153 2023-07-25 15:44:18.000000 tracim_daemon_sdk-1.0.1/README.md
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      633 2023-07-26 15:29:44.000000 tracim_daemon_sdk-1.0.1/pyproject.toml
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)       38 2023-07-26 15:31:10.204312 tracim_daemon_sdk-1.0.1/setup.cfg
+drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2023-07-26 15:31:10.196312 tracim_daemon_sdk-1.0.1/src/
+drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2023-07-26 15:31:10.200312 tracim_daemon_sdk-1.0.1/src/miniclient/
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      858 2023-07-26 15:28:00.000000 tracim_daemon_sdk-1.0.1/src/miniclient/miniclient.py
+drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2023-07-26 15:31:10.204312 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)       35 2023-07-25 15:44:18.000000 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/__init__.py
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      515 2023-07-25 15:44:18.000000 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/daemon_event.py
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     2034 2023-07-25 15:44:18.000000 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/data.py
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      779 2023-07-25 15:44:18.000000 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/event.py
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      350 2023-07-25 15:44:18.000000 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/helper.py
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     4227 2023-07-25 15:53:45.000000 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/sdk.py
+drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2023-07-26 15:31:10.204312 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk.egg-info/
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     2712 2023-07-26 15:31:10.000000 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      435 2023-07-26 15:31:10.000000 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)        1 2023-07-26 15:31:10.000000 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 mathieu   (1000) mathieu   (1000)       29 2023-07-26 15:31:10.000000 tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk.egg-info/top_level.txt
```

### Comparing `tracim_daemon_sdk-1.0.0/LICENCE` & `tracim_daemon_sdk-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `tracim_daemon_sdk-1.0.0/pyproject.toml` & `tracim_daemon_sdk-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tracim_daemon_sdk"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Millefeuille", email="1kfeuille@mlabouri.fr" },
 ]
 description = "An SDK for the TracimDaemon project"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/daemon_event.py` & `tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/daemon_event.py`

 * *Files identical despite different names*

### Comparing `tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/data.py` & `tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/data.py`

 * *Files identical despite different names*

### Comparing `tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/event.py` & `tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/event.py`

 * *Files identical despite different names*

### Comparing `tracim_daemon_sdk-1.0.0/src/tracim_daemon_sdk/sdk.py` & `tracim_daemon_sdk-1.0.1/src/tracim_daemon_sdk/sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,14 +79,15 @@
             try:
                 while 1:
                     data: bytes = conn.recv(4096)
                     if not data:
                         break
                     event: DaemonEvent = decode_json(data)
                     self.__call_handler(EVENT_TYPE_GENERIC, event)
+                    self.__call_handler(event.type, event)
                     if event.type == DAEMON_TRACIM_EVENT:
                         tlm_data: TLMEvent = decode_json(event.data)
                         self.__call_handler(tlm_data.event_type, event)
             except Exception as e:
                 self.__call_handler(EVENT_TYPE_ERROR, DaemonEvent(
                     event_type=EVENT_TYPE_ERROR,
                     data=TypeErrorData(e)
```

