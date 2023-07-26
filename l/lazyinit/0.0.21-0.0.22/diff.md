# Comparing `tmp/lazyinit-0.0.21.tar.gz` & `tmp/lazyinit-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyinit-0.0.21.tar", last modified: Wed Jul 26 04:17:15 2023, max compression
+gzip compressed data, was "lazyinit-0.0.22.tar", last modified: Wed Jul 26 04:18:53 2023, max compression
```

## Comparing `lazyinit-0.0.21.tar` & `lazyinit-0.0.22.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:17:15.250743 lazyinit-0.0.21/
--rw-r--r--   0 dengyifan   (501) staff       (20)       21 2023-07-23 14:48:03.000000 lazyinit-0.0.21/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:17:15.250528 lazyinit-0.0.21/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.21/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:17:15.248775 lazyinit-0.0.21/lazyinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.21/lazyinit/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     7833 2023-07-26 04:13:10.000000 lazyinit-0.0.21/lazyinit/init.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:15:58.000000 lazyinit-0.0.21/lazyinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4862 2023-07-26 03:36:41.000000 lazyinit-0.0.21/lazyinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:17:15.250213 lazyinit-0.0.21/lazyinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:17:15.000000 lazyinit-0.0.21/lazyinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      296 2023-07-26 04:17:15.000000 lazyinit-0.0.21/lazyinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:17:15.000000 lazyinit-0.0.21/lazyinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:17:15.000000 lazyinit-0.0.21/lazyinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       36 2023-07-26 04:17:15.000000 lazyinit-0.0.21/lazyinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:17:15.000000 lazyinit-0.0.21/lazyinit.egg-info/top_level.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:17:15.250832 lazyinit-0.0.21/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      864 2023-07-26 04:17:12.000000 lazyinit-0.0.21/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:18:53.339991 lazyinit-0.0.22/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       21 2023-07-23 14:48:03.000000 lazyinit-0.0.22/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:18:53.339703 lazyinit-0.0.22/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.22/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:18:53.336958 lazyinit-0.0.22/lazyinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.22/lazyinit/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7833 2023-07-26 04:13:10.000000 lazyinit-0.0.22/lazyinit/init.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:15:58.000000 lazyinit-0.0.22/lazyinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4880 2023-07-26 04:18:42.000000 lazyinit-0.0.22/lazyinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:18:53.338233 lazyinit-0.0.22/lazyinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      296 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/top_level.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:18:53.340075 lazyinit-0.0.22/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      842 2023-07-26 04:18:50.000000 lazyinit-0.0.22/setup.py
```

### Comparing `lazyinit-0.0.21/lazyinit/init.py` & `lazyinit-0.0.22/lazyinit/init.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.21/lazyinit/run.py` & `lazyinit-0.0.22/lazyinit/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.21/lazyinit/utils.py` & `lazyinit-0.0.22/lazyinit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from bs4 import BeautifulSoup
 import requests as rq
 import pkg_resources
 import os
 from rich.console import Console
+import subprocess
 
 console = Console()
 
 def package_installed(package_name):
     """
     检查指定包是否已安装
     """
```

### Comparing `lazyinit-0.0.21/setup.py` & `lazyinit-0.0.22/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='lazyinit',
-    version='0.0.21',
+    version='0.0.22',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init zhei environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         'bs4',
         'requests',
         'rich',
         'pyyaml',
-        'subprocess',
     ],
     exclude=["*.tests", "*.tests.*", "tests"],
     include_package_data=True,
     python_requires='>=3.6',
     entry_points = {
         'console_scripts' : [
             # 这一行是安装到命令行运行的关键
```

