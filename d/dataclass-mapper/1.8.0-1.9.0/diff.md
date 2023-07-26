# Comparing `tmp/dataclass_mapper-1.8.0.tar.gz` & `tmp/dataclass_mapper-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclass_mapper-1.8.0.tar", max compression
+gzip compressed data, was "dataclass_mapper-1.9.0.tar", max compression
```

## Comparing `dataclass_mapper-1.8.0.tar` & `dataclass_mapper-1.9.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1057 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/LICENSE.md
--rw-r--r--   0        0        0     5857 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/README.rst
--rw-r--r--   0        0        0      490 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/__init__.py
--rw-r--r--   0        0        0      501 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/__init__.py
--rw-r--r--   0        0        0      498 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/assignment.py
--rw-r--r--   0        0        0     1194 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/function.py
--rw-r--r--   0        0        0      750 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/list.py
--rw-r--r--   0        0        0      806 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/recursive.py
--rw-r--r--   0        0        0      319 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/simple.py
--rw-r--r--   0        0        0      570 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/assignments/utils.py
--rw-r--r--   0        0        0      604 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/classmeta.py
--rw-r--r--   0        0        0     2134 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/code_generator.py
--rw-r--r--   0        0        0     2285 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/enum.py
--rw-r--r--   0        0        0      400 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/__init__.py
--rw-r--r--   0        0        0     3008 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/base.py
--rw-r--r--   0        0        0     1565 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/dataclasses.py
--rw-r--r--   0        0        0     3545 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/pydantic_v1.py
--rw-r--r--   0        0        0     3652 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/pydantic_v2.py
--rw-r--r--   0        0        0      238 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/implementations/utils.py
--rw-r--r--   0        0        0    12792 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/mapper.py
--rw-r--r--   0        0        0     7410 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/mapping_method.py
--rw-r--r--   0        0        0      391 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/namespace.py
--rw-r--r--   0        0        0        0 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/py.typed
--rw-r--r--   0        0        0     1187 2023-07-16 19:31:03.449260 dataclass_mapper-1.8.0/dataclass_mapper/utils.py
--rw-r--r--   0        0        0     1747 2023-07-16 19:32:13.874320 dataclass_mapper-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     6764 1970-01-01 00:00:00.000000 dataclass_mapper-1.8.0/setup.py
--rw-r--r--   0        0        0     6792 1970-01-01 00:00:00.000000 dataclass_mapper-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/LICENSE.md
+-rw-r--r--   0        0        0     5857 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/README.rst
+-rw-r--r--   0        0        0      490 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/__init__.py
+-rw-r--r--   0        0        0      574 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/assignments/__init__.py
+-rw-r--r--   0        0        0      498 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/assignments/assignment.py
+-rw-r--r--   0        0        0      940 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/assignments/dict.py
+-rw-r--r--   0        0        0     1194 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/assignments/function.py
+-rw-r--r--   0        0        0      750 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/assignments/list.py
+-rw-r--r--   0        0        0      806 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/assignments/recursive.py
+-rw-r--r--   0        0        0      319 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/assignments/simple.py
+-rw-r--r--   0        0        0      570 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/assignments/utils.py
+-rw-r--r--   0        0        0      604 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/classmeta.py
+-rw-r--r--   0        0        0     2134 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/code_generator.py
+-rw-r--r--   0        0        0     2285 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/enum.py
+-rw-r--r--   0        0        0      400 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/implementations/__init__.py
+-rw-r--r--   0        0        0     3372 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/implementations/base.py
+-rw-r--r--   0        0        0     1565 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/implementations/dataclasses.py
+-rw-r--r--   0        0        0     3545 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/implementations/pydantic_v1.py
+-rw-r--r--   0        0        0     3652 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/implementations/pydantic_v2.py
+-rw-r--r--   0        0        0      238 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/implementations/utils.py
+-rw-r--r--   0        0        0    12792 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/mapper.py
+-rw-r--r--   0        0        0     7472 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/mapping_method.py
+-rw-r--r--   0        0        0      391 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/namespace.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/py.typed
+-rw-r--r--   0        0        0     1187 2023-07-26 21:11:17.740396 dataclass_mapper-1.9.0/dataclass_mapper/utils.py
+-rw-r--r--   0        0        0     1747 2023-07-26 21:12:39.469384 dataclass_mapper-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6764 1970-01-01 00:00:00.000000 dataclass_mapper-1.9.0/setup.py
+-rw-r--r--   0        0        0     6792 1970-01-01 00:00:00.000000 dataclass_mapper-1.9.0/PKG-INFO
```

### Comparing `dataclass_mapper-1.8.0/LICENSE.md` & `dataclass_mapper-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/README.rst` & `dataclass_mapper-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/assignments/function.py` & `dataclass_mapper-1.9.0/dataclass_mapper/assignments/function.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/assignments/list.py` & `dataclass_mapper-1.9.0/dataclass_mapper/assignments/list.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/assignments/recursive.py` & `dataclass_mapper-1.9.0/dataclass_mapper/assignments/recursive.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/assignments/utils.py` & `dataclass_mapper-1.9.0/dataclass_mapper/assignments/utils.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/classmeta.py` & `dataclass_mapper-1.9.0/dataclass_mapper/classmeta.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/code_generator.py` & `dataclass_mapper-1.9.0/dataclass_mapper/code_generator.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/enum.py` & `dataclass_mapper-1.9.0/dataclass_mapper/enum.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/implementations/base.py` & `dataclass_mapper-1.9.0/dataclass_mapper/implementations/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum, auto
-from typing import Any, Dict, Optional, cast, get_args
+from typing import Any, Dict, Optional, cast, get_args, get_origin
 from uuid import uuid4
 
 import dataclass_mapper.code_generator as cg
 from dataclass_mapper.namespace import Namespace
 from dataclass_mapper.utils import is_union_type
 
 
