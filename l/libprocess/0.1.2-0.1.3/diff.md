# Comparing `tmp/libprocess-0.1.2.tar.gz` & `tmp/libprocess-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libprocess-0.1.2.tar", max compression
+gzip compressed data, was "libprocess-0.1.3.tar", max compression
```

## Comparing `libprocess-0.1.2.tar` & `libprocess-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    34523 2023-07-23 16:52:53.349963 libprocess-0.1.2/LICENSE
--rw-r--r--   0        0        0      761 2023-07-23 16:52:53.349963 libprocess-0.1.2/README.md
--rw-r--r--   0        0        0      313 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/__init__.py
--rw-r--r--   0        0        0     3187 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/_utils/image.py
--rw-r--r--   0        0        0      517 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/_utils/language.py
--rw-r--r--   0        0        0       90 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/david_rumsey_map_collection/__init__.py
--rw-r--r--   0        0        0     6252 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/david_rumsey_map_collection/_process_metadata.py
--rw-r--r--   0        0        0     1590 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/david_rumsey_map_collection/_querier.py
--rw-r--r--   0        0        0     5919 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/david_rumsey_map_collection/_schema.py
--rw-r--r--   0        0        0       56 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/gallica/__init__.py
--rw-r--r--   0        0        0    10264 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/gallica/_process_metadata.py
--rw-r--r--   0        0        0     1502 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/gallica/_querier.py
--rw-r--r--   0        0        0     5382 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/gallica/_schema.py
--rw-r--r--   0        0        0     1025 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/gallica/_utils.py
--rw-r--r--   0        0        0       72 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/internet_archive/__init__.py
--rw-r--r--   0        0        0    10791 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/internet_archive/_process_metadata.py
--rw-r--r--   0        0        0     1626 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/internet_archive/_querier.py
--rw-r--r--   0        0        0     5961 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/internet_archive/_schema.py
--rw-r--r--   0        0        0       76 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/library_of_congress/__init__.py
--rw-r--r--   0        0        0     8754 2023-07-23 16:52:53.349963 libprocess-0.1.2/libprocess/library_of_congress/_process_metadata.py
--rw-r--r--   0        0        0     1554 2023-07-23 16:52:53.353963 libprocess-0.1.2/libprocess/library_of_congress/_querier.py
--rw-r--r--   0        0        0    10292 2023-07-23 16:52:53.353963 libprocess-0.1.2/libprocess/library_of_congress/_schema.py
--rw-r--r--   0        0        0     3466 2023-07-23 16:52:53.353963 libprocess-0.1.2/libprocess/typing.py
--rw-r--r--   0        0        0      545 2023-07-23 16:52:53.353963 libprocess-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 libprocess-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-07-26 11:15:26.134398 libprocess-0.1.3/LICENSE
+-rw-r--r--   0        0        0      761 2023-07-26 11:15:26.134398 libprocess-0.1.3/README.md
+-rw-r--r--   0        0        0      313 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/__init__.py
+-rw-r--r--   0        0        0     3187 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/_utils/image.py
+-rw-r--r--   0        0        0      517 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/_utils/language.py
+-rw-r--r--   0        0        0       90 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/david_rumsey_map_collection/__init__.py
+-rw-r--r--   0        0        0     6156 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/david_rumsey_map_collection/_process_metadata.py
+-rw-r--r--   0        0        0     1610 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/david_rumsey_map_collection/_querier.py
+-rw-r--r--   0        0        0     5919 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/david_rumsey_map_collection/_schema.py
+-rw-r--r--   0        0        0       56 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/gallica/__init__.py
+-rw-r--r--   0        0        0    10244 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/gallica/_process_metadata.py
+-rw-r--r--   0        0        0     1522 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/gallica/_querier.py
+-rw-r--r--   0        0        0     5382 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/gallica/_schema.py
+-rw-r--r--   0        0        0     1025 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/gallica/_utils.py
+-rw-r--r--   0        0        0       72 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/internet_archive/__init__.py
+-rw-r--r--   0        0        0    10771 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/internet_archive/_process_metadata.py
+-rw-r--r--   0        0        0     1646 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/internet_archive/_querier.py
+-rw-r--r--   0        0        0     5961 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/internet_archive/_schema.py
+-rw-r--r--   0        0        0       76 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/library_of_congress/__init__.py
+-rw-r--r--   0        0        0     8712 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/library_of_congress/_process_metadata.py
+-rw-r--r--   0        0        0     1574 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/library_of_congress/_querier.py
+-rw-r--r--   0        0        0    10292 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/library_of_congress/_schema.py
+-rw-r--r--   0        0        0     3110 2023-07-26 11:15:26.134398 libprocess-0.1.3/libprocess/typing.py
+-rw-r--r--   0        0        0      545 2023-07-26 11:15:26.138398 libprocess-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 libprocess-0.1.3/PKG-INFO
```

### Comparing `libprocess-0.1.2/LICENSE` & `libprocess-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libprocess-0.1.2/README.md` & `libprocess-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `libprocess-0.1.2/libprocess/_utils/image.py` & `libprocess-0.1.3/libprocess/_utils/image.py`

 * *Files identical despite different names*

