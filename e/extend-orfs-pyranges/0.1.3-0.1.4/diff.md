# Comparing `tmp/extend_orfs_pyranges-0.1.3.tar.gz` & `tmp/extend_orfs_pyranges-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extend_orfs_pyranges-0.1.3.tar", last modified: Wed Jul 26 13:52:11 2023, max compression
+gzip compressed data, was "extend_orfs_pyranges-0.1.4.tar", last modified: Wed Jul 26 14:29:52 2023, max compression
```

## Comparing `extend_orfs_pyranges-0.1.3.tar` & `extend_orfs_pyranges-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 13:52:11.198746 extend_orfs_pyranges-0.1.3/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-26 13:52:11.198746 extend_orfs_pyranges-0.1.3/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      340 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.3/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.3/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      868 2023-07-26 13:52:11.198746 extend_orfs_pyranges-0.1.3/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.3/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 13:52:11.194746 extend_orfs_pyranges-0.1.3/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 13:52:11.198746 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       80 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-26 13:50:53.000000 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    23390 2023-07-26 13:18:05.000000 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges/extend_orfs_pyranges.bkp.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    25615 2023-07-26 13:50:40.000000 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges/extend_orfs_pyranges.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 13:52:11.198746 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-26 13:52:11.000000 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      458 2023-07-26 13:52:11.000000 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-26 13:52:11.000000 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       63 2023-07-26 13:52:11.000000 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       21 2023-07-26 13:52:11.000000 extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      340 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.4/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.4/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      868 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.4/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       80 2023-07-26 09:48:18.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-07-26 14:29:21.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    23390 2023-07-26 13:18:05.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/extend_orfs_pyranges.bkp.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)    25675 2023-07-26 14:27:22.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/extend_orfs_pyranges.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-07-26 14:29:52.983874 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      800 2023-07-26 14:29:52.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      458 2023-07-26 14:29:52.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-07-26 14:29:52.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       63 2023-07-26 14:29:52.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       21 2023-07-26 14:29:52.000000 extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/top_level.txt
```

### Comparing `extend_orfs_pyranges-0.1.3/PKG-INFO` & `extend_orfs_pyranges-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extend_orfs_pyranges
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fork of Joan Pallares extend_orf based on pyranges
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti and Joan Pallares
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `extend_orfs_pyranges-0.1.3/setup.cfg` & `extend_orfs_pyranges-0.1.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges/extend_orfs_pyranges.bkp.py` & `extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/extend_orfs_pyranges.bkp.py`

 * *Files identical despite different names*

### Comparing `extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges/extend_orfs_pyranges.py` & `extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges/extend_orfs_pyranges.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,16 @@
     found.
     eel_usp is the largest extension possible when the pattern was found.
     usp corrects the extension to the position where the pattern was found.
     If no pattern is found and default_full is True, extend as much as possible
     up to the edge of the chromosome.
     If no pattern is found and default_full is False, no extension is performed.
     """
-
+    # MM # input is a DataFrame
+    
     # Upstream Start Position
     usp = int(df['up_start_pos'].values)
 
     # Effective_Extension_Length of Upstream Start Position
     eel_usp = int(df['EEL_of_up_start_pos'].values)
 
     # Iteration of Upstream Start Position
@@ -502,18 +503,20 @@
 def downstream_filler(df, dictionary, chunk_size, ic): 
     """
     If no pattern has been found for a given range (i.e. pattern_position == -1)
     returns the Extension corresponding to the Full Sequence or the longest one
     possible multiple of 3.
     If a pattern has been found, return the corresponding extension.
     """
+    # MM # input is a SERIES
 
+    
     if df['down_stop_pos'] == -1:
         if df['Strand'] == '+': 
-            extension = dictionary[df['True_Chromosome'].values[0]] - df['Initial_End']
+            extension = dictionary[df['True_Chromosome']] - df['Initial_End']
             return extension - extension % 3
 
         elif df['Strand'] == '-':
             extension = df['Initial_Start']
             return extension - extension % 3 
 
     else:
```

### Comparing `extend_orfs_pyranges-0.1.3/src/extend_orfs_pyranges.egg-info/PKG-INFO` & `extend_orfs_pyranges-0.1.4/src/extend_orfs_pyranges.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extend-orfs-pyranges
-Version: 0.1.3
+Version: 0.1.4
 Summary: Fork of Joan Pallares extend_orf based on pyranges
 Home-page: https://github.com/pypa/sampleproject
 Author: Marco Mariotti and Joan Pallares
 Author-email: marco.mariotti@ub.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

