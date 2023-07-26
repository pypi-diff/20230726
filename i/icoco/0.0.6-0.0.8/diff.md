# Comparing `tmp/icoco-0.0.6.tar.gz` & `tmp/icoco-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/volatile/catA/rl222169/C3PO/ICoCo-python/dist/tmp82o27q3b/icoco-0.0.6.tar", last modified: Thu Mar  9 08:14:26 2023, max compression
+gzip compressed data, was "/volatile/catA/rl222169/softs/icoco/ICoCo-python/dist/tmp048z4m_5/icoco-0.0.8.tar", last modified: Wed Jul 26 09:33:09 2023, max compression
```

## Comparing `icoco-0.0.6.tar` & `icoco-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-03-09 08:14:26.000000 icoco-0.0.6/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2259 2023-03-09 08:14:26.000000 icoco-0.0.6/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       82 2023-03-08 15:19:46.000000 icoco-0.0.6/pyproject.toml
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-03-09 08:14:26.000000 icoco-0.0.6/setup.cfg
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-03-08 15:19:46.000000 icoco-0.0.6/MANIFEST.in
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1874 2023-03-08 15:19:46.000000 icoco-0.0.6/README.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     8664 2023-03-08 15:19:46.000000 icoco-0.0.6/setup.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-03-09 08:14:26.000000 icoco-0.0.6/src/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1135 2023-03-08 15:19:46.000000 icoco-0.0.6/src/README.md
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-03-09 08:14:26.000000 icoco-0.0.6/src/icoco/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-03-09 08:13:11.000000 icoco-0.0.6/src/icoco/VERSION
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      957 2023-03-08 15:21:15.000000 icoco-0.0.6/src/icoco/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1674 2023-03-08 15:19:46.000000 icoco-0.0.6/src/icoco/utils.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    44923 2023-03-08 15:19:46.000000 icoco-0.0.6/src/icoco/problem.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    63507 2023-03-09 08:09:44.000000 icoco-0.0.6/src/icoco/problem_wrapper.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2831 2023-03-08 15:19:46.000000 icoco-0.0.6/src/icoco/exception.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-03-09 08:14:26.000000 icoco-0.0.6/src/icoco.egg-info/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-03-09 08:14:26.000000 icoco-0.0.6/src/icoco.egg-info/top_level.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      363 2023-03-09 08:14:26.000000 icoco-0.0.6/src/icoco.egg-info/SOURCES.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2259 2023-03-09 08:14:26.000000 icoco-0.0.6/src/icoco.egg-info/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-03-09 08:14:26.000000 icoco-0.0.6/src/icoco.egg-info/dependency_links.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      224 2023-03-09 08:14:26.000000 icoco-0.0.6/src/icoco.egg-info/requires.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-03-08 15:19:46.000000 icoco-0.0.6/LICENSE
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-07-26 09:33:09.000000 icoco-0.0.8/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-07-26 09:33:09.000000 icoco-0.0.8/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-07-26 09:33:09.000000 icoco-0.0.8/src/icoco.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2259 2023-07-26 09:33:09.000000 icoco-0.0.8/src/icoco.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      391 2023-07-26 09:33:09.000000 icoco-0.0.8/src/icoco.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      224 2023-07-26 09:33:09.000000 icoco-0.0.8/src/icoco.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-07-26 09:33:09.000000 icoco-0.0.8/src/icoco.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-07-26 09:33:09.000000 icoco-0.0.8/src/icoco.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1135 2023-07-25 08:05:37.000000 icoco-0.0.8/src/README.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-07-26 09:33:09.000000 icoco-0.0.8/src/icoco/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    63507 2023-07-25 08:05:37.000000 icoco-0.0.8/src/icoco/problem_wrapper.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-07-26 09:31:40.000000 icoco-0.0.8/src/icoco/VERSION
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3433 2023-07-25 13:26:35.000000 icoco-0.0.8/src/icoco/utils.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1028 2023-07-25 13:17:48.000000 icoco-0.0.8/src/icoco/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    45155 2023-07-25 14:25:14.000000 icoco-0.0.8/src/icoco/problem.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2831 2023-07-25 08:05:37.000000 icoco-0.0.8/src/icoco/exception.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2569 2023-07-25 14:32:03.000000 icoco-0.0.8/src/icoco/problem_server.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       82 2023-07-25 08:05:37.000000 icoco-0.0.8/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     8664 2023-07-25 08:05:37.000000 icoco-0.0.8/setup.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1874 2023-07-25 08:05:37.000000 icoco-0.0.8/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-07-25 08:05:37.000000 icoco-0.0.8/LICENSE
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-07-26 09:33:09.000000 icoco-0.0.8/setup.cfg
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2259 2023-07-26 09:33:09.000000 icoco-0.0.8/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-07-25 08:05:37.000000 icoco-0.0.8/MANIFEST.in
```

### Comparing `icoco-0.0.6/PKG-INFO` & `icoco-0.0.8/src/icoco.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: icoco
-Version: 0.0.6
+Version: 0.0.8
 Summary: ICoCo Python implementation
