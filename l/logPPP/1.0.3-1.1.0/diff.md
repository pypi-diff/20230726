# Comparing `tmp/logPPP-1.0.3.tar.gz` & `tmp/logPPP-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logPPP-1.0.3.tar", last modified: Wed Jul 12 11:34:35 2023, max compression
+gzip compressed data, was "logPPP-1.1.0.tar", last modified: Wed Jul 26 13:50:46 2023, max compression
```

## Comparing `logPPP-1.0.3.tar` & `logPPP-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.065303 logPPP-1.0.3/
--rw-rw-rw-   0        0        0      126 2023-07-12 11:34:35.064333 logPPP-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-07-12 11:13:39.000000 logPPP-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.058323 logPPP-1.0.3/logPPP.egg-info/
--rw-rw-rw-   0        0        0      126 2023-07-12 11:34:34.000000 logPPP-1.0.3/logPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-12 11:34:35.000000 logPPP-1.0.3/logPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 11:34:34.000000 logPPP-1.0.3/logPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-12 11:34:34.000000 logPPP-1.0.3/logPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 11:34:35.065303 logPPP-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-07-12 11:22:50.000000 logPPP-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.051378 logPPP-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-12 11:34:35.063337 logPPP-1.0.3/src/logPPP/
--rw-rw-rw-   0        0        0      116 2023-07-11 14:54:45.000000 logPPP-1.0.3/src/logPPP/_ConsoleColors.py
--rw-rw-rw-   0        0        0     1422 2023-07-12 11:34:34.000000 logPPP-1.0.3/src/logPPP/__init__.py
--rw-rw-rw-   0        0        0      453 2023-07-11 14:15:21.000000 logPPP-1.0.3/src/logPPP/_util.py
--rw-rw-rw-   0        0        0      373 2023-07-12 11:34:15.000000 logPPP-1.0.3/src/logPPP/logPPPLevel.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:50:46.532469 logPPP-1.1.0/
+-rw-rw-rw-   0        0        0      126 2023-07-26 13:50:46.532469 logPPP-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-07-26 10:16:17.000000 logPPP-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 13:50:46.516822 logPPP-1.1.0/logPPP.egg-info/
+-rw-rw-rw-   0        0        0      126 2023-07-26 13:50:46.000000 logPPP-1.1.0/logPPP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-07-26 13:50:46.000000 logPPP-1.1.0/logPPP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 13:50:46.000000 logPPP-1.1.0/logPPP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-26 13:50:46.000000 logPPP-1.1.0/logPPP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 13:50:46.532469 logPPP-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-07-26 10:16:17.000000 logPPP-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 13:50:46.516822 logPPP-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 13:50:46.516822 logPPP-1.1.0/src/logPPP/
+-rw-rw-rw-   0        0        0      116 2023-07-26 10:16:17.000000 logPPP-1.1.0/src/logPPP/_ConsoleColors.py
+-rw-rw-rw-   0        0        0     1687 2023-07-26 13:50:44.000000 logPPP-1.1.0/src/logPPP/__init__.py
+-rw-rw-rw-   0        0        0      453 2023-07-26 10:16:17.000000 logPPP-1.1.0/src/logPPP/_util.py
+-rw-rw-rw-   0        0        0      373 2023-07-26 10:16:17.000000 logPPP-1.1.0/src/logPPP/logPPPLevel.py
```

### Comparing `logPPP-1.0.3/src/logPPP/__init__.py` & `logPPP-1.1.0/src/logPPP/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import datetime
 
 from ._ConsoleColors import ConsoleColors
 from ._util import *
 from .logPPPLevel import logPPPLevel
 
-__all__ = ['__version__', 'logPPPLevel', 'info', 'warning', 'error', 'debug', 'critical']
-__version__ = '1.0.3'
+__all__ = ['__version__', 'IS_COLOR', 'LEVEL', 'logPPPLevel', 'info', 'warning', 'error', 'debug', 'critical']
+__version__ = '1.1.0'
+
+# 是否开启颜色
+IS_COLOR = True
 # 等级
-level = logPPPLevel.INFO
+LEVEL = logPPPLevel.INFO
 
 
 # 日志输出
-def _base(args, sep=' ', end='\n', file=None, _level=logPPPLevel.INFO, color=ConsoleColors.RESET):
+def _base(args, sep=' ', end='\n', file=None, _level=logPPPLevel.INFO, color=ConsoleColors.RESET, is_color=True):
     timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     args = "{:<20} {:<8} {}  {}".format(timestamp, get_caller_file_basename_path(), _level['name'], args)
-    args = f"{color}{args}{ConsoleColors.RESET}"
-    if _level['level'] >= level['level']:
+    if is_color is None and IS_COLOR or is_color is True:
+        args = f"{color}{args}{ConsoleColors.RESET}"
+    if _level['level'] >= LEVEL['level']:
         print(args, sep=sep, end=end, file=file)
 
 
 # info等级
-def info(args, sep=' ', end='\n', file=None):
-    _base(args, sep, end, file, logPPPLevel.INFO, ConsoleColors.RESET)
+def info(args, sep=' ', end='\n', file=None, is_color=None):
+    _base(args, sep, end, file, logPPPLevel.INFO, ConsoleColors.RESET, is_color)
 
 
 # warning等级
-def warning(args, sep=' ', end='\n', file=None):
-    _base(args, sep, end, file, logPPPLevel.WARNING, ConsoleColors.YELLOW)
+def warning(args, sep=' ', end='\n', file=None, is_color=None):
+    _base(args, sep, end, file, logPPPLevel.WARNING, ConsoleColors.YELLOW, is_color)
 
 
 # error等级
-def error(args, sep=' ', end='\n', file=None):
-    _base(args, sep, end, file, logPPPLevel.ERROR, ConsoleColors.RED)
+def error(args, sep=' ', end='\n', file=None, is_color=None):
+    _base(args, sep, end, file, logPPPLevel.ERROR, ConsoleColors.RED, is_color)
 
 
 # debug等级
-def debug(args, sep=' ', end='\n', file=None):
-    _base(args, sep, end, file, logPPPLevel.DEBUG, ConsoleColors.RED)
+def debug(args, sep=' ', end='\n', file=None, is_color=None):
+    _base(args, sep, end, file, logPPPLevel.DEBUG, ConsoleColors.RED, is_color)
 
 
 # critical等级
-def critical(args, sep=' ', end='\n', file=None):
-    _base(args, sep, end, file, logPPPLevel.CRITICAL, ConsoleColors.RED)
+def critical(args, sep=' ', end='\n', file=None, is_color=None):
+    _base(args, sep, end, file, logPPPLevel.CRITICAL, ConsoleColors.RED, is_color)
```

