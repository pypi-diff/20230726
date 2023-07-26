# Comparing `tmp/AppWrapper-0.1.1-py3-none-any.whl.zip` & `tmp/AppWrapper-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,10 @@
-Zip file size: 2723 bytes, number of entries: 6
+Zip file size: 4349 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       53 b- defN 23-Jun-12 05:28 app_common/__init__.py
 -rw-rw-r--  2.0 unx     5264 b- defN 23-Jul-24 07:10 app_common/app_common.py
--rw-rw-r--  2.0 unx      125 b- defN 23-Jul-24 07:21 AppWrapper-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-24 07:21 AppWrapper-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jul-24 07:21 AppWrapper-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      467 b- defN 23-Jul-24 07:21 AppWrapper-0.1.1.dist-info/RECORD
-6 files, 6012 bytes uncompressed, 1873 bytes compressed:  68.8%
+-rw-rw-r--  2.0 unx       60 b- defN 23-Jul-26 04:31 app_wrapper/__init__.py
+-rw-rw-r--  2.0 unx     4466 b- defN 23-Jul-26 05:40 app_wrapper/app_wrapper.py
+-rw-rw-r--  2.0 unx      125 b- defN 23-Jul-26 05:53 AppWrapper-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-26 05:53 AppWrapper-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       12 b- defN 23-Jul-26 05:53 AppWrapper-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      628 b- defN 23-Jul-26 05:53 AppWrapper-0.1.2.dist-info/RECORD
+8 files, 10700 bytes uncompressed, 3249 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -1,19 +1,25 @@
 Filename: app_common/__init__.py
 Comment: 
 
 Filename: app_common/app_common.py
 Comment: 
 
-Filename: AppWrapper-0.1.1.dist-info/METADATA
+Filename: app_wrapper/__init__.py
 Comment: 
 
-Filename: AppWrapper-0.1.1.dist-info/WHEEL
+Filename: app_wrapper/app_wrapper.py
 Comment: 
 
-Filename: AppWrapper-0.1.1.dist-info/top_level.txt
+Filename: AppWrapper-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: AppWrapper-0.1.1.dist-info/RECORD
+Filename: AppWrapper-0.1.2.dist-info/WHEEL
+Comment: 
+
+Filename: AppWrapper-0.1.2.dist-info/top_level.txt
+Comment: 
+
+Filename: AppWrapper-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

