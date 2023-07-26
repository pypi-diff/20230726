# Comparing `tmp/lazyinit-0.0.26.tar.gz` & `tmp/lazyinit-0.0.261.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyinit-0.0.26.tar", last modified: Wed Jul 26 04:34:19 2023, max compression
+gzip compressed data, was "lazyinit-0.0.261.tar", last modified: Wed Jul 26 04:37:02 2023, max compression
```

## Comparing `lazyinit-0.0.26.tar` & `lazyinit-0.0.261.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:34:19.493384 lazyinit-0.0.26/
--rw-r--r--   0 dengyifan   (501) staff       (20)       65 2023-07-26 04:33:05.000000 lazyinit-0.0.26/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:34:19.493200 lazyinit-0.0.26/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.26/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:34:19.492015 lazyinit-0.0.26/lazyinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.26/lazyinit/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.26/lazyinit/bash_config.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     8140 2023-07-26 04:34:00.000000 lazyinit-0.0.26/lazyinit/init.py
--rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.26/lazyinit/redis.conf
--rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.26/lazyinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4880 2023-07-26 04:18:42.000000 lazyinit-0.0.26/lazyinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:34:19.492966 lazyinit-0.0.26/lazyinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      341 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/top_level.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:34:19.493442 lazyinit-0.0.26/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      842 2023-07-26 04:34:18.000000 lazyinit-0.0.26/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:37:02.961336 lazyinit-0.0.261/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       84 2023-07-26 04:36:39.000000 lazyinit-0.0.261/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-26 04:37:02.961147 lazyinit-0.0.261/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.261/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:37:02.960062 lazyinit-0.0.261/lazyinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.261/lazyinit/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.261/lazyinit/bash_config.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     8140 2023-07-26 04:34:00.000000 lazyinit-0.0.261/lazyinit/init.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.261/lazyinit/redis.conf
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.261/lazyinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4880 2023-07-26 04:18:42.000000 lazyinit-0.0.261/lazyinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:37:02.960913 lazyinit-0.0.261/lazyinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      341 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/top_level.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:37:02.961395 lazyinit-0.0.261/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      843 2023-07-26 04:37:00.000000 lazyinit-0.0.261/setup.py
```

### Comparing `lazyinit-0.0.26/lazyinit/bash_config.txt` & `lazyinit-0.0.261/lazyinit/bash_config.txt`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.26/lazyinit/init.py` & `lazyinit-0.0.261/lazyinit/init.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.26/lazyinit/redis.conf` & `lazyinit-0.0.261/lazyinit/redis.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.26/lazyinit/run.py` & `lazyinit-0.0.261/lazyinit/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.26/lazyinit/utils.py` & `lazyinit-0.0.261/lazyinit/utils.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.26/setup.py` & `lazyinit-0.0.261/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='lazyinit',
-    version='0.0.26',
+    version='0.0.261',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init zhei environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

