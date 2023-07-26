# Comparing `tmp/wattro_sync-0.3.0.tar.gz` & `tmp/wattro_sync-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wattro_sync-0.3.0.tar", last modified: Tue Jul 18 11:46:13 2023, max compression
+gzip compressed data, was "wattro_sync-0.3.1.tar", last modified: Wed Jul 26 08:11:22 2023, max compression
```

## Comparing `wattro_sync-0.3.0.tar` & `wattro_sync-0.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.466155 wattro_sync-0.3.0/
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1073 2022-11-11 16:56:53.000000 wattro_sync-0.3.0/LICENSE
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2570 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/PKG-INFO
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2255 2023-07-18 11:40:16.000000 wattro_sync-0.3.0/README.md
--rw-r--r--   0 bastian   (1000) bastian   (1000)       38 2023-07-18 11:46:13.466155 wattro_sync-0.3.0/setup.cfg
--rw-r--r--   0 bastian   (1000) bastian   (1000)      585 2023-07-18 11:45:36.000000 wattro_sync-0.3.0/setup.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.459488 wattro_sync-0.3.0/tests/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.3.0/tests/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     7419 2022-12-05 15:24:24.000000 wattro_sync-0.3.0/tests/test_hash_history.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.459488 wattro_sync-0.3.0/wattro_sync/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-11-11 16:39:16.000000 wattro_sync-0.3.0/wattro_sync/__init__.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/wattro_sync/api/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-10-28 14:22:35.000000 wattro_sync-0.3.0/wattro_sync/api/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      612 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/api/api_mapping.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1770 2022-12-05 15:24:24.000000 wattro_sync-0.3.0/wattro_sync/api/mail.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2601 2023-07-18 11:40:16.000000 wattro_sync-0.3.0/wattro_sync/api/mosaik_api.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1790 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/api/odbc_api.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     4283 2022-12-07 13:54:46.000000 wattro_sync-0.3.0/wattro_sync/api/rest_api.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2395 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/api/sqlite_api.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     3847 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/api/src_cli.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      573 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/api/topkontor_api.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/wattro_sync/config_reader/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-10-28 12:45:32.000000 wattro_sync-0.3.0/wattro_sync/config_reader/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     3247 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/config_reader/access.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      880 2022-12-05 15:24:36.000000 wattro_sync-0.3.0/wattro_sync/config_reader/types.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/wattro_sync/file_access/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.3.0/wattro_sync/file_access/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)      658 2022-12-05 15:24:36.000000 wattro_sync-0.3.0/wattro_sync/file_access/logging.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     3567 2022-12-12 12:52:21.000000 wattro_sync-0.3.0/wattro_sync/file_access/read_write.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/wattro_sync/hash_history/
--rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.3.0/wattro_sync/hash_history/__init__.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     1567 2022-12-05 15:24:36.000000 wattro_sync-0.3.0/wattro_sync/hash_history/history.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)     3187 2022-12-05 15:24:36.000000 wattro_sync-0.3.0/wattro_sync/helpers.py
--rwxr-xr-x   0 bastian   (1000) bastian   (1000)     9798 2022-12-12 12:54:13.000000 wattro_sync-0.3.0/wattro_sync/setup.py
--rw-r--r--   0 bastian   (1000) bastian   (1000)    10475 2022-12-08 12:37:33.000000 wattro_sync-0.3.0/wattro_sync/sync.py
-drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-18 11:46:13.462821 wattro_sync-0.3.0/wattro_sync.egg-info/
--rw-r--r--   0 bastian   (1000) bastian   (1000)     2570 2023-07-18 11:46:13.000000 wattro_sync-0.3.0/wattro_sync.egg-info/PKG-INFO
--rw-r--r--   0 bastian   (1000) bastian   (1000)      883 2023-07-18 11:46:13.000000 wattro_sync-0.3.0/wattro_sync.egg-info/SOURCES.txt
--rw-r--r--   0 bastian   (1000) bastian   (1000)        1 2023-07-18 11:46:13.000000 wattro_sync-0.3.0/wattro_sync.egg-info/dependency_links.txt
--rw-r--r--   0 bastian   (1000) bastian   (1000)       42 2023-07-18 11:46:13.000000 wattro_sync-0.3.0/wattro_sync.egg-info/requires.txt
--rw-r--r--   0 bastian   (1000) bastian   (1000)       18 2023-07-18 11:46:13.000000 wattro_sync-0.3.0/wattro_sync.egg-info/top_level.txt
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-26 08:11:22.894318 wattro_sync-0.3.1/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1073 2022-11-11 16:56:53.000000 wattro_sync-0.3.1/LICENSE
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2570 2023-07-26 08:11:22.894318 wattro_sync-0.3.1/PKG-INFO
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2255 2023-07-18 11:40:16.000000 wattro_sync-0.3.1/README.md
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       38 2023-07-26 08:11:22.894318 wattro_sync-0.3.1/setup.cfg
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      585 2023-07-26 08:09:20.000000 wattro_sync-0.3.1/setup.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-26 08:11:22.890984 wattro_sync-0.3.1/tests/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.3.1/tests/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     7419 2022-12-05 15:24:24.000000 wattro_sync-0.3.1/tests/test_hash_history.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-26 08:11:22.890984 wattro_sync-0.3.1/wattro_sync/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-11-11 16:39:16.000000 wattro_sync-0.3.1/wattro_sync/__init__.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-26 08:11:22.894318 wattro_sync-0.3.1/wattro_sync/api/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-10-28 14:22:35.000000 wattro_sync-0.3.1/wattro_sync/api/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      612 2022-12-08 12:37:33.000000 wattro_sync-0.3.1/wattro_sync/api/api_mapping.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1770 2022-12-05 15:24:24.000000 wattro_sync-0.3.1/wattro_sync/api/mail.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2601 2023-07-26 07:50:30.000000 wattro_sync-0.3.1/wattro_sync/api/mosaik_api.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2191 2023-07-26 08:08:25.000000 wattro_sync-0.3.1/wattro_sync/api/odbc_api.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     4283 2022-12-07 13:54:46.000000 wattro_sync-0.3.1/wattro_sync/api/rest_api.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2748 2023-07-26 08:08:25.000000 wattro_sync-0.3.1/wattro_sync/api/sqlite_api.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     3847 2022-12-08 12:37:33.000000 wattro_sync-0.3.1/wattro_sync/api/src_cli.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      573 2022-12-08 12:37:33.000000 wattro_sync-0.3.1/wattro_sync/api/topkontor_api.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-26 08:11:22.894318 wattro_sync-0.3.1/wattro_sync/config_reader/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-10-28 12:45:32.000000 wattro_sync-0.3.1/wattro_sync/config_reader/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     3247 2022-12-08 12:37:33.000000 wattro_sync-0.3.1/wattro_sync/config_reader/access.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      880 2022-12-05 15:24:36.000000 wattro_sync-0.3.1/wattro_sync/config_reader/types.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-26 08:11:22.894318 wattro_sync-0.3.1/wattro_sync/file_access/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.3.1/wattro_sync/file_access/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      658 2022-12-05 15:24:36.000000 wattro_sync-0.3.1/wattro_sync/file_access/logging.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     3567 2022-12-12 12:52:21.000000 wattro_sync-0.3.1/wattro_sync/file_access/read_write.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-26 08:11:22.894318 wattro_sync-0.3.1/wattro_sync/hash_history/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        0 2022-12-05 15:24:24.000000 wattro_sync-0.3.1/wattro_sync/hash_history/__init__.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     1567 2022-12-05 15:24:36.000000 wattro_sync-0.3.1/wattro_sync/hash_history/history.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     3187 2022-12-05 15:24:36.000000 wattro_sync-0.3.1/wattro_sync/helpers.py
+-rwxr-xr-x   0 bastian   (1000) bastian   (1000)     9798 2022-12-12 12:54:13.000000 wattro_sync-0.3.1/wattro_sync/setup.py
+-rw-r--r--   0 bastian   (1000) bastian   (1000)    10475 2022-12-08 12:37:33.000000 wattro_sync-0.3.1/wattro_sync/sync.py
+drwxr-xr-x   0 bastian   (1000) bastian   (1000)        0 2023-07-26 08:11:22.890984 wattro_sync-0.3.1/wattro_sync.egg-info/
+-rw-r--r--   0 bastian   (1000) bastian   (1000)     2570 2023-07-26 08:11:22.000000 wattro_sync-0.3.1/wattro_sync.egg-info/PKG-INFO
+-rw-r--r--   0 bastian   (1000) bastian   (1000)      883 2023-07-26 08:11:22.000000 wattro_sync-0.3.1/wattro_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 bastian   (1000) bastian   (1000)        1 2023-07-26 08:11:22.000000 wattro_sync-0.3.1/wattro_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       42 2023-07-26 08:11:22.000000 wattro_sync-0.3.1/wattro_sync.egg-info/requires.txt
+-rw-r--r--   0 bastian   (1000) bastian   (1000)       18 2023-07-26 08:11:22.000000 wattro_sync-0.3.1/wattro_sync.egg-info/top_level.txt
```

### Comparing `wattro_sync-0.3.0/LICENSE` & `wattro_sync-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/PKG-INFO` & `wattro_sync-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wattro_sync
-Version: 0.3.0
+Version: 0.3.1
 Summary: Script collection to sync data from local sources to a wattro node
 Home-page: https://github.com/wattro/wattro_sync
 Author: Wattro GmbH
 Author-email: admin@wattro.de
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wattro_sync-0.3.0/README.md` & `wattro_sync-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/setup.py` & `wattro_sync-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wattro_sync",
-    version="0.3.0",
+    version="0.3.1",
     description="Script collection to sync data from local sources to a wattro node",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wattro/wattro_sync",
     author="Wattro GmbH",
     author_email="admin@wattro.de",
     packages=setuptools.find_packages(),
