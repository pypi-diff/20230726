# Comparing `tmp/pyalltools-1.1.1.tar.gz` & `tmp/pyalltools-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalltools-1.1.1.tar", last modified: Wed Jul 26 11:57:34 2023, max compression
+gzip compressed data, was "pyalltools-2.0.0.tar", last modified: Wed Jul 26 12:08:10 2023, max compression
```

## Comparing `pyalltools-1.1.1.tar` & `pyalltools-2.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 11:57:34.285893 pyalltools-1.1.1/
--rw-rw-rw-   0        0        0      751 2023-07-26 11:57:34.283895 pyalltools-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      127 2023-05-20 09:31:02.000000 pyalltools-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 11:57:34.276501 pyalltools-1.1.1/pyalltools.egg-info/
--rw-rw-rw-   0        0        0      751 2023-07-26 11:57:33.000000 pyalltools-1.1.1/pyalltools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-07-26 11:57:33.000000 pyalltools-1.1.1/pyalltools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 11:57:33.000000 pyalltools-1.1.1/pyalltools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-26 11:57:33.000000 pyalltools-1.1.1/pyalltools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8559 2023-07-26 11:45:26.000000 pyalltools-1.1.1/pyalltools.py
--rw-rw-rw-   0        0        0       42 2023-07-26 11:57:34.286882 pyalltools-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      909 2023-07-26 11:57:20.000000 pyalltools-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 12:08:10.837312 pyalltools-2.0.0/
+-rw-rw-rw-   0        0        0      751 2023-07-26 12:08:10.835277 pyalltools-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      127 2023-05-20 09:31:02.000000 pyalltools-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 12:08:10.833279 pyalltools-2.0.0/pyalltools.egg-info/
+-rw-rw-rw-   0        0        0      751 2023-07-26 12:08:10.000000 pyalltools-2.0.0/pyalltools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-07-26 12:08:10.000000 pyalltools-2.0.0/pyalltools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 12:08:10.000000 pyalltools-2.0.0/pyalltools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-26 12:08:10.000000 pyalltools-2.0.0/pyalltools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8559 2023-07-26 12:07:14.000000 pyalltools-2.0.0/pyalltools.py
+-rw-rw-rw-   0        0        0       42 2023-07-26 12:08:10.838269 pyalltools-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      909 2023-07-26 12:07:35.000000 pyalltools-2.0.0/setup.py
```

### Comparing `pyalltools-1.1.1/PKG-INFO` & `pyalltools-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalltools
-Version: 1.1.1
+Version: 2.0.0
 Summary: Library containing various tools that are required by programmers frequently
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `pyalltools-1.1.1/pyalltools.egg-info/PKG-INFO` & `pyalltools-2.0.0/pyalltools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyalltools
-Version: 1.1.1
+Version: 2.0.0
 Summary: Library containing various tools that are required by programmers frequently
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `pyalltools-1.1.1/pyalltools.py` & `pyalltools-2.0.0/pyalltools.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                             "git clone https://github.com/commixproject/commix.git"
                 ]
 
                 import os
                 for module in modules:
                     os.system(module)
 
-class int:
+class Int:
         @staticmethod
         def chkprime(number):
             if number > 1:
                 for i in range(2, number):
                     if (number % i) == 0:
                         return "Not Prime"
                 else:
@@ -99,15 +99,15 @@
             temp = number
             while number != 0:
                 digit = number % 10
                 sum = sum + digit
                 number //= 10
             return sum
 
-class str:
+class Str:
         @staticmethod
         def palindrome(string):
             rev = ""
             for i in string:
                 rev = i + rev
             if rev == string:
                 return "Palindrome"
@@ -155,15 +155,15 @@
             for i in range(l):
                 ln = len(a[i])
                 if ln > m:
                     m = ln
                     mx = a[i]
             return mx
 
-class list:
+class List:
     @staticmethod
     def frequency(list):
         freq = 0
         lst = [ ]
         result = {}
         for i in list:
             while i not in lst:
@@ -197,15 +197,15 @@
         lst = [ ]
 
         for i in list:
             while i not in lst:
                 lst.append(i)
         return lst
 
-class tuple:
+class Tuple:
     @staticmethod
     def frequency(tuple):
         freq = 0
         tup = ()
         result = {}
         for i in tuple:
             while i not in tup:
```

### Comparing `pyalltools-1.1.1/setup.py` & `pyalltools-2.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyalltools",
-    version="1.1.1",
+    version="2.0.0",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Library containing various tools that are required by programmers frequently",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://techinfoak.wixsite.com/tech-info",
     project_urls={
```

