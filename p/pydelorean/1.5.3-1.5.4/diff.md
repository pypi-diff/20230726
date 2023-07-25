# Comparing `tmp/pydelorean-1.5.3.tar.gz` & `tmp/pydelorean-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelorean-1.5.3.tar", last modified: Tue Jul 25 21:58:15 2023, max compression
+gzip compressed data, was "pydelorean-1.5.4.tar", last modified: Tue Jul 25 22:13:23 2023, max compression
```

## Comparing `pydelorean-1.5.3.tar` & `pydelorean-1.5.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    10173 2023-07-25 21:49:28.000000 pydelorean-1.5.3/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       41 2023-07-25 21:57:13.000000 pydelorean-1.5.3/MANIFEST.in
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2666 2023-07-25 21:58:15.848250 pydelorean-1.5.3/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2192 2023-07-25 21:49:08.000000 pydelorean-1.5.3/README.md
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/media/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    51209 2023-06-09 20:40:37.000000 pydelorean-1.5.3/media/image.png
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/pydelorean/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1007 2023-07-25 21:50:26.000000 pydelorean-1.5.3/pydelorean/__init__.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/pydelorean/base/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      635 2023-07-25 21:51:03.000000 pydelorean-1.5.3/pydelorean/base/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2521 2023-07-25 21:51:10.000000 pydelorean-1.5.3/pydelorean/base/forest.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1844 2023-07-25 21:51:15.000000 pydelorean-1.5.3/pydelorean/base/node.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3712 2023-07-25 21:50:12.000000 pydelorean-1.5.3/pydelorean/delorean.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      784 2023-07-25 21:50:07.000000 pydelorean-1.5.3/pydelorean/errors.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-07-25 21:50:02.000000 pydelorean-1.5.3/pydelorean/files.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/pydelorean/parser/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1266 2023-07-25 21:50:45.000000 pydelorean-1.5.3/pydelorean/parser/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2538 2023-07-25 21:50:52.000000 pydelorean-1.5.3/pydelorean/parser/parser.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     5803 2023-07-25 21:50:58.000000 pydelorean-1.5.3/pydelorean/parser/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/pydelorean/tools/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3329 2023-07-25 21:50:38.000000 pydelorean-1.5.3/pydelorean/tools/__init__.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 21:58:15.848250 pydelorean-1.5.3/pydelorean.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2666 2023-07-25 21:58:15.000000 pydelorean-1.5.3/pydelorean.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      519 2023-07-25 21:58:15.000000 pydelorean-1.5.3/pydelorean.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-25 21:58:15.000000 pydelorean-1.5.3/pydelorean.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-25 21:58:15.000000 pydelorean-1.5.3/pydelorean.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-25 21:58:15.000000 pydelorean-1.5.3/pydelorean.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       83 2023-07-10 10:39:31.000000 pydelorean-1.5.3/requirements.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-25 21:58:15.848250 pydelorean-1.5.3/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1012 2023-07-25 21:58:12.000000 pydelorean-1.5.3/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 22:13:23.278717 pydelorean-1.5.4/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    10173 2023-07-25 21:49:28.000000 pydelorean-1.5.4/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       41 2023-07-25 21:57:13.000000 pydelorean-1.5.4/MANIFEST.in
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2605 2023-07-25 22:13:23.278717 pydelorean-1.5.4/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2131 2023-07-25 22:06:24.000000 pydelorean-1.5.4/README.md
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 22:13:23.278717 pydelorean-1.5.4/media/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    51209 2023-06-09 20:40:37.000000 pydelorean-1.5.4/media/image.png
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 22:13:23.278717 pydelorean-1.5.4/pydelorean/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1007 2023-07-25 21:50:26.000000 pydelorean-1.5.4/pydelorean/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 22:13:23.278717 pydelorean-1.5.4/pydelorean/base/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      635 2023-07-25 21:51:03.000000 pydelorean-1.5.4/pydelorean/base/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2521 2023-07-25 21:51:10.000000 pydelorean-1.5.4/pydelorean/base/forest.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1844 2023-07-25 21:51:15.000000 pydelorean-1.5.4/pydelorean/base/node.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3712 2023-07-25 21:50:12.000000 pydelorean-1.5.4/pydelorean/delorean.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      784 2023-07-25 21:50:07.000000 pydelorean-1.5.4/pydelorean/errors.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-07-25 21:50:02.000000 pydelorean-1.5.4/pydelorean/files.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 22:13:23.278717 pydelorean-1.5.4/pydelorean/parser/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1266 2023-07-25 21:50:45.000000 pydelorean-1.5.4/pydelorean/parser/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2538 2023-07-25 21:50:52.000000 pydelorean-1.5.4/pydelorean/parser/parser.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     5803 2023-07-25 21:50:58.000000 pydelorean-1.5.4/pydelorean/parser/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 22:13:23.278717 pydelorean-1.5.4/pydelorean/tools/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3329 2023-07-25 21:50:38.000000 pydelorean-1.5.4/pydelorean/tools/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-25 22:13:23.278717 pydelorean-1.5.4/pydelorean.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2605 2023-07-25 22:13:23.000000 pydelorean-1.5.4/pydelorean.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      519 2023-07-25 22:13:23.000000 pydelorean-1.5.4/pydelorean.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-25 22:13:23.000000 pydelorean-1.5.4/pydelorean.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-25 22:13:23.000000 pydelorean-1.5.4/pydelorean.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-25 22:13:23.000000 pydelorean-1.5.4/pydelorean.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       83 2023-07-10 10:39:31.000000 pydelorean-1.5.4/requirements.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-25 22:13:23.278717 pydelorean-1.5.4/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1012 2023-07-25 22:13:17.000000 pydelorean-1.5.4/setup.py
```

### Comparing `pydelorean-1.5.3/LICENSE` & `pydelorean-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/PKG-INFO` & `pydelorean-1.5.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 1.5.3
+Version: 1.5.4
 Summary: A package to convert between markup documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.3.zip
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.4.zip
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img style="float: left; padding:20px" src="media/image.svg" alt="pydelorean" width="75"/>
+<img style="float: left; padding:20px" src="media/image.png" alt="pydelorean" width="125"/>
 
 # delorean
 
 A library to convert markup documents into tree data structures and
 vice versa. There is greater functionality available to modify, prune,
 add and delete parts of documents when there are in the MarkdownTree
 structure.
