# Comparing `tmp/satosa_oidcop-3.0.0.tar.gz` & `tmp/satosa_oidcop-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satosa_oidcop-3.0.0.tar", last modified: Tue Jul 25 07:44:56 2023, max compression
+gzip compressed data, was "satosa_oidcop-3.0.1.tar", last modified: Wed Jul 26 11:44:28 2023, max compression
```

## Comparing `satosa_oidcop-3.0.0.tar` & `satosa_oidcop-3.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:56.059185 satosa_oidcop-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-25 07:44:56.059185 satosa_oidcop-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:56.059185 satosa_oidcop-3.0.0/satosa_oidcop/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:56.059185 satosa_oidcop-3.0.0/satosa_oidcop/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/core/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/core/claims.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/core/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:56.059185 satosa_oidcop-3.0.0/satosa_oidcop/core/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/core/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/core/storage/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/core/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/core/user_authn.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/core/user_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    32833 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/satosa_oidcop/idpy_oidcop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 07:44:56.059185 satosa_oidcop-3.0.0/satosa_oidcop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-07-25 07:44:55.000000 satosa_oidcop-3.0.0/satosa_oidcop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-25 07:44:56.000000 satosa_oidcop-3.0.0/satosa_oidcop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 07:44:55.000000 satosa_oidcop-3.0.0/satosa_oidcop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-25 07:44:55.000000 satosa_oidcop-3.0.0/satosa_oidcop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 07:44:55.000000 satosa_oidcop-3.0.0/satosa_oidcop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-25 07:44:56.059185 satosa_oidcop-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-25 07:44:21.000000 satosa_oidcop-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:44:28.811539 satosa_oidcop-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-26 11:44:28.811539 satosa_oidcop-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:44:28.807539 satosa_oidcop-3.0.1/satosa_oidcop/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:44:28.811539 satosa_oidcop-3.0.1/satosa_oidcop/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/core/claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/core/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:44:28.811539 satosa_oidcop-3.0.1/satosa_oidcop/core/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/core/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/core/storage/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/core/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/core/user_authn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/core/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32833 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/satosa_oidcop/idpy_oidcop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:44:28.811539 satosa_oidcop-3.0.1/satosa_oidcop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-07-26 11:44:28.000000 satosa_oidcop-3.0.1/satosa_oidcop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-26 11:44:28.000000 satosa_oidcop-3.0.1/satosa_oidcop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:44:28.000000 satosa_oidcop-3.0.1/satosa_oidcop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 11:44:28.000000 satosa_oidcop-3.0.1/satosa_oidcop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-26 11:44:28.000000 satosa_oidcop-3.0.1/satosa_oidcop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-26 11:44:28.811539 satosa_oidcop-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-26 11:43:52.000000 satosa_oidcop-3.0.1/setup.py
```

### Comparing `satosa_oidcop-3.0.0/LICENSE` & `satosa_oidcop-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-3.0.0/PKG-INFO` & `satosa_oidcop-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: satosa_oidcop
-Version: 3.0.0
+Version: 3.0.1
 Summary: SATOSA Frontend based on idetity python oidcop
 Home-page: https://github.com/UniversitaDellaCalabria/satosa-oidcop
 Author: Giuseppe De Marco
 Author-email: giuseppe.demarco@unical.it
 License: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SATOSA oidcop frontend
```

### Comparing `satosa_oidcop-3.0.0/README.md` & `satosa_oidcop-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-3.0.0/satosa_oidcop/core/application.py` & `satosa_oidcop-3.0.1/satosa_oidcop/core/application.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-3.0.0/satosa_oidcop/core/claims.py` & `satosa_oidcop-3.0.1/satosa_oidcop/core/claims.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-3.0.0/satosa_oidcop/core/storage/base.py` & `satosa_oidcop-3.0.1/satosa_oidcop/core/storage/base.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-3.0.0/satosa_oidcop/core/storage/mongo.py` & `satosa_oidcop-3.0.1/satosa_oidcop/core/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-3.0.0/satosa_oidcop/core/user_authn.py` & `satosa_oidcop-3.0.1/satosa_oidcop/core/user_authn.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-3.0.0/satosa_oidcop/core/user_info.py` & `satosa_oidcop-3.0.1/satosa_oidcop/core/user_info.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-3.0.0/satosa_oidcop/idpy_oidcop.py` & `satosa_oidcop-3.0.1/satosa_oidcop/idpy_oidcop.py`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-3.0.0/satosa_oidcop.egg-info/PKG-INFO` & `satosa_oidcop-3.0.1/satosa_oidcop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: satosa-oidcop
-Version: 3.0.0
+Version: 3.0.1
 Summary: SATOSA Frontend based on idetity python oidcop
 Home-page: https://github.com/UniversitaDellaCalabria/satosa-oidcop
 Author: Giuseppe De Marco
 Author-email: giuseppe.demarco@unical.it
 License: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # SATOSA oidcop frontend
```

### Comparing `satosa_oidcop-3.0.0/satosa_oidcop.egg-info/SOURCES.txt` & `satosa_oidcop-3.0.1/satosa_oidcop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satosa_oidcop-3.0.0/setup.py` & `satosa_oidcop-3.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     long_description=readme(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     url="https://github.com/UniversitaDellaCalabria/satosa-oidcop",
     author="Giuseppe De Marco",
     author_email="giuseppe.demarco@unical.it",
```

