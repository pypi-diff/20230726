# Comparing `tmp/hivecode-0.0.0.8.20.tar.gz` & `tmp/hivecode-0.0.0.8.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hivecode-0.0.0.8.20.tar", last modified: Wed Jul 26 06:19:30 2023, max compression
+gzip compressed data, was "hivecode-0.0.0.8.21.tar", last modified: Wed Jul 26 06:37:27 2023, max compression
```

## Comparing `hivecode-0.0.0.8.20.tar` & `hivecode-0.0.0.8.21.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.548434 hivecode-0.0.0.8.20/
--rw-rw-rw-   0        0        0     3790 2023-07-26 06:19:30.548434 hivecode-0.0.0.8.20/PKG-INFO
--rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.20/README.rst
--rw-rw-rw-   0        0        0     1402 2023-07-26 06:07:55.000000 hivecode-0.0.0.8.20/pyproject.toml
--rw-rw-rw-   0        0        0      226 2023-07-20 05:57:35.000000 hivecode-0.0.0.8.20/requirements.txt
--rw-rw-rw-   0        0        0     1182 2023-07-26 06:19:30.562919 hivecode-0.0.0.8.20/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.487618 hivecode-0.0.0.8.20/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.498784 hivecode-0.0.0.8.20/src/hiveadb/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hiveadb/__init__.py
--rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.20/src/hiveadb/eda.py
--rw-rw-rw-   0        0        0    11500 2023-07-26 06:04:36.000000 hivecode-0.0.0.8.20/src/hiveadb/function.py
--rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.20/src/hiveadb/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hiveadb/py.typed
-drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.524418 hivecode-0.0.0.8.20/src/hivecode.egg-info/
--rw-rw-rw-   0        0        0     3790 2023-07-26 06:19:30.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      749 2023-07-26 06:19:30.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 06:19:30.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      314 2023-07-26 06:19:30.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-26 06:19:30.000000 hivecode-0.0.0.8.20/src/hivecode.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.537554 hivecode-0.0.0.8.20/src/hivecore/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivecore/__init__.py
--rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.20/src/hivecore/constant.py
--rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.20/src/hivecore/decorator.py
--rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.20/src/hivecore/eda.py
--rw-rw-rw-   0        0        0     7676 2023-07-26 05:32:41.000000 hivecode-0.0.0.8.20/src/hivecore/functions.py
--rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.20/src/hivecore/patterns.py
--rw-rw-rw-   0        0        0    28728 2023-07-20 03:05:40.000000 hivecode-0.0.0.8.20/src/hivecore/preprocess.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivecore/py.typed
--rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.20/src/hivecore/visual.py
-drwxrwxrwx   0        0        0        0 2023-07-26 06:19:30.546401 hivecode-0.0.0.8.20/src/hivesignal/
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/__init__.py
--rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/analysis.py
--rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/eda.py
--rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/io.py
--rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/py.typed
--rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.20/src/hivesignal/transform.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.537077 hivecode-0.0.0.8.21/
+-rw-rw-rw-   0        0        0     3790 2023-07-26 06:37:27.537077 hivecode-0.0.0.8.21/PKG-INFO
+-rw-rw-rw-   0        0        0     2807 2023-04-11 20:04:04.000000 hivecode-0.0.0.8.21/README.rst
+-rw-rw-rw-   0        0        0     1402 2023-07-26 06:37:02.000000 hivecode-0.0.0.8.21/pyproject.toml
+-rw-rw-rw-   0        0        0      226 2023-07-20 05:57:35.000000 hivecode-0.0.0.8.21/requirements.txt
+-rw-rw-rw-   0        0        0     1182 2023-07-26 06:37:27.540600 hivecode-0.0.0.8.21/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.474543 hivecode-0.0.0.8.21/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.495233 hivecode-0.0.0.8.21/src/hiveadb/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hiveadb/__init__.py
+-rw-rw-rw-   0        0        0     3690 2023-04-12 04:08:02.000000 hivecode-0.0.0.8.21/src/hiveadb/eda.py
+-rw-rw-rw-   0        0        0    11500 2023-07-26 06:04:36.000000 hivecode-0.0.0.8.21/src/hiveadb/function.py
+-rw-rw-rw-   0        0        0     3694 2023-07-26 06:36:39.000000 hivecode-0.0.0.8.21/src/hiveadb/functions.py
+-rw-rw-rw-   0        0        0    86747 2023-04-11 23:45:25.000000 hivecode-0.0.0.8.21/src/hiveadb/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hiveadb/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.516405 hivecode-0.0.0.8.21/src/hivecode.egg-info/
+-rw-rw-rw-   0        0        0     3790 2023-07-26 06:37:27.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      774 2023-07-26 06:37:27.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 06:37:27.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-18 05:08:33.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      314 2023-07-26 06:37:27.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-26 06:37:27.000000 hivecode-0.0.0.8.21/src/hivecode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.527993 hivecode-0.0.0.8.21/src/hivecore/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivecore/__init__.py
+-rw-rw-rw-   0        0        0     1330 2023-05-08 01:20:28.000000 hivecode-0.0.0.8.21/src/hivecore/constant.py
+-rw-rw-rw-   0        0        0     9402 2023-07-15 21:48:03.000000 hivecode-0.0.0.8.21/src/hivecore/decorator.py
+-rw-rw-rw-   0        0        0     2744 2023-04-25 03:07:04.000000 hivecode-0.0.0.8.21/src/hivecore/eda.py
+-rw-rw-rw-   0        0        0     7676 2023-07-26 05:32:41.000000 hivecode-0.0.0.8.21/src/hivecore/functions.py
+-rw-rw-rw-   0        0        0    32180 2023-07-26 05:19:59.000000 hivecode-0.0.0.8.21/src/hivecore/patterns.py
+-rw-rw-rw-   0        0        0    28728 2023-07-20 03:05:40.000000 hivecode-0.0.0.8.21/src/hivecore/preprocess.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivecore/py.typed
+-rw-rw-rw-   0        0        0     6276 2023-04-25 03:07:19.000000 hivecode-0.0.0.8.21/src/hivecore/visual.py
+drwxrwxrwx   0        0        0        0 2023-07-26 06:37:27.535557 hivecode-0.0.0.8.21/src/hivesignal/
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/__init__.py
+-rw-rw-rw-   0        0        0     1683 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/analysis.py
+-rw-rw-rw-   0        0        0      292 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/eda.py
+-rw-rw-rw-   0        0        0     2383 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/io.py
+-rw-rw-rw-   0        0        0        0 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/py.typed
+-rw-rw-rw-   0        0        0     2126 2023-02-12 17:44:54.000000 hivecode-0.0.0.8.21/src/hivesignal/transform.py
```

### Comparing `hivecode-0.0.0.8.20/PKG-INFO` & `hivecode-0.0.0.8.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.20
+Version: 0.0.0.8.21
 Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
