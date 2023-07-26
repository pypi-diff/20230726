# Comparing `tmp/lesscode_utils-0.0.7.tar.gz` & `tmp/lesscode_utils-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_utils-0.0.7.tar", last modified: Wed Jul 26 10:23:19 2023, max compression
+gzip compressed data, was "dist/lesscode_utils-0.0.8.tar", last modified: Wed Jul 26 10:40:46 2023, max compression
```

## Comparing `lesscode_utils-0.0.7.tar` & `lesscode_utils-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/
--rw-r--r--   0 baai       (501) staff       (20)      375 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)       50 2023-06-15 08:16:15.000000 lesscode_utils-0.0.7/README.md
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/lesscode_utils/
--rw-r--r--   0 baai       (501) staff       (20)        0 2023-06-15 07:55:10.000000 lesscode_utils-0.0.7/lesscode_utils/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     3559 2023-07-26 10:23:14.000000 lesscode_utils-0.0.7/lesscode_utils/company_es_utils.py
--rw-r--r--   0 baai       (501) staff       (20)      261 2023-07-26 01:02:54.000000 lesscode_utils-0.0.7/lesscode_utils/const_utils.py
--rw-r--r--   0 baai       (501) staff       (20)     2777 2023-06-15 09:20:19.000000 lesscode_utils-0.0.7/lesscode_utils/date_time_utils.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/
--rw-r--r--   0 baai       (501) staff       (20)      226 2022-04-19 02:49:20.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/__init__.py
--rw-r--r--   0 baai       (501) staff       (20)     1817 2023-07-18 06:03:34.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/aes.py
--rw-r--r--   0 baai       (501) staff       (20)      621 2023-07-18 07:00:16.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/base64.py
--rw-r--r--   0 baai       (501) staff       (20)     1722 2023-07-18 07:00:16.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/des.py
--rw-r--r--   0 baai       (501) staff       (20)      609 2023-07-18 07:00:16.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/hmac.py
--rw-r--r--   0 baai       (501) staff       (20)      289 2023-07-18 07:00:16.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/md5.py
--rw-r--r--   0 baai       (501) staff       (20)     2264 2023-07-18 07:00:16.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/rsa.py
--rw-r--r--   0 baai       (501) staff       (20)      288 2023-07-18 07:00:16.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/sha1.py
--rw-r--r--   0 baai       (501) staff       (20)      292 2023-07-18 07:00:16.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/sha256.py
--rw-r--r--   0 baai       (501) staff       (20)     3896 2023-07-18 07:00:16.000000 lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/smx.py
--rw-r--r--   0 baai       (501) staff       (20)    10058 2023-07-26 10:22:36.000000 lesscode_utils-0.0.7/lesscode_utils/es_utils.py
--rw-r--r--   0 baai       (501) staff       (20)      854 2023-07-26 04:19:20.000000 lesscode_utils-0.0.7/lesscode_utils/json_utils.py
--rw-r--r--   0 baai       (501) staff       (20)     2162 2023-07-26 07:38:35.000000 lesscode_utils-0.0.7/lesscode_utils/mongo_util.py
--rw-r--r--   0 baai       (501) staff       (20)      266 2023-07-26 01:12:20.000000 lesscode_utils-0.0.7/lesscode_utils/single_instance_utils.py
--rw-r--r--   0 baai       (501) staff       (20)       22 2023-07-26 10:23:14.000000 lesscode_utils-0.0.7/lesscode_utils/version.py
-drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/lesscode_utils.egg-info/
--rw-r--r--   0 baai       (501) staff       (20)      375 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/lesscode_utils.egg-info/PKG-INFO
--rw-r--r--   0 baai       (501) staff       (20)      927 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/lesscode_utils.egg-info/SOURCES.txt
--rw-r--r--   0 baai       (501) staff       (20)        1 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/lesscode_utils.egg-info/dependency_links.txt
--rw-r--r--   0 baai       (501) staff       (20)       16 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/lesscode_utils.egg-info/requires.txt
--rw-r--r--   0 baai       (501) staff       (20)       15 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/lesscode_utils.egg-info/top_level.txt
--rw-r--r--   0 baai       (501) staff       (20)       38 2023-07-26 10:23:19.000000 lesscode_utils-0.0.7/setup.cfg
--rw-r--r--   0 baai       (501) staff       (20)     1265 2023-07-18 07:12:36.000000 lesscode_utils-0.0.7/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/
+-rw-r--r--   0 baai       (501) staff       (20)      375 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)       50 2023-06-15 08:16:15.000000 lesscode_utils-0.0.8/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2023-06-15 07:55:10.000000 lesscode_utils-0.0.8/lesscode_utils/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     3733 2023-07-26 10:40:37.000000 lesscode_utils-0.0.8/lesscode_utils/company_es_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)      261 2023-07-26 01:02:54.000000 lesscode_utils-0.0.8/lesscode_utils/const_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)     2777 2023-06-15 09:20:19.000000 lesscode_utils-0.0.8/lesscode_utils/date_time_utils.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/
+-rw-r--r--   0 baai       (501) staff       (20)      226 2022-04-19 02:49:20.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)     1817 2023-07-18 06:03:34.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/aes.py
+-rw-r--r--   0 baai       (501) staff       (20)      621 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/base64.py
+-rw-r--r--   0 baai       (501) staff       (20)     1722 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/des.py
+-rw-r--r--   0 baai       (501) staff       (20)      609 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/hmac.py
+-rw-r--r--   0 baai       (501) staff       (20)      289 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/md5.py
+-rw-r--r--   0 baai       (501) staff       (20)     2264 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/rsa.py
+-rw-r--r--   0 baai       (501) staff       (20)      288 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/sha1.py
+-rw-r--r--   0 baai       (501) staff       (20)      292 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/sha256.py
+-rw-r--r--   0 baai       (501) staff       (20)     3896 2023-07-18 07:00:16.000000 lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/smx.py
+-rw-r--r--   0 baai       (501) staff       (20)    10058 2023-07-26 10:22:36.000000 lesscode_utils-0.0.8/lesscode_utils/es_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)      854 2023-07-26 04:19:20.000000 lesscode_utils-0.0.8/lesscode_utils/json_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)     2162 2023-07-26 07:38:35.000000 lesscode_utils-0.0.8/lesscode_utils/mongo_util.py
+-rw-r--r--   0 baai       (501) staff       (20)      266 2023-07-26 01:12:20.000000 lesscode_utils-0.0.8/lesscode_utils/single_instance_utils.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2023-07-26 10:40:37.000000 lesscode_utils-0.0.8/lesscode_utils/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)      375 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      927 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       16 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/requires.txt
+-rw-r--r--   0 baai       (501) staff       (20)       15 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/lesscode_utils.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2023-07-26 10:40:46.000000 lesscode_utils-0.0.8/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1265 2023-07-18 07:12:36.000000 lesscode_utils-0.0.8/setup.py
```

### Comparing `lesscode_utils-0.0.7/lesscode_utils/company_es_utils.py` & `lesscode_utils-0.0.8/lesscode_utils/company_es_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -99,33 +99,31 @@
             if _:
                 tag_info["tags"].append(_)
     return tag_info
 
 
 def parse_company_tag(tags: dict, return_type: bool = False, tag_type_list: list = None):
     _tags = []