### Comparing `libprocess-0.1.2/libprocess/_utils/language.py` & `libprocess-0.1.3/libprocess/_utils/language.py`

 * *Files identical despite different names*

### Comparing `libprocess-0.1.2/libprocess/david_rumsey_map_collection/_process_metadata.py` & `libprocess-0.1.3/libprocess/david_rumsey_map_collection/_process_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from libquery.david_rumsey_map_collection._typing import (
     MetadataEntry,
     SourceData,
 )
 from libquery.utils.jsonl import load_jl
 from tqdm import tqdm
 
-from ..typing import BaseProcessedMetadataEntry
+from ..typing import ProcessedMetadataEntry
 from .._utils.image import (
     get_md5_by_uuid,
     get_phash_by_uuid,
     get_shape_by_uuid,
     get_storage_size_by_uuid,
 )
 from .._utils.language import detect_iso6393
@@ -107,36 +107,31 @@
 def get_abstract(field_values: List[Dict]) -> Union[str, None]:
     note = get_first_element(get_attr(field_values, "Note"))
     if note is None:
         return note
     return note.replace("\u200b", "").replace("\u00a0", " ")
 
 
-def process(
-    entry: MetadataEntry, img_dir: Union[str, None]
-) -> BaseProcessedMetadataEntry:
+def process(entry: MetadataEntry, img_dir: Union[str, None]) -> ProcessedMetadataEntry:
     """
-    Postprocess a metadata entry.
+    Process a metadata entry.
     If img directory is not provided, do not compute the image attributes.
     """
 
-    id_in_source = entry["idInSource"]
     source_data = entry["sourceData"]
-
-    source_data_id = source_data["id"]
     field_values = source_data["fieldValues"]
 
     # store size4 if exist and size2 otherwise
     download_url: str = (
         source_data["urlSize4"]
         if "urlSize4" in source_data
         else source_data["urlSize2"]
     )
 
