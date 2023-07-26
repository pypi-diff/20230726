# Comparing `tmp/vembrane-1.0.2.tar.gz` & `tmp/vembrane-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vembrane-1.0.2.tar", max compression
+gzip compressed data, was "vembrane-1.0.3.tar", max compression
```

## Comparing `vembrane-1.0.2.tar` & `vembrane-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-06-12 16:11:32.003118 vembrane-1.0.2/LICENSE
--rw-r--r--   0        0        0    19775 2023-06-12 16:11:32.003118 vembrane-1.0.2/README.md
--rw-r--r--   0        0        0     1101 2023-06-12 16:11:32.007118 vembrane-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      325 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/__init__.py
--rw-r--r--   0        0        0    28683 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/ann_types.py
--rw-r--r--   0        0        0      876 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/cli.py
--rw-r--r--   0        0        0     4166 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/common.py
--rw-r--r--   0        0        0     4667 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/errors.py
--rw-r--r--   0        0        0     5259 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/globals.py
--rw-r--r--   0        0        0        0 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/modules/__init__.py
--rw-r--r--   0        0        0     5880 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/modules/annotate.py
--rw-r--r--   0        0        0    13278 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/modules/filter.py
--rw-r--r--   0        0        0    11108 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/modules/table.py
--rw-r--r--   0        0        0     6935 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/modules/tag.py
--rw-r--r--   0        0        0    13621 2023-06-12 16:11:32.019118 vembrane-1.0.2/vembrane/representations.py
--rw-r--r--   0        0        0    20540 1970-01-01 00:00:00.000000 vembrane-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-26 08:23:40.866787 vembrane-1.0.3/LICENSE
+-rw-r--r--   0        0        0    19775 2023-07-26 08:23:40.866787 vembrane-1.0.3/README.md
+-rw-r--r--   0        0        0     1101 2023-07-26 08:23:40.866787 vembrane-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      325 2023-07-26 08:23:40.870787 vembrane-1.0.3/vembrane/__init__.py
+-rw-r--r--   0        0        0    28683 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/ann_types.py
+-rw-r--r--   0        0        0      876 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/cli.py
+-rw-r--r--   0        0        0     4166 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/common.py
+-rw-r--r--   0        0        0     4667 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/errors.py
+-rw-r--r--   0        0        0     5259 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/globals.py
+-rw-r--r--   0        0        0        0 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/modules/__init__.py
+-rw-r--r--   0        0        0     5880 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/modules/annotate.py
+-rw-r--r--   0        0        0    13581 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/modules/filter.py
+-rw-r--r--   0        0        0    11108 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/modules/table.py
+-rw-r--r--   0        0        0     6935 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/modules/tag.py
+-rw-r--r--   0        0        0    13621 2023-07-26 08:23:40.874787 vembrane-1.0.3/vembrane/representations.py
+-rw-r--r--   0        0        0    20540 1970-01-01 00:00:00.000000 vembrane-1.0.3/PKG-INFO
```

### Comparing `vembrane-1.0.2/LICENSE` & `vembrane-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/README.md` & `vembrane-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/pyproject.toml` & `vembrane-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vembrane"
-version = "1.0.2"
+version = "1.0.3"
 description = "Filter VCF/BCF files with Python expressions."
 authors = ["Till Hartmann", "Christopher Schröder", "Johannes Köster", "Jan Forster", "Marcel Bargull", "Felix Mölder", "Elias Kuthe", "David Lähnemann"]
 readme = "README.md"
 homepage = "https://github.com/vembrane/vembrane"
 repository = "https://github.com/vembrane/vembrane"
 
 [tool.poetry.scripts]
```

### Comparing `vembrane-1.0.2/vembrane/ann_types.py` & `vembrane-1.0.3/vembrane/ann_types.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/vembrane/cli.py` & `vembrane-1.0.3/vembrane/cli.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/vembrane/common.py` & `vembrane-1.0.3/vembrane/common.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/vembrane/errors.py` & `vembrane-1.0.3/vembrane/errors.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/vembrane/globals.py` & `vembrane-1.0.3/vembrane/globals.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/vembrane/modules/annotate.py` & `vembrane-1.0.3/vembrane/modules/annotate.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/vembrane/modules/filter.py` & `vembrane-1.0.3/vembrane/modules/filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,18 +168,26 @@
     ann_key: str,
     keep_unmatched: bool = False,
     preserve_order: bool = False,
     auxiliary: Dict[str, Set[str]] = {},
     overwrite_number: Dict[str, Dict[str, str]] = {},
 ) -> Iterator[VariantRecord]:
     env = Environment(expression, ann_key, vcf.header, auxiliary, overwrite_number)
+    has_mateid_key = vcf.header.info.get("MATEID", None) is not None
+    has_event_key = vcf.header.info.get("EVENT", None) is not None
 
-    def get_event_name(record: VariantRecord) -> Tuple[Optional[str], Optional[str]]:
-        mate_ids: List[str] = record.info.get("MATEID", [])
-        event_name: Optional[str] = record.info.get("EVENT", None)
+    def get_event_name(
+        record: VariantRecord,
+        has_mateid_key=has_mateid_key,
+        has_event_key=has_event_key,
+    ) -> Tuple[Optional[str], Optional[str]]:
+        mate_ids: List[str] = record.info.get("MATEID", []) if has_mateid_key else []
+        event_name: Optional[str] = (
+            record.info.get("EVENT", None) if has_event_key else None
+        )
 
         if len(mate_ids) > 1 and not event_name:
             raise ValueError(
                 f"Filtering of BND records with multiple mates is unsupported "
                 f"(see VCF 4.3, section 5.4.3 'Multiple mates'):\n{str(record)}"
             )
 
@@ -197,15 +205,15 @@
         event_dict: Dict[str, BreakendEvent] = dict()
         for idx, record in enumerate(vcf):
             record, keep = test_and_update_record(
                 env, idx, record, ann_key, keep_unmatched
             )
 
             # Breakend records *may* have the "EVENT" specified, but don't have to.
-            # In that case only the MATEID *may* bee available
+            # In that case only the MATEID *may* be available
             # (which may contain more than one ID)
             if is_bnd_record(record):
                 event_name, mate_pair_name = get_event_name(record)
 
                 # if EVENT is set, it has priority over MATEID.
                 event_name = event_name or mate_pair_name
```

### Comparing `vembrane-1.0.2/vembrane/modules/table.py` & `vembrane-1.0.3/vembrane/modules/table.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/vembrane/modules/tag.py` & `vembrane-1.0.3/vembrane/modules/tag.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/vembrane/representations.py` & `vembrane-1.0.3/vembrane/representations.py`

 * *Files identical despite different names*

### Comparing `vembrane-1.0.2/PKG-INFO` & `vembrane-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vembrane
-Version: 1.0.2
+Version: 1.0.3
 Summary: Filter VCF/BCF files with Python expressions.
 Home-page: https://github.com/vembrane/vembrane
 Author: Till Hartmann
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