```

### Comparing `wattro_sync-0.3.0/tests/test_hash_history.py` & `wattro_sync-0.3.1/tests/test_hash_history.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/api/api_mapping.py` & `wattro_sync-0.3.1/wattro_sync/api/api_mapping.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/api/mail.py` & `wattro_sync-0.3.1/wattro_sync/api/mail.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/api/mosaik_api.py` & `wattro_sync-0.3.1/wattro_sync/api/mosaik_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         fake_api = cls(
             MosaikSyncInfo(
                 odbc_connection_str=connection_info,
                 collection_info=CollectionInfo.empty(),
             )
         )
         db_res = fake_api._exec(
-            "SELECT name FROM SYSOBJECTS WHERE xtype='U' PO xtype='V';"
+            "SELECT name FROM SYSOBJECTS WHERE xtype='U' OR xtype='V';"
         )
         return sorted([x["name"] for x in db_res])
 
     @classmethod
     def get_fields(
         cls, connection_info: Any, collection: str
     ) -> tuple[list[str], dict[str, list]]:
```

### Comparing `wattro_sync-0.3.0/wattro_sync/api/odbc_api.py` & `wattro_sync-0.3.1/wattro_sync/api/odbc_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -28,27 +28,38 @@
             "collection_info": dataclasses.asdict(self.collection_info),
         }
 
 
 class OdbcSrcCli(SrcCli, ABC):
     def __init__(self, sync_info: OdbcSyncInfo):
         self.collection_info = sync_info.collection_info
