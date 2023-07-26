# Comparing `tmp/hashwise-0.0.1.tar.gz` & `tmp/hashwise-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashwise-0.0.1.tar", last modified: Thu Jul 13 03:05:34 2023, max compression
+gzip compressed data, was "hashwise-0.0.2.tar", last modified: Wed Jul 26 15:10:00 2023, max compression
```

## Comparing `hashwise-0.0.1.tar` & `hashwise-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 03:05:34.215000 hashwise-0.0.1/
--rw-rw-rw-   0        0        0      250 2023-07-13 03:05:34.208000 hashwise-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-13 01:33:12.000000 hashwise-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 03:05:34.157000 hashwise-0.0.1/hashwise/
--rw-rw-rw-   0        0        0       23 2023-07-13 01:35:56.000000 hashwise-0.0.1/hashwise/__init__.py
--rw-rw-rw-   0        0        0      107 2023-07-13 01:36:12.000000 hashwise-0.0.1/hashwise/device_status.py
--rw-rw-rw-   0        0        0     6204 2023-07-13 03:03:54.000000 hashwise-0.0.1/hashwise/hashwise.py
-drwxrwxrwx   0        0        0        0 2023-07-13 03:05:34.198000 hashwise-0.0.1/hashwise.egg-info/
--rw-rw-rw-   0        0        0      250 2023-07-13 03:05:33.000000 hashwise-0.0.1/hashwise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      214 2023-07-13 03:05:34.000000 hashwise-0.0.1/hashwise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 03:05:33.000000 hashwise-0.0.1/hashwise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 03:05:33.000000 hashwise-0.0.1/hashwise.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 03:05:34.213000 hashwise-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-07-13 02:16:53.000000 hashwise-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:10:00.008000 hashwise-0.0.2/
+-rw-rw-rw-   0        0        0     3933 2023-07-26 15:09:59.998000 hashwise-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3713 2023-07-26 15:08:40.000000 hashwise-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:59.755000 hashwise-0.0.2/hashwise/
+-rw-rw-rw-   0        0        0       23 2023-07-13 01:35:56.000000 hashwise-0.0.2/hashwise/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:59.835000 hashwise-0.0.2/hashwise/cuda-libraries/
+-rw-rw-rw-   0        0        0   667648 2023-07-18 15:25:23.000000 hashwise-0.0.2/hashwise/cuda-libraries/cudalib-windows-64bit.dll
+-rw-rw-rw-   0        0        0     2648 2023-07-16 01:17:49.000000 hashwise-0.0.2/hashwise/device_status.py
+-rw-rw-rw-   0        0        0      413 2023-07-17 02:24:41.000000 hashwise-0.0.2/hashwise/exceptions.py
+-rw-rw-rw-   0        0        0    21644 2023-07-26 14:52:52.000000 hashwise-0.0.2/hashwise/hashwise.py
+drwxrwxrwx   0        0        0        0 2023-07-26 15:09:59.813000 hashwise-0.0.2/hashwise.egg-info/
+-rw-rw-rw-   0        0        0     3933 2023-07-26 15:09:59.000000 hashwise-0.0.2/hashwise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-07-26 15:09:59.000000 hashwise-0.0.2/hashwise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 15:09:59.000000 hashwise-0.0.2/hashwise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 15:09:59.000000 hashwise-0.0.2/hashwise.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 15:10:00.005000 hashwise-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      708 2023-07-26 15:07:42.000000 hashwise-0.0.2/setup.py
```

### Comparing `hashwise-0.0.1/setup.py` & `hashwise-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='hashwise',
-    version='0.0.1',
-    description='A secure python library for parallelizing hashing algorithms across a graphics card.',
+    version='0.0.2',
+    description='A secure python library for GPU accelerated hashing.',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     author='Anish Kanthamneni',
     packages=find_packages(),
     package_data={
         '': ['*.dll'],
         'hashwise': ['c-libraries/*.dll', 'cuda-libraries/*.dll'],
```

