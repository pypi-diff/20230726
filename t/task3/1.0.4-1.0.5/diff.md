# Comparing `tmp/task3-1.0.4.tar.gz` & `tmp/task3-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "task3-1.0.4.tar", max compression
+gzip compressed data, was "task3-1.0.5.tar", max compression
```

## Comparing `task3-1.0.4.tar` & `task3-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task3-1.0.4/LICENSE
--rw-r--r--   0        0        0      300 2023-07-26 00:05:53.470730 task3-1.0.4/parse_xsv/__init__.py
--rw-r--r--   0        0        0      116 2023-07-12 14:27:57.699438 task3-1.0.4/parse_xsv/__main__.py
--rw-r--r--   0        0        0       23 2023-07-26 00:06:53.464695 task3-1.0.4/parse_xsv/__version__.py
--rw-r--r--   0        0        0      187 2023-07-26 00:05:53.470730 task3-1.0.4/parse_xsv/cli/__init__.py
--rw-r--r--   0        0        0      116 2023-07-12 14:27:57.680442 task3-1.0.4/parse_xsv/cli/__main__.py
--rw-r--r--   0        0        0    17129 2023-07-26 00:05:53.471734 task3-1.0.4/parse_xsv/cli/cli.py
--rw-r--r--   0        0        0     8080 2023-07-26 00:05:53.471734 task3-1.0.4/parse_xsv/parse_xsv.py
--rw-r--r--   0        0        0      113 2023-07-26 00:05:53.472731 task3-1.0.4/parse_xsv/sample_gen/__init__.py
--rw-r--r--   0        0        0      143 2023-07-26 00:05:53.472731 task3-1.0.4/parse_xsv/sample_gen/__main__.py
--rw-r--r--   0        0        0     8109 2023-07-26 00:05:53.472731 task3-1.0.4/parse_xsv/sample_gen/sample_gen.py
--rw-r--r--   0        0        0       97 2023-07-12 14:27:57.666460 task3-1.0.4/parse_xsv/showcase/__init__.py
--rw-r--r--   0        0        0      138 2023-07-12 14:27:57.687500 task3-1.0.4/parse_xsv/showcase/__main__.py
--rw-r--r--   0        0        0    25805 2023-07-26 00:05:53.473731 task3-1.0.4/parse_xsv/showcase/corrupted_sample.csv
--rw-r--r--   0        0        0    29527 2023-07-26 00:05:53.474731 task3-1.0.4/parse_xsv/showcase/sample.csv
--rw-r--r--   0        0        0    29527 2023-07-26 00:05:53.474731 task3-1.0.4/parse_xsv/showcase/sample.tsv
--rw-r--r--   0        0        0    22764 2023-07-26 00:05:53.475731 task3-1.0.4/parse_xsv/showcase/showcase.py
--rw-r--r--   0        0        0      577 2023-07-26 00:06:53.460700 task3-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    26059 2023-07-26 00:05:53.339728 task3-1.0.4/README.md
--rw-r--r--   0        0        0    26180 1970-01-01 00:00:00.000000 task3-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      466 2023-07-08 14:31:48.331141 task3-1.0.5/LICENSE
+-rw-r--r--   0        0        0      300 2023-07-26 00:05:53.470730 task3-1.0.5/parse_xsv/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-12 14:27:57.699438 task3-1.0.5/parse_xsv/__main__.py
+-rw-r--r--   0        0        0       23 2023-07-26 01:06:33.414344 task3-1.0.5/parse_xsv/__version__.py
+-rw-r--r--   0        0        0      187 2023-07-26 00:05:53.470730 task3-1.0.5/parse_xsv/cli/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-12 14:27:57.680442 task3-1.0.5/parse_xsv/cli/__main__.py
+-rw-r--r--   0        0        0    17423 2023-07-26 00:26:06.537155 task3-1.0.5/parse_xsv/cli/cli.py
+-rw-r--r--   0        0        0    12783 2023-07-26 00:26:06.542155 task3-1.0.5/parse_xsv/parse_xsv.py
+-rw-r--r--   0        0        0      113 2023-07-26 00:05:53.472731 task3-1.0.5/parse_xsv/sample_gen/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-26 00:05:53.472731 task3-1.0.5/parse_xsv/sample_gen/__main__.py
+-rw-r--r--   0        0        0     8109 2023-07-26 00:05:53.472731 task3-1.0.5/parse_xsv/sample_gen/sample_gen.py
+-rw-r--r--   0        0        0       97 2023-07-12 14:27:57.666460 task3-1.0.5/parse_xsv/showcase/__init__.py
+-rw-r--r--   0        0        0      138 2023-07-12 14:27:57.687500 task3-1.0.5/parse_xsv/showcase/__main__.py
+-rw-r--r--   0        0        0    25805 2023-07-26 00:05:53.473731 task3-1.0.5/parse_xsv/showcase/corrupted_sample.csv
+-rw-r--r--   0        0        0    29527 2023-07-26 00:05:53.474731 task3-1.0.5/parse_xsv/showcase/sample.csv
+-rw-r--r--   0        0        0    29527 2023-07-26 00:05:53.474731 task3-1.0.5/parse_xsv/showcase/sample.tsv
+-rw-r--r--   0        0        0    22764 2023-07-26 00:05:53.475731 task3-1.0.5/parse_xsv/showcase/showcase.py
+-rw-r--r--   0        0        0      594 2023-07-26 01:12:45.469267 task3-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    26060 2023-07-26 00:55:08.743047 task3-1.0.5/README.md
+-rw-r--r--   0        0        0    26245 1970-01-01 00:00:00.000000 task3-1.0.5/PKG-INFO
```

### Comparing `task3-1.0.4/parse_xsv/cli/cli.py` & `task3-1.0.5/parse_xsv/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,15 @@
                          of tuples with regex expressions: {c_regex}""")
 
         s_regex = RegexPatterns[self.arguments.search_regex].value if self.arguments.search_regex else None
         logger.debug(f"""Convert search_regex argument {self.arguments.search_regex}
                                     to regex expression: {s_regex}""")
 
         output = list(ReaderXSV(self.arguments.file_name,
+                                pure=self.arguments.pure,
                                 no_header=self.arguments.no_header,
                                 search_string=self.arguments.search,
                                 search_regex=s_regex,
                                 column_regex=c_regex,
                                 rows=self.arguments.rows,
                                 columns=self.arguments.columns,
                                 restkey='rest',
@@ -260,14 +261,15 @@
                                 dialect=self.arguments.dialect,
                                 quoting=QuotingTypes[self.arguments.quoting].value,
                                 json=self.arguments.json,
                                 strict=not self.arguments.force))
 
         logger.info(f'Output was generated')
         logger.debug(f"""with the following arguments:
