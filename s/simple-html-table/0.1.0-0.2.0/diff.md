# Comparing `tmp/simple_html_table-0.1.0.tar.gz` & `tmp/simple_html_table-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_html_table-0.1.0.tar", last modified: Sat Jul 22 14:54:42 2023, max compression
+gzip compressed data, was "simple_html_table-0.2.0.tar", last modified: Wed Jul 26 19:15:49 2023, max compression
```

## Comparing `simple_html_table-0.1.0.tar` & `simple_html_table-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-22 14:54:42.439438 simple_html_table-0.1.0/
--rw-rw-rw-   0        0        0     3263 2023-07-22 11:48:12.000000 simple_html_table-0.1.0/.gitignore
--rw-rw-rw-   0        0        0     1091 2023-07-22 11:46:04.000000 simple_html_table-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3555 2023-07-22 14:54:42.439438 simple_html_table-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3104 2023-07-22 13:11:01.000000 simple_html_table-0.1.0/README.md
--rw-rw-rw-   0        0        0      716 2023-07-22 14:54:14.000000 simple_html_table-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-22 14:54:42.439438 simple_html_table-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-22 14:54:42.417924 simple_html_table-0.1.0/simple_html_table/
--rw-rw-rw-   0        0        0      515 2023-07-22 14:53:27.000000 simple_html_table-0.1.0/simple_html_table/__init__.py
--rw-rw-rw-   0        0        0    17332 2023-07-22 13:10:27.000000 simple_html_table-0.1.0/simple_html_table/htmltable.py
-drwxrwxrwx   0        0        0        0 2023-07-22 14:54:42.438437 simple_html_table-0.1.0/simple_html_table.egg-info/
--rw-rw-rw-   0        0        0     3555 2023-07-22 14:54:42.000000 simple_html_table-0.1.0/simple_html_table.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-07-22 14:54:42.000000 simple_html_table-0.1.0/simple_html_table.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-22 14:54:42.000000 simple_html_table-0.1.0/simple_html_table.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-22 14:54:42.000000 simple_html_table-0.1.0/simple_html_table.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-22 14:54:42.000000 simple_html_table-0.1.0/simple_html_table.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-26 19:15:49.509307 simple_html_table-0.2.0/
+-rw-rw-rw-   0        0        0     3263 2023-07-22 11:48:12.000000 simple_html_table-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1091 2023-07-22 11:46:04.000000 simple_html_table-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3555 2023-07-26 19:15:49.509307 simple_html_table-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3104 2023-07-22 13:11:01.000000 simple_html_table-0.2.0/README.md
+-rw-rw-rw-   0        0        0      716 2023-07-26 19:14:45.000000 simple_html_table-0.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-26 19:15:49.487308 simple_html_table-0.2.0/recipe/
+-rw-rw-rw-   0        0        0      702 2023-07-26 19:08:02.000000 simple_html_table-0.2.0/recipe/meta.yaml
+-rw-rw-rw-   0        0        0       42 2023-07-26 19:15:49.510307 simple_html_table-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-26 19:15:49.479307 simple_html_table-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-26 19:15:49.488308 simple_html_table-0.2.0/src/simple_html_table/
+-rw-rw-rw-   0        0        0      515 2023-07-26 19:07:05.000000 simple_html_table-0.2.0/src/simple_html_table/__init__.py
+-rw-rw-rw-   0        0        0    18632 2023-07-26 19:04:38.000000 simple_html_table-0.2.0/src/simple_html_table/htmltable.py
+drwxrwxrwx   0        0        0        0 2023-07-26 19:15:49.508307 simple_html_table-0.2.0/src/simple_html_table.egg-info/
+-rw-rw-rw-   0        0        0     3555 2023-07-26 19:15:49.000000 simple_html_table-0.2.0/src/simple_html_table.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-07-26 19:15:49.000000 simple_html_table-0.2.0/src/simple_html_table.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 19:15:49.000000 simple_html_table-0.2.0/src/simple_html_table.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-07-26 19:15:49.000000 simple_html_table-0.2.0/src/simple_html_table.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-26 19:15:49.000000 simple_html_table-0.2.0/src/simple_html_table.egg-info/top_level.txt
```

### Comparing `simple_html_table-0.1.0/.gitignore` & `simple_html_table-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `simple_html_table-0.1.0/LICENSE` & `simple_html_table-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_html_table-0.1.0/PKG-INFO` & `simple_html_table-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_html_table
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple way to create HTML tables with support for rowspan and colspan attributes.
 Author-email: Gavin Burnell <g.burnell@leeds.ac.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/gb119/simple_html_table
 Keywords: html,table
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simple_html_table Version: 0.1.0 Summary: Simple
+Metadata-Version: 2.1 Name: simple_html_table Version: 0.2.0 Summary: Simple
 way to create HTML tables with support for rowspan and colspan attributes.
 Author-email: Gavin Burnell
 burnell@leeds.ac.uk> License: MIT Project-URL: Homepage, https://github.com/
 gb119/simple_html_table Keywords: html,table Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE # simple_html_table Simple way to create HTML tables with
 support for rowspan and colspan attributes. ## Usage simple_html_table defines
```

