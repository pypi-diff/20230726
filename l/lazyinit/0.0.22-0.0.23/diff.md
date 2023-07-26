# Comparing `tmp/lazyinit-0.0.22.tar.gz` & `tmp/lazyinit-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyinit-0.0.22.tar", last modified: Wed Jul 26 04:18:53 2023, max compression
+gzip compressed data, was "lazyinit-0.0.23.tar", last modified: Wed Jul 26 04:22:05 2023, max compression
```

## Comparing `lazyinit-0.0.22.tar` & `lazyinit-0.0.23.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:18:53.339991 lazyinit-0.0.22/
--rw-r--r--   0 dengyifan   (501) staff       (20)       21 2023-07-23 14:48:03.000000 lazyinit-0.0.22/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:18:53.339703 lazyinit-0.0.22/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.22/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:18:53.336958 lazyinit-0.0.22/lazyinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.22/lazyinit/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     7833 2023-07-26 04:13:10.000000 lazyinit-0.0.22/lazyinit/init.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:15:58.000000 lazyinit-0.0.22/lazyinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4880 2023-07-26 04:18:42.000000 lazyinit-0.0.22/lazyinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:18:53.338233 lazyinit-0.0.22/lazyinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      296 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:18:53.000000 lazyinit-0.0.22/lazyinit.egg-info/top_level.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:18:53.340075 lazyinit-0.0.22/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      842 2023-07-26 04:18:50.000000 lazyinit-0.0.22/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:22:05.115321 lazyinit-0.0.23/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       21 2023-07-23 14:48:03.000000 lazyinit-0.0.23/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:22:05.115146 lazyinit-0.0.23/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.23/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:22:05.114007 lazyinit-0.0.23/lazyinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.23/lazyinit/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7899 2023-07-26 04:21:00.000000 lazyinit-0.0.23/lazyinit/init.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.23/lazyinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4880 2023-07-26 04:18:42.000000 lazyinit-0.0.23/lazyinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:22:05.114927 lazyinit-0.0.23/lazyinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:22:05.000000 lazyinit-0.0.23/lazyinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      296 2023-07-26 04:22:05.000000 lazyinit-0.0.23/lazyinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:22:05.000000 lazyinit-0.0.23/lazyinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:22:05.000000 lazyinit-0.0.23/lazyinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:22:05.000000 lazyinit-0.0.23/lazyinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:22:05.000000 lazyinit-0.0.23/lazyinit.egg-info/top_level.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:22:05.115374 lazyinit-0.0.23/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      842 2023-07-26 04:22:01.000000 lazyinit-0.0.23/setup.py
```

### Comparing `lazyinit-0.0.22/lazyinit/init.py` & `lazyinit-0.0.23/lazyinit/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         else:        
             echo("请在 bash 环境下运行本工具！")
         echo("您可以通过以下命令查看所支持的 Shell 类型：\ncat /etc/shells", "red")
         echo("您可以通过以下命令切换 Shell 类型：\nchsh -s /bin/bash", "red")
         exit()
 
     pkg_current_path = os.path.dirname(os.path.abspath(__file__))
+    pkg_current_path = os.path.join(pkg_current_path, "lazyinit")
     python_version = "3.9"
     env_name = "zhei"
 
     # 读取 ~/.bashrc 文件内容
     if not os.path.exists("~/.bashrc"):
         run_cmd("touch ~/.bashrc")
     bashrc = run_cmd("cat ~/.bashrc")[0]
```

### Comparing `lazyinit-0.0.22/lazyinit/run.py` & `lazyinit-0.0.23/lazyinit/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.22/lazyinit/utils.py` & `lazyinit-0.0.23/lazyinit/utils.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.22/setup.py` & `lazyinit-0.0.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='lazyinit',
-    version='0.0.22',
+    version='0.0.23',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init zhei environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

