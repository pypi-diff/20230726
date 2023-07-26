# Comparing `tmp/multilogue-0.0.1.tar.gz` & `tmp/multilogue-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multilogue-0.0.1.tar", last modified: Sun Jul  2 15:52:42 2023, max compression
+gzip compressed data, was "multilogue-0.0.2.tar", last modified: Wed Jul 26 20:40:25 2023, max compression
```

## Comparing `multilogue-0.0.1.tar` & `multilogue-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-02 15:52:42.199039 multilogue-0.0.1/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.1/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      555 2023-07-02 15:52:42.195039 multilogue-0.0.1/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       55 2023-07-02 15:37:04.000000 multilogue-0.0.1/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      581 2023-07-02 15:47:42.000000 multilogue-0.0.1/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-02 15:52:42.199039 multilogue-0.0.1/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-02 15:52:42.195039 multilogue-0.0.1/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-02 15:52:42.195039 multilogue-0.0.1/src/multilogue/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       33 2023-07-02 15:44:41.000000 multilogue-0.0.1/src/multilogue/__init__.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-02 15:52:42.195039 multilogue-0.0.1/src/multilogue.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      555 2023-07-02 15:52:42.000000 multilogue-0.0.1/src/multilogue.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      211 2023-07-02 15:52:42.000000 multilogue-0.0.1/src/multilogue.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-02 15:52:42.000000 multilogue-0.0.1/src/multilogue.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-07-02 15:52:42.000000 multilogue-0.0.1/src/multilogue.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 20:40:25.823869 multilogue-0.0.2/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.2/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      555 2023-07-26 20:40:25.823869 multilogue-0.0.2/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       55 2023-07-02 15:37:04.000000 multilogue-0.0.2/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      581 2023-07-26 20:35:34.000000 multilogue-0.0.2/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-07-26 20:40:25.823869 multilogue-0.0.2/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 20:40:25.819869 multilogue-0.0.2/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 20:40:25.819869 multilogue-0.0.2/src/multilogue/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       91 2023-07-26 20:35:34.000000 multilogue-0.0.2/src/multilogue/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1159 2023-07-26 20:39:15.000000 multilogue-0.0.2/src/multilogue/entities.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-07-26 20:40:25.819869 multilogue-0.0.2/src/multilogue.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      555 2023-07-26 20:40:25.000000 multilogue-0.0.2/src/multilogue.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      238 2023-07-26 20:40:25.000000 multilogue-0.0.2/src/multilogue.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-07-26 20:40:25.000000 multilogue-0.0.2/src/multilogue.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-07-26 20:40:25.000000 multilogue-0.0.2/src/multilogue.egg-info/top_level.txt
```

### Comparing `multilogue-0.0.1/LICENSE` & `multilogue-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.1/PKG-INFO` & `multilogue-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilogue
-Version: 0.0.1
+Version: 0.0.2
 Summary: Multilogue
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/multilogue
 Project-URL: Bug Tracker, https://github.com/multilogue/multilogue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `multilogue-0.0.1/pyproject.toml` & `multilogue-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "multilogue"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
 description = "Multilogue"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
```

### Comparing `multilogue-0.0.1/src/multilogue.egg-info/PKG-INFO` & `multilogue-0.0.2/src/multilogue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multilogue
-Version: 0.0.1
+Version: 0.0.2
 Summary: Multilogue
 Author-email: Alexander Fedotov <alex.fedotov@aol.com>
 Project-URL: Homepage, https://github.com/multilogue/multilogue
 Project-URL: Bug Tracker, https://github.com/multilogue/multilogue/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

