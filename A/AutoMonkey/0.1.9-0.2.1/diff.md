# Comparing `tmp/AutoMonkey-0.1.9.tar.gz` & `tmp/AutoMonkey-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoMonkey-0.1.9.tar", last modified: Tue Jul 25 20:16:41 2023, max compression
+gzip compressed data, was "AutoMonkey-0.2.1.tar", last modified: Wed Jul 26 20:07:25 2023, max compression
```

## Comparing `AutoMonkey-0.1.9.tar` & `AutoMonkey-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 20:16:41.877695 AutoMonkey-0.1.9/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      178 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/AUTHORS.rst
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 20:16:41.873695 AutoMonkey-0.1.9/AutoMonkey.egg-info/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    12099 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      729 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/SOURCES.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/dependency_links.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       51 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/entry_points.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/not-zip-safe
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      237 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/requires.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       11 2023-07-25 20:16:41.000000 AutoMonkey-0.1.9/AutoMonkey.egg-info/top_level.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3556 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/CONTRIBUTING.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       89 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/HISTORY.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1582 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/LICENSE
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      279 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/MANIFEST.in
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    12099 2023-07-25 20:16:41.877695 AutoMonkey-0.1.9/PKG-INFO
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    11362 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/README.md
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1098 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/README.rst
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 20:16:41.873695 AutoMonkey-0.1.9/automonkey/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      177 2023-07-25 20:04:39.000000 AutoMonkey-0.1.9/automonkey/__init__.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4700 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/app_funcs.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     9336 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/automonkey.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1730 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/constants.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      589 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/exceptions.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    10013 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/img_funcs.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4263 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/mouse_tracker.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4706 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/automonkey/utils.py
-drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-25 20:16:41.877695 AutoMonkey-0.1.9/docs/
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      611 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/Makefile
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       28 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/authors.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4901 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/conf.py
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       33 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/contributing.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       28 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/history.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      307 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/index.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1154 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/installation.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      772 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/make.bat
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       27 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/readme.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       75 2023-07-25 19:36:00.000000 AutoMonkey-0.1.9/docs/usage.rst
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      943 2023-07-25 20:12:40.000000 AutoMonkey-0.1.9/pyproject.toml
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      259 2023-07-25 20:01:33.000000 AutoMonkey-0.1.9/requirements.txt
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      425 2023-07-25 20:16:41.877695 AutoMonkey-0.1.9/setup.cfg
--rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1578 2023-07-25 20:04:39.000000 AutoMonkey-0.1.9/setup.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-26 20:07:25.824465 AutoMonkey-0.2.1/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      178 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/AUTHORS.rst
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-26 20:07:25.820465 AutoMonkey-0.2.1/AutoMonkey.egg-info/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    12099 2023-07-26 20:07:25.000000 AutoMonkey-0.2.1/AutoMonkey.egg-info/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      755 2023-07-26 20:07:25.000000 AutoMonkey-0.2.1/AutoMonkey.egg-info/SOURCES.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2023-07-26 20:07:25.000000 AutoMonkey-0.2.1/AutoMonkey.egg-info/dependency_links.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       51 2023-07-26 20:07:25.000000 AutoMonkey-0.2.1/AutoMonkey.egg-info/entry_points.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)        1 2023-07-26 20:07:25.000000 AutoMonkey-0.2.1/AutoMonkey.egg-info/not-zip-safe
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      237 2023-07-26 20:07:25.000000 AutoMonkey-0.2.1/AutoMonkey.egg-info/requires.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       11 2023-07-26 20:07:25.000000 AutoMonkey-0.2.1/AutoMonkey.egg-info/top_level.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     3556 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/CONTRIBUTING.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       89 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/HISTORY.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1582 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/LICENSE
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      279 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/MANIFEST.in
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    12099 2023-07-26 20:07:25.824465 AutoMonkey-0.2.1/PKG-INFO
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    11362 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/README.md
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1098 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/README.rst
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-26 20:07:25.824465 AutoMonkey-0.2.1/automonkey/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      177 2023-07-26 20:06:37.000000 AutoMonkey-0.2.1/automonkey/__init__.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4700 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/automonkey/app_funcs.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     9472 2023-07-26 20:00:17.000000 AutoMonkey-0.2.1/automonkey/automonkey.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1792 2023-07-26 19:55:04.000000 AutoMonkey-0.2.1/automonkey/constants.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      589 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/automonkey/exceptions.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)    10013 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/automonkey/img_funcs.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1269 2023-07-26 20:01:23.000000 AutoMonkey-0.2.1/automonkey/mouse_funcs.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4263 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/automonkey/mouse_tracker.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4706 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/automonkey/utils.py
+drwxrwxr-x   0 cosmin    (1000) cosmin    (1000)        0 2023-07-26 20:07:25.824465 AutoMonkey-0.2.1/docs/
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      611 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/docs/Makefile
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       28 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/docs/authors.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     4901 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/docs/conf.py
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       33 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/docs/contributing.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       28 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/docs/history.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      307 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/docs/index.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1154 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/docs/installation.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      772 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/docs/make.bat
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       27 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/docs/readme.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)       75 2023-07-25 19:36:00.000000 AutoMonkey-0.2.1/docs/usage.rst
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      943 2023-07-26 20:06:37.000000 AutoMonkey-0.2.1/pyproject.toml
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      259 2023-07-25 20:01:33.000000 AutoMonkey-0.2.1/requirements.txt
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)      425 2023-07-26 20:07:25.824465 AutoMonkey-0.2.1/setup.cfg
+-rw-rw-r--   0 cosmin    (1000) cosmin    (1000)     1578 2023-07-26 20:06:37.000000 AutoMonkey-0.2.1/setup.py
```

### Comparing `AutoMonkey-0.1.9/AutoMonkey.egg-info/PKG-INFO` & `AutoMonkey-0.2.1/AutoMonkey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMonkey
-Version: 0.1.9
+Version: 0.2.1
 Summary: Python Automation using Mouse and Keyboard, for the masses
 Home-page: https://github.com/MihailCosmin/automonkey
 Author: Mihail-Cosmin Munteanu
 Author-email: Mihail-Cosmin Munteanu <munteanumihailcosmin@gmail.com>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/MihailCosmin/AutoMonkey
 Project-URL: Bug Tracker, https://github.com/MihailCosmin/AutoMonkey/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AutoMonkey Version: 0.1.9 Summary: Python
