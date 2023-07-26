# Comparing `tmp/pip_services4_persistence-0.0.1.tar.gz` & `tmp/pip_services4_persistence-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_persistence-0.0.1.tar", last modified: Wed Jul 26 00:21:59 2023, max compression
+gzip compressed data, was "pip_services4_persistence-0.0.2.tar", last modified: Wed Jul 26 00:32:57 2023, max compression
```

## Comparing `pip_services4_persistence-0.0.1.tar` & `pip_services4_persistence-0.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 00:21:59.343923 pip_services4_persistence-0.0.1/
--rw-rw-rw-   0        0        0      297 2023-07-25 23:10:37.000000 pip_services4_persistence-0.0.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1076 2020-12-11 04:36:42.000000 pip_services4_persistence-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       54 2020-12-11 04:36:42.000000 pip_services4_persistence-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2518 2023-07-26 00:21:59.343923 pip_services4_persistence-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1588 2023-07-25 23:44:10.000000 pip_services4_persistence-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 00:21:59.314221 pip_services4_persistence-0.0.1/pip_services4_persistence/
--rw-rw-rw-   0        0        0       38 2023-07-26 00:21:10.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 00:21:59.326705 pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/
--rw-rw-rw-   0        0        0     2203 2023-07-25 23:53:31.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/FilePersistence.py
--rw-rw-rw-   0        0        0     3459 2023-07-25 23:58:15.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/IdentifiableFilePersistence.py
--rw-rw-rw-   0        0        0     8245 2023-07-25 23:54:21.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/IdentifiableMemoryPersistence.py
--rw-rw-rw-   0        0        0     3964 2023-07-25 23:58:15.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/JsonFilePersister.py
--rw-rw-rw-   0        0        0    12134 2023-07-25 23:59:58.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/MemoryPersistence.py
--rw-rw-rw-   0        0        0     1359 2020-12-11 04:36:42.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 00:21:59.333707 pip_services4_persistence-0.0.1/pip_services4_persistence/read/
--rw-rw-rw-   0        0        0     1341 2023-07-25 23:59:58.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/read/IFilteredPageReader.py
--rw-rw-rw-   0        0        0     1323 2023-07-26 00:00:24.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/read/IFilteredReader.py
--rw-rw-rw-   0        0        0      986 2023-07-26 00:01:20.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/read/IGetter.py
--rw-rw-rw-   0        0        0      850 2023-07-26 00:01:20.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/read/ILoader.py
--rw-rw-rw-   0        0        0     1339 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/read/IQuerablePageReader.py
--rw-rw-rw-   0        0        0     1175 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/read/IQuerableReader.py
--rw-rw-rw-   0        0        0      889 2020-12-11 04:36:42.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/read/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 00:21:59.338706 pip_services4_persistence-0.0.1/pip_services4_persistence/write/
--rw-rw-rw-   0        0        0     1108 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/write/IPartialUpdater.py
--rw-rw-rw-   0        0        0      840 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/write/ISaver.py
--rw-rw-rw-   0        0        0      951 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/write/ISetter.py
--rw-rw-rw-   0        0        0     1636 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/write/IWriter.py
--rw-rw-rw-   0        0        0        0 2023-07-25 23:46:30.000000 pip_services4_persistence-0.0.1/pip_services4_persistence/write/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-26 00:21:59.321221 pip_services4_persistence-0.0.1/pip_services4_persistence.egg-info/
--rw-rw-rw-   0        0        0     2518 2023-07-26 00:21:59.000000 pip_services4_persistence-0.0.1/pip_services4_persistence.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1560 2023-07-26 00:21:59.000000 pip_services4_persistence-0.0.1/pip_services4_persistence.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 00:21:59.000000 pip_services4_persistence-0.0.1/pip_services4_persistence.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      142 2023-07-26 00:21:59.000000 pip_services4_persistence-0.0.1/pip_services4_persistence.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-26 00:21:59.000000 pip_services4_persistence-0.0.1/pip_services4_persistence.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 00:21:59.000000 pip_services4_persistence-0.0.1/pip_services4_persistence.egg-info/zip-safe
--rw-rw-rw-   0        0        0      180 2023-07-26 00:21:59.344928 pip_services4_persistence-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1769 2023-07-26 00:16:27.000000 pip_services4_persistence-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-26 00:21:59.308219 pip_services4_persistence-0.0.1/test/
-drwxrwxrwx   0        0        0        0 2023-07-26 00:21:59.342883 pip_services4_persistence-0.0.1/test/persistence/
--rw-rw-rw-   0        0        0      854 2023-07-26 00:06:22.000000 pip_services4_persistence-0.0.1/test/persistence/DummyFilePersistence.py
--rw-rw-rw-   0        0        0     1102 2023-07-26 00:13:23.000000 pip_services4_persistence-0.0.1/test/persistence/DummyMemoryPersistence.py
--rw-rw-rw-   0        0        0        0 2020-12-11 04:36:42.000000 pip_services4_persistence-0.0.1/test/persistence/__init__.py
--rw-rw-rw-   0        0        0      994 2023-07-26 00:13:23.000000 pip_services4_persistence-0.0.1/test/persistence/test_DummyFilePersistence.py
--rw-rw-rw-   0        0        0      924 2023-07-26 00:13:23.000000 pip_services4_persistence-0.0.1/test/persistence/test_DummyMemoryPersistence.py
--rw-rw-rw-   0        0        0      832 2023-07-26 00:13:23.000000 pip_services4_persistence-0.0.1/test/persistence/test_JsonFilePersister.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:32:57.572245 pip_services4_persistence-0.0.2/
+-rw-rw-rw-   0        0        0      297 2023-07-25 23:10:37.000000 pip_services4_persistence-0.0.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1076 2020-12-11 04:36:42.000000 pip_services4_persistence-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-12-11 04:36:42.000000 pip_services4_persistence-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2518 2023-07-26 00:32:57.572245 pip_services4_persistence-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1588 2023-07-25 23:44:10.000000 pip_services4_persistence-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-26 00:32:57.551246 pip_services4_persistence-0.0.2/pip_services4_persistence/
+-rw-rw-rw-   0        0        0       38 2023-07-26 00:21:10.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:32:57.560246 pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/
+-rw-rw-rw-   0        0        0     2217 2023-07-26 00:31:29.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/FilePersistence.py
+-rw-rw-rw-   0        0        0     3459 2023-07-25 23:58:15.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/IdentifiableFilePersistence.py
+-rw-rw-rw-   0        0        0     8530 2023-07-26 00:31:29.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/IdentifiableMemoryPersistence.py
+-rw-rw-rw-   0        0        0     3964 2023-07-25 23:58:15.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/JsonFilePersister.py
+-rw-rw-rw-   0        0        0    12134 2023-07-25 23:59:58.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/MemoryPersistence.py
+-rw-rw-rw-   0        0        0     1359 2020-12-11 04:36:42.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:32:57.565245 pip_services4_persistence-0.0.2/pip_services4_persistence/read/
+-rw-rw-rw-   0        0        0     1403 2023-07-26 00:30:21.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/read/IFilteredPageReader.py
+-rw-rw-rw-   0        0        0     1323 2023-07-26 00:00:24.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/read/IFilteredReader.py
+-rw-rw-rw-   0        0        0      986 2023-07-26 00:01:20.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/read/IGetter.py
+-rw-rw-rw-   0        0        0      850 2023-07-26 00:01:20.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/read/ILoader.py
+-rw-rw-rw-   0        0        0     1339 2023-07-26 00:31:29.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/read/IQuerablePageReader.py
+-rw-rw-rw-   0        0        0     1175 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/read/IQuerableReader.py
+-rw-rw-rw-   0        0        0      705 2023-07-26 00:30:00.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/read/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:32:57.568245 pip_services4_persistence-0.0.2/pip_services4_persistence/write/
+-rw-rw-rw-   0        0        0     1108 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/write/IPartialUpdater.py
+-rw-rw-rw-   0        0        0      840 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/write/ISaver.py
+-rw-rw-rw-   0        0        0      951 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/write/ISetter.py
+-rw-rw-rw-   0        0        0     1636 2023-07-26 00:02:27.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/write/IWriter.py
+-rw-rw-rw-   0        0        0      175 2023-07-26 00:29:38.000000 pip_services4_persistence-0.0.2/pip_services4_persistence/write/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:32:57.556245 pip_services4_persistence-0.0.2/pip_services4_persistence.egg-info/
+-rw-rw-rw-   0        0        0     2518 2023-07-26 00:32:57.000000 pip_services4_persistence-0.0.2/pip_services4_persistence.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1560 2023-07-26 00:32:57.000000 pip_services4_persistence-0.0.2/pip_services4_persistence.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-26 00:32:57.000000 pip_services4_persistence-0.0.2/pip_services4_persistence.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      142 2023-07-26 00:32:57.000000 pip_services4_persistence-0.0.2/pip_services4_persistence.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-26 00:32:57.000000 pip_services4_persistence-0.0.2/pip_services4_persistence.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-26 00:31:58.000000 pip_services4_persistence-0.0.2/pip_services4_persistence.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      180 2023-07-26 00:32:57.573245 pip_services4_persistence-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1769 2023-07-26 00:32:39.000000 pip_services4_persistence-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-26 00:32:57.545248 pip_services4_persistence-0.0.2/test/
+drwxrwxrwx   0        0        0        0 2023-07-26 00:32:57.572245 pip_services4_persistence-0.0.2/test/persistence/
+-rw-rw-rw-   0        0        0      854 2023-07-26 00:06:22.000000 pip_services4_persistence-0.0.2/test/persistence/DummyFilePersistence.py
+-rw-rw-rw-   0        0        0     1103 2023-07-26 00:28:43.000000 pip_services4_persistence-0.0.2/test/persistence/DummyMemoryPersistence.py
+-rw-rw-rw-   0        0        0        0 2020-12-11 04:36:42.000000 pip_services4_persistence-0.0.2/test/persistence/__init__.py
+-rw-rw-rw-   0        0        0      994 2023-07-26 00:13:23.000000 pip_services4_persistence-0.0.2/test/persistence/test_DummyFilePersistence.py
+-rw-rw-rw-   0        0        0      924 2023-07-26 00:13:23.000000 pip_services4_persistence-0.0.2/test/persistence/test_DummyMemoryPersistence.py
+-rw-rw-rw-   0        0        0      832 2023-07-26 00:13:23.000000 pip_services4_persistence-0.0.2/test/persistence/test_JsonFilePersister.py
```

### Comparing `pip_services4_persistence-0.0.1/LICENSE` & `pip_services4_persistence-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/PKG-INFO` & `pip_services4_persistence-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_persistence
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data processing and persistence components for Pip.Services in Python
 Home-page: http://github.com/pip-services3-python/pip-services4-persistence-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_persistence-0.0.1/README.md` & `pip_services4_persistence-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/FilePersistence.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/FilePersistence.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     File persistence implementation.
     
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
 from typing import Optional
 