@@ -78,18 +78,18 @@
 
 For a usage guide, access the `samples/` directory or check out the
 documentation page here - [nil](nil)
 
 ## Features
 
 Some of the features of this library are:
+
 - forest data structure for Markdown, reStructuredText, AsciiDoc, JSON, YAML and XML.
 - 'cleaning' of documents to remove unwanted elements.
-- document manipulation using the tree data structure. 
-
-Refer to the FEATURES.md file for more information or you can visit the documentation page here - [nil](nil)
+- document manipulation using the tree data structure.
+- document generation from tree data structure.
 
 ## License
 
 This project is licensed under the Apache 2.0 License. A copy of the license can be found in the LICENSE file.
```

### Comparing `pydelorean-1.5.3/README.md` & `pydelorean-1.5.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img style="float: left; padding:20px" src="media/image.svg" alt="pydelorean" width="75"/>
+<img style="float: left; padding:20px" src="media/image.png" alt="pydelorean" width="125"/>
 
 # delorean
 
 A library to convert markup documents into tree data structures and
 vice versa. There is greater functionality available to modify, prune,
 add and delete parts of documents when there are in the MarkdownTree
 structure.
@@ -64,16 +64,16 @@
 
 For a usage guide, access the `samples/` directory or check out the
 documentation page here - [nil](nil)
 
 ## Features
 
 Some of the features of this library are:
+
 - forest data structure for Markdown, reStructuredText, AsciiDoc, JSON, YAML and XML.
 - 'cleaning' of documents to remove unwanted elements.
-- document manipulation using the tree data structure. 
-
-Refer to the FEATURES.md file for more information or you can visit the documentation page here - [nil](nil)
+- document manipulation using the tree data structure.
+- document generation from tree data structure.
 
 ## License
 
 This project is licensed under the Apache 2.0 License. A copy of the license can be found in the LICENSE file.
```

### Comparing `pydelorean-1.5.3/media/image.png` & `pydelorean-1.5.4/media/image.png`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/__init__.py` & `pydelorean-1.5.4/pydelorean/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/base/__init__.py` & `pydelorean-1.5.4/pydelorean/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/base/forest.py` & `pydelorean-1.5.4/pydelorean/base/forest.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/base/node.py` & `pydelorean-1.5.4/pydelorean/base/node.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/delorean.py` & `pydelorean-1.5.4/pydelorean/delorean.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/errors.py` & `pydelorean-1.5.4/pydelorean/errors.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/files.py` & `pydelorean-1.5.4/pydelorean/files.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/parser/__init__.py` & `pydelorean-1.5.4/pydelorean/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/parser/parser.py` & `pydelorean-1.5.4/pydelorean/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/parser/utils.py` & `pydelorean-1.5.4/pydelorean/parser/utils.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean/tools/__init__.py` & `pydelorean-1.5.4/pydelorean/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/pydelorean.egg-info/PKG-INFO` & `pydelorean-1.5.4/pydelorean.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 1.5.3
+Version: 1.5.4
 Summary: A package to convert between markup documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.3.zip
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.5.4.zip
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-<img style="float: left; padding:20px" src="media/image.svg" alt="pydelorean" width="75"/>
+<img style="float: left; padding:20px" src="media/image.png" alt="pydelorean" width="125"/>
 
 # delorean
 
 A library to convert markup documents into tree data structures and
 vice versa. There is greater functionality available to modify, prune,
 add and delete parts of documents when there are in the MarkdownTree
 structure.
@@ -78,18 +78,18 @@
 
 For a usage guide, access the `samples/` directory or check out the
 documentation page here - [nil](nil)
 
 ## Features
 
 Some of the features of this library are:
+
 - forest data structure for Markdown, reStructuredText, AsciiDoc, JSON, YAML and XML.
 - 'cleaning' of documents to remove unwanted elements.
-- document manipulation using the tree data structure. 
-
-Refer to the FEATURES.md file for more information or you can visit the documentation page here - [nil](nil)
+- document manipulation using the tree data structure.
+- document generation from tree data structure.
 
 ## License
 
 This project is licensed under the Apache 2.0 License. A copy of the license can be found in the LICENSE file.
```

### Comparing `pydelorean-1.5.3/pydelorean.egg-info/SOURCES.txt` & `pydelorean-1.5.4/pydelorean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydelorean-1.5.3/setup.py` & `pydelorean-1.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '1.5.3'
+VERSION = '1.5.4'
 DESCRIPTION = 'A package to convert between markup documents and a forest data structure for efficient processing.'
 
 setup(
     name = "pydelorean",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
```

