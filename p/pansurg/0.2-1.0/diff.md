# Comparing `tmp/pansurg-0.2.tar.gz` & `tmp/pansurg-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pansurg-0.2.tar", last modified: Tue May  5 10:43:37 2020, max compression
+gzip compressed data, was "pansurg-1.0.tar", last modified: Wed Jul 26 14:48:16 2023, max compression
```

## Comparing `pansurg-0.2.tar` & `pansurg-1.0.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 archives   (501) staff       (20)        0 2020-05-05 10:43:37.000000 pansurg-0.2/
--rw-r--r--   0 archives   (501) staff       (20)     2628 2020-05-05 10:43:37.000000 pansurg-0.2/PKG-INFO
-drwxr-xr-x   0 archives   (501) staff       (20)        0 2020-05-05 10:43:37.000000 pansurg-0.2/tests/
-drwxr-xr-x   0 archives   (501) staff       (20)        0 2020-05-05 10:43:37.000000 pansurg-0.2/tests/papers/
--rw-r--r--   0 archives   (501) staff       (20)        0 2020-05-03 16:01:50.000000 pansurg-0.2/tests/papers/__init__.py
--rw-r--r--   0 archives   (501) staff       (20)      746 2020-05-04 15:55:53.000000 pansurg-0.2/tests/papers/test_data_update.py
--rw-r--r--   0 archives   (501) staff       (20)     2436 2020-05-05 10:40:53.000000 pansurg-0.2/tests/papers/test_papers.py
--rw-r--r--   0 archives   (501) staff       (20)        0 2020-05-03 16:00:01.000000 pansurg-0.2/tests/__init__.py
-drwxr-xr-x   0 archives   (501) staff       (20)        0 2020-05-05 10:43:37.000000 pansurg-0.2/pansurg/
-drwxr-xr-x   0 archives   (501) staff       (20)        0 2020-05-05 10:43:37.000000 pansurg-0.2/pansurg/papers/
--rw-r--r--   0 archives   (501) staff       (20)     1775 2020-05-05 10:40:53.000000 pansurg-0.2/pansurg/papers/papers.py
--rw-r--r--   0 archives   (501) staff       (20)        0 2020-05-03 16:01:25.000000 pansurg-0.2/pansurg/papers/__init__.py
--rw-r--r--   0 archives   (501) staff       (20)      998 2020-05-04 22:18:56.000000 pansurg-0.2/pansurg/papers/data_update.py
--rw-r--r--   0 archives   (501) staff       (20)       34 2020-05-03 16:20:16.000000 pansurg-0.2/pansurg/__init__.py
--rw-r--r--   0 archives   (501) staff       (20)     1610 2020-05-05 10:40:53.000000 pansurg-0.2/README.md
--rw-r--r--   0 archives   (501) staff       (20)      857 2020-05-05 10:40:53.000000 pansurg-0.2/setup.py
--rw-r--r--   0 archives   (501) staff       (20)       38 2020-05-05 10:43:37.000000 pansurg-0.2/setup.cfg
-drwxr-xr-x   0 archives   (501) staff       (20)        0 2020-05-05 10:43:37.000000 pansurg-0.2/pansurg.egg-info/
--rw-r--r--   0 archives   (501) staff       (20)     2628 2020-05-05 10:43:37.000000 pansurg-0.2/pansurg.egg-info/PKG-INFO
--rw-r--r--   0 archives   (501) staff       (20)        1 2020-05-03 19:45:11.000000 pansurg-0.2/pansurg.egg-info/not-zip-safe
--rw-r--r--   0 archives   (501) staff       (20)      378 2020-05-05 10:43:37.000000 pansurg-0.2/pansurg.egg-info/SOURCES.txt
--rw-r--r--   0 archives   (501) staff       (20)       14 2020-05-05 10:43:37.000000 pansurg-0.2/pansurg.egg-info/top_level.txt
--rw-r--r--   0 archives   (501) staff       (20)        1 2020-05-05 10:43:37.000000 pansurg-0.2/pansurg.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:48:16.501648 pansurg-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-26 14:47:52.000000 pansurg-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 14:47:52.000000 pansurg-1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 14:48:16.501648 pansurg-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-26 14:47:52.000000 pansurg-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:48:16.501648 pansurg-1.0/pansurg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-26 14:48:16.000000 pansurg-1.0/pansurg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-26 14:48:16.000000 pansurg-1.0/pansurg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:48:16.000000 pansurg-1.0/pansurg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:48:16.000000 pansurg-1.0/pansurg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-26 14:48:16.000000 pansurg-1.0/pansurg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-26 14:47:52.000000 pansurg-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:48:16.501648 pansurg-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-26 14:47:52.000000 pansurg-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:48:16.501648 pansurg-1.0/surrealdb/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/connection_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:48:16.501648 pansurg-1.0/surrealdb/execution_mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/execution_mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/execution_mixins/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/execution_mixins/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/execution_mixins/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/execution_mixins/set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/execution_mixins/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:48:16.501648 pansurg-1.0/surrealdb/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:47:52.000000 pansurg-1.0/surrealdb/models/another_file.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