### Comparing `simple_html_table-0.1.0/README.md` & `simple_html_table-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_html_table-0.1.0/pyproject.toml` & `simple_html_table-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_html_table-0.1.0/simple_html_table/__init__.py` & `simple_html_table-0.2.0/src/simple_html_table/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 A simple_html_table is a very simple library for making html tables.
 
 The raison d'etre for the package is to allow tables where cells have rowspan and colspan attributes set as well
 as allowing per-table, per-row and per-cell arbitary attributes.
 """
 __all__ = ["Table", "Row", "Cell"]
 
-__version_info__ = (0, 1, 0)
+__version_info__ = (0, 2, 0)
 __version__ = ".".join([str(x) for x in __version_info__])
 __author__ = "Gavin Burnell <https://github.com/gb119>"
 
 from .htmltable import Table, Row, Cell
```

### Comparing `simple_html_table-0.1.0/simple_html_table/htmltable.py` & `simple_html_table-0.2.0/src/simple_html_table/htmltable.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 Module to implement a table that renders to html.
 
 Created on Sat Jun 10 11:24:08 2023
 
 @author: phygbu
 """
 from typing import List, Dict, Tuple, Union, Optional
+from collections.abc import Iterable
 
 from collections.abc import MutableSequence
 
 import numpy as np
 
 
 class HTMLObjectMixin(object):
@@ -102,14 +103,47 @@
         return self._attrs
 
     @property
     def classes_list(self) -> List[str]:
         """Return the HTML classes as a list of strings."""
         return self._classes
 
+    @property
+    def content(self) -> str:
+        """Return the contents of the html tag."""
+        return self._content
+
+    @content.setter
+    def content(self, value: str) -> None:
+        if not isinstance(value, str):
+            value = str(value)
+        self._content = value
+
+
+class HTMLTuple(tuple):
+
+    """A holder for an immutable collection of HTMLObjects."""
+
+    def __init__(self, *args, location=None):
+        """Pull out the location attribute."""
+        super().__init__()
+        self.location = location
+
+    @property
+    def header(self) -> List[bool]:
+        """Get the Header attribute on the contents."""
+        return [x.header for x in self]
+
+    @header.setter
+    def header(self, value: Union[bool, List[bool]]) -> None:
+        if not isinstance(value, Iterable):
+            value = [value] * len(self)
+        for element, header in zip(self, value):
+            element.header = value
+
 
 class Table(HTMLObjectMixin, MutableSequence):
 
     """Represents an HTML table as a sequence of rows, or a 2D array.
 
     Attributes:
         classes (str):
@@ -171,15 +205,19 @@
 
     def __len__(self):
         return len(self._rows)
 
     def __getitem__(self, item: Union[Tuple[int, int], int]) -> Union["Cell", "Row"]:
         if isinstance(item, tuple):
             r, c = item
+            if isinstance(r, slice):
+                return HTMLTuple([self._rows[ix][c] for ix in range(*r.indices(len(self._rows)))], location=c)
             return self._rows[r][c]
+        if isinstance(item, slice):
+            return HTMLTuple([self._rows[ix] for ix in range(*item.indices(len(self._rows)))], location=None)
         return self._rows[item]
 
     def __setitem__(self, item: Union[Tuple[int, int], int], val: Union["Cell", "Row", "str"]) -> None:
         if isinstance(item, tuple) and isinstance(val, Cell):
             r, c = item
             self._rows[r][c] = val
         elif isinstance(item, tuple) and isinstance(val, str):
@@ -434,15 +472,15 @@
     table[0, 0].rowspan = 3
     table[0, 1].attrs_dict.update({"style": "{ background: red; }"})
     table[0].header = True
     for cell in table[0]:
         cell.classes = "table_th"
 
     result = table.render()
-    print(result,"\n")
+    print(result, "\n")
 
     def content_func(cell: Cell) -> str:
         """Callback function to fill in the table."""
         row, col = cell.location
         return contents[row][col]
 
     table2 = Table((3, 4), table_contents=content_func)
```

### Comparing `simple_html_table-0.1.0/simple_html_table.egg-info/PKG-INFO` & `simple_html_table-0.2.0/src/simple_html_table.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-html-table
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple way to create HTML tables with support for rowspan and colspan attributes.
 Author-email: Gavin Burnell <g.burnell@leeds.ac.uk>
 License: MIT
 Project-URL: Homepage, https://github.com/gb119/simple_html_table
 Keywords: html,table
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simple-html-table Version: 0.1.0 Summary: Simple
+Metadata-Version: 2.1 Name: simple-html-table Version: 0.2.0 Summary: Simple
 way to create HTML tables with support for rowspan and colspan attributes.
 Author-email: Gavin Burnell
 burnell@leeds.ac.uk> License: MIT Project-URL: Homepage, https://github.com/
 gb119/simple_html_table Keywords: html,table Classifier: Programming Language
 :: Python :: 3 Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE # simple_html_table Simple way to create HTML tables with
 support for rowspan and colspan attributes. ## Usage simple_html_table defines
```

