# Comparing `tmp/superpathlib-1.0.2.tar.gz` & `tmp/superpathlib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superpathlib-1.0.2.tar", last modified: Thu Jun 22 13:46:35 2023, max compression
+gzip compressed data, was "superpathlib-1.0.3.tar", last modified: Tue Jul 25 23:45:19 2023, max compression
```

## Comparing `superpathlib-1.0.2.tar` & `superpathlib-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-06-22 13:46:35.651064 superpathlib-1.0.2/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-06-22 09:35:22.000000 superpathlib-1.0.2/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-06-22 13:46:35.647064 superpathlib-1.0.2/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2630 2023-06-22 10:13:57.000000 superpathlib-1.0.2/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-06-22 13:46:35.647064 superpathlib-1.0.2/plib/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       23 2023-06-22 09:35:22.000000 superpathlib-1.0.2/plib/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)    15354 2023-06-22 13:45:28.000000 superpathlib-1.0.2/plib/plib.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1152 2023-06-22 09:35:22.000000 superpathlib-1.0.2/plib/tags.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      857 2023-06-22 13:42:15.000000 superpathlib-1.0.2/plib/utils.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      559 2023-06-22 10:17:00.000000 superpathlib-1.0.2/pyproject.toml
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-06-22 13:46:35.651064 superpathlib-1.0.2/setup.cfg
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-06-22 13:46:35.647064 superpathlib-1.0.2/superpathlib.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-06-22 13:46:35.000000 superpathlib-1.0.2/superpathlib.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      406 2023-06-22 13:46:35.000000 superpathlib-1.0.2/superpathlib.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-06-22 13:46:35.000000 superpathlib-1.0.2/superpathlib.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-06-22 13:46:35.000000 superpathlib-1.0.2/superpathlib.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        5 2023-06-22 13:46:35.000000 superpathlib-1.0.2/superpathlib.egg-info/top_level.txt
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-06-22 13:46:35.647064 superpathlib-1.0.2/tests/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     4483 2023-06-22 09:59:18.000000 superpathlib-1.0.2/tests/test_content.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1532 2023-06-22 09:35:22.000000 superpathlib-1.0.2/tests/test_functionality.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1271 2023-06-22 09:35:22.000000 superpathlib-1.0.2/tests/test_metadata.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:45:19.797528 superpathlib-1.0.3/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-07-25 22:35:03.000000 superpathlib-1.0.3/LICENSE
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-07-25 23:45:19.797528 superpathlib-1.0.3/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2630 2023-07-25 23:41:53.000000 superpathlib-1.0.3/README.md
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:45:19.797528 superpathlib-1.0.3/plib/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       23 2023-07-25 22:35:03.000000 superpathlib-1.0.3/plib/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)    15444 2023-07-25 23:42:51.000000 superpathlib-1.0.3/plib/plib.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1152 2023-07-25 22:35:03.000000 superpathlib-1.0.3/plib/tags.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      857 2023-07-25 22:35:03.000000 superpathlib-1.0.3/plib/utils.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      559 2023-07-25 23:40:58.000000 superpathlib-1.0.3/pyproject.toml
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-07-25 23:45:19.797528 superpathlib-1.0.3/setup.cfg
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:45:19.797528 superpathlib-1.0.3/superpathlib.egg-info/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2975 2023-07-25 23:45:19.000000 superpathlib-1.0.3/superpathlib.egg-info/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      373 2023-07-25 23:45:19.000000 superpathlib-1.0.3/superpathlib.egg-info/SOURCES.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-07-25 23:45:19.000000 superpathlib-1.0.3/superpathlib.egg-info/dependency_links.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       69 2023-07-25 23:45:19.000000 superpathlib-1.0.3/superpathlib.egg-info/requires.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        5 2023-07-25 23:45:19.000000 superpathlib-1.0.3/superpathlib.egg-info/top_level.txt
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-25 23:45:19.797528 superpathlib-1.0.3/tests/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1649 2023-07-25 23:32:35.000000 superpathlib-1.0.3/tests/test_content.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1678 2023-07-25 23:15:42.000000 superpathlib-1.0.3/tests/test_encrypted_content.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     2045 2023-07-25 23:43:38.000000 superpathlib-1.0.3/tests/test_functionality.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      937 2023-07-25 23:38:40.000000 superpathlib-1.0.3/tests/test_metadata.py
```

### Comparing `superpathlib-1.0.2/LICENSE` & `superpathlib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.2/PKG-INFO` & `superpathlib-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Extended Pathlib
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/superpathlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `superpathlib-1.0.2/README.md` & `superpathlib-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.2/plib/plib.py` & `superpathlib-1.0.3/plib/plib.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,18 +284,19 @@
             filetype = filetype.split("/")[0]
         return filetype
 
     """
     Additional functionality
     """
 
-    def copy_to(self, dest: Path, include_properties=True):
-        dest.byte_content = self.byte_content
-        if include_properties:
-            self.copy_properties_to(dest)
+    def copy_to(self, dest: Path, include_properties=True, only_if_newer=False):
+        if not only_if_newer or self.mtime > dest.mtime:
+            dest.byte_content = self.byte_content
+            if include_properties:
+                self.copy_properties_to(dest)
 
     def copy_properties_to(self, dest: Path):
         for path in dest.find():
             path.tag = self.tag
             path.mtime = self.mtime
 
     @cached_property
```