```

### Comparing `hivecode-0.0.0.8.20/README.rst` & `hivecode-0.0.0.8.21/README.rst`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/pyproject.toml` & `hivecode-0.0.0.8.21/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "hivecode"
 description = "Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell."
-version = "0.0.0.8.20"
+version = "0.0.0.8.21"
 requires-python = ">=3.8.0"
 readme = "README.rst"
 authors = [
     {name = "Juan Manuel Mejía Botero", email="juanmam941025@gmail.com"},
     {name = "Sebastian López Valencia", email="sebaslv12@hotmail.com"}
 ]
```

### Comparing `hivecode-0.0.0.8.20/setup.cfg` & `hivecode-0.0.0.8.21/setup.cfg`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hiveadb/eda.py` & `hivecode-0.0.0.8.21/src/hiveadb/eda.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hiveadb/function.py` & `hivecode-0.0.0.8.21/src/hiveadb/function.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hiveadb/io.py` & `hivecode-0.0.0.8.21/src/hiveadb/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hivecode.egg-info/PKG-INFO` & `hivecode-0.0.0.8.21/src/hivecode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hivecode
-Version: 0.0.0.8.20
+Version: 0.0.0.8.21
 Summary: Hivecode is a series of libraries desgined to make programming less of an artisan task and more of an engineering task. It includes functions, decorators and multiple classes desgiined to make the implementation of development and analytical proyects more oriented to desigin and architecture and less of an implementation hell.
 Author: Juan Manuel Mejía Botero
 Author-email: Juan Manuel Mejía Botero <juanmam941025@gmail.com>, Sebastian López Valencia <sebaslv12@hotmail.com>
 Project-URL: Homepage, https://github.com/Juanmam/hivecode
 Project-URL: Documentation, https://hivecode.readthedocs.io/en/latest/
 Platform: unix
 Platform: linux
```

### Comparing `hivecode-0.0.0.8.20/src/hivecode.egg-info/SOURCES.txt` & `hivecode-0.0.0.8.21/src/hivecode.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 src/hiveadb/__init__.py
 src/hiveadb/eda.py
 src/hiveadb/function.py
+src/hiveadb/functions.py
 src/hiveadb/io.py
 src/hiveadb/py.typed
 src/hivecode.egg-info/PKG-INFO
 src/hivecode.egg-info/SOURCES.txt
 src/hivecode.egg-info/dependency_links.txt
 src/hivecode.egg-info/not-zip-safe
 src/hivecode.egg-info/requires.txt
```

### Comparing `hivecode-0.0.0.8.20/src/hivecore/constant.py` & `hivecode-0.0.0.8.21/src/hivecore/constant.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hivecore/decorator.py` & `hivecode-0.0.0.8.21/src/hivecore/decorator.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hivecore/eda.py` & `hivecode-0.0.0.8.21/src/hivecore/eda.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hivecore/functions.py` & `hivecode-0.0.0.8.21/src/hivecore/functions.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hivecore/patterns.py` & `hivecode-0.0.0.8.21/src/hivecore/patterns.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hivecore/preprocess.py` & `hivecode-0.0.0.8.21/src/hivecore/preprocess.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hivecore/visual.py` & `hivecode-0.0.0.8.21/src/hivecore/visual.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hivesignal/analysis.py` & `hivecode-0.0.0.8.21/src/hivesignal/analysis.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hivesignal/io.py` & `hivecode-0.0.0.8.21/src/hivesignal/io.py`

 * *Files identical despite different names*

### Comparing `hivecode-0.0.0.8.20/src/hivesignal/transform.py` & `hivecode-0.0.0.8.21/src/hivesignal/transform.py`

 * *Files identical despite different names*

