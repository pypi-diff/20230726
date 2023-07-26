# Comparing `tmp/codedjson-1.2.0.tar.gz` & `tmp/codedjson-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedjson-1.2.0.tar", last modified: Mon Jul 24 15:18:17 2023, max compression
+gzip compressed data, was "codedjson-1.3.2.tar", last modified: Wed Jul 26 16:42:34 2023, max compression
```

## Comparing `codedjson-1.2.0.tar` & `codedjson-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 15:18:17.409061 codedjson-1.2.0/
--rw-rw-rw-   0        0        0     1093 2023-06-30 14:35:27.000000 codedjson-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     3090 2023-07-24 15:18:17.408063 codedjson-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2213 2023-07-22 14:14:14.000000 codedjson-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-24 15:18:17.371629 codedjson-1.2.0/cjson/
-drwxrwxrwx   0        0        0        0 2023-07-24 15:18:17.387875 codedjson-1.2.0/cjson/src/
--rw-rw-rw-   0        0        0     6399 2023-07-22 14:14:43.000000 codedjson-1.2.0/cjson/src/cjson.py
-drwxrwxrwx   0        0        0        0 2023-07-24 15:18:17.386874 codedjson-1.2.0/cjson/src/codedjson.egg-info/
--rw-rw-rw-   0        0        0     3090 2023-07-24 15:18:17.000000 codedjson-1.2.0/cjson/src/codedjson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-07-24 15:18:17.000000 codedjson-1.2.0/cjson/src/codedjson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 15:18:17.000000 codedjson-1.2.0/cjson/src/codedjson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-24 15:18:17.000000 codedjson-1.2.0/cjson/src/codedjson.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-24 15:18:17.405062 codedjson-1.2.0/cjson/src/utils/
--rw-rw-rw-   0        0        0        0 2023-06-30 14:35:27.000000 codedjson-1.2.0/cjson/src/utils/__init__.py
--rw-rw-rw-   0        0        0      907 2023-06-30 14:35:27.000000 codedjson-1.2.0/cjson/src/utils/_is.py
--rw-rw-rw-   0        0        0     4491 2023-07-22 14:14:43.000000 codedjson-1.2.0/cjson/src/utils/_json.py
--rw-rw-rw-   0        0        0      204 2023-07-17 15:54:59.000000 codedjson-1.2.0/cjson/src/utils/file.py
--rw-rw-rw-   0        0        0      307 2023-07-22 14:14:43.000000 codedjson-1.2.0/cjson/src/utils/keywords.py
--rw-rw-rw-   0        0        0       42 2023-07-24 15:18:17.410064 codedjson-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1201 2023-07-22 14:14:43.000000 codedjson-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:42:34.760780 codedjson-1.3.2/
+-rw-rw-rw-   0        0        0     1093 2023-06-30 14:35:27.000000 codedjson-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     3090 2023-07-26 16:42:34.758778 codedjson-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2213 2023-07-22 14:14:14.000000 codedjson-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 16:42:34.725132 codedjson-1.3.2/cjson/
+drwxrwxrwx   0        0        0        0 2023-07-26 16:42:34.741777 codedjson-1.3.2/cjson/src/
+-rw-rw-rw-   0        0        0     7276 2023-07-26 15:29:24.000000 codedjson-1.3.2/cjson/src/cjson.py
+drwxrwxrwx   0        0        0        0 2023-07-26 16:42:34.739781 codedjson-1.3.2/cjson/src/codedjson.egg-info/
+-rw-rw-rw-   0        0        0     3090 2023-07-26 16:42:34.000000 codedjson-1.3.2/cjson/src/codedjson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      548 2023-07-26 16:42:34.000000 codedjson-1.3.2/cjson/src/codedjson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 16:42:34.000000 codedjson-1.3.2/cjson/src/codedjson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-26 16:42:34.000000 codedjson-1.3.2/cjson/src/codedjson.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 16:42:34.756780 codedjson-1.3.2/cjson/src/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-30 14:35:27.000000 codedjson-1.3.2/cjson/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      313 2023-07-26 15:29:24.000000 codedjson-1.3.2/cjson/src/utils/_exceptions.py
+-rw-rw-rw-   0        0        0      907 2023-06-30 14:35:27.000000 codedjson-1.3.2/cjson/src/utils/_is.py
+-rw-rw-rw-   0        0        0     4491 2023-07-22 14:14:43.000000 codedjson-1.3.2/cjson/src/utils/_json.py
+-rw-rw-rw-   0        0        0      359 2023-07-26 15:29:24.000000 codedjson-1.3.2/cjson/src/utils/file.py
+-rw-rw-rw-   0        0        0      307 2023-07-22 14:14:43.000000 codedjson-1.3.2/cjson/src/utils/keywords.py
+-rw-rw-rw-   0        0        0       42 2023-07-26 16:42:34.761777 codedjson-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1201 2023-07-26 15:29:24.000000 codedjson-1.3.2/setup.py
```

### Comparing `codedjson-1.2.0/LICENSE` & `codedjson-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codedjson-1.2.0/PKG-INFO` & `codedjson-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedjson
-Version: 1.2.0
+Version: 1.3.2
 Summary: CJSON is a data file format(inspired from JSON), but supports logical expressions too. Having extended language support to NodeJS, Python and Java, users has experienced data reusability. For features and examples, please refer to this documentation as base document.
 Author: Shubhendu Shekhar Gupta
 Author-email: subhendushekhargupta@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `codedjson-1.2.0/README.md` & `codedjson-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `codedjson-1.2.0/cjson/src/cjson.py` & `codedjson-1.3.2/cjson/src/cjson.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,49 @@