+                                    pure={self.arguments.pure},
                                     no_header={self.arguments.no_header},
                                     search_string={self.arguments.search},
                                     search_regex={s_regex},
                                     column_regex={c_regex},
                                     rows={self.arguments.rows},
                                     columns={self.arguments.columns},
                                     restkey={'rest'},
@@ -309,14 +311,19 @@
              {','.join(csv.list_dialects())}"""),
 
     Argument('-j', '--json',
              dest='json',
              action='store_true',
              help='Show output in JSON format. If filename is passed'),
 
+    Argument('-p', '--pure',
+             dest='pure',
+             action='store_true',
+             help='Using pure Python library parsing without CSV module'),
+
     Argument('-q', '--quoting',
              dest='quoting',
              metavar='',
              choices=[e.name for e in QuotingTypes],
              default='QUOTE_MINIMAL',
              help=f"""How values are quoted in the CSV file (default: QUOTE_MINIMAL).
              Possible values could be:
```

### Comparing `task3-1.0.4/parse_xsv/sample_gen/sample_gen.py` & `task3-1.0.5/parse_xsv/sample_gen/sample_gen.py`

 * *Files identical despite different names*

### Comparing `task3-1.0.4/parse_xsv/showcase/corrupted_sample.csv` & `task3-1.0.5/parse_xsv/showcase/corrupted_sample.csv`

 * *Files identical despite different names*

### Comparing `task3-1.0.4/parse_xsv/showcase/sample.csv` & `task3-1.0.5/parse_xsv/showcase/sample.csv`

 * *Files identical despite different names*

### Comparing `task3-1.0.4/parse_xsv/showcase/sample.tsv` & `task3-1.0.5/parse_xsv/showcase/sample.tsv`

 * *Files identical despite different names*

### Comparing `task3-1.0.4/parse_xsv/showcase/showcase.py` & `task3-1.0.5/parse_xsv/showcase/showcase.py`

 * *Files identical despite different names*

### Comparing `task3-1.0.4/pyproject.toml` & `task3-1.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "task3"
-version = "1.0.4"
+version = "1.0.5"
 description = "xSV file parser CLI and library"
 authors = ["Bill.Avramenko <billavramenko@gmail.com>"]
 readme = "README.md"
 packages = [{include = "parse_xsv"}]
