# Comparing `tmp/foundationdb-7.3.7.tar.gz` & `tmp/foundationdb-7.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/foundationdb-7.3.7.tar", last modified: Tue Jul 11 13:38:04 2023, max compression
+gzip compressed data, was "dist/foundationdb-7.3.8.tar", last modified: Wed Jul 26 02:37:09 2023, max compression
```

## Comparing `foundationdb-7.3.7.tar` & `foundationdb-7.3.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-07-11 13:38:04.000000 foundationdb-7.3.7/
-drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-07-11 13:38:04.000000 foundationdb-7.3.7/fdb/
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1913 2023-07-11 02:40:22.000000 foundationdb-7.3.7/fdb/subspace_impl.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    30888 2023-07-11 02:40:22.000000 foundationdb-7.3.7/fdb/six.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)       25 2023-07-11 02:14:46.000000 foundationdb-7.3.7/fdb/apiversion.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    21791 2023-07-11 02:40:22.000000 foundationdb-7.3.7/fdb/tuple.py
--rwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    26547 2023-07-11 02:40:22.000000 foundationdb-7.3.7/fdb/directory_impl.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     4811 2023-07-11 02:40:22.000000 foundationdb-7.3.7/fdb/__init__.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     5842 2023-07-11 02:40:22.000000 foundationdb-7.3.7/fdb/tenant_management.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     2814 2023-07-11 02:40:22.000000 foundationdb-7.3.7/fdb/locality.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    38989 2023-07-11 02:16:58.000000 foundationdb-7.3.7/fdb/fdboptions.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    66069 2023-07-11 02:40:22.000000 foundationdb-7.3.7/fdb/impl.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)      252 2023-07-11 02:40:22.000000 foundationdb-7.3.7/README.rst
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1434 2023-07-11 13:38:04.000000 foundationdb-7.3.7/PKG-INFO
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1416 2023-07-11 02:14:46.000000 foundationdb-7.3.7/setup.py
--rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    11665 2023-07-11 02:14:46.000000 foundationdb-7.3.7/LICENSE
+drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-07-26 02:37:09.000000 foundationdb-7.3.8/
+drwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)        0 2023-07-26 02:37:09.000000 foundationdb-7.3.8/fdb/
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1913 2023-07-26 01:15:23.000000 foundationdb-7.3.8/fdb/subspace_impl.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    30888 2023-07-26 01:15:23.000000 foundationdb-7.3.8/fdb/six.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)       25 2023-07-26 01:12:17.000000 foundationdb-7.3.8/fdb/apiversion.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    21791 2023-07-26 01:15:23.000000 foundationdb-7.3.8/fdb/tuple.py
+-rwxrwxr-x   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    26547 2023-07-26 01:15:23.000000 foundationdb-7.3.8/fdb/directory_impl.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     4811 2023-07-26 01:15:23.000000 foundationdb-7.3.8/fdb/__init__.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     5842 2023-07-26 01:15:23.000000 foundationdb-7.3.8/fdb/tenant_management.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     2814 2023-07-26 01:15:23.000000 foundationdb-7.3.8/fdb/locality.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    38989 2023-07-26 01:15:23.000000 foundationdb-7.3.8/fdb/fdboptions.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    66069 2023-07-26 01:15:23.000000 foundationdb-7.3.8/fdb/impl.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)      252 2023-07-26 01:15:23.000000 foundationdb-7.3.8/README.rst
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1434 2023-07-26 02:37:09.000000 foundationdb-7.3.8/PKG-INFO
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)     1416 2023-07-26 01:12:17.000000 foundationdb-7.3.8/setup.py
+-rw-rw-r--   0 foundationdb_ci  (1001) foundationdb_ci  (1001)    11665 2023-07-26 01:12:17.000000 foundationdb-7.3.8/LICENSE
```

### Comparing `foundationdb-7.3.7/fdb/subspace_impl.py` & `foundationdb-7.3.8/fdb/subspace_impl.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.7/fdb/six.py` & `foundationdb-7.3.8/fdb/six.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.7/fdb/tuple.py` & `foundationdb-7.3.8/fdb/tuple.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.7/fdb/directory_impl.py` & `foundationdb-7.3.8/fdb/directory_impl.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.7/fdb/__init__.py` & `foundationdb-7.3.8/fdb/__init__.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.7/fdb/tenant_management.py` & `foundationdb-7.3.8/fdb/tenant_management.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.7/fdb/locality.py` & `foundationdb-7.3.8/fdb/locality.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.7/fdb/fdboptions.py` & `foundationdb-7.3.8/fdb/fdboptions.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.7/fdb/impl.py` & `foundationdb-7.3.8/fdb/impl.py`

 * *Files identical despite different names*

### Comparing `foundationdb-7.3.7/PKG-INFO` & `foundationdb-7.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: foundationdb
-Version: 7.3.7
+Version: 7.3.8
 Summary: Python bindings for the FoundationDB database
 Home-page: https://www.foundationdb.org
 Author: FoundationDB
 Author-email: fdb-dist@apple.com
 License: UNKNOWN
 Description: Complete documentation of the FoundationDB Python API can be found at https://apple.github.io/foundationdb/api-python.html.
```

### Comparing `foundationdb-7.3.7/setup.py` & `foundationdb-7.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 try:
     with open("README.rst") as f:
         long_desc = f.read()
 except:
     long_desc = ""
 
 setup(name="foundationdb",
-      version="7.3.7",
+      version="7.3.8",
       author="FoundationDB",
       author_email="fdb-dist@apple.com",
       description="Python bindings for the FoundationDB database",
       url="https://www.foundationdb.org",
       packages=['fdb'],
       package_data={'fdb': ["fdb/*.py"]},
       long_description=long_desc,
```

### Comparing `foundationdb-7.3.7/LICENSE` & `foundationdb-7.3.8/LICENSE`

 * *Files identical despite different names*

