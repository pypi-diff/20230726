# Comparing `tmp/implicitdict-2.1.1.tar.gz` & `tmp/implicitdict-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "implicitdict-2.1.1.tar", last modified: Thu Mar 30 18:45:59 2023, max compression
+gzip compressed data, was "implicitdict-2.2.0.tar", last modified: Wed Jul 26 21:50:40 2023, max compression
```

## Comparing `implicitdict-2.1.1.tar` & `implicitdict-2.2.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:45:59.356212 implicitdict-2.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:45:59.352211 implicitdict-2.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:45:59.356212 implicitdict-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-30 18:45:46.000000 implicitdict-2.1.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-30 18:45:46.000000 implicitdict-2.1.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-30 18:45:46.000000 implicitdict-2.1.1/.github/workflows/test_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-30 18:45:46.000000 implicitdict-2.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-30 18:45:46.000000 implicitdict-2.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-30 18:45:46.000000 implicitdict-2.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-03-30 18:45:59.356212 implicitdict-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-30 18:45:46.000000 implicitdict-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-30 18:45:46.000000 implicitdict-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-30 18:45:46.000000 implicitdict-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 18:45:59.356212 implicitdict-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:45:59.352211 implicitdict-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:45:59.356212 implicitdict-2.1.1/src/implicitdict/
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-03-30 18:45:46.000000 implicitdict-2.1.1/src/implicitdict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-30 18:45:59.000000 implicitdict-2.1.1/src/implicitdict/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:45:59.356212 implicitdict-2.1.1/src/implicitdict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-03-30 18:45:59.000000 implicitdict-2.1.1/src/implicitdict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-30 18:45:59.000000 implicitdict-2.1.1/src/implicitdict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 18:45:59.000000 implicitdict-2.1.1/src/implicitdict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-30 18:45:59.000000 implicitdict-2.1.1/src/implicitdict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-30 18:45:59.000000 implicitdict-2.1.1/src/implicitdict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 18:45:59.356212 implicitdict-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-03-30 18:45:46.000000 implicitdict-2.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-03-30 18:45:46.000000 implicitdict-2.1.1/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-30 18:45:46.000000 implicitdict-2.1.1/tests/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-03-30 18:45:46.000000 implicitdict-2.1.1/tests/test_mutability.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-03-30 18:45:46.000000 implicitdict-2.1.1/tests/test_normal_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-03-30 18:45:46.000000 implicitdict-2.1.1/tests/test_optional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-03-30 18:45:46.000000 implicitdict-2.1.1/tests/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-03-30 18:45:46.000000 implicitdict-2.1.1/tests/test_string_based_date_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-03-30 18:45:46.000000 implicitdict-2.1.1/tests/test_string_based_time_delta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:50:40.934617 implicitdict-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:50:40.930617 implicitdict-2.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:50:40.930617 implicitdict-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-26 21:50:31.000000 implicitdict-2.2.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-26 21:50:31.000000 implicitdict-2.2.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-26 21:50:31.000000 implicitdict-2.2.0/.github/workflows/test_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-26 21:50:31.000000 implicitdict-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-26 21:50:31.000000 implicitdict-2.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-26 21:50:31.000000 implicitdict-2.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-07-26 21:50:40.934617 implicitdict-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-07-26 21:50:31.000000 implicitdict-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-26 21:50:31.000000 implicitdict-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-26 21:50:31.000000 implicitdict-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:50:40.934617 implicitdict-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:50:40.930617 implicitdict-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:50:40.930617 implicitdict-2.2.0/src/implicitdict/
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-07-26 21:50:31.000000 implicitdict-2.2.0/src/implicitdict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 21:50:40.000000 implicitdict-2.2.0/src/implicitdict/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-26 21:50:31.000000 implicitdict-2.2.0/src/implicitdict/jsonschema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:50:40.930617 implicitdict-2.2.0/src/implicitdict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14382 2023-07-26 21:50:40.000000 implicitdict-2.2.0/src/implicitdict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-26 21:50:40.000000 implicitdict-2.2.0/src/implicitdict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:50:40.000000 implicitdict-2.2.0/src/implicitdict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 21:50:40.000000 implicitdict-2.2.0/src/implicitdict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-26 21:50:40.000000 implicitdict-2.2.0/src/implicitdict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:50:40.934617 implicitdict-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/test_jsonschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/test_mutability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/test_normal_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/test_optional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/test_string_based_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/test_string_based_time_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-26 21:50:31.000000 implicitdict-2.2.0/tests/test_types.py
```

### Comparing `implicitdict-2.1.1/.github/workflows/publish.yaml` & `implicitdict-2.2.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `implicitdict-2.1.1/.github/workflows/test.yaml` & `implicitdict-2.2.0/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `implicitdict-2.1.1/.github/workflows/test_publish.yaml` & `implicitdict-2.2.0/.github/workflows/test_publish.yaml`

 * *Files identical despite different names*

### Comparing `implicitdict-2.1.1/.gitignore` & `implicitdict-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `implicitdict-2.1.1/LICENSE.md` & `implicitdict-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `implicitdict-2.1.1/PKG-INFO` & `implicitdict-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: implicitdict
-Version: 2.1.1
+Version: 2.2.0
 Summary: ImplicitDict base class that turns a subclass into a dict indexing attributes, making [de]serialization easy for complex typing-annotated data types.
 Author-email: InterUSS Platform <tsc@lists.interussplatform.org>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `implicitdict-2.1.1/README.md` & `implicitdict-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `implicitdict-2.1.1/pyproject.toml` & `implicitdict-2.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 license = { file = "LICENSE.md" }
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["arrow", "pytimeparse"]
+dependencies = ["arrow", "jsonschema", "pytimeparse"]
 [project.optional-dependencies]
 dev = ["pytest==5.0.0", "pytest-cov[all]", "black==21.10b0"]
 [project.urls]
 "Homepage" = "https://github.com/interuss/implicitdict"
 "Bug Tracker" = "https://github.com/interuss/implicitdict/issues"
 
 [tool.black]
