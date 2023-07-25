# Comparing `tmp/promptcloud-1.0.0.tar.gz` & `tmp/promptcloud-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptcloud-1.0.0.tar", last modified: Tue Jul 25 21:22:47 2023, max compression
+gzip compressed data, was "promptcloud-1.0.1.tar", last modified: Tue Jul 25 23:37:23 2023, max compression
```

## Comparing `promptcloud-1.0.0.tar` & `promptcloud-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 mattyhogan   (501) staff       (20)        0 2023-07-25 21:22:47.423189 promptcloud-1.0.0/
--rw-r--r--   0 mattyhogan   (501) staff       (20)      265 2023-07-25 21:22:47.423076 promptcloud-1.0.0/PKG-INFO
-drwxr-xr-x   0 mattyhogan   (501) staff       (20)        0 2023-07-25 21:22:47.422320 promptcloud-1.0.0/promptcloud/
--rw-r--r--   0 mattyhogan   (501) staff       (20)        0 2023-07-18 18:51:52.000000 promptcloud-1.0.0/promptcloud/__init__.py
--rw-r--r--   0 mattyhogan   (501) staff       (20)     2704 2023-07-25 16:00:39.000000 promptcloud-1.0.0/promptcloud/client.py
--rw-r--r--   0 mattyhogan   (501) staff       (20)      678 2023-07-25 15:24:05.000000 promptcloud-1.0.0/promptcloud/error.py
--rw-r--r--   0 mattyhogan   (501) staff       (20)     5171 2023-07-25 21:18:18.000000 promptcloud-1.0.0/promptcloud/prompt.py
--rw-r--r--   0 mattyhogan   (501) staff       (20)      561 2023-07-25 21:15:28.000000 promptcloud-1.0.0/promptcloud/schema.py
-drwxr-xr-x   0 mattyhogan   (501) staff       (20)        0 2023-07-25 21:22:47.422887 promptcloud-1.0.0/promptcloud.egg-info/
--rw-r--r--   0 mattyhogan   (501) staff       (20)      265 2023-07-25 21:22:47.000000 promptcloud-1.0.0/promptcloud.egg-info/PKG-INFO
--rw-r--r--   0 mattyhogan   (501) staff       (20)      293 2023-07-25 21:22:47.000000 promptcloud-1.0.0/promptcloud.egg-info/SOURCES.txt
--rw-r--r--   0 mattyhogan   (501) staff       (20)        1 2023-07-25 21:22:47.000000 promptcloud-1.0.0/promptcloud.egg-info/dependency_links.txt
--rw-r--r--   0 mattyhogan   (501) staff       (20)       16 2023-07-25 21:22:47.000000 promptcloud-1.0.0/promptcloud.egg-info/requires.txt
--rw-r--r--   0 mattyhogan   (501) staff       (20)       12 2023-07-25 21:22:47.000000 promptcloud-1.0.0/promptcloud.egg-info/top_level.txt
--rw-r--r--   0 mattyhogan   (501) staff       (20)       38 2023-07-25 21:22:47.423230 promptcloud-1.0.0/setup.cfg
--rw-r--r--   0 mattyhogan   (501) staff       (20)      384 2023-07-25 15:23:39.000000 promptcloud-1.0.0/setup.py
+drwxr-xr-x   0 mattyhogan   (501) staff       (20)        0 2023-07-25 23:37:23.816305 promptcloud-1.0.1/
+-rw-r--r--   0 mattyhogan   (501) staff       (20)      274 2023-07-25 23:37:23.816197 promptcloud-1.0.1/PKG-INFO
+-rw-r--r--   0 mattyhogan   (501) staff       (20)     5663 2023-07-25 21:38:15.000000 promptcloud-1.0.1/README.md
+drwxr-xr-x   0 mattyhogan   (501) staff       (20)        0 2023-07-25 23:37:23.815289 promptcloud-1.0.1/promptcloud/
+-rw-r--r--   0 mattyhogan   (501) staff       (20)        0 2023-07-18 18:51:52.000000 promptcloud-1.0.1/promptcloud/__init__.py
+-rw-r--r--   0 mattyhogan   (501) staff       (20)     2704 2023-07-25 16:00:39.000000 promptcloud-1.0.1/promptcloud/client.py
+-rw-r--r--   0 mattyhogan   (501) staff       (20)      678 2023-07-25 15:24:05.000000 promptcloud-1.0.1/promptcloud/error.py
+-rw-r--r--   0 mattyhogan   (501) staff       (20)     5171 2023-07-25 21:18:18.000000 promptcloud-1.0.1/promptcloud/prompt.py
+-rw-r--r--   0 mattyhogan   (501) staff       (20)      561 2023-07-25 21:15:28.000000 promptcloud-1.0.1/promptcloud/schema.py
+drwxr-xr-x   0 mattyhogan   (501) staff       (20)        0 2023-07-25 23:37:23.815998 promptcloud-1.0.1/promptcloud.egg-info/
+-rw-r--r--   0 mattyhogan   (501) staff       (20)      274 2023-07-25 23:37:23.000000 promptcloud-1.0.1/promptcloud.egg-info/PKG-INFO
+-rw-r--r--   0 mattyhogan   (501) staff       (20)      303 2023-07-25 23:37:23.000000 promptcloud-1.0.1/promptcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 mattyhogan   (501) staff       (20)        1 2023-07-25 23:37:23.000000 promptcloud-1.0.1/promptcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 mattyhogan   (501) staff       (20)       16 2023-07-25 23:37:23.000000 promptcloud-1.0.1/promptcloud.egg-info/requires.txt
+-rw-r--r--   0 mattyhogan   (501) staff       (20)       12 2023-07-25 23:37:23.000000 promptcloud-1.0.1/promptcloud.egg-info/top_level.txt
+-rw-r--r--   0 mattyhogan   (501) staff       (20)       38 2023-07-25 23:37:23.816350 promptcloud-1.0.1/setup.cfg
+-rw-r--r--   0 mattyhogan   (501) staff       (20)      393 2023-07-25 23:36:44.000000 promptcloud-1.0.1/setup.py
```

### Comparing `promptcloud-1.0.0/promptcloud/client.py` & `promptcloud-1.0.1/promptcloud/client.py`

 * *Files identical despite different names*

### Comparing `promptcloud-1.0.0/promptcloud/error.py` & `promptcloud-1.0.1/promptcloud/error.py`

 * *Files identical despite different names*

### Comparing `promptcloud-1.0.0/promptcloud/prompt.py` & `promptcloud-1.0.1/promptcloud/prompt.py`

 * *Files identical despite different names*

### Comparing `promptcloud-1.0.0/promptcloud/schema.py` & `promptcloud-1.0.1/promptcloud/schema.py`

 * *Files identical despite different names*