-from pip_services4_components.config import IConfigurable
+from pip_services4_components.config import IConfigurable, ConfigParams
 
 from .JsonFilePersister import JsonFilePersister
 from .MemoryPersistence import MemoryPersistence
 
 
 class FilePersistence(MemoryPersistence, IConfigurable):
     """
```

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/IdentifiableFilePersistence.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/IdentifiableFilePersistence.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/IdentifiableMemoryPersistence.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/IdentifiableMemoryPersistence.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,22 @@
     Identifiable memory persistence implementation
     
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
 from typing import Optional, Any, List, TypeVar
 
+from pip_services4_commons.data import AnyValueMap
+from pip_services4_components.context import IContext
+from pip_services4_data.data import IIdentifiable
+from pip_services4_data.keys import IdGenerator
 
 from .MemoryPersistence import MemoryPersistence
-from ..read import IGetter
+from ..read import IGetter, ILoader
+from ..write import ISaver
 from ..write.ISetter import ISetter
 from ..write.IWriter import IWriter
 
 # This function will be overriden in the code
 filtered = filter
 
 T = TypeVar('T')  # Declare type variable
@@ -52,17 +57,17 @@
         class MyMemoryPersistence(IdentifiableMemoryPersistence):
 
             def get_page_by_filter(self, context, filter, paging):
                 super().get_page_by_filter(context, filter, paging, None)
 
             persistence = MyMemoryPersistence("./data/data.json")
 
-            item = persistence.create("123", MyData("1", "ABC"))
+            item = persistence.create(Context.from_trace_id("123"), MyData("1", "ABC"))
 
-            mydata = persistence.get_page_by_filter("123", FilterParams.from_tuples("name", "ABC"), None, None)
+            mydata = persistence.get_page_by_filter(Context.from_trace_id("123"), FilterParams.from_tuples("name", "ABC"), None, None)
             print str(mydata.get_data())
 
             persistence.delete_by_id("123", "1")
     """
 
     def __init__(self, loader: ILoader = None, saver: ISaver = None):
         """
```

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/JsonFilePersister.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/JsonFilePersister.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/MemoryPersistence.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/MemoryPersistence.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/persistence/__init__.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/read/IFilteredPageReader.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/read/IFilteredReader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # -*- coding: utf-8 -*-
 """
