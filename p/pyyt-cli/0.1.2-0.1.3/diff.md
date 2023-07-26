# Comparing `tmp/pyyt-cli-0.1.2.tar.gz` & `tmp/pyyt-cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyyt-cli-0.1.2.tar", last modified: Wed Jul 26 18:12:59 2023, max compression
+gzip compressed data, was "pyyt-cli-0.1.3.tar", last modified: Wed Jul 26 18:16:41 2023, max compression
```

## Comparing `pyyt-cli-0.1.2.tar` & `pyyt-cli-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:12:59.341749 pyyt-cli-0.1.2/
--rw-r--r--   0 dvitto     (501) staff       (20)     1211 2021-01-23 14:08:38.000000 pyyt-cli-0.1.2/LICENSE
--rw-r--r--   0 dvitto     (501) staff       (20)     1444 2023-07-26 18:12:59.341848 pyyt-cli-0.1.2/PKG-INFO
--rw-r--r--   0 dvitto     (501) staff       (20)      800 2023-07-26 17:46:23.000000 pyyt-cli-0.1.2/README.md
--rw-r--r--   0 dvitto     (501) staff       (20)       85 2023-07-26 17:53:17.000000 pyyt-cli-0.1.2/pyproject.toml
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:12:59.340131 pyyt-cli-0.1.2/pyyt_cli.egg-info/
--rw-r--r--   0 dvitto     (501) staff       (20)     1444 2023-07-26 18:12:59.000000 pyyt-cli-0.1.2/pyyt_cli.egg-info/PKG-INFO
--rw-r--r--   0 dvitto     (501) staff       (20)      320 2023-07-26 18:12:59.000000 pyyt-cli-0.1.2/pyyt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 dvitto     (501) staff       (20)        1 2023-07-26 18:12:59.000000 pyyt-cli-0.1.2/pyyt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       39 2023-07-26 18:12:59.000000 pyyt-cli-0.1.2/pyyt_cli.egg-info/entry_points.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       84 2023-07-26 18:12:59.000000 pyyt-cli-0.1.2/pyyt_cli.egg-info/requires.txt
--rw-r--r--   0 dvitto     (501) staff       (20)        4 2023-07-26 18:12:59.000000 pyyt-cli-0.1.2/pyyt_cli.egg-info/top_level.txt
--rw-r--r--   0 dvitto     (501) staff       (20)       67 2023-07-26 18:12:59.342189 pyyt-cli-0.1.2/setup.cfg
--rw-r--r--   0 dvitto     (501) staff       (20)     1754 2023-07-26 18:12:52.000000 pyyt-cli-0.1.2/setup.py
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:12:59.341095 pyyt-cli-0.1.2/src/
--rw-r--r--   0 dvitto     (501) staff       (20)        0 2023-07-26 16:02:06.000000 pyyt-cli-0.1.2/src/__init__.py
--rw-r--r--   0 dvitto     (501) staff       (20)      360 2023-07-26 15:44:13.000000 pyyt-cli-0.1.2/src/options.py
--rw-r--r--   0 dvitto     (501) staff       (20)     1301 2023-07-26 15:44:13.000000 pyyt-cli-0.1.2/src/pyyt.py
--rw-r--r--   0 dvitto     (501) staff       (20)     2729 2023-07-26 15:44:13.000000 pyyt-cli-0.1.2/src/utils.py
-drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:12:59.341512 pyyt-cli-0.1.2/tests/
--rw-r--r--   0 dvitto     (501) staff       (20)     2289 2023-07-26 16:45:33.000000 pyyt-cli-0.1.2/tests/test_pyyt.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:16:41.195151 pyyt-cli-0.1.3/
+-rw-r--r--   0 dvitto     (501) staff       (20)     1211 2021-01-23 14:08:38.000000 pyyt-cli-0.1.3/LICENSE
+-rw-r--r--   0 dvitto     (501) staff       (20)     1444 2023-07-26 18:16:41.195299 pyyt-cli-0.1.3/PKG-INFO
+-rw-r--r--   0 dvitto     (501) staff       (20)      800 2023-07-26 17:46:23.000000 pyyt-cli-0.1.3/README.md
+-rw-r--r--   0 dvitto     (501) staff       (20)       85 2023-07-26 17:53:17.000000 pyyt-cli-0.1.3/pyproject.toml
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:16:41.193340 pyyt-cli-0.1.3/pyyt_cli.egg-info/
+-rw-r--r--   0 dvitto     (501) staff       (20)     1444 2023-07-26 18:16:41.000000 pyyt-cli-0.1.3/pyyt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 dvitto     (501) staff       (20)      320 2023-07-26 18:16:41.000000 pyyt-cli-0.1.3/pyyt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)        1 2023-07-26 18:16:41.000000 pyyt-cli-0.1.3/pyyt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       39 2023-07-26 18:16:41.000000 pyyt-cli-0.1.3/pyyt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       83 2023-07-26 18:16:41.000000 pyyt-cli-0.1.3/pyyt_cli.egg-info/requires.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)        4 2023-07-26 18:16:41.000000 pyyt-cli-0.1.3/pyyt_cli.egg-info/top_level.txt
+-rw-r--r--   0 dvitto     (501) staff       (20)       67 2023-07-26 18:16:41.195667 pyyt-cli-0.1.3/setup.cfg
+-rw-r--r--   0 dvitto     (501) staff       (20)     1753 2023-07-26 18:16:31.000000 pyyt-cli-0.1.3/setup.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:16:41.194641 pyyt-cli-0.1.3/src/
+-rw-r--r--   0 dvitto     (501) staff       (20)        0 2023-07-26 16:02:06.000000 pyyt-cli-0.1.3/src/__init__.py
+-rw-r--r--   0 dvitto     (501) staff       (20)      360 2023-07-26 15:44:13.000000 pyyt-cli-0.1.3/src/options.py
+-rw-r--r--   0 dvitto     (501) staff       (20)     1301 2023-07-26 15:44:13.000000 pyyt-cli-0.1.3/src/pyyt.py
+-rw-r--r--   0 dvitto     (501) staff       (20)     2729 2023-07-26 15:44:13.000000 pyyt-cli-0.1.3/src/utils.py
+drwxr-xr-x   0 dvitto     (501) staff       (20)        0 2023-07-26 18:16:41.194922 pyyt-cli-0.1.3/tests/
+-rw-r--r--   0 dvitto     (501) staff       (20)     2289 2023-07-26 16:45:33.000000 pyyt-cli-0.1.3/tests/test_pyyt.py
```

### Comparing `pyyt-cli-0.1.2/LICENSE` & `pyyt-cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.2/PKG-INFO` & `pyyt-cli-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyt-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python script to download videos as audio from a given YouTube playlist/video
 Home-page: https://github.com/patillacode/pyyt
 Author: Patilla Code
 Author-email: patillacode@gmail.com
 License: Apache 2.0
 Keywords: converter,audio,youtube,download,mp3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyyt-cli-0.1.2/README.md` & `pyyt-cli-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.2/pyyt_cli.egg-info/PKG-INFO` & `pyyt-cli-0.1.3/pyyt_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyyt-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python script to download videos as audio from a given YouTube playlist/video
 Home-page: https://github.com/patillacode/pyyt
 Author: Patilla Code
 Author-email: patillacode@gmail.com
 License: Apache 2.0
 Keywords: converter,audio,youtube,download,mp3
 Classifier: Intended Audience :: Developers
