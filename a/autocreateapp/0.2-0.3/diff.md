# Comparing `tmp/autocreateapp-0.2.tar.gz` & `tmp/autocreateapp-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autocreateapp-0.2.tar", last modified: Wed Jul 26 09:17:50 2023, max compression
+gzip compressed data, was "autocreateapp-0.3.tar", last modified: Wed Jul 26 09:31:12 2023, max compression
```

## Comparing `autocreateapp-0.2.tar` & `autocreateapp-0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 09:17:50.365319 autocreateapp-0.2/
--rw-rw-r--   0 asc       (1000) asc       (1000)      185 2023-07-26 09:17:50.365319 autocreateapp-0.2/PKG-INFO
-drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 09:17:50.365319 autocreateapp-0.2/autocreateapp/
--rw-rw-r--   0 asc       (1000) asc       (1000)        0 2023-07-26 08:44:37.000000 autocreateapp-0.2/autocreateapp/__init__.py
--rw-rw-r--   0 asc       (1000) asc       (1000)     2488 2023-07-26 08:55:05.000000 autocreateapp-0.2/autocreateapp/create_project.py
-drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 09:17:50.365319 autocreateapp-0.2/autocreateapp.egg-info/
--rw-rw-r--   0 asc       (1000) asc       (1000)      185 2023-07-26 09:17:50.000000 autocreateapp-0.2/autocreateapp.egg-info/PKG-INFO
--rw-rw-r--   0 asc       (1000) asc       (1000)      290 2023-07-26 09:17:50.000000 autocreateapp-0.2/autocreateapp.egg-info/SOURCES.txt
--rw-rw-r--   0 asc       (1000) asc       (1000)        1 2023-07-26 09:17:50.000000 autocreateapp-0.2/autocreateapp.egg-info/dependency_links.txt
--rw-rw-r--   0 asc       (1000) asc       (1000)       86 2023-07-26 09:17:50.000000 autocreateapp-0.2/autocreateapp.egg-info/entry_points.txt
--rw-rw-r--   0 asc       (1000) asc       (1000)        7 2023-07-26 09:17:50.000000 autocreateapp-0.2/autocreateapp.egg-info/requires.txt
--rw-rw-r--   0 asc       (1000) asc       (1000)       14 2023-07-26 09:17:50.000000 autocreateapp-0.2/autocreateapp.egg-info/top_level.txt
--rw-rw-r--   0 asc       (1000) asc       (1000)       38 2023-07-26 09:17:50.365319 autocreateapp-0.2/setup.cfg
--rw-rw-r--   0 asc       (1000) asc       (1000)      391 2023-07-26 09:17:23.000000 autocreateapp-0.2/setup.py
+drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 09:31:12.081260 autocreateapp-0.3/
+-rw-rw-r--   0 asc       (1000) asc       (1000)     3552 2023-07-26 09:31:12.081260 autocreateapp-0.3/PKG-INFO
+-rw-rw-r--   0 asc       (1000) asc       (1000)     2836 2023-07-26 09:30:19.000000 autocreateapp-0.3/README.md
+drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 09:31:12.077260 autocreateapp-0.3/autocreateapp/
+-rw-rw-r--   0 asc       (1000) asc       (1000)        0 2023-07-26 08:44:37.000000 autocreateapp-0.3/autocreateapp/__init__.py
+-rw-rw-r--   0 asc       (1000) asc       (1000)     2488 2023-07-26 08:55:05.000000 autocreateapp-0.3/autocreateapp/create_project.py
+drwxrwxr-x   0 asc       (1000) asc       (1000)        0 2023-07-26 09:31:12.081260 autocreateapp-0.3/autocreateapp.egg-info/
+-rw-rw-r--   0 asc       (1000) asc       (1000)     3552 2023-07-26 09:31:11.000000 autocreateapp-0.3/autocreateapp.egg-info/PKG-INFO
+-rw-rw-r--   0 asc       (1000) asc       (1000)      300 2023-07-26 09:31:12.000000 autocreateapp-0.3/autocreateapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 asc       (1000) asc       (1000)        1 2023-07-26 09:31:11.000000 autocreateapp-0.3/autocreateapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 asc       (1000) asc       (1000)       86 2023-07-26 09:31:11.000000 autocreateapp-0.3/autocreateapp.egg-info/entry_points.txt
+-rw-rw-r--   0 asc       (1000) asc       (1000)        7 2023-07-26 09:31:11.000000 autocreateapp-0.3/autocreateapp.egg-info/requires.txt
+-rw-rw-r--   0 asc       (1000) asc       (1000)       14 2023-07-26 09:31:11.000000 autocreateapp-0.3/autocreateapp.egg-info/top_level.txt
+-rw-rw-r--   0 asc       (1000) asc       (1000)       38 2023-07-26 09:31:12.081260 autocreateapp-0.3/setup.cfg
+-rw-rw-r--   0 asc       (1000) asc       (1000)      610 2023-07-26 09:30:54.000000 autocreateapp-0.3/setup.py
```

### Comparing `autocreateapp-0.2/autocreateapp/create_project.py` & `autocreateapp-0.3/autocreateapp/create_project.py`

 * *Files identical despite different names*

