# Comparing `tmp/khmernormalizer-0.0.3.tar.gz` & `tmp/khmernormalizer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khmernormalizer-0.0.3.tar", last modified: Wed Jul 19 09:25:56 2023, max compression
+gzip compressed data, was "khmernormalizer-0.0.4.tar", last modified: Wed Jul 26 10:16:10 2023, max compression
```

## Comparing `khmernormalizer-0.0.3.tar` & `khmernormalizer-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-19 09:25:56.732277 khmernormalizer-0.0.3/
--rw-r--r--   0 seanghay   (501) staff       (20)     1065 2023-07-19 08:59:08.000000 khmernormalizer-0.0.3/LICENSE
--rw-r--r--   0 seanghay   (501) staff       (20)     1772 2023-07-19 09:25:56.731981 khmernormalizer-0.0.3/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)     1268 2023-07-19 09:25:39.000000 khmernormalizer-0.0.3/README.md
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-19 09:25:56.729910 khmernormalizer-0.0.3/khmernormalizer/
--rw-r--r--   0 seanghay   (501) staff       (20)      101 2023-07-19 09:25:51.000000 khmernormalizer-0.0.3/khmernormalizer/__init__.py
--rw-r--r--   0 seanghay   (501) staff       (20)    12453 2023-07-19 08:39:10.000000 khmernormalizer-0.0.3/khmernormalizer/mappings.py
--rw-r--r--   0 seanghay   (501) staff       (20)     1859 2023-07-19 09:25:39.000000 khmernormalizer-0.0.3/khmernormalizer/normalizer.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-19 09:25:56.731582 khmernormalizer-0.0.3/khmernormalizer.egg-info/
--rw-r--r--   0 seanghay   (501) staff       (20)     1772 2023-07-19 09:25:56.000000 khmernormalizer-0.0.3/khmernormalizer.egg-info/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      306 2023-07-19 09:25:56.000000 khmernormalizer-0.0.3/khmernormalizer.egg-info/SOURCES.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        1 2023-07-19 09:25:56.000000 khmernormalizer-0.0.3/khmernormalizer.egg-info/dependency_links.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       31 2023-07-19 09:25:56.000000 khmernormalizer-0.0.3/khmernormalizer.egg-info/requires.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       16 2023-07-19 09:25:56.000000 khmernormalizer-0.0.3/khmernormalizer.egg-info/top_level.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       38 2023-07-19 09:25:56.732364 khmernormalizer-0.0.3/setup.cfg
--rw-r--r--   0 seanghay   (501) staff       (20)      891 2023-07-19 09:25:39.000000 khmernormalizer-0.0.3/setup.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-26 10:16:10.900368 khmernormalizer-0.0.4/
+-rw-r--r--   0 seanghay   (501) staff       (20)     1065 2023-07-19 08:59:08.000000 khmernormalizer-0.0.4/LICENSE
+-rw-r--r--   0 seanghay   (501) staff       (20)     1769 2023-07-26 10:16:10.899813 khmernormalizer-0.0.4/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)     1265 2023-07-19 09:26:46.000000 khmernormalizer-0.0.4/README.md
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-26 10:16:10.896737 khmernormalizer-0.0.4/khmernormalizer/
+-rw-r--r--   0 seanghay   (501) staff       (20)      101 2023-07-26 10:11:26.000000 khmernormalizer-0.0.4/khmernormalizer/__init__.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     7309 2023-07-26 10:09:55.000000 khmernormalizer-0.0.4/khmernormalizer/khnormal.py
+-rw-r--r--   0 seanghay   (501) staff       (20)    12404 2023-07-26 10:04:58.000000 khmernormalizer-0.0.4/khmernormalizer/mappings.py
+-rw-r--r--   0 seanghay   (501) staff       (20)     1929 2023-07-26 10:11:20.000000 khmernormalizer-0.0.4/khmernormalizer/normalizer.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2023-07-26 10:16:10.899295 khmernormalizer-0.0.4/khmernormalizer.egg-info/
+-rw-r--r--   0 seanghay   (501) staff       (20)     1769 2023-07-26 10:16:10.000000 khmernormalizer-0.0.4/khmernormalizer.egg-info/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)      334 2023-07-26 10:16:10.000000 khmernormalizer-0.0.4/khmernormalizer.egg-info/SOURCES.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)        1 2023-07-26 10:16:10.000000 khmernormalizer-0.0.4/khmernormalizer.egg-info/dependency_links.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       31 2023-07-26 10:16:10.000000 khmernormalizer-0.0.4/khmernormalizer.egg-info/requires.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       16 2023-07-26 10:16:10.000000 khmernormalizer-0.0.4/khmernormalizer.egg-info/top_level.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       38 2023-07-26 10:16:10.900496 khmernormalizer-0.0.4/setup.cfg
+-rw-r--r--   0 seanghay   (501) staff       (20)      891 2023-07-19 09:25:39.000000 khmernormalizer-0.0.4/setup.py
```

### Comparing `khmernormalizer-0.0.3/LICENSE` & `khmernormalizer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `khmernormalizer-0.0.3/PKG-INFO` & `khmernormalizer-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khmernormalizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A missing toolkit for Khmer Natural Language Processing.
 Home-page: https://github.com/seanghay/khmernormalizer
 Author: Seanghay Yath
 Author-email: seanghay.dev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -59,10 +59,10 @@
 Result:
 ```
 តាម៖សេចក្តីរាយការណ៍ឱ្យដឹងថា!
 
 កាល ពីវេលាម៉ោងៗ ប្រមាណ១១យប់ថ្ងៃទី៤?
 កាត់
 មិន 
