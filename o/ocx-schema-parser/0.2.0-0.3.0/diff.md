# Comparing `tmp/ocx-schema-parser-0.2.0.tar.gz` & `tmp/ocx_schema_parser-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocx-schema-parser-0.2.0.tar", last modified: Fri Feb  3 09:59:15 2023, max compression
+gzip compressed data, was "ocx_schema_parser-0.3.0.tar", max compression
```

## Comparing `ocx-schema-parser-0.2.0.tar` & `ocx_schema_parser-0.3.0.tar`

### file list

```diff
@@ -1,93 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.941967 ocx-schema-parser-0.2.0/
--rw-rw-rw-   0        0        0      633 2023-02-03 09:30:24.000000 ocx-schema-parser-0.2.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0     2931 2023-01-30 14:59:24.000000 ocx-schema-parser-0.2.0/.cookiecutterrc
--rw-rw-rw-   0        0        0      197 2023-01-30 14:59:24.000000 ocx-schema-parser-0.2.0/.coveragerc
--rw-rw-rw-   0        0        0      373 2023-01-30 14:59:24.000000 ocx-schema-parser-0.2.0/.editorconfig
--rw-rw-rw-   0        0        0      660 2023-01-30 14:59:24.000000 ocx-schema-parser-0.2.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0      241 2023-01-30 14:59:24.000000 ocx-schema-parser-0.2.0/.readthedocs.yml
--rw-rw-rw-   0        0        0       66 2023-01-30 14:59:24.000000 ocx-schema-parser-0.2.0/AUTHORS.rst
--rw-rw-rw-   0        0        0       94 2023-01-30 14:59:24.000000 ocx-schema-parser-0.2.0/CHANGELOG.rst
--rw-rw-rw-   0        0        0     3377 2023-02-01 15:36:51.000000 ocx-schema-parser-0.2.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1112 2023-01-31 15:31:32.000000 ocx-schema-parser-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      487 2023-02-03 09:44:50.000000 ocx-schema-parser-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3645 2023-02-03 07:45:02.000000 ocx-schema-parser-0.2.0/Makefile
--rw-rw-rw-   0        0        0     2835 2023-02-03 09:59:15.942963 ocx-schema-parser-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3045 2023-02-03 09:30:24.000000 ocx-schema-parser-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.891902 ocx-schema-parser-0.2.0/ci/
--rw-rw-rw-   0        0        0     3016 2023-01-30 14:59:25.000000 ocx-schema-parser-0.2.0/ci/bootstrap.py
--rw-rw-rw-   0        0        0       78 2023-01-30 14:59:25.000000 ocx-schema-parser-0.2.0/ci/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.869974 ocx-schema-parser-0.2.0/ci/templates/
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.870972 ocx-schema-parser-0.2.0/ci/templates/.github/
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.892897 ocx-schema-parser-0.2.0/ci/templates/.github/workflows/
--rw-rw-rw-   0        0        0     2066 2023-01-30 14:59:25.000000 ocx-schema-parser-0.2.0/ci/templates/.github/workflows/github-actions.yml
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.900921 ocx-schema-parser-0.2.0/docs/
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.901918 ocx-schema-parser-0.2.0/docs/_static/
--rw-rw-rw-   0        0        0     3150 2023-02-03 08:44:09.000000 ocx-schema-parser-0.2.0/docs/_static/logo.jpg
--rw-rw-rw-   0        0        0     5879 2023-01-23 15:06:58.000000 ocx-schema-parser-0.2.0/docs/_static/logo.png
--rw-rw-rw-   0        0        0       29 2023-01-30 14:59:25.000000 ocx-schema-parser-0.2.0/docs/authors.rst
--rw-rw-rw-   0        0        0       31 2023-01-30 14:59:25.000000 ocx-schema-parser-0.2.0/docs/changelog.rst
--rw-rw-rw-   0        0        0     1372 2023-02-03 09:48:04.000000 ocx-schema-parser-0.2.0/docs/conf.py
--rw-rw-rw-   0        0        0       34 2023-01-30 14:59:25.000000 ocx-schema-parser-0.2.0/docs/contributing.rst
--rw-rw-rw-   0        0        0      265 2023-01-30 14:59:25.000000 ocx-schema-parser-0.2.0/docs/index.rst
--rw-rw-rw-   0        0        0      104 2023-01-30 14:59:25.000000 ocx-schema-parser-0.2.0/docs/installation.rst
--rw-rw-rw-   0        0        0       28 2023-01-30 14:59:25.000000 ocx-schema-parser-0.2.0/docs/readme.rst
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.904908 ocx-schema-parser-0.2.0/docs/reference/
--rw-rw-rw-   0        0        0       68 2023-02-03 07:26:21.000000 ocx-schema-parser-0.2.0/docs/reference/index.rst
--rw-rw-rw-   0        0        0     1521 2023-02-03 08:37:05.000000 ocx-schema-parser-0.2.0/docs/reference/schema.rst
--rw-rw-rw-   0        0        0      109 2023-02-03 07:40:14.000000 ocx-schema-parser-0.2.0/docs/reference/utils.rst
--rw-rw-rw-   0        0        0       54 2023-02-02 15:34:24.000000 ocx-schema-parser-0.2.0/docs/requirements.txt
--rw-rw-rw-   0        0        0      120 2023-01-30 14:59:25.000000 ocx-schema-parser-0.2.0/docs/spelling_wordlist.txt
--rw-rw-rw-   0        0        0     1363 2023-02-02 13:00:18.000000 ocx-schema-parser-0.2.0/docs/usage.rst
--rw-rw-rw-   0        0        0     1156 2023-02-03 09:53:08.000000 ocx-schema-parser-0.2.0/environment.yaml
--rw-rw-rw-   0        0        0      559 2023-02-03 09:04:57.000000 ocx-schema-parser-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      806 2023-01-30 14:59:24.000000 ocx-schema-parser-0.2.0/pytest.ini
--rw-rw-rw-   0        0        0      392 2023-02-03 09:59:15.943960 ocx-schema-parser-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     3275 2023-02-03 09:59:06.000000 ocx-schema-parser-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.872964 ocx-schema-parser-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.915819 ocx-schema-parser-0.2.0/src/ocx_schema_parser.egg-info/
--rw-rw-rw-   0        0        0     2835 2023-02-03 09:59:15.000000 ocx-schema-parser-0.2.0/src/ocx_schema_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2046 2023-02-03 09:59:15.000000 ocx-schema-parser-0.2.0/src/ocx_schema_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 09:59:15.000000 ocx-schema-parser-0.2.0/src/ocx_schema_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-03 09:59:15.000000 ocx-schema-parser-0.2.0/src/ocx_schema_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      206 2023-02-03 09:59:15.000000 ocx-schema-parser-0.2.0/src/ocx_schema_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-02-03 09:59:15.000000 ocx-schema-parser-0.2.0/src/ocx_schema_parser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.921657 ocx-schema-parser-0.2.0/src/schema_parser/
--rw-rw-rw-   0        0        0      617 2023-02-03 09:46:42.000000 ocx-schema-parser-0.2.0/src/schema_parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.922697 ocx-schema-parser-0.2.0/src/schema_parser/configs/
--rw-rw-rw-   0        0        0     2177 2023-01-23 15:06:58.000000 ocx-schema-parser-0.2.0/src/schema_parser/configs/schema_config.yaml
--rw-rw-rw-   0        0        0     2523 2023-02-03 08:52:03.000000 ocx-schema-parser-0.2.0/src/schema_parser/data_classes.py
--rw-rw-rw-   0        0        0    19277 2023-02-01 10:49:16.000000 ocx-schema-parser-0.2.0/src/schema_parser/elements.py
--rw-rw-rw-   0        0        0     6281 2023-02-02 12:17:15.000000 ocx-schema-parser-0.2.0/src/schema_parser/helpers.py
--rw-rw-rw-   0        0        0    27108 2023-02-02 12:17:15.000000 ocx-schema-parser-0.2.0/src/schema_parser/parser.py
--rw-rw-rw-   0        0        0    18019 2023-02-02 12:17:15.000000 ocx-schema-parser-0.2.0/src/schema_parser/xelement.py
--rw-rw-rw-   0        0        0     4212 2023-02-02 12:17:15.000000 ocx-schema-parser-0.2.0/src/schema_parser/xparse.py
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.925023 ocx-schema-parser-0.2.0/src/utils/
--rw-rw-rw-   0        0        0       77 2023-02-03 08:41:04.000000 ocx-schema-parser-0.2.0/src/utils/__init__.py
--rw-rw-rw-   0        0        0     5691 2023-02-03 09:46:57.000000 ocx-schema-parser-0.2.0/src/utils/utilities.py
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.930008 ocx-schema-parser-0.2.0/tests/
--rw-rw-rw-   0        0        0     2067 2023-02-02 12:29:45.000000 ocx-schema-parser-0.2.0/tests/conftest.py
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.930008 ocx-schema-parser-0.2.0/tests/test_schema_helpers/
--rw-rw-rw-   0        0        0    62871 2023-01-27 13:56:21.000000 ocx-schema-parser-0.2.0/tests/test_schema_helpers/test_find_schema_changes.yml
--rw-rw-rw-   0        0        0     1065 2023-01-31 16:34:42.000000 ocx-schema-parser-0.2.0/tests/test_schema_helpers.py
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.935987 ocx-schema-parser-0.2.0/tests/test_schema_reader/
--rw-rw-rw-   0        0        0     1569 2023-01-27 13:56:26.000000 ocx-schema-parser-0.2.0/tests/test_schema_reader/test_attribute_types.yml
--rw-rw-rw-   0        0        0     1569 2023-01-27 13:56:26.000000 ocx-schema-parser-0.2.0/tests/test_schema_reader/test_complex_types.yml
--rw-rw-rw-   0        0        0     1569 2023-01-27 13:56:25.000000 ocx-schema-parser-0.2.0/tests/test_schema_reader/test_element_types.yml
--rw-rw-rw-   0        0        0      658 2023-01-27 13:56:23.000000 ocx-schema-parser-0.2.0/tests/test_schema_reader/test_summary_table.yml
--rw-rw-rw-   0        0        0     2391 2023-01-27 13:56:24.000000 ocx-schema-parser-0.2.0/tests/test_schema_reader/test_tbl_attribute_groups.yml
--rw-rw-rw-   0        0        0     1569 2023-01-27 13:56:24.000000 ocx-schema-parser-0.2.0/tests/test_schema_reader/test_tbl_simple_types.yml
--rw-rw-rw-   0        0        0     1329 2023-01-31 16:34:42.000000 ocx-schema-parser-0.2.0/tests/test_schema_reader.py
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.935987 ocx-schema-parser-0.2.0/tests/test_utilities/
--rw-rw-rw-   0        0        0     1717 2023-01-30 12:59:39.000000 ocx-schema-parser-0.2.0/tests/test_utilities/test_load_yaml_config.yml
--rw-rw-rw-   0        0        0     1076 2023-02-03 09:47:24.000000 ocx-schema-parser-0.2.0/tests/test_utilities.py
--rw-rw-rw-   0        0        0     6896 2023-02-02 12:17:15.000000 ocx-schema-parser-0.2.0/tests/test_xelement.py
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.938977 ocx-schema-parser-0.2.0/tests/test_xml_parser/
--rw-rw-rw-   0        0        0      261 2023-01-27 13:56:27.000000 ocx-schema-parser-0.2.0/tests/test_xml_parser/test_get_namespaces.yml
--rw-rw-rw-   0        0        0      142 2023-01-27 13:56:27.000000 ocx-schema-parser-0.2.0/tests/test_xml_parser/test_get_referenced_files.yml
--rw-rw-rw-   0        0        0       73 2023-01-27 13:56:27.000000 ocx-schema-parser-0.2.0/tests/test_xml_parser/test_get_target_namespace.yml
-drwxrwxrwx   0        0        0        0 2023-02-03 09:59:15.941967 ocx-schema-parser-0.2.0/tests/test_xparse/
--rw-rw-rw-   0        0        0      261 2023-01-30 11:59:37.000000 ocx-schema-parser-0.2.0/tests/test_xparse/test_get_namespaces.yml
--rw-rw-rw-   0        0        0      142 2023-01-30 11:59:38.000000 ocx-schema-parser-0.2.0/tests/test_xparse/test_get_referenced_files.yml
--rw-rw-rw-   0        0        0       73 2023-01-30 11:59:38.000000 ocx-schema-parser-0.2.0/tests/test_xparse/test_get_target_namespace.yml
--rw-rw-rw-   0        0        0     1348 2023-01-23 15:06:58.000000 ocx-schema-parser-0.2.0/tests/test_xparse.py
--rw-rw-rw-   0        0        0     1954 2023-02-01 09:48:50.000000 ocx-schema-parser-0.2.0/tox.ini
+-rw-r--r--   0        0        0     1112 2023-01-31 15:31:32.807974 ocx_schema_parser-0.3.0/LICENSE
+-rw-r--r--   0        0        0      811 2023-07-24 09:28:18.051584 ocx_schema_parser-0.3.0/ocx_schema_parser/__init__.py
+-rw-r--r--   0        0        0     3591 2023-07-23 11:37:55.544187 ocx_schema_parser-0.3.0/ocx_schema_parser/check.py
+-rw-r--r--   0        0        0     2838 2023-07-20 12:06:32.144927 ocx_schema_parser-0.3.0/ocx_schema_parser/configs/schema_config.yaml
+-rw-r--r--   0        0        0     3013 2023-02-10 14:09:27.039093 ocx_schema_parser-0.3.0/ocx_schema_parser/data_classes.py
+-rw-r--r--   0        0        0    20844 2023-07-23 14:11:26.183591 ocx_schema_parser-0.3.0/ocx_schema_parser/elements.py
+-rw-r--r--   0        0        0     6281 2023-02-02 12:17:15.518318 ocx_schema_parser-0.3.0/ocx_schema_parser/helpers.py
+-rw-r--r--   0        0        0       73 2023-02-22 08:18:40.121172 ocx_schema_parser-0.3.0/ocx_schema_parser/ocxtransformer/__init__.py
+-rw-r--r--   0        0        0     1301 2023-07-23 10:58:44.430743 ocx_schema_parser-0.3.0/ocx_schema_parser/ocxtransformer/downloader.py
+-rw-r--r--   0        0        0      542 2023-07-19 17:15:38.276801 ocx_schema_parser-0.3.0/ocx_schema_parser/ocxtransformer/transformer.py
+-rw-r--r--   0        0        0    28430 2023-07-23 14:23:09.261189 ocx_schema_parser-0.3.0/ocx_schema_parser/parser.py
+-rw-r--r--   0        0        0       77 2023-02-03 08:41:04.027159 ocx_schema_parser-0.3.0/ocx_schema_parser/utils/__init__.py
+-rw-r--r--   0        0        0     6019 2023-07-23 11:54:20.437216 ocx_schema_parser-0.3.0/ocx_schema_parser/utils/utilities.py
+-rw-r--r--   0        0        0    18052 2023-07-23 10:28:25.071035 ocx_schema_parser-0.3.0/ocx_schema_parser/xelement.py
+-rw-r--r--   0        0        0     4255 2023-07-20 11:21:24.276611 ocx_schema_parser-0.3.0/ocx_schema_parser/xparse.py
+-rw-r--r--   0        0        0       73 2023-02-22 14:45:18.569527 ocx_schema_parser-0.3.0/ocx_schema_parser/xsclasses/__init__.py
+-rw-r--r--   0        0        0    38272 2023-02-17 11:23:24.538267 ocx_schema_parser-0.3.0/ocx_schema_parser/xsclasses/xsd.py
+-rw-r--r--   0        0        0     1963 2023-07-26 09:25:28.360870 ocx_schema_parser-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-07-19 16:31:21.428220 ocx_schema_parser-0.3.0/README.md
+-rw-r--r--   0        0        0      591 1970-01-01 00:00:00.000000 ocx_schema_parser-0.3.0/PKG-INFO
```

### Comparing `ocx-schema-parser-0.2.0/LICENSE` & `ocx_schema_parser-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocx-schema-parser-0.2.0/src/schema_parser/data_classes.py` & `ocx_schema_parser-0.3.0/ocx_schema_parser/data_classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""The data_class module contains the dataclasses holding schema attributes after parsing."""
+"""The data_classes module contains the dataclasses holding schema attributes after parsing."""
 #  Copyright (c) 2023. OCX Consortium https://3docx.org. See the LICENSE
 from dataclasses import dataclass
 from dataclasses import field
 from dataclasses import fields
 from typing import Dict
 from typing import List
 from typing import Tuple
 
 
 @dataclass
 class BaseDataClass:
     """Base class for OCX dataclasses.
 