```

### Comparing `pyyt-cli-0.1.2/setup.py` & `pyyt-cli-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         """Run all tests!"""
         errno = call(["py.test", "--cov=pyyt", "--cov-report=term-missing"])
         raise SystemExit(errno)
 
 
 setup(
     name="pyyt-cli",
-    version="0.1.2",
+    version="0.1.3",
     description="Python script to download videos as audio from a given YouTube playlist/video",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/patillacode/pyyt",
     author="Patilla Code",
     author_email="patillacode@gmail.com",
     license="Apache 2.0",
@@ -44,15 +44,15 @@
         "License :: Public Domain",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.11",
     ],
     keywords="converter, audio, youtube, download, mp3",
     packages=find_packages(exclude=["docs", "tests*", "downloads", "examples"]),
-    install_requires=["pyfiglet", "fsimple-term-menu", "yt-dlp", "termcolor"],
+    install_requires=["pyfiglet", "simple-term-menu", "yt-dlp", "termcolor"],
     extras_require={
         "test": ["coverage", "pytest", "pytest-cov", "mock"],
     },
     entry_points={
         "console_scripts": [
             "pyyt=src.pyyt:main",
         ],
```

### Comparing `pyyt-cli-0.1.2/src/pyyt.py` & `pyyt-cli-0.1.3/src/pyyt.py`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.2/src/utils.py` & `pyyt-cli-0.1.3/src/utils.py`

 * *Files identical despite different names*

### Comparing `pyyt-cli-0.1.2/tests/test_pyyt.py` & `pyyt-cli-0.1.3/tests/test_pyyt.py`

 * *Files identical despite different names*

