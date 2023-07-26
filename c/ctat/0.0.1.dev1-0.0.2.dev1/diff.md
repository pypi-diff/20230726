# Comparing `tmp/ctat-0.0.1.dev1.tar.gz` & `tmp/ctat-0.0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctat-0.0.1.dev1.tar", last modified: Fri Jul 14 10:48:21 2023, max compression
+gzip compressed data, was "ctat-0.0.2.dev1.tar", last modified: Wed Jul 26 11:26:13 2023, max compression
```

## Comparing `ctat-0.0.1.dev1.tar` & `ctat-0.0.2.dev1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:48:21.894914 ctat-0.0.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 10:48:06.000000 ctat-0.0.1.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 10:48:06.000000 ctat-0.0.1.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-14 10:48:21.894914 ctat-0.0.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-14 10:48:06.000000 ctat-0.0.1.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 10:48:21.894914 ctat-0.0.1.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-14 10:48:06.000000 ctat-0.0.1.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:48:21.890914 ctat-0.0.1.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:48:21.894914 ctat-0.0.1.dev1/src/ctat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 10:48:06.000000 ctat-0.0.1.dev1/src/ctat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-14 10:48:06.000000 ctat-0.0.1.dev1/src/ctat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-14 10:48:06.000000 ctat-0.0.1.dev1/src/ctat/cell_type_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-14 10:48:06.000000 ctat-0.0.1.dev1/src/ctat/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-14 10:48:06.000000 ctat-0.0.1.dev1/src/ctat/schema_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:48:21.894914 ctat-0.0.1.dev1/src/ctat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-14 10:48:21.000000 ctat-0.0.1.dev1/src/ctat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-14 10:48:21.000000 ctat-0.0.1.dev1/src/ctat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 10:48:21.000000 ctat-0.0.1.dev1/src/ctat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 10:48:21.000000 ctat-0.0.1.dev1/src/ctat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-14 10:48:21.000000 ctat-0.0.1.dev1/src/ctat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 10:48:21.000000 ctat-0.0.1.dev1/src/ctat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 10:48:21.894914 ctat-0.0.1.dev1/src/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-14 10:48:06.000000 ctat-0.0.1.dev1/src/schema/ctat_schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:26:13.008688 ctat-0.0.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 11:25:54.000000 ctat-0.0.2.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-26 11:25:54.000000 ctat-0.0.2.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-26 11:26:13.008688 ctat-0.0.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-26 11:25:54.000000 ctat-0.0.2.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 11:26:13.008688 ctat-0.0.2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-26 11:25:54.000000 ctat-0.0.2.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:26:13.004687 ctat-0.0.2.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:26:13.008688 ctat-0.0.2.dev1/src/ctat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 11:25:54.000000 ctat-0.0.2.dev1/src/ctat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-26 11:25:54.000000 ctat-0.0.2.dev1/src/ctat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-26 11:25:54.000000 ctat-0.0.2.dev1/src/ctat/cell_type_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-07-26 11:25:54.000000 ctat-0.0.2.dev1/src/ctat/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-26 11:25:54.000000 ctat-0.0.2.dev1/src/ctat/schema_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:26:13.008688 ctat-0.0.2.dev1/src/ctat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-26 11:26:12.000000 ctat-0.0.2.dev1/src/ctat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-26 11:26:12.000000 ctat-0.0.2.dev1/src/ctat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 11:26:12.000000 ctat-0.0.2.dev1/src/ctat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-26 11:26:12.000000 ctat-0.0.2.dev1/src/ctat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-26 11:26:12.000000 ctat-0.0.2.dev1/src/ctat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-26 11:26:12.000000 ctat-0.0.2.dev1/src/ctat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 11:26:13.008688 ctat-0.0.2.dev1/src/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-26 11:25:54.000000 ctat-0.0.2.dev1/src/schema/ctat_schema.yaml
```

### Comparing `ctat-0.0.1.dev1/LICENSE` & `ctat-0.0.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctat-0.0.1.dev1/PKG-INFO` & `ctat-0.0.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctat
-Version: 0.0.1.dev1
+Version: 0.0.2.dev1
 Summary: The aim of this project is to specify the Cell Type Annotation schema and related data standardization operations.
 Home-page: https://github.com/hkir-dev/cell-type-annotation-tools
 Author: 
 License: Apache-2.0 license
 Description: # Cell Type Annotation Tools
         
         This repository provides schema of the cell type annotation and related data standardization operations.
```

### Comparing `ctat-0.0.1.dev1/README.md` & `ctat-0.0.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `ctat-0.0.1.dev1/setup.py` & `ctat-0.0.2.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
 
 setup(
     name="ctat",
-    version="0.0.1.dev1",
+    version="0.0.2.dev1",
     description="The aim of this project is to specify the Cell Type Annotation schema and related data standardization operations.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/hkir-dev/cell-type-annotation-tools",
     author="",
     license="Apache-2.0 license",
     classifiers=[
```

### Comparing `ctat-0.0.1.dev1/src/ctat/__main__.py` & `ctat-0.0.2.dev1/src/ctat/__main__.py`

 * *Files identical despite different names*

