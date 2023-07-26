# Comparing `tmp/xmltread-0.1.tar.gz` & `tmp/xmltread-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmltread-0.1.tar", last modified: Tue Jul 25 22:33:47 2023, max compression
+gzip compressed data, was "xmltread-0.2.tar", last modified: Wed Jul 26 03:19:52 2023, max compression
```

## Comparing `xmltread-0.1.tar` & `xmltread-0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-25 22:33:47.265185 xmltread-0.1/
--rw-rw-r--   0 pj        (1000) pj        (1000)    35149 2023-07-25 04:53:13.000000 xmltread-0.1/LICENSE
--rw-rw-r--   0 pj        (1000) pj        (1000)    44046 2023-07-25 22:33:47.265185 xmltread-0.1/PKG-INFO
--rw-rw-r--   0 pj        (1000) pj        (1000)     2571 2023-07-25 22:31:44.000000 xmltread-0.1/README.md
--rw-rw-r--   0 pj        (1000) pj        (1000)     1038 2023-07-25 22:31:44.000000 xmltread-0.1/pyproject.toml
--rw-rw-r--   0 pj        (1000) pj        (1000)       38 2023-07-25 22:33:47.265185 xmltread-0.1/setup.cfg
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-25 22:33:47.261185 xmltread-0.1/tests/
--rw-rw-r--   0 pj        (1000) pj        (1000)     4822 2023-07-25 07:11:58.000000 xmltread-0.1/tests/test_orig.py
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-25 22:33:47.261185 xmltread-0.1/xmltread/
--rw-rw-r--   0 pj        (1000) pj        (1000)       24 2023-07-25 05:13:34.000000 xmltread-0.1/xmltread/__init__.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     1616 2023-07-25 07:12:02.000000 xmltread-0.1/xmltread/seeder.py
--rw-rw-r--   0 pj        (1000) pj        (1000)     7710 2023-07-25 07:22:19.000000 xmltread-0.1/xmltread/xmltramp.py
-drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-25 22:33:47.265185 xmltread-0.1/xmltread.egg-info/
--rw-rw-r--   0 pj        (1000) pj        (1000)    44046 2023-07-25 22:33:47.000000 xmltread-0.1/xmltread.egg-info/PKG-INFO
--rw-rw-r--   0 pj        (1000) pj        (1000)      271 2023-07-25 22:33:47.000000 xmltread-0.1/xmltread.egg-info/SOURCES.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)        1 2023-07-25 22:33:47.000000 xmltread-0.1/xmltread.egg-info/dependency_links.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)       44 2023-07-25 22:33:47.000000 xmltread-0.1/xmltread.egg-info/requires.txt
--rw-rw-r--   0 pj        (1000) pj        (1000)        9 2023-07-25 22:33:47.000000 xmltread-0.1/xmltread.egg-info/top_level.txt
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-26 03:19:52.824470 xmltread-0.2/
+-rw-rw-r--   0 pj        (1000) pj        (1000)    35149 2023-07-25 04:53:13.000000 xmltread-0.2/LICENSE
+-rw-rw-r--   0 pj        (1000) pj        (1000)    44046 2023-07-26 03:19:52.820470 xmltread-0.2/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)     2571 2023-07-25 22:31:44.000000 xmltread-0.2/README.md
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1038 2023-07-26 03:19:31.000000 xmltread-0.2/pyproject.toml
+-rw-rw-r--   0 pj        (1000) pj        (1000)       38 2023-07-26 03:19:52.824470 xmltread-0.2/setup.cfg
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-26 03:19:52.820470 xmltread-0.2/tests/
+-rw-rw-r--   0 pj        (1000) pj        (1000)     4822 2023-07-25 07:11:58.000000 xmltread-0.2/tests/test_orig.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-26 03:19:52.820470 xmltread-0.2/xmltread/
+-rw-rw-r--   0 pj        (1000) pj        (1000)       24 2023-07-25 05:13:34.000000 xmltread-0.2/xmltread/__init__.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     1616 2023-07-25 23:05:19.000000 xmltread-0.2/xmltread/seeder.py
+-rw-rw-r--   0 pj        (1000) pj        (1000)     7861 2023-07-26 03:19:31.000000 xmltread-0.2/xmltread/xmltramp.py
+drwxrwxr-x   0 pj        (1000) pj        (1000)        0 2023-07-26 03:19:52.820470 xmltread-0.2/xmltread.egg-info/
+-rw-rw-r--   0 pj        (1000) pj        (1000)    44046 2023-07-26 03:19:52.000000 xmltread-0.2/xmltread.egg-info/PKG-INFO
+-rw-rw-r--   0 pj        (1000) pj        (1000)      271 2023-07-26 03:19:52.000000 xmltread-0.2/xmltread.egg-info/SOURCES.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)        1 2023-07-26 03:19:52.000000 xmltread-0.2/xmltread.egg-info/dependency_links.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)       44 2023-07-26 03:19:52.000000 xmltread-0.2/xmltread.egg-info/requires.txt
+-rw-rw-r--   0 pj        (1000) pj        (1000)        9 2023-07-26 03:19:52.000000 xmltread-0.2/xmltread.egg-info/top_level.txt
```

### Comparing `xmltread-0.1/LICENSE` & `xmltread-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xmltread-0.1/PKG-INFO` & `xmltread-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmltread
-Version: 0.1
+Version: 0.2
 Summary: Make XML documents more easily accessible
 Author-email: Aaron Swartz <me@aaronsw.com>, Paul Jimenez <pj@place.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `xmltread-0.1/README.md` & `xmltread-0.2/README.md`

 * *Files identical despite different names*

### Comparing `xmltread-0.1/pyproject.toml` & `xmltread-0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xmltread"
-version = "0.1"
+version = "0.2"
 requires-python = ">=3.8"
 description = "Make XML documents more easily accessible"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
     {name = "Aaron Swartz", email = "me@aaronsw.com"},
     {name = "Paul Jimenez", email = "pj@place.org"}
```

### Comparing `xmltread-0.1/tests/test_orig.py` & `xmltread-0.2/tests/test_orig.py`

 * *Files identical despite different names*

### Comparing `xmltread-0.1/xmltread/seeder.py` & `xmltread-0.2/xmltread/seeder.py`

 * *Files identical despite different names*

### Comparing `xmltread-0.1/xmltread/xmltramp.py` & `xmltread-0.2/xmltread/xmltramp.py`

 * *Files 6% similar despite different names*

```diff
@@ -261,19 +261,28 @@
     def __getattr__(self, n):
         return (self.__uri, n)
 
     def __getitem__(self, n):
         return (self.__uri, n)
 
 
-def parse(text):
-    from io import StringIO
+def load_fileobj(fileobj):
     from .seeder import seed
 
-    return seed(StringIO(text))
+    return seed(fileobj)
 
 
-def load(url):
+def load_url(url):
     from urllib.request import urlopen
-    from .seeder import seed
 
-    return seed(urlopen(url))
+    return load_fileobj(urlopen(url))
+
+
+def load_file(filename: str):
+    with open(filename) as fileobj:
+        return load_fileobj(fileobj)
+
+
+def parse(text):
+    from io import StringIO
+
+    return load_fileobj(StringIO(text))
```

### Comparing `xmltread-0.1/xmltread.egg-info/PKG-INFO` & `xmltread-0.2/xmltread.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmltread
-Version: 0.1
+Version: 0.2
 Summary: Make XML documents more easily accessible
 Author-email: Aaron Swartz <me@aaronsw.com>, Paul Jimenez <pj@place.org>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

