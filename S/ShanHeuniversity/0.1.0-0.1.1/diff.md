# Comparing `tmp/ShanHeuniversity-0.1.0.tar.gz` & `tmp/ShanHeuniversity-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ShanHeuniversity-0.1.0.tar", last modified: Wed Jul 26 08:16:52 2023, max compression
+gzip compressed data, was "ShanHeuniversity-0.1.1.tar", last modified: Wed Jul 26 08:41:14 2023, max compression
```

## Comparing `ShanHeuniversity-0.1.0.tar` & `ShanHeuniversity-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 08:16:52.295256 ShanHeuniversity-0.1.0/
--rw-rw-rw-   0        0        0     4711 2023-07-26 08:16:52.295256 ShanHeuniversity-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-26 08:16:52.257437 ShanHeuniversity-0.1.0/ShanHeuniversity/
-drwxrwxrwx   0        0        0        0 2023-07-26 08:16:52.283954 ShanHeuniversity-0.1.0/ShanHeuniversity/MobAI/
--rw-rw-rw-   0        0        0       21 2023-07-26 06:50:24.000000 ShanHeuniversity-0.1.0/ShanHeuniversity/MobAI/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:16:52.295256 ShanHeuniversity-0.1.0/ShanHeuniversity/MobAI/webapi/
--rw-rw-rw-   0        0        0     1370 2023-07-26 07:18:45.000000 ShanHeuniversity-0.1.0/ShanHeuniversity/MobAI/webapi/ApiData.py
--rw-rw-rw-   0        0        0       57 2023-07-26 07:17:01.000000 ShanHeuniversity-0.1.0/ShanHeuniversity/MobAI/webapi/__init__.py
--rw-rw-rw-   0        0        0     1885 2023-07-26 07:17:01.000000 ShanHeuniversity-0.1.0/ShanHeuniversity/MobAI/webapi/api.py
--rw-rw-rw-   0        0        0      426 2023-07-26 08:15:45.000000 ShanHeuniversity-0.1.0/ShanHeuniversity/MobAI/webapi/common.py
--rw-rw-rw-   0        0        0      216 2023-07-26 07:05:25.000000 ShanHeuniversity-0.1.0/ShanHeuniversity/MobAI/webapi/error.py
--rw-rw-rw-   0        0        0       20 2023-07-26 06:50:15.000000 ShanHeuniversity-0.1.0/ShanHeuniversity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 08:16:52.283954 ShanHeuniversity-0.1.0/ShanHeuniversity.egg-info/
--rw-rw-rw-   0        0        0     4711 2023-07-26 08:16:52.000000 ShanHeuniversity-0.1.0/ShanHeuniversity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-07-26 08:16:52.000000 ShanHeuniversity-0.1.0/ShanHeuniversity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 08:16:52.000000 ShanHeuniversity-0.1.0/ShanHeuniversity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-26 08:16:52.000000 ShanHeuniversity-0.1.0/ShanHeuniversity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-26 08:16:52.295256 ShanHeuniversity-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     4771 2023-07-26 08:07:23.000000 ShanHeuniversity-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:14.011206 ShanHeuniversity-0.1.1/
+-rw-rw-rw-   0        0        0     4753 2023-07-26 08:41:14.011206 ShanHeuniversity-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:13.957341 ShanHeuniversity-0.1.1/ShanHeuniversity/
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:13.988556 ShanHeuniversity-0.1.1/ShanHeuniversity/MobAI/
+-rw-rw-rw-   0        0        0       21 2023-07-26 06:50:24.000000 ShanHeuniversity-0.1.1/ShanHeuniversity/MobAI/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:14.000682 ShanHeuniversity-0.1.1/ShanHeuniversity/MobAI/webapi/
+-rw-rw-rw-   0        0        0     1370 2023-07-26 07:18:45.000000 ShanHeuniversity-0.1.1/ShanHeuniversity/MobAI/webapi/ApiData.py
+-rw-rw-rw-   0        0        0       57 2023-07-26 07:17:01.000000 ShanHeuniversity-0.1.1/ShanHeuniversity/MobAI/webapi/__init__.py
+-rw-rw-rw-   0        0        0     1885 2023-07-26 08:39:29.000000 ShanHeuniversity-0.1.1/ShanHeuniversity/MobAI/webapi/api.py
+-rw-rw-rw-   0        0        0      448 2023-07-26 08:33:39.000000 ShanHeuniversity-0.1.1/ShanHeuniversity/MobAI/webapi/common.py
+-rw-rw-rw-   0        0        0      216 2023-07-26 07:05:25.000000 ShanHeuniversity-0.1.1/ShanHeuniversity/MobAI/webapi/error.py
+-rw-rw-rw-   0        0        0       20 2023-07-26 06:50:15.000000 ShanHeuniversity-0.1.1/ShanHeuniversity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 08:41:13.988556 ShanHeuniversity-0.1.1/ShanHeuniversity.egg-info/
+-rw-rw-rw-   0        0        0     4753 2023-07-26 08:41:13.000000 ShanHeuniversity-0.1.1/ShanHeuniversity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-07-26 08:41:13.000000 ShanHeuniversity-0.1.1/ShanHeuniversity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 08:41:13.000000 ShanHeuniversity-0.1.1/ShanHeuniversity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-26 08:41:13.000000 ShanHeuniversity-0.1.1/ShanHeuniversity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 08:41:14.011206 ShanHeuniversity-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     4813 2023-07-26 08:41:01.000000 ShanHeuniversity-0.1.1/setup.py
```

### Comparing `ShanHeuniversity-0.1.0/PKG-INFO` & `ShanHeuniversity-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ShanHeuniversity
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a module for MobAI.API.
-Home-page: https://shu.university/
+Home-page: https://github.com/ShanHeUniversityOfficial/pypi-ShanHeUniversity
 Author: MoYeRanQianZhi
 Author-email: moyeranqianzhi@gmail.com
 License: MIT License
         
         Copyright (c) 2023 MYR
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ShanHeuniversity-0.1.0/ShanHeuniversity/MobAI/webapi/ApiData.py` & `ShanHeuniversity-0.1.1/ShanHeuniversity/MobAI/webapi/ApiData.py`

 * *Files identical despite different names*

### Comparing `ShanHeuniversity-0.1.0/ShanHeuniversity/MobAI/webapi/api.py` & `ShanHeuniversity-0.1.1/ShanHeuniversity/MobAI/webapi/api.py`

 * *Files identical despite different names*

### Comparing `ShanHeuniversity-0.1.0/ShanHeuniversity.egg-info/PKG-INFO` & `ShanHeuniversity-0.1.1/ShanHeuniversity.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ShanHeuniversity
-Version: 0.1.0
+Version: 0.1.1
 Summary: This is a module for MobAI.API.
-Home-page: https://shu.university/
+Home-page: https://github.com/ShanHeUniversityOfficial/pypi-ShanHeUniversity
 Author: MoYeRanQianZhi
 Author-email: moyeranqianzhi@gmail.com
 License: MIT License
         
         Copyright (c) 2023 MYR
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `ShanHeuniversity-0.1.0/setup.py` & `ShanHeuniversity-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,17 +167,17 @@
     )
 
 ```
 '''
 
 setup(
     name='ShanHeuniversity',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
-    url='https://shu.university/',
+    url='https://github.com/ShanHeUniversityOfficial/pypi-ShanHeUniversity',
     license=LICENSE,
     author='MoYeRanQianZhi',
     author_email='moyeranqianzhi@gmail.com',
     description='This is a module for MobAI.API.',
     long_description=md,
     long_description_content_type='text/markdown',
     classifiers=[
```

