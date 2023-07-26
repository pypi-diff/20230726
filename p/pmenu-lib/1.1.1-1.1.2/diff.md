# Comparing `tmp/pmenu_lib-1.1.1.tar.gz` & `tmp/pmenu_lib-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmenu_lib-1.1.1.tar", last modified: Wed Jul 26 17:20:17 2023, max compression
+gzip compressed data, was "pmenu_lib-1.1.2.tar", last modified: Wed Jul 26 17:25:29 2023, max compression
```

## Comparing `pmenu_lib-1.1.1.tar` & `pmenu_lib-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 17:20:17.249842 pmenu_lib-1.1.1/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1073 2023-07-26 17:20:17.249842 pmenu_lib-1.1.1/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      719 2023-07-26 17:18:52.000000 pmenu_lib-1.1.1/README.md
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 17:20:17.249842 pmenu_lib-1.1.1/pmenu_lib/
--rw-rw-r--   0 omega     (1000) omega     (1000)       29 2023-07-26 10:03:29.000000 pmenu_lib-1.1.1/pmenu_lib/__init__.py
--rw-rw-r--   0 omega     (1000) omega     (1000)     3755 2023-07-26 17:05:55.000000 pmenu_lib-1.1.1/pmenu_lib/pmenu_lib.py
-drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 17:20:17.249842 pmenu_lib-1.1.1/pmenu_lib.egg-info/
--rw-rw-r--   0 omega     (1000) omega     (1000)     1073 2023-07-26 17:20:17.000000 pmenu_lib-1.1.1/pmenu_lib.egg-info/PKG-INFO
--rw-rw-r--   0 omega     (1000) omega     (1000)      195 2023-07-26 17:20:17.000000 pmenu_lib-1.1.1/pmenu_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-26 17:20:17.000000 pmenu_lib-1.1.1/pmenu_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       10 2023-07-26 17:20:17.000000 pmenu_lib-1.1.1/pmenu_lib.egg-info/top_level.txt
--rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-26 17:20:17.249842 pmenu_lib-1.1.1/setup.cfg
--rw-rw-r--   0 omega     (1000) omega     (1000)      506 2023-07-26 17:20:00.000000 pmenu_lib-1.1.1/setup.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 17:25:29.199545 pmenu_lib-1.1.2/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1070 2023-07-26 17:25:29.199545 pmenu_lib-1.1.2/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      716 2023-07-26 17:25:03.000000 pmenu_lib-1.1.2/README.md
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 17:25:29.199545 pmenu_lib-1.1.2/pmenu_lib/
+-rw-rw-r--   0 omega     (1000) omega     (1000)       29 2023-07-26 10:03:29.000000 pmenu_lib-1.1.2/pmenu_lib/__init__.py
+-rw-rw-r--   0 omega     (1000) omega     (1000)     3755 2023-07-26 17:05:55.000000 pmenu_lib-1.1.2/pmenu_lib/pmenu_lib.py
+drwxrwxr-x   0 omega     (1000) omega     (1000)        0 2023-07-26 17:25:29.199545 pmenu_lib-1.1.2/pmenu_lib.egg-info/
+-rw-rw-r--   0 omega     (1000) omega     (1000)     1070 2023-07-26 17:25:29.000000 pmenu_lib-1.1.2/pmenu_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 omega     (1000) omega     (1000)      195 2023-07-26 17:25:29.000000 pmenu_lib-1.1.2/pmenu_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)        1 2023-07-26 17:25:29.000000 pmenu_lib-1.1.2/pmenu_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       10 2023-07-26 17:25:29.000000 pmenu_lib-1.1.2/pmenu_lib.egg-info/top_level.txt
+-rw-rw-r--   0 omega     (1000) omega     (1000)       38 2023-07-26 17:25:29.199545 pmenu_lib-1.1.2/setup.cfg
+-rw-rw-r--   0 omega     (1000) omega     (1000)      506 2023-07-26 17:25:07.000000 pmenu_lib-1.1.2/setup.py
```

### Comparing `pmenu_lib-1.1.1/PKG-INFO` & `pmenu_lib-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmenu_lib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Sleek dmenu alternative written in Python and powered by curses.
 Home-page: https://github.com/Julynx/pmenu
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
@@ -50,8 +50,8 @@
 <br>
 
 ## Menu bindings
 
 - **Up arrow**: Highlight the previous menu entry.
 - **Down arrow**: Highlight the next menu entry.
 - **Enter**: Select the highlighted entry.
-- **Escape**: Close the menu.
+- **Esc**: Close the menu.
```

### Comparing `pmenu_lib-1.1.1/README.md` & `pmenu_lib-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 <br>
 
 ## Menu bindings
 
 - **Up arrow**: Highlight the previous menu entry.
 - **Down arrow**: Highlight the next menu entry.
 - **Enter**: Select the highlighted entry.
-- **Escape**: Close the menu.
+- **Esc**: Close the menu.
```

### Comparing `pmenu_lib-1.1.1/pmenu_lib/pmenu_lib.py` & `pmenu_lib-1.1.2/pmenu_lib/pmenu_lib.py`

 * *Files identical despite different names*

### Comparing `pmenu_lib-1.1.1/pmenu_lib.egg-info/PKG-INFO` & `pmenu_lib-1.1.2/pmenu_lib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmenu-lib
-Version: 1.1.1
+Version: 1.1.2
 Summary: Sleek dmenu alternative written in Python and powered by curses.
 Home-page: https://github.com/Julynx/pmenu
 Author: Julio Cabria
 Author-email: juliocabria@tutanota.com
 Maintainer: Julio Cabria
 Maintainer-email: juliocabria@tutanota.com
 License: GPLv2
@@ -50,8 +50,8 @@
 <br>
 
 ## Menu bindings
 
 - **Up arrow**: Highlight the previous menu entry.
 - **Down arrow**: Highlight the next menu entry.
 - **Enter**: Select the highlighted entry.
-- **Escape**: Close the menu.
+- **Esc**: Close the menu.
```

