# Comparing `tmp/niltype-0.3.4.tar.gz` & `tmp/niltype-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niltype-0.3.4.tar", last modified: Thu Jun 22 15:26:25 2023, max compression
+gzip compressed data, was "niltype-1.0.0.tar", last modified: Wed Jul 26 15:55:34 2023, max compression
```

## Comparing `niltype-0.3.4.tar` & `niltype-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:26:25.801982 niltype-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 15:26:12.000000 niltype-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-22 15:26:25.801982 niltype-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 15:26:12.000000 niltype-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:26:25.801982 niltype-0.3.4/niltype/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 15:26:12.000000 niltype-0.3.4/niltype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 15:26:12.000000 niltype-0.3.4/niltype/_nilable.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 15:26:12.000000 niltype-0.3.4/niltype/_niltype.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 15:26:12.000000 niltype-0.3.4/niltype/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:26:12.000000 niltype-0.3.4/niltype/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:26:25.801982 niltype-0.3.4/niltype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-22 15:26:25.000000 niltype-0.3.4/niltype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-22 15:26:25.000000 niltype-0.3.4/niltype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:26:25.000000 niltype-0.3.4/niltype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 15:26:25.000000 niltype-0.3.4/niltype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-22 15:26:25.801982 niltype-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-22 15:26:12.000000 niltype-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:26:25.801982 niltype-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-22 15:26:12.000000 niltype-0.3.4/tests/test_niltype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:55:34.802885 niltype-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-26 15:55:24.000000 niltype-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-26 15:55:34.806885 niltype-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-26 15:55:24.000000 niltype-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:55:34.802885 niltype-1.0.0/niltype/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-26 15:55:24.000000 niltype-1.0.0/niltype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-26 15:55:24.000000 niltype-1.0.0/niltype/_nilable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-26 15:55:24.000000 niltype-1.0.0/niltype/_niltype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 15:55:24.000000 niltype-1.0.0/niltype/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:55:24.000000 niltype-1.0.0/niltype/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:55:34.802885 niltype-1.0.0/niltype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-26 15:55:34.000000 niltype-1.0.0/niltype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-26 15:55:34.000000 niltype-1.0.0/niltype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:55:34.000000 niltype-1.0.0/niltype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-26 15:55:34.000000 niltype-1.0.0/niltype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-26 15:55:34.806885 niltype-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-26 15:55:24.000000 niltype-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:55:34.802885 niltype-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-26 15:55:24.000000 niltype-1.0.0/tests/test_niltype.py
```

### Comparing `niltype-0.3.4/LICENSE` & `niltype-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `niltype-0.3.4/PKG-INFO` & `niltype-1.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niltype
-Version: 0.3.4
+Version: 1.0.0
 Summary: Like a None
 Home-page: https://github.com/tsv1/niltype
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `niltype-0.3.4/README.md` & `niltype-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `niltype-0.3.4/niltype/_niltype.py` & `niltype-1.0.0/niltype/_niltype.py`

 * *Files identical despite different names*

### Comparing `niltype-0.3.4/niltype.egg-info/PKG-INFO` & `niltype-1.0.0/niltype.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: niltype
-Version: 0.3.4
+Version: 1.0.0
 Summary: Like a None
 Home-page: https://github.com/tsv1/niltype
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `niltype-0.3.4/setup.cfg` & `niltype-1.0.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.4
+current_version = 1.0.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `niltype-0.3.4/setup.py` & `niltype-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="niltype",
-    version="0.3.4",
+    version="1.0.0",
     description="Like a None",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
     url="https://github.com/tsv1/niltype",
```

### Comparing `niltype-0.3.4/tests/test_niltype.py` & `niltype-1.0.0/tests/test_niltype.py`

 * *Files identical despite different names*

