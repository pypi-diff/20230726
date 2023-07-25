# Comparing `tmp/dsakit-2.0.0.tar.gz` & `tmp/dsakit-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsakit-2.0.0.tar", last modified: Tue Jul 25 22:43:22 2023, max compression
+gzip compressed data, was "dsakit-2.0.1.tar", last modified: Tue Jul 25 22:59:40 2023, max compression
```

## Comparing `dsakit-2.0.0.tar` & `dsakit-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 22:43:22.673865 dsakit-2.0.0/
--rw-rw-rw-   0        0        0     1088 2023-07-25 18:45:54.000000 dsakit-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     2483 2023-07-25 22:43:22.672865 dsakit-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1905 2023-07-25 22:29:47.000000 dsakit-2.0.0/README.md
--rw-rw-rw-   0        0        0      656 2023-07-25 22:43:02.000000 dsakit-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-25 22:43:22.673865 dsakit-2.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-25 22:43:22.659865 dsakit-2.0.0/src/
--rw-rw-rw-   0        0        0     3608 2023-07-25 21:05:00.000000 dsakit-2.0.0/src/BinaryTree.py
--rw-rw-rw-   0        0        0     5171 2023-07-25 20:57:00.000000 dsakit-2.0.0/src/LinkedList.py
--rw-rw-rw-   0        0        0     1609 2023-07-25 21:46:29.000000 dsakit-2.0.0/src/Trie.py
--rw-rw-rw-   0        0        0     1881 2023-07-25 21:45:36.000000 dsakit-2.0.0/src/UnionFind.py
--rw-rw-rw-   0        0        0       80 2023-07-25 21:17:24.000000 dsakit-2.0.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 22:43:22.671865 dsakit-2.0.0/src/dsakit.egg-info/
--rw-rw-rw-   0        0        0     2483 2023-07-25 22:43:22.000000 dsakit-2.0.0/src/dsakit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-25 22:43:22.000000 dsakit-2.0.0/src/dsakit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 22:43:22.000000 dsakit-2.0.0/src/dsakit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-07-25 22:43:22.000000 dsakit-2.0.0/src/dsakit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-25 22:59:40.074222 dsakit-2.0.1/
+-rw-rw-rw-   0        0        0     1088 2023-07-25 18:45:54.000000 dsakit-2.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2535 2023-07-25 22:59:40.073217 dsakit-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1957 2023-07-25 22:57:41.000000 dsakit-2.0.1/README.md
+-rw-rw-rw-   0        0        0      656 2023-07-25 22:58:59.000000 dsakit-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-25 22:59:40.074222 dsakit-2.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-25 22:59:40.055215 dsakit-2.0.1/src/
+-rw-rw-rw-   0        0        0     3608 2023-07-25 21:05:00.000000 dsakit-2.0.1/src/BinaryTree.py
+-rw-rw-rw-   0        0        0     5171 2023-07-25 20:57:00.000000 dsakit-2.0.1/src/LinkedList.py
+-rw-rw-rw-   0        0        0     1609 2023-07-25 21:46:29.000000 dsakit-2.0.1/src/Trie.py
+-rw-rw-rw-   0        0        0     1881 2023-07-25 21:45:36.000000 dsakit-2.0.1/src/UnionFind.py
+-rw-rw-rw-   0        0        0      101 2023-07-25 22:54:26.000000 dsakit-2.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 22:59:40.071217 dsakit-2.0.1/src/dsakit.egg-info/
+-rw-rw-rw-   0        0        0     2535 2023-07-25 22:59:40.000000 dsakit-2.0.1/src/dsakit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-25 22:59:40.000000 dsakit-2.0.1/src/dsakit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 22:59:40.000000 dsakit-2.0.1/src/dsakit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-07-25 22:59:40.000000 dsakit-2.0.1/src/dsakit.egg-info/top_level.txt
```

### Comparing `dsakit-2.0.0/LICENSE` & `dsakit-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsakit-2.0.0/PKG-INFO` & `dsakit-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsakit
-Version: 2.0.0
+Version: 2.0.1
 Summary: A package aimed at providing various data structures and their functions to solve dsa problems
 Author-email: Aayush65 <cdtaayushgupta@gmail.com>
 Project-URL: Homepage, https://github.com/Aayush65/DSAKit
 Project-URL: Bug Tracker, https://github.com/Aayush65/DSAKit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,8 +62,8 @@
 from BinaryTree import *
 from Trie import *
 from UnionFind import *
 ```
 
 ## License
 
-DSA Kit is open-source software released under the (MIT License)[]. Feel free to use it in your projects.
+DSA Kit is open-source software released under the [MIT License](https://github.com/Aayush65/DSAKit/blob/main/LICENSE). Feel free to use it in your projects.
```

### Comparing `dsakit-2.0.0/README.md` & `dsakit-2.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -48,8 +48,8 @@
 from BinaryTree import *
 from Trie import *
 from UnionFind import *
 ```
 
 ## License
 
-DSA Kit is open-source software released under the (MIT License)[]. Feel free to use it in your projects.
+DSA Kit is open-source software released under the [MIT License](https://github.com/Aayush65/DSAKit/blob/main/LICENSE). Feel free to use it in your projects.
```

### Comparing `dsakit-2.0.0/pyproject.toml` & `dsakit-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dsakit"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name="Aayush65", email="cdtaayushgupta@gmail.com" },
 ]
 description = "A package aimed at providing various data structures and their functions to solve dsa problems"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dsakit-2.0.0/src/BinaryTree.py` & `dsakit-2.0.1/src/BinaryTree.py`

 * *Files identical despite different names*

### Comparing `dsakit-2.0.0/src/LinkedList.py` & `dsakit-2.0.1/src/LinkedList.py`

 * *Files identical despite different names*

### Comparing `dsakit-2.0.0/src/Trie.py` & `dsakit-2.0.1/src/Trie.py`

 * *Files identical despite different names*

### Comparing `dsakit-2.0.0/src/UnionFind.py` & `dsakit-2.0.1/src/UnionFind.py`

 * *Files identical despite different names*

### Comparing `dsakit-2.0.0/src/dsakit.egg-info/PKG-INFO` & `dsakit-2.0.1/src/dsakit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsakit
-Version: 2.0.0
+Version: 2.0.1
 Summary: A package aimed at providing various data structures and their functions to solve dsa problems
 Author-email: Aayush65 <cdtaayushgupta@gmail.com>
 Project-URL: Homepage, https://github.com/Aayush65/DSAKit
 Project-URL: Bug Tracker, https://github.com/Aayush65/DSAKit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -62,8 +62,8 @@
 from BinaryTree import *
 from Trie import *
 from UnionFind import *
 ```
 
 ## License
 
-DSA Kit is open-source software released under the (MIT License)[]. Feel free to use it in your projects.
+DSA Kit is open-source software released under the [MIT License](https://github.com/Aayush65/DSAKit/blob/main/LICENSE). Feel free to use it in your projects.
```

