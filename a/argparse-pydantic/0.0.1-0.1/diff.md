# Comparing `tmp/argparse_pydantic-0.0.1.tar.gz` & `tmp/argparse_pydantic-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparse_pydantic-0.0.1.tar", last modified: Thu Jul 20 13:54:10 2023, max compression
+gzip compressed data, was "argparse_pydantic-0.1.tar", last modified: Wed Jul 26 09:16:33 2023, max compression
```

## Comparing `argparse_pydantic-0.0.1.tar` & `argparse_pydantic-0.1.tar`

### file list

```diff
@@ -1,17 +1,28 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-20 13:54:10.715124 argparse_pydantic-0.0.1/
--rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-07-20 13:37:56.000000 argparse_pydantic-0.0.1/LICENSE
--rw-rw-r--   0 aya       (1000) aya       (1000)      828 2023-07-20 13:54:10.715124 argparse_pydantic-0.0.1/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      325 2023-07-20 13:45:40.000000 argparse_pydantic-0.0.1/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      673 2023-07-20 13:54:10.715124 argparse_pydantic-0.0.1/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-07-20 13:39:29.000000 argparse_pydantic-0.0.1/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-20 13:54:10.711124 argparse_pydantic-0.0.1/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-20 13:54:10.711124 argparse_pydantic-0.0.1/src/argparse_pydantic/
--rw-rw-r--   0 aya       (1000) aya       (1000)        0 2023-07-20 13:44:17.000000 argparse_pydantic-0.0.1/src/argparse_pydantic/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)        0 2023-07-20 13:51:58.000000 argparse_pydantic-0.0.1/src/argparse_pydantic/core.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       21 2023-07-20 13:52:50.000000 argparse_pydantic-0.0.1/src/argparse_pydantic/version.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-20 13:54:10.715124 argparse_pydantic-0.0.1/src/argparse_pydantic.egg-info/
--rw-rw-r--   0 aya       (1000) aya       (1000)      828 2023-07-20 13:54:10.000000 argparse_pydantic-0.0.1/src/argparse_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)      357 2023-07-20 13:54:10.000000 argparse_pydantic-0.0.1/src/argparse_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-07-20 13:54:10.000000 argparse_pydantic-0.0.1/src/argparse_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       61 2023-07-20 13:54:10.000000 argparse_pydantic-0.0.1/src/argparse_pydantic.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       18 2023-07-20 13:54:10.000000 argparse_pydantic-0.0.1/src/argparse_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-26 09:16:33.606055 argparse_pydantic-0.1/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2023-07-20 13:37:56.000000 argparse_pydantic-0.1/LICENSE
+-rw-rw-r--   0 aya       (1000) aya       (1000)      826 2023-07-26 09:16:33.606055 argparse_pydantic-0.1/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      325 2023-07-20 13:45:40.000000 argparse_pydantic-0.1/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      673 2023-07-26 09:16:33.606055 argparse_pydantic-0.1/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      597 2023-07-20 13:39:29.000000 argparse_pydantic-0.1/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-26 09:16:33.602055 argparse_pydantic-0.1/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-26 09:16:33.602055 argparse_pydantic-0.1/src/argparse_pydantic/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      139 2023-07-21 12:12:36.000000 argparse_pydantic-0.1/src/argparse_pydantic/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5110 2023-07-26 08:49:40.000000 argparse_pydantic-0.1/src/argparse_pydantic/core.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1284 2023-07-21 09:37:02.000000 argparse_pydantic-0.1/src/argparse_pydantic/helpers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3240 2023-07-21 09:37:02.000000 argparse_pydantic-0.1/src/argparse_pydantic/test_tools.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       20 2023-07-26 09:13:28.000000 argparse_pydantic-0.1/src/argparse_pydantic/version.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-26 09:16:33.606055 argparse_pydantic-0.1/src/argparse_pydantic.egg-info/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      826 2023-07-26 09:16:33.000000 argparse_pydantic-0.1/src/argparse_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)      673 2023-07-26 09:16:33.000000 argparse_pydantic-0.1/src/argparse_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-07-26 09:16:33.000000 argparse_pydantic-0.1/src/argparse_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       61 2023-07-26 09:16:33.000000 argparse_pydantic-0.1/src/argparse_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       18 2023-07-26 09:16:33.000000 argparse_pydantic-0.1/src/argparse_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-26 09:16:33.606055 argparse_pydantic-0.1/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2469 2023-07-25 09:08:03.000000 argparse_pydantic-0.1/tests/test_add_argument_action.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1956 2023-07-24 13:37:01.000000 argparse_pydantic-0.1/tests/test_add_argument_flag.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4895 2023-07-25 12:20:22.000000 argparse_pydantic-0.1/tests/test_add_argument_json_schema_extra.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1276 2023-07-21 13:39:35.000000 argparse_pydantic-0.1/tests/test_add_argument_simple.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      980 2023-07-25 09:20:47.000000 argparse_pydantic-0.1/tests/test_core_base.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1199 2023-07-21 09:37:02.000000 argparse_pydantic-0.1/tests/test_create_parser.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      521 2023-07-24 13:38:31.000000 argparse_pydantic-0.1/tests/test_parse_args.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3778 2023-07-21 09:37:02.000000 argparse_pydantic-0.1/tests/test_test_tools.py
```

### Comparing `argparse_pydantic-0.0.1/LICENSE` & `argparse_pydantic-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.0.1/PKG-INFO` & `argparse_pydantic-0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse_pydantic
-Version: 0.0.1
+Version: 0.1
 Summary: argparse config with pydantic model.
 Home-page: https://github.com/ayasyrev/argparse_pydantic
 Author: Yasyrev Andrei
 Author-email: a.yasyrev@gmail.com
 License: apache2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `argparse_pydantic-0.0.1/setup.cfg` & `argparse_pydantic-0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.0.1/setup.py` & `argparse_pydantic-0.1/setup.py`

 * *Files identical despite different names*

### Comparing `argparse_pydantic-0.0.1/src/argparse_pydantic.egg-info/PKG-INFO` & `argparse_pydantic-0.1/src/argparse_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argparse-pydantic
-Version: 0.0.1
+Version: 0.1
 Summary: argparse config with pydantic model.
 Home-page: https://github.com/ayasyrev/argparse_pydantic
 Author: Yasyrev Andrei
 Author-email: a.yasyrev@gmail.com
 License: apache2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

