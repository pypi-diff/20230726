# Comparing `tmp/flake8_private_name_import-0.1.2.tar.gz` & `tmp/flake8_private_name_import-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flake8_private_name_import-0.1.2.tar", last modified: Tue Jul 25 21:01:28 2023, max compression
+gzip compressed data, was "dist/flake8_private_name_import-0.1.3.tar", last modified: Wed Jul 26 18:57:01 2023, max compression
```

## Comparing `flake8_private_name_import-0.1.2.tar` & `flake8_private_name_import-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/
--rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/PKG-INFO
--rw-rw-r--   0 rows      (1000) rows      (1000)       81 2023-07-25 20:19:44.000000 flake8_private_name_import-0.1.2/README.md
-drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/
--rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/PKG-INFO
--rw-rw-r--   0 rows      (1000) rows      (1000)      399 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/SOURCES.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/dependency_links.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       63 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/entry_points.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/not-zip-safe
--rw-rw-r--   0 rows      (1000) rows      (1000)       29 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/requires.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)       27 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/top_level.txt
--rw-rw-r--   0 rows      (1000) rows      (1000)     1383 2023-07-25 21:00:14.000000 flake8_private_name_import-0.1.2/flake8_private_name_import.py
--rw-rw-r--   0 rows      (1000) rows      (1000)       38 2023-07-25 21:01:28.000000 flake8_private_name_import-0.1.2/setup.cfg
--rw-rw-r--   0 rows      (1000) rows      (1000)     1779 2023-07-25 21:00:14.000000 flake8_private_name_import-0.1.2/setup.py
+drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/PKG-INFO
+-rw-rw-r--   0 rows      (1000) rows      (1000)       81 2023-07-25 20:19:44.000000 flake8_private_name_import-0.1.3/README.md
+drwxrwxr-x   0 rows      (1000) rows      (1000)        0 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1308 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/PKG-INFO
+-rw-rw-r--   0 rows      (1000) rows      (1000)      399 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/SOURCES.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/dependency_links.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)       63 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/entry_points.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)        1 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/not-zip-safe
+-rw-rw-r--   0 rows      (1000) rows      (1000)       29 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/requires.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)       27 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/top_level.txt
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1827 2023-07-26 18:56:58.000000 flake8_private_name_import-0.1.3/flake8_private_name_import.py
+-rw-rw-r--   0 rows      (1000) rows      (1000)       38 2023-07-26 18:57:01.000000 flake8_private_name_import-0.1.3/setup.cfg
+-rw-rw-r--   0 rows      (1000) rows      (1000)     1779 2023-07-26 18:56:58.000000 flake8_private_name_import-0.1.3/setup.py
```

### Comparing `flake8_private_name_import-0.1.2/PKG-INFO` & `flake8_private_name_import-0.1.3/flake8_private_name_import.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flake8_private_name_import
-Version: 0.1.2
+Name: flake8-private-name-import
+Version: 0.1.3
 Summary: flake8 plugin that reports imports of private names
 Home-page: https://github.com/rows-s/flake8_private_name_import
 Author: Vladimir Marmuz
 Author-email: vladimir.rows@gmail.com
 License: MIT
 Description: flake8 plugin that reports imports of private names
 Keywords: python pep8 flake8 private import
```

### Comparing `flake8_private_name_import-0.1.2/flake8_private_name_import.egg-info/PKG-INFO` & `flake8_private_name_import-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: flake8-private-name-import
-Version: 0.1.2
+Name: flake8_private_name_import
+Version: 0.1.3
 Summary: flake8 plugin that reports imports of private names
 Home-page: https://github.com/rows-s/flake8_private_name_import
 Author: Vladimir Marmuz
 Author-email: vladimir.rows@gmail.com
 License: MIT
 Description: flake8 plugin that reports imports of private names
 Keywords: python pep8 flake8 private import
```

### Comparing `flake8_private_name_import-0.1.2/flake8_private_name_import.py` & `flake8_private_name_import-0.1.3/flake8_private_name_import.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 import ast
+import re
 from itertools import chain
 from typing import Any, Generator, Iterator, List, Tuple, Type
 
+SKIP_NAMES = ('__future__',)
+TEST_PATH_PATTERN = re.compile('/test|test[/.]')  # directory or file name starts or ends with 'test'
+
 
 class Visitor(ast.NodeVisitor):
-    def __init__(self) -> None:
+    def __init__(self, tree: ast.AST, file_name: str) -> None:
+        self.tree = tree
+        self.file_name = file_name
         self.reports: List[Tuple[int, int, str]] = []
 
+    def run(self) -> Iterator[Tuple[int, int, str]]:
+        if TEST_PATH_PATTERN.search(self.file_name):
+            return
+        self.visit(self.tree)
+        yield from iter(self.reports)
+
     def visit_Import(self, node: ast.Import) -> None:
         self._report_names(
             line_num=node.lineno,
             col_num=node.col_offset,
             names=chain.from_iterable(alias.name.split('.') for alias in node.names)
         )
 
@@ -21,23 +33,20 @@
             names=chain(node.module.split('.'), (alias.name for alias in node.names))
         )
 
     def _report_names(self, line_num: int, col_num: int, names: Iterator[str]) -> None:
         self.reports.extend(
             (line_num, col_num, f'PNI001 found import of private name: {name}')
             for name in names
-            if name.startswith('_')
+            if name.startswith('_') and name not in SKIP_NAMES
         )
 
 
 class Plugin:
     name = __name__
-    version = '0.1.2'
+    version = '0.1.3'
 
-    def __init__(self, tree: ast.AST) -> None:
-        self._tree = tree
+    def __init__(self, tree: ast.AST, filename: str) -> None:
+        self._visitor = Visitor(tree=tree, file_name=filename)
 
     def run(self) -> Generator[Tuple[int, int, str, Type[Any]], None, None]:
-        visitor = Visitor()
-        visitor.visit(self._tree)
-        for line_num, col_num, msg in visitor.reports:
-            yield line_num, col_num, msg, type(self)
+        yield from ((line_num, col_num, msg, type(self)) for line_num, col_num, msg in self._visitor.run())
```

### Comparing `flake8_private_name_import-0.1.2/setup.py` & `flake8_private_name_import-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='flake8_private_name_import',
-    version='0.1.2',
+    version='0.1.3',
     description="flake8 plugin that reports imports of private names",
     long_description="flake8 plugin that reports imports of private names",
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Framework :: Flake8',
```