-    Each sub-class has to implement a field metadata with name `header` for each of its attributes, for example:
+    Each subclass has to implement a field metadata with name `header` for each of its attributes, for example:
 
         ``name : str = field(metadata={'header': '<User friendly field name>'})``
 
     """
 
     def to_dict(self) -> Dict:
         """Output the data class as a dict with field names as keys."""
@@ -27,15 +27,15 @@
             table[my_fields[i].metadata["header"]] = value
             i += 1
         return table
 
 
 @dataclass
 class SchemaChange(BaseDataClass):
-    """Class for keeping track of OCX schema changes
+    """Class for keeping track of OCX schema changes.
 
     Args:
          version: The schema version the change applies to
          author: The author of the schem change
          date: The date of the schema change
          description: A description of the change
 
@@ -45,15 +45,15 @@
     author: str = field(metadata={"header": "Author"})
     date: str = field(metadata={"header": "Date"})
     description: str = field(default="", metadata={"header": "Description"})
 
 
 @dataclass
 class SchemaType(BaseDataClass):
-    """Class for xsd schema type information
+    """Class for xsd schema type information.
 
     Args:
          name: The schema type name
          prefix: The schema type namespace prefix
          source_line: The line number in the schema file where the type is defined
          tag: The schema type tag
 
@@ -63,19 +63,34 @@
     name: str = field(metadata={"header": "Name"})
     tag: str = field(metadata={"header": "Tag"})
     source_line: int = field(metadata={"header": "Source Line"})
 
 
 @dataclass
 class SchemaSummary:
-    """Class for schema summary information
+    """Class for schema summary information.
 
     Args:
          schema_version: The schema version
          schema_types: Tuples of the number of schema types
          schema_namespaces: Tuples of namespace prefixes
 
     """
 
     schema_version: List[Tuple] = field(metadata={"header": "Schema Version"})
     schema_types: List[Tuple] = field(metadata={"header": "Schema Types"})
     schema_namespaces: List[Tuple] = field(metadata={"header": "Namespaces"})
