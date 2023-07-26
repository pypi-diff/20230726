# Comparing `tmp/auto-group-1.3.0.tar.gz` & `tmp/auto-group-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-group-1.3.0.tar", last modified: Wed Mar  8 19:14:43 2023, max compression
+gzip compressed data, was "auto-group-1.3.1.tar", last modified: Wed Jul 26 07:24:31 2023, max compression
```

## Comparing `auto-group-1.3.0.tar` & `auto-group-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-03-08 19:14:43.577138 auto-group-1.3.0/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1080 2021-01-07 18:29:55.000000 auto-group-1.3.0/LICENSE
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2023-01-12 18:27:18.000000 auto-group-1.3.0/MANIFEST.in
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     7118 2023-03-08 19:14:43.577138 auto-group-1.3.0/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     6653 2023-02-11 10:41:48.000000 auto-group-1.3.0/README.md
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-03-08 19:14:43.577138 auto-group-1.3.0/auto_group/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     9782 2023-03-08 14:46:51.000000 auto-group-1.3.0/auto_group/__init__.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     4316 2023-01-12 17:27:26.000000 auto-group-1.3.0/auto_group/advanced.py
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     2408 2023-02-11 10:45:54.000000 auto-group-1.3.0/auto_group/tools.py
-drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-03-08 19:14:43.577138 auto-group-1.3.0/auto_group.egg-info/
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     7118 2023-03-08 19:14:43.000000 auto-group-1.3.0/auto_group.egg-info/PKG-INFO
--rw-rw-r--   0 alda78    (1000) alda78    (1000)      273 2023-03-08 19:14:43.000000 auto-group-1.3.0/auto_group.egg-info/SOURCES.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-03-08 19:14:43.000000 auto-group-1.3.0/auto_group.egg-info/dependency_links.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-01-12 18:27:39.000000 auto-group-1.3.0/auto_group.egg-info/not-zip-safe
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       11 2023-03-08 19:14:43.000000 auto-group-1.3.0/auto_group.egg-info/top_level.txt
--rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-03-08 19:14:43.577138 auto-group-1.3.0/setup.cfg
--rw-rw-r--   0 alda78    (1000) alda78    (1000)     1378 2023-01-12 18:26:52.000000 auto-group-1.3.0/setup.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 07:24:31.809239 auto-group-1.3.1/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1080 2021-01-07 18:29:55.000000 auto-group-1.3.1/LICENSE
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        0 2023-01-12 18:27:18.000000 auto-group-1.3.1/MANIFEST.in
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     7194 2023-07-26 07:24:31.809239 auto-group-1.3.1/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     6729 2023-07-26 07:22:27.000000 auto-group-1.3.1/README.md
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 07:24:31.809239 auto-group-1.3.1/auto_group/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     9782 2023-03-08 14:46:51.000000 auto-group-1.3.1/auto_group/__init__.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     4316 2023-01-12 17:27:26.000000 auto-group-1.3.1/auto_group/advanced.py
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     2734 2023-07-26 07:14:56.000000 auto-group-1.3.1/auto_group/tools.py
+drwxrwxr-x   0 alda78    (1000) alda78    (1000)        0 2023-07-26 07:24:31.809239 auto-group-1.3.1/auto_group.egg-info/
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     7194 2023-07-26 07:24:31.000000 auto-group-1.3.1/auto_group.egg-info/PKG-INFO
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)      273 2023-07-26 07:24:31.000000 auto-group-1.3.1/auto_group.egg-info/SOURCES.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-07-26 07:24:31.000000 auto-group-1.3.1/auto_group.egg-info/dependency_links.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)        1 2023-07-26 07:24:31.000000 auto-group-1.3.1/auto_group.egg-info/not-zip-safe
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       11 2023-07-26 07:24:31.000000 auto-group-1.3.1/auto_group.egg-info/top_level.txt
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)       38 2023-07-26 07:24:31.809239 auto-group-1.3.1/setup.cfg
+-rw-rw-r--   0 alda78    (1000) alda78    (1000)     1378 2023-01-12 18:26:52.000000 auto-group-1.3.1/setup.py
```

### Comparing `auto-group-1.3.0/LICENSE` & `auto-group-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-group-1.3.0/PKG-INFO` & `auto-group-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-group
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tools for creating tree structures from flat list of dicts
 Home-page: https://gitlab.com/alda78/auto-group
 Author: Ales Adamek, Filip Cima
 Author-email: alda78@seznam.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -272,7 +272,8 @@
 - `dicts_into_list`: Converts dict of dicts into list structure.
 - `sort_list_of_dicts`: Sort list of dicts by selected column.
 - `dict_pass`: Whitelist dictionary attributes.
 - `dict_filter`: Blacklist dictionary attributes.
 - `list_into_dict`: Converts list into dict where dict keys are list indexes.
 - `dict_swap`: Swap dict keys into values and values into keys.
 - `map_dict_into_list`: Maps dict keys into list positions based on keys_map defined in key map list
