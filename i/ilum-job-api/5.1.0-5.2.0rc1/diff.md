# Comparing `tmp/ilum_job_api-5.1.0.tar.gz` & `tmp/ilum_job_api-5.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilum_job_api-5.1.0.tar", last modified: Wed Jul 26 08:26:26 2023, max compression
+gzip compressed data, was "ilum_job_api-5.2.0rc1.tar", last modified: Thu Jul 20 07:47:06 2023, max compression
```

## Comparing `ilum_job_api-5.1.0.tar` & `ilum_job_api-5.2.0rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-26 08:26:26.144176 ilum_job_api-5.1.0/
--rw-rw-r--   0 oem      (29999) oem      (29999)     6516 2023-07-26 08:19:35.000000 ilum_job_api-5.1.0/LICENSE
--rw-rw-r--   0 oem      (29999) oem      (29999)      231 2023-07-26 08:26:26.144176 ilum_job_api-5.1.0/PKG-INFO
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-26 08:26:26.140176 ilum_job_api-5.1.0/ilum_job_api/
--rw-rw-r--   0 oem      (29999) oem      (29999)        0 2023-07-26 08:19:35.000000 ilum_job_api-5.1.0/ilum_job_api/__init__.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-26 08:26:26.144176 ilum_job_api-5.1.0/ilum_job_api/api/
--rw-rw-r--   0 oem      (29999) oem      (29999)        0 2023-07-26 08:19:35.000000 ilum_job_api-5.1.0/ilum_job_api/api/__init__.py
--rw-rw-r--   0 oem      (29999) oem      (29999)      654 2023-07-26 08:19:35.000000 ilum_job_api-5.1.0/ilum_job_api/api/job_interface.py
-drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-26 08:26:26.144176 ilum_job_api-5.1.0/ilum_job_api.egg-info/
--rw-rw-r--   0 oem      (29999) oem      (29999)      231 2023-07-26 08:26:24.000000 ilum_job_api-5.1.0/ilum_job_api.egg-info/PKG-INFO
--rw-rw-r--   0 oem      (29999) oem      (29999)      248 2023-07-26 08:26:26.000000 ilum_job_api-5.1.0/ilum_job_api.egg-info/SOURCES.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-07-26 08:26:24.000000 ilum_job_api-5.1.0/ilum_job_api.egg-info/dependency_links.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       13 2023-07-26 08:26:25.000000 ilum_job_api-5.1.0/ilum_job_api.egg-info/top_level.txt
--rw-rw-r--   0 oem      (29999) oem      (29999)       38 2023-07-26 08:26:26.144176 ilum_job_api-5.1.0/setup.cfg
--rw-rw-r--   0 oem      (29999) oem      (29999)      335 2023-07-26 08:19:35.000000 ilum_job_api-5.1.0/setup.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-20 07:47:06.715228 ilum_job_api-5.2.0rc1/
+-rw-rw-r--   0 oem      (29999) oem      (29999)     6516 2023-07-10 22:51:25.000000 ilum_job_api-5.2.0rc1/LICENSE
+-rw-rw-r--   0 oem      (29999) oem      (29999)      234 2023-07-20 07:47:06.715228 ilum_job_api-5.2.0rc1/PKG-INFO
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-20 07:47:06.715228 ilum_job_api-5.2.0rc1/ilum_job_api/
+-rw-rw-r--   0 oem      (29999) oem      (29999)        0 2023-07-10 22:51:25.000000 ilum_job_api-5.2.0rc1/ilum_job_api/__init__.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-20 07:47:06.715228 ilum_job_api-5.2.0rc1/ilum_job_api/api/
+-rw-rw-r--   0 oem      (29999) oem      (29999)        0 2023-07-10 22:51:25.000000 ilum_job_api-5.2.0rc1/ilum_job_api/api/__init__.py
+-rw-rw-r--   0 oem      (29999) oem      (29999)      654 2023-07-10 22:51:25.000000 ilum_job_api-5.2.0rc1/ilum_job_api/api/job_interface.py
+drwxrwxr-x   0 oem      (29999) oem      (29999)        0 2023-07-20 07:47:06.715228 ilum_job_api-5.2.0rc1/ilum_job_api.egg-info/
+-rw-rw-r--   0 oem      (29999) oem      (29999)      234 2023-07-20 07:47:06.000000 ilum_job_api-5.2.0rc1/ilum_job_api.egg-info/PKG-INFO
+-rw-rw-r--   0 oem      (29999) oem      (29999)      248 2023-07-20 07:47:06.000000 ilum_job_api-5.2.0rc1/ilum_job_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)        1 2023-07-20 07:47:06.000000 ilum_job_api-5.2.0rc1/ilum_job_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       13 2023-07-20 07:47:06.000000 ilum_job_api-5.2.0rc1/ilum_job_api.egg-info/top_level.txt
+-rw-rw-r--   0 oem      (29999) oem      (29999)       38 2023-07-20 07:47:06.715228 ilum_job_api-5.2.0rc1/setup.cfg
+-rw-rw-r--   0 oem      (29999) oem      (29999)      339 2023-07-20 07:46:52.000000 ilum_job_api-5.2.0rc1/setup.py
```

### Comparing `ilum_job_api-5.1.0/LICENSE` & `ilum_job_api-5.2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ilum_job_api-5.1.0/ilum_job_api/api/job_interface.py` & `ilum_job_api-5.2.0rc1/ilum_job_api/api/job_interface.py`

 * *Files identical despite different names*

