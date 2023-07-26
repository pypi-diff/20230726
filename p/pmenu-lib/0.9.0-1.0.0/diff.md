# Comparing `tmp/pmenu_lib-0.9.0.tar.gz` & `tmp/pmenu_lib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmenu_lib-0.9.0.tar", last modified: Wed Jul 26 11:21:46 2023, max compression
+gzip compressed data, was "pmenu_lib-1.0.0.tar", last modified: Wed Jul 26 11:55:53 2023, max compression
```

## Comparing `pmenu_lib-0.9.0.tar` & `pmenu_lib-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 11:21:46.535076 pmenu_lib-0.9.0/
--rw-rw-r--   0 omega     (1000) omega     (1000)      869 2023-07-26 11:21:46.531077 pmenu_lib-0.9.0/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      515 2023-07-26 11:17:18.000000 pmenu_lib-0.9.0/README.md
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 11:21:46.531077 pmenu_lib-0.9.0/pmenu_lib/
--rw-rw-r--   0 omega     (1000) omega     (1000)       29 2023-07-26 10:03:29.000000 pmenu_lib-0.9.0/pmenu_lib/__init__.py
--rw-rw-r--   0 omega     (1000) omega     (1000)     2025 2023-07-26 10:04:16.000000 pmenu_lib-0.9.0/pmenu_lib/pmenu_lib.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 11:21:46.531077 pmenu_lib-0.9.0/pmenu_lib.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)      869 2023-07-26 11:21:46.000000 pmenu_lib-0.9.0/pmenu_lib.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      195 2023-07-26 11:21:46.000000 pmenu_lib-0.9.0/pmenu_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-26 11:21:46.000000 pmenu_lib-0.9.0/pmenu_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       10 2023-07-26 11:21:46.000000 pmenu_lib-0.9.0/pmenu_lib.egg-info/top_level.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-26 11:21:46.535076 pmenu_lib-0.9.0/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      505 2023-07-26 10:03:31.000000 pmenu_lib-0.9.0/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 11:55:53.432474 pmenu_lib-1.0.0/
+-rw-rw-r--   0 omega     (1000) omega     (1000)      869 2023-07-26 11:55:53.432474 pmenu_lib-1.0.0/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      515 2023-07-26 11:17:18.000000 pmenu_lib-1.0.0/README.md
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 11:55:53.432474 pmenu_lib-1.0.0/pmenu_lib/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       29 2023-07-26 10:03:29.000000 pmenu_lib-1.0.0/pmenu_lib/__init__.py
+-rw-rw-r--   0 omega     (1000) omega     (1000)     2088 2023-07-26 11:54:44.000000 pmenu_lib-1.0.0/pmenu_lib/pmenu_lib.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 11:55:53.432474 pmenu_lib-1.0.0/pmenu_lib.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)      869 2023-07-26 11:55:53.000000 pmenu_lib-1.0.0/pmenu_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      195 2023-07-26 11:55:53.000000 pmenu_lib-1.0.0/pmenu_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-26 11:55:53.000000 pmenu_lib-1.0.0/pmenu_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       10 2023-07-26 11:55:53.000000 pmenu_lib-1.0.0/pmenu_lib.egg-info/top_level.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-26 11:55:53.432474 pmenu_lib-1.0.0/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      506 2023-07-26 11:55:26.000000 pmenu_lib-1.0.0/setup.py
```

### Comparing `pmenu_lib-0.9.0/PKG-INFO` & `pmenu_lib-1.0.0/pmenu_lib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pmenu_lib
-Version: 0.9.0
+Name: pmenu-lib
+Version: 1.0.0
 Summary: Sleek dmenu alternative written in Python and powered by curses.
 Home-page: https://github.com/Julynx/pmenu
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

### Comparing `pmenu_lib-0.9.0/README.md` & `pmenu_lib-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pmenu_lib-0.9.0/pmenu_lib/pmenu_lib.py` & `pmenu_lib-1.0.0/pmenu_lib/pmenu_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,18 @@
 
     Args:
         lines: The lines to display in the menu.
 
     Returns:
         The selected option or None if the user quits the menu.
     """
-    return curses.wrapper(_display_menu, lines)
+    try:
+        return curses.wrapper(_display_menu, lines)
+    except KeyboardInterrupt:
+        return None
 
 
 def _display_menu(stdscr, lines):
     """
     Display a menu with the given lines and return the selected option.
 
     Args:
```

### Comparing `pmenu_lib-0.9.0/pmenu_lib.egg-info/PKG-INFO` & `pmenu_lib-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pmenu-lib
-Version: 0.9.0
+Name: pmenu_lib
+Version: 1.0.0
 Summary: Sleek dmenu alternative written in Python and powered by curses.
 Home-page: https://github.com/Julynx/pmenu
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
```

