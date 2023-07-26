# Comparing `tmp/lesscode_utils-0.0.4.tar.gz` & `tmp/lesscode_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_utils-0.0.4.tar", last modified: Tue Jul 25 15:58:22 2023, max compression
+gzip compressed data, was "dist/lesscode_utils-0.0.5.tar", last modified: Wed Jul 26 04:19:49 2023, max compression
```

## Comparing `lesscode_utils-0.0.4.tar` & `lesscode_utils-0.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/
--rw-r--r--   0 navy      (1000) navy      (1000)      375 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)       50 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/README.md
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/lesscode_utils/
--rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/__init__.py
--rw-r--r--   0 navy      (1000) navy      (1000)      261 2023-07-25 15:55:27.000000 lesscode_utils-0.0.4/lesscode_utils/const_utils.py
--rw-r--r--   0 navy      (1000) navy      (1000)     2777 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/date_time_utils.py
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/
--rw-r--r--   0 navy      (1000) navy      (1000)      226 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/__init__.py
--rw-r--r--   0 navy      (1000) navy      (1000)     1817 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/aes.py
--rw-r--r--   0 navy      (1000) navy      (1000)      621 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/base64.py
--rw-r--r--   0 navy      (1000) navy      (1000)     1722 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/des.py
--rw-r--r--   0 navy      (1000) navy      (1000)      609 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/hmac.py
--rw-r--r--   0 navy      (1000) navy      (1000)      289 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/md5.py
--rw-r--r--   0 navy      (1000) navy      (1000)     2264 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/rsa.py
--rw-r--r--   0 navy      (1000) navy      (1000)      288 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/sha1.py
--rw-r--r--   0 navy      (1000) navy      (1000)      292 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/sha256.py
--rw-r--r--   0 navy      (1000) navy      (1000)     3896 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/smx.py
--rw-r--r--   0 navy      (1000) navy      (1000)    10058 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/es_utils.py
--rw-r--r--   0 navy      (1000) navy      (1000)      786 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/lesscode_utils/json_utils.py
--rw-r--r--   0 navy      (1000) navy      (1000)      266 2023-07-25 15:57:34.000000 lesscode_utils-0.0.4/lesscode_utils/single_instance_utils.py
--rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-07-25 15:57:33.000000 lesscode_utils-0.0.4/lesscode_utils/version.py
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/lesscode_utils.egg-info/
--rw-r--r--   0 navy      (1000) navy      (1000)      375 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/lesscode_utils.egg-info/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)      863 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/lesscode_utils.egg-info/SOURCES.txt
--rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/lesscode_utils.egg-info/dependency_links.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       16 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/lesscode_utils.egg-info/requires.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       15 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/lesscode_utils.egg-info/top_level.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-07-25 15:58:22.000000 lesscode_utils-0.0.4/setup.cfg
--rw-r--r--   0 navy      (1000) navy      (1000)     1265 2023-07-25 15:23:06.000000 lesscode_utils-0.0.4/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/
+-rw-r--r--   0 baai       (501) staff       (20)      375 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       50 2023-06-15 08:16:15.000000 lesscode_utils-0.0.5/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/lesscode_utils/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-06-15 07:55:10.000000 lesscode_utils-0.0.5/lesscode_utils/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)      261 2023-07-26 01:02:54.000000 lesscode_utils-0.0.5/lesscode_utils/const_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)     2777 2023-06-15 09:20:19.000000 lesscode_utils-0.0.5/lesscode_utils/date_time_utils.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/
+-rw-r--r--   0 baai       (501) staff       (20)      226 2022-04-19 02:49:20.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1817 2023-07-18 06:03:34.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/aes.py
+-rw-r--r--   0 baai       (501) staff       (20)      621 2023-07-18 07:00:16.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/base64.py
+-rw-r--r--   0 baai       (501) staff       (20)     1722 2023-07-18 07:00:16.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/des.py
+-rw-r--r--   0 baai       (501) staff       (20)      609 2023-07-18 07:00:16.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/hmac.py
+-rw-r--r--   0 baai       (501) staff       (20)      289 2023-07-18 07:00:16.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/md5.py
+-rw-r--r--   0 baai       (501) staff       (20)     2264 2023-07-18 07:00:16.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/rsa.py
+-rw-r--r--   0 baai       (501) staff       (20)      288 2023-07-18 07:00:16.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/sha1.py
+-rw-r--r--   0 baai       (501) staff       (20)      292 2023-07-18 07:00:16.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/sha256.py
+-rw-r--r--   0 baai       (501) staff       (20)     3896 2023-07-18 07:00:16.000000 lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/smx.py
+-rw-r--r--   0 baai       (501) staff       (20)    10058 2023-07-18 10:48:39.000000 lesscode_utils-0.0.5/lesscode_utils/es_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)      854 2023-07-26 04:19:20.000000 lesscode_utils-0.0.5/lesscode_utils/json_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)      266 2023-07-26 01:12:20.000000 lesscode_utils-0.0.5/lesscode_utils/single_instance_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-07-26 04:19:43.000000 lesscode_utils-0.0.5/lesscode_utils/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/lesscode_utils.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      375 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/lesscode_utils.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      863 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/lesscode_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/lesscode_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       16 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/lesscode_utils.egg-info/requires.txt
+-rw-r--r--   0 baai       (501) staff       (20)       15 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/lesscode_utils.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-07-26 04:19:49.000000 lesscode_utils-0.0.5/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1265 2023-07-18 07:12:36.000000 lesscode_utils-0.0.5/setup.py
```

### Comparing `lesscode_utils-0.0.4/lesscode_utils/date_time_utils.py` & `lesscode_utils-0.0.5/lesscode_utils/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/aes.py` & `lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/aes.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/base64.py` & `lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/base64.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/des.py` & `lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/des.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/hmac.py` & `lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/hmac.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/rsa.py` & `lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/rsa.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.4/lesscode_utils/encryption_algorithm/smx.py` & `lesscode_utils-0.0.5/lesscode_utils/encryption_algorithm/smx.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.4/lesscode_utils/es_utils.py` & `lesscode_utils-0.0.5/lesscode_utils/es_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.4/lesscode_utils/json_utils.py` & `lesscode_utils-0.0.5/lesscode_utils/json_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 class JSONEncoder(json.JSONEncoder):
     def default(self, o):
         object_class_name = o.__class__.__name__
         if object_class_name == "ObjectId":
             return str(o)
         elif object_class_name == "datetime":
             return str(o)
+        elif object_class_name == "date":
+            return str(o)
         elif object_class_name == "bytes":
             return str(o, encoding="utf-8")
         elif object_class_name == "set":
             return list(o)
         elif object_class_name == "Decimal":
             return str(o)
         elif object_class_name == "ndarray":
```

### Comparing `lesscode_utils-0.0.4/lesscode_utils.egg-info/SOURCES.txt` & `lesscode_utils-0.0.5/lesscode_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.4/setup.py` & `lesscode_utils-0.0.5/setup.py`

 * *Files identical despite different names*

