# Comparing `tmp/grai_source_dbt-0.3.0a9.tar.gz` & `tmp/grai_source_dbt-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_dbt-0.3.0a9.tar", max compression
+gzip compressed data, was "grai_source_dbt-0.3.1.tar", max compression
```

## Comparing `grai_source_dbt-0.3.0a9.tar` & `grai_source_dbt-0.3.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0      124 2023-05-02 08:01:59.695588 grai_source_dbt-0.3.0a9/README.md
--rw-r--r--   0        0        0     1078 2023-07-12 11:23:17.119508 grai_source_dbt-0.3.0a9/pyproject.toml
--rw-r--r--   0        0        0      217 2023-07-12 10:52:48.694390 grai_source_dbt-0.3.0a9/src/grai_source_dbt/__init__.py
--rw-r--r--   0        0        0      112 2023-02-22 09:54:48.652302 grai_source_dbt-0.3.0a9/src/grai_source_dbt/adapters/__init__.py
--rw-r--r--   0        0        0     8357 2023-07-12 10:52:48.699928 grai_source_dbt-0.3.0a9/src/grai_source_dbt/adapters/adapters.py
--rw-r--r--   0        0        0      695 2023-06-06 17:35:16.802940 grai_source_dbt-0.3.0a9/src/grai_source_dbt/adapters/v5.py
--rw-r--r--   0        0        0     1085 2023-07-12 11:10:18.665361 grai_source_dbt-0.3.0a9/src/grai_source_dbt/base.py
--rw-r--r--   0        0        0    30063 2023-02-14 12:06:39.089774 grai_source_dbt-0.3.0a9/src/grai_source_dbt/data/graph.gpickle
--rw-r--r--   0        0        0   249725 2023-02-14 12:06:39.090263 grai_source_dbt-0.3.0a9/src/grai_source_dbt/data/manifest.json
--rw-r--r--   0        0        0      995 2023-06-06 17:35:16.803842 grai_source_dbt-0.3.0a9/src/grai_source_dbt/data_tools.py
--rw-r--r--   0        0        0     2043 2023-06-06 17:35:16.804153 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/__init__.py
--rw-r--r--   0        0        0      985 2023-06-06 17:35:16.804291 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/base.py
--rw-r--r--   0        0        0      288 2023-06-06 17:35:16.804400 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/utils.py
--rw-r--r--   0        0        0     6197 2023-06-16 16:15:18.431432 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v1.py
--rw-r--r--   0        0        0     1032 2023-02-22 09:54:48.653526 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v2.py
--rw-r--r--   0        0        0     1033 2023-02-22 09:54:48.653655 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v3.py
--rw-r--r--   0        0        0     1109 2023-02-22 09:54:48.653765 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v4.py
--rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653884 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v5.py
--rw-r--r--   0        0        0     1108 2023-02-22 09:54:48.653991 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v6.py
--rw-r--r--   0        0        0     2423 2023-06-06 17:35:16.804770 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v7.py
--rw-r--r--   0        0        0      549 2023-02-24 17:33:29.685755 grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v8.py
--rw-r--r--   0        0        0       48 2023-02-22 09:54:48.654363 grai_source_dbt-0.3.0a9/src/grai_source_dbt/models/__init__.py
--rw-r--r--   0        0        0     2501 2023-06-16 16:15:18.431554 grai_source_dbt-0.3.0a9/src/grai_source_dbt/models/grai.py
--rw-r--r--   0        0        0     2584 2023-06-06 17:35:16.805007 grai_source_dbt-0.3.0a9/src/grai_source_dbt/models/shared.py
--rw-r--r--   0        0        0      189 2023-06-06 17:35:16.805133 grai_source_dbt-0.3.0a9/src/grai_source_dbt/package_definitions.py
--rw-r--r--   0        0        0     2631 2023-07-12 10:52:48.701382 grai_source_dbt-0.3.0a9/src/grai_source_dbt/processor.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.090850 grai_source_dbt-0.3.0a9/src/grai_source_dbt/py.typed
--rw-r--r--   0        0        0     1243 2023-06-06 17:35:16.805384 grai_source_dbt-0.3.0a9/src/grai_source_dbt/utils.py
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 grai_source_dbt-0.3.0a9/PKG-INFO
+-rw-r--r--   0        0        0      124 2023-05-19 11:07:12.925670 grai_source_dbt-0.3.1/README.md
+-rw-r--r--   0        0        0      996 2023-07-26 20:50:36.730141 grai_source_dbt-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      210 2023-07-26 20:50:36.736293 grai_source_dbt-0.3.1/src/grai_source_dbt/__init__.py
+-rw-r--r--   0        0        0      112 2023-02-23 22:53:26.660996 grai_source_dbt-0.3.1/src/grai_source_dbt/adapters/__init__.py
+-rw-r--r--   0        0        0     8256 2023-07-20 03:27:21.116478 grai_source_dbt-0.3.1/src/grai_source_dbt/adapters/adapters.py
+-rw-r--r--   0        0        0      695 2023-06-14 21:02:53.383553 grai_source_dbt-0.3.1/src/grai_source_dbt/adapters/v5.py
+-rw-r--r--   0        0        0     1063 2023-07-20 03:27:21.116582 grai_source_dbt-0.3.1/src/grai_source_dbt/base.py
+-rw-r--r--   0        0        0    30063 2023-01-03 17:11:14.023697 grai_source_dbt-0.3.1/src/grai_source_dbt/data/graph.gpickle
+-rw-r--r--   0        0        0   249725 2023-01-03 17:11:14.024284 grai_source_dbt-0.3.1/src/grai_source_dbt/data/manifest.json
+-rw-r--r--   0        0        0      995 2023-06-14 21:02:53.397163 grai_source_dbt-0.3.1/src/grai_source_dbt/data_tools.py
+-rw-r--r--   0        0        0     2375 2023-07-26 20:51:10.485798 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/__init__.py
+-rw-r--r--   0        0        0      985 2023-06-14 21:02:53.361163 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/base.py
+-rw-r--r--   0        0        0      288 2023-06-01 16:01:43.259425 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/utils.py
+-rw-r--r--   0        0        0     6197 2023-06-15 00:41:57.149113 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v1.py
+-rw-r--r--   0        0        0      499 2023-07-26 20:51:10.157868 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v10.py
+-rw-r--r--   0        0        0     1032 2023-06-14 21:02:53.401692 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v2.py
+-rw-r--r--   0        0        0     1033 2023-06-14 21:02:53.414206 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v3.py
+-rw-r--r--   0        0        0     1109 2023-06-14 21:02:53.264349 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v4.py
+-rw-r--r--   0        0        0     1108 2023-06-14 21:02:53.241314 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v5.py
+-rw-r--r--   0        0        0     1108 2023-06-14 21:02:53.407738 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v6.py
+-rw-r--r--   0        0        0     2423 2023-06-14 21:02:53.245984 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v7.py
+-rw-r--r--   0        0        0      487 2023-07-26 20:51:10.165601 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v8.py
+-rw-r--r--   0        0        0      487 2023-07-26 20:51:10.166595 grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v9.py
+-rw-r--r--   0        0        0       48 2023-02-23 22:53:26.663732 grai_source_dbt-0.3.1/src/grai_source_dbt/models/__init__.py
+-rw-r--r--   0        0        0     2501 2023-06-15 00:41:57.149291 grai_source_dbt-0.3.1/src/grai_source_dbt/models/grai.py
+-rw-r--r--   0        0        0     2584 2023-06-01 16:01:43.259940 grai_source_dbt-0.3.1/src/grai_source_dbt/models/shared.py
+-rw-r--r--   0        0        0      189 2023-06-01 16:01:43.260046 grai_source_dbt-0.3.1/src/grai_source_dbt/package_definitions.py
+-rw-r--r--   0        0        0     3204 2023-07-26 20:51:10.486957 grai_source_dbt-0.3.1/src/grai_source_dbt/processor.py
+-rw-r--r--   0        0        0        0 2023-01-03 17:11:14.024727 grai_source_dbt-0.3.1/src/grai_source_dbt/py.typed
+-rw-r--r--   0        0        0     1243 2023-06-01 16:01:43.260280 grai_source_dbt-0.3.1/src/grai_source_dbt/utils.py
+-rw-r--r--   0        0        0     1000 1970-01-01 00:00:00.000000 grai_source_dbt-0.3.1/PKG-INFO
```

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/adapters/adapters.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/adapters/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,21 +219,17 @@
 
     Returns:
 
     Raises:
 
     """
     integration_meta = build_app_metadata(obj, version)
-    base_metadata = build_grai_metadata(obj, version)
-    integration_meta["grai"] = base_metadata
+    integration_meta["grai"] = build_grai_metadata(obj, version)
 
-    return {
-        base_config.metadata_id: base_metadata,
-        config.metadata_id: integration_meta,
-    }
+    return integration_meta
 
 
 @multimethod
 def adapt_to_client(current: Any, version: Any) -> None:
     """
 
     Args:
@@ -341,24 +337,24 @@
     Raises:
 
     """
     return [adapt_to_client(item, source, version) for item in objs]
 
 
 @adapt_to_client.register
-def adapt_to_client_default_version(obj: Any):
+def adapt_to_client_default_version(obj: Any, source: SourceV1):
     """
 
     Args:
         obj (Any):
 
     Returns:
 
     Raises:
 
     """
-    return adapt_to_client(obj, version="v1")
+    return adapt_to_client(obj, source, "v1")
 
 
 @adapt_to_client.register
 def adapt_source_spec_v1_to_client(obj: X, source: SourceV1, version: Y) -> T:
     return adapt_to_client(obj, source.spec, version)
```

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/adapters/v5.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/adapters/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/base.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,13 @@
     ):
         super().__init__(source, version)
 
         self.manifest_file = manifest_file
         self.namespace = namespace
 
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
-        manifest = ManifestProcessor.load(
-            self.manifest_file, self.namespace, self.source
-        )
+        manifest = ManifestProcessor.load(self.manifest_file, self.namespace, self.source)
         return manifest.adapted_nodes, manifest.adapted_edges
 
     def ready(self) -> bool:
         _ = ManifestProcessor.load(self.manifest_file, self.namespace, self.source)
         return True
