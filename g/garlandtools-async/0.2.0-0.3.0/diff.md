# Comparing `tmp/garlandtools_async-0.2.0.tar.gz` & `tmp/garlandtools_async-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garlandtools_async-0.2.0.tar", max compression
+gzip compressed data, was "garlandtools_async-0.3.0.tar", max compression
```

## Comparing `garlandtools_async-0.2.0.tar` & `garlandtools_async-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/LICENSE
--rw-r--r--   0        0        0      571 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/__init__.py
--rw-r--r--   0        0        0     2640 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/client.py
--rw-r--r--   0        0        0        0 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/__init__.py
--rw-r--r--   0        0        0      152 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/lang.py
--rw-r--r--   0        0        0        0 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/partials/__init__.py
--rw-r--r--   0        0        0      593 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/partials/item_partial.py
--rw-r--r--   0        0        0      311 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/partials/partial.py
--rw-r--r--   0        0        0     2301 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/records/base_record.py
--rw-r--r--   0        0        0     1253 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/records/factory.py
--rw-r--r--   0        0        0     2820 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/records/item.py
--rw-r--r--   0        0        0      328 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/garlandtools/models/type.py
--rw-r--r--   0        0        0      848 2023-06-25 00:10:43.069486 garlandtools_async-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 garlandtools_async-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/LICENSE
+-rw-r--r--   0        0        0      571 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/__init__.py
+-rw-r--r--   0        0        0     2640 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/client.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/models/__init__.py
+-rw-r--r--   0        0        0      152 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/models/lang.py
+-rw-r--r--   0        0        0        0 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/models/partials/__init__.py
+-rw-r--r--   0        0        0      593 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/models/partials/item_partial.py
+-rw-r--r--   0        0        0      311 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/models/partials/partial.py
+-rw-r--r--   0        0        0     2301 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/models/records/base_record.py
+-rw-r--r--   0        0        0     1253 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/models/records/factory.py
+-rw-r--r--   0        0        0     2820 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/models/records/item.py
+-rw-r--r--   0        0        0      328 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/garlandtools/models/type.py
+-rw-r--r--   0        0        0      848 2023-07-26 21:23:43.774020 garlandtools_async-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 garlandtools_async-0.3.0/PKG-INFO
```

### Comparing `garlandtools_async-0.2.0/LICENSE` & `garlandtools_async-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.2.0/README.md` & `garlandtools_async-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.2.0/garlandtools/client.py` & `garlandtools_async-0.3.0/garlandtools/client.py`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.2.0/garlandtools/models/partials/item_partial.py` & `garlandtools_async-0.3.0/garlandtools/models/partials/item_partial.py`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.2.0/garlandtools/models/records/base_record.py` & `garlandtools_async-0.3.0/garlandtools/models/records/base_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from garlandtools.models.partials.item_partial import ItemPartial
 
 
 class BaseRecord(ABC):
     @property
     @abstractmethod
-    def TYPE(self) -> Type:
+    def type(self) -> Type:
         """The type of the record."""
 
     @property
     def id(self) -> int:
         """The ID of the item record."""
         if self._data is not None:
             return self._data["id"]
@@ -55,16 +55,16 @@
             return self._data[key]
 
         async with self._fetch_lock:
             # Check again in case another coroutine
             # fetched the data while we were waiting
             if self._data is not None:
                 return self._data[key]
-            record_data = await self._client._get_by_id(self.id, self.TYPE)
-            self._data = record_data[self.TYPE.value]
+            record_data = await self._client._get_by_id(self.id, self.type)
+            self._data = record_data[self.type.value]
             self._related_records = [
                 partial_factory(partial, client=self._client)
                 for partial in record_data["partials"]
             ]
             return self._data[key]
 
     def __repr__(self) -> str:
```

### Comparing `garlandtools_async-0.2.0/garlandtools/models/records/factory.py` & `garlandtools_async-0.3.0/garlandtools/models/records/factory.py`

 * *Files identical despite different names*

### Comparing `garlandtools_async-0.2.0/garlandtools/models/records/item.py` & `garlandtools_async-0.3.0/garlandtools/models/records/item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from garlandtools.models.records.base_record import BaseRecord
 from garlandtools.models.type import Type
 
 
 class Item(BaseRecord):
     @property
-    def TYPE(self) -> Type:
+    def type(self) -> Type:
         """The type of the record."""
         return Type.ITEM
 
     @property
     def ilvl(self) -> int:
         """The item level of the item."""
         if self._data is not None:
```

### Comparing `garlandtools_async-0.2.0/pyproject.toml` & `garlandtools_async-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "garlandtools-async"
-version = "0.2.0"
+version = "0.3.0"
 description = "A async python wrapper for the https://garlandtools.org/ API"
 authors = ["Abigail Howe <abby@abigailhowe.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "garlandtools"}]
 
 [tool.poetry.dependencies]
```

### Comparing `garlandtools_async-0.2.0/PKG-INFO` & `garlandtools_async-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garlandtools-async
-Version: 0.2.0
+Version: 0.3.0
 Summary: A async python wrapper for the https://garlandtools.org/ API
 License: MIT
 Author: Abigail Howe
 Author-email: abby@abigailhowe.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

