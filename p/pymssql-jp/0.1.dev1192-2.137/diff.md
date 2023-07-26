# Comparing `tmp/pymssql-jp-2.137.tar.gz` & `tmp/pymssql-jp-2.137b.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Jul 26 13:18:05 2023, from Unix
+gzip compressed data, last modified: Wed Jul 26 13:19:36 2023, from Unix
```

## Comparing `pymssql-jp-2.137.tar` & `pymssql-jp-2.137b.tar`

### file list

```diff
@@ -1,11 +1,11 @@
 -rwxr-xr-x   0 teserak    (501) staff       (20)      224 2023-07-26 13:10:47.000000 ._pymssql-jp-2.137
 drwxr-xr-x   0 teserak    (501) staff       (20)        0 2023-07-26 13:10:47.753649 pymssql-jp-2.137/
--rw-r--r--   0 teserak    (501) staff       (20)      367 2023-07-26 13:17:44.000000 pymssql-jp-2.137/._PKG-INFO
--rw-r--r--   0 teserak    (501) staff       (20)     4551 2023-07-26 13:17:44.587243 pymssql-jp-2.137/PKG-INFO
+-rw-r--r--   0 teserak    (501) staff       (20)      367 2023-07-26 13:19:13.000000 pymssql-jp-2.137/._PKG-INFO
+-rw-r--r--   0 teserak    (501) staff       (20)     4545 2023-07-26 13:19:13.823443 pymssql-jp-2.137/PKG-INFO
 -rw-r--r--   0 teserak    (501) staff       (20)      224 2023-07-26 12:44:41.000000 pymssql-jp-2.137/._pytest.ini
 -rw-r--r--   0 teserak    (501) staff       (20)      447 2023-07-26 12:44:41.000000 pymssql-jp-2.137/pytest.ini
 -rw-r--r--   0 teserak    (501) staff       (20)      224 2023-07-26 12:44:41.000000 pymssql-jp-2.137/._LICENSE
 -rw-r--r--   0 teserak    (501) staff       (20)    26436 2023-07-26 12:44:41.000000 pymssql-jp-2.137/LICENSE
 -rw-r--r--   0 teserak    (501) staff       (20)      224 2023-07-26 12:44:41.000000 pymssql-jp-2.137/._Dockerfile
 -rw-r--r--   0 teserak    (501) staff       (20)      964 2023-07-26 12:44:41.000000 pymssql-jp-2.137/Dockerfile
 -rw-r--r--   0 teserak    (501) staff       (20)      224 2023-07-26 12:45:15.000000 pymssql-jp-2.137/._pyproject.toml
```

### pymssql-jp-2.137/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymssql-jp
-Version: 0.1.dev1192
+Version: 2.137
 Summary: DB-API interface to Microsoft SQL Server for Python. (new Cython-based version)
 Author: Damien Churchill
 Author-email: damoxc@gmail.com
 Maintainer: Mikhail Terekhov
 Maintainer-email: termim@gmail.com
 License: LGPL
 Project-URL: Documentation, http://pymssql.readthedocs.io
```