@@ -37,21 +37,32 @@
 
     @property
     def type_string(self) -> str:
         try:
             type_name = cast(str, self.type.__name__)
         except Exception:
             type_name = str(self.type)
-        if self.allow_none:
-            type_name = f"Optional[{type_name}]"
+
         if is_union_type(self.type):
             ts = ", ".join(self.get_class_name(t) for t in get_args(self.type))
             if self.allow_none:
                 ts += ", NoneType"
             type_name = f"Union[{ts}]"
+            return type_name
+
+        if get_origin(self.type) is list:
+            type_name = f"List[{self.get_class_name(get_args(self.type)[0])}]"
+
+        if get_origin(self.type) is dict:
+            key_type, value_type = get_args(self.type)
+            type_name = f"Dict[{self.get_class_name(key_type)}, {self.get_class_name(value_type)}]"
+
+        if self.allow_none:
+            type_name = f"Optional[{type_name}]"
+
         return type_name
 
     @staticmethod
     def get_class_name(clazz: Any) -> str:
         try:
             return str(clazz.__name__)
         except AttributeError:
```

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/implementations/dataclasses.py` & `dataclass_mapper-1.9.0/dataclass_mapper/implementations/dataclasses.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/implementations/pydantic_v1.py` & `dataclass_mapper-1.9.0/dataclass_mapper/implementations/pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/implementations/pydantic_v2.py` & `dataclass_mapper-1.9.0/dataclass_mapper/implementations/pydantic_v2.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/mapper.py` & `dataclass_mapper-1.9.0/dataclass_mapper/mapper.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/mapping_method.py` & `dataclass_mapper-1.9.0/dataclass_mapper/mapping_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from enum import Enum, auto
 from typing import Callable, Dict, List, Optional, Type, Union
 
 from . import code_generator as cg
 from .assignments import (
     Assignment,
     CallableWithMax1Parameter,
+    DictRecursiveAssignment,
     FunctionAssignment,
     ListRecursiveAssignment,
     RecursiveAssignment,
     SimpleAssignment,
     get_var_name,
 )
 from .implementations.base import ClassMeta, FieldMeta
@@ -102,14 +103,15 @@
 class MappingMethodSourceCode:
     """Source code of the mapping method"""
 
     AssignmentClasses: List[Type[Assignment]] = [
         SimpleAssignment,
         RecursiveAssignment,
         ListRecursiveAssignment,
+        DictRecursiveAssignment,
     ]
 
     def __init__(self, source_cls: ClassMeta, target_cls: ClassMeta) -> None:
         self.source_cls = source_cls
         self.target_cls = target_cls
         self.function = cg.Function(
             "convert",
```

