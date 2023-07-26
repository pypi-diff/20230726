# Comparing `tmp/dictionary-search-1.0.0.tar.gz` & `tmp/dictionary-search-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictionary-search-1.0.0.tar", last modified: Tue Jul 19 10:20:43 2022, max compression
+gzip compressed data, was "dictionary-search-1.1.0.tar", last modified: Wed Jul 26 17:08:45 2023, max compression
```

## Comparing `dictionary-search-1.0.0.tar` & `dictionary-search-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 10:20:43.787902 dictionary-search-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-07-19 10:20:40.000000 dictionary-search-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-07-19 10:20:40.000000 dictionary-search-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-07-19 10:20:43.787902 dictionary-search-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1754 2022-07-19 10:20:40.000000 dictionary-search-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-19 10:20:40.000000 dictionary-search-1.0.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 10:20:43.783902 dictionary-search-1.0.0/dictionary_search/
--rw-r--r--   0 runner    (1001) docker     (121)     1467 2022-07-19 10:20:40.000000 dictionary-search-1.0.0/dictionary_search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-19 10:20:43.787902 dictionary-search-1.0.0/dictionary_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-07-19 10:20:43.000000 dictionary-search-1.0.0/dictionary_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-07-19 10:20:43.000000 dictionary-search-1.0.0/dictionary_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 10:20:43.000000 dictionary-search-1.0.0/dictionary_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-07-19 10:20:43.000000 dictionary-search-1.0.0/dictionary_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-19 10:20:43.000000 dictionary-search-1.0.0/dictionary_search.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-07-19 10:20:43.787902 dictionary-search-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-19 10:20:40.000000 dictionary-search-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/dictionary_search/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/dictionary_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/dictionary_search/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/dictionary_search/structural.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/dictionary_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-07-26 17:08:45.000000 dictionary-search-1.1.0/dictionary_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-26 17:08:45.000000 dictionary-search-1.1.0/dictionary_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:08:45.000000 dictionary-search-1.1.0/dictionary_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-26 17:08:45.000000 dictionary-search-1.1.0/dictionary_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 17:08:45.000000 dictionary-search-1.1.0/dictionary_search.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:45.321568 dictionary-search-1.1.0/tests/structural/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/structural/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/structural/test_flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/structural/test_nest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/test_search_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-26 17:08:43.000000 dictionary-search-1.1.0/tests/test_search_one.py
```

### Comparing `dictionary-search-1.0.0/LICENSE` & `dictionary-search-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dictionary-search-1.0.0/PKG-INFO` & `dictionary-search-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: dictionary-search
-Version: 1.0.0
+Version: 1.1.0
 Summary: Small dictionary search utils
 Home-page: https://github.com/cr0hn/python-dictionary-search
 Author: Daniel Garcia / Cesar Gallego
 Maintainer: Daniel Garcia (cr0hn)
 Maintainer-email: cr0hn@cr0hn.com
 License: License :: OSI Approved :: MIT License
 Description: # Dictionary Search tools
         
         ![License](https://img.shields.io/badge/License-Apache2-SUCCESS)
         ![Pypi](https://img.shields.io/pypi/v/dictionary-search)
         ![Python Versions](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10-blue)
         
         In a nutshell ``Dictionary Search`` is a small library to search in a dictionaries recursively.
+        Also have some other dictionary tools to make your life easier.
         
         # Install
         
         ```bash
         > pip install dictionary-search
         ```
         
-        # Usage example
+        # Search
         
         ```python
         # File: example.py
         
         from dictionary_search import search_first, search_all
         
         d = {
@@ -51,23 +52,36 @@
         print("Search First (path as tuple): ", search_first(d, "c", path_as_string=False))
         print("Search All (path as tuple): ", search_all(d, "c", path_as_string=False))
         
         ```
         
         After running the code, you will see:
         
-        ``````bash
+        ```bash
         > python examples/example.py
         Search First:  ('a.b.c', 'C value 1')
         Search All:  [('a.b.c', 'C value 1'), ('h.c', 'C value 2')]
         
         Search First (path as tuple):  (('a', 'b', 'c'), 'C value 1')
         Search All (path as tuple):  [(('a', 'b', 'c'), 'C value 1'), (('h', 'c'), 'C value 2')]
         ```
         
+        # Flat and Nest
+        
+        Allow you to flat and rebuild a dict. Nest only work with str and index keys.
+        
+        ```python
+        data = {"a": {"b": 1, "c": 2}}
+        flat_data = flat(data) # will produce: [("a.b", 1), ("a.c", 2)]
+        assert data == nest(flat_data)
+        ```
+        
+        > TODO: describe list
+        
+        If you want more information, please take a look to our test
         
         
         # Authors
         
         - [Cesar Gallego](https://github.com/CesarGallego)
         - [cr0hn](https://github.com/cr0hn)
         
@@ -83,14 +97,15 @@
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: System Administrators
```

### Comparing `dictionary-search-1.0.0/README.md` & `dictionary-search-1.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Dictionary Search tools
 
 ![License](https://img.shields.io/badge/License-Apache2-SUCCESS)
 ![Pypi](https://img.shields.io/pypi/v/dictionary-search)
 ![Python Versions](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10-blue)
 
 In a nutshell ``Dictionary Search`` is a small library to search in a dictionaries recursively.
+Also have some other dictionary tools to make your life easier.
 
 # Install
 
 ```bash
 > pip install dictionary-search
 ```
 
-# Usage example
+# Search
 
 ```python
 # File: example.py
 
 from dictionary_search import search_first, search_all
 
 d = {
@@ -42,23 +43,36 @@
 print("Search First (path as tuple): ", search_first(d, "c", path_as_string=False))
 print("Search All (path as tuple): ", search_all(d, "c", path_as_string=False))
 
 ```
 
 After running the code, you will see:
 
-``````bash
+```bash
 > python examples/example.py
 Search First:  ('a.b.c', 'C value 1')
 Search All:  [('a.b.c', 'C value 1'), ('h.c', 'C value 2')]
 
 Search First (path as tuple):  (('a', 'b', 'c'), 'C value 1')
 Search All (path as tuple):  [(('a', 'b', 'c'), 'C value 1'), (('h', 'c'), 'C value 2')]
 ```
 
+# Flat and Nest
+
+Allow you to flat and rebuild a dict. Nest only work with str and index keys.
+
+```python
+data = {"a": {"b": 1, "c": 2}}
+flat_data = flat(data) # will produce: [("a.b", 1), ("a.c", 2)]
+assert data == nest(flat_data)
+```
+
+> TODO: describe list
+
+If you want more information, please take a look to our test
 
 
 # Authors
 
 - [Cesar Gallego](https://github.com/CesarGallego)
 - [cr0hn](https://github.com/cr0hn)
```

### Comparing `dictionary-search-1.0.0/dictionary_search/__init__.py` & `dictionary-search-1.1.0/dictionary_search/search.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,16 @@
         if target in current:
             yield (*path, target), current[target]
 
         for x, y in current.items():
             for res in _search(y, target, (*path, x)):
                 yield res
     elif isinstance(current, list):
-        for item in current:
-            for res in _search(item, target, path):
+        for i, item in enumerate(current):
+            for res in _search(item, target, (*path, f"[{i}]")):
                 yield res
 
 
 def search_first(tree: dict,
                  target: str,
                  ancestors: Set[str] = None,
                  path_as_string: bool = True) -> Tuple[str, str]:
@@ -47,8 +47,8 @@
             else:
                 _path = path
 
             res.append((_path, element))
 
     return res
 
-__all__ = ("search_first", "search_all")
+__all__ = ["search_first", "search_all"]
```

### Comparing `dictionary-search-1.0.0/dictionary_search.egg-info/PKG-INFO` & `dictionary-search-1.1.0/dictionary_search.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: dictionary-search
-Version: 1.0.0
+Version: 1.1.0
 Summary: Small dictionary search utils
 Home-page: https://github.com/cr0hn/python-dictionary-search
 Author: Daniel Garcia / Cesar Gallego
 Maintainer: Daniel Garcia (cr0hn)
 Maintainer-email: cr0hn@cr0hn.com
 License: License :: OSI Approved :: MIT License
 Description: # Dictionary Search tools
         
         ![License](https://img.shields.io/badge/License-Apache2-SUCCESS)
         ![Pypi](https://img.shields.io/pypi/v/dictionary-search)
         ![Python Versions](https://img.shields.io/badge/Python-3.8%20%7C%203.9%20%7C%203.10-blue)
         
         In a nutshell ``Dictionary Search`` is a small library to search in a dictionaries recursively.
+        Also have some other dictionary tools to make your life easier.
         
         # Install
         
         ```bash
         > pip install dictionary-search
         ```
         
-        # Usage example
+        # Search
         
         ```python
         # File: example.py
         
         from dictionary_search import search_first, search_all
         
         d = {
@@ -51,23 +52,36 @@
         print("Search First (path as tuple): ", search_first(d, "c", path_as_string=False))
         print("Search All (path as tuple): ", search_all(d, "c", path_as_string=False))
         
         ```
         
         After running the code, you will see:
         
-        ``````bash
+        ```bash
         > python examples/example.py
         Search First:  ('a.b.c', 'C value 1')
         Search All:  [('a.b.c', 'C value 1'), ('h.c', 'C value 2')]
         
         Search First (path as tuple):  (('a', 'b', 'c'), 'C value 1')
         Search All (path as tuple):  [(('a', 'b', 'c'), 'C value 1'), (('h', 'c'), 'C value 2')]
         ```
         
+        # Flat and Nest
+        
+        Allow you to flat and rebuild a dict. Nest only work with str and index keys.
+        
+        ```python
+        data = {"a": {"b": 1, "c": 2}}
+        flat_data = flat(data) # will produce: [("a.b", 1), ("a.c", 2)]
+        assert data == nest(flat_data)
+        ```
+        
+        > TODO: describe list
+        
+        If you want more information, please take a look to our test
         
         
         # Authors
         
         - [Cesar Gallego](https://github.com/CesarGallego)
         - [cr0hn](https://github.com/cr0hn)
         
@@ -83,14 +97,15 @@
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: System Administrators
```

### Comparing `dictionary-search-1.0.0/setup.cfg` & `dictionary-search-1.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 license = License :: OSI Approved :: MIT License
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Environment :: Console
 	Operating System :: POSIX
 	Operating System :: MacOS
 	Operating System :: OS Independent
 	Operating System :: Microsoft :: Windows
 	Intended Audience :: Other Audience
 	Intended Audience :: System Administrators
```

