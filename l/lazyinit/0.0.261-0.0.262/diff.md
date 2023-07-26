# Comparing `tmp/lazyinit-0.0.261.tar.gz` & `tmp/lazyinit-0.0.262.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyinit-0.0.261.tar", last modified: Wed Jul 26 04:37:02 2023, max compression
+gzip compressed data, was "lazyinit-0.0.262.tar", last modified: Wed Jul 26 04:51:36 2023, max compression
```

## Comparing `lazyinit-0.0.261.tar` & `lazyinit-0.0.262.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:37:02.961336 lazyinit-0.0.261/
--rw-r--r--   0 dengyifan   (501) staff       (20)       84 2023-07-26 04:36:39.000000 lazyinit-0.0.261/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-26 04:37:02.961147 lazyinit-0.0.261/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.261/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:37:02.960062 lazyinit-0.0.261/lazyinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.261/lazyinit/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.261/lazyinit/bash_config.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     8140 2023-07-26 04:34:00.000000 lazyinit-0.0.261/lazyinit/init.py
--rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.261/lazyinit/redis.conf
--rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.261/lazyinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4880 2023-07-26 04:18:42.000000 lazyinit-0.0.261/lazyinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:37:02.960913 lazyinit-0.0.261/lazyinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      341 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:37:02.000000 lazyinit-0.0.261/lazyinit.egg-info/top_level.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:37:02.961395 lazyinit-0.0.261/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      843 2023-07-26 04:37:00.000000 lazyinit-0.0.261/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:51:36.858404 lazyinit-0.0.262/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       84 2023-07-26 04:36:39.000000 lazyinit-0.0.262/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-26 04:51:36.858185 lazyinit-0.0.262/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.262/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:51:36.856926 lazyinit-0.0.262/lazyinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.262/lazyinit/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.262/lazyinit/bash_config.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     8118 2023-07-26 04:51:31.000000 lazyinit-0.0.262/lazyinit/init.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.262/lazyinit/redis.conf
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.262/lazyinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4979 2023-07-26 04:50:29.000000 lazyinit-0.0.262/lazyinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:51:36.857885 lazyinit-0.0.262/lazyinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      378 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      341 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:51:36.000000 lazyinit-0.0.262/lazyinit.egg-info/top_level.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:51:36.858476 lazyinit-0.0.262/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      843 2023-07-26 04:51:34.000000 lazyinit-0.0.262/setup.py
```

### Comparing `lazyinit-0.0.261/lazyinit/bash_config.txt` & `lazyinit-0.0.262/lazyinit/bash_config.txt`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.261/lazyinit/init.py` & `lazyinit-0.0.262/lazyinit/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,17 +143,16 @@
             run_cmd(torchaudio_install)
 
         elif step == "5":
             run_cmd([
                 "cd ~/",
                 "wget https://download.redis.io/redis-stable.tar.gz",
                 "tar -xzvf redis-stable.tar.gz",
-                "cd redis-stable",
+                "cd redis-stable/src",
                 "make",
-                "cd src",
                 "make install PREFIX=~/redis",
                 "cp {}/redis.conf ~/redis/bin/".format(pkg_current_path),
                 "~/redis/bin/redis-server ~/redis/bin/redis.conf",
             ])
             
         elif step == "6":
             run_cmd([
```

### Comparing `lazyinit-0.0.261/lazyinit/redis.conf` & `lazyinit-0.0.262/lazyinit/redis.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.261/lazyinit/run.py` & `lazyinit-0.0.262/lazyinit/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.261/lazyinit/utils.py` & `lazyinit-0.0.262/lazyinit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from bs4 import BeautifulSoup
 import requests as rq
 import pkg_resources
 import os
 from rich.console import Console
 import subprocess
+from rich.progress import track
 
 console = Console()
 
 def package_installed(package_name):
     """
     检查指定包是否已安装
     """
@@ -21,15 +22,16 @@
 def echo(msg, color="green"):
     console.print(msg, style=color)
 
 def run_cmd(cmd_list):
     if not isinstance(cmd_list, list):
         cmd_list = [cmd_list]
     outputs = []
-    for cmd in cmd_list:
+    for cmd in track(cmd_list, description="命令执行中..."):
+        echo(cmd, "blue")
         while True:
             exitcode, output = subprocess.getstatusoutput(cmd)
             if exitcode != 0:
                 echo("执行 {} 失败！".format(cmd), "#FF6AB3")
                 echo("可通过在下方修改命令继续执行，或者直接按下回车键忽略该错误：")
                 cmd = input()
                 if cmd == "":
```

### Comparing `lazyinit-0.0.261/setup.py` & `lazyinit-0.0.262/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='lazyinit',
-    version='0.0.261',
+    version='0.0.262',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init zhei environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

