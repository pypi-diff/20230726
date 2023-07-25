# Comparing `tmp/shell_whiz-0.1.8.tar.gz` & `tmp/shell_whiz-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_whiz-0.1.8.tar", max compression
+gzip compressed data, was "shell_whiz-0.1.9.tar", max compression
```

## Comparing `shell_whiz-0.1.8.tar` & `shell_whiz-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-07-25 22:34:11.922033 shell_whiz-0.1.8/LICENSE
--rw-r--r--   0        0        0     3259 2023-07-25 22:34:11.922033 shell_whiz-0.1.8/README.md
--rw-r--r--   0        0        0      538 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4186 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/__init__.py
--rw-r--r--   0        0        0       58 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/__main__.py
--rw-r--r--   0        0        0     1686 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/config.py
--rw-r--r--   0        0        0      378 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/constants.py
--rw-r--r--   0        0        0      108 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/exceptions.py
--rw-r--r--   0        0        0     8293 2023-07-25 22:34:11.926033 shell_whiz-0.1.8/shell_whiz/openai.py
--rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 shell_whiz-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-25 22:37:50.555686 shell_whiz-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3305 2023-07-25 22:37:50.555686 shell_whiz-0.1.9/README.md
+-rw-r--r--   0        0        0      538 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4186 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/__init__.py
+-rw-r--r--   0        0        0       58 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/__main__.py
+-rw-r--r--   0        0        0     1686 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/config.py
+-rw-r--r--   0        0        0      378 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/constants.py
+-rw-r--r--   0        0        0      108 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/exceptions.py
+-rw-r--r--   0        0        0     8293 2023-07-25 22:37:50.559686 shell_whiz-0.1.9/shell_whiz/openai.py
+-rw-r--r--   0        0        0     3906 1970-01-01 00:00:00.000000 shell_whiz-0.1.9/PKG-INFO
```

### Comparing `shell_whiz-0.1.8/LICENSE` & `shell_whiz-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.8/README.md` & `shell_whiz-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <p align="center">
-  <img src="./images/shell-whiz.png" />
+  <img src="https://github.com/beimzhan/shell-whiz/raw/main/images/shell-whiz.png" />
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/pypi/v/shell-whiz" alt="PyPI" />
   <img src="https://img.shields.io/pypi/dm/shell-whiz" alt="PyPI - Downloads" />
   <img
     src="https://img.shields.io/github/stars/beimzhan/shell-whiz"
```

### Comparing `shell_whiz-0.1.8/pyproject.toml` & `shell_whiz-0.1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shell-whiz"
-version = "0.1.8"
+version = "0.1.9"
 description = "Shell Whiz: AI assistant right in your terminal"
 authors = ["Tamerlan Bimzhanov <bimzhanovt.net@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shell_whiz"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `shell_whiz-0.1.8/shell_whiz/__init__.py` & `shell_whiz-0.1.9/shell_whiz/__init__.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.8/shell_whiz/config.py` & `shell_whiz-0.1.9/shell_whiz/config.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.8/shell_whiz/openai.py` & `shell_whiz-0.1.9/shell_whiz/openai.py`

 * *Files identical despite different names*

### Comparing `shell_whiz-0.1.8/PKG-INFO` & `shell_whiz-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-whiz
-Version: 0.1.8
+Version: 0.1.9
 Summary: Shell Whiz: AI assistant right in your terminal
 Author: Tamerlan Bimzhanov
 Author-email: bimzhanovt.net@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
@@ -12,15 +12,15 @@
 Requires-Dist: jsonschema (>=4.18.4,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: prompt-toolkit (>=3.0.39,<4.0.0)
 Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
-  <img src="./images/shell-whiz.png" />
+  <img src="https://github.com/beimzhan/shell-whiz/raw/main/images/shell-whiz.png" />
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/pypi/v/shell-whiz" alt="PyPI" />
   <img src="https://img.shields.io/pypi/dm/shell-whiz" alt="PyPI - Downloads" />
   <img
     src="https://img.shields.io/github/stars/beimzhan/shell-whiz"
```

