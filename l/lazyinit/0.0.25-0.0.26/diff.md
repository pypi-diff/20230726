# Comparing `tmp/lazyinit-0.0.25.tar.gz` & `tmp/lazyinit-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazyinit-0.0.25.tar", last modified: Wed Jul 26 04:28:14 2023, max compression
+gzip compressed data, was "lazyinit-0.0.26.tar", last modified: Wed Jul 26 04:34:19 2023, max compression
```

## Comparing `lazyinit-0.0.25.tar` & `lazyinit-0.0.26.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:28:14.464812 lazyinit-0.0.25/
--rw-r--r--   0 dengyifan   (501) staff       (20)       46 2023-07-26 04:25:33.000000 lazyinit-0.0.25/MANIFEST.in
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:28:14.464622 lazyinit-0.0.25/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.25/README.md
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:28:14.463192 lazyinit-0.0.25/lazyinit/
--rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.25/lazyinit/__init__.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.25/lazyinit/bash_config.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)     7833 2023-07-26 04:28:02.000000 lazyinit-0.0.25/lazyinit/init.py
--rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.25/lazyinit/redis.conf
--rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.25/lazyinit/run.py
--rw-r--r--   0 dengyifan   (501) staff       (20)     4880 2023-07-26 04:18:42.000000 lazyinit-0.0.25/lazyinit/utils.py
-drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:28:14.464339 lazyinit-0.0.25/lazyinit.egg-info/
--rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/PKG-INFO
--rw-r--r--   0 dengyifan   (501) staff       (20)      341 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/SOURCES.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/dependency_links.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/entry_points.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/requires.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:28:14.000000 lazyinit-0.0.25/lazyinit.egg-info/top_level.txt
--rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:28:14.464878 lazyinit-0.0.25/setup.cfg
--rw-r--r--   0 dengyifan   (501) staff       (20)      842 2023-07-26 04:28:12.000000 lazyinit-0.0.25/setup.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:34:19.493384 lazyinit-0.0.26/
+-rw-r--r--   0 dengyifan   (501) staff       (20)       65 2023-07-26 04:33:05.000000 lazyinit-0.0.26/MANIFEST.in
+-rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:34:19.493200 lazyinit-0.0.26/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      138 2023-07-23 13:52:05.000000 lazyinit-0.0.26/README.md
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:34:19.492015 lazyinit-0.0.26/lazyinit/
+-rw-r--r--   0 dengyifan   (501) staff       (20)        0 2023-07-23 14:24:47.000000 lazyinit-0.0.26/lazyinit/__init__.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     3876 2023-07-26 03:36:41.000000 lazyinit-0.0.26/lazyinit/bash_config.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)     8140 2023-07-26 04:34:00.000000 lazyinit-0.0.26/lazyinit/init.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)   106548 2023-07-26 03:36:41.000000 lazyinit-0.0.26/lazyinit/redis.conf
+-rw-r--r--   0 dengyifan   (501) staff       (20)     7011 2023-07-26 04:21:53.000000 lazyinit-0.0.26/lazyinit/run.py
+-rw-r--r--   0 dengyifan   (501) staff       (20)     4880 2023-07-26 04:18:42.000000 lazyinit-0.0.26/lazyinit/utils.py
+drwxr-xr-x   0 dengyifan   (501) staff       (20)        0 2023-07-26 04:34:19.492966 lazyinit-0.0.26/lazyinit.egg-info/
+-rw-r--r--   0 dengyifan   (501) staff       (20)      377 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/PKG-INFO
+-rw-r--r--   0 dengyifan   (501) staff       (20)      341 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/SOURCES.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        1 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/dependency_links.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       66 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/entry_points.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       25 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/requires.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)        9 2023-07-26 04:34:19.000000 lazyinit-0.0.26/lazyinit.egg-info/top_level.txt
+-rw-r--r--   0 dengyifan   (501) staff       (20)       38 2023-07-26 04:34:19.493442 lazyinit-0.0.26/setup.cfg
+-rw-r--r--   0 dengyifan   (501) staff       (20)      842 2023-07-26 04:34:18.000000 lazyinit-0.0.26/setup.py
```

### Comparing `lazyinit-0.0.25/lazyinit/bash_config.txt` & `lazyinit-0.0.26/lazyinit/bash_config.txt`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.25/lazyinit/init.py` & `lazyinit-0.0.26/lazyinit/init.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
         print("未找到 zhei-init 配置，即将注入配置到 ~/.bashrc（完成后可能需要重启初始化工具）")
         # ---------------------------------------------------------------------------- #
         #                         配置 Bash 环境变量                                     
         # ---------------------------------------------------------------------------- #
         bash = [
             "cd ~/",
             "cat {}/bash_config.txt >> ~/.bashrc".format(pkg_current_path),
-            "source ~/.bashrc",
         ]
         run_cmd(bash)
+        echo("运行 {} 以完成配置（运行后需要重启工具）".format("source ~/.bashrc"), "yellow")
         
     echo("")
     echo("")
     echo("")
     echo("      _____                          _      ____                  _")
     echo("     |  __ \\                        | |    |  _ \\                | |")
     echo("     | |__) |____      _____ _ __ __| |    | |_) |_   _          | |")
@@ -103,16 +103,20 @@
 
         elif step == "4":
             # ---------------------------------------------------------------------------- #
             #                         创建 zhei 环境                                     
             # ---------------------------------------------------------------------------- #
             echo("即将创建 zhei 环境，请在下方输入 Python 版本号，默认为 3.9：", "yellow")
             python_version = input()
+            if python_version == "":
+                python_version = "3.9"
             echo("即将创建 zhei 环境，请在下方输入环境名称，将会自动安装 zhei 包，默认名称为 zhei：", "yellow")
             env_name = input()
+            if env_name == "":
+                env_name = "zhei"
             zhei = [
                 "conda create -n {} python={}".format(env_name, python_version),
                 "conda activate {}".format(env_name),
                 "python -m pip install zhei --upgrade",
             ]
             run_cmd(zhei)
 
@@ -156,14 +160,16 @@
                 "cd ~/.ssh",
                 "ssh-keygen -t rsa",
                 "cat id_rsa.pub"
             ])
             
         elif step == "7":
             target_path = input("请输入项目路径（包含新的项目文件夹名），默认为 ~/code/zhei_project：")
+            if target_path == "":
+                target_path = "~/code/zhei_project"
             run_cmd([
                 "cp -r {}/ProjectTemplate {}".format(pkg_current_path, target_path),        
             ])
             
         elif step == "0":
             exit()
```

### Comparing `lazyinit-0.0.25/lazyinit/redis.conf` & `lazyinit-0.0.26/lazyinit/redis.conf`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.25/lazyinit/run.py` & `lazyinit-0.0.26/lazyinit/run.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.25/lazyinit/utils.py` & `lazyinit-0.0.26/lazyinit/utils.py`

 * *Files identical despite different names*

### Comparing `lazyinit-0.0.25/setup.py` & `lazyinit-0.0.26/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='lazyinit',
-    version='0.0.25',
+    version='0.0.26',
     author='deng1fan',
     author_email='dengyifan@iie.ac.cn',
     url='https://github.com/deng1fan',
     description=u'Init zhei environment.',
     long_description=open("README.md", "r", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

