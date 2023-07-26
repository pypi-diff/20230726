# Comparing `tmp/pyimgurapi-0.4.2.tar.gz` & `tmp/pyimgurapi-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimgurapi-0.4.2.tar", max compression
+gzip compressed data, was "pyimgurapi-0.4.3.tar", max compression
```

## Comparing `pyimgurapi-0.4.2.tar` & `pyimgurapi-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1080 2023-05-05 16:45:13.078314 pyimgurapi-0.4.2/LICENSE
--rw-r--r--   0        0        0       54 2023-05-08 15:51:05.855700 pyimgurapi-0.4.2/pyimgurapi/__init__.py
--rw-r--r--   0        0        0     2771 2023-07-23 11:47:22.776243 pyimgurapi-0.4.2/pyimgurapi/api.py
--rw-r--r--   0        0        0      241 2023-05-08 18:48:16.094298 pyimgurapi-0.4.2/pyimgurapi/endpoints/__init__.py
--rw-r--r--   0        0        0     6338 2023-07-23 01:11:40.129544 pyimgurapi-0.4.2/pyimgurapi/endpoints/account.py
--rw-r--r--   0        0        0     3993 2023-06-11 20:39:27.669271 pyimgurapi-0.4.2/pyimgurapi/endpoints/album.py
--rw-r--r--   0        0        0     2601 2023-07-19 21:36:40.810670 pyimgurapi-0.4.2/pyimgurapi/endpoints/base_endpoint.py
--rw-r--r--   0        0        0     2409 2023-06-25 12:25:21.696989 pyimgurapi-0.4.2/pyimgurapi/endpoints/comment.py
--rw-r--r--   0        0        0       82 2023-05-08 18:11:01.478181 pyimgurapi-0.4.2/pyimgurapi/endpoints/feed.py
--rw-r--r--   0        0        0       85 2023-05-08 18:11:01.512250 pyimgurapi-0.4.2/pyimgurapi/endpoints/gallery.py
--rw-r--r--   0        0        0     9856 2023-07-23 01:12:22.523470 pyimgurapi-0.4.2/pyimgurapi/endpoints/image.py
--rw-r--r--   0        0        0      502 2023-05-11 18:42:58.380280 pyimgurapi-0.4.2/pyimgurapi/exceptions.py
--rw-r--r--   0        0        0     2951 2023-07-12 18:16:54.887240 pyimgurapi-0.4.2/pyimgurapi/form_factories.py
--rw-r--r--   0        0        0     3846 2023-07-23 11:43:47.712185 pyimgurapi-0.4.2/pyimgurapi/utils.py
--rw-r--r--   0        0        0      388 2023-07-23 16:36:07.344205 pyimgurapi-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     5094 2023-07-23 16:33:31.233528 pyimgurapi-0.4.2/README.md
--rw-r--r--   0        0        0     5436 1970-01-01 00:00:00.000000 pyimgurapi-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-05 16:45:13.078314 pyimgurapi-0.4.3/LICENSE
+-rw-r--r--   0        0        0       54 2023-05-08 15:51:05.855700 pyimgurapi-0.4.3/pyimgurapi/__init__.py
+-rw-r--r--   0        0        0     2771 2023-07-23 11:47:22.776243 pyimgurapi-0.4.3/pyimgurapi/api.py
+-rw-r--r--   0        0        0      241 2023-05-08 18:48:16.094298 pyimgurapi-0.4.3/pyimgurapi/endpoints/__init__.py
+-rw-r--r--   0        0        0     6338 2023-07-23 01:11:40.129544 pyimgurapi-0.4.3/pyimgurapi/endpoints/account.py
+-rw-r--r--   0        0        0     3993 2023-06-11 20:39:27.669271 pyimgurapi-0.4.3/pyimgurapi/endpoints/album.py
+-rw-r--r--   0        0        0     2601 2023-07-19 21:36:40.810670 pyimgurapi-0.4.3/pyimgurapi/endpoints/base_endpoint.py
+-rw-r--r--   0        0        0    10933 2023-07-26 20:39:09.374900 pyimgurapi-0.4.3/pyimgurapi/endpoints/comment.py
+-rw-r--r--   0        0        0       82 2023-05-08 18:11:01.478181 pyimgurapi-0.4.3/pyimgurapi/endpoints/feed.py
+-rw-r--r--   0        0        0       85 2023-05-08 18:11:01.512250 pyimgurapi-0.4.3/pyimgurapi/endpoints/gallery.py
+-rw-r--r--   0        0        0     9856 2023-07-23 01:12:22.523470 pyimgurapi-0.4.3/pyimgurapi/endpoints/image.py
+-rw-r--r--   0        0        0      502 2023-05-11 18:42:58.380280 pyimgurapi-0.4.3/pyimgurapi/exceptions.py
+-rw-r--r--   0        0        0     2951 2023-07-12 18:16:54.887240 pyimgurapi-0.4.3/pyimgurapi/form_factories.py
+-rw-r--r--   0        0        0     3846 2023-07-23 11:43:47.712185 pyimgurapi-0.4.3/pyimgurapi/utils.py
+-rw-r--r--   0        0        0      597 2023-07-26 21:15:43.190641 pyimgurapi-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     5094 2023-07-23 16:33:31.233528 pyimgurapi-0.4.3/README.md
+-rw-r--r--   0        0        0     5649 1970-01-01 00:00:00.000000 pyimgurapi-0.4.3/PKG-INFO
```

### Comparing `pyimgurapi-0.4.2/LICENSE` & `pyimgurapi-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyimgurapi-0.4.2/pyimgurapi/api.py` & `pyimgurapi-0.4.3/pyimgurapi/api.py`

 * *Files identical despite different names*

### Comparing `pyimgurapi-0.4.2/pyimgurapi/endpoints/account.py` & `pyimgurapi-0.4.3/pyimgurapi/endpoints/account.py`

 * *Files identical despite different names*

### Comparing `pyimgurapi-0.4.2/pyimgurapi/endpoints/album.py` & `pyimgurapi-0.4.3/pyimgurapi/endpoints/album.py`

 * *Files identical despite different names*

### Comparing `pyimgurapi-0.4.2/pyimgurapi/endpoints/base_endpoint.py` & `pyimgurapi-0.4.3/pyimgurapi/endpoints/base_endpoint.py`

 * *Files identical despite different names*

### Comparing `pyimgurapi-0.4.2/pyimgurapi/endpoints/image.py` & `pyimgurapi-0.4.3/pyimgurapi/endpoints/image.py`

 * *Files identical despite different names*

### Comparing `pyimgurapi-0.4.2/pyimgurapi/form_factories.py` & `pyimgurapi-0.4.3/pyimgurapi/form_factories.py`

 * *Files identical despite different names*

### Comparing `pyimgurapi-0.4.2/pyimgurapi/utils.py` & `pyimgurapi-0.4.3/pyimgurapi/utils.py`

 * *Files identical despite different names*

### Comparing `pyimgurapi-0.4.2/README.md` & `pyimgurapi-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyimgurapi-0.4.2/PKG-INFO` & `pyimgurapi-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: pyimgurapi
-Version: 0.4.2
-Summary: 
+Version: 0.4.3
+Summary: A Python SDK for the Imgur API.
+Home-page: https://github.com/nautics889/PyImgurApi
+License: MIT
 Author: nautics889
 Author-email: cyberukr@gmail.com
 Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/nautics889/PyImgurApi
 Description-Content-Type: text/markdown
 
 # PyImgurAPI
 
 [![PyPI](https://img.shields.io/pypi/v/pyimgurapi.svg)](https://pypi.org/project/pyimgurapi/)
 [![Python Version](https://img.shields.io/pypi/pyversions/pyimgurapi.svg)](https://pypi.org/project/pyimgurapi/)
```

