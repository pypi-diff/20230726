# Comparing `tmp/e2xcore-0.0.1.tar.gz` & `tmp/e2xcore-0.0.2.tar.gz`

## Comparing `e2xcore-0.0.1.tar` & `e2xcore-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,18 @@
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/content/28e32ca0ac5f358
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/content/3c52bb72a04b6bd9
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/content/44ecbf6b468661d7
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/content/621e93c67b18efc9
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/content/81b832535905bf56
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/content/83081bac811ca6b2
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/content/9cd1d6bbd710c3e3
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/content/a15ab731fb008f6d
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/content/a55ee5d2fa9e5bbd
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.ruff_cache/content/c3cc4a7b099c5848
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 e2xcore-0.0.1/e2xcore/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 e2xcore-0.0.1/e2xcore/__version__.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 e2xcore-0.0.1/e2xcore/app.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 e2xcore-0.0.1/e2xcore/utils.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 e2xcore-0.0.1/e2xcore/handlers/__init__.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 e2xcore-0.0.1/e2xcore/handlers/base.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 e2xcore-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xcore-0.0.1/LICENSE
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 e2xcore-0.0.1/README.md
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 e2xcore-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 e2xcore-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 e2xcore-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/__version__.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/api/__init__.py
+-rw-r--r--   0        0        0    14279 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/api/api.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/app/__init__.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/app/app.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/handlers/__init__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/handlers/base.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/utils/__init__.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/utils/e2xgrader_cells.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/utils/nbgrader_cells.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 e2xcore-0.0.2/e2xcore/utils/utils.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 e2xcore-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xcore-0.0.2/LICENSE
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 e2xcore-0.0.2/README.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 e2xcore-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 e2xcore-0.0.2/PKG-INFO
```

### Comparing `e2xcore-0.0.1/e2xcore/app.py` & `e2xcore-0.0.2/e2xcore/app/app.py`

 * *Files identical despite different names*

### Comparing `e2xcore-0.0.1/e2xcore/utils.py` & `e2xcore-0.0.2/e2xcore/utils/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 import re
 from typing import Any, Dict, List
 from urllib.parse import parse_qsl, urlencode, urlparse
 
+from nbgrader.apps import NbGrader
+
+
+def get_nbgrader_config():
+    nbgrader = NbGrader()
+    nbgrader.initialize([])
+    return nbgrader.config
+
 
 def format_url(url: str, params: Dict[str, Any]) -> str:
     """Join a url with search parameters
 
     Args:
         url (str): The url
         params (Dict[str, Any]): A dictionary of parameters
```

### Comparing `e2xcore-0.0.1/.gitignore` & `e2xcore-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `e2xcore-0.0.1/LICENSE` & `e2xcore-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `e2xcore-0.0.1/pyproject.toml` & `e2xcore-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
+    "nbgrader>=0.7,<0.9",
     "notebook>=6,<7",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://e2x.inf.h-brs.de"
 Issues = "https://github.com/Digiklausur/e2xcore/issues"
@@ -40,15 +41,15 @@
 path = "e2xcore/__version__.py"
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
-current = "0.0.1"
+current = "0.0.2"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `e2xcore-0.0.1/PKG-INFO` & `e2xcore-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: e2xcore
-Version: 0.0.1
+Version: 0.0.2
 Summary: An template for a server app for e2xgrader
 Project-URL: Documentation, https://e2x.inf.h-brs.de
 Project-URL: Issues, https://github.com/Digiklausur/e2xcore/issues
 Project-URL: Source, https://github.com/Digiklausur/e2xcore
 Author-email: Tim Metzler <tim.metzler@h-brs.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
+Requires-Dist: nbgrader<0.9,>=0.7
 Requires-Dist: notebook<7,>=6
 Provides-Extra: dev
 Requires-Dist: hatchling; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: tbump; extra == 'dev'
 Description-Content-Type: text/markdown
```