-from utils.file import read
+from utils.file import read, is_path_absolute
 from utils._is import Is
 from utils.keywords import Keywords
 from utils._json import Json, is_content_json as content_json_check
 from os import path
 import json, re
+from utils._exceptions import AbsolutePathConstraintError, FilePathAndCJSONCotentConflict
 
 def is_content_json(content: str, is_file_path: bool = False):
         ''' Checks if the parsed content is JSON
         '''
         return content_json_check(content, is_file_path=is_file_path)
 
 class Cjson(Is):
     __obj:any
     __file_path: str
     __content: str = ""
+    __is_content_cjson: bool = False
     json: Json | None = None
 
-    def __init__(self, file_path: str):
+    def __init__(self, content: str, is_content_cjson: bool = False):
         ''' Initializes and decodes `CJSON` files.
 
             This can also be used for parsing JSON files in `CJSON` way.
+
+            `content` can be file path and cjson/json type string.
+
             Parsing in CJSON way unlocks many functions. For more details, see function documentation.
+
         '''
         super().__init__()
         self.__obj = None
-        self.__file_path = file_path
-        self.__content = read(self.__file_path)
+
+        if(is_path_absolute(content) and is_content_cjson):
+            raise FilePathAndCJSONCotentConflict()
+        elif is_content_cjson == True:
+            self.__is_content_cjson = is_content_cjson
+            self.__content = content
+            self.__file_path = None
+        else:
+            self.__file_path = content
+            self.__content = read(self.__file_path)
     
     def __decode_keywords(self):
         is_changed: bool = False
         while(True):
             is_changed = False
 
             if self._is_import(self.__content):
@@ -100,17 +114,26 @@
         ''' Returns the JSON compiled object for the given `CJSON` file. '''
         return self.__obj
     
     def __get_file_path(self, line_item: str):
         return line_item.split(Keywords.import_key)[1].split("\"")[0]
 
     def __decode_import(self, line_item: str):
+        global import_file_path
+        
         file_path: str = self.__get_file_path(line_item=line_item)
