# Comparing `tmp/owl-results-0.1.3.tar.gz` & `tmp/owl_results-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owl-results-0.1.3.tar", max compression
+gzip compressed data, was "owl_results-0.1.4.tar", max compression
```

## Comparing `owl-results-0.1.3.tar` & `owl_results-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      126 2022-11-30 00:50:33.146950 owl-results-0.1.3/owl_results/__init__.py
--rw-r--r--   0        0        0       44 2022-11-30 00:50:24.620358 owl-results-0.1.3/owl_results/bp/__init__.py
--rw-r--r--   0        0        0     2109 2022-11-30 01:11:43.436408 owl-results-0.1.3/owl_results/bp/owl_results_api.py
--rw-r--r--   0        0        0       91 2022-11-30 00:41:25.696075 owl-results-0.1.3/owl_results/dmo/__init__.py
--rw-r--r--   0        0        0     1046 2022-11-30 00:41:31.892463 owl-results-0.1.3/owl_results/dmo/edge_dedupe.py
--rw-r--r--   0        0        0     1078 2022-11-30 00:40:29.740991 owl-results-0.1.3/owl_results/dmo/ontology_node_dedupe.py
--rw-r--r--   0        0        0      156 2022-11-30 00:16:19.940182 owl-results-0.1.3/owl_results/dto/__init__.py
--rw-r--r--   0        0        0      675 2022-09-21 16:56:56.000000 owl-results-0.1.3/owl_results/dto/typedefs.py
--rw-r--r--   0        0        0      174 2022-11-30 01:10:40.221105 owl-results-0.1.3/owl_results/svc/__init__.py
--rw-r--r--   0        0        0     5555 2022-11-30 00:56:54.277664 owl-results-0.1.3/owl_results/svc/create_graph_structure.py
--rw-r--r--   0        0        0     1444 2022-11-30 01:46:15.871242 owl-results-0.1.3/owl_results/svc/create_normalized_text.py
--rw-r--r--   0        0        0     1223 2022-11-30 01:01:55.732968 owl-results-0.1.3/owl_results/svc/post_process_structure.py
--rw-r--r--   0        0        0     1429 2022-11-30 01:45:50.030415 owl-results-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-30 00:00:14.733906 owl-results-0.1.3/README.md
--rw-r--r--   0        0        0      782 2022-11-30 01:46:56.994384 owl-results-0.1.3/setup.py
--rw-r--r--   0        0        0      917 2022-11-30 01:46:56.994384 owl-results-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      126 2022-11-30 00:50:33.000000 owl_results-0.1.4/owl_results/__init__.py
+-rw-r--r--   0        0        0       44 2022-11-30 00:50:24.000000 owl_results-0.1.4/owl_results/bp/__init__.py
+-rw-r--r--   0        0        0     2109 2022-11-30 01:11:43.000000 owl_results-0.1.4/owl_results/bp/owl_results_api.py
+-rw-r--r--   0        0        0       91 2022-11-30 00:41:25.000000 owl_results-0.1.4/owl_results/dmo/__init__.py
+-rw-r--r--   0        0        0     1046 2022-11-30 00:41:31.000000 owl_results-0.1.4/owl_results/dmo/edge_dedupe.py
+-rw-r--r--   0        0        0     1078 2022-11-30 00:40:29.000000 owl_results-0.1.4/owl_results/dmo/ontology_node_dedupe.py
+-rw-r--r--   0        0        0      156 2022-11-30 00:16:19.000000 owl_results-0.1.4/owl_results/dto/__init__.py
+-rw-r--r--   0        0        0      675 2022-09-21 16:56:56.000000 owl_results-0.1.4/owl_results/dto/typedefs.py
+-rw-r--r--   0        0        0      174 2022-11-30 01:10:40.000000 owl_results-0.1.4/owl_results/svc/__init__.py
+-rw-r--r--   0        0        0     5555 2022-11-30 00:56:54.000000 owl_results-0.1.4/owl_results/svc/create_graph_structure.py
+-rw-r--r--   0        0        0     1444 2022-11-30 01:46:15.000000 owl_results-0.1.4/owl_results/svc/create_normalized_text.py
+-rw-r--r--   0        0        0     1223 2022-11-30 01:01:55.000000 owl_results-0.1.4/owl_results/svc/post_process_structure.py
+-rw-r--r--   0        0        0     1429 2023-07-26 18:13:33.833439 owl_results-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-30 00:00:14.000000 owl_results-0.1.4/README.md
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 owl_results-0.1.4/setup.py
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 owl_results-0.1.4/PKG-INFO
```

### Comparing `owl-results-0.1.3/owl_results/bp/owl_results_api.py` & `owl_results-0.1.4/owl_results/bp/owl_results_api.py`

 * *Files identical despite different names*

### Comparing `owl-results-0.1.3/owl_results/dmo/edge_dedupe.py` & `owl_results-0.1.4/owl_results/dmo/edge_dedupe.py`

 * *Files identical despite different names*

### Comparing `owl-results-0.1.3/owl_results/dmo/ontology_node_dedupe.py` & `owl_results-0.1.4/owl_results/dmo/ontology_node_dedupe.py`

 * *Files identical despite different names*

### Comparing `owl-results-0.1.3/owl_results/dto/typedefs.py` & `owl_results-0.1.4/owl_results/dto/typedefs.py`

 * *Files identical despite different names*

### Comparing `owl-results-0.1.3/owl_results/svc/create_graph_structure.py` & `owl_results-0.1.4/owl_results/svc/create_graph_structure.py`

 * *Files identical despite different names*

### Comparing `owl-results-0.1.3/owl_results/svc/create_normalized_text.py` & `owl_results-0.1.4/owl_results/svc/create_normalized_text.py`

 * *Files identical despite different names*

### Comparing `owl-results-0.1.3/owl_results/svc/post_process_structure.py` & `owl_results-0.1.4/owl_results/svc/post_process_structure.py`

 * *Files identical despite different names*

### Comparing `owl-results-0.1.3/pyproject.toml` & `owl_results-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Craig Trim <craigtrim@gmail.com>",
 ]
 
 description = "Manipulate Complex OWL Parse Results"
 license = "None"
 name = "owl-results"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 keywords = ["nlp", "nlu", "text", "classify", "classification"]
 repository = "https://github.com/craigtrim/owl-results"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Software Development :: Libraries :: Python Modules",