```

### Comparing `implicitdict-2.1.1/src/implicitdict/__init__.py` & `implicitdict-2.2.0/src/implicitdict/__init__.py`

 * *Files identical despite different names*

### Comparing `implicitdict-2.1.1/src/implicitdict.egg-info/PKG-INFO` & `implicitdict-2.2.0/src/implicitdict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: implicitdict
-Version: 2.1.1
+Version: 2.2.0
 Summary: ImplicitDict base class that turns a subclass into a dict indexing attributes, making [de]serialization easy for complex typing-annotated data types.
 Author-email: InterUSS Platform <tsc@lists.interussplatform.org>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `implicitdict-2.1.1/src/implicitdict.egg-info/SOURCES.txt` & `implicitdict-2.2.0/src/implicitdict.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 pyproject.toml
 requirements.txt
 .github/workflows/publish.yaml
 .github/workflows/test.yaml
 .github/workflows/test_publish.yaml
 src/implicitdict/__init__.py
 src/implicitdict/_version.py
+src/implicitdict/jsonschema.py
 src/implicitdict.egg-info/PKG-INFO
 src/implicitdict.egg-info/SOURCES.txt
 src/implicitdict.egg-info/dependency_links.txt
 src/implicitdict.egg-info/requires.txt
 src/implicitdict.egg-info/top_level.txt
+tests/__init__.py
 tests/conftest.py
 tests/test_containers.py
 tests/test_inheritance.py
+tests/test_jsonschema.py
 tests/test_mutability.py
 tests/test_normal_usage.py
 tests/test_optional.py
 tests/test_properties.py
 tests/test_string_based_date_time.py
-tests/test_string_based_time_delta.py
+tests/test_string_based_time_delta.py
+tests/test_types.py
```

### Comparing `implicitdict-2.1.1/tests/conftest.py` & `implicitdict-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `implicitdict-2.1.1/tests/test_mutability.py` & `implicitdict-2.2.0/tests/test_mutability.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-from typing import Optional, List
-
 from implicitdict import ImplicitDict
 
