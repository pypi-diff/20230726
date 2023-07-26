# Comparing `tmp/stdflow-0.0.4.tar.gz` & `tmp/stdflow-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdflow-0.0.4.tar", last modified: Wed Jul 26 01:54:26 2023, max compression
+gzip compressed data, was "stdflow-0.0.5.tar", last modified: Wed Jul 26 02:02:42 2023, max compression
```

## Comparing `stdflow-0.0.4.tar` & `stdflow-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,12 @@
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-26 01:54:26.487314 stdflow-0.0.4/
--rw-r--r--   0 cyprien    (501) staff       (20)     1071 2023-07-24 15:57:38.000000 stdflow-0.0.4/LICENSE
--rw-r--r--   0 cyprien    (501) staff       (20)     6493 2023-07-26 01:54:26.487192 stdflow-0.0.4/PKG-INFO
--rw-r--r--   0 cyprien    (501) staff       (20)     5931 2023-07-24 15:39:08.000000 stdflow-0.0.4/README.md
--rw-r--r--   0 cyprien    (501) staff       (20)      930 2023-07-26 01:34:31.000000 stdflow-0.0.4/pyproject.toml
--rw-r--r--   0 cyprien    (501) staff       (20)       38 2023-07-26 01:54:26.487362 stdflow-0.0.4/setup.cfg
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-26 01:54:26.485292 stdflow-0.0.4/stdflow/
--rw-r--r--   0 cyprien    (501) staff       (20)     5530 2023-07-26 01:34:31.000000 stdflow-0.0.4/stdflow/__init__.py
--rw-r--r--   0 cyprien    (501) staff       (20)      135 2023-07-25 05:16:26.000000 stdflow-0.0.4/stdflow/config.py
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-26 01:54:26.486613 stdflow-0.0.4/stdflow/loaders/
--rw-r--r--   0 cyprien    (501) staff       (20)      339 2023-07-24 02:46:01.000000 stdflow-0.0.4/stdflow/loaders/__init__.py
--rw-r--r--   0 cyprien    (501) staff       (20)     1134 2023-07-25 03:46:32.000000 stdflow-0.0.4/stdflow/loaders/csv.py
--rw-r--r--   0 cyprien    (501) staff       (20)     3389 2023-07-26 01:26:13.000000 stdflow-0.0.4/stdflow/metadata.py
--rw-r--r--   0 cyprien    (501) staff       (20)     6483 2023-07-25 07:16:02.000000 stdflow-0.0.4/stdflow/path.py
--rw-r--r--   0 cyprien    (501) staff       (20)    15035 2023-07-26 01:33:31.000000 stdflow-0.0.4/stdflow/step.py
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-26 01:54:26.486866 stdflow-0.0.4/stdflow/utils/
--rw-r--r--   0 cyprien    (501) staff       (20)     8112 2023-07-26 01:23:14.000000 stdflow-0.0.4/stdflow/utils/__init__.py
-drwxr-xr-x   0 cyprien    (501) staff       (20)        0 2023-07-26 01:54:26.486074 stdflow-0.0.4/stdflow.egg-info/
--rw-r--r--   0 cyprien    (501) staff       (20)     6493 2023-07-26 01:54:26.000000 stdflow-0.0.4/stdflow.egg-info/PKG-INFO
--rw-r--r--   0 cyprien    (501) staff       (20)      353 2023-07-26 01:54:26.000000 stdflow-0.0.4/stdflow.egg-info/SOURCES.txt
--rw-r--r--   0 cyprien    (501) staff       (20)        1 2023-07-26 01:54:26.000000 stdflow-0.0.4/stdflow.egg-info/dependency_links.txt
--rw-r--r--   0 cyprien    (501) staff       (20)       83 2023-07-26 01:54:26.000000 stdflow-0.0.4/stdflow.egg-info/requires.txt
--rw-r--r--   0 cyprien    (501) staff       (20)        8 2023-07-26 01:54:26.000000 stdflow-0.0.4/stdflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:02:42.891794 stdflow-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-26 02:02:26.000000 stdflow-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-26 02:02:42.891794 stdflow-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-26 02:02:26.000000 stdflow-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-26 02:02:26.000000 stdflow-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 02:02:42.891794 stdflow-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 02:02:42.891794 stdflow-0.0.5/stdflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-07-26 02:02:42.000000 stdflow-0.0.5/stdflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-26 02:02:42.000000 stdflow-0.0.5/stdflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 02:02:42.000000 stdflow-0.0.5/stdflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-26 02:02:42.000000 stdflow-0.0.5/stdflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 02:02:42.000000 stdflow-0.0.5/stdflow.egg-info/top_level.txt
```

### Comparing `stdflow-0.0.4/LICENSE` & `stdflow-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.4/PKG-INFO` & `stdflow-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdflow
-Version: 0.0.4
+Version: 0.0.5
 Summary: [alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output.
 Author-email: Cyprien Ricque <ricque.cyprien@gmail.com>
 Keywords: data science,data,flow,data flow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `stdflow-0.0.4/README.md` & `stdflow-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `stdflow-0.0.4/pyproject.toml` & `stdflow-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ["stdflow"]
 
 [project]
 name = "stdflow"
-version = "0.0.4"
+version = "0.0.5"
 description = "[alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output."
 readme = "README.md"
 authors = [
     { name = "Cyprien Ricque", email = "ricque.cyprien@gmail.com" },
 ]
 keywords = ["data science", "data", "flow", "data flow"]
 requires-python = ">=3.9"
```

### Comparing `stdflow-0.0.4/stdflow.egg-info/PKG-INFO` & `stdflow-0.0.5/stdflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdflow
-Version: 0.0.4
+Version: 0.0.5
 Summary: [alpha] A package that transform your notebooks and python files into pipeline steps by standardizing the data input / output.
 Author-email: Cyprien Ricque <ricque.cyprien@gmail.com>
 Keywords: data science,data,flow,data flow
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
```

