# Comparing `tmp/gauth_python-0.1.0.tar.gz` & `tmp/gauth_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gauth_python-0.1.0.tar", last modified: Wed Jul 26 08:44:19 2023, max compression
+gzip compressed data, was "gauth_python-0.1.1.tar", last modified: Wed Jul 26 08:47:02 2023, max compression
```

## Comparing `gauth_python-0.1.0.tar` & `gauth_python-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 08:44:19.415280 gauth_python-0.1.0/
--rw-r--r--   0 yohan      (501) staff       (20)     1061 2023-07-26 08:05:07.000000 gauth_python-0.1.0/LICENSE
--rw-r--r--   0 yohan      (501) staff       (20)      181 2023-07-26 08:44:19.415142 gauth_python-0.1.0/PKG-INFO
--rw-r--r--   0 yohan      (501) staff       (20)       23 2023-07-25 08:41:42.000000 gauth_python-0.1.0/README.md
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 08:44:19.414608 gauth_python-0.1.0/gauth_python.egg-info/
--rw-r--r--   0 yohan      (501) staff       (20)      181 2023-07-26 08:44:19.000000 gauth_python-0.1.0/gauth_python.egg-info/PKG-INFO
--rw-r--r--   0 yohan      (501) staff       (20)      240 2023-07-26 08:44:19.000000 gauth_python-0.1.0/gauth_python.egg-info/SOURCES.txt
--rw-r--r--   0 yohan      (501) staff       (20)        1 2023-07-26 08:44:19.000000 gauth_python-0.1.0/gauth_python.egg-info/dependency_links.txt
--rw-r--r--   0 yohan      (501) staff       (20)       21 2023-07-26 08:44:19.000000 gauth_python-0.1.0/gauth_python.egg-info/top_level.txt
-drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 08:44:19.414817 gauth_python-0.1.0/gauth_python_package/
--rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 10:32:26.000000 gauth_python-0.1.0/gauth_python_package/__init__.py
--rw-r--r--   0 yohan      (501) staff       (20)     1310 2023-07-26 08:30:17.000000 gauth_python-0.1.0/gauth_python_package/gauth_python.py
--rw-r--r--   0 yohan      (501) staff       (20)       38 2023-07-26 08:44:19.415326 gauth_python-0.1.0/setup.cfg
--rw-r--r--   0 yohan      (501) staff       (20)      363 2023-07-26 08:43:03.000000 gauth_python-0.1.0/setup.py
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 08:47:02.259791 gauth_python-0.1.1/
+-rw-r--r--   0 yohan      (501) staff       (20)     1061 2023-07-26 08:05:07.000000 gauth_python-0.1.1/LICENSE
+-rw-r--r--   0 yohan      (501) staff       (20)      190 2023-07-26 08:47:02.259648 gauth_python-0.1.1/PKG-INFO
+-rw-r--r--   0 yohan      (501) staff       (20)       23 2023-07-25 08:41:42.000000 gauth_python-0.1.1/README.md
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 08:47:02.258747 gauth_python-0.1.1/gauth_python.egg-info/
+-rw-r--r--   0 yohan      (501) staff       (20)      190 2023-07-26 08:47:02.000000 gauth_python-0.1.1/gauth_python.egg-info/PKG-INFO
+-rw-r--r--   0 yohan      (501) staff       (20)      240 2023-07-26 08:47:02.000000 gauth_python-0.1.1/gauth_python.egg-info/SOURCES.txt
+-rw-r--r--   0 yohan      (501) staff       (20)        1 2023-07-26 08:47:02.000000 gauth_python-0.1.1/gauth_python.egg-info/dependency_links.txt
+-rw-r--r--   0 yohan      (501) staff       (20)       21 2023-07-26 08:47:02.000000 gauth_python-0.1.1/gauth_python.egg-info/top_level.txt
+drwxr-xr-x   0 yohan      (501) staff       (20)        0 2023-07-26 08:47:02.259181 gauth_python-0.1.1/gauth_python_package/
+-rw-r--r--   0 yohan      (501) staff       (20)        0 2023-07-25 10:32:26.000000 gauth_python-0.1.1/gauth_python_package/__init__.py
+-rw-r--r--   0 yohan      (501) staff       (20)     1310 2023-07-26 08:30:17.000000 gauth_python-0.1.1/gauth_python_package/gauth_python.py
+-rw-r--r--   0 yohan      (501) staff       (20)       38 2023-07-26 08:47:02.259833 gauth_python-0.1.1/setup.cfg
+-rw-r--r--   0 yohan      (501) staff       (20)      372 2023-07-26 08:46:56.000000 gauth_python-0.1.1/setup.py
```

### Comparing `gauth_python-0.1.0/LICENSE` & `gauth_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gauth_python-0.1.0/gauth_python_package/gauth_python.py` & `gauth_python-0.1.1/gauth_python_package/gauth_python.py`

 * *Files identical despite different names*