+
+
+@dataclass
+class SchemaEnumerator(BaseDataClass):
+    """Enumerator class.
+
+    Args:
+        name: The name of the ``xs:attribute`` enumerator
+        values: Enumeration values
+        descriptions: Enumeration descriptions
+    """
+
+    name: str = field(metadata={"header": "Attribute name"})
+    values: List[str] = field(metadata={"header": "Value"}, default_factory=lambda: [])
+    descriptions: List[str] = field(metadata={"header": "Source Line"}, default_factory=lambda: [])
```

### Comparing `ocx-schema-parser-0.2.0/src/schema_parser/elements.py` & `ocx_schema_parser-0.3.0/ocx_schema_parser/elements.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,75 @@
 """The OCX Schema content classes."""
-# Copyright (c) 2022-2023.  OCX Consortium https://3docx.org. See the LICENSE
+#  Copyright (c) 2022-2023. OCX Consortium https://3docx.org. See the LICENSE
 
 from collections import defaultdict
 from logging import Logger
 from typing import Dict
 from typing import List
 from typing import Union
 
 from lxml.etree import Element
 from lxml.etree import QName
 
 from .helpers import SchemaHelper
 from .xelement import LxmlElement
+from .data_classes import SchemaEnumerator
 
 
 class OcxAttribute:
