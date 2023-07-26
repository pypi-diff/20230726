# Comparing `tmp/unit_syntax-0.2.0.tar.gz` & `tmp/unit_syntax-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_syntax-0.2.0.tar", max compression
+gzip compressed data, was "unit_syntax-0.2.1.tar", max compression
```

## Comparing `unit_syntax-0.2.0.tar` & `unit_syntax-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     4894 2023-07-25 01:01:25.036554 unit_syntax-0.2.0/README.md
--rw-r--r--   0        0        0      644 2023-07-25 01:01:25.036554 unit_syntax-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2104 2023-07-25 01:01:25.036554 unit_syntax-0.2.0/unit_syntax/__init__.py
--rw-r--r--   0        0        0   149661 2023-07-25 01:01:25.036554 unit_syntax-0.2.0/unit_syntax/parser.py
--rw-r--r--   0        0        0     5039 2023-07-25 01:01:25.036554 unit_syntax-0.2.0/unit_syntax/transform.py
--rw-r--r--   0        0        0     5570 1970-01-01 00:00:00.000000 unit_syntax-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     5471 2023-07-26 03:41:02.897945 unit_syntax-0.2.1/README.md
+-rw-r--r--   0        0        0      644 2023-07-26 03:41:02.901944 unit_syntax-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2104 2023-07-26 03:41:02.901944 unit_syntax-0.2.1/unit_syntax/__init__.py
+-rw-r--r--   0        0        0       48 2023-07-26 03:41:02.901944 unit_syntax-0.2.1/unit_syntax/ipython/__init__.py
+-rw-r--r--   0        0        0   333763 2023-07-26 03:41:02.901944 unit_syntax-0.2.1/unit_syntax/parser.py
+-rw-r--r--   0        0        0     1592 2023-07-26 03:41:02.901944 unit_syntax-0.2.1/unit_syntax/transform.py
+-rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 unit_syntax-0.2.1/PKG-INFO
```

### Comparing `unit_syntax-0.2.0/README.md` & `unit_syntax-0.2.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,31 +4,30 @@
 >>> speed = 5 meters/second
 >>> (2 seconds) * speed
 10 meter
 ```
 
 Why? I often use Python as an interactive calculator for physical problems, and wished it had the type safety of explicit units along with the readability of normal notation.
 
-Where? `unit-syntax` currently supports Jupyter notebooks and the IPython interpreter; support for standalone scripts is planned.
+`unit-syntax` currently supports Jupyter notebooks and the IPython interpreter; maybe someday support for standalone scripts.
 
-How? A syntax transformer based on the official Python grammar turns these expression into calls to the excellent [Pint](https://pint.readthedocs.io/) units library.
+[How does it work?](#how-does-it-work)
 
 ## Getting Started
 
 Install the package:
 
 ```shell
 $ pip install unit-syntax
 ```
 
 To enable unit-syntax in a Jupyter/IPython session run:
 
 ```python
-import unit_syntax
-unit_syntax.enable_ipython()
+import unit_syntax.ipython
 ```
 
 Tip: In Jupyter this must be run in its own cell before any units expressions are evaluated.
 
 ## Usage
 
 [An interactive notebook to play around with units](https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV)
@@ -37,21 +36,21 @@
 
 - number: `1 meter`
 - variables: `x parsec`, `y.z watts`, `area[id] meters**2`
 - lists and tuples: `[1., 37.] newton meters`
 - unary operators: `-x dBm`
 - power: `x**2 meters`
 
-To apply units within a more complex expression, use parentheses:
+In expressions mixing units and binary operators, parenthesize:
 
 ```python
 one_lux = (1 lumen)/(1 meter**2)
 ```
 
-Units can be used in other places where Python allows expressions like:
+Units can be used in any place where Python allows expressions, e.g:
 
 - function arguments: `area_of_circle(radius=1 meter)`
 - list comprehensions: `[x meters for x in range(10)]`
 
 Quantities can be converted to another measurement system:
 
 ```python
