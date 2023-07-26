# Comparing `tmp/aviewpy-1.3.3.tar.gz` & `tmp/aviewpy-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aviewpy-1.3.3.tar", last modified: Thu Jul 13 18:57:08 2023, max compression
+gzip compressed data, was "aviewpy-1.3.4.tar", last modified: Wed Jul 26 17:00:23 2023, max compression
```

## Comparing `aviewpy-1.3.3.tar` & `aviewpy-1.3.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 18:57:08.134859 aviewpy-1.3.3/
--rw-rw-rw-   0        0        0     1091 2022-12-20 23:52:04.000000 aviewpy-1.3.3/LICENSE
--rw-rw-rw-   0        0        0       34 2022-12-20 23:52:04.000000 aviewpy-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0      664 2023-07-13 18:57:08.133862 aviewpy-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-03-03 21:26:40.000000 aviewpy-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 18:57:07.424822 aviewpy-1.3.3/aviewpy/
--rw-rw-rw-   0        0        0       66 2022-12-20 23:55:30.000000 aviewpy-1.3.3/aviewpy/__init__.py
--rw-rw-rw-   0        0        0    11000 2023-04-12 16:38:53.000000 aviewpy-1.3.3/aviewpy/contact.py
--rw-rw-rw-   0        0        0     3770 2022-12-21 00:15:59.000000 aviewpy-1.3.3/aviewpy/cs.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:57:07.736820 aviewpy-1.3.3/aviewpy/files/
--rw-rw-rw-   0        0        0        0 2022-12-21 00:31:35.000000 aviewpy-1.3.3/aviewpy/files/__init__.py
--rw-rw-rw-   0        0        0      331 2023-04-28 18:01:01.000000 aviewpy-1.3.3/aviewpy/files/acf.py
--rw-rw-rw-   0        0        0      309 2023-04-28 18:01:16.000000 aviewpy-1.3.3/aviewpy/files/adm.py
--rw-rw-rw-   0        0        0     2141 2023-05-01 20:20:51.000000 aviewpy-1.3.3/aviewpy/files/bin.py
--rw-rw-rw-   0        0        0     1354 2023-02-24 15:52:22.000000 aviewpy-1.3.3/aviewpy/files/cmd.py
--rw-rw-rw-   0        0        0     7470 2023-05-12 18:33:02.000000 aviewpy-1.3.3/aviewpy/files/shell.py
--rw-rw-rw-   0        0        0     7063 2023-05-03 15:18:21.000000 aviewpy-1.3.3/aviewpy/files/to.py
--rw-rw-rw-   0        0        0     3035 2023-04-26 14:59:26.000000 aviewpy-1.3.3/aviewpy/model.py
--rw-rw-rw-   0        0        0     1102 2023-02-01 01:25:09.000000 aviewpy-1.3.3/aviewpy/move.py
--rw-rw-rw-   0        0        0     5232 2023-03-03 21:02:08.000000 aviewpy-1.3.3/aviewpy/objects.py
--rw-rw-rw-   0        0        0     2557 2023-07-07 22:57:12.000000 aviewpy-1.3.3/aviewpy/results.py
--rw-rw-rw-   0        0        0     8017 2023-07-11 17:41:18.000000 aviewpy-1.3.3/aviewpy/sim.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:57:07.913822 aviewpy-1.3.3/aviewpy/ui/
--rw-rw-rw-   0        0        0        0 2022-12-21 14:52:37.000000 aviewpy-1.3.3/aviewpy/ui/__init__.py
--rw-rw-rw-   0        0        0      941 2023-06-06 21:51:39.000000 aviewpy-1.3.3/aviewpy/ui/alerts.py
--rw-rw-rw-   0        0        0      875 2023-07-10 15:08:16.000000 aviewpy-1.3.3/aviewpy/ui/messages.py
--rw-rw-rw-   0        0        0     2807 2023-05-12 17:01:09.000000 aviewpy-1.3.3/aviewpy/ui/progressbar.py
--rw-rw-rw-   0        0        0      416 2023-02-14 13:55:42.000000 aviewpy-1.3.3/aviewpy/ui/windows.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:57:08.129862 aviewpy-1.3.3/aviewpy/utils/
--rw-rw-rw-   0        0        0       20 2022-12-21 00:01:02.000000 aviewpy-1.3.3/aviewpy/utils/__init__.py
--rw-rw-rw-   0        0        0     6041 2023-03-03 21:05:07.000000 aviewpy-1.3.3/aviewpy/utils/dereferencer.py
--rw-rw-rw-   0        0        0     1682 2023-03-18 19:28:15.000000 aviewpy-1.3.3/aviewpy/utils/excepthook.py
--rw-rw-rw-   0        0        0     5173 2022-12-20 23:52:04.000000 aviewpy-1.3.3/aviewpy/utils/res_to_csv.py
--rw-rw-rw-   0        0        0     3885 2023-06-06 14:31:27.000000 aviewpy-1.3.3/aviewpy/utils/utils.py
--rw-rw-rw-   0        0        0     5058 2023-05-31 12:46:11.000000 aviewpy-1.3.3/aviewpy/variables.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:57:07.544820 aviewpy-1.3.3/aviewpy.egg-info/
--rw-rw-rw-   0        0        0      664 2023-07-13 18:57:05.000000 aviewpy-1.3.3/aviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      774 2023-07-13 18:57:06.000000 aviewpy-1.3.3/aviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 18:57:05.000000 aviewpy-1.3.3/aviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-07-13 18:57:05.000000 aviewpy-1.3.3/aviewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-13 18:57:06.000000 aviewpy-1.3.3/aviewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-13 18:57:08.136861 aviewpy-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1094 2022-12-21 15:27:19.000000 aviewpy-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 18:57:08.130861 aviewpy-1.3.3/test/
--rw-rw-rw-   0        0        0     5501 2023-01-06 20:15:20.000000 aviewpy-1.3.3/test/test_shell.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:00:23.631529 aviewpy-1.3.4/
+-rw-rw-rw-   0        0        0     1091 2022-12-20 23:52:04.000000 aviewpy-1.3.4/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-12-20 23:52:04.000000 aviewpy-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      664 2023-07-26 17:00:23.631529 aviewpy-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-03-03 21:26:40.000000 aviewpy-1.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 17:00:23.571527 aviewpy-1.3.4/aviewpy/
+-rw-rw-rw-   0        0        0       66 2022-12-20 23:55:30.000000 aviewpy-1.3.4/aviewpy/__init__.py
+-rw-rw-rw-   0        0        0    11000 2023-04-12 16:38:53.000000 aviewpy-1.3.4/aviewpy/contact.py
+-rw-rw-rw-   0        0        0     3770 2022-12-21 00:15:59.000000 aviewpy-1.3.4/aviewpy/cs.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:00:23.617527 aviewpy-1.3.4/aviewpy/files/
+-rw-rw-rw-   0        0        0        0 2022-12-21 00:31:35.000000 aviewpy-1.3.4/aviewpy/files/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-04-28 18:01:01.000000 aviewpy-1.3.4/aviewpy/files/acf.py
+-rw-rw-rw-   0        0        0      309 2023-04-28 18:01:16.000000 aviewpy-1.3.4/aviewpy/files/adm.py
+-rw-rw-rw-   0        0        0     2327 2023-07-26 14:11:53.000000 aviewpy-1.3.4/aviewpy/files/bin.py
+-rw-rw-rw-   0        0        0     1412 2023-07-26 14:08:21.000000 aviewpy-1.3.4/aviewpy/files/cmd.py
+-rw-rw-rw-   0        0        0     7470 2023-05-12 18:33:02.000000 aviewpy-1.3.4/aviewpy/files/shell.py
+-rw-rw-rw-   0        0        0     7063 2023-05-03 15:18:21.000000 aviewpy-1.3.4/aviewpy/files/to.py
+-rw-rw-rw-   0        0        0     3035 2023-04-26 14:59:26.000000 aviewpy-1.3.4/aviewpy/model.py
+-rw-rw-rw-   0        0        0     1102 2023-02-01 01:25:09.000000 aviewpy-1.3.4/aviewpy/move.py
+-rw-rw-rw-   0        0        0     5232 2023-03-03 21:02:08.000000 aviewpy-1.3.4/aviewpy/objects.py
+-rw-rw-rw-   0        0        0     2557 2023-07-07 22:57:12.000000 aviewpy-1.3.4/aviewpy/results.py
+-rw-rw-rw-   0        0        0     8017 2023-07-11 17:41:18.000000 aviewpy-1.3.4/aviewpy/sim.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:00:23.622527 aviewpy-1.3.4/aviewpy/ui/
+-rw-rw-rw-   0        0        0        0 2022-12-21 14:52:37.000000 aviewpy-1.3.4/aviewpy/ui/__init__.py
+-rw-rw-rw-   0        0        0      941 2023-06-06 21:51:39.000000 aviewpy-1.3.4/aviewpy/ui/alerts.py
+-rw-rw-rw-   0        0        0      875 2023-07-10 15:08:16.000000 aviewpy-1.3.4/aviewpy/ui/messages.py
+-rw-rw-rw-   0        0        0     2807 2023-05-12 17:01:09.000000 aviewpy-1.3.4/aviewpy/ui/progressbar.py
+-rw-rw-rw-   0        0        0      416 2023-02-14 13:55:42.000000 aviewpy-1.3.4/aviewpy/ui/windows.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:00:23.628528 aviewpy-1.3.4/aviewpy/utils/
+-rw-rw-rw-   0        0        0       20 2022-12-21 00:01:02.000000 aviewpy-1.3.4/aviewpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     6041 2023-03-03 21:05:07.000000 aviewpy-1.3.4/aviewpy/utils/dereferencer.py
+-rw-rw-rw-   0        0        0     1682 2023-03-18 19:28:15.000000 aviewpy-1.3.4/aviewpy/utils/excepthook.py
+-rw-rw-rw-   0        0        0     5173 2022-12-20 23:52:04.000000 aviewpy-1.3.4/aviewpy/utils/res_to_csv.py
+-rw-rw-rw-   0        0        0     3885 2023-06-06 14:31:27.000000 aviewpy-1.3.4/aviewpy/utils/utils.py
+-rw-rw-rw-   0        0        0     5058 2023-05-31 12:46:11.000000 aviewpy-1.3.4/aviewpy/variables.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:00:23.607529 aviewpy-1.3.4/aviewpy.egg-info/
+-rw-rw-rw-   0        0        0      664 2023-07-26 17:00:23.000000 aviewpy-1.3.4/aviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      774 2023-07-26 17:00:23.000000 aviewpy-1.3.4/aviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 17:00:23.000000 aviewpy-1.3.4/aviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-07-26 17:00:23.000000 aviewpy-1.3.4/aviewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-26 17:00:23.000000 aviewpy-1.3.4/aviewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 17:00:23.631529 aviewpy-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1094 2022-12-21 15:27:19.000000 aviewpy-1.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 17:00:23.630527 aviewpy-1.3.4/test/
+-rw-rw-rw-   0        0        0     5501 2023-01-06 20:15:20.000000 aviewpy-1.3.4/test/test_shell.py
```

### Comparing `aviewpy-1.3.3/LICENSE` & `aviewpy-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/PKG-INFO` & `aviewpy-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aviewpy
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python tools for working with in the Adams View python environment
 Home-page: https://github.com/bthornton191/aviewpy
 Author: Ben Thornton
 Author-email: ben.thornton@hexagon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `aviewpy-1.3.3/aviewpy/contact.py` & `aviewpy-1.3.4/aviewpy/contact.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/cs.py` & `aviewpy-1.3.4/aviewpy/cs.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/files/bin.py` & `aviewpy-1.3.4/aviewpy/files/bin.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 from typing import Union
 import unicodedata
 
 import Adams  # type: ignore # noqa
 from Object import Object  # type: ignore # noqa
 
 
-def write_bin_file(filename: Path, entity: Object = None, alert=False):
+def write_bin_file(filename: Path, entity: Union[Object, str] = None, alert=False):
     cmd = 'file bin write file="{}" alert={}'.format(filename, 'yes' if alert else 'no')
-    if entity is not None:
+    if isinstance(entity, str):
+        cmd += f' entity={entity}'
+    elif isinstance(entity, Object):
         cmd += f' entity={entity.full_name}'
+    elif entity is not None:
+        raise TypeError('entity must be a string or an Object')
 
     Adams.execute_cmd(cmd)
 
 
 def read_bin_file(filename: Path, entity_name: str = None, alert=False):
     cmd = 'file bin read file="{}" alert={}'.format(filename, 'yes' if alert else 'no')
     if entity_name is not None:
```