+license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 questionary = "^1.10.0"
 faker = "^19.2.0"
 
 [tool.poetry.scripts]
```

### Comparing `task3-1.0.4/README.md` & `task3-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 </h1>
 
 <p align="center">
   <div align="center">
     <a href="https://pypi.org/project/task3/">
       <img src="https://img.shields.io/pypi/v/task3.svg?style=for-the-badge&label=task 3" alt="TASK 3" />
     </a>&nbsp;
-    <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task3/-/blob/783fe98d0c073fb7de18c872eb6b2d9dfbe81dbc/LICENSE">
-      <img src="https://img.shields.io/pypi/l/task2b.svg?style=for-the-badge" alt="License" />
+    <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task3ab/-/blob/c8b5559d33a26d7bd60aecf68d403fd286c764ed/LICENSE">
+      <img src="https://img.shields.io/pypi/l/task3.svg?style=for-the-badge" alt="License" />
     </a>&nbsp;
     <a href="https://python-poetry.org/">
       <img src="https://img.shields.io/pypi/v/poetry.svg?style=for-the-badge&label=poetry&color=green" alt="POETRY" />
     </a>&nbsp;
     <a href="https://www.python.org/downloads/">
       <img src="https://img.shields.io/pypi/pyversions/task3?style=for-the-badge" alt="PYTHON" />
     </a>&nbsp;
@@ -413,15 +413,15 @@
 
 ### Showcase
 
 To showcase the behavior of the parse_xsv library, an interactive command called "parse_xsv_showcase" has been created.
 This command utilizes both the parse_xsv CLI and the parse_xsv library. It's an interactive command you can invoke via `parse_xsv_showcase` or `python3 -m parse_xsv.showcase`.
 It has an optional flag that allows you to view all use cases at once without any interaction.
 You can use the command `parse_xsv_showcase --all` to activate this feature.
-There are also ready-made xSV files present - `sample.csv`, `sample.tsv' and `corrupted_sample.csv`,
+There are also ready-made xSV files present - `sample.csv`, `sample.tsv` and `corrupted_sample.csv`,
 but you can use the [хsv_sample_gen](#xsv-example-file-generator) command for this purpose.
 
 ![showcase_demo.gif](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/a1a8daf14233ad3f2e7aa73d72abac906ea2867d/m2-python/task-3/images/showcase_demo_task3.gif)
 
 ## General provisions
 
 All materials provided and/or made available contain EPAM’s proprietary and confidential information and must not to be copied,
```

#### html2text {}

```diff
@@ -273,15 +273,15 @@
 operator or pipe |. ``` ### Showcase To showcase the behavior of the parse_xsv
 library, an interactive command called "parse_xsv_showcase" has been created.
 This command utilizes both the parse_xsv CLI and the parse_xsv library. It's an
 interactive command you can invoke via `parse_xsv_showcase` or `python3 -
 m parse_xsv.showcase`. It has an optional flag that allows you to view all use
 cases at once without any interaction. You can use the command
 `parse_xsv_showcase --all` to activate this feature. There are also ready-made
-xSV files present - `sample.csv`, `sample.tsv' and `corrupted_sample.csv`, but
+xSV files present - `sample.csv`, `sample.tsv` and `corrupted_sample.csv`, but
 you can use the [Ñsv_sample_gen](#xsv-example-file-generator) command for this
 purpose. ![showcase_demo.gif](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-
 assets/-/raw/a1a8daf14233ad3f2e7aa73d72abac906ea2867d/m2-python/task-3/images/
 showcase_demo_task3.gif) ## General provisions All materials provided and/or
 made available contain EPAMâs proprietary and confidential information and
 must not to be copied, reproduced or disclosed to any third party or to any
 other person, other than those persons who have a bona fide need to review it
```

### Comparing `task3-1.0.4/PKG-INFO` & `task3-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: task3
-Version: 1.0.4
+Version: 1.0.5
 Summary: xSV file parser CLI and library
