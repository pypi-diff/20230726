# Comparing `tmp/tap-intercom-2.0.0.tar.gz` & `tmp/tap-intercom-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-intercom-2.0.0.tar", last modified: Tue Dec 13 18:28:07 2022, max compression
+gzip compressed data, was "dist/tap-intercom-2.0.1.tar", last modified: Wed Jul 26 14:33:40 2023, max compression
```

## Comparing `tap-intercom-2.0.0.tar` & `tap-intercom-2.0.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-13 18:28:07.502002 tap-intercom-2.0.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2022-12-13 18:28:07.498002 tap-intercom-2.0.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11521 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2022-12-13 18:28:07.502002 tap-intercom-2.0.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      890 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-13 18:28:07.494002 tap-intercom-2.0.0/tap_intercom/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      981 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10427 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1588 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1960 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-13 18:28:07.498002 tap-intercom-2.0.0/tap_intercom/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1161 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/admins.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2230 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/companies.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1275 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/company_attributes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      533 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/company_segments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1570 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/contact_attributes.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7585 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/contacts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3256 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/conversation_parts.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16973 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/conversations.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      533 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/segments.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/tags.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/schemas/teams.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32805 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4007 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5606 2022-12-13 15:46:55.000000 tap-intercom-2.0.0/tap_intercom/transform.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-12-13 18:28:07.498002 tap-intercom-2.0.0/tap_intercom.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2022-12-13 18:28:07.000000 tap-intercom-2.0.0/tap_intercom.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      843 2022-12-13 18:28:07.000000 tap-intercom-2.0.0/tap_intercom.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-13 18:28:07.000000 tap-intercom-2.0.0/tap_intercom.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2022-12-13 18:28:07.000000 tap-intercom-2.0.0/tap_intercom.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      100 2022-12-13 18:28:07.000000 tap-intercom-2.0.0/tap_intercom.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2022-12-13 18:28:07.000000 tap-intercom-2.0.0/tap_intercom.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/tap_intercom/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1588 2021-11-04 13:38:11.000000 tap-intercom-2.0.1/tap_intercom/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1960 2021-11-04 13:38:11.000000 tap-intercom-2.0.1/tap_intercom/schema.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32805 2023-07-25 18:01:51.000000 tap-intercom-2.0.1/tap_intercom/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5606 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/tap_intercom/transform.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/tap_intercom/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1275 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/tap_intercom/schemas/company_attributes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2230 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/tap_intercom/schemas/companies.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7585 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/tap_intercom/schemas/contacts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16765 2023-07-26 14:33:12.000000 tap-intercom-2.0.1/tap_intercom/schemas/conversations.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3256 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/tap_intercom/schemas/conversation_parts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      533 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/tap_intercom/schemas/segments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      238 2021-11-04 13:38:11.000000 tap-intercom-2.0.1/tap_intercom/schemas/tags.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1161 2021-11-04 13:38:11.000000 tap-intercom-2.0.1/tap_intercom/schemas/admins.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      533 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/tap_intercom/schemas/company_segments.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1570 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/tap_intercom/schemas/contact_attributes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      445 2021-11-04 13:38:11.000000 tap-intercom-2.0.1/tap_intercom/schemas/teams.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4007 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/tap_intercom/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      981 2021-11-04 13:38:11.000000 tap-intercom-2.0.1/tap_intercom/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10427 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/tap_intercom/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      890 2023-07-26 14:33:12.000000 tap-intercom-2.0.1/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11521 2023-07-25 14:49:54.000000 tap-intercom-2.0.1/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2021-11-04 13:38:11.000000 tap-intercom-2.0.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2021-11-04 13:38:11.000000 tap-intercom-2.0.1/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/tap_intercom.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      100 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/tap_intercom.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      843 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/tap_intercom.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/tap_intercom.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/tap_intercom.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/tap_intercom.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/tap_intercom.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      302 2023-07-26 14:33:40.000000 tap-intercom-2.0.1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tap-intercom-2.0.0/LICENSE` & `tap-intercom-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/README.md` & `tap-intercom-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/setup.py` & `tap-intercom-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-intercom',
-      version='2.0.0',
+      version='2.0.1',
       description='Singer.io tap for extracting data from the Intercom API',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_intercom'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.23.0',
```

### Comparing `tap-intercom-2.0.0/tap_intercom/__init__.py` & `tap-intercom-2.0.1/tap_intercom/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/client.py` & `tap-intercom-2.0.1/tap_intercom/client.py`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/discover.py` & `tap-intercom-2.0.1/tap_intercom/discover.py`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/schema.py` & `tap-intercom-2.0.1/tap_intercom/schema.py`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/schemas/admins.json` & `tap-intercom-2.0.1/tap_intercom/schemas/admins.json`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/schemas/companies.json` & `tap-intercom-2.0.1/tap_intercom/schemas/companies.json`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/schemas/company_attributes.json` & `tap-intercom-2.0.1/tap_intercom/schemas/company_attributes.json`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/schemas/company_segments.json` & `tap-intercom-2.0.1/tap_intercom/schemas/segments.json`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/schemas/contact_attributes.json` & `tap-intercom-2.0.1/tap_intercom/schemas/contact_attributes.json`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/schemas/contacts.json` & `tap-intercom-2.0.1/tap_intercom/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/schemas/conversation_parts.json` & `tap-intercom-2.0.1/tap_intercom/schemas/conversation_parts.json`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/schemas/conversations.json` & `tap-intercom-2.0.1/tap_intercom/schemas/conversations.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998015873015873%*

 * *Differences: {"'properties'": "{'custom_attributes': {'additionalProperties': True, delete: ['properties']}}"}*

```diff
@@ -297,28 +297,15 @@
             "format": "date-time",
             "type": [
                 "null",
                 "string"
             ]
         },
         "custom_attributes": {
-            "properties": {
-                "issue_type": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                },
-                "priority": {
-                    "type": [
-                        "null",
-                        "string"
-                    ]
-                }
-            },
+            "additionalProperties": true,
             "type": [
                 "null",
                 "object"
             ]
         },
         "customer_first_reply": {
             "additionalProperties": false,
```

### Comparing `tap-intercom-2.0.0/tap_intercom/schemas/segments.json` & `tap-intercom-2.0.1/tap_intercom/schemas/company_segments.json`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/streams.py` & `tap-intercom-2.0.1/tap_intercom/streams.py`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/sync.py` & `tap-intercom-2.0.1/tap_intercom/sync.py`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom/transform.py` & `tap-intercom-2.0.1/tap_intercom/transform.py`

 * *Files identical despite different names*

### Comparing `tap-intercom-2.0.0/tap_intercom.egg-info/SOURCES.txt` & `tap-intercom-2.0.1/tap_intercom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

