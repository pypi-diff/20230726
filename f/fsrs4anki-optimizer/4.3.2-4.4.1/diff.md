# Comparing `tmp/fsrs4anki_optimizer-4.3.2.tar.gz` & `tmp/fsrs4anki_optimizer-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-4.3.2.tar", last modified: Fri Jul 21 12:34:53 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-4.4.1.tar", last modified: Wed Jul 26 03:17:55 2023, max compression
```

## Comparing `fsrs4anki_optimizer-4.3.2.tar` & `fsrs4anki_optimizer-4.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:34:53.932449 fsrs4anki_optimizer-4.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 12:34:53.932449 fsrs4anki_optimizer-4.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:34:53.932449 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-21 12:34:44.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-07-21 12:34:44.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51382 2023-07-21 12:34:44.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 12:34:53.932449 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-21 12:34:53.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-21 12:34:53.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 12:34:53.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-21 12:34:53.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-21 12:34:53.000000 fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-21 12:34:44.000000 fsrs4anki_optimizer-4.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 12:34:53.932449 fsrs4anki_optimizer-4.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-21 12:34:44.000000 fsrs4anki_optimizer-4.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:17:55.368882 fsrs4anki_optimizer-4.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-26 03:17:55.368882 fsrs4anki_optimizer-4.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:17:55.368882 fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-26 03:17:44.000000 fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-26 03:17:44.000000 fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51382 2023-07-26 03:17:44.000000 fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:17:55.368882 fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-26 03:17:55.000000 fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-26 03:17:55.000000 fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 03:17:55.000000 fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 03:17:55.000000 fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-26 03:17:55.000000 fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-26 03:17:44.000000 fsrs4anki_optimizer-4.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 03:17:55.368882 fsrs4anki_optimizer-4.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 03:17:44.000000 fsrs4anki_optimizer-4.4.1/setup.py
```

### Comparing `fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# python fsrs4anki_optimizer_cmd.py <filename.apkg|filename.colpkg>
 import fsrs4anki_optimizer
 import argparse
 import json
 import pytz
 import os
 
 def prompt(msg: str, fallback):
@@ -82,15 +81,15 @@
             f.show()
 
     optimizer.preview(optimizer.optimal_retention)
 
     profile = \
     f"""{{
     // Generated, Optimized anki deck settings
-    "deckName": "{args.filename}",// PLEASE CHANGE THIS TO THE DECKS PROPER NAME
+    "deckName": "{os.path.splitext(os.path.basename(filename))[0]}",// PLEASE CHANGE THIS TO THE DECKS PROPER NAME
     "w": {optimizer.w},
     "requestRetention": {optimizer.optimal_retention},
     "maximumInterval": 36500,
 }},
 """
 
     print("Paste this into your scheduling code")
@@ -108,26 +107,30 @@
             f.show()
 
 if __name__ == "__main__":
 
     config_save = os.path.expanduser(".fsrs4anki_optimizer")
 
     parser = argparse.ArgumentParser()
-    parser.add_argument("filename")
+    parser.add_argument("filenames", nargs='+')
     parser.add_argument("-y","--yes",
                         action=argparse.BooleanOptionalAction,
                         help="If set automatically defaults on all stdin settings."
                         )
     parser.add_argument("-o","--out",
                         help="File to APPEND the automatically generated profile to."
                         )
     args = parser.parse_args()
 
-
-    if os.path.isdir(args.filename):
-        files = [f for f in os.listdir(args.filename) if f.lower().endswith('.apkg')]
-        files = [os.path.join(args.filename, f) for f in files]
-        for file_path in files:
-            process(file_path)
-    else:
-        process(args.filename)
+    for filename in args.filenames:
+        if os.path.isdir(filename):
+            files = [f for f in os.listdir(filename) if f.lower().endswith('.apkg')]
+            files = [os.path.join(filename, f) for f in files]
+            for file_path in files:
+                try:
+                    process(file_path)
+                except Exception as e:
+                    print(f"Failed to process {file_path}")
+                    continue
+        else:
+            process(filename)
```

### Comparing `fsrs4anki_optimizer-4.3.2/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-4.4.1/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files identical despite different names*

