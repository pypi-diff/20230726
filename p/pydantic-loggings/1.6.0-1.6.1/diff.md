# Comparing `tmp/pydantic-loggings-1.6.0.tar.gz` & `tmp/pydantic-loggings-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-1.6.0.tar", last modified: Wed Jul 26 18:22:25 2023, max compression
+gzip compressed data, was "pydantic-loggings-1.6.1.tar", last modified: Wed Jul 26 18:47:18 2023, max compression
```

## Comparing `pydantic-loggings-1.6.0.tar` & `pydantic-loggings-1.6.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.551401 pydantic-loggings-1.6.0/
--rw-r--r--   0 root         (0) root         (0)     3140 2023-07-26 18:22:25.551401 pydantic-loggings-1.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2313 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/README.md
--rw-r--r--   0 root         (0) root         (0)     2531 2023-07-26 18:22:16.000000 pydantic-loggings-1.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 18:22:25.551401 pydantic-loggings-1.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.543401 pydantic-loggings-1.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.543401 pydantic-loggings-1.6.0/src/pydantic_loggings/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.547401 pydantic-loggings-1.6.0/src/pydantic_loggings/base/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/base/loggings.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.547401 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/loggings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.551401 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/__init__.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/filters.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/formatters.py
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/handlers.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/loggers.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/rich/loggings.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/types_.py
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-26 18:22:15.000000 pydantic-loggings-1.6.0/src/pydantic_loggings/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:22:25.547401 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3140 2023-07-26 18:22:25.000000 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1097 2023-07-26 18:22:25.000000 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 18:22:25.000000 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-07-26 18:22:25.000000 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 18:22:25.000000 pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:47:18.782350 pydantic-loggings-1.6.1/
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-07-26 18:47:18.782350 pydantic-loggings-1.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 18:47:18.782350 pydantic-loggings-1.6.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:47:18.778350 pydantic-loggings-1.6.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:47:18.782350 pydantic-loggings-1.6.1/src/pydantic_loggings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:47:18.782350 pydantic-loggings-1.6.1/src/pydantic_loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/base/loggings.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:47:18.782350 pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/loggings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:47:18.782350 pydantic-loggings-1.6.1/src/pydantic_loggings/rich/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/rich/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/rich/filters.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/rich/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/rich/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/rich/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/rich/loggings.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/types_.py
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-26 18:47:10.000000 pydantic-loggings-1.6.1/src/pydantic_loggings/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 18:47:18.782350 pydantic-loggings-1.6.1/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-07-26 18:47:18.000000 pydantic-loggings-1.6.1/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-07-26 18:47:18.000000 pydantic-loggings-1.6.1/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 18:47:18.000000 pydantic-loggings-1.6.1/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-26 18:47:18.000000 pydantic-loggings-1.6.1/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-26 18:47:18.000000 pydantic-loggings-1.6.1/src/pydantic_loggings.egg-info/top_level.txt
```

### Comparing `pydantic-loggings-1.6.0/PKG-INFO` & `pydantic-loggings-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 1.6.0
+Version: 1.6.1
 Summary: Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-loggings
 Project-URL: Source, https://github.com/m9810223/pydantic-loggings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pydantic-loggings-1.6.0/README.md` & `pydantic-loggings-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.6.0/pyproject.toml` & `pydantic-loggings-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Homepage = "https://github.com/m9810223/pydantic-loggings"
 Source = "https://github.com/m9810223/pydantic-loggings"
 
 
 [project]
 name = "pydantic-loggings"
 description = "Configure 🎁 Your 🤗 Python 🐍 Logging 📝"
-version = "1.6.0"
+version = "1.6.1"
 authors = [{ name = "m9810223", email = "m9810223@gmail.com" }]
 requires-python = ">=3.9"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.9",
```

### Comparing `pydantic-loggings-1.6.0/src/pydantic_loggings/base/loggings.py` & `pydantic-loggings-1.6.1/src/pydantic_loggings/base/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.6.0/src/pydantic_loggings/mixins.py` & `pydantic-loggings-1.6.1/src/pydantic_loggings/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/formatters.py` & `pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/handlers.py` & `pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/loggers.py` & `pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/loggers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.6.0/src/pydantic_loggings/not_set/loggings.py` & `pydantic-loggings-1.6.1/src/pydantic_loggings/not_set/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.6.0/src/pydantic_loggings/rich/handlers.py` & `pydantic-loggings-1.6.1/src/pydantic_loggings/rich/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.6.0/src/pydantic_loggings/rich/loggings.py` & `pydantic-loggings-1.6.1/src/pydantic_loggings/rich/loggings.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/PKG-INFO` & `pydantic-loggings-1.6.1/src/pydantic_loggings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 1.6.0
+Version: 1.6.1
 Summary: Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-loggings
 Project-URL: Source, https://github.com/m9810223/pydantic-loggings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pydantic-loggings-1.6.0/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-1.6.1/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