-    """Global schema attribute class capturing the xsd schema definition of a global xs:attribute.
+    """Global schema attribute class capturing the XSD schema definition of a global ``xs:attribute``.
 
     Args:
-        xs_attribute: The lxml.etree.Element class
+        xs_attribute: The ``lxml.etree.Element`` instance
 
     Attributes:
+        _xs_attribute: The ``lxml.etree.Element`` instance
         _name : The attribute name
         _type : The attribute type
         _use : Whether the attribute is optional or required
         _fixed: Whether the attribute has a fixed value if any
-        _default: The deaflalt value of the attribute if any
+        _default: The default value of the attribute if any
         _annotation: The attribute description
         _is_global: True if the element is global, False otherwise
+        _enumerations: List of enumerator values. Empty if the attribute is not an enumerator
 
     """
 
     def __init__(self, xs_attribute: Element):
         # Private
+        self._xs_attribute = xs_attribute
         self._name = LxmlElement.get_name(xs_attribute)
         self._type = SchemaHelper.get_type(xs_attribute)
         self._use = LxmlElement.get_use(xs_attribute)
         self._fixed = xs_attribute.get("fixed")
         self._default = xs_attribute.get("default")
         self._annotation = LxmlElement.get_element_text(xs_attribute)
         self._is_global = False
+        self._enumerator = self.find_enumerations()
 
     def get_use(self) -> str:
         """The xs:attribute use (optional or required)
 
         Returns:
             Returns either 'required' or 'optional'
 
         """
         return self._use
 
+    def assign_referenced_attribute(self, reference: Element):
+        """Assign the actual referenced attribute and update members.
+
+        Args:
+            reference: The reference to the attribute ``xs:attribute`` definition
+
+        """
+
+        self._xs_attribute = reference
+        self._enumerator = self.find_enumerations()
+
     def get_fixed(self) -> str:
         """The fixed value of the xs:attribute
 
         Returns:
             Returns the fixed value of the attribute or an empty string if None
 
         """
@@ -159,14 +175,36 @@
             "Type": self.get_type(),
             "Use": self.get_use(),
             "Default": self.get_default(),
             "Fixed": self.get_fixed(),
             "Description": self.get_description(),
         }
 
+    def is_enumerator(self):
+        """True if the attribute is an enumeration, False otherwise."""
+        return len(LxmlElement.find_all_children_with_name(self._xs_attribute, 'enumeration')) > 0
+
+    def find_enumerations(self) -> Union[SchemaEnumerator, None]:
+        """Find any enumeration values."""
+        enum = None
+        if self.is_enumerator():
+            enum = SchemaEnumerator(self.get_name())
+            values = []
+            descriptions = []
+            for e in LxmlElement.iter(self._xs_attribute, '{*}enumeration'):
+                values.append(e.get('value'))
+                descriptions.append(LxmlElement.get_element_text(e))
+            enum.values = values
+            enum.descriptions = descriptions
+        return enum
+
+    def get_enumerations(self) -> SchemaEnumerator:
+        """Return the enumerator data class."""
+        return self._enumerator
+
 
 class OcxChildElement:
     """Class capturing the OCX xsd schema definition of a child or sub element ``xs:element``.
 
     Args:
         xs_element: The lxml.etree.Element class
 
@@ -472,15 +510,15 @@
         Returns:
             None
 
         """
         self._children[tag] = child
 
     def get_children(self) -> List:
-        """Get all my children xsd types
+        """Get all my children XSD types.
 
         Returns:
             Return all children as a dict of key-value pairs ``(tag, OCXChildElement)``
 
         """
         return self._children
 
