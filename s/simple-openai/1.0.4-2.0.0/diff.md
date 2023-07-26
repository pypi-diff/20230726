# Comparing `tmp/simple-openai-1.0.4.tar.gz` & `tmp/simple-openai-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-openai-1.0.4.tar", last modified: Wed Jun 14 17:56:03 2023, max compression
+gzip compressed data, was "simple-openai-2.0.0.tar", last modified: Wed Jul 26 20:20:26 2023, max compression
```

## Comparing `simple-openai-1.0.4.tar` & `simple-openai-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-14 17:56:03.498294 simple-openai-1.0.4/
--rw-r--r--   0 steve      (501) staff       (20)    11357 2023-04-15 11:09:16.000000 simple-openai-1.0.4/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)    16536 2023-06-14 17:56:03.498077 simple-openai-1.0.4/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     2639 2023-04-16 15:14:11.000000 simple-openai-1.0.4/README.md
--rw-r--r--   0 steve      (501) staff       (20)     1179 2023-06-14 17:53:17.000000 simple-openai-1.0.4/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-06-14 17:56:03.498336 simple-openai-1.0.4/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-14 17:56:03.493663 simple-openai-1.0.4/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-14 17:56:03.496048 simple-openai-1.0.4/src/simple_openai/
--rw-r--r--   0 steve      (501) staff       (20)      223 2023-04-16 13:49:41.000000 simple-openai-1.0.4/src/simple_openai/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6571 2023-04-16 13:37:12.000000 simple-openai-1.0.4/src/simple_openai/async_simple_openai.py
--rw-r--r--   0 steve      (501) staff       (20)      184 2023-04-16 13:51:48.000000 simple-openai-1.0.4/src/simple_openai/constants.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-14 17:56:03.497180 simple-openai-1.0.4/src/simple_openai/models/
--rw-r--r--   0 steve      (501) staff       (20)      888 2023-06-14 17:51:45.000000 simple-openai-1.0.4/src/simple_openai/models/open_ai_models.py
--rw-r--r--   0 steve      (501) staff       (20)      672 2023-04-16 13:21:37.000000 simple-openai-1.0.4/src/simple_openai/responses.py
--rw-r--r--   0 steve      (501) staff       (20)     6054 2023-05-26 20:55:41.000000 simple-openai-1.0.4/src/simple_openai/simple_openai.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-14 17:56:03.497000 simple-openai-1.0.4/src/simple_openai.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    16536 2023-06-14 17:56:03.000000 simple-openai-1.0.4/src/simple_openai.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      506 2023-06-14 17:56:03.000000 simple-openai-1.0.4/src/simple_openai.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-06-14 17:56:03.000000 simple-openai-1.0.4/src/simple_openai.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       89 2023-06-14 17:56:03.000000 simple-openai-1.0.4/src/simple_openai.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       14 2023-06-14 17:56:03.000000 simple-openai-1.0.4/src/simple_openai.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-14 17:56:03.497693 simple-openai-1.0.4/tests/
--rw-r--r--   0 steve      (501) staff       (20)     1579 2023-04-16 19:32:12.000000 simple-openai-1.0.4/tests/test_AsyncSimpleOpenai.py
--rw-r--r--   0 steve      (501) staff       (20)     1461 2023-04-16 13:51:21.000000 simple-openai-1.0.4/tests/test_SimpleOpenai.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-26 20:20:26.884118 simple-openai-2.0.0/
+-rw-r--r--   0 steve      (501) staff       (20)    11357 2023-04-15 11:09:16.000000 simple-openai-2.0.0/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)    16536 2023-07-26 20:20:26.883943 simple-openai-2.0.0/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     2639 2023-04-16 15:14:11.000000 simple-openai-2.0.0/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     1179 2023-07-08 20:16:05.000000 simple-openai-2.0.0/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-07-26 20:20:26.884169 simple-openai-2.0.0/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-26 20:20:26.879855 simple-openai-2.0.0/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-26 20:20:26.881757 simple-openai-2.0.0/src/simple_openai/
+-rw-r--r--   0 steve      (501) staff       (20)      223 2023-06-17 09:54:32.000000 simple-openai-2.0.0/src/simple_openai/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6571 2023-07-08 20:15:20.000000 simple-openai-2.0.0/src/simple_openai/async_simple_openai.py
+-rw-r--r--   0 steve      (501) staff       (20)      184 2023-04-16 13:51:48.000000 simple-openai-2.0.0/src/simple_openai/constants.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-26 20:20:26.882869 simple-openai-2.0.0/src/simple_openai/models/
+-rw-r--r--   0 steve      (501) staff       (20)      875 2023-07-08 20:15:50.000000 simple-openai-2.0.0/src/simple_openai/models/open_ai_models.py
+-rw-r--r--   0 steve      (501) staff       (20)      672 2023-06-17 10:00:41.000000 simple-openai-2.0.0/src/simple_openai/responses.py
+-rw-r--r--   0 steve      (501) staff       (20)     6054 2023-06-17 09:54:32.000000 simple-openai-2.0.0/src/simple_openai/simple_openai.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-26 20:20:26.882648 simple-openai-2.0.0/src/simple_openai.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    16536 2023-07-26 20:20:26.000000 simple-openai-2.0.0/src/simple_openai.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      506 2023-07-26 20:20:26.000000 simple-openai-2.0.0/src/simple_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-07-26 20:20:26.000000 simple-openai-2.0.0/src/simple_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       89 2023-07-26 20:20:26.000000 simple-openai-2.0.0/src/simple_openai.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       14 2023-07-26 20:20:26.000000 simple-openai-2.0.0/src/simple_openai.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-26 20:20:26.883544 simple-openai-2.0.0/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     1579 2023-07-08 20:15:20.000000 simple-openai-2.0.0/tests/test_AsyncSimpleOpenai.py
+-rw-r--r--   0 steve      (501) staff       (20)     1461 2023-04-16 13:51:21.000000 simple-openai-2.0.0/tests/test_SimpleOpenai.py
```

### Comparing `simple-openai-1.0.4/LICENSE` & `simple-openai-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.4/PKG-INFO` & `simple-openai-2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-openai
-Version: 1.0.4
+Version: 2.0.0
 Summary: Simple OpenAI API wrapper
 Author-email: Stephen Schleising <stephen@schleising.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple-openai-1.0.4/README.md` & `simple-openai-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.4/pyproject.toml` & `simple-openai-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-openai"