+License: MIT
 Author: Bill.Avramenko
 Author-email: billavramenko@gmail.com
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faker (>=19.2.0,<20.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
@@ -26,16 +28,16 @@
 </h1>
 
 <p align="center">
   <div align="center">
     <a href="https://pypi.org/project/task3/">
       <img src="https://img.shields.io/pypi/v/task3.svg?style=for-the-badge&label=task 3" alt="TASK 3" />
     </a>&nbsp;
-    <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task3/-/blob/783fe98d0c073fb7de18c872eb6b2d9dfbe81dbc/LICENSE">
-      <img src="https://img.shields.io/pypi/l/task2b.svg?style=for-the-badge" alt="License" />
+    <a href="https://gitlab.com/Bill-EPAM-DevOpsInt2023/python/task3ab/-/blob/c8b5559d33a26d7bd60aecf68d403fd286c764ed/LICENSE">
+      <img src="https://img.shields.io/pypi/l/task3.svg?style=for-the-badge" alt="License" />
     </a>&nbsp;
     <a href="https://python-poetry.org/">
       <img src="https://img.shields.io/pypi/v/poetry.svg?style=for-the-badge&label=poetry&color=green" alt="POETRY" />
     </a>&nbsp;
     <a href="https://www.python.org/downloads/">
       <img src="https://img.shields.io/pypi/pyversions/task3?style=for-the-badge" alt="PYTHON" />
     </a>&nbsp;
@@ -429,15 +431,15 @@
 
 ### Showcase
 
 To showcase the behavior of the parse_xsv library, an interactive command called "parse_xsv_showcase" has been created.
 This command utilizes both the parse_xsv CLI and the parse_xsv library. It's an interactive command you can invoke via `parse_xsv_showcase` or `python3 -m parse_xsv.showcase`.
 It has an optional flag that allows you to view all use cases at once without any interaction.
 You can use the command `parse_xsv_showcase --all` to activate this feature.
-There are also ready-made xSV files present - `sample.csv`, `sample.tsv' and `corrupted_sample.csv`,
+There are also ready-made xSV files present - `sample.csv`, `sample.tsv` and `corrupted_sample.csv`,
 but you can use the [хsv_sample_gen](#xsv-example-file-generator) command for this purpose.
 
 ![showcase_demo.gif](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-assets/-/raw/a1a8daf14233ad3f2e7aa73d72abac906ea2867d/m2-python/task-3/images/showcase_demo_task3.gif)
 
 ## General provisions
 
 All materials provided and/or made available contain EPAM’s proprietary and confidential information and must not to be copied,
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1 Name: task3 Version: 1.0.4 Summary: xSV file parser CLI
-and library Author: Bill.Avramenko Author-email: billavramenko@gmail.com
-Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
+Metadata-Version: 2.1 Name: task3 Version: 1.0.5 Summary: xSV file parser CLI
+and library License: MIT Author: Bill.Avramenko Author-email:
+billavramenko@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: faker
 (>=19.2.0,<20.0.0) Requires-Dist: questionary (>=1.10.0,<2.0.0) Description-
 Content-Type: text/markdown
                     [EPAM_DevOps-7_Internal_Lab_title_logo]
                        Parsing xSV with Regex in Python.
@@ -281,15 +282,15 @@
 operator or pipe |. ``` ### Showcase To showcase the behavior of the parse_xsv
 library, an interactive command called "parse_xsv_showcase" has been created.
 This command utilizes both the parse_xsv CLI and the parse_xsv library. It's an
 interactive command you can invoke via `parse_xsv_showcase` or `python3 -
 m parse_xsv.showcase`. It has an optional flag that allows you to view all use
 cases at once without any interaction. You can use the command
 `parse_xsv_showcase --all` to activate this feature. There are also ready-made
-xSV files present - `sample.csv`, `sample.tsv' and `corrupted_sample.csv`, but
+xSV files present - `sample.csv`, `sample.tsv` and `corrupted_sample.csv`, but
 you can use the [Ñsv_sample_gen](#xsv-example-file-generator) command for this
 purpose. ![showcase_demo.gif](https://gitlab.com/EPAM-DevOpsInt2023/devops-7-
 assets/-/raw/a1a8daf14233ad3f2e7aa73d72abac906ea2867d/m2-python/task-3/images/
 showcase_demo_task3.gif) ## General provisions All materials provided and/or
 made available contain EPAMâs proprietary and confidential information and
 must not to be copied, reproduced or disclosed to any third party or to any
 other person, other than those persons who have a bona fide need to review it
```

