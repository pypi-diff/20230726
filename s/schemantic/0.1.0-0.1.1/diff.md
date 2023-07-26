# Comparing `tmp/schemantic-0.1.0.tar.gz` & `tmp/schemantic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemantic-0.1.0.tar", max compression
+gzip compressed data, was "schemantic-0.1.1.tar", max compression
```

## Comparing `schemantic-0.1.0.tar` & `schemantic-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1658 2023-04-22 06:37:56.957876 schemantic-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     3646 2023-07-21 10:19:34.585806 schemantic-0.1.0/README.md
--rw-r--r--   0        0        0      857 2023-07-21 09:04:23.115680 schemantic-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      149 2023-07-20 13:49:23.765353 schemantic-0.1.0/schemantic/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 12:09:04.396978 schemantic-0.1.0/schemantic/model/__init__.py
--rw-r--r--   0        0        0     6273 2023-07-21 10:18:13.332261 schemantic-0.1.0/schemantic/model/field_info.py
--rw-r--r--   0        0        0     3263 2023-07-21 10:08:08.425583 schemantic-0.1.0/schemantic/model/schematic.py
--rw-r--r--   0        0        0     1599 2023-07-20 15:11:31.740543 schemantic-0.1.0/schemantic/project.py
--rw-r--r--   0        0        0       74 2023-07-20 13:48:44.549590 schemantic-0.1.0/schemantic/schema/__init__.py
--rw-r--r--   0        0        0     4095 2023-07-21 10:11:56.538350 schemantic-0.1.0/schemantic/schema/abstract.py
--rw-r--r--   0        0        0    20160 2023-07-21 10:10:18.734882 schemantic-0.1.0/schemantic/schema/main.py
--rw-r--r--   0        0        0        0 2023-07-18 13:10:43.500286 schemantic-0.1.0/schemantic/utils/__init__.py
--rw-r--r--   0        0        0      185 2023-07-19 09:35:47.546132 schemantic-0.1.0/schemantic/utils/constant.py
--rw-r--r--   0        0        0      870 2023-07-21 10:03:29.885030 schemantic-0.1.0/schemantic/utils/misc.py
--rw-r--r--   0        0        0      351 2023-07-21 10:10:18.725883 schemantic-0.1.0/schemantic/utils/typing.py
--rw-r--r--   0        0        0     4421 1970-01-01 00:00:00.000000 schemantic-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1658 2023-04-22 06:37:56.957876 schemantic-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0     4006 2023-07-21 16:08:39.683555 schemantic-0.1.1/README.md
+-rw-r--r--   0        0        0      812 2023-07-26 05:47:30.908141 schemantic-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      149 2023-07-20 13:49:23.765353 schemantic-0.1.1/schemantic/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:09:04.396978 schemantic-0.1.1/schemantic/model/__init__.py
+-rw-r--r--   0        0        0     6273 2023-07-21 10:18:13.332261 schemantic-0.1.1/schemantic/model/field_info.py
+-rw-r--r--   0        0        0     3263 2023-07-21 10:08:08.425583 schemantic-0.1.1/schemantic/model/schematic.py
+-rw-r--r--   0        0        0     1599 2023-07-20 15:11:31.740543 schemantic-0.1.1/schemantic/project.py
+-rw-r--r--   0        0        0       74 2023-07-20 13:48:44.549590 schemantic-0.1.1/schemantic/schema/__init__.py
+-rw-r--r--   0        0        0     4095 2023-07-21 10:11:56.538350 schemantic-0.1.1/schemantic/schema/abstract.py
+-rw-r--r--   0        0        0    20160 2023-07-21 10:10:18.734882 schemantic-0.1.1/schemantic/schema/main.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:10:43.500286 schemantic-0.1.1/schemantic/utils/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-19 09:35:47.546132 schemantic-0.1.1/schemantic/utils/constant.py
+-rw-r--r--   0        0        0      870 2023-07-21 10:03:29.885030 schemantic-0.1.1/schemantic/utils/misc.py
+-rw-r--r--   0        0        0      351 2023-07-21 10:10:18.725883 schemantic-0.1.1/schemantic/utils/typing.py
+-rw-r--r--   0        0        0     4693 1970-01-01 00:00:00.000000 schemantic-0.1.1/PKG-INFO
```

### Comparing `schemantic-0.1.0/LICENSE.md` & `schemantic-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.0/README.md` & `schemantic-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -50,42 +50,51 @@
 ## Methods
 `HomologSchema`, `GroupSchema`, and `CultureSchema` have the following methods.
 
 ### `.schema()`
 Creates a dictionary, which represents the schema of the origin class/model.
 
 ```python
-my_schema.schema()
+my_homolog.schema()
 ```
-
-Gives:
+Output:
 ```yaml
 "class_name": "Thief"
 "common": {
     steals_only: "jewelry"
 }
-"copycat": {
-    stolen_goods: 10
-}
-"pink_panther": {
-    stolen_goods: 14
-}
+"copycat": {}
+"pink_panther": {}
 "required": ["stolen_goods", "steals_only"]
 "field_to_info": {"stolen_goods": "integer"}
 ```
 
 ### `.dump()`
 Dump the dictionary from `.schema()` to a yaml or toml file.
 ```python
 my_schema.dump("my/path/schema.yaml")
 # There is also toml support
 my_schema.dump("my/path/schema.toml")
 ```
 
 ### `.parse()`
