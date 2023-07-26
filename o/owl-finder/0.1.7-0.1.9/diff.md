# Comparing `tmp/owl-finder-0.1.7.tar.gz` & `tmp/owl-finder-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owl-finder-0.1.7.tar", max compression
+gzip compressed data, was "owl-finder-0.1.9.tar", max compression
```

## Comparing `owl-finder-0.1.7.tar` & `owl-finder-0.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      170 2022-11-25 23:03:41.093632 owl-finder-0.1.7/owl_finder/__init__.py
--rw-r--r--   0        0        0        0 2022-09-14 02:31:05.588766 owl-finder-0.1.7/owl_finder/multiquery/__init__.py
--rw-r--r--   0        0        0       50 2022-09-14 02:31:05.589266 owl-finder-0.1.7/owl_finder/multiquery/bp/__init__.py
--rw-r--r--   0        0        0    28139 2022-11-29 02:41:23.310897 owl-finder-0.1.7/owl_finder/multiquery/bp/find_ontology_data.py
--rw-r--r--   0        0        0      394 2022-10-26 21:57:26.307587 owl-finder-0.1.7/owl_finder/multiquery/dmo/__init__.py
--rw-r--r--   0        0        0     2250 2022-11-01 18:28:21.903529 owl-finder-0.1.7/owl_finder/multiquery/dmo/external_synonym_loader.py
--rw-r--r--   0        0        0     2231 2022-11-24 20:18:09.768356 owl-finder-0.1.7/owl_finder/multiquery/dmo/model_result_merge.py
--rw-r--r--   0        0        0     2854 2022-11-01 18:28:21.901028 owl-finder-0.1.7/owl_finder/multiquery/dmo/ner_pallete_lookup.py
--rw-r--r--   0        0        0       94 2022-09-14 02:31:05.592766 owl-finder-0.1.7/owl_finder/multiquery/dmo/span/__init__.py
--rw-r--r--   0        0        0     4223 2022-10-26 22:03:19.443027 owl-finder-0.1.7/owl_finder/multiquery/dmo/span/owl_span_augment.py
--rw-r--r--   0        0        0     2252 2022-10-26 21:57:26.365088 owl-finder-0.1.7/owl_finder/multiquery/dmo/span/owl_span_generate.py
--rw-r--r--   0        0        0     1712 2022-11-24 01:21:10.775234 owl-finder-0.1.7/owl_finder/multiquery/dmo/view_generator_lookup.py
--rw-r--r--   0        0        0     1936 2022-09-14 02:31:05.594766 owl-finder-0.1.7/owl_finder/multiquery/dmo/view_generator_nerdepth.py
--rw-r--r--   0        0        0     1442 2022-09-14 02:31:05.595267 owl-finder-0.1.7/owl_finder/multiquery/dmo/view_generator_nerlabel.py
--rw-r--r--   0        0        0     1227 2022-09-14 02:31:05.595765 owl-finder-0.1.7/owl_finder/multiquery/dmo/view_generator_nertaxo.py
--rw-r--r--   0        0        0      278 2022-10-26 21:57:26.191587 owl-finder-0.1.7/owl_finder/multiquery/svc/__init__.py
--rw-r--r--   0        0        0     4361 2022-11-01 18:28:21.898529 owl-finder-0.1.7/owl_finder/multiquery/svc/find_ner.py
--rw-r--r--   0        0        0     7057 2022-11-01 18:28:21.908028 owl-finder-0.1.7/owl_finder/multiquery/svc/find_synonyms.py
--rw-r--r--   0        0        0     7888 2022-10-26 21:57:24.001088 owl-finder-0.1.7/owl_finder/multiquery/svc/find_types.py
--rw-r--r--   0        0        0     4150 2022-11-24 20:14:24.900911 owl-finder-0.1.7/owl_finder/multiquery/svc/load_synonyms.py
--rw-r--r--   0        0        0     2561 2022-11-24 01:21:10.775234 owl-finder-0.1.7/owl_finder/multiquery/svc/query_ner_depth.py
--rw-r--r--   0        0        0     2815 2022-11-24 01:21:10.775234 owl-finder-0.1.7/owl_finder/multiquery/svc/query_ner_label.py
--rw-r--r--   0        0        0     2114 2022-11-24 01:21:10.775234 owl-finder-0.1.7/owl_finder/multiquery/svc/query_ner_taxo.py
--rw-r--r--   0        0        0       79 2022-10-26 21:57:26.234087 owl-finder-0.1.7/owl_finder/singlequery/__init__.py
--rw-r--r--   0        0        0       36 2022-09-14 02:31:05.604267 owl-finder-0.1.7/owl_finder/singlequery/bp/__init__.py
--rw-r--r--   0        0        0    13879 2022-11-29 00:27:20.289314 owl-finder-0.1.7/owl_finder/singlequery/bp/ask_owl_api.py
--rw-r--r--   0        0        0      152 2022-09-14 02:31:05.605765 owl-finder-0.1.7/owl_finder/singlequery/dmo/__init__.py
--rw-r--r--   0        0        0     3664 2022-11-29 03:07:01.900350 owl-finder-0.1.7/owl_finder/singlequery/dmo/owl_graph_connector.py
--rw-r--r--   0        0        0     5294 2022-11-24 01:21:10.774732 owl-finder-0.1.7/owl_finder/singlequery/dmo/owl_query_extract.py
--rw-r--r--   0        0        0     1636 2022-10-26 21:57:26.375587 owl-finder-0.1.7/owl_finder/singlequery/dmo/owl_query_normalize.py
--rw-r--r--   0        0        0       48 2022-09-14 02:31:05.607766 owl-finder-0.1.7/owl_finder/singlequery/dto/__init__.py
--rw-r--r--   0        0        0      243 2022-09-14 02:31:05.608270 owl-finder-0.1.7/owl_finder/singlequery/dto/query_result_type.py
--rw-r--r--   0        0        0      318 2022-11-26 03:52:02.516079 owl-finder-0.1.7/owl_finder/singlequery/svc/__init__.py
--rw-r--r--   0        0        0     2279 2022-11-29 02:26:40.660911 owl-finder-0.1.7/owl_finder/singlequery/svc/generate_plus_spans.py
--rw-r--r--   0        0        0     6398 2022-11-29 02:25:59.539852 owl-finder-0.1.7/owl_finder/singlequery/svc/generate_view_spans.py
--rw-r--r--   0        0        0     2948 2022-11-26 04:11:11.752667 owl-finder-0.1.7/owl_finder/singlequery/svc/generate_view_synonyms.py
--rw-r--r--   0        0        0     1887 2022-09-14 02:31:05.610268 owl-finder-0.1.7/owl_finder/singlequery/svc/generate_view_trie.py
--rw-r--r--   0        0        0     2900 2022-11-24 01:21:10.774732 owl-finder-0.1.7/owl_finder/singlequery/svc/load_ontology_model.py
--rw-r--r--   0        0        0     3378 2022-11-24 01:21:10.774732 owl-finder-0.1.7/owl_finder/singlequery/svc/query_ontology_model.py
--rw-r--r--   0        0        0     1426 2022-11-29 02:42:20.653667 owl-finder-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       77 2022-11-23 22:29:31.314598 owl-finder-0.1.7/README.md
--rw-r--r--   0        0        0     1086 2022-11-29 03:09:23.033522 owl-finder-0.1.7/setup.py
--rw-r--r--   0        0        0     1000 2022-11-29 03:09:23.033522 owl-finder-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      170 2022-11-25 23:03:41.093632 owl-finder-0.1.9/owl_finder/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-14 02:31:05.588766 owl-finder-0.1.9/owl_finder/multiquery/__init__.py
+-rw-r--r--   0        0        0       50 2022-09-14 02:31:05.589266 owl-finder-0.1.9/owl_finder/multiquery/bp/__init__.py
+-rw-r--r--   0        0        0    28355 2022-11-29 03:43:23.094294 owl-finder-0.1.9/owl_finder/multiquery/bp/find_ontology_data.py
+-rw-r--r--   0        0        0      394 2022-10-26 21:57:26.307587 owl-finder-0.1.9/owl_finder/multiquery/dmo/__init__.py
+-rw-r--r--   0        0        0     2250 2022-11-01 18:28:21.903529 owl-finder-0.1.9/owl_finder/multiquery/dmo/external_synonym_loader.py
+-rw-r--r--   0        0        0     2231 2022-11-24 20:18:09.768356 owl-finder-0.1.9/owl_finder/multiquery/dmo/model_result_merge.py
+-rw-r--r--   0        0        0     2854 2022-11-01 18:28:21.901028 owl-finder-0.1.9/owl_finder/multiquery/dmo/ner_pallete_lookup.py
+-rw-r--r--   0        0        0       94 2022-09-14 02:31:05.592766 owl-finder-0.1.9/owl_finder/multiquery/dmo/span/__init__.py
+-rw-r--r--   0        0        0     4223 2022-10-26 22:03:19.443027 owl-finder-0.1.9/owl_finder/multiquery/dmo/span/owl_span_augment.py
+-rw-r--r--   0        0        0     2252 2022-10-26 21:57:26.365088 owl-finder-0.1.9/owl_finder/multiquery/dmo/span/owl_span_generate.py
+-rw-r--r--   0        0        0     1712 2022-11-24 01:21:10.775234 owl-finder-0.1.9/owl_finder/multiquery/dmo/view_generator_lookup.py
+-rw-r--r--   0        0        0     1936 2022-09-14 02:31:05.594766 owl-finder-0.1.9/owl_finder/multiquery/dmo/view_generator_nerdepth.py
+-rw-r--r--   0        0        0     1442 2022-09-14 02:31:05.595267 owl-finder-0.1.9/owl_finder/multiquery/dmo/view_generator_nerlabel.py
+-rw-r--r--   0        0        0     1227 2022-09-14 02:31:05.595765 owl-finder-0.1.9/owl_finder/multiquery/dmo/view_generator_nertaxo.py
+-rw-r--r--   0        0        0      278 2022-10-26 21:57:26.191587 owl-finder-0.1.9/owl_finder/multiquery/svc/__init__.py
+-rw-r--r--   0        0        0     4361 2022-11-01 18:28:21.898529 owl-finder-0.1.9/owl_finder/multiquery/svc/find_ner.py
+-rw-r--r--   0        0        0     7057 2022-11-01 18:28:21.908028 owl-finder-0.1.9/owl_finder/multiquery/svc/find_synonyms.py
+-rw-r--r--   0        0        0     7888 2022-10-26 21:57:24.001088 owl-finder-0.1.9/owl_finder/multiquery/svc/find_types.py
+-rw-r--r--   0        0        0     4150 2022-11-24 20:14:24.900911 owl-finder-0.1.9/owl_finder/multiquery/svc/load_synonyms.py
+-rw-r--r--   0        0        0     2561 2022-11-24 01:21:10.775234 owl-finder-0.1.9/owl_finder/multiquery/svc/query_ner_depth.py
+-rw-r--r--   0        0        0     2815 2022-11-24 01:21:10.775234 owl-finder-0.1.9/owl_finder/multiquery/svc/query_ner_label.py
+-rw-r--r--   0        0        0     2114 2022-11-24 01:21:10.775234 owl-finder-0.1.9/owl_finder/multiquery/svc/query_ner_taxo.py
+-rw-r--r--   0        0        0       79 2022-10-26 21:57:26.234087 owl-finder-0.1.9/owl_finder/singlequery/__init__.py
+-rw-r--r--   0        0        0       36 2022-09-14 02:31:05.604267 owl-finder-0.1.9/owl_finder/singlequery/bp/__init__.py
+-rw-r--r--   0        0        0    13879 2022-11-29 00:27:20.289314 owl-finder-0.1.9/owl_finder/singlequery/bp/ask_owl_api.py
+-rw-r--r--   0        0        0      152 2022-09-14 02:31:05.605765 owl-finder-0.1.9/owl_finder/singlequery/dmo/__init__.py
+-rw-r--r--   0        0        0     3664 2022-11-29 03:07:01.900350 owl-finder-0.1.9/owl_finder/singlequery/dmo/owl_graph_connector.py
+-rw-r--r--   0        0        0     5294 2022-11-24 01:21:10.774732 owl-finder-0.1.9/owl_finder/singlequery/dmo/owl_query_extract.py
+-rw-r--r--   0        0        0     1636 2022-10-26 21:57:26.375587 owl-finder-0.1.9/owl_finder/singlequery/dmo/owl_query_normalize.py
+-rw-r--r--   0        0        0       48 2022-09-14 02:31:05.607766 owl-finder-0.1.9/owl_finder/singlequery/dto/__init__.py
+-rw-r--r--   0        0        0      243 2022-09-14 02:31:05.608270 owl-finder-0.1.9/owl_finder/singlequery/dto/query_result_type.py
+-rw-r--r--   0        0        0      318 2022-11-26 03:52:02.516079 owl-finder-0.1.9/owl_finder/singlequery/svc/__init__.py
+-rw-r--r--   0        0        0     2279 2022-11-29 02:26:40.660911 owl-finder-0.1.9/owl_finder/singlequery/svc/generate_plus_spans.py
+-rw-r--r--   0        0        0     6398 2022-11-29 02:25:59.539852 owl-finder-0.1.9/owl_finder/singlequery/svc/generate_view_spans.py
+-rw-r--r--   0        0        0     2948 2022-11-26 04:11:11.752667 owl-finder-0.1.9/owl_finder/singlequery/svc/generate_view_synonyms.py
+-rw-r--r--   0        0        0     1887 2022-09-14 02:31:05.610268 owl-finder-0.1.9/owl_finder/singlequery/svc/generate_view_trie.py
+-rw-r--r--   0        0        0     2900 2022-11-24 01:21:10.774732 owl-finder-0.1.9/owl_finder/singlequery/svc/load_ontology_model.py
+-rw-r--r--   0        0        0     3378 2022-11-24 01:21:10.774732 owl-finder-0.1.9/owl_finder/singlequery/svc/query_ontology_model.py
+-rw-r--r--   0        0        0     1426 2022-11-29 03:42:07.765249 owl-finder-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       77 2022-11-23 22:29:31.314598 owl-finder-0.1.9/README.md
+-rw-r--r--   0        0        0     1086 2022-11-29 03:43:51.442333 owl-finder-0.1.9/setup.py
+-rw-r--r--   0        0        0     1000 2022-11-29 03:43:51.442333 owl-finder-0.1.9/PKG-INFO
```

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/bp/find_ontology_data.py` & `owl-finder-0.1.9/owl_finder/multiquery/bp/find_ontology_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -913,7 +913,15 @@
         """
         d_synonyms_fwd = self.synonyms()
 
         if not d_synonyms_fwd or not len(d_synonyms_fwd):
             return None
 
         return ViewGeneratorLookup().process(d_synonyms_fwd)
+
+    def has_data(self) -> bool:
+        """ Check if the underlying Ontologies have data
+
+        Returns:
+            bool: _description_
+        """
+        return self.synonyms() and len(self.synonyms())
```

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/dmo/external_synonym_loader.py` & `owl-finder-0.1.9/owl_finder/multiquery/dmo/external_synonym_loader.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/dmo/model_result_merge.py` & `owl-finder-0.1.9/owl_finder/multiquery/dmo/model_result_merge.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/dmo/ner_pallete_lookup.py` & `owl-finder-0.1.9/owl_finder/multiquery/dmo/ner_pallete_lookup.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/dmo/span/owl_span_augment.py` & `owl-finder-0.1.9/owl_finder/multiquery/dmo/span/owl_span_augment.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/dmo/span/owl_span_generate.py` & `owl-finder-0.1.9/owl_finder/multiquery/dmo/span/owl_span_generate.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/dmo/view_generator_lookup.py` & `owl-finder-0.1.9/owl_finder/multiquery/dmo/view_generator_lookup.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/dmo/view_generator_nerdepth.py` & `owl-finder-0.1.9/owl_finder/multiquery/dmo/view_generator_nerdepth.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/dmo/view_generator_nerlabel.py` & `owl-finder-0.1.9/owl_finder/multiquery/dmo/view_generator_nerlabel.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/dmo/view_generator_nertaxo.py` & `owl-finder-0.1.9/owl_finder/multiquery/dmo/view_generator_nertaxo.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/svc/find_ner.py` & `owl-finder-0.1.9/owl_finder/multiquery/svc/find_ner.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/svc/find_synonyms.py` & `owl-finder-0.1.9/owl_finder/multiquery/svc/find_synonyms.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/svc/find_types.py` & `owl-finder-0.1.9/owl_finder/multiquery/svc/find_types.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/svc/load_synonyms.py` & `owl-finder-0.1.9/owl_finder/multiquery/svc/load_synonyms.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/svc/query_ner_depth.py` & `owl-finder-0.1.9/owl_finder/multiquery/svc/query_ner_depth.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/svc/query_ner_label.py` & `owl-finder-0.1.9/owl_finder/multiquery/svc/query_ner_label.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/multiquery/svc/query_ner_taxo.py` & `owl-finder-0.1.9/owl_finder/multiquery/svc/query_ner_taxo.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/singlequery/bp/ask_owl_api.py` & `owl-finder-0.1.9/owl_finder/singlequery/bp/ask_owl_api.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/singlequery/dmo/owl_graph_connector.py` & `owl-finder-0.1.9/owl_finder/singlequery/dmo/owl_graph_connector.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/singlequery/dmo/owl_query_extract.py` & `owl-finder-0.1.9/owl_finder/singlequery/dmo/owl_query_extract.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/singlequery/dmo/owl_query_normalize.py` & `owl-finder-0.1.9/owl_finder/singlequery/dmo/owl_query_normalize.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/singlequery/svc/generate_plus_spans.py` & `owl-finder-0.1.9/owl_finder/singlequery/svc/generate_plus_spans.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/singlequery/svc/generate_view_spans.py` & `owl-finder-0.1.9/owl_finder/singlequery/svc/generate_view_spans.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/singlequery/svc/generate_view_synonyms.py` & `owl-finder-0.1.9/owl_finder/singlequery/svc/generate_view_synonyms.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/singlequery/svc/generate_view_trie.py` & `owl-finder-0.1.9/owl_finder/singlequery/svc/generate_view_trie.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/singlequery/svc/load_ontology_model.py` & `owl-finder-0.1.9/owl_finder/singlequery/svc/load_ontology_model.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/owl_finder/singlequery/svc/query_ontology_model.py` & `owl-finder-0.1.9/owl_finder/singlequery/svc/query_ontology_model.py`

 * *Files identical despite different names*

### Comparing `owl-finder-0.1.7/pyproject.toml` & `owl-finder-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Craig Trim <craigtrim@gmail.com>",
 ]
 
 description = "Perform Ontology Queries with a Finder Facade"
 license = "None"
 name = "owl-finder"
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.9"
 
 keywords = ["nlp", "nlu", "text", "classify", "classification"]
 repository = "https://github.com/craigtrim/owl-finder"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `owl-finder-0.1.7/setup.py` & `owl-finder-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 {'': ['*']}
 
 install_requires = \
 ['baseblock', 'rdflib>=6.2.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'owl-finder',
-    'version': '0.1.7',
+    'version': '0.1.9',
     'description': 'Perform Ontology Queries with a Finder Facade',
     'long_description': '# Ontology Finder (owl-finder)\nA Finder Facade for Querying Ontology Files\n',
     'author': 'Craig Trim',
     'author_email': 'craigtrim@gmail.com',
     'maintainer': 'Craig Trim',
     'maintainer_email': 'craigtrim@gmail.com',
     'url': 'https://github.com/craigtrim/owl-finder',
```

### Comparing `owl-finder-0.1.7/PKG-INFO` & `owl-finder-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owl-finder
-Version: 0.1.7
+Version: 0.1.9
 Summary: Perform Ontology Queries with a Finder Facade
 Home-page: https://github.com/craigtrim/owl-finder
 License: None
 Keywords: nlp,nlu,text,classify,classification
 Author: Craig Trim
 Author-email: craigtrim@gmail.com
 Maintainer: Craig Trim
```

