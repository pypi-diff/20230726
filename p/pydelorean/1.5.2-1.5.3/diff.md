# Comparing `tmp/pydelorean-1.5.2.tar.gz` & `tmp/pydelorean-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelorean-1.5.2.tar", last modified: Tue Jul 25 21:56:25 2023, max compression
+gzip compressed data, was "pydelorean-1.5.3.tar", last modified: Tue Jul 25 21:58:15 2023, max compression
```

## Comparing `pydelorean-1.5.2.tar` & `pydelorean-1.5.3.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:56:25.045474 pydelorean-1.5.2/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    10173 2023-07-25 21:49:28.000000 pydelorean-1.5.2/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2666 2023-07-25 21:56:25.045474 pydelorean-1.5.2/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2192 2023-07-25 21:49:08.000000 pydelorean-1.5.2/README.md
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:56:25.045474 pydelorean-1.5.2/pydelorean/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1007 2023-07-25 21:50:26.000000 pydelorean-1.5.2/pydelorean/__init__.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:56:25.045474 pydelorean-1.5.2/pydelorean/base/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      635 2023-07-25 21:51:03.000000 pydelorean-1.5.2/pydelorean/base/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2521 2023-07-25 21:51:10.000000 pydelorean-1.5.2/pydelorean/base/forest.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1844 2023-07-25 21:51:15.000000 pydelorean-1.5.2/pydelorean/base/node.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3712 2023-07-25 21:50:12.000000 pydelorean-1.5.2/pydelorean/delorean.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      784 2023-07-25 21:50:07.000000 pydelorean-1.5.2/pydelorean/errors.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-07-25 21:50:02.000000 pydelorean-1.5.2/pydelorean/files.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:56:25.045474 pydelorean-1.5.2/pydelorean/parser/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1266 2023-07-25 21:50:45.000000 pydelorean-1.5.2/pydelorean/parser/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2538 2023-07-25 21:50:52.000000 pydelorean-1.5.2/pydelorean/parser/parser.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     5803 2023-07-25 21:50:58.000000 pydelorean-1.5.2/pydelorean/parser/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:56:25.045474 pydelorean-1.5.2/pydelorean/tools/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3329 2023-07-25 21:50:38.000000 pydelorean-1.5.2/pydelorean/tools/__init__.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:56:25.045474 pydelorean-1.5.2/pydelorean.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2666 2023-07-25 21:56:24.000000 pydelorean-1.5.2/pydelorean.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      474 2023-07-25 21:56:24.000000 pydelorean-1.5.2/pydelorean.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-25 21:56:24.000000 pydelorean-1.5.2/pydelorean.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-25 21:56:24.000000 pydelorean-1.5.2/pydelorean.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-25 21:56:24.000000 pydelorean-1.5.2/pydelorean.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-25 21:56:25.045474 pydelorean-1.5.2/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1012 2023-07-25 21:56:22.000000 pydelorean-1.5.2/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    10173 2023-07-25 21:49:28.000000 pydelorean-1.5.3/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       41 2023-07-25 21:57:13.000000 pydelorean-1.5.3/MANIFEST.in
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2666 2023-07-25 21:58:15.848250 pydelorean-1.5.3/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2192 2023-07-25 21:49:08.000000 pydelorean-1.5.3/README.md
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/media/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    51209 2023-06-09 20:40:37.000000 pydelorean-1.5.3/media/image.png
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/pydelorean/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1007 2023-07-25 21:50:26.000000 pydelorean-1.5.3/pydelorean/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/pydelorean/base/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      635 2023-07-25 21:51:03.000000 pydelorean-1.5.3/pydelorean/base/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2521 2023-07-25 21:51:10.000000 pydelorean-1.5.3/pydelorean/base/forest.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1844 2023-07-25 21:51:15.000000 pydelorean-1.5.3/pydelorean/base/node.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3712 2023-07-25 21:50:12.000000 pydelorean-1.5.3/pydelorean/delorean.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      784 2023-07-25 21:50:07.000000 pydelorean-1.5.3/pydelorean/errors.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-07-25 21:50:02.000000 pydelorean-1.5.3/pydelorean/files.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/pydelorean/parser/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1266 2023-07-25 21:50:45.000000 pydelorean-1.5.3/pydelorean/parser/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2538 2023-07-25 21:50:52.000000 pydelorean-1.5.3/pydelorean/parser/parser.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     5803 2023-07-25 21:50:58.000000 pydelorean-1.5.3/pydelorean/parser/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/pydelorean/tools/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3329 2023-07-25 21:50:38.000000 pydelorean-1.5.3/pydelorean/tools/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/pydelorean.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2666 2023-07-25 21:58:15.000000 pydelorean-1.5.3/pydelorean.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      519 2023-07-25 21:58:15.000000 pydelorean-1.5.3/pydelorean.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-25 21:58:15.000000 pydelorean-1.5.3/pydelorean.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-25 21:58:15.000000 pydelorean-1.5.3/pydelorean.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-25 21:58:15.000000 pydelorean-1.5.3/pydelorean.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       83 2023-07-10 10:39:31.000000 pydelorean-1.5.3/requirements.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-25 21:58:15.848250 pydelorean-1.5.3/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1012 2023-07-25 21:58:12.000000 pydelorean-1.5.3/setup.py
```

### Comparing `pydelorean-1.5.2/LICENSE` & `pydelorean-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/PKG-INFO` & `pydelorean-1.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 1.5.2
+Version: 1.5.3
 Summary: A package to convert between markup documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.2.zip
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.3.zip
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img style="float: left; padding:20px" src="media/image.svg" alt="pydelorean" width="75"/>
```

### Comparing `pydelorean-1.5.2/README.md` & `pydelorean-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/__init__.py` & `pydelorean-1.5.3/pydelorean/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/base/__init__.py` & `pydelorean-1.5.3/pydelorean/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/base/forest.py` & `pydelorean-1.5.3/pydelorean/base/forest.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/base/node.py` & `pydelorean-1.5.3/pydelorean/base/node.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/delorean.py` & `pydelorean-1.5.3/pydelorean/delorean.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/errors.py` & `pydelorean-1.5.3/pydelorean/errors.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/files.py` & `pydelorean-1.5.3/pydelorean/files.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/parser/__init__.py` & `pydelorean-1.5.3/pydelorean/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/parser/parser.py` & `pydelorean-1.5.3/pydelorean/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/parser/utils.py` & `pydelorean-1.5.3/pydelorean/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean/tools/__init__.py` & `pydelorean-1.5.3/pydelorean/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.2/pydelorean.egg-info/PKG-INFO` & `pydelorean-1.5.3/pydelorean.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 1.5.2
+Version: 1.5.3
 Summary: A package to convert between markup documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.2.zip
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.3.zip
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img style="float: left; padding:20px" src="media/image.svg" alt="pydelorean" width="75"/>
```

### Comparing `pydelorean-1.5.2/setup.py` & `pydelorean-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '1.5.2'
+VERSION = '1.5.3'
 DESCRIPTION = 'A package to convert between markup documents and a forest data structure for efficient processing.'
 
 setup(
     name = "pydelorean",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
```