+- `chunk_list`: Iterator which divides list into chunks with specified size
```

### Comparing `auto-group-1.3.0/README.md` & `auto-group-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -258,7 +258,8 @@
 - `dicts_into_list`: Converts dict of dicts into list structure.
 - `sort_list_of_dicts`: Sort list of dicts by selected column.
 - `dict_pass`: Whitelist dictionary attributes.
 - `dict_filter`: Blacklist dictionary attributes.
 - `list_into_dict`: Converts list into dict where dict keys are list indexes.
 - `dict_swap`: Swap dict keys into values and values into keys.
 - `map_dict_into_list`: Maps dict keys into list positions based on keys_map defined in key map list
+- `chunk_list`: Iterator which divides list into chunks with specified size
```

### Comparing `auto-group-1.3.0/auto_group/__init__.py` & `auto-group-1.3.1/auto_group/__init__.py`

 * *Files identical despite different names*

### Comparing `auto-group-1.3.0/auto_group/advanced.py` & `auto-group-1.3.1/auto_group/advanced.py`

 * *Files identical despite different names*

### Comparing `auto-group-1.3.0/auto_group/tools.py` & `auto-group-1.3.1/auto_group/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -74,7 +74,19 @@
     result = [None] * len(keys_map)
     map_of_keys = dict_swap(list_into_dict(keys_map))
 
     for key, value in d.items():
         list_index = map_of_keys[key]
         result[list_index] = value
     return result
+
+
+def chunk_list(l: list, chunk_size: int):
+    """
+    Iterator which divides list into chunks with specified size
+    :param l: List of items to be chunked
+    :param chunk_size: Chunk size
+    :return: 
+    """
+    for index in range(0, len(l), chunk_size):
+        chunk = l[index: index + chunk_size]
+        yield chunk
```

### Comparing `auto-group-1.3.0/auto_group.egg-info/PKG-INFO` & `auto-group-1.3.1/auto_group.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-group
-Version: 1.3.0
+Version: 1.3.1
 Summary: Tools for creating tree structures from flat list of dicts
 Home-page: https://gitlab.com/alda78/auto-group
 Author: Ales Adamek, Filip Cima
 Author-email: alda78@seznam.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -272,7 +272,8 @@
 - `dicts_into_list`: Converts dict of dicts into list structure.
 - `sort_list_of_dicts`: Sort list of dicts by selected column.
 - `dict_pass`: Whitelist dictionary attributes.
 - `dict_filter`: Blacklist dictionary attributes.
 - `list_into_dict`: Converts list into dict where dict keys are list indexes.
 - `dict_swap`: Swap dict keys into values and values into keys.
 - `map_dict_into_list`: Maps dict keys into list positions based on keys_map defined in key map list
+- `chunk_list`: Iterator which divides list into chunks with specified size
```

### Comparing `auto-group-1.3.0/setup.py` & `auto-group-1.3.1/setup.py`

 * *Files identical despite different names*