### Comparing `ctat-0.0.1.dev1/src/ctat/cell_type_annotation.py` & `ctat-0.0.2.dev1/src/ctat/cell_type_annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ctat.schema_validator import load_config, validate
 from ctat.file_utils import read_tsv_to_dict
 
 
 class EncoderMixin(DataClassJsonMixin):
     dataclass_json_config = dataclasses_json.config(
-        letter_case=dataclasses_json.LetterCase.CAMEL,
+        # letter_case=dataclasses_json.LetterCase.CAMEL,
         undefined=dataclasses_json.Undefined.EXCLUDE,
         exclude=lambda f: f is None
     )["dataclasses_json"]
 
 
 @dataclass
 class TaxonomyMetadata(EncoderMixin):
@@ -54,27 +54,29 @@
 
     annotation_set: str
     """The unique name of the set of cell annotations associated with a single file."""
 
     cell_label: str
     """This denotes any free-text term which the author uses to label cells."""
 
+    rank: Optional[int] = 0
+
     cell_ontology_term_id: Optional[str] = None
     """This MUST be a term from either the Cell Ontology or from some ontology that extends it by classifying cell 
     types under terms from the Cell Ontology e.g. the Provisional Cell Ontology."""
 
     cell_ontology_term: Optional[str] = None
     """This MUST be the human-readable name assigned to the value of 'cell_ontology_term_id"""
 
-    accession_id: Optional[str] = None
+    cell_set_accession: Optional[str] = None
 
     cell_ids: Optional[List[str]] = None  # mandatory for cell types
     """List of cell barcode sequences/UUIDs used to uniquely identify the cells"""
 
-    parent_node_name: Optional[str] = None
+    parent_cell_set_name: Optional[str] = None
 
     synonyms: Optional[List[str]] = None
     """This field denotes any free-text term of a biological entity which the author associates as synonymous with the 
     biological entity listed in the field 'cell_label'."""
 
     annotation_transfer: Optional[AnnotationTransfer] = None
 
@@ -137,18 +139,20 @@
         for field in config_fields:
             # handle hierarchical columns
             if field["column_type"] == "cluster_name":
                 ao.annotation_set = field["column_name"]
                 ao.cell_label = str(record[field["column_name"]])
                 utilized_columns.add(field["column_name"])
             if field["column_type"] == "cluster_id":
-                ao.accession_id = str(record[field["column_name"]])
+                ao.cell_set_accession = str(record[field["column_name"]])
+                ao.rank = int(str(field["rank"]).strip())
                 utilized_columns.add(field["column_name"])
             if field["column_type"] == "cell_set":
                 parent_ao = Annotation(field["column_name"], record[field["column_name"]])
+                parent_ao.rank = int(str(field["rank"]).strip())
                 parents.insert(int(str(field["rank"]).strip()), parent_ao)
                 utilized_columns.add(field["column_name"])
             else:
                 # handle annotation columns
                 setattr(ao, field["column_type"], record[field["column_name"]])
                 utilized_columns.add(field["column_name"])
 
@@ -184,20 +188,20 @@
     Creates parent nodes if necessary and creates a cluster hierarchy through assinging parent_node_names.
     :param ao: current annotation object
     :param ao_names: list of all created annotation objects
     :param cta: main object
     :param parents: list of current annotation object's parents
     """
     if parents:
-        ao.parent_node_name = parents[1].cell_label
+        ao.parent_cell_set_name = parents[1].cell_label
         prev = None
         for parent in reversed(parents):
             if parent:
                 if prev:
-                    parent.parent_node_name = prev.cell_label
+                    parent.parent_cell_set_name = prev.cell_label
                 prev = parent
                 if parent.cell_label not in ao_names:
                     cta.add_annotation_object(parent)
                     ao_names[parent.cell_label] = parent
 
 
 def get_taxonomy_metadata(config):
```

### Comparing `ctat-0.0.1.dev1/src/ctat/file_utils.py` & `ctat-0.0.2.dev1/src/ctat/file_utils.py`

 * *Files identical despite different names*

### Comparing `ctat-0.0.1.dev1/src/ctat/schema_validator.py` & `ctat-0.0.2.dev1/src/ctat/schema_validator.py`

 * *Files identical despite different names*

### Comparing `ctat-0.0.1.dev1/src/ctat.egg-info/PKG-INFO` & `ctat-0.0.2.dev1/src/ctat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctat
-Version: 0.0.1.dev1
+Version: 0.0.2.dev1
 Summary: The aim of this project is to specify the Cell Type Annotation schema and related data standardization operations.
 Home-page: https://github.com/hkir-dev/cell-type-annotation-tools
 Author: 
 License: Apache-2.0 license
 Description: # Cell Type Annotation Tools
         
         This repository provides schema of the cell type annotation and related data standardization operations.
```

### Comparing `ctat-0.0.1.dev1/src/schema/ctat_schema.yaml` & `ctat-0.0.2.dev1/src/schema/ctat_schema.yaml`

 * *Files identical despite different names*