-version = "1.0.4"
+version = "2.0.0"
 description = "Simple OpenAI API wrapper"
 readme = "README.md"
 authors = [{ name = "Stephen Schleising", email = "stephen@schleising.net" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `simple-openai-1.0.4/src/simple_openai/async_simple_openai.py` & `simple-openai-2.0.0/src/simple_openai/async_simple_openai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.4/src/simple_openai/models/open_ai_models.py` & `simple-openai-2.0.0/src/simple_openai/models/open_ai_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pydantic import BaseModel
 
 class ChatMessage(BaseModel):
     role: str = 'user'
     content: str
 
 class ChatRequest(BaseModel):
-    model: str = 'gpt-3.5-turbo-0613'
+    model: str = 'gpt-4'
     messages: list[ChatMessage]
 
 class Choice(BaseModel):
     index: int
     message: ChatMessage
     finish_reason: str
```

### Comparing `simple-openai-1.0.4/src/simple_openai/responses.py` & `simple-openai-2.0.0/src/simple_openai/responses.py`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.4/src/simple_openai/simple_openai.py` & `simple-openai-2.0.0/src/simple_openai/simple_openai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.4/src/simple_openai.egg-info/PKG-INFO` & `simple-openai-2.0.0/src/simple_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-openai
-Version: 1.0.4
+Version: 2.0.0
 Summary: Simple OpenAI API wrapper
 Author-email: Stephen Schleising <stephen@schleising.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `simple-openai-1.0.4/tests/test_AsyncSimpleOpenai.py` & `simple-openai-2.0.0/tests/test_AsyncSimpleOpenai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-1.0.4/tests/test_SimpleOpenai.py` & `simple-openai-2.0.0/tests/test_SimpleOpenai.py`

 * *Files identical despite different names*

