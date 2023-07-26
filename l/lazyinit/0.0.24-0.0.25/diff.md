# Comparing `tmp/lazyinit-0.0.24.tar.gz` & `tmp/lazyinit-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyinit-0.0.24.tar", last modified: Wed Jul 26 04:25:41 2023, max compression
+gzip compressed data, was "lazyinit-0.0.25.tar", last modified: Wed Jul 26 04:28:14 2023, max compression
```

## Comparing `lazyinit-0.0.24.tar` & `lazyinit-0.0.25.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:25:41.948838 lazyinit-0.0.24/
--rw-r--r--   0 dengyifan   (501) staff       (20)       46 2023-07-26 04:25:33.000000 lazyinit-0.0.24/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:25:41.948645 lazyinit-0.0.24/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.24/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:25:41.947449 lazyinit-0.0.24/lazyinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.24/lazyinit/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.24/lazyinit/bash_config.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     7899 2023-07-26 04:21:00.000000 lazyinit-0.0.24/lazyinit/init.py
--rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.24/lazyinit/redis.conf
--rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.24/lazyinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4880 2023-07-26 04:18:42.000000 lazyinit-0.0.24/lazyinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:25:41.948351 lazyinit-0.0.24/lazyinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:25:41.000000 lazyinit-0.0.24/lazyinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      341 2023-07-26 04:25:41.000000 lazyinit-0.0.24/lazyinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:25:41.000000 lazyinit-0.0.24/lazyinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:25:41.000000 lazyinit-0.0.24/lazyinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:25:41.000000 lazyinit-0.0.24/lazyinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:25:41.000000 lazyinit-0.0.24/lazyinit.egg-info/top_level.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:25:41.948901 lazyinit-0.0.24/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      842 2023-07-26 04:25:39.000000 lazyinit-0.0.24/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:28:14.464812 lazyinit-0.0.25/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       46 2023-07-26 04:25:33.000000 lazyinit-0.0.25/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:28:14.464622 lazyinit-0.0.25/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.25/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:28:14.463192 lazyinit-0.0.25/lazyinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.25/lazyinit/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.25/lazyinit/bash_config.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7833 2023-07-26 04:28:02.000000 lazyinit-0.0.25/lazyinit/init.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.25/lazyinit/redis.conf
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.25/lazyinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4880 2023-07-26 04:18:42.000000 lazyinit-0.0.25/lazyinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:28:14.464339 lazyinit-0.0.25/lazyinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      341 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/top_level.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:28:14.464878 lazyinit-0.0.25/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      842 2023-07-26 04:28:12.000000 lazyinit-0.0.25/setup.py
```

### Comparing `lazyinit-0.0.24/lazyinit/bash_config.txt` & `lazyinit-0.0.25/lazyinit/bash_config.txt`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.24/lazyinit/init.py` & `lazyinit-0.0.25/lazyinit/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         else:        
             echo("请在 bash 环境下运行本工具！")
         echo("您可以通过以下命令查看所支持的 Shell 类型：\ncat /etc/shells", "red")
         echo("您可以通过以下命令切换 Shell 类型：\nchsh -s /bin/bash", "red")
         exit()
 
     pkg_current_path = os.path.dirname(os.path.abspath(__file__))
-    pkg_current_path = os.path.join(pkg_current_path, "lazyinit")
     python_version = "3.9"
     env_name = "zhei"
 
     # 读取 ~/.bashrc 文件内容
     if not os.path.exists("~/.bashrc"):
         run_cmd("touch ~/.bashrc")
     bashrc = run_cmd("cat ~/.bashrc")[0]
```

### Comparing `lazyinit-0.0.24/lazyinit/redis.conf` & `lazyinit-0.0.25/lazyinit/redis.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.24/lazyinit/run.py` & `lazyinit-0.0.25/lazyinit/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.24/lazyinit/utils.py` & `lazyinit-0.0.25/lazyinit/utils.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.24/setup.py` & `lazyinit-0.0.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='lazyinit',
-    version='0.0.24',
+    version='0.0.25',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init zhei environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

