# Comparing `tmp/prettynumbers-0.3.4.tar.gz` & `tmp/prettynumbers-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.3.4.tar", max compression
+gzip compressed data, was "prettynumbers-0.3.5.tar", max compression
```

## Comparing `prettynumbers-0.3.4.tar` & `prettynumbers-0.3.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    14849 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/LICENSE.txt
--rw-r--r--   0        0        0     1138 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/README.md
--rw-r--r--   0        0        0      138 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/pretty_numbers/__init__.py
--rwxr-xr-x   0        0        0     2580 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/pretty_numbers/pretty_numbers.py
--rw-r--r--   0        0        0        0 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/pretty_numbers/py.typed
--rw-r--r--   0        0        0      808 2023-07-20 12:42:03.540660 prettynumbers-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 prettynumbers-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    14849 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/LICENSE.txt
+-rw-r--r--   0        0        0     1138 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/README.md
+-rw-r--r--   0        0        0      138 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/pretty_numbers/__init__.py
+-rwxr-xr-x   0        0        0     2580 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/pretty_numbers/pretty_numbers.py
+-rw-r--r--   0        0        0        0 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/pretty_numbers/py.typed
+-rw-r--r--   0        0        0      807 2023-07-26 08:59:46.080920 prettynumbers-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 prettynumbers-0.3.5/PKG-INFO
```

### Comparing `prettynumbers-0.3.4/LICENSE.txt` & `prettynumbers-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.4/README.md` & `prettynumbers-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.4/pretty_numbers/pretty_numbers.py` & `prettynumbers-0.3.5/pretty_numbers/pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.3.4/pyproject.toml` & `prettynumbers-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prettynumbers"
-version = "0.3.4"
+version = "0.3.5"
 authors = ["gerardk <gerardk@gmail.com>"]
 description="Display a range of numbers in a human readable way"
 license="GNU GENERAL PUBLIC LICENSE"
 packages = [{include = "pretty_numbers"}]
 readme = "README.md"
 repository = "https://github.com/vfxGer/pretty-numbers"
 
@@ -12,15 +12,15 @@
 python = "^3.8.0"
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^2.17.3"
 isort = "^5.12.0"
 nose = "^1.3.7"
 codecov = "^2.1.12"
-black = "^21.11b1"
+black = "^22.3.0"
 mypy = "^0.910"
 twine = "^3.6.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `prettynumbers-0.3.4/PKG-INFO` & `prettynumbers-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.3.4
+Version: 0.3.5
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
 License: GNU GENERAL PUBLIC LICENSE
 Author: gerardk
 Author-email: gerardk@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: Other/Proprietary License
```