+Metadata-Version: 2.1 Name: AutoMonkey Version: 0.2.1 Summary: Python
 Automation using Mouse and Keyboard, for the masses Home-page: https://
 github.com/MihailCosmin/automonkey Author: Mihail-Cosmin Munteanu Author-email:
 Mihail-Cosmin Munteanu
 gmail.com> License: GNU General Public License v3 Project-URL: Homepage, https:
 //github.com/MihailCosmin/AutoMonkey Project-URL: Bug Tracker, https://
 github.com/MihailCosmin/AutoMonkey/issues Keywords: automonkey Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `AutoMonkey-0.1.9/AutoMonkey.egg-info/SOURCES.txt` & `AutoMonkey-0.2.1/AutoMonkey.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 AutoMonkey.egg-info/top_level.txt
 automonkey/__init__.py
 automonkey/app_funcs.py
 automonkey/automonkey.py
 automonkey/constants.py
 automonkey/exceptions.py
 automonkey/img_funcs.py
+automonkey/mouse_funcs.py
 automonkey/mouse_tracker.py
 automonkey/utils.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
```

### Comparing `AutoMonkey-0.1.9/CONTRIBUTING.rst` & `AutoMonkey-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/LICENSE` & `AutoMonkey-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/PKG-INFO` & `AutoMonkey-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoMonkey
-Version: 0.1.9
+Version: 0.2.1
 Summary: Python Automation using Mouse and Keyboard, for the masses
 Home-page: https://github.com/MihailCosmin/automonkey
 Author: Mihail-Cosmin Munteanu
 Author-email: Mihail-Cosmin Munteanu <munteanumihailcosmin@gmail.com>
 License: GNU General Public License v3
 Project-URL: Homepage, https://github.com/MihailCosmin/AutoMonkey
 Project-URL: Bug Tracker, https://github.com/MihailCosmin/AutoMonkey/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: AutoMonkey Version: 0.1.9 Summary: Python
