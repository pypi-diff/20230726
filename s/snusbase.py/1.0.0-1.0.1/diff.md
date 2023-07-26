# Comparing `tmp/snusbase.py-1.0.0.tar.gz` & `tmp/snusbase.py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snusbase.py-1.0.0.tar", last modified: Wed Jul 26 06:52:49 2023, max compression
+gzip compressed data, was "snusbase.py-1.0.1.tar", last modified: Wed Jul 26 06:54:26 2023, max compression
```

## Comparing `snusbase.py-1.0.0.tar` & `snusbase.py-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-26 06:52:49.151920 snusbase.py-1.0.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1072 2023-07-26 06:27:18.000000 snusbase.py-1.0.0/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       59 2023-07-26 06:19:01.000000 snusbase.py-1.0.0/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2013 2023-07-26 06:52:49.147920 snusbase.py-1.0.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1106 2023-07-26 06:52:18.000000 snusbase.py-1.0.0/README.rst
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-07-26 06:37:49.000000 snusbase.py-1.0.0/requirements.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-26 06:52:49.151920 snusbase.py-1.0.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1628 2023-07-26 06:50:32.000000 snusbase.py-1.0.0/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-26 06:52:49.147920 snusbase.py-1.0.0/snusbase/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      214 2023-07-26 06:26:35.000000 snusbase.py-1.0.0/snusbase/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6522 2023-07-26 06:44:44.000000 snusbase.py-1.0.0/snusbase/client.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      195 2023-07-26 06:43:50.000000 snusbase.py-1.0.0/snusbase/errors.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-26 06:52:49.147920 snusbase.py-1.0.0/snusbase.py.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2013 2023-07-26 06:52:49.000000 snusbase.py-1.0.0/snusbase.py.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      289 2023-07-26 06:52:49.000000 snusbase.py-1.0.0/snusbase.py.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-26 06:52:49.000000 snusbase.py-1.0.0/snusbase.py.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-07-26 06:52:49.000000 snusbase.py-1.0.0/snusbase.py.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-26 06:52:49.000000 snusbase.py-1.0.0/snusbase.py.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-26 06:54:26.491921 snusbase.py-1.0.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1072 2023-07-26 06:27:18.000000 snusbase.py-1.0.1/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       59 2023-07-26 06:19:01.000000 snusbase.py-1.0.1/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2010 2023-07-26 06:54:26.491921 snusbase.py-1.0.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1103 2023-07-26 06:54:01.000000 snusbase.py-1.0.1/README.rst
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       53 2023-07-26 06:37:49.000000 snusbase.py-1.0.1/requirements.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-07-26 06:54:26.491921 snusbase.py-1.0.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1628 2023-07-26 06:50:32.000000 snusbase.py-1.0.1/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-26 06:54:26.487921 snusbase.py-1.0.1/snusbase/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      214 2023-07-26 06:54:18.000000 snusbase.py-1.0.1/snusbase/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6522 2023-07-26 06:44:44.000000 snusbase.py-1.0.1/snusbase/client.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      195 2023-07-26 06:43:50.000000 snusbase.py-1.0.1/snusbase/errors.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-07-26 06:54:26.491921 snusbase.py-1.0.1/snusbase.py.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2010 2023-07-26 06:54:26.000000 snusbase.py-1.0.1/snusbase.py.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      289 2023-07-26 06:54:26.000000 snusbase.py-1.0.1/snusbase.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-07-26 06:54:26.000000 snusbase.py-1.0.1/snusbase.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-07-26 06:54:26.000000 snusbase.py-1.0.1/snusbase.py.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-07-26 06:54:26.000000 snusbase.py-1.0.1/snusbase.py.egg-info/top_level.txt
```

### Comparing `snusbase.py-1.0.0/LICENSE` & `snusbase.py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snusbase.py-1.0.0/PKG-INFO` & `snusbase.py-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snusbase.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: an un-official async wrapper for the Snusbase API
 Author: igna
 License: MIT
 Project-URL: Website, https://snusbase.com
 Project-URL: Issue tracker, https://github.com/obstructive/snusbase.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -58,18 +58,18 @@
    speedup)
 
 Quick Example
 =============
 
 .. code:: py
 
-   from snusbase.py import SnusbaseApi
+   from snusbase import SnusbaseAPI
    from asyncio import get_event_loop
 
-   client = SnusbaseApi("token")
+   client = SnusbaseAPI("token")
 
 
    async def main():
        result = await client.search_by_username("example")
        print(result)
```

### Comparing `snusbase.py-1.0.0/README.rst` & `snusbase.py-1.0.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -34,18 +34,18 @@
    speedup)
 
 Quick Example
 =============
 
 .. code:: py
 
-   from snusbase.py import SnusbaseApi
+   from snusbase import SnusbaseAPI
    from asyncio import get_event_loop
 
-   client = SnusbaseApi("token")
+   client = SnusbaseAPI("token")
 
 
    async def main():
        result = await client.search_by_username("example")
        print(result)
```

### Comparing `snusbase.py-1.0.0/setup.py` & `snusbase.py-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `snusbase.py-1.0.0/snusbase/client.py` & `snusbase.py-1.0.1/snusbase/client.py`

 * *Files identical despite different names*

### Comparing `snusbase.py-1.0.0/snusbase.py.egg-info/PKG-INFO` & `snusbase.py-1.0.1/snusbase.py.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snusbase.py
-Version: 1.0.0
+Version: 1.0.1
 Summary: an un-official async wrapper for the Snusbase API
 Author: igna
 License: MIT
 Project-URL: Website, https://snusbase.com
 Project-URL: Issue tracker, https://github.com/obstructive/snusbase.py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -58,18 +58,18 @@
    speedup)
 
 Quick Example
 =============
 
 .. code:: py
 
-   from snusbase.py import SnusbaseApi
+   from snusbase import SnusbaseAPI
    from asyncio import get_event_loop
 
-   client = SnusbaseApi("token")
+   client = SnusbaseAPI("token")
 
 
    async def main():
        result = await client.search_by_username("example")
        print(result)
```

