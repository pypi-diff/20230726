# Comparing `tmp/kobo-md-0.1.tar.gz` & `tmp/kobo-md-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kobo-md-0.1.tar", last modified: Wed Jul 26 20:58:58 2023, max compression
+gzip compressed data, was "kobo-md-0.1.1.tar", last modified: Wed Jul 26 21:04:47 2023, max compression
```

## Comparing `kobo-md-0.1.tar` & `kobo-md-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 20:58:58.571653 kobo-md-0.1/
--rw-r--r--   0 dwall      (501) staff       (20)     1086 2023-07-26 20:39:20.000000 kobo-md-0.1/LICENSE.txt
--rw-r--r--   0 dwall      (501) staff       (20)       46 2023-07-26 08:15:21.000000 kobo-md-0.1/MANIFEST.in
--rw-r--r--   0 dwall      (501) staff       (20)      156 2023-07-26 20:58:58.571695 kobo-md-0.1/PKG-INFO
--rw-r--r--   0 dwall      (501) staff       (20)      608 2023-07-26 20:24:39.000000 kobo-md-0.1/README.md
--rw-r--r--   0 dwall      (501) staff       (20)      106 2023-07-26 20:58:58.571882 kobo-md-0.1/setup.cfg
--rw-r--r--   0 dwall      (501) staff       (20)      917 2023-07-26 20:58:42.000000 kobo-md-0.1/setup.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 20:58:58.567375 kobo-md-0.1/src/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 20:58:58.569676 kobo-md-0.1/src/kobo/
--rw-r--r--   0 dwall      (501) staff       (20)       42 2023-07-26 20:33:16.000000 kobo-md-0.1/src/kobo/__init__.py
--rw-r--r--   0 dwall      (501) staff       (20)     1770 2023-07-26 08:44:52.000000 kobo-md-0.1/src/kobo/__main__.py
--rw-r--r--   0 dwall      (501) staff       (20)      791 2023-07-26 08:48:12.000000 kobo-md-0.1/src/kobo/helper.py
--rw-r--r--   0 dwall      (501) staff       (20)     6274 2023-07-26 20:33:36.000000 kobo-md-0.1/src/kobo/parser.py
--rw-r--r--   0 dwall      (501) staff       (20)      344 2023-07-26 07:12:37.000000 kobo-md-0.1/src/kobo/redirects.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 20:58:58.567304 kobo-md-0.1/src/kobo/resources/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 20:58:58.569867 kobo-md-0.1/src/kobo/resources/content/
--rw-r--r--   0 dwall      (501) staff       (20)       94 2023-07-26 08:39:44.000000 kobo-md-0.1/src/kobo/resources/content/index.md
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 20:58:58.567229 kobo-md-0.1/src/kobo/resources/static/
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 20:58:58.570253 kobo-md-0.1/src/kobo/resources/static/css/
--rw-r--r--   0 dwall      (501) staff       (20)     2527 2023-07-26 07:01:14.000000 kobo-md-0.1/src/kobo/resources/static/css/grid.css
--rw-r--r--   0 dwall      (501) staff       (20)      608 2023-07-26 07:01:14.000000 kobo-md-0.1/src/kobo/resources/static/css/main.css
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 20:58:58.571064 kobo-md-0.1/src/kobo/resources/templates/
--rw-r--r--   0 dwall      (501) staff       (20)      296 2023-07-26 07:01:18.000000 kobo-md-0.1/src/kobo/resources/templates/404.html
--rw-r--r--   0 dwall      (501) staff       (20)      383 2023-07-26 07:01:18.000000 kobo-md-0.1/src/kobo/resources/templates/index-list.html
--rw-r--r--   0 dwall      (501) staff       (20)      381 2023-07-26 07:01:18.000000 kobo-md-0.1/src/kobo/resources/templates/index.html
--rw-r--r--   0 dwall      (501) staff       (20)      375 2023-07-26 07:01:18.000000 kobo-md-0.1/src/kobo/resources/templates/page.html
--rw-r--r--   0 dwall      (501) staff       (20)     2534 2023-07-26 07:39:13.000000 kobo-md-0.1/src/kobo/server.py
-drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 20:58:58.571568 kobo-md-0.1/src/kobo_md.egg-info/
--rw-r--r--   0 dwall      (501) staff       (20)      156 2023-07-26 20:58:58.000000 kobo-md-0.1/src/kobo_md.egg-info/PKG-INFO
--rw-r--r--   0 dwall      (501) staff       (20)      589 2023-07-26 20:58:58.000000 kobo-md-0.1/src/kobo_md.egg-info/SOURCES.txt
--rw-r--r--   0 dwall      (501) staff       (20)        1 2023-07-26 20:58:58.000000 kobo-md-0.1/src/kobo_md.egg-info/dependency_links.txt
--rw-r--r--   0 dwall      (501) staff       (20)        5 2023-07-26 20:58:58.000000 kobo-md-0.1/src/kobo_md.egg-info/top_level.txt
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 21:04:47.726618 kobo-md-0.1.1/
+-rw-r--r--   0 dwall      (501) staff       (20)     1086 2023-07-26 20:39:20.000000 kobo-md-0.1.1/LICENSE.txt
+-rw-r--r--   0 dwall      (501) staff       (20)       46 2023-07-26 08:15:21.000000 kobo-md-0.1.1/MANIFEST.in
+-rw-r--r--   0 dwall      (501) staff       (20)      760 2023-07-26 21:04:47.726799 kobo-md-0.1.1/PKG-INFO
+-rw-r--r--   0 dwall      (501) staff       (20)      561 2023-07-26 21:02:59.000000 kobo-md-0.1.1/README.md
+-rw-r--r--   0 dwall      (501) staff       (20)      106 2023-07-26 21:04:47.727102 kobo-md-0.1.1/setup.cfg
+-rw-r--r--   0 dwall      (501) staff       (20)     1128 2023-07-26 21:04:39.000000 kobo-md-0.1.1/setup.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 21:04:47.721977 kobo-md-0.1.1/src/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 21:04:47.724279 kobo-md-0.1.1/src/kobo/
+-rw-r--r--   0 dwall      (501) staff       (20)       42 2023-07-26 20:33:16.000000 kobo-md-0.1.1/src/kobo/__init__.py
+-rw-r--r--   0 dwall      (501) staff       (20)     1770 2023-07-26 08:44:52.000000 kobo-md-0.1.1/src/kobo/__main__.py
+-rw-r--r--   0 dwall      (501) staff       (20)      791 2023-07-26 08:48:12.000000 kobo-md-0.1.1/src/kobo/helper.py
+-rw-r--r--   0 dwall      (501) staff       (20)     6274 2023-07-26 20:33:36.000000 kobo-md-0.1.1/src/kobo/parser.py
+-rw-r--r--   0 dwall      (501) staff       (20)      344 2023-07-26 07:12:37.000000 kobo-md-0.1.1/src/kobo/redirects.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 21:04:47.721919 kobo-md-0.1.1/src/kobo/resources/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 21:04:47.724512 kobo-md-0.1.1/src/kobo/resources/content/
+-rw-r--r--   0 dwall      (501) staff       (20)       94 2023-07-26 08:39:44.000000 kobo-md-0.1.1/src/kobo/resources/content/index.md
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 21:04:47.721861 kobo-md-0.1.1/src/kobo/resources/static/
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 21:04:47.724926 kobo-md-0.1.1/src/kobo/resources/static/css/
+-rw-r--r--   0 dwall      (501) staff       (20)     2527 2023-07-26 07:01:14.000000 kobo-md-0.1.1/src/kobo/resources/static/css/grid.css
+-rw-r--r--   0 dwall      (501) staff       (20)      608 2023-07-26 07:01:14.000000 kobo-md-0.1.1/src/kobo/resources/static/css/main.css
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 21:04:47.725692 kobo-md-0.1.1/src/kobo/resources/templates/
+-rw-r--r--   0 dwall      (501) staff       (20)      296 2023-07-26 07:01:18.000000 kobo-md-0.1.1/src/kobo/resources/templates/404.html
+-rw-r--r--   0 dwall      (501) staff       (20)      383 2023-07-26 07:01:18.000000 kobo-md-0.1.1/src/kobo/resources/templates/index-list.html
+-rw-r--r--   0 dwall      (501) staff       (20)      381 2023-07-26 07:01:18.000000 kobo-md-0.1.1/src/kobo/resources/templates/index.html
+-rw-r--r--   0 dwall      (501) staff       (20)      375 2023-07-26 07:01:18.000000 kobo-md-0.1.1/src/kobo/resources/templates/page.html
+-rw-r--r--   0 dwall      (501) staff       (20)     2534 2023-07-26 07:39:13.000000 kobo-md-0.1.1/src/kobo/server.py
+drwxr-xr-x   0 dwall      (501) staff       (20)        0 2023-07-26 21:04:47.726492 kobo-md-0.1.1/src/kobo_md.egg-info/
+-rw-r--r--   0 dwall      (501) staff       (20)      760 2023-07-26 21:04:47.000000 kobo-md-0.1.1/src/kobo_md.egg-info/PKG-INFO
+-rw-r--r--   0 dwall      (501) staff       (20)      589 2023-07-26 21:04:47.000000 kobo-md-0.1.1/src/kobo_md.egg-info/SOURCES.txt
+-rw-r--r--   0 dwall      (501) staff       (20)        1 2023-07-26 21:04:47.000000 kobo-md-0.1.1/src/kobo_md.egg-info/dependency_links.txt
+-rw-r--r--   0 dwall      (501) staff       (20)        5 2023-07-26 21:04:47.000000 kobo-md-0.1.1/src/kobo_md.egg-info/top_level.txt
```

### Comparing `kobo-md-0.1/LICENSE.txt` & `kobo-md-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1/setup.py` & `kobo-md-0.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #!/usr/bin/env python
 