-        self.obdc_connection_str = sync_info.odbc_connection_str
+        self.odbc_connection_str = sync_info.odbc_connection_str
 
     def _exec(self, qry: str, params=None) -> DBRes:
-        cnxn = pyodbc.connect(self.obdc_connection_str)
-        cursor = cnxn.cursor()
-        if params is None:
-            params = tuple()
-        rows = cursor.execute(qry, params).fetchall()
-        if not rows:
-            res = DBRes([], [])
-        else:
-            res = DBRes([n[0] for n in cursor.description], rows)
-        cnxn.close()
+        try:
+            cnxn = pyodbc.connect(self.odbc_connection_str)
+        except Exception as err:
+            raise ConnectionError(
+                f"Failed to connect using {self.odbc_connection_str!r}"
+            ) from err
+        try:
+            cursor = cnxn.cursor()
+            if params is None:
+                params = tuple()
+            rows = cursor.execute(qry, params).fetchall()
+            if not rows:
+                res = DBRes([], [])
+            else:
+                res = DBRes([n[0] for n in cursor.description], rows)
+        except Exception as err:
+            raise RuntimeError(
+                f"Failed to execute {qry = !r} with {params = !r}"
+            ) from err
+        finally:
+            cnxn.close()
         return res
 
 
 class OdbcSrcCliAltSample(OdbcSrcCli, ABC):
     def get_sample(self) -> DBRes:
         """For Sources that do not implement the LIMIT statement but the TOP statement."""
         qry = self._qry("").strip(";")