+```yaml
+"class_name": "Thief"
+"common": {
+    steals_only: "jewelry"
+}
+"copycat": {
+    stolen_goods: 10
+}
+"pink_panther": {
+    stolen_goods: 14
+}
+"required": ["stolen_goods", "steals_only"]
+"field_to_info": {"stolen_goods": "integer"}
+```
 ```python
 parsed = my_homolog.parse_schema("my/path/schema.yaml")
 
 # parsed["copycat"].stolen_goods == 10
 # parsed["pink_panther"].stolen_goods == 14
 
 # Both -> steals_only == "jewelry"
@@ -148,7 +157,18 @@
     @computed_field(return_type=set[str])
     @property
     def fields_to_exclude_from_single_schema(cls) -> set[str]:
         upstream = super().fields_to_exclude_from_single_schema
         upstream.update(("exclude_me",))
         return upstream
 ```
+
+### Install
+```shell
+pip install schemantic
+```
+
+For `toml` or `yaml` dumping and parsing
+```shell
+pip install schemantic[toml]
+pip install schemantic[yaml]
+```
```

### Comparing `schemantic-0.1.0/pyproject.toml` & `schemantic-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [tool.poetry]
 name = "schemantic"
-version = "0.1.0"
+version = "0.1.1"
 description = "Manipulate model schemas utilizing homologous, grouped, or cultured paradigms"
 authors = ["caniko <python@rotas.mozmail.com>"]
 license = "BSD-4"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 pydantic = "^2.0"
 ordered-set = "^4.1.0"
 
 rtoml = { version="*", optional=true }
 ruamel-yaml = { version="*", optional=true }
-parameterized = "^0.9.0"
-coverage = "^7.2.7"
 
 [tool.poetry.extras]
 toml = ["rtoml"]
 yaml = ["ruamel-yaml"]
 
 [tool.poetry.group.dev.dependencies]
 parameterized = "^0.9.0"
```

### Comparing `schemantic-0.1.0/schemantic/model/field_info.py` & `schemantic-0.1.1/schemantic/model/field_info.py`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.0/schemantic/model/schematic.py` & `schemantic-0.1.1/schemantic/model/schematic.py`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.0/schemantic/project.py` & `schemantic-0.1.1/schemantic/project.py`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.0/schemantic/schema/abstract.py` & `schemantic-0.1.1/schemantic/schema/abstract.py`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.0/schemantic/schema/main.py` & `schemantic-0.1.1/schemantic/schema/main.py`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.0/schemantic/utils/misc.py` & `schemantic-0.1.1/schemantic/utils/misc.py`

 * *Files identical despite different names*

### Comparing `schemantic-0.1.0/PKG-INFO` & `schemantic-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: schemantic
-Version: 0.1.0
+Version: 0.1.1
 Summary: Manipulate model schemas utilizing homologous, grouped, or cultured paradigms
 License: BSD-4
 Author: caniko
 Author-email: python@rotas.mozmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: toml
 Provides-Extra: yaml
-Requires-Dist: coverage (>=7.2.7,<8.0.0)
 Requires-Dist: ordered-set (>=4.1.0,<5.0.0)
-Requires-Dist: parameterized (>=0.9.0,<0.10.0)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: rtoml ; extra == "toml"
 Requires-Dist: ruamel-yaml ; extra == "yaml"
 Description-Content-Type: text/markdown
 
 # Schemantic
 
@@ -72,42 +70,51 @@
 ## Methods
 `HomologSchema`, `GroupSchema`, and `CultureSchema` have the following methods.
 
 ### `.schema()`
 Creates a dictionary, which represents the schema of the origin class/model.
 
 ```python
-my_schema.schema()
+my_homolog.schema()
 ```
-
-Gives:
+Output:
 ```yaml
 "class_name": "Thief"
 "common": {
     steals_only: "jewelry"
 }
-"copycat": {
-    stolen_goods: 10
-}
-"pink_panther": {
-    stolen_goods: 14
-}
+"copycat": {}
+"pink_panther": {}
 "required": ["stolen_goods", "steals_only"]
 "field_to_info": {"stolen_goods": "integer"}
 ```
 
 ### `.dump()`
 Dump the dictionary from `.schema()` to a yaml or toml file.
 ```python
 my_schema.dump("my/path/schema.yaml")
 # There is also toml support
 my_schema.dump("my/path/schema.toml")
 ```
 
 ### `.parse()`
+```yaml
+"class_name": "Thief"
+"common": {
+    steals_only: "jewelry"
+}
+"copycat": {
+    stolen_goods: 10
+}
+"pink_panther": {
+    stolen_goods: 14
+}
+"required": ["stolen_goods", "steals_only"]
+"field_to_info": {"stolen_goods": "integer"}
+```
 ```python
 parsed = my_homolog.parse_schema("my/path/schema.yaml")
 
 # parsed["copycat"].stolen_goods == 10
 # parsed["pink_panther"].stolen_goods == 14
 
 # Both -> steals_only == "jewelry"
@@ -171,7 +178,18 @@
     @property
     def fields_to_exclude_from_single_schema(cls) -> set[str]:
         upstream = super().fields_to_exclude_from_single_schema
         upstream.update(("exclude_me",))
         return upstream
 ```
 
+### Install
+```shell
+pip install schemantic
+```
+
+For `toml` or `yaml` dumping and parsing
+```shell
+pip install schemantic[toml]
+pip install schemantic[yaml]
+```
+
```

