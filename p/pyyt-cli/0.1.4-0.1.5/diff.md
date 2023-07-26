# Comparing `tmp/pyyt-cli-0.1.4.tar.gz` & `tmp/pyyt-cli-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyt-cli-0.1.4.tar", last modified: Wed Jul 26 18:20:50 2023, max compression
+gzip compressed data, was "pyyt-cli-0.1.5.tar", last modified: Wed Jul 26 18:51:33 2023, max compression
```

## Comparing `pyyt-cli-0.1.4.tar` & `pyyt-cli-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:20:50.799860 pyyt-cli-0.1.4/
--rw-r--r--   0 dvitto     (501) staff       (20)     1211 2021-01-23 14:08:38.000000 pyyt-cli-0.1.4/LICENSE
--rw-r--r--   0 dvitto     (501) staff       (20)     1444 2023-07-26 18:20:50.800031 pyyt-cli-0.1.4/PKG-INFO
--rw-r--r--   0 dvitto     (501) staff       (20)      800 2023-07-26 17:46:23.000000 pyyt-cli-0.1.4/README.md
--rw-r--r--   0 dvitto     (501) staff       (20)       85 2023-07-26 17:53:17.000000 pyyt-cli-0.1.4/pyproject.toml
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:20:50.797087 pyyt-cli-0.1.4/pyyt_cli.egg-info/
--rw-r--r--   0 dvitto     (501) staff       (20)     1444 2023-07-26 18:20:50.000000 pyyt-cli-0.1.4/pyyt_cli.egg-info/PKG-INFO
--rw-r--r--   0 dvitto     (501) staff       (20)      320 2023-07-26 18:20:50.000000 pyyt-cli-0.1.4/pyyt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 dvitto     (501) staff       (20)        1 2023-07-26 18:20:50.000000 pyyt-cli-0.1.4/pyyt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       39 2023-07-26 18:20:50.000000 pyyt-cli-0.1.4/pyyt_cli.egg-info/entry_points.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       83 2023-07-26 18:20:50.000000 pyyt-cli-0.1.4/pyyt_cli.egg-info/requires.txt
--rw-r--r--   0 dvitto     (501) staff       (20)        4 2023-07-26 18:20:50.000000 pyyt-cli-0.1.4/pyyt_cli.egg-info/top_level.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       67 2023-07-26 18:20:50.800704 pyyt-cli-0.1.4/setup.cfg
--rw-r--r--   0 dvitto     (501) staff       (20)     1769 2023-07-26 18:19:54.000000 pyyt-cli-0.1.4/setup.py
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:20:50.799028 pyyt-cli-0.1.4/src/
--rw-r--r--   0 dvitto     (501) staff       (20)        0 2023-07-26 16:02:06.000000 pyyt-cli-0.1.4/src/__init__.py
--rw-r--r--   0 dvitto     (501) staff       (20)      360 2023-07-26 15:44:13.000000 pyyt-cli-0.1.4/src/options.py
--rw-r--r--   0 dvitto     (501) staff       (20)     1302 2023-07-26 18:19:26.000000 pyyt-cli-0.1.4/src/pyyt.py
--rw-r--r--   0 dvitto     (501) staff       (20)     2729 2023-07-26 15:44:13.000000 pyyt-cli-0.1.4/src/utils.py
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:20:50.799473 pyyt-cli-0.1.4/tests/
--rw-r--r--   0 dvitto     (501) staff       (20)     2289 2023-07-26 16:45:33.000000 pyyt-cli-0.1.4/tests/test_pyyt.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:51:33.425730 pyyt-cli-0.1.5/
+-rw-r--r--   0 dvitto     (501) staff       (20)     1211 2021-01-23 14:08:38.000000 pyyt-cli-0.1.5/LICENSE
+-rw-r--r--   0 dvitto     (501) staff       (20)     1444 2023-07-26 18:51:33.425842 pyyt-cli-0.1.5/PKG-INFO
+-rw-r--r--   0 dvitto     (501) staff       (20)      800 2023-07-26 17:46:23.000000 pyyt-cli-0.1.5/README.md
+-rw-r--r--   0 dvitto     (501) staff       (20)       85 2023-07-26 17:53:17.000000 pyyt-cli-0.1.5/pyproject.toml
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:51:33.423839 pyyt-cli-0.1.5/pyyt_cli.egg-info/
+-rw-r--r--   0 dvitto     (501) staff       (20)     1444 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 dvitto     (501) staff       (20)      320 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)        1 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       39 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       83 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/requires.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)        4 2023-07-26 18:51:33.000000 pyyt-cli-0.1.5/pyyt_cli.egg-info/top_level.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       67 2023-07-26 18:51:33.426217 pyyt-cli-0.1.5/setup.cfg
+-rw-r--r--   0 dvitto     (501) staff       (20)     1769 2023-07-26 18:51:25.000000 pyyt-cli-0.1.5/setup.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:51:33.425010 pyyt-cli-0.1.5/src/
+-rw-r--r--   0 dvitto     (501) staff       (20)        0 2023-07-26 16:02:06.000000 pyyt-cli-0.1.5/src/__init__.py
+-rw-r--r--   0 dvitto     (501) staff       (20)      360 2023-07-26 15:44:13.000000 pyyt-cli-0.1.5/src/options.py
+-rw-r--r--   0 dvitto     (501) staff       (20)     1302 2023-07-26 18:19:26.000000 pyyt-cli-0.1.5/src/pyyt.py
+-rw-r--r--   0 dvitto     (501) staff       (20)     2730 2023-07-26 18:21:52.000000 pyyt-cli-0.1.5/src/utils.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:51:33.425356 pyyt-cli-0.1.5/tests/
+-rw-r--r--   0 dvitto     (501) staff       (20)     2289 2023-07-26 16:45:33.000000 pyyt-cli-0.1.5/tests/test_pyyt.py
```

### Comparing `pyyt-cli-0.1.4/LICENSE` & `pyyt-cli-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.4/PKG-INFO` & `pyyt-cli-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyt-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python script to download videos as audio from a given YouTube playlist/video
 Home-page: https://github.com/patillacode/pyyt
 Author: Patilla Code
 Author-email: patillacode@gmail.com
 License: Apache 2.0
 Keywords: converter,audio,youtube,download,mp3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyyt-cli-0.1.4/README.md` & `pyyt-cli-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.4/pyyt_cli.egg-info/PKG-INFO` & `pyyt-cli-0.1.5/pyyt_cli.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyt-cli
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python script to download videos as audio from a given YouTube playlist/video
 Home-page: https://github.com/patillacode/pyyt
 Author: Patilla Code
 Author-email: patillacode@gmail.com
 License: Apache 2.0
 Keywords: converter,audio,youtube,download,mp3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyyt-cli-0.1.4/setup.py` & `pyyt-cli-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """Run all tests!"""
         errno = call(["py.test", "--cov=pyyt", "--cov-report=term-missing"])
         raise SystemExit(errno)
 
 
 setup(
     name="pyyt-cli",
-    version="0.1.4",
+    version="0.1.5",
     description=(
         "Python script to download videos as audio from a given YouTube playlist/video"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/patillacode/pyyt",
     author="Patilla Code",
```

### Comparing `pyyt-cli-0.1.4/src/pyyt.py` & `pyyt-cli-0.1.5/src/pyyt.py`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.4/src/utils.py` & `pyyt-cli-0.1.5/src/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import yt_dlp
 
 from pyfiglet import Figlet
 from simple_term_menu import TerminalMenu
 from termcolor import colored
 
-from options import ydl_opts
+from .options import ydl_opts
 
 
 def menu(selectable_items: List[str]) -> int:
     """
     Display a terminal menu and allow the user to select an item.
 
     Args:
```

### Comparing `pyyt-cli-0.1.4/tests/test_pyyt.py` & `pyyt-cli-0.1.5/tests/test_pyyt.py`

 * *Files identical despite different names*