-    pip_services3_data.IFilteredPageReader
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    pip_services3_data.IFilteredReader
+    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     
-    Interface for filtered paging data readers.
+    Interface for filtered data readers.
     
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
 from abc import ABC
-from typing import Optional
+from typing import List, Optional, TypeVar
 
 from pip_services4_components.context import IContext
-from pip_services4_data.query.PagingParams import PagingParams
-from pip_services4_data.query.DataPage import DataPage
 
+from pip_services4_data.query.FilterParams import FilterParams
+from pip_services4_data.query.SortParams import SortParams
 
-class IFilteredPageReader(ABC):
+T = TypeVar('T')  # Declare type variable
+
+
+class IFilteredReader(ABC):
     """
-    Interface for data processing components that can retrieve a page of data items by a filter.
+    Interface for data processing components that can retrieve a list of data items by filter.
     """
 
-    def get_page_by_filter(self, context: Optional[IContext], filter: Optional[FilterParams],
-                           paging: Optional[PagingParams],
-                           sort: Optional[SortParams] = None) -> DataPage:
+    def get_list_by_filter(self, context: Optional[IContext], filter: Optional[FilterParams],
+                           sort: Optional[SortParams] = None) -> List[T]:
         """
-        Gets a page of data items using filter parameters.
+        Gets a list of data items using filter parameters.
 
         :param context: (optional) transaction id to trace execution through call chain.
 
         :param filter: (optional) filter parameters
 
-        :param paging: (optional) paging parameters
-
         :param sort: (optional) sort parameters
 
+        :param paging: (optional) paging parameters
+
         :return: list of items
         """
         raise NotImplementedError('Method from interface definition')