@@ -69,22 +68,40 @@
 ```python
 # parsed as a function call, will result in a runtime error
 x (newton meters)/(second*kg)
 # a-ok
 x newton meters/(second*kg)
 ```
 
+Using invalid units produces a syntax error at import time:
+
+```python
+>>> 1 smoot
+...
+SyntaxError: 'smoot' is not defined in the unit registry
+```
+
+## How does it work?
+
+The parser is [pegen](https://we-like-parsers.github.io/pegen/), which is the same parser generator used by Python itself. The grammar is a lightly modified version the official Python grammar.
+
+Syntax transformation in IPython/Jupyter uses [IPython custom input transformers](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html).
+
+````python
+
+An IPython [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) parses the new syntax using a modified version of the official Python grammar, and translates it into calls to the excellent [Pint](https://pint.readthedocs.io/) units library.
+
 ## Why only allow units on simple expressions?
 
 The rule for applying units only to "simple" expressions rather than treating it as a typical operator is to avoid unintentional error. Imagine units were instead parsed as operator with high precedence and you wrote this reasonable looking expression:
 
 ```python
 ppi = 300 pixels/inch
 y = x inches * ppi
-```
+````
 
 `inches * ppi` would be parsed as the unit, leading to (at best) a runtime error sometime later and at worst an incorrect calculation. This could be avoided by parenthesizing the expression (e.g. `(x inches) * ppi`, but in general it's too error prone to allow free intermixing of operators and units. (Note: This is not a hypoethical concern, I hit this within 10 minutes of first trying out the idea)
 
 ## Help!
 
 If you're getting an unexpected result, try using `unit_syntax.enable_ipython(debug_transform=True)`. This will log the transformed Python code to the console.
 
@@ -104,27 +121,25 @@
 
 A [long discussion on the python-ideas mailing list](https://lwn.net/Articles/900739/) about literal units in Python.
 
 ## Development
 
 To regenerate the parser:
 
-`python -m pegen grammar.txt -o unit_syntax/parser.py`
+`python -m pegen python_units.gram -o unit_syntax/parser.py`
 
 Running tests:
 
 ```
 $ poetry install --with dev
 $ poetry run pytest
 ```
 
 ## Future work and open questions
 
 - Test against various ipython and python versions
 - Support standalone scripts through sys.meta_path
-- Check units at parse time
 - Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
 - Expand the demo Colab notebook
 - Typography of output
 - make it work with numba
 - understand how numpy interop works
-- fail more clearly when units are used in an invalid location
```

### Comparing `unit_syntax-0.2.0/pyproject.toml` & `unit_syntax-0.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unit-syntax"
-version = "0.2.0"
+version = "0.2.1"
 authors = ["Adam Hupp <adam@hupp.org>"]
 packages = [{ include = "unit_syntax" }]
 readme = "README.md"
 repository = "https://github.com/ahupp/unit-syntax"
 description = "Physical unit literals for Jupyter and IPython"
 
 [tool.poetry.dependencies]
```

### Comparing `unit_syntax-0.2.0/unit_syntax/__init__.py` & `unit_syntax-0.2.1/unit_syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.2.0/PKG-INFO` & `unit_syntax-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unit-syntax
-Version: 0.2.0
+Version: 0.2.1
 Summary: Physical unit literals for Jupyter and IPython
 Home-page: https://github.com/ahupp/unit-syntax
 Author: Adam Hupp
 Author-email: adam@hupp.org
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -23,31 +23,30 @@
 >>> speed = 5 meters/second
 >>> (2 seconds) * speed
 10 meter
 ```
 
 Why? I often use Python as an interactive calculator for physical problems, and wished it had the type safety of explicit units along with the readability of normal notation.
 
-Where? `unit-syntax` currently supports Jupyter notebooks and the IPython interpreter; support for standalone scripts is planned.
+`unit-syntax` currently supports Jupyter notebooks and the IPython interpreter; maybe someday support for standalone scripts.
 
-How? A syntax transformer based on the official Python grammar turns these expression into calls to the excellent [Pint](https://pint.readthedocs.io/) units library.
+[How does it work?](#how-does-it-work)
 
 ## Getting Started
 
 Install the package:
 
 ```shell
 $ pip install unit-syntax
 ```
 
 To enable unit-syntax in a Jupyter/IPython session run:
 
 ```python
-import unit_syntax
-unit_syntax.enable_ipython()
+import unit_syntax.ipython
 ```
 
 Tip: In Jupyter this must be run in its own cell before any units expressions are evaluated.
 
 ## Usage
 
 [An interactive notebook to play around with units](https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV)
@@ -56,21 +55,21 @@
 
 - number: `1 meter`
 - variables: `x parsec`, `y.z watts`, `area[id] meters**2`
 - lists and tuples: `[1., 37.] newton meters`
 - unary operators: `-x dBm`
 - power: `x**2 meters`
 
-To apply units within a more complex expression, use parentheses:
+In expressions mixing units and binary operators, parenthesize:
 
 ```python
 one_lux = (1 lumen)/(1 meter**2)
 ```
 
-Units can be used in other places where Python allows expressions like:
+Units can be used in any place where Python allows expressions, e.g:
 
 - function arguments: `area_of_circle(radius=1 meter)`
 - list comprehensions: `[x meters for x in range(10)]`
 
 Quantities can be converted to another measurement system:
 
 ```python
@@ -88,22 +87,40 @@
 ```python
 # parsed as a function call, will result in a runtime error
 x (newton meters)/(second*kg)
 # a-ok
 x newton meters/(second*kg)
 ```
 
+Using invalid units produces a syntax error at import time:
+
+```python
+>>> 1 smoot
+...
+SyntaxError: 'smoot' is not defined in the unit registry
+```
+
+## How does it work?
+
+The parser is [pegen](https://we-like-parsers.github.io/pegen/), which is the same parser generator used by Python itself. The grammar is a lightly modified version the official Python grammar.
+
+Syntax transformation in IPython/Jupyter uses [IPython custom input transformers](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html).
+
+````python
+
+An IPython [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) parses the new syntax using a modified version of the official Python grammar, and translates it into calls to the excellent [Pint](https://pint.readthedocs.io/) units library.
+
 ## Why only allow units on simple expressions?
 
 The rule for applying units only to "simple" expressions rather than treating it as a typical operator is to avoid unintentional error. Imagine units were instead parsed as operator with high precedence and you wrote this reasonable looking expression:
 
 ```python
 ppi = 300 pixels/inch
 y = x inches * ppi
-```
+````
 
 `inches * ppi` would be parsed as the unit, leading to (at best) a runtime error sometime later and at worst an incorrect calculation. This could be avoided by parenthesizing the expression (e.g. `(x inches) * ppi`, but in general it's too error prone to allow free intermixing of operators and units. (Note: This is not a hypoethical concern, I hit this within 10 minutes of first trying out the idea)
 
 ## Help!
 
 If you're getting an unexpected result, try using `unit_syntax.enable_ipython(debug_transform=True)`. This will log the transformed Python code to the console.
 
@@ -123,28 +140,26 @@
 
 A [long discussion on the python-ideas mailing list](https://lwn.net/Articles/900739/) about literal units in Python.
 
 ## Development
 
 To regenerate the parser:
 
-`python -m pegen grammar.txt -o unit_syntax/parser.py`
+`python -m pegen python_units.gram -o unit_syntax/parser.py`
 
 Running tests:
 
 ```
 $ poetry install --with dev
 $ poetry run pytest
 ```
 
 ## Future work and open questions
 
 - Test against various ipython and python versions
 - Support standalone scripts through sys.meta_path
-- Check units at parse time
 - Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
 - Expand the demo Colab notebook
 - Typography of output
 - make it work with numba
 - understand how numpy interop works
-- fail more clearly when units are used in an invalid location
```

