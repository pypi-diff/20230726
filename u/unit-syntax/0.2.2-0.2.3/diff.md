# Comparing `tmp/unit_syntax-0.2.2.tar.gz` & `tmp/unit_syntax-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_syntax-0.2.2.tar", max compression
+gzip compressed data, was "unit_syntax-0.2.3.tar", max compression
```

## Comparing `unit_syntax-0.2.2.tar` & `unit_syntax-0.2.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4687 2023-07-26 06:37:09.664332 unit_syntax-0.2.2/README.md
--rw-r--r--   0        0        0      644 2023-07-26 06:37:09.664332 unit_syntax-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      283 2023-07-26 06:37:09.668332 unit_syntax-0.2.2/unit_syntax/__init__.py
--rw-r--r--   0        0        0     2033 2023-07-26 06:37:09.668332 unit_syntax-0.2.2/unit_syntax/ipython.py
--rw-r--r--   0        0        0   333763 2023-07-26 06:37:09.668332 unit_syntax-0.2.2/unit_syntax/parser.py
--rw-r--r--   0        0        0     1195 2023-07-26 06:37:09.668332 unit_syntax-0.2.2/unit_syntax/transform.py
--rw-r--r--   0        0        0     5363 1970-01-01 00:00:00.000000 unit_syntax-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4687 2023-07-26 06:58:59.164708 unit_syntax-0.2.3/README.md
+-rw-r--r--   0        0        0      644 2023-07-26 06:58:59.164708 unit_syntax-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-07-26 06:58:59.164708 unit_syntax-0.2.3/unit_syntax/__init__.py
+-rw-r--r--   0        0        0     2018 2023-07-26 06:58:59.164708 unit_syntax-0.2.3/unit_syntax/ipython.py
+-rw-r--r--   0        0        0   333763 2023-07-26 06:58:59.164708 unit_syntax-0.2.3/unit_syntax/parser.py
+-rw-r--r--   0        0        0     1195 2023-07-26 06:58:59.164708 unit_syntax-0.2.3/unit_syntax/transform.py
+-rw-r--r--   0        0        0     5363 1970-01-01 00:00:00.000000 unit_syntax-0.2.3/PKG-INFO
```

### Comparing `unit_syntax-0.2.2/README.md` & `unit_syntax-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.2.2/pyproject.toml` & `unit_syntax-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unit-syntax"
-version = "0.2.2"
+version = "0.2.3"
 authors = ["Adam Hupp <adam@hupp.org>"]
 packages = [{ include = "unit_syntax" }]
 readme = "README.md"
 repository = "https://github.com/ahupp/unit-syntax"
 description = "Physical unit literals for Jupyter and IPython"
 
 [tool.poetry.dependencies]
```

### Comparing `unit_syntax-0.2.2/unit_syntax/ipython.py` & `unit_syntax-0.2.3/unit_syntax/ipython.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .transform import transform
 import pint
+import logging
 
 
 def _add_formatters(ipython):
     # Overide default formatters to use reduced units.  This lets us keep using the
     # default registry for interop with other pint-using libraries, but gives more
     # sensible output in the notebook.
     def add_formatter(mime, display_fn_name):
@@ -33,39 +34,33 @@
     return transform("".join(lines)).splitlines(keepends=True)
 
 
 def ipython_transform(lines):
     ret = transform_lines(lines)
 
     if _debug:
-        import logging
-
         global _has_init_log
         if not _has_init_log:
             logging.basicConfig(level=logging.DEBUG, force=True)
         _has_init_log = True
         logging.debug("unit_syntax: %s -> %s", "\n".join(lines), "\n".join(ret))
     return ret
 
 
 def load_ipython_extension(ipython):
+    logging.debug("unit_syntax: loading extension")
+
     if not hasattr(ipython, "input_transformers_post"):
         raise ImportError("Unsupported IPython version, version >=7 is required")
 
     ipython.input_transformers_post.append(ipython_transform)
 
     _add_formatters(ipython)
 
     from . import BOOTSTRAP
 
     ipython.run_cell(BOOTSTRAP)
 
-    try:
-        import matplotlib
-
-        pint.setup_matplotlib(True)
-    except ImportError:
-        pass
-
 
 def unload_ipython_extension(ipython):
+    logging.debug("unit_syntax: unload extension")
     ipython.input_transformers_post.remove(ipython_transform)
```

### Comparing `unit_syntax-0.2.2/unit_syntax/parser.py` & `unit_syntax-0.2.3/unit_syntax/parser.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.2.2/unit_syntax/transform.py` & `unit_syntax-0.2.3/unit_syntax/transform.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.2.2/PKG-INFO` & `unit_syntax-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unit-syntax
-Version: 0.2.2
+Version: 0.2.3
 Summary: Physical unit literals for Jupyter and IPython
 Home-page: https://github.com/ahupp/unit-syntax
 Author: Adam Hupp
 Author-email: adam@hupp.org
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