### Comparing `dataclass_mapper-1.8.0/dataclass_mapper/utils.py` & `dataclass_mapper-1.9.0/dataclass_mapper/utils.py`

 * *Files identical despite different names*

### Comparing `dataclass_mapper-1.8.0/pyproject.toml` & `dataclass_mapper-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclass-mapper"
-version = "1.8.0"
+version = "1.9.0"
 description = "Autogenerate mappings between dataclasses"
 authors = ["Jakob Kogler <jakob.kogler@gmail.com>"]
 
 readme = "README.rst"
 license = "MIT"
 
 repository = "https://github.com/dataclass-mapper/dataclass-mapper"
```

### Comparing `dataclass_mapper-1.8.0/setup.py` & `dataclass_mapper-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 {'': ['*']}
 
 extras_require = \
 {'pydantic': ['pydantic>=1.9.0']}
 
 setup_kwargs = {
     'name': 'dataclass-mapper',
-    'version': '1.8.0',
+    'version': '1.9.0',
     'description': 'Autogenerate mappings between dataclasses',
     'long_description': 'dataclass-mapper\n================\n\n|pypi| |support| |licence| |readthedocs| |build| |coverage|\n\n.. |pypi| image:: https://img.shields.io/pypi/v/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: pypi version\n\n.. |support| image:: https://img.shields.io/pypi/pyversions/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: supported Python version\n\n.. |build| image:: https://github.com/dataclass-mapper/dataclass-mapper/actions/workflows/test.yml/badge.svg\n    :target: https://github.com/dataclass-mapper/dataclass-mapper/actions\n    :alt: build status\n\n.. |coverage| image:: https://codecov.io/gh/dataclass-mapper/dataclass-mapper/branch/main/graphs/badge.svg?branch=main\n    :target: https://codecov.io/gh/dataclass-mapper/dataclass-mapper?branch=main\n    :alt: Code coverage\n\n.. |licence| image:: https://img.shields.io/pypi/l/dataclass-mapper.svg?style=flat-square\n    :target: https://pypi.org/project/dataclass-mapper/\n    :alt: licence\n\n.. |readthedocs| image:: https://img.shields.io/readthedocs/dataclass-mapper/latest.svg?style=flat-square&label=Read%20the%20Docs\n   :alt: Read the documentation at https://dataclass-mapper.readthedocs.io/en/latest/\n   :target: https://dataclass-mapper.readthedocs.io/en/latest/\n\nWriting mapper methods between two similar dataclasses is boring, need to be actively maintained and are error-prone.\nMuch better to let this library auto-generate them for you.\n\nThe focus of this library is:\n\n- **Concise and easy syntax:**\n  \n  - using it has to be a lot less overhead than writing the mappers by hand\n  - trivial mappings should not require code\n  - identical syntax for mapping between dataclasses and Pydantic models\n\n- **Safety:**\n\n  - using this library must give equal or more type safety than writing the mappers by hand\n  - the types between source and target classes must matches (including optional checks)\n  - all target fields must be actually initialized\n  - mappings cannot reference non-existing fields\n  - in case of an error a clean exception must be raised\n\n- **Performance:**\n\n  - mapping an object using this library must be the same speed than mapping using a custom mapper function\n  - the type checks shouldn\'t slow down the program\n  - because of the first two points, all type checks and the generation of the mapper functions happen during the definition of the classes\n\nMotivation\n----------\n\nA couple of example usecases, that show why this library might be useful.\n\n* Given an API with multiple, different interfaces (e.g. different API versions), that are all connected to a common algorithm with some common datamodel.\n  All the different API models needs to be mapped to the common datamodel, and afterwards mapped back to the API model.\n* Given an API that has a ``POST`` and a ``GET`` endpoint.\n  Both models (``POST`` request body model and ``GET`` response body model) are almost the same, but there are some minor differences.\n  E.g. response model has an additional ``id`` parameter.\n  You need a way of mapping the request model to a response model.\n\nInstallation\n------------\n\n``dataclass-mapper`` can be installed using:\n\n.. code-block:: bash\n\n   pip install dataclass-mapper\n   # or for Pydantic support\n   pip install \'dataclass-mapper[pydantic]\'\n\nExample\n-------\n\nWe have the following target data structure, a class called ``Person``.\n\n.. code-block:: python\n\n   >>> from dataclasses import dataclass\n\n   >>> @dataclass\n   ... class Person:\n   ...     first_name: str\n   ...     second_name: str\n   ...     age: int\n\n\nWe want to have a mapper from the source data structure, a class called ``ContactInfo``.\nNotice that the attribute ``second_name`` of ``Person`` is called ``surname`` in ``ContactInfo``.\nOther than that, all the attribute names are the same.\n\nInstead of writing a mapper function by hand, you can let it autogenerate one using this library:\n\n.. code-block:: python\n\n   >>> from dataclass_mapper import map_to, mapper\n   >>>\n   >>> @mapper(Person, {"second_name": "surname"})\n   ... @dataclass\n   ... class ContactInfo:\n   ...     first_name: str\n   ...     surname: str\n   ...     age: int\n   >>>\n   >>> contact = ContactInfo(first_name="Henry", surname="Kaye", age=42)\n   >>> map_to(contact, Person)\n   Person(first_name=\'Henry\', second_name=\'Kaye\', age=42)\n\nThe ``dataclass-mapper`` library autogenerated a mapper, that can be used with the ``map_to`` function.\nAll we had to specify was the name of the target class, and optionally specify which fields map to which other fields.\nNotice that we only had to specify that the ``second_name`` field has to be mapped to ``surname``,\nall other fields were mapped automatically because the field names didn\'t change.\n\nAnd the ``dataclass-mapper`` library will perform a lot of checks around this mapping.\nIt will check if the data types match, if some fields would be left uninitialized, etc.\n\nFeatures\n--------\n\nThe current version has support for:\n\n* Python\'s ``dataclass`` (with recursive models, custom initializers, optional types, extra-context, ...): see `Supported features <https://dataclass-mapper.readthedocs.io/en/latest/features.html>`_ for the full list and examples\n* Mappings between Enum classes:  see `Enum mappings <https://dataclass-mapper.readthedocs.io/en/latest/enums.html>`_\n* Pydantic models:  see `Pydantic support <https://dataclass-mapper.readthedocs.io/en/latest/pydantic.html>`_\n* Type/Value checks:  see `Type safety <https://dataclass-mapper.readthedocs.io/en/latest/type_safety.html>`_\n\nContributing\n------------\n\nSee `CONTRIBUTING.rst <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/CONTRIBUTING.rst>`_.\n\nLicense\n-------\n\nThe project is released under the `MIT license <https://github.com/dataclass-mapper/dataclass-mapper/blob/main/LICENSE.md>`_.\n',
     'author': 'Jakob Kogler',
     'author_email': 'jakob.kogler@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dataclass-mapper.readthedocs.io',
```

### Comparing `dataclass_mapper-1.8.0/PKG-INFO` & `dataclass_mapper-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclass-mapper
-Version: 1.8.0
+Version: 1.9.0
 Summary: Autogenerate mappings between dataclasses
 Home-page: https://dataclass-mapper.readthedocs.io
 License: MIT
 Keywords: dataclass,pydantic,python,automation
 Author: Jakob Kogler
 Author-email: jakob.kogler@gmail.com
 Requires-Python: >=3.8,<4.0
```