-        dir_name: str = path.dirname(path.abspath(self.__file_path))
-        import_file_path: str = path.join(dir_name, file_path)
+
+        if(is_path_absolute(file_path=file_path)):
+            import_file_path = file_path
+        elif(not is_path_absolute(file_path=file_path) and self.__is_content_cjson):
+            raise AbsolutePathConstraintError("Only absolute path is supported in import statements")
+        else:
+            dir_name: str = path.dirname(path.abspath(self.__file_path))
+            import_file_path = path.join(dir_name, file_path)
+        
         self.__content = self.__content.replace(Keywords.import_key + file_path + "\"", read(import_file_path))
 
     def __decode_single_line_comment(self, line_item: str):
         line_split: list[str] = line_item.split("\n")
         for i in range(0, len(line_split)):
             if line_split[i].strip() != "" and line_split[i].strip().startswith(Keywords.single_line_comment):
                 self.__content = self.__content.replace(line_split[i], "")
@@ -143,24 +166,24 @@
                 self.__content = self.__content.replace("\"<-" + each_key + "->\"", json.dumps(injecting_obj[each_key]))
             else:
                 self.__content = self.__content.replace("<-" + each_key + "->", str(injecting_obj[each_key]))
         
         self.__refine_obj(self.__content)
 
         return self.__obj
-    
 
-# cjson = Cjson(r"C:\Users\632400\Desktop\projects\cjson\tests\test-files\VariableInjection.cjson")
-# injec_data = {
-#             "fruit": "apple",
-#             "quantity": 1,
-#             "jsonTypeData": {
-#                 "secondaryData": {
-#                     "type": "fruit",
-#                     "seeds": "yes"
-#                 }
-#             }
-#         }
+# a = '''
+# {
+#     "source": $import "C:\\Users\\Home\\OneDrive\\Desktop\\projects\\cjson\\tests\\test-files\\source.json",
+#     "target": {
+#         "fruit": "Apple",
+#         "size": "Large",
+#         "color": "Red"
+#     }
+# }
+# '''
+# c = "C:\\Users\\Home\\OneDrive\\Desktop\\projects\\cjson\\tests\\test-files\\targetRelativeCalls.cjson"
 
-# data = cjson.inject(injecting_obj=injec_data)
+# b = Cjson(c, True)
 
-# print(data)
+# k = b.deserialize()
+# print(k)
```

### Comparing `codedjson-1.2.0/cjson/src/codedjson.egg-info/PKG-INFO` & `codedjson-1.3.2/cjson/src/codedjson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codedjson
-Version: 1.2.0
+Version: 1.3.2
 Summary: CJSON is a data file format(inspired from JSON), but supports logical expressions too. Having extended language support to NodeJS, Python and Java, users has experienced data reusability. For features and examples, please refer to this documentation as base document.
 Author: Shubhendu Shekhar Gupta
 Author-email: subhendushekhargupta@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
```

### Comparing `codedjson-1.2.0/cjson/src/utils/_is.py` & `codedjson-1.3.2/cjson/src/utils/_is.py`

 * *Files identical despite different names*

### Comparing `codedjson-1.2.0/cjson/src/utils/_json.py` & `codedjson-1.3.2/cjson/src/utils/_json.py`

 * *Files identical despite different names*

### Comparing `codedjson-1.2.0/setup.py` & `codedjson-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 __readme_file = open("README.md")
 __description = __readme_file.read()
 
 setuptools.setup(
     name="codedjson",
-    version="1.2.0",
+    version="1.3.2",
     description="CJSON is a data file format(inspired from JSON), but supports logical expressions too. Having extended language support to NodeJS, Python and Java, users has experienced data reusability. For features and examples, please refer to this documentation as base document.",
     long_description=__description,
     long_description_content_type="text/markdown",
     author="Shubhendu Shekhar Gupta",
     author_email="subhendushekhargupta@gmail.com",
     packages= [".", "utils/"],
     classifiers=[
```