@@ -27,15 +27,15 @@
 [tool.poetry.dependencies]
 baseblock = "*"
 python = "^3.8.5"
 regression-framework = "*"
 
 [tool.poetry.dev-dependencies]
 autopep8 = "*"
-en-core-web-sm = {path = "resources/lib/en_core_web_sm-3.3.0.tar.gz"}
+en-core-web-sm = {path = "resources/lib/en_core_web_sm-3.5.0.tar.gz"}
 flakeheaven = "*"
 plac = "*"
 pre-commit = "^2.20.0"
 pytest = "*"
 
 [tool.poetry.build]
 generate-setup-file = true
```

### Comparing `owl-results-0.1.3/setup.py` & `owl_results-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock', 'regression-framework']
 
 setup_kwargs = {
     'name': 'owl-results',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Manipulate Complex OWL Parse Results',
     'long_description': '',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/owl-results',
```

### Comparing `owl-results-0.1.3/PKG-INFO` & `owl_results-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: owl-results
-Version: 0.1.3
+Version: 0.1.4
 Summary: Manipulate Complex OWL Parse Results
 Home-page: https://github.com/craigtrim/owl-results
 License: None
 Keywords: nlp,nlu,text,classify,classification
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
 Maintainer-email: craigtrim@gmail.com
 Requires-Python: >=3.8.5,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: baseblock
 Requires-Dist: regression-framework
 Project-URL: Bug Tracker, https://github.com/craigtrim/owl-results/issues
 Project-URL: Repository, https://github.com/craigtrim/owl-results
 Description-Content-Type: text/markdown
```