-
-class MyData(ImplicitDict):
-    primitive: str
-    list_of_primitives: List[str]
-    generic_dict: dict
-    subtype: Optional["MyData"]
+from .test_types import MutabilityData
 
 
 def test_mutability_from_constructor():
     primitive = 'foobar'
     primitive_list = ['one', 'two']
     generic_dict = {'level1': 'foo', 'level2': {'bar': 'baz'}}
-    data = MyData(primitive=primitive, list_of_primitives=primitive_list, generic_dict=generic_dict)
+    data = MutabilityData(primitive=primitive, list_of_primitives=primitive_list, generic_dict=generic_dict)
     assert data.primitive == primitive
     assert data.list_of_primitives == primitive_list
     assert data.generic_dict == generic_dict
 
     primitive = 'foobar2'
     assert data.primitive != primitive
 
@@ -32,16 +25,16 @@
     assert data.generic_dict['level2']['bar'] == 'buzz'
 
 
 def test_mutability_from_parse():
     primitive = 'foobar'
     primitive_list = ['one', 'two']
     generic_dict = {'level1': 'foo', 'level2': {'bar': 'baz'}}
-    data_source = MyData(primitive=primitive, list_of_primitives=primitive_list, generic_dict=generic_dict)
-    data: MyData = ImplicitDict.parse(data_source, MyData)
+    data_source = MutabilityData(primitive=primitive, list_of_primitives=primitive_list, generic_dict=generic_dict)
+    data: MutabilityData = ImplicitDict.parse(data_source, MutabilityData)
     assert data.primitive == primitive
     assert data.list_of_primitives == primitive_list
     assert data.generic_dict == generic_dict
 
     primitive = 'foobar2'
     assert data.primitive != primitive
```

### Comparing `implicitdict-2.1.1/tests/test_normal_usage.py` & `implicitdict-2.2.0/tests/test_normal_usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from enum import Enum
 import json
 import pytest
 from typing import Dict, List, Literal, Optional
 
 from implicitdict import ImplicitDict, StringBasedDateTime, StringBasedTimeDelta
 
-
-class MyData(ImplicitDict):
-    foo: str
-    bar: int = 0
-    baz: Optional[float]
+from .test_types import NormalUsageData
 
 
 def test_basic_usage():
     # Most basic usage is to parse a plain dict into an ImplicitDict...
-    data: MyData = ImplicitDict.parse({'foo': 'asdf', 'bar': 1}, MyData)
+    data: NormalUsageData = ImplicitDict.parse({'foo': 'asdf', 'bar': 1}, NormalUsageData)
     # ...and implicitly serialize the ImplicitDict to a plain dict
     assert json.dumps(data) == '{"foo": "asdf", "bar": 1}'
 
     # Fields can be referenced directly...
     assert data.foo == 'asdf'
     assert data.bar == 1
     # ...or implicitly by name (because the object is implicitly a dict)
@@ -27,26 +23,26 @@
 
     # Optional fields that aren't specified simply don't exist
     assert 'baz' not in data
     with pytest.raises(KeyError):
         assert data.baz == 0
 
     # Optional fields can be omitted (fields with defaults are optional)
-    data = MyData(foo='asdf')
+    data = NormalUsageData(foo='asdf')
     assert json.loads(json.dumps(data)) == {'foo': 'asdf', 'bar': 0}
 
     # Optional fields can be specified
-    data = ImplicitDict.parse({'foo': 'asdf', 'baz': 1.23}, MyData)
+    data = ImplicitDict.parse({'foo': 'asdf', 'baz': 1.23}, NormalUsageData)
     assert json.loads(json.dumps(data)) == {'foo': 'asdf', 'bar': 0, 'baz': 1.23}
     assert 'baz' in data
     assert data.baz == 1.23
 
     # Failing to specify a required field ("foo") raises a ValueError
     with pytest.raises(ValueError):
-        MyData(bar=1)
+        NormalUsageData(bar=1)
 
 
 class MyIntEnum(int, Enum):
     Value1 = 1
     Value2 = 2
     Value3 = 3
 
