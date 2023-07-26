# Comparing `tmp/openai_function-0.1.1.tar.gz` & `tmp/openai_function-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_function-0.1.1.tar", max compression
+gzip compressed data, was "openai_function-0.1.2.tar", max compression
```

## Comparing `openai_function-0.1.1.tar` & `openai_function-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-07-26 11:34:37.860827 openai_function-0.1.1/README.md
--rw-r--r--   0        0        0     3517 2023-07-26 17:12:21.525691 openai_function-0.1.1/openai_function/__init__.py
--rw-r--r--   0        0        0     2626 2023-07-26 15:12:49.735133 openai_function-0.1.1/openai_function/chat_completion.py
--rw-r--r--   0        0        0    12597 2023-07-26 17:06:59.504095 openai_function-0.1.1/openai_function/client.py
--rw-r--r--   0        0        0      463 2023-07-26 16:38:20.109822 openai_function-0.1.1/openai_function/embeddings.py
--rw-r--r--   0        0        0        0 2023-07-26 17:12:06.025143 openai_function-0.1.1/openai_function/faunadb/__init__.py
--rwxr-xr-x   0        0        0     7771 2023-07-26 16:40:14.681565 openai_function-0.1.1/openai_function/faunadb/errors.py
--rwxr-xr-x   0        0        0     5659 2023-07-26 16:40:14.681565 openai_function-0.1.1/openai_function/faunadb/objects.py
--rwxr-xr-x   0        0        0     1637 2023-07-26 16:40:14.681565 openai_function-0.1.1/openai_function/faunadb/page.py
--rwxr-xr-x   0        0        0    17374 2023-07-26 16:40:14.681565 openai_function-0.1.1/openai_function/faunadb/query.py
--rwxr-xr-x   0        0        0     6628 2023-07-26 16:41:01.737479 openai_function-0.1.1/openai_function/json.py
--rw-r--r--   0        0        0     2863 2023-07-26 14:58:26.964143 openai_function-0.1.1/openai_function/logging.py
--rwxr-xr-x   0        0        0    11253 2023-07-26 17:12:04.473088 openai_function-0.1.1/openai_function/odm.py
--rw-r--r--   0        0        0     3868 2023-07-26 17:06:58.160026 openai_function-0.1.1/openai_function/openai_functions.py
--rw-r--r--   0        0        0     1052 2023-07-26 17:06:56.179925 openai_function-0.1.1/openai_function/typedefs.py
--rw-r--r--   0        0        0     2450 2023-07-26 17:12:57.330924 openai_function-0.1.1/openai_function/vectorstore.py
--rw-r--r--   0        0        0      444 2023-07-26 17:21:50.545526 openai_function-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 openai_function-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-26 11:34:37.860827 openai_function-0.1.2/README.md
+-rw-r--r--   0        0        0     3517 2023-07-26 17:12:21.525691 openai_function-0.1.2/openai_function/__init__.py
+-rw-r--r--   0        0        0     2626 2023-07-26 15:12:49.735133 openai_function-0.1.2/openai_function/chat_completion.py
+-rw-r--r--   0        0        0    12597 2023-07-26 17:06:59.504095 openai_function-0.1.2/openai_function/client.py
+-rw-r--r--   0        0        0      463 2023-07-26 16:38:20.109822 openai_function-0.1.2/openai_function/embeddings.py
+-rw-r--r--   0        0        0        0 2023-07-26 17:12:06.025143 openai_function-0.1.2/openai_function/faunadb/__init__.py
+-rwxr-xr-x   0        0        0     7771 2023-07-26 16:40:14.681565 openai_function-0.1.2/openai_function/faunadb/errors.py
+-rwxr-xr-x   0        0        0     5659 2023-07-26 16:40:14.681565 openai_function-0.1.2/openai_function/faunadb/objects.py
+-rwxr-xr-x   0        0        0     1637 2023-07-26 16:40:14.681565 openai_function-0.1.2/openai_function/faunadb/page.py
+-rwxr-xr-x   0        0        0    17374 2023-07-26 16:40:14.681565 openai_function-0.1.2/openai_function/faunadb/query.py
+-rwxr-xr-x   0        0        0     6628 2023-07-26 16:41:01.737479 openai_function-0.1.2/openai_function/json.py
+-rw-r--r--   0        0        0     2863 2023-07-26 14:58:26.964143 openai_function-0.1.2/openai_function/logging.py
+-rwxr-xr-x   0        0        0    11253 2023-07-26 17:12:04.473088 openai_function-0.1.2/openai_function/odm.py
+-rw-r--r--   0        0        0     3868 2023-07-26 17:06:58.160026 openai_function-0.1.2/openai_function/openai_functions.py
+-rw-r--r--   0        0        0     1052 2023-07-26 17:06:56.179925 openai_function-0.1.2/openai_function/typedefs.py
+-rw-r--r--   0        0        0     2450 2023-07-26 17:12:57.330924 openai_function-0.1.2/openai_function/vectorstore.py
+-rw-r--r--   0        0        0      445 2023-07-26 17:52:39.293498 openai_function-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 openai_function-0.1.2/PKG-INFO
```

### Comparing `openai_function-0.1.1/openai_function/__init__.py` & `openai_function-0.1.2/openai_function/__init__.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/chat_completion.py` & `openai_function-0.1.2/openai_function/chat_completion.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/client.py` & `openai_function-0.1.2/openai_function/client.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/faunadb/errors.py` & `openai_function-0.1.2/openai_function/faunadb/errors.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/faunadb/objects.py` & `openai_function-0.1.2/openai_function/faunadb/objects.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/faunadb/page.py` & `openai_function-0.1.2/openai_function/faunadb/page.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/faunadb/query.py` & `openai_function-0.1.2/openai_function/faunadb/query.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/json.py` & `openai_function-0.1.2/openai_function/json.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/logging.py` & `openai_function-0.1.2/openai_function/logging.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/odm.py` & `openai_function-0.1.2/openai_function/odm.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/openai_functions.py` & `openai_function-0.1.2/openai_function/openai_functions.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/typedefs.py` & `openai_function-0.1.2/openai_function/typedefs.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/openai_function/vectorstore.py` & `openai_function-0.1.2/openai_function/vectorstore.py`

 * *Files identical despite different names*

### Comparing `openai_function-0.1.1/PKG-INFO` & `openai_function-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: openai-function
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Oscar Bahamonde
 Author-email: oscarmartinbahamondemunoz@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pydantic[dotenv] (>=2.1.1,<3.0.0)
+Requires-Dist: pydantic[dotenv] (==1.10.11)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Description-Content-Type: text/markdown
```