-    image_attributes = (
+    image_properties = (
         {}
         if img_dir is None
         else {
             "md5": get_md5_by_uuid(entry["uuid"], img_dir),
             "phash": get_phash_by_uuid(entry["uuid"], img_dir),
             "resolution": get_shape_by_uuid(entry["uuid"], img_dir),
             "fileSize": get_storage_size_by_uuid(entry["uuid"], img_dir),
@@ -146,42 +141,42 @@
     return {
         "uuid": entry["uuid"],
         "authors": get_authors(field_values),
         "displayName": get_display_name(source_data),
         "publishDate": {
             "year": int(get_first_element(get_attr(field_values, "Pub Date"))),
         },
-        "viewUrl": f"https://www.davidrumsey.com/luna/servlet/detail/{source_data_id}",
+        "viewUrl": f"https://www.davidrumsey.com/luna/servlet/detail/{source_data['id']}",
         "downloadUrl": download_url,
-        **image_attributes,
+        **image_properties,
         "languages": get_languages(field_values),
         "tags": get_tags(field_values),
         # Note: all the entries have either no note (stored as None) or 1 note
         "abstract": get_abstract(field_values),
         # Reference: https://www.davidrumsey.com/about
         "rights": "CC BY-NC-SA 3.0",
         "source": {
             "name": entry["source"],
             # Note: do not use entry['url'], which is not a stable link
-            "url": f"https://www.davidrumsey.com/luna/servlet/as/search?mid={id_in_source}",
+            "url": f"https://www.davidrumsey.com/luna/servlet/as/search?mid={entry['idInSource']}",
             "accessDate": entry["accessDate"],
         },
         # Deprecated properties:
         # 'publisher': get_first_element(get_attr(field_values, 'Publisher')),
         # 'publisherAddress': get_first_element(get_attr(field_values, 'Publisher Location')),
         # 'publishTitle': publish_title,
         # 'publishNote': get_first_element(get_attr(field_values, 'Pub Note')),
     }
 
 
 def process_batch(
     metadata_path: str,
     img_dir: Union[str, None],
     uuids: Union[List[str], None] = None,
-) -> List[BaseProcessedMetadataEntry]:
+) -> List[ProcessedMetadataEntry]:
     """
     Process a batch of metadata entries.
     """
 
     metadata = load_jl(metadata_path)
     processed_metadata = [
         process(d, img_dir)
```

### Comparing `libprocess-0.1.2/libprocess/david_rumsey_map_collection/_querier.py` & `libprocess-0.1.3/libprocess/david_rumsey_map_collection/_querier.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,11 +42,11 @@
         """
 
         output_dir = os.path.dirname(save_path)
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
         img_dir = self.img_dir if use_img else None
-        metadata = process_batch(self.metadata_path, img_dir, uuids)
+        processed_metadata = process_batch(self.metadata_path, img_dir, uuids)
 
         with open(save_path, "w", encoding="utf-8") as f:
-            f.write(json.dumps(metadata, indent=4, ensure_ascii=False))
+            f.write(json.dumps(processed_metadata, indent=4, ensure_ascii=False))
```

### Comparing `libprocess-0.1.2/libprocess/david_rumsey_map_collection/_schema.py` & `libprocess-0.1.3/libprocess/david_rumsey_map_collection/_schema.py`

 * *Files identical despite different names*

### Comparing `libprocess-0.1.2/libprocess/gallica/_process_metadata.py` & `libprocess-0.1.3/libprocess/gallica/_process_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,24 @@
     - numero
     - pagination_type
 """
 
 import re
 from typing import Any, Dict, List, Union
 
-from tqdm import tqdm
 from libquery.gallica._typing import (
     MetadataEntry,
     Page,
     Record,
 )
 from libquery.utils.jsonl import load_jl
+from tqdm import tqdm
 
 from ..typing import (
-    BaseProcessedMetadataEntry,
+    ProcessedMetadataEntry,
     TimePoint,
 )
 from .._utils.image import (
     get_md5_by_uuid,
     get_phash_by_uuid,
     get_shape_by_uuid,
     get_storage_size_by_uuid,
@@ -245,17 +245,17 @@
     return None
 
 
 def process(
     entry: MetadataEntry,
     img_dir: Union[str, None],
     uuids: Union[List[str], None] = None,
-) -> List[BaseProcessedMetadataEntry]:
+) -> List[ProcessedMetadataEntry]:
     """
-    Postprocess a metadata entry.
+    Process a metadata entry.
     Create a list of metadata entries from the metadata entry.
     If img directory is not provided, do not compute the image attributes.
 
     Each metadata entry stored in Gallica contains a list of images.
     """
 
     metadata_entries = []
@@ -324,17 +324,17 @@
     return metadata_entries
 
 
 def process_batch(
     metadata_path: str,
     img_dir: Union[str, None],
     uuids: Union[List[str], None] = None,
-) -> List[BaseProcessedMetadataEntry]:
+) -> List[ProcessedMetadataEntry]:
     """
-    Postprocess a batch of metadata entries.
+    Process a batch of metadata entries.
     """
 
     metadata = load_jl(metadata_path)
     processed_metadata = []
     for d in tqdm(metadata, desc="Process Metadata Progress"):
         if "pages" not in d["sourceData"]:
             continue
```

### Comparing `libprocess-0.1.2/libprocess/gallica/_querier.py` & `libprocess-0.1.3/libprocess/gallica/_querier.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,11 +42,11 @@
         """
 
         output_dir = os.path.dirname(save_path)
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
         img_dir = self.img_dir if use_img else None
-        metadata = process_batch(self.metadata_path, img_dir, uuids)
+        processed_metadata = process_batch(self.metadata_path, img_dir, uuids)
 
         with open(save_path, "w", encoding="utf-8") as f:
-            f.write(json.dumps(metadata, indent=4, ensure_ascii=False))
+            f.write(json.dumps(processed_metadata, indent=4, ensure_ascii=False))
```

### Comparing `libprocess-0.1.2/libprocess/gallica/_schema.py` & `libprocess-0.1.3/libprocess/gallica/_schema.py`

 * *Files identical despite different names*

### Comparing `libprocess-0.1.2/libprocess/gallica/_utils.py` & `libprocess-0.1.3/libprocess/gallica/_utils.py`

 * *Files identical despite different names*

### Comparing `libprocess-0.1.2/libprocess/internet_archive/_process_metadata.py` & `libprocess-0.1.3/libprocess/internet_archive/_process_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from libquery.internet_archive._utils import get_image_uuid
 from nltk import ne_chunk, pos_tag, word_tokenize
 from nltk.tree import Tree
 from tqdm import tqdm
 from zipfile import ZipFile
 
 from ..typing import (
-    BaseProcessedMetadataEntry,
+    ProcessedMetadataEntry,
     TimePoint,
 )
 from .._utils.image import (
     get_md5_by_path,
     get_phash_by_path,
     get_shape_by_path,
     get_storage_size_by_path,
@@ -165,17 +165,17 @@
 
 
 def process(
     entry: MetadataEntry,
     download_dir: str,
     img_dir: Union[str, None],
     uuids: Union[List[str], None] = None,
-) -> List[BaseProcessedMetadataEntry]:
+) -> List[ProcessedMetadataEntry]:
     """
-    Postprocess a metadata entry.
+    Process a metadata entry.
     If img directory is not provided, do not compute the image attributes.
     """
 
     id_in_source = entry["idInSource"]
     source_data = entry["sourceData"]
     identifier = source_data["metadata"]["identifier"]
     filename = _get_filename(source_data)
@@ -277,17 +277,17 @@
 
 
 def process_batch(
     metadata_path: str,
     download_dir: str,
     img_dir: Union[str, None],
     uuids: Union[List[str], None] = None,
-) -> List[BaseProcessedMetadataEntry]:
+) -> List[ProcessedMetadataEntry]:
     """
-    Postprocess a batch of metadata entries.
+    Process a batch of metadata entries.
     """
 
     metadata = load_jl(metadata_path)
     processed_metadata = []
     for d in tqdm(metadata, desc="Process Metadata Progress"):
         processed_metadata += process(d, download_dir, img_dir, uuids)
```

### Comparing `libprocess-0.1.2/libprocess/internet_archive/_querier.py` & `libprocess-0.1.3/libprocess/internet_archive/_querier.py`

 * *Files 15% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         """
 
         output_dir = os.path.dirname(save_path)
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
         img_dir = self.img_dir if use_img else None
-        metadata = process_batch(
+        processed_metadata = process_batch(
             self.metadata_path,
             self.download_dir,
             img_dir,
             uuids,
         )
 
         with open(save_path, "w", encoding="utf-8") as f:
-            f.write(json.dumps(metadata, indent=4, ensure_ascii=False))
+            f.write(json.dumps(processed_metadata, indent=4, ensure_ascii=False))
```

### Comparing `libprocess-0.1.2/libprocess/internet_archive/_schema.py` & `libprocess-0.1.3/libprocess/internet_archive/_schema.py`

 * *Files identical despite different names*

### Comparing `libprocess-0.1.2/libprocess/library_of_congress/_process_metadata.py` & `libprocess-0.1.3/libprocess/library_of_congress/_process_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 from libquery.library_of_congress._typing import (
     MetadataEntry,
     SourceData,
 )
 from libquery.utils.jsonl import load_jl
 from tqdm import tqdm
 
-from ..typing import BaseProcessedMetadataEntry, TimePoint
+from ..typing import ProcessedMetadataEntry, TimePoint
 from .._utils.image import (
     get_md5_by_uuid,
     get_phash_by_uuid,
     get_shape_by_uuid,
     get_storage_size_by_uuid,
 )
 
@@ -225,39 +225,36 @@
     assert len(rights) <= 1, f"Unexpected rights with length > 1: {rights}"
 
     if len(rights) == 0:
         return "unknown"
     return clean_rights(rights[0])
 
 
-def process(
-    entry: MetadataEntry, img_dir: Union[str, None]
-) -> BaseProcessedMetadataEntry:
+def process(entry: MetadataEntry, img_dir: Union[str, None]) -> ProcessedMetadataEntry:
     """
-    Postprocess a metadata entry.
+    Process a metadata entry.
     If img directory is not provided, do not compute the image attributes.
     """
 
     source_data = entry["sourceData"]
-    item = source_data["item"]
 
     image_properties = (
         {}
         if img_dir is None
         else {
             "md5": get_md5_by_uuid(entry["uuid"], img_dir),
             "phash": get_phash_by_uuid(entry["uuid"], img_dir),
             "resolution": get_shape_by_uuid(entry["uuid"], img_dir),
             "fileSize": get_storage_size_by_uuid(entry["uuid"], img_dir),
         }
     )
 
     return {
         "uuid": entry["uuid"],
-        "authors": item.get("contributors", None),
+        "authors": source_data["item"].get("contributors", None),
         "displayName": source_data["title"],
         "publishDate": get_publish_date(source_data),
         "viewUrl": source_data["url"],
         # Note: the image_url stores URLs of the image with different resolution.
         # The last entry of the image_url gives the highest resolution.
         "downloadUrl": source_data["image_url"][-1],
         **image_properties,
@@ -273,17 +270,17 @@
     }
 
 
 def process_batch(
     metadata_path: str,
     img_dir: Union[str, None],
     uuids: Union[List[str], None] = None,
-) -> List[BaseProcessedMetadataEntry]:
+) -> List[ProcessedMetadataEntry]:
     """
-    Postprocess a batch of metadata entries.
+    Process a batch of metadata entries.
     """
 
     metadata = load_jl(metadata_path)
     processed_metadata = [
         process(d, img_dir)
         for d in tqdm(metadata, desc="Process Metadata Progress")
         if (uuids is None) or (d["uuid"] in uuids)
```

### Comparing `libprocess-0.1.2/libprocess/library_of_congress/_querier.py` & `libprocess-0.1.3/libprocess/library_of_congress/_querier.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,11 +42,11 @@
         """
 
         output_dir = os.path.dirname(save_path)
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
         img_dir = self.img_dir if use_img else None
-        metadata = process_batch(self.metadata_path, img_dir, uuids)
+        processed_metadata = process_batch(self.metadata_path, img_dir, uuids)
 
         with open(save_path, "w", encoding="utf-8") as f:
-            f.write(json.dumps(metadata, indent=4, ensure_ascii=False))
+            f.write(json.dumps(processed_metadata, indent=4, ensure_ascii=False))
```

### Comparing `libprocess-0.1.2/libprocess/library_of_congress/_schema.py` & `libprocess-0.1.3/libprocess/library_of_congress/_schema.py`

 * *Files identical despite different names*

### Comparing `libprocess-0.1.2/libprocess/typing.py` & `libprocess-0.1.3/libprocess/typing.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     """
 
     name: str
     url: str
     accessDate: str
 
 
-class BaseProcessedMetadataEntry(TypedDict):
+class ProcessedMetadataEntry(TypedDict):
     """
     The data structure of an entry of processed metadata.
 
     Attributes
     ----------
     uuid : str
         The UUID of the metadata entry.
@@ -54,21 +54,21 @@
     viewUrl : str
         The url where the item can be viewed in a browser.
     downloadUrl : str
         The url where the item can be downloaded with a get request.
         DownloadUrl can serve the purpose of viewUrl,
         while viewUrl may not always be the same as downloadUrl,
         because some data sources provide web-based viewing functions.
-    md5 : str
+    md5 : NotRequired[str]
         The MD5 hash of the image.
-    phash : str
+    phash : NotRequired[str]
         The perceptual hash of the visualization image.
-    resolution : Tuple[int, int]
+    resolution : NotRequired[Tuple[int, int]]
         The (width, height) of the image in pixels.
-    fileSize: int
+    fileSize: NotRequired[int]
         The storage size of the image in bytes.
     languages : Union[List[str], None]
         The languages used in the visualization.
         Store the language name in ISO 639-3 codes.
         Store None if unknown.
     tags : List[str]
         The tags of the item to be used for searching.
@@ -84,34 +84,16 @@
 
     uuid: str
     authors: Union[List[str], None]
     displayName: str
     publishDate: Union[TimePoint, List[TimePoint], None]
     viewUrl: str
     downloadUrl: str
+    md5: NotRequired[str]
+    phash: NotRequired[str]
+    resolution: NotRequired[Tuple[int, int]]
+    fileSize: NotRequired[int]
     languages: Union[List[str], None]
     tags: List[str]
     abstract: Union[str, None]
     rights: str
     source: Source
-
-
-class ProcessedMetadataEntry(BaseProcessedMetadataEntry):
-    """
-    The data structure of an entry of processed metadata.
-
-    Attributes
-    ----------
-    md5 : str
-        The MD5 hash of the image.
-    phash : str
-        The perceptual hash of the visualization image.
-    resolution : Tuple[int, int]
-        The (width, height) of the image in pixels.
-    fileSize: int
-        The storage size of the image in bytes.
-    """
-
-    md5: str
-    phash: str
-    resolution: Tuple[int, int]
-    fileSize: int
```

### Comparing `libprocess-0.1.2/pyproject.toml` & `libprocess-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libprocess"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Yu Zhang <yuzhang94@outlook.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 jsonschema = "^4.18.3"
```

### Comparing `libprocess-0.1.2/PKG-INFO` & `libprocess-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libprocess
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Yu Zhang
 Author-email: yuzhang94@outlook.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libprocess Version: 0.1.2 Summary: Author: Yu Zhang
+Metadata-Version: 2.1 Name: libprocess Version: 0.1.3 Summary: Author: Yu Zhang
 Author-email: yuzhang94@outlook.com Requires-Python: >=3.10,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 html2text (>=2020.1.16,<2021.0.0) Requires-Dist: imagehash (>=4.3.1,<5.0.0)
 Requires-Dist: jsonschema (>=4.18.3,<5.0.0) Requires-Dist: langcodes
 (>=3.3.0,<4.0.0) Requires-Dist: langdetect (>=1.0.9,<2.0.0) Requires-Dist:
 language-data (>=1.1,<2.0) Requires-Dist: libquery (>=0.1.1,<0.2.0) Requires-
```