-Home-page: https://github.com/roland-lenain/ICoCo-python
+Home-page: https://github.com/code-coupling/ICoCo-python
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/roland-lenain/ICoCo-python/issues
+Project-URL: Bug Reports, https://github.com/code-coupling/ICoCo-python/issues
 Project-URL: Doc, https://icoco-python.readthedocs.io/en/latest/index.html
-Project-URL: Source, https://github.com/roland-lenain/ICoCo-python
+Project-URL: Source, https://github.com/code-coupling/ICoCo-python
 Keywords: couping,medcoupling,salome,c3po
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `icoco-0.0.6/README.md` & `icoco-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `icoco-0.0.6/setup.py` & `icoco-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     # This field corresponds to the "Description-Content-Type" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     # This should be a valid link to your project's main homepage.
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
-    url="https://github.com/roland-lenain/ICoCo-python",  # Optional
+    url="https://github.com/code-coupling/ICoCo-python",  # Optional
     # This should be your name or the name of the organization which owns the
     # project.
     author="R. Lenain",  # Optional
     # This should be a valid email address corresponding to the author listed
     # above.
     author_email="roland.lenain@cea.fr",  # Optional
     # Classifiers help users find your project by categorizing it.
@@ -180,12 +180,12 @@
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     #
     # Examples listed include a pattern for specifying where the package tracks
     # issues, where the source is hosted, where to say thanks to the package
     # maintainers, and where to support the project financially. The key is
     # what's used to render the link text on PyPI.
     project_urls={  # Optional
-        "Bug Reports": "https://github.com/roland-lenain/ICoCo-python/issues",
+        "Bug Reports": "https://github.com/code-coupling/ICoCo-python/issues",
         "Doc": "https://icoco-python.readthedocs.io/en/latest/index.html",
-        "Source": "https://github.com/roland-lenain/ICoCo-python",
+        "Source": "https://github.com/code-coupling/ICoCo-python",
     },
 )
```

### Comparing `icoco-0.0.6/src/README.md` & `icoco-0.0.8/src/README.md`

 * *Files identical despite different names*

### Comparing `icoco-0.0.6/src/icoco/__init__.py` & `icoco-0.0.8/src/icoco/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,9 +22,10 @@
 __author__ = 'CEA'
 
 from .utils import (ICOCO_VERSION, ICOCO_MAJOR_VERSION, ICOCO_MINOR_VERSION,  # noqa: F401
                     ValueType, medcoupling)  # noqa: F401
 
 from .exception import WrongContext, WrongArgument, NotImplementedMethod  # noqa: F401
 
+from .problem_server import ProblemClient, ServerManager  # noqa: F401
 from .problem_wrapper import ProblemWrapper  # noqa: F401
 from .problem import Problem  # noqa: F401
```

### Comparing `icoco-0.0.6/src/icoco/problem.py` & `icoco-0.0.8/src/icoco/problem.py`

 * *Files 2% similar despite different names*

```diff
@@ -515,14 +515,18 @@
         WrongContext
             exception if called before initialize() or after terminate().
         WrongArgument
             exception if the method or label argument is invalid.
         """
         raise NotImplementedMethod(prob=self.problem_name, method="forget")
 
+    # ******************************************************
+    # section Field I/O.
+    # Reminder: all methods are **optional** not all of them need to be implemented!
+    # ******************************************************
     def getInputFieldsNames(self) -> List[str]:
         """(Optional) Get the list of input fields accepted by the code.
 
         Returns
         -------
         List[str]
             the list of field names that represent inputs of the code
```

### Comparing `icoco-0.0.6/src/icoco/problem_wrapper.py` & `icoco-0.0.8/src/icoco/problem_wrapper.py`

 * *Files identical despite different names*

### Comparing `icoco-0.0.6/src/icoco/exception.py` & `icoco-0.0.8/src/icoco/exception.py`

 * *Files identical despite different names*

### Comparing `icoco-0.0.6/src/icoco.egg-info/PKG-INFO` & `icoco-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: icoco
-Version: 0.0.6
+Version: 0.0.8
 Summary: ICoCo Python implementation
-Home-page: https://github.com/roland-lenain/ICoCo-python
+Home-page: https://github.com/code-coupling/ICoCo-python
 Author: R. Lenain
 Author-email: roland.lenain@cea.fr
 License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/roland-lenain/ICoCo-python/issues
+Project-URL: Bug Reports, https://github.com/code-coupling/ICoCo-python/issues
 Project-URL: Doc, https://icoco-python.readthedocs.io/en/latest/index.html
-Project-URL: Source, https://github.com/roland-lenain/ICoCo-python
+Project-URL: Source, https://github.com/code-coupling/ICoCo-python
 Keywords: couping,medcoupling,salome,c3po
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `icoco-0.0.6/LICENSE` & `icoco-0.0.8/LICENSE`

 * *Files identical despite different names*