```

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/read/IFilteredReader.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/read/IFilteredPageReader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 # -*- coding: utf-8 -*-
 """
-    pip_services3_data.IFilteredReader
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+    pip_services3_data.IFilteredPageReader
+    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
     
-    Interface for filtered data readers.
+    Interface for filtered paging data readers.
     
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
 from abc import ABC
-from typing import List, Optional, TypeVar
+from typing import Optional
 
 from pip_services4_components.context import IContext
+from pip_services4_data.query import SortParams, FilterParams
+from pip_services4_data.query.PagingParams import PagingParams
+from pip_services4_data.query.DataPage import DataPage
 
-from pip_services4_data.query.FilterParams import FilterParams
-from pip_services4_data.query.SortParams import SortParams
 
-T = TypeVar('T')  # Declare type variable
-
-
-class IFilteredReader(ABC):
+class IFilteredPageReader(ABC):
     """
-    Interface for data processing components that can retrieve a list of data items by filter.
+    Interface for data processing components that can retrieve a page of data items by a filter.
     """
 
-    def get_list_by_filter(self, context: Optional[IContext], filter: Optional[FilterParams],
-                           sort: Optional[SortParams] = None) -> List[T]:
+    def get_page_by_filter(self, context: Optional[IContext], filter: Optional[FilterParams],
+                           paging: Optional[PagingParams],
+                           sort: Optional[SortParams] = None) -> DataPage:
         """
-        Gets a list of data items using filter parameters.
+        Gets a page of data items using filter parameters.
 
         :param context: (optional) transaction id to trace execution through call chain.
 
         :param filter: (optional) filter parameters
 
-        :param sort: (optional) sort parameters
-
         :param paging: (optional) paging parameters
 
+        :param sort: (optional) sort parameters
+
         :return: list of items
         """
         raise NotImplementedError('Method from interface definition')
```

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/read/IGetter.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/read/IGetter.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/read/ILoader.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/read/ILoader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/read/IQuerablePageReader.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/read/IQuerablePageReader.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
 from abc import ABC
 from typing import Optional
 
 from pip_services4_components.context import IContext