### Comparing `superpathlib-1.0.2/plib/tags.py` & `superpathlib-1.0.3/plib/tags.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.2/plib/utils.py` & `superpathlib-1.0.3/plib/utils.py`

 * *Files identical despite different names*

### Comparing `superpathlib-1.0.2/pyproject.toml` & `superpathlib-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "superpathlib"
-version = "1.0.2"
+version = "1.0.3"
 description = "Extended Pathlib"
 authors = [{name = "Quinten Roets", email = "qdr2104@columbia.edu"}]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = []
```

### Comparing `superpathlib-1.0.2/superpathlib.egg-info/PKG-INFO` & `superpathlib-1.0.3/superpathlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superpathlib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Extended Pathlib
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/superpathlib
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `superpathlib-1.0.2/tests/test_functionality.py` & `superpathlib-1.0.3/tests/test_functionality.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,70 @@
-import pytest
+from content import byte_content
+from utils import ignore_fixture_warning
 
 from plib import Path
 
 
-@pytest.fixture()
-def path():
-    with Path.tempfile() as path:
-        yield path
-    assert not path.exists()
-
-
-@pytest.fixture()
-def folder():
-    with Path.tempfile() as path:
-        path.unlink()
-        path.mkdir()
-        yield path
-        path.rmtree()
-        path.touch()
-
-
 def test_tempfile():
     with Path.tempfile() as path:
         assert path.exists()
     assert not path.exists()
 
 
-def test_deletion(path):
+def test_deletion(path: Path):
     path.unlink()
     assert not path.exists()
 
 
-def test_parent(path):
-    child_path = path / "child.txt"
+def test_parent(path: Path):
+    child_path = path / path.name
     assert child_path.parent == path
 
 
-def test_tar_unpack(folder):
+def test_tar_unpack(folder: Path):
     archive_assets = Path(__file__).parent / "assets" / "archives"
     archive_path = archive_assets / "test.tar.gz"
     archive_path.unpack(folder, remove_existing=True, remove_original=False)
     test_file = folder / "test.txt"
     assert test_file.text.strip() == "testcontent"
 
 
-def test_recursive_unpack(folder):
+def test_recursive_unpack(folder: Path):
     archive_assets = Path(__file__).parent / "assets" / "archives"
     archive_path = archive_assets / "recursive.zip"
     archive_path.unpack(folder, remove_existing=True, remove_original=False)
     test_file = folder / "test" / "test" / "test.txt"
     assert test_file.text.strip() == "testcontent"
 
 
-def test_unpack_check(folder):
+def test_unpack_check(folder: Path):
     non_archive_assets = Path(__file__).parent / "assets" / "non_archives"
     assert not non_archive_assets.is_empty()
     for path in non_archive_assets.iterdir():
         path.unpack_if_archive(folder)
         assert folder.is_empty()
+
+
+@ignore_fixture_warning
+@byte_content
+def test_copy(path: Path, path2: Path, content: bytes):
+    path.byte_content = content
+    path.copy_to(path2)
+    assert path2.byte_content == content
+
+
+@ignore_fixture_warning
+@byte_content
+def test_copy_if_newer_copies(path: Path, path2: Path, content: bytes):
+    path.byte_content = content
+    path.mtime = path2.mtime + 1
+    path.copy_to(path2, only_if_newer=True)
+    assert path2.byte_content == content
+
+
+@ignore_fixture_warning
+@byte_content
+def test_copy_if_newer_skips(path: Path, path2: Path, content: bytes):
+    path.byte_content = content
+    path.mtime = path2.mtime - 1
+    path.copy_to(path2, only_if_newer=True)
+    assert path2.byte_content == b""
```

