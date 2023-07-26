# Comparing `tmp/arthub_login_widgets-0.4.5.tar.gz` & `tmp/arthub_login_widgets-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arthub_login_widgets-0.4.5.tar", last modified: Mon Jul 17 10:21:50 2023, max compression
+gzip compressed data, was "arthub_login_widgets-0.4.6.tar", last modified: Wed Jul 26 14:48:48 2023, max compression
```

## Comparing `arthub_login_widgets-0.4.5.tar` & `arthub_login_widgets-0.4.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 10:21:50.791120 arthub_login_widgets-0.4.5/
--rw-rw-rw-   0        0        0      375 2023-07-17 10:21:50.790123 arthub_login_widgets-0.4.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 10:21:50.762126 arthub_login_widgets-0.4.5/arthub_login_widgets/
--rw-rw-rw-   0        0        0      435 2023-03-23 06:34:09.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/__init__.py
--rw-rw-rw-   0        0        0       23 2023-07-17 10:21:45.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/__version__.py
--rw-rw-rw-   0        0        0      590 2023-07-17 06:03:02.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/constants.py
--rw-rw-rw-   0        0        0    10243 2023-07-17 10:21:32.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/core.py
--rw-rw-rw-   0        0        0     1182 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/filesystem.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:21:50.766187 arthub_login_widgets-0.4.5/arthub_login_widgets/resources/
--rw-rw-rw-   0        0        0        0 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/resources/__init__.py
--rw-rw-rw-   0        0        0    12338 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/resources/arthub_white.png
--rw-rw-rw-   0        0        0     1073 2023-07-17 10:16:02.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/resources/style.qss
-drwxrwxrwx   0        0        0        0 2023-07-17 10:21:50.772097 arthub_login_widgets-0.4.5/arthub_login_widgets/test/
--rw-rw-rw-   0        0        0      173 2023-01-31 11:18:49.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/test/__init__.py
--rw-rw-rw-   0        0        0     1628 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/test/test_core.py
--rw-rw-rw-   0        0        0      766 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/test/test_filesystem.py
--rw-rw-rw-   0        0        0      699 2023-02-07 12:54:18.000000 arthub_login_widgets-0.4.5/arthub_login_widgets/test/test_imports.py
-drwxrwxrwx   0        0        0        0 2023-07-17 10:21:50.783142 arthub_login_widgets-0.4.5/arthub_login_widgets.egg-info/
--rw-rw-rw-   0        0        0      375 2023-07-17 10:21:50.000000 arthub_login_widgets-0.4.5/arthub_login_widgets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1177 2023-07-17 10:21:50.000000 arthub_login_widgets-0.4.5/arthub_login_widgets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 10:21:50.000000 arthub_login_widgets-0.4.5/arthub_login_widgets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-07-17 10:21:50.000000 arthub_login_widgets-0.4.5/arthub_login_widgets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-07-17 10:21:50.000000 arthub_login_widgets-0.4.5/arthub_login_widgets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 10:21:50.792117 arthub_login_widgets-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0     1219 2023-06-27 13:46:39.000000 arthub_login_widgets-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:48.256134 arthub_login_widgets-0.4.6/
+-rw-rw-rw-   0        0        0      375 2023-07-26 14:48:48.255623 arthub_login_widgets-0.4.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:48.227686 arthub_login_widgets-0.4.6/arthub_login_widgets/
+-rw-rw-rw-   0        0        0      435 2023-03-23 06:34:09.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-07-26 14:48:42.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/__version__.py
+-rw-rw-rw-   0        0        0      590 2023-07-17 06:03:02.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/constants.py
+-rw-rw-rw-   0        0        0    10237 2023-07-26 14:46:28.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/core.py
+-rw-rw-rw-   0        0        0     1182 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/filesystem.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:48.232614 arthub_login_widgets-0.4.6/arthub_login_widgets/resources/
+-rw-rw-rw-   0        0        0        0 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/resources/__init__.py
+-rw-rw-rw-   0        0        0    12338 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/resources/arthub_white.png
+-rw-rw-rw-   0        0        0     1073 2023-07-17 10:16:02.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/resources/style.qss
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:48.238647 arthub_login_widgets-0.4.6/arthub_login_widgets/test/
+-rw-rw-rw-   0        0        0      173 2023-01-31 11:18:49.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/test/__init__.py
+-rw-rw-rw-   0        0        0     1628 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/test/test_core.py
+-rw-rw-rw-   0        0        0      766 2023-02-08 03:29:52.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/test/test_filesystem.py
+-rw-rw-rw-   0        0        0      699 2023-02-07 12:54:18.000000 arthub_login_widgets-0.4.6/arthub_login_widgets/test/test_imports.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:48.249700 arthub_login_widgets-0.4.6/arthub_login_widgets.egg-info/
+-rw-rw-rw-   0        0        0      375 2023-07-26 14:48:47.000000 arthub_login_widgets-0.4.6/arthub_login_widgets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1177 2023-07-26 14:48:48.000000 arthub_login_widgets-0.4.6/arthub_login_widgets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 14:48:47.000000 arthub_login_widgets-0.4.6/arthub_login_widgets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-07-26 14:48:47.000000 arthub_login_widgets-0.4.6/arthub_login_widgets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-07-26 14:48:47.000000 arthub_login_widgets-0.4.6/arthub_login_widgets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 14:48:48.256649 arthub_login_widgets-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-07-26 14:47:14.000000 arthub_login_widgets-0.4.6/setup.py
```

### Comparing `arthub_login_widgets-0.4.5/arthub_login_widgets/constants.py` & `arthub_login_widgets-0.4.6/arthub_login_widgets/constants.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.5/arthub_login_widgets/core.py` & `arthub_login_widgets-0.4.6/arthub_login_widgets/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 # Import built-in modules
 import logging
 import webbrowser
 import os
 
 # Import third-party modules
