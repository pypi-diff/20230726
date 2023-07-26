# Comparing `tmp/unit_syntax-0.2.1.tar.gz` & `tmp/unit_syntax-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_syntax-0.2.1.tar", max compression
+gzip compressed data, was "unit_syntax-0.2.2.tar", max compression
```

## Comparing `unit_syntax-0.2.1.tar` & `unit_syntax-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     5471 2023-07-26 03:41:02.897945 unit_syntax-0.2.1/README.md
--rw-r--r--   0        0        0      644 2023-07-26 03:41:02.901944 unit_syntax-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2104 2023-07-26 03:41:02.901944 unit_syntax-0.2.1/unit_syntax/__init__.py
--rw-r--r--   0        0        0       48 2023-07-26 03:41:02.901944 unit_syntax-0.2.1/unit_syntax/ipython/__init__.py
--rw-r--r--   0        0        0   333763 2023-07-26 03:41:02.901944 unit_syntax-0.2.1/unit_syntax/parser.py
--rw-r--r--   0        0        0     1592 2023-07-26 03:41:02.901944 unit_syntax-0.2.1/unit_syntax/transform.py
--rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 unit_syntax-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4687 2023-07-26 06:37:09.664332 unit_syntax-0.2.2/README.md
+-rw-r--r--   0        0        0      644 2023-07-26 06:37:09.664332 unit_syntax-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-07-26 06:37:09.668332 unit_syntax-0.2.2/unit_syntax/__init__.py
+-rw-r--r--   0        0        0     2033 2023-07-26 06:37:09.668332 unit_syntax-0.2.2/unit_syntax/ipython.py
+-rw-r--r--   0        0        0   333763 2023-07-26 06:37:09.668332 unit_syntax-0.2.2/unit_syntax/parser.py
+-rw-r--r--   0        0        0     1195 2023-07-26 06:37:09.668332 unit_syntax-0.2.2/unit_syntax/transform.py
+-rw-r--r--   0        0        0     5363 1970-01-01 00:00:00.000000 unit_syntax-0.2.2/PKG-INFO
```

### Comparing `unit_syntax-0.2.1/README.md` & `unit_syntax-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,35 @@
+Metadata-Version: 2.1
+Name: unit-syntax
+Version: 0.2.2
+Summary: Physical unit literals for Jupyter and IPython
+Home-page: https://github.com/ahupp/unit-syntax
+Author: Adam Hupp
+Author-email: adam@hupp.org
+Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pint (>0.20)
+Requires-Dist: ipython (>=7)
+Requires-Dist: pegen (>=0.2,<0.3)
+Project-URL: Repository, https://github.com/ahupp/unit-syntax
+Description-Content-Type: text/markdown
+
 `unit-syntax` adds support for physical units to the Python language:
 
 ```python
 >>> speed = 5 meters/second
 >>> (2 seconds) * speed
 10 meter
 ```
 
