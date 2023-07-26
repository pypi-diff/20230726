# Comparing `tmp/LCPDelta-0.1.0.1.tar.gz` & `tmp/LCPDelta-0.1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LCPDelta-0.1.0.1.tar", last modified: Wed Jul 26 13:29:57 2023, max compression
+gzip compressed data, was "LCPDelta-0.1.0.2.tar", last modified: Wed Jul 26 14:00:34 2023, max compression
```

## Comparing `LCPDelta-0.1.0.1.tar` & `LCPDelta-0.1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 13:29:57.543709 LCPDelta-0.1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-16 15:59:44.000000 LCPDelta-0.1.0.1/LICENSE
--rw-rw-rw-   0        0        0      563 2023-07-26 13:29:57.542709 LCPDelta-0.1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       85 2023-06-16 15:59:46.000000 LCPDelta-0.1.0.1/README.md
--rw-rw-rw-   0        0        0      612 2023-07-25 16:30:15.000000 LCPDelta-0.1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-26 13:29:57.544709 LCPDelta-0.1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-26 13:29:57.480804 LCPDelta-0.1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-26 13:29:57.515708 LCPDelta-0.1.0.1/src/LCPDelta/
--rw-rw-rw-   0        0        0    34999 2023-07-26 11:08:30.000000 LCPDelta-0.1.0.1/src/LCPDelta/Enact.py
--rw-rw-rw-   0        0        0        0 2023-06-20 13:20:32.000000 LCPDelta-0.1.0.1/src/LCPDelta/FlexTrack.py
--rw-rw-rw-   0        0        0      314 2023-07-25 16:29:17.000000 LCPDelta-0.1.0.1/src/LCPDelta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 13:29:57.540805 LCPDelta-0.1.0.1/src/LCPDelta.egg-info/
--rw-rw-rw-   0        0        0      563 2023-07-26 13:29:57.000000 LCPDelta-0.1.0.1/src/LCPDelta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-07-26 13:29:57.000000 LCPDelta-0.1.0.1/src/LCPDelta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 13:29:57.000000 LCPDelta-0.1.0.1/src/LCPDelta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 13:29:57.000000 LCPDelta-0.1.0.1/src/LCPDelta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-26 13:29:57.000000 LCPDelta-0.1.0.1/src/LCPDelta.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 14:00:34.651956 LCPDelta-0.1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-16 15:59:44.000000 LCPDelta-0.1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      563 2023-07-26 14:00:34.650955 LCPDelta-0.1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       85 2023-06-16 15:59:46.000000 LCPDelta-0.1.0.2/README.md
+-rw-rw-rw-   0        0        0      632 2023-07-26 14:00:10.000000 LCPDelta-0.1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-26 14:00:34.651956 LCPDelta-0.1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 14:00:34.578435 LCPDelta-0.1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 14:00:34.618969 LCPDelta-0.1.0.2/src/LCPDelta/
+-rw-rw-rw-   0        0        0    34999 2023-07-26 11:08:30.000000 LCPDelta-0.1.0.2/src/LCPDelta/Enact.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 13:20:32.000000 LCPDelta-0.1.0.2/src/LCPDelta/FlexTrack.py
+-rw-rw-rw-   0        0        0      314 2023-07-25 16:29:17.000000 LCPDelta-0.1.0.2/src/LCPDelta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:00:34.648955 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/
+-rw-rw-rw-   0        0        0      563 2023-07-26 14:00:34.000000 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-07-26 14:00:34.000000 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 14:00:34.000000 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-07-26 14:00:34.000000 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-26 14:00:34.000000 LCPDelta-0.1.0.2/src/LCPDelta.egg-info/top_level.txt
```

### Comparing `LCPDelta-0.1.0.1/LICENSE` & `LCPDelta-0.1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LCPDelta-0.1.0.1/PKG-INFO` & `LCPDelta-0.1.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LCPDelta
-Version: 0.1.0.1
+Version: 0.1.0.2
 Summary: LCPDelta test package
 Author-email: Sushanth Kolluru <enact.helpdesk@lcp.uk.com>
 Project-URL: Homepage, https://enact.lcpdelta.com/
 Keywords: LCPDelta,Enact,Flextrack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `LCPDelta-0.1.0.1/pyproject.toml` & `LCPDelta-0.1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LCPDelta"
-version = "0.1.0.1"
+version = "0.1.0.2"
 authors = [
   { name="Sushanth Kolluru", email="enact.helpdesk@lcp.uk.com" },
 ]
 description = "LCPDelta test package"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["LCPDelta", "Enact", "Flextrack"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "requests"
+    "requests",
+    "signalrcore"
 ]
 [project.urls]
 "Homepage" = "https://enact.lcpdelta.com/"
```

### Comparing `LCPDelta-0.1.0.1/src/LCPDelta/Enact.py` & `LCPDelta-0.1.0.2/src/LCPDelta/Enact.py`

 * *Files identical despite different names*

### Comparing `LCPDelta-0.1.0.1/src/LCPDelta.egg-info/PKG-INFO` & `LCPDelta-0.1.0.2/src/LCPDelta.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LCPDelta
-Version: 0.1.0.1
+Version: 0.1.0.2
 Summary: LCPDelta test package
 Author-email: Sushanth Kolluru <enact.helpdesk@lcp.uk.com>
 Project-URL: Homepage, https://enact.lcpdelta.com/
 Keywords: LCPDelta,Enact,Flextrack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

