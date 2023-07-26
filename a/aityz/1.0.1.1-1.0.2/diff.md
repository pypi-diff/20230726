# Comparing `tmp/aityz-1.0.1.1.tar.gz` & `tmp/aityz-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aityz-1.0.1.1.tar", last modified: Wed Jul 26 11:05:30 2023, max compression
+gzip compressed data, was "aityz-1.0.2.tar", last modified: Wed Jul 26 11:08:44 2023, max compression
```

## Comparing `aityz-1.0.1.1.tar` & `aityz-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:05:30.025861 aityz-1.0.1.1/
--rw-rw-rw-   0        0        0    35821 2023-07-26 03:38:00.000000 aityz-1.0.1.1/LICENSE
--rw-rw-rw-   0        0        0      449 2023-07-26 11:05:30.023856 aityz-1.0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-07-26 11:03:01.000000 aityz-1.0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 11:05:29.981777 aityz-1.0.1.1/aityz/
--rw-rw-rw-   0        0        0       10 2023-07-26 11:05:19.000000 aityz-1.0.1.1/aityz/__init__.py
--rw-rw-rw-   0        0        0     4066 2023-07-26 11:05:19.000000 aityz-1.0.1.1/aityz/encryption.py
--rw-rw-rw-   0        0        0      440 2023-07-26 11:05:19.000000 aityz-1.0.1.1/aityz/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-26 11:05:30.017768 aityz-1.0.1.1/aityz.egg-info/
--rw-rw-rw-   0        0        0      449 2023-07-26 11:05:29.000000 aityz-1.0.1.1/aityz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-26 11:05:29.000000 aityz-1.0.1.1/aityz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:05:29.000000 aityz-1.0.1.1/aityz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-26 11:05:29.000000 aityz-1.0.1.1/aityz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-26 11:05:29.000000 aityz-1.0.1.1/aityz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      625 2023-07-26 03:53:16.000000 aityz-1.0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 11:05:30.025861 aityz-1.0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-07-26 11:05:28.000000 aityz-1.0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:08:44.607725 aityz-1.0.2/
+-rw-rw-rw-   0        0        0    35821 2023-07-26 03:38:00.000000 aityz-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      447 2023-07-26 11:08:44.605421 aityz-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-07-26 11:03:01.000000 aityz-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 11:08:44.578122 aityz-1.0.2/aityz/
+-rw-rw-rw-   0        0        0        0 2023-07-26 11:07:26.000000 aityz-1.0.2/aityz/__init__.py
+-rw-rw-rw-   0        0        0     4078 2023-07-26 11:07:49.000000 aityz-1.0.2/aityz/encryption.py
+-rw-rw-rw-   0        0        0      440 2023-07-26 11:05:19.000000 aityz-1.0.2/aityz/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-26 11:08:44.600516 aityz-1.0.2/aityz.egg-info/
+-rw-rw-rw-   0        0        0      447 2023-07-26 11:08:44.000000 aityz-1.0.2/aityz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-26 11:08:44.000000 aityz-1.0.2/aityz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 11:08:44.000000 aityz-1.0.2/aityz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-26 11:08:44.000000 aityz-1.0.2/aityz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 11:08:44.000000 aityz-1.0.2/aityz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      625 2023-07-26 03:53:16.000000 aityz-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 11:08:44.607725 aityz-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      579 2023-07-26 11:08:20.000000 aityz-1.0.2/setup.py
```

### Comparing `aityz-1.0.1.1/LICENSE` & `aityz-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aityz-1.0.1.1/aityz/encryption.py` & `aityz-1.0.2/aityz/encryption.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from aityz import exceptions
+import rsa
 
 def pad(pad, length=16):
     """
     Pad a given string `pad` with spaces to a specified `length`.
 
     :param pad: The string to be padded.
     :param length: The desired length of the padded string. Default is 16.
```

### Comparing `aityz-1.0.1.1/pyproject.toml` & `aityz-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aityz-1.0.1.1/setup.py` & `aityz-1.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aityz',
-    version='1.0.1.1',
+    version='1.0.2',
     packages=find_packages(),
     install_requires=[
         'rsa'
     ],
     author='Aityz',
     author_email='itzaityz@gmail.com',
     description='The multipurpose package, built for programmers',
```

