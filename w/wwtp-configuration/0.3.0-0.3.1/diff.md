# Comparing `tmp/wwtp-configuration-0.3.0.tar.gz` & `tmp/wwtp-configuration-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwtp-configuration-0.3.0.tar", last modified: Thu Jul  6 03:55:22 2023, max compression
+gzip compressed data, was "wwtp-configuration-0.3.1.tar", last modified: Wed Jul 26 00:54:59 2023, max compression
```

## Comparing `wwtp-configuration-0.3.0.tar` & `wwtp-configuration-0.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:55:22.495190 wwtp-configuration-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-06 03:55:22.495190 wwtp-configuration-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:55:22.491190 wwtp-configuration-0.3.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/connection.rst
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/node.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/parse_json.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/tag.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/units.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/docs/visualize.rst
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-06 03:55:22.499190 wwtp-configuration-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:55:22.495190 wwtp-configuration-0.3.0/wwtp_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:55:22.495190 wwtp-configuration-0.3.0/wwtp_configuration/data/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/data/sample.json
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/data/unit_definitions.txt
--rw-r--r--   0 runner    (1001) docker     (123)    71289 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    44321 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/parse_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    28125 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-06 03:55:16.000000 wwtp-configuration-0.3.0/wwtp_configuration/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 03:55:22.495190 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 03:55:22.000000 wwtp-configuration-0.3.0/wwtp_configuration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:54:59.679244 wwtp-configuration-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35666 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-26 00:54:59.679244 wwtp-configuration-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:54:59.679244 wwtp-configuration-0.3.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/connection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/node.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/parse_json.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/tag.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/units.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/docs/visualize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-26 00:54:59.679244 wwtp-configuration-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:54:59.679244 wwtp-configuration-0.3.1/wwtp_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:54:59.679244 wwtp-configuration-0.3.1/wwtp_configuration/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/data/sample.json
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/data/unit_definitions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    71289 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44375 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/parse_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28176 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25351 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-07-26 00:54:54.000000 wwtp-configuration-0.3.1/wwtp_configuration/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:54:59.679244 wwtp-configuration-0.3.1/wwtp_configuration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-26 00:54:59.000000 wwtp-configuration-0.3.1/wwtp_configuration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-26 00:54:59.000000 wwtp-configuration-0.3.1/wwtp_configuration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:54:59.000000 wwtp-configuration-0.3.1/wwtp_configuration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:54:59.000000 wwtp-configuration-0.3.1/wwtp_configuration.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-07-26 00:54:59.000000 wwtp-configuration-0.3.1/wwtp_configuration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 00:54:59.000000 wwtp-configuration-0.3.1/wwtp_configuration.egg-info/top_level.txt
```

### Comparing `wwtp-configuration-0.3.0/CONTRIBUTING.rst` & `wwtp-configuration-0.3.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/LICENSE` & `wwtp-configuration-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/PKG-INFO` & `wwtp-configuration-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwtp-configuration
-Version: 0.3.0
+Version: 0.3.1
 Summary: Class hierarchy to represent a wastewater treatment plant's configuration.
 Home-page: https://github.com/we3lab/wwtp-configuration
 Author: WE3 Lab
 Author-email: fchapin@stanford.edu
 License: UNKNOWN
 Keywords: wwtp-configuration
 Platform: UNKNOWN
```

### Comparing `wwtp-configuration-0.3.0/README.rst` & `wwtp-configuration-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/docs/Makefile` & `wwtp-configuration-0.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/docs/conf.py` & `wwtp-configuration-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/docs/index.rst` & `wwtp-configuration-0.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/docs/make.bat` & `wwtp-configuration-0.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/setup.py` & `wwtp-configuration-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,10 +63,10 @@
     python_requires=">=3.9",
     install_requires=requirements,
     setup_requires=setup_requirements,
     tests_require=test_requirements,
     extras_require=extra_requirements,
     test_suite="tests",
     url="https://github.com/we3lab/wwtp-configuration",
-    version="0.3.0",
+    version="0.3.1",
     zip_safe=False,
 )
```

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration/connection.py` & `wwtp-configuration-0.3.1/wwtp_configuration/connection.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration/data/sample.json` & `wwtp-configuration-0.3.1/wwtp_configuration/data/sample.json`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration/node.py` & `wwtp-configuration-0.3.1/wwtp_configuration/node.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration/parse_json.py` & `wwtp-configuration-0.3.1/wwtp_configuration/parse_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -905,14 +905,15 @@
             `tag_obj` in dictionary form
         """
         tag_dict = {}
         if isinstance(tag_obj, VirtualTag):
             tag_dict["tags"] = [tag.id for tag in tag_obj.tags]
             tag_dict["unary_operations"] = tag_obj.unary_operations
             tag_dict["binary_operations"] = tag_obj.binary_operations
+            tag_dict["parent_id"] = tag_obj.parent_id
         elif isinstance(tag_obj, Tag):
             tag_dict["units"] = "{!s}".format(tag_obj.units)
             tag_dict["source_unit_id"] = tag_obj.source_unit_id
             tag_dict["dest_unit_id"] = tag_obj.dest_unit_id
             tag_dict["totalized"] = tag_obj.totalized
         else:
             raise TypeError("'tag_obj' must be of type Tag or VirtualTag")
```

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration/tag.py` & `wwtp-configuration-0.3.1/wwtp_configuration/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,15 @@
                 else:
                     prev_unit = unit
 
             self.binary_operations = [binary_operations] * (len(self.tags) - 1)
         else:
             if len(self.tags) != 1:
                 raise ValueError(
-                    "Binary operations must be specified"
+                    "Binary operations must be specified "
                     "when more than one tag is given."
                 )
             self.binary_operations = None
             prev_unit = units[0]
 
         self.units = prev_unit
 
@@ -469,14 +469,15 @@
             and self.contents == other.contents
             and self.tag_type == other.tag_type
             and self.totalized == other.totalized
             and self.units == other.units
             and self.tags == other.tags
             and self.unary_operations == other.unary_operations
             and self.binary_operations == other.binary_operations
+            and self.parent_id == other.parent_id
         )
 
     def __hash__(self):
         return hash(
             (
                 self.id,
                 str(self.tags),
```

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration/units.py` & `wwtp-configuration-0.3.1/wwtp_configuration/units.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration/utils.py` & `wwtp-configuration-0.3.1/wwtp_configuration/utils.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration/visualize.py` & `wwtp-configuration-0.3.1/wwtp_configuration/visualize.py`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration.egg-info/PKG-INFO` & `wwtp-configuration-0.3.1/wwtp_configuration.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwtp-configuration
-Version: 0.3.0
+Version: 0.3.1
 Summary: Class hierarchy to represent a wastewater treatment plant's configuration.
 Home-page: https://github.com/we3lab/wwtp-configuration
 Author: WE3 Lab
 Author-email: fchapin@stanford.edu
 License: UNKNOWN
 Keywords: wwtp-configuration
 Platform: UNKNOWN
```

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration.egg-info/SOURCES.txt` & `wwtp-configuration-0.3.1/wwtp_configuration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wwtp-configuration-0.3.0/wwtp_configuration.egg-info/requires.txt` & `wwtp-configuration-0.3.1/wwtp_configuration.egg-info/requires.txt`

 * *Files identical despite different names*