-from pip_services4_data.query.FilterParams import PagingParams
+from pip_services4_data.query.PagingParams import PagingParams
 from pip_services4_data.query.DataPage import DataPage
 from pip_services4_data.query.SortParams import SortParams
 
 
 class IQuerablePageReader(ABC):
     """
     Interface for data processing components that can query a page of data items.
```

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/read/IQuerableReader.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/read/IQuerableReader.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/read/__init__.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/read/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,23 +6,18 @@
     Contains interfaces for various design patterns that work with data.
     
     :copyright: Conceptual Vision Consulting LLC 2018-2019, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
 
 __all__ = [
-    'IPartialUpdater', 'IFilteredPageReader', 'IFilteredReader',
+    'IFilteredPageReader', 'IFilteredReader',
     'IGetter', 'ILoader', 'IQuerablePageReader', 'IQuerableReader',
-    'ISaver', 'ISetter', 'IWriter'
 ]
 
-from .IPartialUpdater import IPartialUpdater
 from .IFilteredPageReader import IFilteredPageReader
 from .IFilteredReader import IFilteredReader
 from .IGetter import IGetter
 from .ILoader import ILoader
 from .IQuerablePageReader import IQuerablePageReader
 from .IQuerableReader import IQuerableReader
-from .ISaver import ISaver
-from .ISetter import ISetter
-from .IWriter import IWriter
```

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/write/IPartialUpdater.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/write/IPartialUpdater.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/write/ISaver.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/write/ISaver.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/write/ISetter.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/write/ISetter.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence/write/IWriter.py` & `pip_services4_persistence-0.0.2/pip_services4_persistence/write/IWriter.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence.egg-info/PKG-INFO` & `pip_services4_persistence-0.0.2/pip_services4_persistence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-services4-persistence
-Version: 0.0.1
+Version: 0.0.2
 Summary: Data processing and persistence components for Pip.Services in Python
 Home-page: http://github.com/pip-services3-python/pip-services4-persistence-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_persistence-0.0.1/pip_services4_persistence.egg-info/SOURCES.txt` & `pip_services4_persistence-0.0.2/pip_services4_persistence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/setup.py` & `pip_services4_persistence-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 try:
     readme = open('readme.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_persistence',
-    version='0.0.1',
+    version='0.0.2',
     url='http://github.com/pip-services3-python/pip-services4-persistence-python',
     license='MIT',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     description='Data processing and persistence components for Pip.Services in Python',
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['config', 'data', 'test']),
     include_package_data=True,
     zip_safe=True,
     platforms='any',
     install_requires=[
         'pip_services4_commons >= 0.0.1, < 1.0',
         'pip_services4_components >= 0.0.1, < 1.0',
-        'pip_services4_data >= 0.0.2, < 1.0',
+        'pip_services4_data >= 0.0.3, < 1.0',
         'pip_services4_observability >= 0.0.1, < 1.0',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

### Comparing `pip_services4_persistence-0.0.1/test/persistence/DummyFilePersistence.py` & `pip_services4_persistence-0.0.2/test/persistence/DummyFilePersistence.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/test/persistence/DummyMemoryPersistence.py` & `pip_services4_persistence-0.0.2/test/persistence/DummyMemoryPersistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Dummy memory persistence implementation
     
     :copyright: Conceptual Vision Consulting LLC 2015-2016, see AUTHORS for more details.
     :license: MIT, see LICENSE for more details.
 """
 from pip_services4_persistence.persistence import IdentifiableMemoryPersistence
 from pip_services4_persistence.write.IPartialUpdater import IPartialUpdater
-from pip_services4_data.data.FilterParams import FilterParams
+from pip_services4_data.query.FilterParams import FilterParams
 
 
 class DummyMemoryPersistence(IdentifiableMemoryPersistence, IPartialUpdater):
 
     def __init__(self):
         super(DummyMemoryPersistence, self).__init__()
```

### Comparing `pip_services4_persistence-0.0.1/test/persistence/test_DummyFilePersistence.py` & `pip_services4_persistence-0.0.2/test/persistence/test_DummyFilePersistence.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/test/persistence/test_DummyMemoryPersistence.py` & `pip_services4_persistence-0.0.2/test/persistence/test_DummyMemoryPersistence.py`

 * *Files identical despite different names*

### Comparing `pip_services4_persistence-0.0.1/test/persistence/test_JsonFilePersister.py` & `pip_services4_persistence-0.0.2/test/persistence/test_JsonFilePersister.py`

 * *Files identical despite different names*

