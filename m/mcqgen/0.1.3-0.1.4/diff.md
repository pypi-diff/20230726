# Comparing `tmp/mcqgen-0.1.3.tar.gz` & `tmp/mcqgen-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcqgen-0.1.3.tar", last modified: Wed Jul 26 00:11:05 2023, max compression
+gzip compressed data, was "mcqgen-0.1.4.tar", last modified: Wed Jul 26 00:13:44 2023, max compression
```

## Comparing `mcqgen-0.1.3.tar` & `mcqgen-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:11:05.071851 mcqgen-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 00:11:01.000000 mcqgen-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-26 00:11:05.071851 mcqgen-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-26 00:11:01.000000 mcqgen-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:11:05.071851 mcqgen-0.1.3/mcqgen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:11:01.000000 mcqgen-0.1.3/mcqgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-26 00:11:01.000000 mcqgen-0.1.3/mcqgen/mcqgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:11:05.071851 mcqgen-0.1.3/mcqgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-26 00:11:05.000000 mcqgen-0.1.3/mcqgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-26 00:11:05.000000 mcqgen-0.1.3/mcqgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:11:05.000000 mcqgen-0.1.3/mcqgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:11:05.000000 mcqgen-0.1.3/mcqgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:11:05.000000 mcqgen-0.1.3/mcqgen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 00:11:05.071851 mcqgen-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-26 00:11:01.000000 mcqgen-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:13:44.112968 mcqgen-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-26 00:13:41.000000 mcqgen-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-26 00:13:44.112968 mcqgen-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-26 00:13:41.000000 mcqgen-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:13:44.112968 mcqgen-0.1.4/mcqgen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 00:13:41.000000 mcqgen-0.1.4/mcqgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-26 00:13:41.000000 mcqgen-0.1.4/mcqgen/mcqgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 00:13:44.112968 mcqgen-0.1.4/mcqgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-26 00:13:44.000000 mcqgen-0.1.4/mcqgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-26 00:13:44.000000 mcqgen-0.1.4/mcqgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 00:13:44.000000 mcqgen-0.1.4/mcqgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:13:44.000000 mcqgen-0.1.4/mcqgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 00:13:44.000000 mcqgen-0.1.4/mcqgen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 00:13:44.112968 mcqgen-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-26 00:13:41.000000 mcqgen-0.1.4/setup.py
```

### Comparing `mcqgen-0.1.3/LICENSE` & `mcqgen-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mcqgen-0.1.3/PKG-INFO` & `mcqgen-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,13 @@
-Metadata-Version: 2.1
-Name: mcqgen
-Version: 0.1.3
-Summary: Generate Multiple Choice Questions, Choices and Correct Answer in JSON Format
-Author: Abhilash Mhaisne
-License: MIT License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # mcqgen
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Python Version](https://img.shields.io/badge/Python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org/downloads/)
 
-Generate MCQs with options and correct answers in JSON Format. Uses GPT
+Generate MCQs with options and correct answers in JSON Format. Uses GPT.
 
 ## Installation
 
 You can install the package using pip:
 
 ```bash
 pip install mcqgen
@@ -35,8 +26,8 @@
 data = gen.generate_mcqs('Cricket', model="gpt-3.5-turbo", no=3)
 print(data)
 ```
 ```
 {'questions': [{'question': 'Who holds the record for the highest individual score in Test cricket?', 'options': ['a) Sachin Tendulkar', 'b) Brian Lara', 'c) Don Bradman', 'd) Ricky Ponting'], 'answer': 'b) Brian Lara'}, {'question': 'Which cricketer has scored the most centuries in One Day Internationals (ODIs)?', 'options': ['a) Sachin Tendulkar', 'b) Ricky 
 Ponting', 'c) Virat Kohli', 'd) Kumar Sangakkara'], 'answer': 'a) Sachin Tendulkar'}, {'question': 'Who has the best bowling figures in a Test innings?', 'options': ['a) Jim Laker', 'b) Anil Kumble', 'c) Muttiah Muralitharan', 'd) Shaun Pollock'], 'answer': 'a) Jim Laker'}]}
 
-```
+```
```

### Comparing `mcqgen-0.1.3/README.md` & `mcqgen-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,22 @@
+Metadata-Version: 2.1
+Name: mcqgen
+Version: 0.1.4
+Summary: Generate Multiple Choice Questions, Choices and Correct Answer in JSON Format
+Author: Abhilash Mhaisne
+License: MIT License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # mcqgen
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Python Version](https://img.shields.io/badge/Python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org/downloads/)
 
-Generate MCQs with options and correct answers in JSON Format. Uses GPT
+Generate MCQs with options and correct answers in JSON Format. Uses GPT.
 
 ## Installation
 
 You can install the package using pip:
 
 ```bash
 pip install mcqgen
@@ -26,8 +35,8 @@
 data = gen.generate_mcqs('Cricket', model="gpt-3.5-turbo", no=3)
 print(data)
 ```
 ```
 {'questions': [{'question': 'Who holds the record for the highest individual score in Test cricket?', 'options': ['a) Sachin Tendulkar', 'b) Brian Lara', 'c) Don Bradman', 'd) Ricky Ponting'], 'answer': 'b) Brian Lara'}, {'question': 'Which cricketer has scored the most centuries in One Day Internationals (ODIs)?', 'options': ['a) Sachin Tendulkar', 'b) Ricky 
 Ponting', 'c) Virat Kohli', 'd) Kumar Sangakkara'], 'answer': 'a) Sachin Tendulkar'}, {'question': 'Who has the best bowling figures in a Test innings?', 'options': ['a) Jim Laker', 'b) Anil Kumble', 'c) Muttiah Muralitharan', 'd) Shaun Pollock'], 'answer': 'a) Jim Laker'}]}
 
-```
+```
```

### Comparing `mcqgen-0.1.3/mcqgen/mcqgen.py` & `mcqgen-0.1.4/mcqgen/mcqgen.py`

 * *Files identical despite different names*

### Comparing `mcqgen-0.1.3/mcqgen.egg-info/PKG-INFO` & `mcqgen-0.1.4/mcqgen.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mcqgen
-Version: 0.1.3
+Version: 0.1.4
 Summary: Generate Multiple Choice Questions, Choices and Correct Answer in JSON Format
 Author: Abhilash Mhaisne
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mcqgen
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Python Version](https://img.shields.io/badge/Python-3.6%20%7C%203.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org/downloads/)
 
-Generate MCQs with options and correct answers in JSON Format. Uses GPT
+Generate MCQs with options and correct answers in JSON Format. Uses GPT.
 
 ## Installation
 
 You can install the package using pip:
 
 ```bash
 pip install mcqgen
```

