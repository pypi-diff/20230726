# Comparing `tmp/klarf-reader-0.3.5.tar.gz` & `tmp/klarf-reader-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarf-reader-0.3.5.tar", last modified: Wed Jul 19 12:17:45 2023, max compression
+gzip compressed data, was "klarf-reader-0.3.6.tar", last modified: Wed Jul 26 14:48:59 2023, max compression
```

## Comparing `klarf-reader-0.3.5.tar` & `klarf-reader-0.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 12:17:45.611900 klarf-reader-0.3.5/
--rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0      569 2023-07-19 12:17:45.610902 klarf-reader-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-19 12:17:45.563455 klarf-reader-0.3.5/klarf_reader/
--rw-rw-rw-   0        0        0     1060 2023-06-27 07:08:50.000000 klarf-reader-0.3.5/klarf_reader/klarf.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:17:45.591902 klarf-reader-0.3.5/klarf_reader/models/
--rw-rw-rw-   0        0        0     2472 2023-06-27 08:18:10.000000 klarf-reader-0.3.5/klarf_reader/models/klarf_content.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:17:45.596933 klarf-reader-0.3.5/klarf_reader/readers/
--rw-rw-rw-   0        0        0    14064 2023-07-19 11:18:23.000000 klarf-reader-0.3.5/klarf_reader/readers/klarf_file_reader.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:17:45.601347 klarf-reader-0.3.5/klarf_reader/utils/
--rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.5/klarf_reader/utils/klarf_convert.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:17:45.588003 klarf-reader-0.3.5/klarf_reader.egg-info/
--rw-rw-rw-   0        0        0      569 2023-07-19 12:17:45.000000 klarf-reader-0.3.5/klarf_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2023-07-19 12:17:45.000000 klarf-reader-0.3.5/klarf_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 12:17:45.000000 klarf-reader-0.3.5/klarf_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-19 12:17:45.000000 klarf-reader-0.3.5/klarf_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-19 12:17:45.000000 klarf-reader-0.3.5/klarf_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-19 12:17:45.612900 klarf-reader-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      842 2023-07-19 12:17:08.000000 klarf-reader-0.3.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 12:17:45.606636 klarf-reader-0.3.5/tests/
--rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.5/tests/test_klarf.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:59.013451 klarf-reader-0.3.6/
+-rw-rw-rw-   0        0        0     1077 2023-01-23 09:00:52.000000 klarf-reader-0.3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      569 2023-07-26 14:48:59.010454 klarf-reader-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2023-03-30 07:40:20.000000 klarf-reader-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:58.965584 klarf-reader-0.3.6/klarf_reader/
+-rw-rw-rw-   0        0        0     1060 2023-06-27 07:08:50.000000 klarf-reader-0.3.6/klarf_reader/klarf.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:58.992879 klarf-reader-0.3.6/klarf_reader/models/
+-rw-rw-rw-   0        0        0     2472 2023-06-27 08:18:10.000000 klarf-reader-0.3.6/klarf_reader/models/klarf_content.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:58.997879 klarf-reader-0.3.6/klarf_reader/readers/
+-rw-rw-rw-   0        0        0    14081 2023-07-26 14:47:02.000000 klarf-reader-0.3.6/klarf_reader/readers/klarf_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:59.001597 klarf-reader-0.3.6/klarf_reader/utils/
+-rw-rw-rw-   0        0        0     1507 2023-06-27 07:19:15.000000 klarf-reader-0.3.6/klarf_reader/utils/klarf_convert.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:58.988159 klarf-reader-0.3.6/klarf_reader.egg-info/
+-rw-rw-rw-   0        0        0      569 2023-07-26 14:48:58.000000 klarf-reader-0.3.6/klarf_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2023-07-26 14:48:58.000000 klarf-reader-0.3.6/klarf_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 14:48:58.000000 klarf-reader-0.3.6/klarf_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 14:48:58.000000 klarf-reader-0.3.6/klarf_reader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-26 14:48:58.000000 klarf-reader-0.3.6/klarf_reader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-26 14:48:59.014217 klarf-reader-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0      842 2023-07-26 14:47:36.000000 klarf-reader-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 14:48:59.005601 klarf-reader-0.3.6/tests/
+-rw-rw-rw-   0        0        0     4195 2023-06-27 07:43:51.000000 klarf-reader-0.3.6/tests/test_klarf.py
```

### Comparing `klarf-reader-0.3.5/LICENSE.txt` & `klarf-reader-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.5/PKG-INFO` & `klarf-reader-0.3.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.5
+Version: 0.3.6
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.5.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.5/README.md` & `klarf-reader-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.5/klarf_reader/klarf.py` & `klarf-reader-0.3.6/klarf_reader/klarf.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.5/klarf_reader/models/klarf_content.py` & `klarf-reader-0.3.6/klarf_reader/models/klarf_content.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.5/klarf_reader/readers/klarf_file_reader.py` & `klarf-reader-0.3.6/klarf_reader/readers/klarf_file_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         "CLUSTERNUMBER",
         "ROUGHBINNUMBER",
         "FINEBINNUMBER",
         "IMAGECOUNT",
     ]
 
     setup_id = "no_setup"
+    sample_type = None
     next_line_has_coords, next_line_has_numb = False, False
     has_sample_test_plan, next_line_has_sample_test_plan = False, False
     sample_plan_test_x, sample_plan_test_y = [], []
     wafers: List[Wafer] = []
     tests: List[Test] = []
 
     if custom_columns_wafer is None:
@@ -227,20 +228,20 @@
                 column: parameters.index(column) - 1
                 for column in custom_columns_defect
                 if column in parameters
             }
 
             continue
 
-        if line.lstrip().lower().startswith("defectlist") and not (
-            line.rstrip().endswith(";")
-        ):
+        if line.lstrip().lower().startswith("defectlist"):
             next_line_has_coords = True
             defects = []
-            continue
+
+            if not line.rstrip().endswith(";"):
+                continue
 
         if next_line_has_coords:
             if line.startswith(" "):
                 defect_parameters = line.strip().split(";")[0].split()
 
                 defect_paramters_values = {
                     k.lower(): defect_parameters[v - 1]
```

### Comparing `klarf-reader-0.3.5/klarf_reader/utils/klarf_convert.py` & `klarf-reader-0.3.6/klarf_reader/utils/klarf_convert.py`

 * *Files identical despite different names*

### Comparing `klarf-reader-0.3.5/klarf_reader.egg-info/PKG-INFO` & `klarf-reader-0.3.6/klarf_reader.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: klarf-reader
-Version: 0.3.5
+Version: 0.3.6
 Summary: A project to parse klarf file and get klarf content as dataclass
 Home-page: https://github.com/Impro02/klarf_reader
-Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.5.tar.gz
+Download-URL: https://github.com/Impro02/klarf_reader/archive/refs/tags/0.3.6.tar.gz
 Author: Maxime MARTIN
 Author-email: maxime.martin02@hotmail.fr
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `klarf-reader-0.3.5/setup.py` & `klarf-reader-0.3.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = "0.3.5"
+version = "0.3.6"
 
 setup(
     name="klarf-reader",
     version=version,
     packages=[
         "klarf_reader",
         "klarf_reader.models",
```

### Comparing `klarf-reader-0.3.5/tests/test_klarf.py` & `klarf-reader-0.3.6/tests/test_klarf.py`

 * *Files identical despite different names*