-from qtpy import QtCore
-from qtpy import QtGui
-from qtpy import QtWidgets
+from Qt import QtCore
+from Qt import QtGui
+from Qt import QtWidgets
 
 # Import local modules
 from arthub_login_widgets.constants import ARTHUB_RESET_PASSWORD_WEB_URL
 from arthub_login_widgets.constants import ARTHUB_SET_ACCOUNT_INFO_WEB_URL
 from arthub_login_widgets.constants import UI_TEXT_MAP
 from arthub_login_widgets.filesystem import get_login_account
 from arthub_login_widgets.filesystem import get_resource_file
```

### Comparing `arthub_login_widgets-0.4.5/arthub_login_widgets/filesystem.py` & `arthub_login_widgets-0.4.6/arthub_login_widgets/filesystem.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.5/arthub_login_widgets/resources/arthub_white.png` & `arthub_login_widgets-0.4.6/arthub_login_widgets/resources/arthub_white.png`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.5/arthub_login_widgets/resources/style.qss` & `arthub_login_widgets-0.4.6/arthub_login_widgets/resources/style.qss`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.5/arthub_login_widgets/test/test_core.py` & `arthub_login_widgets-0.4.6/arthub_login_widgets/test/test_core.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.5/arthub_login_widgets/test/test_filesystem.py` & `arthub_login_widgets-0.4.6/arthub_login_widgets/test/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.5/arthub_login_widgets/test/test_imports.py` & `arthub_login_widgets-0.4.6/arthub_login_widgets/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.5/arthub_login_widgets.egg-info/SOURCES.txt` & `arthub_login_widgets-0.4.6/arthub_login_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arthub_login_widgets-0.4.5/setup.py` & `arthub_login_widgets-0.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,10 +32,10 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
     install_requires=[
         "arthub_api==1.4.1",
         "platformdirs==2.0.2",
-        "qtpy"
+        "Qt.py"
     ]
 )
```