+Metadata-Version: 2.1 Name: AutoMonkey Version: 0.2.1 Summary: Python
 Automation using Mouse and Keyboard, for the masses Home-page: https://
 github.com/MihailCosmin/automonkey Author: Mihail-Cosmin Munteanu Author-email:
 Mihail-Cosmin Munteanu
 gmail.com> License: GNU General Public License v3 Project-URL: Homepage, https:
 //github.com/MihailCosmin/AutoMonkey Project-URL: Bug Tracker, https://
 github.com/MihailCosmin/AutoMonkey/issues Keywords: automonkey Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
```

### Comparing `AutoMonkey-0.1.9/README.md` & `AutoMonkey-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/README.rst` & `AutoMonkey-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/automonkey/app_funcs.py` & `AutoMonkey-0.2.1/automonkey/app_funcs.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/automonkey/automonkey.py` & `AutoMonkey-0.2.1/automonkey/automonkey.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,14 +54,19 @@
     from .app_funcs import maximize
     from .app_funcs import close
     from .app_funcs import restore
     from .app_funcs import focus
     from .app_funcs import msoffice_replace
     from .app_funcs import copy
 
+from .mouse_funcs import movedown
+from .mouse_funcs import moveleft
+from .mouse_funcs import moveright
+from .mouse_funcs import moveup
+
 from .img_funcs import _add_ext
 from .img_funcs import is_on_screen
 from .img_funcs import get_center
 from .img_funcs import diagonal_point
 
 from .utils import waitwhile
 from .utils import waituntil
```

### Comparing `AutoMonkey-0.1.9/automonkey/constants.py` & `AutoMonkey-0.2.1/automonkey/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,18 @@
     "rightclick",
     "doubleclick",
     "tripleclick",
     "scrollup",
     "scrolldown",
     "scrollleft",
     "scrollright",
+    "moveup",
+    "movedown",
+    "moveleft",
+    "moveright"
 )
 
 WAIT_ACTIONS = (
     "waitwhile",
     "waituntil",
 )
```

### Comparing `AutoMonkey-0.1.9/automonkey/exceptions.py` & `AutoMonkey-0.2.1/automonkey/exceptions.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/automonkey/img_funcs.py` & `AutoMonkey-0.2.1/automonkey/img_funcs.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/automonkey/mouse_tracker.py` & `AutoMonkey-0.2.1/automonkey/mouse_tracker.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/automonkey/utils.py` & `AutoMonkey-0.2.1/automonkey/utils.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/docs/Makefile` & `AutoMonkey-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/docs/conf.py` & `AutoMonkey-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/docs/installation.rst` & `AutoMonkey-0.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/docs/make.bat` & `AutoMonkey-0.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AutoMonkey-0.1.9/pyproject.toml` & `AutoMonkey-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "pyperclip>=1.8.2",
     "PyScreeze>=0.1.27",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AutoMonkey"
-version = "0.1.9"
+version = "0.2.1"
 authors = [
   { name="Mihail-Cosmin Munteanu", email="munteanumihailcosmin@gmail.com" },
 ]
 description = "Python Automation using Mouse and Keyboard, for the masses"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `AutoMonkey-0.1.9/setup.py` & `AutoMonkey-0.2.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='automonkey',
     name='automonkey',
     packages=find_packages(include=['automonkey', 'automonkey.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/MihailCosmin/automonkey',
-    version="0.1.9",
+    version="0.2.1",
     zip_safe=False,
 )
```

