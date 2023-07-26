# Comparing `tmp/ohnlptk-xlang-python-0.0.1.tar.gz` & `tmp/ohnlptk-xlang-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohnlptk-xlang-python-0.0.1.tar", last modified: Mon Jul 17 15:32:51 2023, max compression
+gzip compressed data, was "ohnlptk-xlang-python-0.0.2.tar", last modified: Wed Jul 26 14:56:03 2023, max compression
```

## Comparing `ohnlptk-xlang-python-0.0.1.tar` & `ohnlptk-xlang-python-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:32:51.346955 ohnlptk-xlang-python-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 15:32:45.000000 ohnlptk-xlang-python-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-17 15:32:51.346955 ohnlptk-xlang-python-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-17 15:32:45.000000 ohnlptk-xlang-python-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:32:51.346955 ohnlptk-xlang-python-0.0.1/ohnlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:32:45.000000 ohnlptk-xlang-python-0.0.1/ohnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:32:51.346955 ohnlptk-xlang-python-0.0.1/ohnlp/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:32:45.000000 ohnlptk-xlang-python-0.0.1/ohnlp/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:32:51.346955 ohnlptk-xlang-python-0.0.1/ohnlp/toolkit/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:32:45.000000 ohnlptk-xlang-python-0.0.1/ohnlp/toolkit/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-07-17 15:32:45.000000 ohnlptk-xlang-python-0.0.1/ohnlp/toolkit/backbone/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-17 15:32:45.000000 ohnlptk-xlang-python-0.0.1/ohnlp/toolkit/backbone/backbone_module_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:32:51.346955 ohnlptk-xlang-python-0.0.1/ohnlptk_xlang_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-17 15:32:51.000000 ohnlptk-xlang-python-0.0.1/ohnlptk_xlang_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-17 15:32:51.000000 ohnlptk-xlang-python-0.0.1/ohnlptk_xlang_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:32:51.000000 ohnlptk-xlang-python-0.0.1/ohnlptk_xlang_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-17 15:32:51.000000 ohnlptk-xlang-python-0.0.1/ohnlptk_xlang_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 15:32:51.000000 ohnlptk-xlang-python-0.0.1/ohnlptk_xlang_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:32:51.346955 ohnlptk-xlang-python-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-17 15:32:45.000000 ohnlptk-xlang-python-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/ohnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/ohnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/backbone_module_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 14:56:03.000000 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 14:56:03.000000 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:56:03.000000 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 14:56:03.000000 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 14:56:03.000000 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/setup.py
```

### Comparing `ohnlptk-xlang-python-0.0.1/LICENSE` & `ohnlptk-xlang-python-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ohnlptk-xlang-python-0.0.1/README.md` & `ohnlptk-xlang-python-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ohnlptk-xlang-python-0.0.1/ohnlp/toolkit/backbone/api.py` & `ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,21 @@
 
     def get_fields(self) -> Union[List[SchemaField], JavaClass]:
         return ListConverter().convert(self._fields, self._gateway._gateway_client)
 
     def get_field(self, name: str) -> SchemaField:
         return self._fields_by_name[name]
 
+    def toString(self):
+        ret: list[str] = []
+        ret.append('Fields: ')
+        for field in self._fields:
+            ret.append('- ' + field.get_name() + ', ' + field.get_field_type().get_type_name())
+        return '\r\n'.join(ret)
+
     class Java:
         implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonSchema"]
 
 
 class Row(object):
     def __init__(self, schema: Schema, values: List[object]):
         self._schema: Schema = schema
@@ -105,14 +112,24 @@
     def set_value(self, field_name: str, value: object):
         index = self.get_field_index(field_name)
         if index is not None:
             self._values[index] = value
         else:
             raise KeyError("Reference to non-existent field_name " + field_name + " in set_value")
 
+    def toString(self):
+        ret: list[str] = []
+        ret.append('Schema: ' + self._schema.toString())
+        ret.append('Values: ')
+        for value in self.get_values():
+            ret.append('- ' + str(value))
+        return '\r\n'.join(ret)
+
+
+
     class Java:
         implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonRow"]
 
 
 class TaggedRow(object):
     def __init__(self, tag: str, row: Row):
         self._tag: str = tag
```

### Comparing `ohnlptk-xlang-python-0.0.1/ohnlp/toolkit/backbone/backbone_module_launcher.py` & `ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/backbone_module_launcher.py`

 * *Files identical despite different names*

