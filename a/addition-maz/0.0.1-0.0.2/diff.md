# Comparing `tmp/addition_maz-0.0.1-py3-none-any.whl.zip` & `tmp/addition_maz-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 2447 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       20 b- defN 23-Jul-25 21:11 addition_maz/__init__.py
+Zip file size: 2667 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx       58 b- defN 23-Jul-25 21:55 addition_maz/__init__.py
 -rw-rw-r--  2.0 unx       32 b- defN 23-Jul-25 21:10 addition_maz/add_f.py
--rwxrwxr-x  2.0 unx     1054 b- defN 23-Jul-25 21:43 addition_maz-0.0.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      619 b- defN 23-Jul-25 21:43 addition_maz-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 21:43 addition_maz-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 23-Jul-25 21:43 addition_maz-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      569 b- defN 23-Jul-25 21:43 addition_maz-0.0.1.dist-info/RECORD
-7 files, 2399 bytes uncompressed, 1427 bytes compressed:  40.5%
+-rw-rw-r--  2.0 unx       32 b- defN 23-Jul-25 21:52 addition_maz/sub_f.py
+-rwxrwxr-x  2.0 unx     1054 b- defN 23-Jul-25 21:57 addition_maz-0.0.2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      619 b- defN 23-Jul-25 21:57 addition_maz-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-25 21:57 addition_maz-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       13 b- defN 23-Jul-25 21:57 addition_maz-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      645 b- defN 23-Jul-25 21:57 addition_maz-0.0.2.dist-info/RECORD
+8 files, 2545 bytes uncompressed, 1529 bytes compressed:  39.9%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: addition_maz/__init__.py
 Comment: 
 
 Filename: addition_maz/add_f.py
 Comment: 
 
-Filename: addition_maz-0.0.1.dist-info/LICENSE.txt
+Filename: addition_maz/sub_f.py
 Comment: 
 
-Filename: addition_maz-0.0.1.dist-info/METADATA
+Filename: addition_maz-0.0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: addition_maz-0.0.1.dist-info/WHEEL
+Filename: addition_maz-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: addition_maz-0.0.1.dist-info/top_level.txt
+Filename: addition_maz-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: addition_maz-0.0.1.dist-info/RECORD
+Filename: addition_maz-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: addition_maz-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## addition_maz/__init__.py

```diff
@@ -1 +1,3 @@
-from .add_f import *
+from . import add_f, sub_f
+
+__all__ = ['add_f', 'sub_f']
```

## Comparing `addition_maz-0.0.1.dist-info/LICENSE.txt` & `addition_maz-0.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `addition_maz-0.0.1.dist-info/METADATA` & `addition_maz-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: addition-maz
-Version: 0.0.1
+Version: 0.0.2
 Summary: File to add two numbers
 Home-page: UNKNOWN
 Author: SYED MAZHAR
 Author-email: eusyedmazhar2806@gmail.com
 License: MIT
 Keywords: add
 Platform: UNKNOWN
```