```

### Comparing `wattro_sync-0.3.0/wattro_sync/api/rest_api.py` & `wattro_sync-0.3.1/wattro_sync/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/api/sqlite_api.py` & `wattro_sync-0.3.1/wattro_sync/api/sqlite_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,18 +58,27 @@
                 db_path=connection_info, collection_info=CollectionInfo.empty()
             )
         )
         db_res = fake_api._exec(f"PRAGMA table_list")
         return sorted([x["name"] for x in db_res])
 
     def _exec(self, qry: str, params=None) -> DBRes:
-        cnxn = sqlite3.connect(self.db_path)
-        cursr = cnxn.cursor()
-        if params is None:
-            params = tuple()
-        rows = cursr.execute(qry, params).fetchall()
-        if not rows:
-            res = DBRes([], [])
-        else:
-            res = DBRes([n[0] for n in cursr.description], rows)
-        cnxn.close()
+        try:
+            cnxn = sqlite3.connect(self.db_path)
+        except Exception as err:
+            raise ConnectionError(f"Failed to open db at {self.db_path}") from err
+        try:
+            cursr = cnxn.cursor()
+            if params is None:
+                params = tuple()
+            rows = cursr.execute(qry, params).fetchall()
+            if not rows:
+                res = DBRes([], [])
+            else:
+                res = DBRes([n[0] for n in cursr.description], rows)
+        except Exception as err:
+            raise RuntimeError(
+                "Failed to execute {qry = !r} with {params = !r}"
+            ) from err
+        finally:
+            cnxn.close()
         return res
```

### Comparing `wattro_sync-0.3.0/wattro_sync/api/src_cli.py` & `wattro_sync-0.3.1/wattro_sync/api/src_cli.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/api/topkontor_api.py` & `wattro_sync-0.3.1/wattro_sync/api/topkontor_api.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/config_reader/access.py` & `wattro_sync-0.3.1/wattro_sync/config_reader/access.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/config_reader/types.py` & `wattro_sync-0.3.1/wattro_sync/config_reader/types.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/file_access/logging.py` & `wattro_sync-0.3.1/wattro_sync/file_access/logging.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/file_access/read_write.py` & `wattro_sync-0.3.1/wattro_sync/file_access/read_write.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/hash_history/history.py` & `wattro_sync-0.3.1/wattro_sync/hash_history/history.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/helpers.py` & `wattro_sync-0.3.1/wattro_sync/helpers.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/setup.py` & `wattro_sync-0.3.1/wattro_sync/setup.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync/sync.py` & `wattro_sync-0.3.1/wattro_sync/sync.py`

 * *Files identical despite different names*

### Comparing `wattro_sync-0.3.0/wattro_sync.egg-info/PKG-INFO` & `wattro_sync-0.3.1/wattro_sync.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wattro-sync
-Version: 0.3.0
+Version: 0.3.1
 Summary: Script collection to sync data from local sources to a wattro node
 Home-page: https://github.com/wattro/wattro_sync
 Author: Wattro GmbH
 Author-email: admin@wattro.de
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `wattro_sync-0.3.0/wattro_sync.egg-info/SOURCES.txt` & `wattro_sync-0.3.1/wattro_sync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

