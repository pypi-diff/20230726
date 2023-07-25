# Comparing `tmp/task3-0.1.4.tar.gz` & `tmp/task3-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task3-0.1.4.tar", max compression
+gzip compressed data, was "task3-1.0.3.tar", max compression
```

## Comparing `task3-0.1.4.tar` & `task3-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task3-0.1.4/LICENSE
--rw-r--r--   0        0        0      300 2023-07-21 16:40:54.009144 task3-0.1.4/parse_xsv/__init__.py
--rw-r--r--   0        0        0      116 2023-07-12 14:27:57.699438 task3-0.1.4/parse_xsv/__main__.py
--rw-r--r--   0        0        0       23 2023-07-24 20:01:57.866941 task3-0.1.4/parse_xsv/__version__.py
--rw-r--r--   0        0        0      187 2023-07-23 21:21:28.183243 task3-0.1.4/parse_xsv/cli/__init__.py
--rw-r--r--   0        0        0      116 2023-07-12 14:27:57.680442 task3-0.1.4/parse_xsv/cli/__main__.py
--rw-r--r--   0        0        0    17423 2023-07-24 19:58:50.624510 task3-0.1.4/parse_xsv/cli/cli.py
--rw-r--r--   0        0        0    12813 2023-07-24 19:56:50.742584 task3-0.1.4/parse_xsv/parse_xsv.py
--rw-r--r--   0        0        0      113 2023-07-15 09:18:39.572916 task3-0.1.4/parse_xsv/sample_gen/__init__.py
--rw-r--r--   0        0        0      143 2023-07-15 09:18:39.582913 task3-0.1.4/parse_xsv/sample_gen/__main__.py
--rw-r--r--   0        0        0     8109 2023-07-24 20:00:04.379744 task3-0.1.4/parse_xsv/sample_gen/sample_gen.py
--rw-r--r--   0        0        0       97 2023-07-12 14:27:57.666460 task3-0.1.4/parse_xsv/showcase/__init__.py
--rw-r--r--   0        0        0      138 2023-07-12 14:27:57.687500 task3-0.1.4/parse_xsv/showcase/__main__.py
--rw-r--r--   0        0        0    25805 2023-07-24 17:03:10.652441 task3-0.1.4/parse_xsv/showcase/corrupted_sample.csv
--rw-r--r--   0        0        0    29527 2023-07-24 15:54:36.768020 task3-0.1.4/parse_xsv/showcase/sample.csv
--rw-r--r--   0        0        0    29527 2023-07-24 16:01:30.014978 task3-0.1.4/parse_xsv/showcase/sample.tsv
--rw-r--r--   0        0        0    22754 2023-07-24 19:26:22.674171 task3-0.1.4/parse_xsv/showcase/showcase.py
--rw-r--r--   0        0        0      577 2023-07-24 20:01:57.871941 task3-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    17428 2023-07-11 12:14:12.015389 task3-0.1.4/README.md
--rw-r--r--   0        0        0    17733 1970-01-01 00:00:00.000000 task3-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task3-1.0.3/LICENSE
+-rw-r--r--   0        0        0      300 2023-07-21 16:40:54.009144 task3-1.0.3/parse_xsv/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-12 14:27:57.699438 task3-1.0.3/parse_xsv/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-25 22:44:57.358938 task3-1.0.3/parse_xsv/__version__.py
+-rw-r--r--   0        0        0      187 2023-07-23 21:21:28.183243 task3-1.0.3/parse_xsv/cli/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-12 14:27:57.680442 task3-1.0.3/parse_xsv/cli/__main__.py
+-rw-r--r--   0        0        0    17423 2023-07-24 19:58:50.624510 task3-1.0.3/parse_xsv/cli/cli.py
+-rw-r--r--   0        0        0    12813 2023-07-24 19:56:50.742584 task3-1.0.3/parse_xsv/parse_xsv.py
+-rw-r--r--   0        0        0      113 2023-07-15 09:18:39.572916 task3-1.0.3/parse_xsv/sample_gen/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-15 09:18:39.582913 task3-1.0.3/parse_xsv/sample_gen/__main__.py
+-rw-r--r--   0        0        0     8109 2023-07-24 20:00:04.379744 task3-1.0.3/parse_xsv/sample_gen/sample_gen.py
+-rw-r--r--   0        0        0       97 2023-07-12 14:27:57.666460 task3-1.0.3/parse_xsv/showcase/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-12 14:27:57.687500 task3-1.0.3/parse_xsv/showcase/__main__.py
+-rw-r--r--   0        0        0    25805 2023-07-24 17:03:10.652441 task3-1.0.3/parse_xsv/showcase/corrupted_sample.csv
+-rw-r--r--   0        0        0    29527 2023-07-24 15:54:36.768020 task3-1.0.3/parse_xsv/showcase/sample.csv
+-rw-r--r--   0        0        0    29527 2023-07-24 16:01:30.014978 task3-1.0.3/parse_xsv/showcase/sample.tsv
+-rw-r--r--   0        0        0    22764 2023-07-24 20:21:36.580930 task3-1.0.3/parse_xsv/showcase/showcase.py
+-rw-r--r--   0        0        0      577 2023-07-25 22:44:42.027372 task3-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    26061 2023-07-25 22:43:44.856072 task3-1.0.3/README.md
+-rw-r--r--   0        0        0    26182 1970-01-01 00:00:00.000000 task3-1.0.3/PKG-INFO
```

### Comparing `task3-0.1.4/parse_xsv/cli/cli.py` & `task3-1.0.3/parse_xsv/cli/cli.py`

 * *Files identical despite different names*

### Comparing `task3-0.1.4/parse_xsv/parse_xsv.py` & `task3-1.0.3/parse_xsv/parse_xsv.py`

 * *Files identical despite different names*

### Comparing `task3-0.1.4/parse_xsv/sample_gen/sample_gen.py` & `task3-1.0.3/parse_xsv/sample_gen/sample_gen.py`

 * *Files identical despite different names*

### Comparing `task3-0.1.4/parse_xsv/showcase/corrupted_sample.csv` & `task3-1.0.3/parse_xsv/showcase/corrupted_sample.csv`

 * *Files identical despite different names*

### Comparing `task3-0.1.4/parse_xsv/showcase/sample.csv` & `task3-1.0.3/parse_xsv/showcase/sample.csv`

 * *Files identical despite different names*

### Comparing `task3-0.1.4/parse_xsv/showcase/sample.tsv` & `task3-1.0.3/parse_xsv/showcase/sample.tsv`

 * *Files identical despite different names*

### Comparing `task3-0.1.4/parse_xsv/showcase/showcase.py` & `task3-1.0.3/parse_xsv/showcase/showcase.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,15 @@
         'descr': 're',
         'type': 'select',
         'name': 'regex',
         'message': 'Which regular expression would you like to choose?',
         'choices': [Choice(title=val.name, value=val.name) for val in RegexPatterns],
         'instruction': '(Use arrow keys to navigate through the menu)',
         'pointer': '>',
-        'default': RegexPatterns.IP4.name,
+        'filter': lambda val: val if val else 'IP4',
         'use_shortcuts': True,
     },
     'j': {
         'descr': 'j',
         'type': 'confirm',
         'message': 'Would you like to output in JSON format?',
         'default': False,
```

### Comparing `task3-0.1.4/pyproject.toml` & `task3-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "task3"
-version = "0.1.4"
+version = "1.0.3"
 description = "xSV file parser CLI and library"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "parse_xsv"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