### Comparing `aviewpy-1.3.3/aviewpy/files/cmd.py` & `aviewpy-1.3.4/aviewpy/files/cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from pathlib import Path
 
 from .bin import get_bin_version, read_bin_file, write_bin_file
 
 import Adams # type: ignore # isort: skip # pylint: disable=wrong-import-order
 
-def cached_model_import(cmd_file: Path):
+def cached_model_import(cmd_file: Path, mod_name: str = None, alert=False):
     """Imports a model from a cmd file and caches it in a binary file. Imports from the binary
     file if it already exists and is newer than the cmd file.
 
     Parameters
     ----------
     cmd_file : Path
         Adams View Command (.cmd) file containing a single model.
@@ -22,15 +22,15 @@
     # Check
     if (cached_file.exists()
             and cached_file.stat().st_mtime > cmd_file.stat().st_mtime
             and get_bin_version(cached_file) == os.environ['VERSION']):
 
         # If the cache file exists and it is newer than the cmd file and uses the same version,
         # Read in the cached file
-        read_bin_file(cached_file)
+        read_bin_file(cached_file, mod_name, alert=alert)
     
     else:
 
         # If the cached file does not exist or it is older than the cmd file
         # Read in the cmd file
         Adams.read_command_file(cmd_file)
```

### Comparing `aviewpy-1.3.3/aviewpy/files/shell.py` & `aviewpy-1.3.4/aviewpy/files/shell.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/files/to.py` & `aviewpy-1.3.4/aviewpy/files/to.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/model.py` & `aviewpy-1.3.4/aviewpy/model.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/move.py` & `aviewpy-1.3.4/aviewpy/move.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/objects.py` & `aviewpy-1.3.4/aviewpy/objects.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/results.py` & `aviewpy-1.3.4/aviewpy/results.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/sim.py` & `aviewpy-1.3.4/aviewpy/sim.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/ui/alerts.py` & `aviewpy-1.3.4/aviewpy/ui/alerts.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/ui/messages.py` & `aviewpy-1.3.4/aviewpy/ui/messages.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/ui/progressbar.py` & `aviewpy-1.3.4/aviewpy/ui/progressbar.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/utils/dereferencer.py` & `aviewpy-1.3.4/aviewpy/utils/dereferencer.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/utils/excepthook.py` & `aviewpy-1.3.4/aviewpy/utils/excepthook.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/utils/res_to_csv.py` & `aviewpy-1.3.4/aviewpy/utils/res_to_csv.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/utils/utils.py` & `aviewpy-1.3.4/aviewpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy/variables.py` & `aviewpy-1.3.4/aviewpy/variables.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/aviewpy.egg-info/PKG-INFO` & `aviewpy-1.3.4/aviewpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aviewpy
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python tools for working with in the Adams View python environment
 Home-page: https://github.com/bthornton191/aviewpy
 Author: Ben Thornton
 Author-email: ben.thornton@hexagon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `aviewpy-1.3.3/aviewpy.egg-info/SOURCES.txt` & `aviewpy-1.3.4/aviewpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/setup.py` & `aviewpy-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `aviewpy-1.3.3/test/test_shell.py` & `aviewpy-1.3.4/test/test_shell.py`

 * *Files identical despite different names*