@@ -729,12 +767,12 @@
                  - Type
                  - Use
                  - Cardinality
                  - Description
 
         """
         table = defaultdict(list)
-        for child in self._children:
+        for child in sorted(self._children, key=lambda x: x.get_name()):
             attributes = child.attributes_to_dict()
             for a in attributes:
                 table[a].append(attributes[a])
         return table
```

### Comparing `ocx-schema-parser-0.2.0/src/schema_parser/helpers.py` & `ocx_schema_parser-0.3.0/ocx_schema_parser/helpers.py`

 * *Files identical despite different names*

### Comparing `ocx-schema-parser-0.2.0/src/schema_parser/parser.py` & `ocx_schema_parser-0.3.0/ocx_schema_parser/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #  Copyright (c) 3-2023.  OCX Consortium https://3docx.org. See the LICENSE
-
+# System imports
 from collections import defaultdict
-from logging import Logger
 from pathlib import Path
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
-
+# Third party imports
+from loguru import logger
 import requests
 from lxml.etree import Element
 from lxml.etree import QName
 from requests import HTTPError
-
-from . import DEFAULT_SCHEMA
-from . import PROCESS_SCHEMA_TYPES
-from . import SCHEMA_FOLDER
-from . import W3C_SCHEMA_BUILT_IN_TYPES
+# Application imports
+from ocx_schema_parser import DEFAULT_SCHEMA
+from ocx_schema_parser import PROCESS_SCHEMA_TYPES
+from ocx_schema_parser import SCHEMA_FOLDER
+from ocx_schema_parser import W3C_SCHEMA_BUILT_IN_TYPES
 from .data_classes import SchemaSummary
 from .data_classes import SchemaType
-from .elements import OcxAttribute
-from .elements import OcxChildElement
-from .elements import OcxGlobalElement
+from .data_classes import SchemaEnumerator
+from .elements import OcxAttribute, OcxChildElement, OcxGlobalElement
 from .helpers import SchemaHelper
 from .xparse import LxmlElement
 from .xparse import LxmlParser
+from ocx_schema_parser.ocxtransformer.transformer import SchemaTransformer
 
 
 class OcxSchema:
     """The OcxSchema provides functionality for parsing the OCX xsd schema and storing all the elements.
 
     Args:
         logger: The main python logger
@@ -43,24 +43,25 @@
         _local_folder: The local folder where any external schemas will be downloaded
         _schema_changes: A list of all schema changes described by the tag SchemaChange contained in the xsd file.
         _schema_types: The list of xsd types to be parsed. Only these types will be stored.
         _default_schema: The default schema to be parsed
         _builtin_xs_types: W3C primitive data types.
             `www.w3.org <https://www.w3.org/TR/xmlschema-2/#built-in-primitive-datatypes>`_. Defined in ``config.yaml``
 
+
     """
 
-    def __init__(self, logger: Logger, local_folder: str = SCHEMA_FOLDER):
-        self._parser = LxmlParser(logger)
-        self.log = logger
+    def __init__(self, log: logger, local_folder: str = SCHEMA_FOLDER):
+        self._parser = LxmlParser(log)
+        self.log = log
         # Default namespace map for the reserved prefix xml. See https://www.w3.org/TR/xml-names/#sec-namespaces
         self._namespace = {"xml": "http://www.w3.org/XML/1998/namespace"}
-        Path(SCHEMA_FOLDER).mkdir(parents=True, exist_ok=True)
         self._is_parsed = False
         self._local_folder = local_folder
+        Path(self._local_folder).mkdir(parents=True, exist_ok=True)
         self._default_schema = DEFAULT_SCHEMA
         self._all_schema_elements = {}  # Hash table with tag as key schema_elements[tag] = lxml.etree.Element
         self._ocx_global_elements = {}  # Hash table with tag as key, value pairs(tag, OcxGlobalElement)
         self._all_types = defaultdict(list)  # Hash table with tag as key: all_types[tag] = lxml.etree.Element
         self._schema_types = PROCESS_SCHEMA_TYPES
         self._schema_version = None
         self._schema_changes = defaultdict(list)
@@ -236,14 +237,16 @@
         elements = self._get_schema_element_types()
         for tag in elements:
             e = self._get_element(tag)
             qn = QName(tag)
             name = qn.localname
             self.log.debug(f"Adding global element {name}")
             ocx = OcxGlobalElement(e, tag, self.log)
+            transformer = SchemaTransformer()
+            xsd_element = transformer.transform(e, LxmlElement.get_namespace(e))
             # store in look-up table
             self._add_global_ocx_element(tag, ocx)
             # Find all parents and add them to the instance
             self._find_all_my_parents(ocx)
             # Process all xs:attribute elements including all supertypes
             self._process_attributes(ocx)
             # Process ald children including super type children
@@ -327,14 +330,15 @@
         """
         attribute = OcxAttribute(xs_attribute)
         reference = LxmlElement.get_reference(xs_attribute)
         if reference is not None:
             # Get the referenced element
             tag, a = self._get_element_from_type(reference)
             attribute.put_name(LxmlElement.get_name(a))