-    tag_list = [parse_company_industry_tag(tags),
-                parse_company_permission_level_tag,
-                parse_company_permission_name_tag,
-                parse_company_certification_tag,
-                parse_company_award_tag,
-                parse_company_rank_tag,
-                parse_company_diy_tag
-                ]
-
-    if tag_type_list and return_type:
-        for x in tag_list:
-            if x in tag_type_list:
-                _tags.append(x)
-    elif tag_type_list and not return_type:
-        for x in tag_list:
-            if x in tag_type_list:
-                _ = x.get("tags")
-                if _:
-                    _tags.extend(_)
-    elif not tag_type_list and return_type:
-        _tags = tag_list
+    tag_dict = {
+        "产业标签": parse_company_industry_tag,
+        "备案许可级别": parse_company_permission_level_tag,
+        "备案许可名称": parse_company_permission_name_tag,
+        "资质认证名称": parse_company_certification_tag,
+        "奖项名称": parse_company_award_tag,
+        "榜单名称": parse_company_rank_tag,
+        "diy标签": parse_company_diy_tag
+    }
+    if tag_type_list:
+        for tag_type in tag_dict:
+            if tag_type in tag_type_list and tag_type in tag_dict:
+                if not return_type:
+                    _tags.extend(tag_dict.get(tag_type)(tags).get("tags", []))
+                else:
+                    _tags.extend(tag_dict.get(tag_type)(tags))
     else:
-        for x in tag_list:
-            _ = x.get("tags")
-            if _:
-                _tags.extend(_)
+        for tag_type in tag_dict:
+            if tag_type in tag_dict:
+                if not return_type:
+                    _tags.extend(tag_dict.get(tag_type)(tags).get("tags", []))
+                else:
+                    _tags.extend(tag_dict.get(tag_type)(tags))
+    return _tags
```

### Comparing `lesscode_utils-0.0.7/lesscode_utils/date_time_utils.py` & `lesscode_utils-0.0.8/lesscode_utils/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/aes.py` & `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/aes.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/base64.py` & `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/base64.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/des.py` & `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/des.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/hmac.py` & `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/hmac.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/rsa.py` & `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/rsa.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/lesscode_utils/encryption_algorithm/smx.py` & `lesscode_utils-0.0.8/lesscode_utils/encryption_algorithm/smx.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/lesscode_utils/es_utils.py` & `lesscode_utils-0.0.8/lesscode_utils/es_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/lesscode_utils/json_utils.py` & `lesscode_utils-0.0.8/lesscode_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/lesscode_utils/mongo_util.py` & `lesscode_utils-0.0.8/lesscode_utils/mongo_util.py`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/lesscode_utils.egg-info/SOURCES.txt` & `lesscode_utils-0.0.8/lesscode_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lesscode_utils-0.0.7/setup.py` & `lesscode_utils-0.0.8/setup.py`

 * *Files identical despite different names*