-Why? I often use Python as an interactive calculator for physical problems, and wished it had the type safety of explicit units along with the readability of normal notation.
+Why? I often use Python as an interactive calculator for physical problems and wished it had the type safety of explicit units along with the readability of normal notation.
 
 `unit-syntax` currently supports Jupyter notebooks and the IPython interpreter; maybe someday support for standalone scripts.
 
 [How does it work?](#how-does-it-work)
 
 ## Getting Started
 
@@ -19,15 +38,15 @@
 ```shell
 $ pip install unit-syntax
 ```
 
 To enable unit-syntax in a Jupyter/IPython session run:
 
 ```python
-import unit_syntax.ipython
+%load_ext unit_syntax
 ```
 
 Tip: In Jupyter this must be run in its own cell before any units expressions are evaluated.
 
 ## Usage
 
 [An interactive notebook to play around with units](https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV)
@@ -82,38 +101,26 @@
 
 ## How does it work?
 
 The parser is [pegen](https://we-like-parsers.github.io/pegen/), which is the same parser generator used by Python itself. The grammar is a lightly modified version the official Python grammar.
 
 Syntax transformation in IPython/Jupyter uses [IPython custom input transformers](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html).
 
-````python
-
-An IPython [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) parses the new syntax using a modified version of the official Python grammar, and translates it into calls to the excellent [Pint](https://pint.readthedocs.io/) units library.
-
 ## Why only allow units on simple expressions?
 
-The rule for applying units only to "simple" expressions rather than treating it as a typical operator is to avoid unintentional error. Imagine units were instead parsed as operator with high precedence and you wrote this reasonable looking expression:
+Imagine units were instead parsed as operator with high precedence and you wrote this reasonable looking expression:
 
 ```python
 ppi = 300 pixels/inch
 y = x inches * ppi
-````
-
-`inches * ppi` would be parsed as the unit, leading to (at best) a runtime error sometime later and at worst an incorrect calculation. This could be avoided by parenthesizing the expression (e.g. `(x inches) * ppi`, but in general it's too error prone to allow free intermixing of operators and units. (Note: This is not a hypoethical concern, I hit this within 10 minutes of first trying out the idea)
-
-## Help!
-
-If you're getting an unexpected result, try using `unit_syntax.enable_ipython(debug_transform=True)`. This will log the transformed Python code to the console.
+```
 
-If you're stuck, feel free to open an issue.
+`inches * ppi` would be parsed as the unit, leading to (at best) a runtime error sometime later and at worst an incorrect calculation. This could be avoided by parenthesizing the expression (e.g. `(x inches) * ppi`, but in general it's too error prone to allow free intermixing of operators and units. (Note: This is not a hypothical concern, I hit this within 10 minutes of first trying out the idea)
 
-## How does it work?
-
-The parser is derived from the official Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself. The transformer hooks into IPython/Jupyter using [custom input transformers](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html).
+It's easy to detect units used when they aren't allowed (that syntax isn't valid anywhere else), but not generally possible to determine if you forgot parens or meant to write a unit.
 
 ## Prior Art
 
 The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf) from Sun Microsystems. Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
 
 F# (an OCaml derivative from Microsoft) also [has first class support for units](https://en.wikibooks.org/wiki/F_Sharp_Programming/Units_of_Measure).
 
@@ -139,7 +146,9 @@
 - Test against various ipython and python versions
 - Support standalone scripts through sys.meta_path
 - Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
 - Expand the demo Colab notebook
 - Typography of output
 - make it work with numba
 - understand how numpy interop works
+- pre-parse units
+
```

### Comparing `unit_syntax-0.2.1/pyproject.toml` & `unit_syntax-0.2.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unit-syntax"
-version = "0.2.1"
+version = "0.2.2"
 authors = ["Adam Hupp <adam@hupp.org>"]
 packages = [{ include = "unit_syntax" }]
 readme = "README.md"
 repository = "https://github.com/ahupp/unit-syntax"
 description = "Physical unit literals for Jupyter and IPython"
 
 [tool.poetry.dependencies]
```

### Comparing `unit_syntax-0.2.1/unit_syntax/parser.py` & `unit_syntax-0.2.2/unit_syntax/parser.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.2.1/unit_syntax/transform.py` & `unit_syntax-0.2.2/unit_syntax/transform.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import ast
-from io import StringIO
-from typing import Iterator, Optional, Generator
 from .parser import parse_string, UnitsExpr
 import pint
-from pprint import pprint
 
 
 class UnitExprTransformer(ast.NodeTransformer):
+    """
+    AST transformer to turn python-with-units into standard python
+    """
+
     ureg: pint.UnitRegistry
 
     def __init__(self, ureg: pint.UnitRegistry):
         self.ureg = ureg
 
     def generic_visit(self, node):
         if isinstance(node, UnitsExpr):
@@ -18,33 +19,23 @@
             try:
                 self.ureg.parse_units(node.units.value)
             except pint.UndefinedUnitError as e:
                 raise SyntaxError(e)
 
             value = self.generic_visit(node.value)
             return ast.Call(
-                func=ast.Attribute(
-                    ast.Name(id="unit_syntax", ctx=ast.Load()),
-                    "Quantity",
-                    ctx=ast.Load(),
-                ),
+                ast.Name(id="_unit_syntax_q", ctx=ast.Load()),
                 args=[value, node.units],
                 keywords=[],
             )
         else:
             return super().generic_visit(node)
 
 
 def transform(code: str) -> str:
     """Transform a string of python-with-units into a standard python string"""
 
     tree = parse_string(code, mode="file")
-    ureg = pint.UnitRegistry()
+    ureg = pint._DEFAULT_REGISTRY
     tree_std = UnitExprTransformer(ureg).visit(tree)
     tree_std = ast.fix_missing_locations(tree_std)
     return ast.unparse(tree_std)
-
-
-def transform_lines(lines: list[str]) -> list[str]:
-    """IPython transforms provide a list of strings in the current cell, but to parse correctly we
-    need to parse them as a single string"""
-    return transform("".join(lines)).splitlines(keepends=True)
```

### Comparing `unit_syntax-0.2.1/PKG-INFO` & `unit_syntax-0.2.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,16 @@
-Metadata-Version: 2.1
-Name: unit-syntax
-Version: 0.2.1
-Summary: Physical unit literals for Jupyter and IPython
-Home-page: https://github.com/ahupp/unit-syntax
-Author: Adam Hupp
-Author-email: adam@hupp.org
-Requires-Python: >=3.8,<4
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pint (>0.20)
-Requires-Dist: ipython (>=7)
-Requires-Dist: pegen (>=0.2,<0.3)
-Project-URL: Repository, https://github.com/ahupp/unit-syntax
-Description-Content-Type: text/markdown
-
 `unit-syntax` adds support for physical units to the Python language:
 
 ```python
 >>> speed = 5 meters/second
 >>> (2 seconds) * speed
 10 meter
 ```
 
-Why? I often use Python as an interactive calculator for physical problems, and wished it had the type safety of explicit units along with the readability of normal notation.
+Why? I often use Python as an interactive calculator for physical problems and wished it had the type safety of explicit units along with the readability of normal notation.
 
 `unit-syntax` currently supports Jupyter notebooks and the IPython interpreter; maybe someday support for standalone scripts.
 
 [How does it work?](#how-does-it-work)
 
 ## Getting Started
 
@@ -38,15 +19,15 @@
 ```shell
 $ pip install unit-syntax
 ```
 
 To enable unit-syntax in a Jupyter/IPython session run:
 
 ```python
-import unit_syntax.ipython
+%load_ext unit_syntax
 ```
 
 Tip: In Jupyter this must be run in its own cell before any units expressions are evaluated.
 
 ## Usage
 
 [An interactive notebook to play around with units](https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV)
@@ -101,38 +82,26 @@
 
 ## How does it work?
 
 The parser is [pegen](https://we-like-parsers.github.io/pegen/), which is the same parser generator used by Python itself. The grammar is a lightly modified version the official Python grammar.
 
 Syntax transformation in IPython/Jupyter uses [IPython custom input transformers](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html).
 
-````python
-
-An IPython [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) parses the new syntax using a modified version of the official Python grammar, and translates it into calls to the excellent [Pint](https://pint.readthedocs.io/) units library.
-
 ## Why only allow units on simple expressions?
 
-The rule for applying units only to "simple" expressions rather than treating it as a typical operator is to avoid unintentional error. Imagine units were instead parsed as operator with high precedence and you wrote this reasonable looking expression:
+Imagine units were instead parsed as operator with high precedence and you wrote this reasonable looking expression:
 
 ```python
 ppi = 300 pixels/inch
 y = x inches * ppi
-````
-
-`inches * ppi` would be parsed as the unit, leading to (at best) a runtime error sometime later and at worst an incorrect calculation. This could be avoided by parenthesizing the expression (e.g. `(x inches) * ppi`, but in general it's too error prone to allow free intermixing of operators and units. (Note: This is not a hypoethical concern, I hit this within 10 minutes of first trying out the idea)
-
-## Help!
-
-If you're getting an unexpected result, try using `unit_syntax.enable_ipython(debug_transform=True)`. This will log the transformed Python code to the console.
+```
 
-If you're stuck, feel free to open an issue.
+`inches * ppi` would be parsed as the unit, leading to (at best) a runtime error sometime later and at worst an incorrect calculation. This could be avoided by parenthesizing the expression (e.g. `(x inches) * ppi`, but in general it's too error prone to allow free intermixing of operators and units. (Note: This is not a hypothical concern, I hit this within 10 minutes of first trying out the idea)
 
-## How does it work?
-
-The parser is derived from the official Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself. The transformer hooks into IPython/Jupyter using [custom input transformers](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html).
+It's easy to detect units used when they aren't allowed (that syntax isn't valid anywhere else), but not generally possible to determine if you forgot parens or meant to write a unit.
 
 ## Prior Art
 
 The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf) from Sun Microsystems. Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
 
 F# (an OCaml derivative from Microsoft) also [has first class support for units](https://en.wikibooks.org/wiki/F_Sharp_Programming/Units_of_Measure).
 
@@ -158,8 +127,8 @@
 - Test against various ipython and python versions
 - Support standalone scripts through sys.meta_path
 - Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
 - Expand the demo Colab notebook
 - Typography of output
 - make it work with numba
 - understand how numpy interop works
-
+- pre-parse units
```