+            attribute.assign_referenced_attribute(a)
             if attribute.get_description() == "":
                 attribute.put_description(LxmlElement.get_element_text(a))
             attribute.put_type(SchemaHelper.get_type(a))
         return attribute
 
     def _process_child(self, xs_element: Element) -> OcxChildElement:
         """Process an xs:element child element
@@ -455,14 +459,44 @@
                         return None
                     else:
                         return self._ocx_global_elements[tag]
         else:
             self.log.debug(f'{__class__}: The _namespace prefix  "{nsprefix}" is not defined')
             return None
 
+    def get_ocx_children_data(self, schema_type: str) -> Dict:
+        """Method to retrieve the ocx ``OcxGlobalElement`` children data
+
+        Args:
+            schema_type: the ocx type on the form ``prefix:name``
+
+        Returns:
+            All children data attributes of the element
+
+        """
+        element = self.get_ocx_element_from_type(schema_type)
+        if element:
+            return element.children_to_dict()
+        return {}
+
+    def get_ocx_attribute_data(self, schema_type: str) -> Dict:
+        """Method to retrieve the ocx ``OcxGlobalElement`` attribute data
+
+        Args:
+            schema_type: the ocx type on the form ``prefix:name``
+
+        Returns:
+            All the ocx element attribute data
+
+        """
+        element = self.get_ocx_element_from_type(schema_type)
+        if element:
+            return element.attributes_to_dict()
+        return {}
+
     def _get_prefix_from_namespace(self, namespace: str) -> str:
         """Return the namespace prefix
 
         Returns:
             the namespace prefix
 
         """
@@ -499,42 +533,42 @@
 
         Returns:
             The dict of namespaces as (namespace,prefix) key-value pairs
 
         """
         return self._namespace
 
-    def _get_all_schema_elements(self) -> Dict:
-        """All ``lxml.etree.Element`` schema elements
+    def get_all_schema_elements(self) -> Dict:
+        """Return all OCX schema elements.
 
         Returns:
-            The dict of all global xsd lxml.etree.Element elements with tag as key
+            The dict of all global XSD ``lxml.etree.Element`` elements with the unique tag ``{namespace}name`` as key.
 
         """
         return self._all_schema_elements
 
     def _sort_schema_elements(self):
         """Sorts the schema hash table"""
         sorted_dict = sorted(self._all_schema_elements.items(), key=lambda kv: kv[0])
         self._all_schema_elements = sorted_dict
 
     def _get_schema_types(self, schema_type: str) -> List[str]:
-        """Internal function to retrieve a list of tags of ``lxml.etree.Element`` schema elements of a specific type
+        """Internal function to retrieve a list of tags of ``lxml.etree.Element`` schema elements of a specific type.
 
         Returns:
             The sorted list of all tags of ``lxml.etree.Element`` of type ``schema_type``
 
         """
         elements = []
         for tag in self._all_types[schema_type]:
             elements.append(tag)
         return sorted(elements)
 
-    def get_ocx_elements(self) -> List:
-        """All ocx ``OcxGlobalElement`` elements
+    def get_ocx_elements(self) -> List[OcxGlobalElement]:
+        """All ocx ``OcxGlobalElement`` elements.
 
         Returns:
             The list of all parsed ``OcxGlobalElement`` instances
 
         """
         return list(self._ocx_global_elements.values())
 
@@ -544,61 +578,61 @@
         Returns:
             The coded version string of the OCX schema
 
         """
         return self._schema_version
 
     def get_schema_changes(self) -> Dict:
-        """The OCX schema change history
+        """The OCX schema change history.
 
         Returns:
             The schema changes for all schema versions
 
         """
         return self._schema_changes
 
     def _get_schema_element_types(self) -> List:
-        """All schema elements of type ``element``
+        """All schema elements of type ``element``.
 
         Returns:
             The list of all etree.Element of type ``element``
 
         """
         return self._get_schema_types("element")
 
     def _get_schema_complex_types(self) -> List[str]:
-        """All tags for schema elements of type ``complexType``
+        """All tags for schema elements of type ``complexType``.
 
         Returns:
             The list of tags of all ``etree.Element`` of type ``complexType``
 
         """
         return self._get_schema_types("complexType")
 
     def _get_schema_simple_types(self) -> List[str]:
-        """Alle schema elements of type ``simpleType``
+        """Alle schema elements of type ``simpleType``.
 
         Returns:
             The list of tags of all etree.Element of type ``simpleType``
 
         """
         return self._get_schema_types("simpleType")
 
     def _get_schema_attribute_tyepes(self) -> List[str]:
         """All schema elements of type ``attribute'
 
         Returns:
-            The list of unique tags for all etree.Element of type ``attribute``
+            The list of unique tags for all etree.Element of type ``attribute``.
 
         """
 
         return self._get_schema_types("attribute")
 
     def _get_schema_attribute_group_types(self) -> List[str]:
-        """All schema elements of type ``attributeGroup``
+        """All schema elements of type ``attributeGroup``.
 
         Returns:
             The list of all etree.Element of type ``attributeGroup``
         """
         return self._get_schema_types("attributeGroup")
 
     def tbl_summary(self) -> SchemaSummary:
@@ -610,86 +644,86 @@
 
         schema_version = [("Schema Version", self.get_schema_version())]
         schema_types = [(schema_type, len(self._all_types[schema_type])) for schema_type in self._all_types]
         namespaces = [(ns, self._namespace[ns]) for ns in self._namespace]
         return SchemaSummary(schema_version, schema_types, namespaces)
 
     def tbl_attribute_groups(self) -> Dict:
-        """All parsed ``attributeGroup`` types in the schema and any referenced schemas'
+        """All parsed ``attributeGroup`` types in the schema and any referenced schemas.
 
         Returns:
 
              List of  ``SchemaType`` data class holding ``attributeGroup`` attributes.
         """
 
         table = {}
         elements = self._get_schema_attribute_group_types()
         for tag in elements:
             table[tag] = self._get_schema_type_data_class(tag).to_dict()
         return table
 
     def tbl_simple_types(self) -> Dict:
-        """The table of all parsed ``simpleType`` elements in the schema and any referenced schemas'
+        """The table of all parsed ``simpleType`` elements in the schema and any referenced schemas.
 
         Returns:
 
             The ``SchemaType`` data class attributes of ``simpleType``
 
         """
 
         table = {}
         elements = self._get_schema_simple_types()
         for tag in elements:
             table[tag] = self._get_schema_type_data_class(tag).to_dict()
         return table
 
     def tbl_attribute_types(self) -> Dict:
-        """The table of all parsed attribute elements in the schema and any referenced schemas'
+        """The table of all parsed attribute elements in the schema and any referenced schemas.
 
         Returns:
 
             The ``SchemaType`` data class attributes of ``attributeType``
         """
 
         table = {}
         elements = self._get_schema_attribute_tyepes()
         for tag in elements:
             table[tag] = self._get_schema_type_data_class(tag).to_dict()
         return table
 
     def tbl_element_types(self) -> Dict:
-        """The table of all parsed elements of type element in the schema and any referenced schemas'
+        """The table of all parsed elements of type element in the schema and any referenced schemas.
 
         Returns:
 
             The ``SchemaType`` data class attributes of ``element``
         """
 
         table = {}
         elements = self._get_schema_element_types()
         for tag in elements:
             table[tag] = self._get_schema_type_data_class(tag).to_dict()
         return table
 
     def tbl_complex_types(self) -> Dict:
-        """The table of all parsed complexType elements in the schema and any referenced schemas'
+        """The table of all parsed complexType elements in the schema and any referenced schemas.
 
         Returns:
 
             The ``SchemaType`` data class attributes of ``complexType``
         """
 
         table = {}
         elements = self._get_schema_complex_types()
         for tag in elements:
             table[tag] = self._get_schema_type_data_class(tag).to_dict()
         return table
 
     def _get_schema_type_data_class(self, tag: str) -> SchemaType:
-        """Return the ``SchemaType`` dataclass of the schema type with ``tag``
+        """Return the ``SchemaType`` dataclass of the schema type with ``tag``.
             Args:
                 tag: the schema ``tag``
 
             Returns:
 
                 A ``dataclass`` with the attributes of the element with the ``tag``
         '"""
```

### Comparing `ocx-schema-parser-0.2.0/src/schema_parser/xelement.py` & `ocx_schema_parser-0.3.0/ocx_schema_parser/xelement.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,15 +327,15 @@
 
         """
         attributes = LxmlElement.get_xml_attrib(element)
         return attributes.get("substitutionGroup")
 
     @staticmethod
     def get_element_text(element: Element) -> str:
-        """The text between the element's start and end tags without any tail text
+        """The text between the element's start and end tags without any tail text.
 
         Args:
             element: the etree.Element instance
 
         Returns:
 
             The element text stripped of any special characters
@@ -582,17 +582,18 @@
             element = element[i + 1 : len(element)]
         return element
 
     @staticmethod
     def strip_namespace_tag(element: str) -> str:
         """Returns the element name without the namespace tag
         Args:
-            element: The element name without tag
+            element: The element name with or without namespace as a string
 
         Returns:
-            The element name without tag
+            The element without namespace tag
 
         """
         i = element.find("}")
         if not i == -1:
             element = element[i + 1 : len(element)]
         return element
+
```

### Comparing `ocx-schema-parser-0.2.0/src/schema_parser/xparse.py` & `ocx_schema_parser-0.3.0/ocx_schema_parser/xparse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #  Copyright (c) 2023.  OCX Consortium https://3docx.org. See the LICENSE
-
-from logging import Logger
+# System imports
 from typing import Dict
-
+# Third party imports
+from loguru import logger
 from lxml import etree
 from lxml.etree import Element
 from lxml.etree import XMLSyntaxError
-
+# Application imports
 from .xelement import LxmlElement
 
 
 class LxmlParser:
     """A wrapper of the lxml etree document tree and parser.
 
     Args:
@@ -18,17 +18,17 @@
 
     Attributes:
         _tree : The ``lxml.etree`` DOM
         _log: The Python logger
 
     """
 
-    def __init__(self, logger: Logger):
+    def __init__(self, log: logger):
         self._tree: Element = None
-        self._log: Logger = logger
+        self._log = log
 
     def parse(self, file: str, store_ids: bool = False) -> bool:
         """Parses an XML file
         Args:
             file: The file name of the xml document to be parsed. The parser can only parse from a local file.
             store_ids: If set to True, the parser will create a hash table of the xml IDs
```

### Comparing `ocx-schema-parser-0.2.0/src/utils/utilities.py` & `ocx_schema_parser-0.3.0/ocx_schema_parser/utils/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 import errno
 import logging
 import os
 import re
 from collections import defaultdict
 from pathlib import Path
-from typing import Dict
+from typing import Dict, List
 
 import yaml
 
 
 def root_dir() -> str:
     """Path to the directory of the parent module."""
-    return os.path.realpath(os.path.join(os.path.dirname(__file__), "../"))
+    return os.path.realpath(os.path.join(os.path.dirname(__file__), "../../"))
 
 
 def current_dir(file: str) -> str:
     """The full path to the folder containing the ``file``
 
     Args:
         file: The name of an existing file
@@ -195,7 +195,17 @@
     """
     if config.exists():
         with open(config.absolute()) as f:
             app_config = yaml.safe_load(f)
         return app_config
     else:
         raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), config.absolute())
