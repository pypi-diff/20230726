# Comparing `tmp/efpy-0.1.2.tar.gz` & `tmp/efpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efpy-0.1.2.tar", last modified: Fri Apr 28 23:41:39 2023, max compression
+gzip compressed data, was "efpy-0.1.3.tar", last modified: Wed Jul 26 14:01:03 2023, max compression
```

## Comparing `efpy-0.1.2.tar` & `efpy-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 23:41:39.549472 efpy-0.1.2/
--rw-rw-rw-   0        0        0      255 2023-04-28 23:41:39.548473 efpy-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-28 23:41:39.538386 efpy-0.1.2/efpy/
--rw-rw-rw-   0        0        0      836 2023-04-28 23:40:39.000000 efpy-0.1.2/efpy/__init__.py
--rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.2/efpy/env.py
-drwxrwxrwx   0        0        0        0 2023-04-28 23:41:39.547446 efpy-0.1.2/efpy.egg-info/
--rw-rw-rw-   0        0        0      255 2023-04-28 23:41:39.000000 efpy-0.1.2/efpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      149 2023-04-28 23:41:39.000000 efpy-0.1.2/efpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 23:41:39.000000 efpy-0.1.2/efpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-28 23:41:39.000000 efpy-0.1.2/efpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 23:41:39.549472 efpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      741 2023-04-28 23:41:30.000000 efpy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:01:03.425197 efpy-0.1.3/
+-rw-rw-rw-   0        0        0      255 2023-07-26 14:01:03.425197 efpy-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 14:01:03.425197 efpy-0.1.3/efpy/
+-rw-rw-rw-   0        0        0     1082 2023-07-26 14:00:22.000000 efpy-0.1.3/efpy/__init__.py
+-rw-rw-rw-   0        0        0     1447 2021-06-24 08:59:48.000000 efpy-0.1.3/efpy/env.py
+-rw-rw-rw-   0        0        0     2723 2023-07-26 13:58:57.000000 efpy-0.1.3/efpy/expHelper.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:01:03.425197 efpy-0.1.3/efpy.egg-info/
+-rw-rw-rw-   0        0        0      255 2023-07-26 14:01:03.000000 efpy-0.1.3/efpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-26 14:01:03.000000 efpy-0.1.3/efpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 14:01:03.000000 efpy-0.1.3/efpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 14:01:03.000000 efpy-0.1.3/efpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-26 14:01:03.000000 efpy-0.1.3/efpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 14:01:03.425197 efpy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      752 2023-07-26 13:58:19.000000 efpy-0.1.3/setup.py
```

### Comparing `efpy-0.1.2/efpy/env.py` & `efpy-0.1.3/efpy/env.py`

 * *Files identical despite different names*

### Comparing `efpy-0.1.2/setup.py` & `efpy-0.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 #############################################
 
 
 from setuptools import setup, find_packages
 
 setup(
     name = "efpy",
-    version = "0.1.2",
+    version = "0.1.3",
     keywords = ("experience","environment"),
     description = "experience",
     long_description = "experience",
     license = "MIT Licence",
 
     url = "https://github.com/imcjp/efpy",
     author = "Cai Jianping",
     author_email = "jpingcai@163.com",
 
     packages = find_packages(),
     include_package_data = True,
     platforms = "any",
-    install_requires = []
+    install_requires = ['yaml','re']
 )
```