```

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/data/graph.gpickle` & `grai_source_dbt-0.3.1/src/grai_source_dbt/data/graph.gpickle`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/data/manifest.json` & `grai_source_dbt-0.3.1/src/grai_source_dbt/data/manifest.json`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/data_tools.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/data_tools.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/__init__.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,51 @@
 from typing import Type, Union, get_args
 
 from dbt_artifacts_parser.parsers.version_map import ArtifactTypes
 
-from grai_source_dbt.loaders import base, utils, v1, v2, v3, v4, v5, v6, v7, v8
+from grai_source_dbt.loaders import base, utils, v1, v2, v3, v4, v5, v6, v7, v8, v9, v10
 from grai_source_dbt.loaders.v1 import ManifestLoaderV1
 from grai_source_dbt.loaders.v7 import ManifestLoaderV7
 from grai_source_dbt.utils import full_name, set_extra_fields
 
 ManifestTypes = Union[
-    v1.ManifestV1, v2.ManifestV2, v3.ManifestV3, v4.ManifestV4, v6.ManifestV6, v7.ManifestV7, v8.ManifestV8
+    v1.ManifestV1,
+    v2.ManifestV2,
+    v3.ManifestV3,
+    v4.ManifestV4,
+    v6.ManifestV6,
+    v7.ManifestV7,
+    v8.ManifestV8,
+    v9.ManifestV9,
+    v10.ManifestV10,
 ]
 NodeTypes = Union[
-    v1.NodeTypes, v2.NodeTypes, v3.NodeTypes, v4.NodeTypes, v5.NodeTypes, v6.NodeTypes, v7.NodeTypes, v8.NodeTypes
+    v1.NodeTypes,
+    v2.NodeTypes,
+    v3.NodeTypes,
+    v4.NodeTypes,
+    v5.NodeTypes,
+    v6.NodeTypes,
+    v7.NodeTypes,
+    v8.NodeTypes,
+    v9.NodeTypes,
+    v10.NodeTypes,
 ]
 
 SourceTypes = Union[
     v1.SourceTypes,
     v2.SourceTypes,
     v3.SourceTypes,
     v4.SourceTypes,
     v5.SourceTypes,
     v6.SourceTypes,
     v7.SourceTypes,
     v8.SourceTypes,
+    v9.SourceTypes,
+    v10.SourceTypes,
 ]
 AllDbtNodeTypes = Union[NodeTypes, SourceTypes]
 AllDbtNodeInstances = get_args(AllDbtNodeTypes)
 set_extra_fields(AllDbtNodeInstances)
 
 
 @full_name.register
@@ -64,11 +83,13 @@
     ArtifactTypes.MANIFEST_V2.value.dbt_schema_version: ManifestLoaderV1,
     ArtifactTypes.MANIFEST_V3.value.dbt_schema_version: ManifestLoaderV1,
     ArtifactTypes.MANIFEST_V4.value.dbt_schema_version: ManifestLoaderV1,
     ArtifactTypes.MANIFEST_V5.value.dbt_schema_version: ManifestLoaderV1,
     ArtifactTypes.MANIFEST_V6.value.dbt_schema_version: ManifestLoaderV1,
     ArtifactTypes.MANIFEST_V7.value.dbt_schema_version: ManifestLoaderV7,
     ArtifactTypes.MANIFEST_V8.value.dbt_schema_version: ManifestLoaderV7,
+    ArtifactTypes.MANIFEST_V9.value.dbt_schema_version: ManifestLoaderV7,
+    # ArtifactTypes.MANIFEST_V10.value.dbt_schema_version: ManifestLoaderV7,
 }
 
 
 SUPPORTED_VERSIONS = [utils.get_schema_id_from_version(label) for label in MANIFEST_MAP.keys()]
```

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/base.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v1.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v1.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v2.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v2.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v3.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v3.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v4.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v4.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v5.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v5.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v6.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v6.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/loaders/v7.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/loaders/v7.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/models/grai.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/models/grai.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/models/shared.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/models/shared.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/src/grai_source_dbt/utils.py` & `grai_source_dbt-0.3.1/src/grai_source_dbt/utils.py`

 * *Files identical despite different names*

### Comparing `grai_source_dbt-0.3.0a9/PKG-INFO` & `grai_source_dbt-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: grai-source-dbt
-Version: 0.3.0a9
+Version: 0.3.1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: dbt-artifacts-parser (>=0.2.4,<0.3.0)
-Requires-Dist: grai-client (>=0.3.0a21,<0.4.0)
-Requires-Dist: grai-schemas (>=0.2.0a1,<0.3.0)
+Requires-Dist: dbt-artifacts-parser (>=v0.4.0-rc1,<0.5.0)
+Requires-Dist: grai-client (>=0.3.0,<0.4.0)
+Requires-Dist: grai-schemas (>=0.2.0,<0.3.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-integrations/source-dbt
 Description-Content-Type: text/markdown
 
 # Grai dbt Integration
```