+
+
+def camel_case_split(str) -> List:
+    """Split camel case string to individual strings."""
+    return re.findall(r'[A-Z](?:[a-z]+|[A-Z]*(?=[A-Z]|$))', str)
+
+
+def dromedary_case_split(str) -> List:
+    """Split camel case string to individual strings."""
+    return re.findall(r'[A-Z]?[a-z]+|[A-Z]+(?=[A-Z]|$)', str)
```

### Comparing `ocx-schema-parser-0.2.0/tests/test_utilities/test_load_yaml_config.yml` & `ocx_schema_parser-0.3.0/ocx_schema_parser/configs/schema_config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,63 @@
-DEFAULT_SCHEMA: https://raw.githubusercontent.com/OCXStandard/OCX_Schema/working_draft/OCX_Schema.xsd
-PROCESS_SCHEMA_TYPES:
-- element
-- attribute
-- complexType
-- simpleType
-- attributeGroup
-SCHEMA_FOLDER: schema_versions\
-SUB_COMMAND: schema
-W3C_SCHEMA_BUILT_IN_TYPES:
-  '{http://www.w3.org/2001/XMLSchema}NOTATION': https://www.w3.org/TR/xmlschema-2/#NOTATION
-  '{http://www.w3.org/2001/XMLSchema}QName': https://www.w3.org/TR/xmlschema-2/#QName
-  '{http://www.w3.org/2001/XMLSchema}anyURI': https://www.w3.org/TR/xmlschema-2/#string
-  '{http://www.w3.org/2001/XMLSchema}base64Binary': https://www.w3.org/TR/xmlschema-2/#base64Binary
-  '{http://www.w3.org/2001/XMLSchema}boolean': https://www.w3.org/TR/xmlschema-2/#boolean
-  '{http://www.w3.org/2001/XMLSchema}dateTime': https://www.w3.org/TR/xmlschema-2/#dateTime
-  '{http://www.w3.org/2001/XMLSchema}decimal': https://www.w3.org/TR/xmlschema-2/#decimal
-  '{http://www.w3.org/2001/XMLSchema}double': https://www.w3.org/TR/xmlschema-2/#double
-  '{http://www.w3.org/2001/XMLSchema}duration': https://www.w3.org/TR/xmlschema-2/#duration
-  '{http://www.w3.org/2001/XMLSchema}float': https://www.w3.org/TR/xmlschema-2/#float
-  '{http://www.w3.org/2001/XMLSchema}gMonthDay': https://www.w3.org/TR/xmlschema-2/#gMonthDay
-  '{http://www.w3.org/2001/XMLSchema}gYear': https://www.w3.org/TR/xmlschema-2/#gYear
-  '{http://www.w3.org/2001/XMLSchema}gYearMonth': https://www.w3.org/TR/xmlschema-2/#gYearMonth
-  '{http://www.w3.org/2001/XMLSchema}hexBinary': https://www.w3.org/TR/xmlschema-2/#hexBinary
-  '{http://www.w3.org/2001/XMLSchema}string': https://www.w3.org/TR/xmlschema-2/#string
-  '{http://www.w3.org/2001/XMLSchema}token': https://www.w3.org/TR/xmlschema-2/#token
+#  Copyright (c) 2023.  OCX Consortium https://3docx.org. See the LICENSE
+# Module specific config settings
+SCHEMA_FOLDER: 'schema_versions\'
+# DEFAULT_SCHEMA: 'https://3docx.org/fileadmin/ocx_schema/V286/OCX_Schema.xsd'
+# The working draft version on github:
+WORKING_DRAFT: 'https://raw.githubusercontent.com/OCXStandard/OCX_Schema/working_draft/OCX_Schema.xsd'
+DEFAULT_SCHEMA: 'https://3docx.org/fileadmin/ocx_schema/V286/OCX_Schema.xsd'
+SUB_COMMAND: 'schema'
+# w3c primitive data types. ref https://www.w3.org/TR/xmlschema-2/#built-in-primitive-datatypes
+W3C_SCHEMA_BUILT_IN_TYPES: {
+  '{http://www.w3.org/2001/XMLSchema}string': 'https://www.w3.org/TR/xmlschema-2/#string',
+  '{http://www.w3.org/2001/XMLSchema}boolean': 'https://www.w3.org/TR/xmlschema-2/#boolean',
+  '{http://www.w3.org/2001/XMLSchema}decimal': 'https://www.w3.org/TR/xmlschema-2/#decimal',
+  '{http://www.w3.org/2001/XMLSchema}float': 'https://www.w3.org/TR/xmlschema-2/#float',
+  '{http://www.w3.org/2001/XMLSchema}double': 'https://www.w3.org/TR/xmlschema-2/#double',
+  '{http://www.w3.org/2001/XMLSchema}duration': 'https://www.w3.org/TR/xmlschema-2/#duration',
+  '{http://www.w3.org/2001/XMLSchema}dateTime': 'https://www.w3.org/TR/xmlschema-2/#dateTime',
+  '{http://www.w3.org/2001/XMLSchema}gYearMonth': 'https://www.w3.org/TR/xmlschema-2/#gYearMonth',
+  '{http://www.w3.org/2001/XMLSchema}gYear': 'https://www.w3.org/TR/xmlschema-2/#gYear',
+  '{http://www.w3.org/2001/XMLSchema}gMonthDay': 'https://www.w3.org/TR/xmlschema-2/#gMonthDay',
+  '{http://www.w3.org/2001/XMLSchema}hexBinary': 'https://www.w3.org/TR/xmlschema-2/#hexBinary',
+  '{http://www.w3.org/2001/XMLSchema}base64Binary': 'https://www.w3.org/TR/xmlschema-2/#base64Binary',
+  '{http://www.w3.org/2001/XMLSchema}anyURI': 'https://www.w3.org/TR/xmlschema-2/#string',
+  '{http://www.w3.org/2001/XMLSchema}QName': 'https://www.w3.org/TR/xmlschema-2/#QName',
+  '{http://www.w3.org/2001/XMLSchema}token': 'https://www.w3.org/TR/xmlschema-2/#token',
+  '{http://www.w3.org/2001/XMLSchema}NOTATION': 'https://www.w3.org/TR/xmlschema-2/#NOTATION'
+}
+# Process only these XSD schema types
+PROCESS_SCHEMA_TYPES: [ 'element', 'attribute', 'complexType', 'simpleType', 'attributeGroup' ]
+# Known words for the spell checker
+KNOWN_WORD_LIST: [
+      '3D',
+      'NURBS',
+      'OCX',
+      'XML',
+      'authoring',
+      'circumcircle',
+      'consumables',
+      'enumerated',
+      'mm',
+      'modulus',
+      'multiplicities',
+      'ordinate',
+      'orthogonal',
+      'scantling',
+      'scantlings',
+      'schema',
+      'stiffeners',
+]
+# Schema naming conformance exceptions
+OCX_NAME_EXCEPTIONS: [
+      'AP_Pos',
+      'FP_Pos',
+      'GUIDRef',
+      'U_NURBSproperties',
+      'V_NURBSproperties',
+      'application_version',
+      'ocxXML',
+      'originating_system',
+      'time_stamp',
+]
+
+
```

