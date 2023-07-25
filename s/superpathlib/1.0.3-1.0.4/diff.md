# Comparing `tmp/superpathlib-1.0.3.tar.gz` & `tmp/superpathlib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpathlib-1.0.3.tar", last modified: Tue Jul 25 23:45:19 2023, max compression
+gzip compressed data, was "superpathlib-1.0.4.tar", last modified: Tue Jul 25 23:51:01 2023, max compression
```

## Comparing `superpathlib-1.0.3.tar` & `superpathlib-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:45:19.797528 superpathlib-1.0.3/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-07-25 22:35:03.000000 superpathlib-1.0.3/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-07-25 23:45:19.797528 superpathlib-1.0.3/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2630 2023-07-25 23:41:53.000000 superpathlib-1.0.3/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:45:19.797528 superpathlib-1.0.3/plib/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       23 2023-07-25 22:35:03.000000 superpathlib-1.0.3/plib/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)    15444 2023-07-25 23:42:51.000000 superpathlib-1.0.3/plib/plib.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1152 2023-07-25 22:35:03.000000 superpathlib-1.0.3/plib/tags.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      857 2023-07-25 22:35:03.000000 superpathlib-1.0.3/plib/utils.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      559 2023-07-25 23:40:58.000000 superpathlib-1.0.3/pyproject.toml
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-07-25 23:45:19.797528 superpathlib-1.0.3/setup.cfg
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:45:19.797528 superpathlib-1.0.3/superpathlib.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-07-25 23:45:19.000000 superpathlib-1.0.3/superpathlib.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      373 2023-07-25 23:45:19.000000 superpathlib-1.0.3/superpathlib.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-07-25 23:45:19.000000 superpathlib-1.0.3/superpathlib.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-07-25 23:45:19.000000 superpathlib-1.0.3/superpathlib.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        5 2023-07-25 23:45:19.000000 superpathlib-1.0.3/superpathlib.egg-info/top_level.txt
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:45:19.797528 superpathlib-1.0.3/tests/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1649 2023-07-25 23:32:35.000000 superpathlib-1.0.3/tests/test_content.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1678 2023-07-25 23:15:42.000000 superpathlib-1.0.3/tests/test_encrypted_content.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2045 2023-07-25 23:43:38.000000 superpathlib-1.0.3/tests/test_functionality.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      937 2023-07-25 23:38:40.000000 superpathlib-1.0.3/tests/test_metadata.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:51:01.340200 superpathlib-1.0.4/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-07-25 23:50:13.000000 superpathlib-1.0.4/LICENSE
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-07-25 23:51:01.340200 superpathlib-1.0.4/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2630 2023-07-25 23:50:13.000000 superpathlib-1.0.4/README.md
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:51:01.336200 superpathlib-1.0.4/plib/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       23 2023-07-25 23:50:13.000000 superpathlib-1.0.4/plib/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)    15444 2023-07-25 23:50:13.000000 superpathlib-1.0.4/plib/plib.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1152 2023-07-25 23:50:13.000000 superpathlib-1.0.4/plib/tags.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      857 2023-07-25 23:50:13.000000 superpathlib-1.0.4/plib/utils.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      722 2023-07-25 23:50:25.000000 superpathlib-1.0.4/pyproject.toml
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-07-25 23:51:01.340200 superpathlib-1.0.4/setup.cfg
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:51:01.340200 superpathlib-1.0.4/superpathlib.egg-info/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-07-25 23:51:01.000000 superpathlib-1.0.4/superpathlib.egg-info/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      373 2023-07-25 23:51:01.000000 superpathlib-1.0.4/superpathlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-07-25 23:51:01.000000 superpathlib-1.0.4/superpathlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-07-25 23:51:01.000000 superpathlib-1.0.4/superpathlib.egg-info/requires.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        5 2023-07-25 23:51:01.000000 superpathlib-1.0.4/superpathlib.egg-info/top_level.txt
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:51:01.340200 superpathlib-1.0.4/tests/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1649 2023-07-25 23:50:13.000000 superpathlib-1.0.4/tests/test_content.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1678 2023-07-25 23:50:13.000000 superpathlib-1.0.4/tests/test_encrypted_content.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2045 2023-07-25 23:50:13.000000 superpathlib-1.0.4/tests/test_functionality.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      937 2023-07-25 23:50:13.000000 superpathlib-1.0.4/tests/test_metadata.py
```

### Comparing `superpathlib-1.0.3/LICENSE` & `superpathlib-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.3/PKG-INFO` & `superpathlib-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Extended Pathlib
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/superpathlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `superpathlib-1.0.3/README.md` & `superpathlib-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.3/plib/plib.py` & `superpathlib-1.0.4/plib/plib.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.3/plib/tags.py` & `superpathlib-1.0.4/plib/tags.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.3/plib/utils.py` & `superpathlib-1.0.4/plib/utils.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.3/superpathlib.egg-info/PKG-INFO` & `superpathlib-1.0.4/superpathlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.0.3
+Version: 1.0.4
 Summary: Extended Pathlib
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/superpathlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `superpathlib-1.0.3/tests/test_content.py` & `superpathlib-1.0.4/tests/test_content.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.3/tests/test_encrypted_content.py` & `superpathlib-1.0.4/tests/test_encrypted_content.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.3/tests/test_functionality.py` & `superpathlib-1.0.4/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.3/tests/test_metadata.py` & `superpathlib-1.0.4/tests/test_metadata.py`

 * *Files identical despite different names*