@@ -59,15 +55,15 @@
 
 class Features(ImplicitDict):
     int_enum: MyIntEnum
     str_enum: MyStrEnum
     t_start: StringBasedDateTime
     my_duration: StringBasedTimeDelta
     my_literal: Literal['Must be this string']
-    nested: Optional[MyData]
+    nested: Optional[NormalUsageData]
 
 
 def test_features():
     src_dict = {
         'int_enum': 2,
         'str_enum': 'baz',
         't_start': '2022-01-01T01:23:45.6789Z',
@@ -102,15 +98,15 @@
 
     src_dict['my_literal'] = 'Not that string'
     with pytest.raises(ValueError):
         ImplicitDict.parse(src_dict, Features)
 
 
 class NestedStructures(ImplicitDict):
-    my_list: List[MyData]
+    my_list: List[NormalUsageData]
     my_list_2: List[List[int]]
     my_list_3: List[List[List[int]]]
     my_dict: Dict[str, List[float]]
 
 
 def test_nested_structures():
     src_dict = {
```

### Comparing `implicitdict-2.1.1/tests/test_optional.py` & `implicitdict-2.2.0/tests/test_optional.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,18 @@
 import json
-from typing import Optional
 
 import pytest
 
 from implicitdict import ImplicitDict
 
-
-class MyData(ImplicitDict):
-    required_field: str
-    optional_field1: Optional[str]
-    field_with_default: str = "default value"
-    optional_field2_with_none_default: Optional[str] = None
-    optional_field3_with_default: Optional[str] = "concrete default"
+from .test_types import OptionalData
 
 
 def test_fully_defined():
-    data = MyData(
-        required_field="foo1",
-        optional_field1="foo2",
-        field_with_default="foo3",
-        optional_field2_with_none_default="foo4",
-        optional_field3_with_default="foo5",
-    )
+    data = OptionalData.example_values()["fully_defined"]
     assert "required_field" in data
     assert "optional_field1" in data
     assert "field_with_default" in data
     assert "optional_field2_with_none_default" in data
     assert "optional_field3_with_default" in data
     s = json.dumps(data)
     assert "required_field" in s
@@ -37,30 +24,23 @@
     assert "foo2" in s
     assert "foo3" in s
     assert "foo4" in s
     assert "foo5" in s
 
 
 def test_over_defined():
-    data = MyData(
-        required_field="foo1",
-        optional_field1="foo2",
-        field_with_default="foo3",
-        optional_field2_with_none_default="foo4",
-        optional_field3_with_default="foo5",
-        unknown_field="foo6",
-    )
+    data = OptionalData.example_values()["over_defined"]
     d = json.loads(json.dumps(data))
     d["another_unknown_field"] = {"third_unknown_field": "foo7"}
-    _ = ImplicitDict.parse(d, MyData)
+    _ = ImplicitDict.parse(d, OptionalData)
 
 
 def test_minimally_defined():
     # An unspecified optional field will not be present in the object at all
-    data = MyData(required_field="foo1")
+    data = OptionalData.example_values()["minimally_defined"]
     assert "required_field" in data
     assert "optional_field1" not in data
     assert "field_with_default" in data
     assert "optional_field2_with_none_default" in data
     assert "optional_field3_with_default" in data
     with pytest.raises(KeyError):
         # Trying to reference the Optional field will result in a KeyError
@@ -73,15 +53,15 @@
     assert "field_with_default" in s
     assert "optional_field2" in s
     assert "optional_field3" in s
     assert "foo1" in s
 
 
 def test_provide_optional_field():
-    data = MyData(required_field="foo1", optional_field1="foo2")
+    data = OptionalData.example_values()["provide_optional_field"]
     assert "required_field" in data
     assert "optional_field1" in data
     assert "field_with_default" in data
     assert "optional_field2_with_none_default" in data
     assert "optional_field3_with_default" in data
     s = json.dumps(data)
     assert "required_field" in s
@@ -91,15 +71,15 @@
     assert "optional_field3" in s
     assert "foo1" in s
     assert "foo2" in s
 
 
 def test_provide_optional_field_as_none():
     # If an optional field with no default is explicitly provided as None, then that field will not be included in the object
-    data = MyData(required_field="foo1", optional_field1=None)
+    data = OptionalData.example_values()["provide_optional_field_as_none"]
     assert "required_field" in data
     assert "optional_field1" not in data  # <--
     assert "field_with_default" in data
     assert "optional_field2_with_none_default" in data
     assert "optional_field3_with_default" in data
     s = json.dumps(data)
     assert "required_field" in s
@@ -108,15 +88,15 @@
     assert "optional_field2" in s
     assert "optional_field3" in s
     assert "foo1" in s
 
 
 def test_provide_optional_field_with_none_default_as_none():
     # If a field has a default value, the field will always be present in the object, even if that default value is None and the field is Optional
-    data = MyData(required_field="foo1", optional_field2_with_none_default=None)
+    data = OptionalData.example_values()["provide_optional_field_with_none_default_as_none"]
     assert "required_field" in data
     assert "optional_field1" not in data
     assert "field_with_default" in data
     assert "optional_field2_with_none_default" in data  # <--
     assert "optional_field3_with_default" in data
     s = json.dumps(data)
     assert "required_field" in s
@@ -125,15 +105,15 @@
     assert "optional_field2" in s  # <--
     assert "optional_field3" in s
     assert "foo1" in s
 
 
 def test_provide_optional_field_with_default_as_none():
     # If a field has a default value, the field will always be present in the object
-    data = MyData(required_field="foo1", optional_field3_with_default=None)
+    data = OptionalData.example_values()["provide_optional_field_with_default_as_none"]
     assert "required_field" in data
     assert "optional_field1" not in data
     assert "field_with_default" in data
     assert "optional_field2_with_none_default" in data
     assert "optional_field3_with_default" in data  # <--
     s = json.dumps(data)
     assert "required_field" in s
```

### Comparing `implicitdict-2.1.1/tests/test_properties.py` & `implicitdict-2.2.0/tests/test_properties.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,37 @@
 import json
 
 from implicitdict import ImplicitDict
 
-
-class MyData(ImplicitDict):
-    foo: str
-
-    @property
-    def bar(self) -> str:
-        return self.foo + 'bar'
-
-    def get_baz(self) -> str:
-        return self.foo + 'baz'
-
-    def set_baz(self, value: str) -> None:
-        self.foo = value
-
-    baz = property(get_baz, set_baz)
-
-    @property
-    def booz(self) -> str:
-        return self.foo + 'booz'
-
-    @booz.setter
-    def booz(self, value: str) -> None:
-        self.foo = value
+from .test_types import PropertiesData
 
 
 def test_property_exclusion():
     """Ensure implicitdict doesn't serialize dynamic properties.
 
     Properties of a class instance are computed dynamically -- they are
     methods with syntactic sugar which makes them look like fields.  Because we
     shouldn't serialize the result of a class method, we also shouldn't
     serialize the result of a class property, even if that property includes a
     setter.
     """
     # Create class instance and ensure it works as expected
-    data = MyData(foo='foo')
+    data = PropertiesData.example_value()
     assert data.bar == 'foobar'
     assert data.baz == 'foobaz'
     assert data.booz == 'foobooz'
 
     # Serialize class instance and ensure the properties weren't serialized
     obj = json.loads(json.dumps(data))
     assert 'bar' not in obj
     assert 'baz' not in obj
     assert 'booz' not in obj
 
     # Ensure serialization can be deserialized to class instance
-    data: MyData = ImplicitDict.parse(obj, MyData)
+    data: PropertiesData = ImplicitDict.parse(obj, PropertiesData)
 
     # Ensure deserialized instance works as expected
     assert data.bar == 'foobar'
     assert data.baz == 'foobaz'
     assert data.booz == 'foobooz'
```

### Comparing `implicitdict-2.1.1/tests/test_string_based_date_time.py` & `implicitdict-2.2.0/tests/test_string_based_date_time.py`

 * *Files identical despite different names*

### Comparing `implicitdict-2.1.1/tests/test_string_based_time_delta.py` & `implicitdict-2.2.0/tests/test_string_based_time_delta.py`

 * *Files identical despite different names*