-មួយរយៈះ
+មួយរយៈ
 រយៈពេល
 ```
```

### Comparing `khmernormalizer-0.0.3/README.md` & `khmernormalizer-0.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,10 +44,10 @@
 Result:
 ```
 តាម៖សេចក្តីរាយការណ៍ឱ្យដឹងថា!
 
 កាល ពីវេលាម៉ោងៗ ប្រមាណ១១យប់ថ្ងៃទី៤?
 កាត់
 មិន 
-មួយរយៈះ
+មួយរយៈ
 រយៈពេល
 ```
```

### Comparing `khmernormalizer-0.0.3/khmernormalizer/mappings.py` & `khmernormalizer-0.0.4/khmernormalizer/mappings.py`

 * *Files 2% similar despite different names*

```diff
@@ -582,18 +582,15 @@
     "។ល។": "\u17d8",
     "ឨញ្ញា": "ឧក",
     "ឣ": "អ",
     "ឤ": "អា",
     "ឲ": "ឱ",
     "\u17DD": "\u17D1",
     "\u17D3": "\u17C6",
-    
-    "ីុ": "៊ី",
-    "៉ី": "៊ី",
-    
+        
     "\u17C1\u17B8": "\u17BE",
     "\u17B8\u17C1": "\u17BE",
     "\u17C1\u17B6": "\u17C4",
     
     "\u17bb\u17d0": "\u17c9\u17d0",
     
     "\u17c9\u17c6": "\u17bb\u17c6",
```

### Comparing `khmernormalizer-0.0.3/khmernormalizer/normalizer.py` & `khmernormalizer-0.0.4/khmernormalizer/normalizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 # adapted from https://github.com/csebuetnlp/normalizer/blob/main/normalizer/const.py
 from ftfy import fix_text, TextFixerConfig
 from emoji import replace_emoji
 from khmernormalizer import mappings
+from khmernormalizer.khnormal import khmer_normalize
 
 import re
 import unicodedata
 
 def fix_quotes(text):
     text = mappings.SINGLE_QUOTE_REGEX.sub("'", text)
     text = mappings.DOUBLE_QUOTE_REGEX.sub('"', text)
@@ -60,8 +61,8 @@
     
   # remove space between punctuation
   text = re.sub(r"[ ]+([៙៚៖!?។៕\u17d8])", r"\1", text)
   
   # remove space between the repeat char
   text = re.sub(r"[^\S\r\n]+ៗ", "ៗ", text)
   
-  return text.strip()
+  return khmer_normalize(text.strip())
```

### Comparing `khmernormalizer-0.0.3/khmernormalizer.egg-info/PKG-INFO` & `khmernormalizer-0.0.4/khmernormalizer.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khmernormalizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A missing toolkit for Khmer Natural Language Processing.
 Home-page: https://github.com/seanghay/khmernormalizer
 Author: Seanghay Yath
 Author-email: seanghay.dev@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -59,10 +59,10 @@
 Result:
 ```
 តាម៖សេចក្តីរាយការណ៍ឱ្យដឹងថា!
 
 កាល ពីវេលាម៉ោងៗ ប្រមាណ១១យប់ថ្ងៃទី៤?
 កាត់
 មិន 
-មួយរយៈះ
+មួយរយៈ
 រយៈពេល
 ```
```

### Comparing `khmernormalizer-0.0.3/setup.py` & `khmernormalizer-0.0.4/setup.py`

 * *Files identical despite different names*

