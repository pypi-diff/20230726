# Comparing `tmp/saturn-python-1.3.tar.gz` & `tmp/saturn-python-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saturn-python-1.3.tar", last modified: Tue Jul 25 14:10:43 2023, max compression
+gzip compressed data, was "dist/saturn-python-1.4.tar", last modified: Wed Jul 26 14:57:30 2023, max compression
```

## Comparing `saturn-python-1.3.tar` & `saturn-python-1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:43.990210 saturn-python-1.3/
--rw-rw-rw-   0        0        0     1640 2023-07-25 14:10:43.989120 saturn-python-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1236 2023-07-25 14:09:17.000000 saturn-python-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:43.972173 saturn-python-1.3/saturn/
--rw-rw-rw-   0        0        0     1098 2023-07-25 13:54:44.000000 saturn-python-1.3/saturn/__init__.py
--rw-rw-rw-   0        0        0      328 2023-07-25 13:54:44.000000 saturn-python-1.3/saturn/scope.py
--rw-rw-rw-   0        0        0     3414 2023-07-25 14:02:08.000000 saturn-python-1.3/saturn/terminal.py
--rw-rw-rw-   0        0        0       20 2023-07-25 14:09:11.000000 saturn-python-1.3/saturn/version.py
-drwxrwxrwx   0        0        0        0 2023-07-25 14:10:43.988111 saturn-python-1.3/saturn_python.egg-info/
--rw-rw-rw-   0        0        0     1640 2023-07-25 14:10:43.000000 saturn-python-1.3/saturn_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-25 14:10:43.000000 saturn-python-1.3/saturn_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 14:10:43.000000 saturn-python-1.3/saturn_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-07-25 14:10:43.000000 saturn-python-1.3/saturn_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 14:06:08.000000 saturn-python-1.3/saturn_python.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-07-25 14:10:43.000000 saturn-python-1.3/saturn_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 14:10:43.990210 saturn-python-1.3/setup.cfg
--rw-rw-rw-   0        0        0      785 2023-07-25 14:10:29.000000 saturn-python-1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:57:30.000000 saturn-python-1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-26 14:57:30.000000 saturn-python-1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-26 14:57:27.000000 saturn-python-1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:57:30.000000 saturn-python-1.4/saturn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-26 14:57:27.000000 saturn-python-1.4/saturn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-26 14:57:27.000000 saturn-python-1.4/saturn/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-26 14:57:27.000000 saturn-python-1.4/saturn/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 14:57:27.000000 saturn-python-1.4/saturn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:57:30.000000 saturn-python-1.4/saturn_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-07-26 14:57:29.000000 saturn-python-1.4/saturn_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-26 14:57:30.000000 saturn-python-1.4/saturn_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:57:29.000000 saturn-python-1.4/saturn_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-26 14:57:29.000000 saturn-python-1.4/saturn_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:57:29.000000 saturn-python-1.4/saturn_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 14:57:29.000000 saturn-python-1.4/saturn_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:57:30.000000 saturn-python-1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-26 14:57:27.000000 saturn-python-1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `saturn-python-1.3/README.md` & `saturn-python-1.4/README.md`

 * *Files identical despite different names*

### Comparing `saturn-python-1.3/saturn/__init__.py` & `saturn-python-1.4/saturn/__init__.py`

 * *Files identical despite different names*

### Comparing `saturn-python-1.3/saturn/terminal.py` & `saturn-python-1.4/saturn/terminal.py`

 * *Files identical despite different names*

### Comparing `saturn-python-1.3/setup.py` & `saturn-python-1.4/setup.py`

 * *Files identical despite different names*

