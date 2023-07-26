# Comparing `tmp/ohnlptk-xlang-python-0.0.2.tar.gz` & `tmp/ohnlptk-xlang-python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohnlptk-xlang-python-0.0.2.tar", last modified: Wed Jul 26 14:56:03 2023, max compression
+gzip compressed data, was "ohnlptk-xlang-python-0.0.3.tar", last modified: Wed Jul 26 15:20:14 2023, max compression
```

## Comparing `ohnlptk-xlang-python-0.0.2.tar` & `ohnlptk-xlang-python-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/ohnlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/ohnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/backbone_module_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 14:56:03.000000 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 14:56:03.000000 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:56:03.000000 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 14:56:03.000000 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 14:56:03.000000 ohnlptk-xlang-python-0.0.2/ohnlptk_xlang_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:56:03.907098 ohnlptk-xlang-python-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-26 14:56:00.000000 ohnlptk-xlang-python-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/ohnlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/ohnlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/backbone_module_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-26 15:20:14.000000 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-26 15:20:14.000000 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 15:20:14.000000 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-26 15:20:14.000000 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-26 15:20:14.000000 ohnlptk-xlang-python-0.0.3/ohnlptk_xlang_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 15:20:14.501302 ohnlptk-xlang-python-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-26 15:20:08.000000 ohnlptk-xlang-python-0.0.3/setup.py
```

### Comparing `ohnlptk-xlang-python-0.0.2/LICENSE` & `ohnlptk-xlang-python-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ohnlptk-xlang-python-0.0.2/README.md` & `ohnlptk-xlang-python-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/api.py` & `ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,28 +103,28 @@
             return None
 
     def get_value(self, field_name: str) -> Union[object, None]:
         index = self.get_field_index(field_name)
         return None if index is None else self._values[index]
 
     def get_values(self) -> Union[List[object], JavaClass]:
-        return ListConverter().convert(self.get_values(), self.get_schema()._gateway._gateway_client)
+        return ListConverter().convert(self._values, self.get_schema()._gateway._gateway_client)
 
     def set_value(self, field_name: str, value: object):
         index = self.get_field_index(field_name)
         if index is not None:
             self._values[index] = value
         else:
             raise KeyError("Reference to non-existent field_name " + field_name + " in set_value")
 
     def toString(self):
         ret: list[str] = []
         ret.append('Schema: ' + self._schema.toString())
         ret.append('Values: ')
-        for value in self.get_values():
+        for value in self._values:
             ret.append('- ' + str(value))
         return '\r\n'.join(ret)
 
 
 
     class Java:
         implements = ["org.ohnlp.backbone.api.components.xlang.python.PythonRow"]
```

### Comparing `ohnlptk-xlang-python-0.0.2/ohnlp/toolkit/backbone/backbone_module_launcher.py` & `ohnlptk-xlang-python-0.0.3/ohnlp/toolkit/backbone/backbone_module_launcher.py`

 * *Files identical despite different names*