+VERSION = '0.1.1'
+
 import setuptools
 import os
 import sys
+import pathlib
+
 
 def project_path(*sub_paths):
     project_dirpath = os.path.abspath(os.path.dirname(__file__))
     return os.path.join(project_dirpath, *sub_paths)
 
 
 def read(*sub_paths):
@@ -16,18 +20,23 @@
 package_dir = {'': 'src'}
 install_requires = [
     line.strip()
     for line in read('requirements.txt').splitlines()
     if line.strip() and not line.startswith("#")
 ]
 
+PACKAGE_DIR = pathlib.Path(__file__).parent
+README = (PACKAGE_DIR / 'README.md').read_text()
+
 setuptools.setup(
     name='kobo-md',
-    version='0.1',
+    version=VERSION,
     description='Markdown Compiler + Server',
+    long_description=README,
+    long_description_content_type='text/markdown',
     author='Dylan Wallace',
     packages=['kobo'],
     package_dir=package_dir,
     package_data={'kobo': [
         'resources/templates/*',
         'resources/static/css/*',
         'resources/static/js',
```

### Comparing `kobo-md-0.1/src/kobo/__main__.py` & `kobo-md-0.1.1/src/kobo/__main__.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1/src/kobo/helper.py` & `kobo-md-0.1.1/src/kobo/helper.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1/src/kobo/parser.py` & `kobo-md-0.1.1/src/kobo/parser.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1/src/kobo/resources/static/css/grid.css` & `kobo-md-0.1.1/src/kobo/resources/static/css/grid.css`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1/src/kobo/resources/static/css/main.css` & `kobo-md-0.1.1/src/kobo/resources/static/css/main.css`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1/src/kobo/server.py` & `kobo-md-0.1.1/src/kobo/server.py`

 * *Files identical despite different names*

### Comparing `kobo-md-0.1/src/kobo_md.egg-info/SOURCES.txt` & `kobo-md-0.1.1/src/kobo_md.egg-info/SOURCES.txt`

 * *Files identical despite different names*

