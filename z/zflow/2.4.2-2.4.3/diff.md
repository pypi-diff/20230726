# Comparing `tmp/zflow-2.4.2.tar.gz` & `tmp/zflow-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zflow-2.4.2.tar", last modified: Thu Jul 13 09:42:54 2023, max compression
+gzip compressed data, was "zflow-2.4.3.tar", last modified: Wed Jul 26 13:36:21 2023, max compression
```

## Comparing `zflow-2.4.2.tar` & `zflow-2.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:42:54.498710 zflow-2.4.2/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-13 09:42:50.000000 zflow-2.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-13 09:42:54.498710 zflow-2.4.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-13 09:42:50.000000 zflow-2.4.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-13 09:42:50.000000 zflow-2.4.2/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-13 09:42:54.498710 zflow-2.4.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1441 2023-07-13 09:42:50.000000 zflow-2.4.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-13 09:42:54.498710 zflow-2.4.2/zflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      244 2023-07-13 09:42:54.000000 zflow-2.4.2/zflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2023-07-13 09:42:54.000000 zflow-2.4.2/zflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 09:42:54.000000 zflow-2.4.2/zflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-13 09:42:54.000000 zflow-2.4.2/zflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-13 09:42:54.000000 zflow-2.4.2/zflow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:36:21.820851 zflow-2.4.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-26 13:36:17.000000 zflow-2.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 13:36:21.820851 zflow-2.4.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-26 13:36:17.000000 zflow-2.4.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-07-26 13:36:17.000000 zflow-2.4.3/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-07-26 13:36:21.820851 zflow-2.4.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2023-07-26 13:36:17.000000 zflow-2.4.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 13:36:21.820851 zflow-2.4.3/zflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-26 13:36:21.000000 zflow-2.4.3/zflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2023-07-26 13:36:21.000000 zflow-2.4.3/zflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 13:36:21.000000 zflow-2.4.3/zflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 13:36:21.000000 zflow-2.4.3/zflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-26 13:36:21.000000 zflow-2.4.3/zflow.egg-info/top_level.txt
```

### Comparing `zflow-2.4.2/LICENSE` & `zflow-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zflow-2.4.2/setup.py` & `zflow-2.4.3/setup.py`

 * *Files identical despite different names*

