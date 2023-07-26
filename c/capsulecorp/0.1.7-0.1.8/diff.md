# Comparing `tmp/capsulecorp-0.1.7.tar.gz` & `tmp/capsulecorp-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsulecorp-0.1.7.tar", last modified: Wed Jul 19 14:17:51 2023, max compression
+gzip compressed data, was "capsulecorp-0.1.8.tar", last modified: Wed Jul 26 15:42:59 2023, max compression
```

## Comparing `capsulecorp-0.1.7.tar` & `capsulecorp-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-19 14:17:51.727478 capsulecorp-0.1.7/
--rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.7/LICENSE
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-19 14:17:51.726590 capsulecorp-0.1.7/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.7/README.md
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-19 14:17:51.705343 capsulecorp-0.1.7/capsulecorp/
--rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.7/capsulecorp/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.7/capsulecorp/query_driver.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-19 14:17:51.724106 capsulecorp-0.1.7/capsulecorp/utilities/
--rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.7/capsulecorp/utilities/__init__.py
--rw-r--r--   0 daless383   (502) staff       (20)     8822 2023-07-18 18:00:19.000000 capsulecorp-0.1.7/capsulecorp/utilities/databricks_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.7/capsulecorp/utilities/github_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)    11719 2023-07-19 13:41:59.000000 capsulecorp-0.1.7/capsulecorp/utilities/s3_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.7/capsulecorp/utilities/slack_utils.py
--rw-r--r--   0 daless383   (502) staff       (20)     5206 2023-07-19 13:43:55.000000 capsulecorp-0.1.7/capsulecorp/utils.py
--rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-18 16:47:33.000000 capsulecorp-0.1.7/capsulecorp/version.py
-drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-19 14:17:51.712840 capsulecorp-0.1.7/capsulecorp.egg-info/
--rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-19 14:17:50.000000 capsulecorp-0.1.7/capsulecorp.egg-info/PKG-INFO
--rw-r--r--   0 daless383   (502) staff       (20)      496 2023-07-19 14:17:51.000000 capsulecorp-0.1.7/capsulecorp.egg-info/SOURCES.txt
--rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-19 14:17:50.000000 capsulecorp-0.1.7/capsulecorp.egg-info/dependency_links.txt
--rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-19 14:17:51.000000 capsulecorp-0.1.7/capsulecorp.egg-info/requires.txt
--rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-19 14:17:51.000000 capsulecorp-0.1.7/capsulecorp.egg-info/top_level.txt
--rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.7/pyproject.toml
--rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-19 14:17:51.727766 capsulecorp-0.1.7/setup.cfg
--rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.7/setup.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-26 15:42:59.304899 capsulecorp-0.1.8/
+-rw-r--r--   0 daless383   (502) staff       (20)    11357 2023-02-13 20:25:15.000000 capsulecorp-0.1.8/LICENSE
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-26 15:42:59.304171 capsulecorp-0.1.8/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)       99 2023-02-13 20:25:15.000000 capsulecorp-0.1.8/README.md
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-26 15:42:59.289193 capsulecorp-0.1.8/capsulecorp/
+-rw-r--r--   0 daless383   (502) staff       (20)       63 2023-02-14 15:14:02.000000 capsulecorp-0.1.8/capsulecorp/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     7967 2023-05-04 16:53:29.000000 capsulecorp-0.1.8/capsulecorp/query_driver.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-26 15:42:59.302496 capsulecorp-0.1.8/capsulecorp/utilities/
+-rw-r--r--   0 daless383   (502) staff       (20)        0 2023-07-13 15:20:45.000000 capsulecorp-0.1.8/capsulecorp/utilities/__init__.py
+-rw-r--r--   0 daless383   (502) staff       (20)     8822 2023-07-18 18:00:19.000000 capsulecorp-0.1.8/capsulecorp/utilities/databricks_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     1441 2023-07-10 20:48:28.000000 capsulecorp-0.1.8/capsulecorp/utilities/github_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)    11719 2023-07-26 15:36:05.000000 capsulecorp-0.1.8/capsulecorp/utilities/s3_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     2320 2023-05-18 14:36:49.000000 capsulecorp-0.1.8/capsulecorp/utilities/slack_utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)     5206 2023-07-19 13:43:55.000000 capsulecorp-0.1.8/capsulecorp/utils.py
+-rw-r--r--   0 daless383   (502) staff       (20)      269 2023-07-26 15:34:06.000000 capsulecorp-0.1.8/capsulecorp/version.py
+drwxr-xr-x   0 daless383   (502) staff       (20)        0 2023-07-26 15:42:59.295246 capsulecorp-0.1.8/capsulecorp.egg-info/
+-rw-r--r--   0 daless383   (502) staff       (20)      461 2023-07-26 15:42:58.000000 capsulecorp-0.1.8/capsulecorp.egg-info/PKG-INFO
+-rw-r--r--   0 daless383   (502) staff       (20)      496 2023-07-26 15:42:59.000000 capsulecorp-0.1.8/capsulecorp.egg-info/SOURCES.txt
+-rw-r--r--   0 daless383   (502) staff       (20)        1 2023-07-26 15:42:58.000000 capsulecorp-0.1.8/capsulecorp.egg-info/dependency_links.txt
+-rw-r--r--   0 daless383   (502) staff       (20)      106 2023-07-26 15:42:59.000000 capsulecorp-0.1.8/capsulecorp.egg-info/requires.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       12 2023-07-26 15:42:59.000000 capsulecorp-0.1.8/capsulecorp.egg-info/top_level.txt
+-rw-r--r--   0 daless383   (502) staff       (20)       86 2023-02-14 15:04:49.000000 capsulecorp-0.1.8/pyproject.toml
+-rw-r--r--   0 daless383   (502) staff       (20)       38 2023-07-26 15:42:59.305134 capsulecorp-0.1.8/setup.cfg
+-rw-r--r--   0 daless383   (502) staff       (20)     6621 2023-07-12 13:53:07.000000 capsulecorp-0.1.8/setup.py
```

### Comparing `capsulecorp-0.1.7/LICENSE` & `capsulecorp-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.7/capsulecorp/query_driver.py` & `capsulecorp-0.1.8/capsulecorp/query_driver.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.7/capsulecorp/utilities/databricks_utils.py` & `capsulecorp-0.1.8/capsulecorp/utilities/databricks_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.7/capsulecorp/utilities/github_utils.py` & `capsulecorp-0.1.8/capsulecorp/utilities/github_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.7/capsulecorp/utilities/s3_utils.py` & `capsulecorp-0.1.8/capsulecorp/utilities/s3_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,20 +25,20 @@
     """
         This method will parse an s3 url.
 
         Args:
             s3_url (str): s3 url
 
         Returns:
-            s3 bucket name and s3 key
+            prefix and bucket name
     """
     # Parse proper output url
     parse_result = urlparse(s3_url)
-    # Return bucket name and s3 key
-    return parse_result.netloc, parse_result.path[1:]
+    # Return prefix and bucket name 
+    return parse_result.path[1:], parse_result.netloc, 
 
 
 def read_file(access_key, secret_key, s3_prefix, bucket_name):
     """
         This method will read files from s3 using a boto3 client.
 
         Args:
```

### Comparing `capsulecorp-0.1.7/capsulecorp/utilities/slack_utils.py` & `capsulecorp-0.1.8/capsulecorp/utilities/slack_utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.7/capsulecorp/utils.py` & `capsulecorp-0.1.8/capsulecorp/utils.py`

 * *Files identical despite different names*

### Comparing `capsulecorp-0.1.7/setup.py` & `capsulecorp-0.1.8/setup.py`

 * *Files identical despite different names*

