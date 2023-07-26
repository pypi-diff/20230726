# Comparing `tmp/cubo-2023.7.0.tar.gz` & `tmp/cubo-2023.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubo-2023.7.0.tar", last modified: Sun Jul  9 12:42:25 2023, max compression
+gzip compressed data, was "cubo-2023.7.1.tar", last modified: Wed Jul 26 14:25:17 2023, max compression
```

## Comparing `cubo-2023.7.0.tar` & `cubo-2023.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 12:42:25.384298 cubo-2023.7.0/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 12:31:14.000000 cubo-2023.7.0/LICENSE
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7699 2023-07-09 12:42:25.384298 cubo-2023.7.0/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7050 2023-07-09 12:31:14.000000 cubo-2023.7.0/README.md
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 12:42:25.380965 cubo-2023.7.0/cubo/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      178 2023-07-09 12:33:10.000000 cubo-2023.7.0/cubo/__init__.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4004 2023-07-09 12:31:14.000000 cubo-2023.7.0/cubo/cubo.py
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2401 2023-07-09 12:31:14.000000 cubo-2023.7.0/cubo/utils.py
-drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-09 12:42:25.384298 cubo-2023.7.0/cubo.egg-info/
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7699 2023-07-09 12:42:25.000000 cubo-2023.7.0/cubo.egg-info/PKG-INFO
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      209 2023-07-09 12:42:25.000000 cubo-2023.7.0/cubo.egg-info/SOURCES.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-09 12:42:25.000000 cubo-2023.7.0/cubo.egg-info/dependency_links.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)      110 2023-07-09 12:42:25.000000 cubo-2023.7.0/cubo.egg-info/requires.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)        5 2023-07-09 12:42:25.000000 cubo-2023.7.0/cubo.egg-info/top_level.txt
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-09 12:42:25.384298 cubo-2023.7.0/setup.cfg
--rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1340 2023-07-09 12:31:42.000000 cubo-2023.7.0/setup.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 14:25:17.367131 cubo-2023.7.1/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1077 2023-07-09 12:31:14.000000 cubo-2023.7.1/LICENSE
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7679 2023-07-26 14:25:17.367131 cubo-2023.7.1/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7050 2023-07-09 12:31:14.000000 cubo-2023.7.1/README.md
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 14:25:17.363797 cubo-2023.7.1/cubo/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      178 2023-07-26 14:11:23.000000 cubo-2023.7.1/cubo/__init__.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     4006 2023-07-26 14:05:48.000000 cubo-2023.7.1/cubo/cubo.py
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     2401 2023-07-09 12:31:14.000000 cubo-2023.7.1/cubo/utils.py
+drwxr-xr-x   0 dmontero  (1001) dmontero  (1001)        0 2023-07-26 14:25:17.363797 cubo-2023.7.1/cubo.egg-info/
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     7679 2023-07-26 14:25:17.000000 cubo-2023.7.1/cubo.egg-info/PKG-INFO
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      209 2023-07-26 14:25:17.000000 cubo-2023.7.1/cubo.egg-info/SOURCES.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        1 2023-07-26 14:25:17.000000 cubo-2023.7.1/cubo.egg-info/dependency_links.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)      110 2023-07-26 14:25:17.000000 cubo-2023.7.1/cubo.egg-info/requires.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)        5 2023-07-26 14:25:17.000000 cubo-2023.7.1/cubo.egg-info/top_level.txt
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)       38 2023-07-26 14:25:17.367131 cubo-2023.7.1/setup.cfg
+-rw-r--r--   0 dmontero  (1001) dmontero  (1001)     1340 2023-07-26 14:11:30.000000 cubo-2023.7.1/setup.py
```

### Comparing `cubo-2023.7.0/LICENSE` & `cubo-2023.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cubo-2023.7.0/PKG-INFO` & `cubo-2023.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubo
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Easily create EO mini cubes from STAC in Python
 Home-page: https://github.com/davemlz/cubo
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -200,9 +199,7 @@
 The project is licensed under the MIT license.
 
 ## Logo Attribution
 
 The logo and images were created using <a href="https://www.flaticon.com/free-icons/dice" title="dice icons">dice icons created by Freepik - Flaticon</a>.
 
 [![RSC4Earth](https://github.com/davemlz/cubo/raw/main/docs/_static/esds.png)](https://rsc4earth.de/authors/esds/)
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: cubo Version: 2023.7.0 Summary: Easily create EO
+Metadata-Version: 2.1 Name: cubo Version: 2023.7.1 Summary: Easily create EO
 mini cubes from STAC in Python Home-page: https://github.com/davemlz/cubo
 Author: David Montero Loaiza Author-email: dml.mont@gmail.com License: MIT
-Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
-text/markdown License-File: LICENSE
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
+License-File: LICENSE
                                     [cubo]
                 Easily create EO mini cubes from STAC in Python
 [PyPI] [conda-forge] [Documentation_Status] [Tests] [License] [GitHub_Sponsors]
               [Buy_me_a_coffee] [Ko-fi] [Twitter] [Black] [isort]
 --- **GitHub**: [https://github.com/davemlz/cubo](https://github.com/davemlz/
 cubo) **Documentation**: [https://cubo.readthedocs.io/](https://
 cubo.readthedocs.io/) **PyPI**: [https://pypi.org/project/cubo/](https://
```

### Comparing `cubo-2023.7.0/README.md` & `cubo-2023.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cubo-2023.7.0/cubo/cubo.py` & `cubo-2023.7.1/cubo/cubo.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         intersects=bbox_latlon,
         datetime=f"{start_date}/{end_date}",
         collections=[collection],
         **kwargs,
     )
 
     # Get all items and sign if using Planetary Computer
-    items = SEARCH.get_all_items()
+    items = SEARCH.item_collection()
 
     if stac == "https://planetarycomputer.microsoft.com/api/stac/v1":
         items = pc.sign(items)
 
     # Put the bands into list if not a list already
     if not isinstance(bands, list) and bands is not None:
         bands = [bands]
```

### Comparing `cubo-2023.7.0/cubo/utils.py` & `cubo-2023.7.1/cubo/utils.py`

 * *Files identical despite different names*

### Comparing `cubo-2023.7.0/cubo.egg-info/PKG-INFO` & `cubo-2023.7.1/cubo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubo
-Version: 2023.7.0
+Version: 2023.7.1
 Summary: Easily create EO mini cubes from STAC in Python
 Home-page: https://github.com/davemlz/cubo
 Author: David Montero Loaiza
 Author-email: dml.mont@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -200,9 +199,7 @@
 The project is licensed under the MIT license.
 
 ## Logo Attribution
 
 The logo and images were created using <a href="https://www.flaticon.com/free-icons/dice" title="dice icons">dice icons created by Freepik - Flaticon</a>.
 
 [![RSC4Earth](https://github.com/davemlz/cubo/raw/main/docs/_static/esds.png)](https://rsc4earth.de/authors/esds/)
-
-
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: cubo Version: 2023.7.0 Summary: Easily create EO
+Metadata-Version: 2.1 Name: cubo Version: 2023.7.1 Summary: Easily create EO
 mini cubes from STAC in Python Home-page: https://github.com/davemlz/cubo
 Author: David Montero Loaiza Author-email: dml.mont@gmail.com License: MIT
-Platform: UNKNOWN Classifier: Development Status :: 2 - Pre-Alpha Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
-text/markdown License-File: LICENSE
+Classifier: Development Status :: 2 - Pre-Alpha Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Description-Content-Type: text/markdown
+License-File: LICENSE
                                     [cubo]
                 Easily create EO mini cubes from STAC in Python
 [PyPI] [conda-forge] [Documentation_Status] [Tests] [License] [GitHub_Sponsors]
               [Buy_me_a_coffee] [Ko-fi] [Twitter] [Black] [isort]
 --- **GitHub**: [https://github.com/davemlz/cubo](https://github.com/davemlz/
 cubo) **Documentation**: [https://cubo.readthedocs.io/](https://
 cubo.readthedocs.io/) **PyPI**: [https://pypi.org/project/cubo/](https://
```

### Comparing `cubo-2023.7.0/setup.py` & `cubo-2023.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding="utf-8") as fd:
         return re.sub(text_type(r":[a-z]+:`~?(.*?)`"), text_type(r"``\1``"), fd.read())
 
 
 setup(
     name="cubo",
-    version="2023.7.0",
+    version="2023.7.1",
     url="https://github.com/davemlz/cubo",
     license="MIT",
     author="David Montero Loaiza",
     author_email="dml.mont@gmail.com",
     description="Easily create EO mini cubes from STAC in Python",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
```

