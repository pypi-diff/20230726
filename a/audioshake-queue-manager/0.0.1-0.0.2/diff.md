# Comparing `tmp/audioshake_queue_manager-0.0.1.tar.gz` & `tmp/audioshake_queue_manager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audioshake_queue_manager-0.0.1.tar", last modified: Wed Jul 26 06:20:04 2023, max compression
+gzip compressed data, was "audioshake_queue_manager-0.0.2.tar", last modified: Wed Jul 26 06:25:13 2023, max compression
```

## Comparing `audioshake_queue_manager-0.0.1.tar` & `audioshake_queue_manager-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 06:20:04.979783 audioshake_queue_manager-0.0.1/
--rw-r--r--   0 theslyguy   (501) staff       (20)      183 2023-07-26 06:20:04.979407 audioshake_queue_manager-0.0.1/PKG-INFO
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 06:20:04.977443 audioshake_queue_manager-0.0.1/audioshake_queue_manager/
--rw-r--r--   0 theslyguy   (501) staff       (20)        0 2023-07-26 03:25:13.000000 audioshake_queue_manager-0.0.1/audioshake_queue_manager/__init__.py
--rw-r--r--   0 theslyguy   (501) staff       (20)     3224 2023-07-26 06:13:43.000000 audioshake_queue_manager-0.0.1/audioshake_queue_manager/__main__.py
-drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 06:20:04.978980 audioshake_queue_manager-0.0.1/audioshake_queue_manager.egg-info/
--rw-r--r--   0 theslyguy   (501) staff       (20)      183 2023-07-26 06:20:04.000000 audioshake_queue_manager-0.0.1/audioshake_queue_manager.egg-info/PKG-INFO
--rw-r--r--   0 theslyguy   (501) staff       (20)      327 2023-07-26 06:20:04.000000 audioshake_queue_manager-0.0.1/audioshake_queue_manager.egg-info/SOURCES.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-26 06:20:04.000000 audioshake_queue_manager-0.0.1/audioshake_queue_manager.egg-info/dependency_links.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-26 06:20:04.000000 audioshake_queue_manager-0.0.1/audioshake_queue_manager.egg-info/requires.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)       25 2023-07-26 06:20:04.000000 audioshake_queue_manager-0.0.1/audioshake_queue_manager.egg-info/top_level.txt
--rw-r--r--   0 theslyguy   (501) staff       (20)      401 2023-07-26 06:19:43.000000 audioshake_queue_manager-0.0.1/pyproject.toml
--rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-26 06:20:04.979882 audioshake_queue_manager-0.0.1/setup.cfg
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 06:25:13.041646 audioshake_queue_manager-0.0.2/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      183 2023-07-26 06:25:13.041148 audioshake_queue_manager-0.0.2/PKG-INFO
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 06:25:13.038425 audioshake_queue_manager-0.0.2/audioshake_queue_manager/
+-rw-r--r--   0 theslyguy   (501) staff       (20)     3224 2023-07-26 06:24:12.000000 audioshake_queue_manager-0.0.2/audioshake_queue_manager/__init__.py
+drwxr-xr-x   0 theslyguy   (501) staff       (20)        0 2023-07-26 06:25:13.040732 audioshake_queue_manager-0.0.2/audioshake_queue_manager.egg-info/
+-rw-r--r--   0 theslyguy   (501) staff       (20)      183 2023-07-26 06:25:12.000000 audioshake_queue_manager-0.0.2/audioshake_queue_manager.egg-info/PKG-INFO
+-rw-r--r--   0 theslyguy   (501) staff       (20)      290 2023-07-26 06:25:13.000000 audioshake_queue_manager-0.0.2/audioshake_queue_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        1 2023-07-26 06:25:12.000000 audioshake_queue_manager-0.0.2/audioshake_queue_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)        6 2023-07-26 06:25:12.000000 audioshake_queue_manager-0.0.2/audioshake_queue_manager.egg-info/requires.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)       25 2023-07-26 06:25:12.000000 audioshake_queue_manager-0.0.2/audioshake_queue_manager.egg-info/top_level.txt
+-rw-r--r--   0 theslyguy   (501) staff       (20)      401 2023-07-26 06:24:25.000000 audioshake_queue_manager-0.0.2/pyproject.toml
+-rw-r--r--   0 theslyguy   (501) staff       (20)       38 2023-07-26 06:25:13.041787 audioshake_queue_manager-0.0.2/setup.cfg
```

### Comparing `audioshake_queue_manager-0.0.1/audioshake_queue_manager/__main__.py` & `audioshake_queue_manager-0.0.2/audioshake_queue_manager/__init__.py`

 * *Files identical despite different names*

