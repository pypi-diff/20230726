# Comparing `tmp/phlorest-1.1.0.tar.gz` & `tmp/phlorest-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phlorest-1.1.0.tar", last modified: Thu Jul 20 09:56:17 2023, max compression
+gzip compressed data, was "phlorest-1.2.0.tar", last modified: Wed Jul 26 09:25:27 2023, max compression
```

## Comparing `phlorest-1.1.0.tar` & `phlorest-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,51 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/
--rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-23 10:52:09.000000 phlorest-1.1.0/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)       50 2022-12-23 10:52:09.000000 phlorest-1.1.0/MANIFEST.in
--rw-rw-r--   0 robert    (1000) robert    (1000)     2907 2023-07-20 09:56:17.119885 phlorest-1.1.0/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     1934 2023-07-17 08:36:51.000000 phlorest-1.1.0/README.md
--rw-rw-r--   0 robert    (1000) robert    (1000)       81 2022-12-23 10:52:09.000000 phlorest-1.1.0/pyproject.toml
--rw-rw-r--   0 robert    (1000) robert    (1000)     2242 2023-07-20 09:56:17.119885 phlorest-1.1.0/setup.cfg
--rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2022-12-23 10:52:08.000000 phlorest-1.1.0/setup.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/
--rw-rw-r--   0 robert    (1000) robert    (1000)      293 2023-07-20 09:55:39.000000 phlorest-1.1.0/src/phlorest/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3945 2022-12-23 10:52:07.000000 phlorest-1.1.0/src/phlorest/__main__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3307 2023-07-12 10:55:15.000000 phlorest-1.1.0/src/phlorest/beast.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    11035 2023-07-20 06:21:20.000000 phlorest-1.1.0/src/phlorest/cldfwriter.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/commands/
--rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/commands/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2429 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/commands/check.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     1734 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/commands/merge_characters.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     8676 2023-07-18 11:31:01.000000 phlorest-1.1.0/src/phlorest/dataset.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2192 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/metadata.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3700 2023-07-17 11:04:32.000000 phlorest-1.1.0/src/phlorest/nexuslib.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/phlorest_template/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/phlorest_template/.github/
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/phlorest_template/.github/workflows/
--rw-rw-r--   0 robert    (1000) robert    (1000)      632 2023-07-18 13:29:33.000000 phlorest-1.1.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml
--rw-rw-r--   0 robert    (1000) robert    (1000)      796 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest/phlorest_template/etc/
--rw-rw-r--   0 robert    (1000) robert    (1000)       10 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/phlorest_template/etc/characters.csv
--rw-rw-r--   0 robert    (1000) robert    (1000)       16 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/phlorest_template/etc/taxa.csv
--rw-rw-r--   0 robert    (1000) robert    (1000)       89 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/phlorest_template/setup.cfg
--rw-rw-r--   0 robert    (1000) robert    (1000)      605 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/phlorest_template/setup.py_tmpl
--rw-rw-r--   0 robert    (1000) robert    (1000)      258 2022-12-23 10:52:08.000000 phlorest-1.1.0/src/phlorest/scaffold.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/src/phlorest.egg-info/
--rw-rw-r--   0 robert    (1000) robert    (1000)     2907 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     1078 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)      171 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/entry_points.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-12-23 10:52:07.000000 phlorest-1.1.0/src/phlorest.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)      245 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        9 2023-07-20 09:56:17.000000 phlorest-1.1.0/src/phlorest.egg-info/top_level.txt
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 09:56:17.119885 phlorest-1.1.0/tests/
--rw-rw-r--   0 robert    (1000) robert    (1000)      663 2023-07-12 10:55:15.000000 phlorest-1.1.0/tests/test_beast.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2730 2023-07-20 06:32:03.000000 phlorest-1.1.0/tests/test_cldfwriter.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      681 2022-12-23 10:52:07.000000 phlorest-1.1.0/tests/test_cli.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3552 2023-07-20 06:25:32.000000 phlorest-1.1.0/tests/test_dataset.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      409 2022-12-23 10:52:07.000000 phlorest-1.1.0/tests/test_metadata.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      917 2023-07-20 06:22:43.000000 phlorest-1.1.0/tests/test_nexuslib.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      261 2022-12-23 10:52:07.000000 phlorest-1.1.0/tests/test_scaffold.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-26 09:25:27.762507 phlorest-1.2.0/
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11357 2022-12-23 10:52:09.000000 phlorest-1.2.0/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)       50 2022-12-23 10:52:09.000000 phlorest-1.2.0/MANIFEST.in
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3080 2023-07-26 09:25:27.762507 phlorest-1.2.0/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2107 2023-07-26 08:50:37.000000 phlorest-1.2.0/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)       81 2022-12-23 10:52:09.000000 phlorest-1.2.0/pyproject.toml
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2242 2023-07-26 09:25:27.762507 phlorest-1.2.0/setup.cfg
+-rwxrwxr-x   0 robert    (1000) robert    (1000)       39 2022-12-23 10:52:08.000000 phlorest-1.2.0/setup.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-26 09:25:27.758507 phlorest-1.2.0/src/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-26 09:25:27.758507 phlorest-1.2.0/src/phlorest/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      293 2023-07-26 09:24:51.000000 phlorest-1.2.0/src/phlorest/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3945 2022-12-23 10:52:07.000000 phlorest-1.2.0/src/phlorest/__main__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3307 2023-07-12 10:55:15.000000 phlorest-1.2.0/src/phlorest/beast.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2687 2023-07-26 08:32:51.000000 phlorest-1.2.0/src/phlorest/check.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    11035 2023-07-20 06:21:20.000000 phlorest-1.2.0/src/phlorest/cldfwriter.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-26 09:25:27.758507 phlorest-1.2.0/src/phlorest/commands/
+-rw-rw-r--   0 robert    (1000) robert    (1000)        0 2022-12-23 10:52:08.000000 phlorest-1.2.0/src/phlorest/commands/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      627 2023-07-26 08:39:18.000000 phlorest-1.2.0/src/phlorest/commands/check.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1734 2022-12-23 10:52:08.000000 phlorest-1.2.0/src/phlorest/commands/merge_characters.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     9395 2023-07-25 13:13:03.000000 phlorest-1.2.0/src/phlorest/dataset.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2998 2023-07-26 05:33:25.000000 phlorest-1.2.0/src/phlorest/metadata.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3700 2023-07-17 11:04:32.000000 phlorest-1.2.0/src/phlorest/nexuslib.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-26 09:25:27.758507 phlorest-1.2.0/src/phlorest/phlorest_template/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-26 09:25:27.758507 phlorest-1.2.0/src/phlorest/phlorest_template/.github/
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-26 09:25:27.758507 phlorest-1.2.0/src/phlorest/phlorest_template/.github/workflows/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      632 2023-07-18 13:29:33.000000 phlorest-1.2.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml
+-rw-rw-r--   0 robert    (1000) robert    (1000)      796 2022-12-23 10:52:08.000000 phlorest-1.2.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-26 09:25:27.758507 phlorest-1.2.0/src/phlorest/phlorest_template/etc/
+-rw-rw-r--   0 robert    (1000) robert    (1000)       10 2022-12-23 10:52:08.000000 phlorest-1.2.0/src/phlorest/phlorest_template/etc/characters.csv
+-rw-rw-r--   0 robert    (1000) robert    (1000)       16 2022-12-23 10:52:08.000000 phlorest-1.2.0/src/phlorest/phlorest_template/etc/taxa.csv
+-rw-rw-r--   0 robert    (1000) robert    (1000)       89 2022-12-23 10:52:08.000000 phlorest-1.2.0/src/phlorest/phlorest_template/setup.cfg
+-rw-rw-r--   0 robert    (1000) robert    (1000)      605 2022-12-23 10:52:08.000000 phlorest-1.2.0/src/phlorest/phlorest_template/setup.py_tmpl
+-rw-rw-r--   0 robert    (1000) robert    (1000)      238 2023-07-26 08:32:51.000000 phlorest-1.2.0/src/phlorest/phlorest_template/test.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      258 2022-12-23 10:52:08.000000 phlorest-1.2.0/src/phlorest/scaffold.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-26 09:25:27.758507 phlorest-1.2.0/src/phlorest.egg-info/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3080 2023-07-26 09:25:27.000000 phlorest-1.2.0/src/phlorest.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1159 2023-07-26 09:25:27.000000 phlorest-1.2.0/src/phlorest.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-07-26 09:25:27.000000 phlorest-1.2.0/src/phlorest.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)      171 2023-07-26 09:25:27.000000 phlorest-1.2.0/src/phlorest.egg-info/entry_points.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-12-23 10:52:07.000000 phlorest-1.2.0/src/phlorest.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)      245 2023-07-26 09:25:27.000000 phlorest-1.2.0/src/phlorest.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        9 2023-07-26 09:25:27.000000 phlorest-1.2.0/src/phlorest.egg-info/top_level.txt
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-26 09:25:27.762507 phlorest-1.2.0/tests/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      663 2023-07-12 10:55:15.000000 phlorest-1.2.0/tests/test_beast.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      213 2023-07-26 08:50:01.000000 phlorest-1.2.0/tests/test_check.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2730 2023-07-20 06:32:03.000000 phlorest-1.2.0/tests/test_cldfwriter.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      681 2022-12-23 10:52:07.000000 phlorest-1.2.0/tests/test_cli.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3552 2023-07-20 06:25:32.000000 phlorest-1.2.0/tests/test_dataset.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      409 2022-12-23 10:52:07.000000 phlorest-1.2.0/tests/test_metadata.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      917 2023-07-20 06:22:43.000000 phlorest-1.2.0/tests/test_nexuslib.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      261 2022-12-23 10:52:07.000000 phlorest-1.2.0/tests/test_scaffold.py
```

### Comparing `phlorest-1.1.0/LICENSE` & `phlorest-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/PKG-INFO` & `phlorest-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phlorest
-Version: 1.1.0
+Version: 1.2.0
 Summary: A cldfbench plugin to curate language phylogenies
 Home-page: https://github.com/phlorest/phlorest
 Author: Simon Greenhill and Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/phlorest/phlorest/issues
 Keywords: cldf
@@ -95,11 +95,20 @@
 
 The resulting CLDF dataset can be validated running
 ```shell
 pytest
 ```
 
 
+### Release workflow
+
+```shell
+cldfbench makecldf --glottolog-version vX.Y --with-zenodo --with-cldfreadme cldfbench_<id>.py
+pytest
+cldfbench readme cldfbench_<id>.py
+```
+
+
 ## Dependencies
 
 The `run_treeannotator` method of `Dataset` requires the `treeannotator` command from BEAST to be
 installed. For details on how to install `treeannotator` (and `BEAST`), see https://beast.community/index.html
```

### Comparing `phlorest-1.1.0/README.md` & `phlorest-1.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -68,11 +68,20 @@
 
 The resulting CLDF dataset can be validated running
 ```shell
 pytest
 ```
 
 
+### Release workflow
+
+```shell
+cldfbench makecldf --glottolog-version vX.Y --with-zenodo --with-cldfreadme cldfbench_<id>.py
+pytest
+cldfbench readme cldfbench_<id>.py
+```
+
+
 ## Dependencies
 
 The `run_treeannotator` method of `Dataset` requires the `treeannotator` command from BEAST to be
 installed. For details on how to install `treeannotator` (and `BEAST`), see https://beast.community/index.html
```

### Comparing `phlorest-1.1.0/setup.cfg` & `phlorest-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phlorest
-version = 1.1.0
+version = 1.2.0
 author = Simon Greenhill and Robert Forkel
 author_email = dlce.rdm@eva.mpg.de
 description = A cldfbench plugin to curate language phylogenies
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = cldf
 license = Apache 2.0
```

### Comparing `phlorest-1.1.0/src/phlorest/__main__.py` & `phlorest-1.2.0/src/phlorest/__main__.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/src/phlorest/beast.py` & `phlorest-1.2.0/src/phlorest/beast.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/src/phlorest/cldfwriter.py` & `phlorest-1.2.0/src/phlorest/cldfwriter.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/src/phlorest/commands/check.py` & `phlorest-1.2.0/src/phlorest/check.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,76 +1,81 @@
-"""
-Checks datasets for compliance
-"""
-from cldfbench.cli_util import add_dataset_spec, get_dataset
+import typing
+
+from pycldf import Dataset as CLDFDataset
+
+import attr
+from cldfbench.dataset import dataset_from_module
+
+from phlorest import Dataset, Metadata
 
 # values in metadata.json that should be present and should not be empty
-METAKEYS = [
-    'id', 'title', 'license', 'citation', 'name', 'author',
-    'scaling', 'analysis', 'family'
-]
-# FIXME: maybe get these from phlorest.Metadata?
-
-
-def register(parser):  # pragma: no cover
-    add_dataset_spec(parser)
-
-
-def run(args, d=None):
-    if d is None:  # pragma: no cover
-        try:
-            d = get_dataset(args)
-        except Exception as e:
-            args.log.error("Unable to load %s - %s" % (args.dataset, e))
-            raise
+METAKEYS = [a.name for a in attr.fields(Metadata) if a.metadata.get('required')]
+
+
+def run_checks(d: typing.Union[CLDFDataset, Dataset], log) -> bool:
+    """
+    Run a couple of Phlorest-specific checks on a dataset.
+
+    To invoke from a dataset's `test.py` module, include
+
+    .. code-block:: python
+
+        def test_phlorest_check(cldf_dataset, cldf_logger):
+            from phlorest.check import run_checks
+            assert run_checks(cldf_dataset, cldf_logger)
+
+    :return: `True` if all checks passed, `False` otherwise.
+    """
+    if isinstance(d, CLDFDataset):
+        d = dataset_from_module(
+            d.directory.joinpath('..', 'cldfbench_{}.py'.format(d.properties['rdf:ID'])))
+
+    success = True
 
     def check(condition, msg):
         if condition:
-            args.log.warning('{0.id}: {1}'.format(d, msg))
+            log.warning('{0.id}: {1}'.format(d, msg))
+            return False
+        return True
 
     # check metadata
     for mdkey in METAKEYS:
-        check(
+        success &= check(
             not getattr(d.metadata, mdkey, ''),
             "metadata missing value for `%s`" % mdkey)
 
-    check(
+    success &= check(
         not (d.raw_dir / 'source.bib').exists(),
         "raw/source.bib file missing")
 
-    check(
-        not getattr(d.metadata, 'title', '').startswith("Phlorest phylogeny derived from"),
-        "title does not follow `Phlorest phylogeny derived from`")
-
-    check(
-        not (d.cldf_dir / 'summary.trees').exists() and not d.metadata.missing.get('summary'),
-        "summary tree file missing")
-
-    check(
-        not (d.cldf_dir / 'posterior.trees').exists() and not d.metadata.missing.get('posterior'),
-        "posterior tree file missing")
-
-    check(
-        not (d.cldf_dir / 'data.nex').exists() and not d.metadata.missing.get('nexus'),
-        "nexus data file missing")
-
-    check(
-        not d.characters and not d.metadata.missing.get('characters'),
-        "characters.csv file missing")
+    success &= check(
+        not (d.dir / 'CONTRIBUTORS.md').exists(),
+        "CONTRIBUTORS.md file missing")
+
+    success &= check(
+        not ((d.cldf_dir / 'summary.trees').exists() or d.metadata.missing.get('summary')),
+        "missing summary tree not declared")
+
+    success &= check(
+        not ((d.cldf_dir / 'posterior.trees.zip').exists() or d.metadata.missing.get('posterior')),
+        "missing posterior tree not declared")
+
+    success &= check(
+        not ((d.cldf_dir / 'data.nex').exists() or d.metadata.missing.get('nexus')),
+        "missing nexus data not declared")
+
+    success &= check(
+        not (d.characters or d.metadata.missing.get('characters')),
+        "missing characters.csv not declared")
 
-    check(
+    success &= check(
         any('concepticonReference' in char for char in d.characters),
         "characters.csv uses `concepticonReference` rather than `Concepticon_ID`")
 
     # check that characters are coded if possible
     if d.characters and not d.metadata.missing.get('concepticon'):
-        check(
+        success &= check(
             all(char.get('Concepticon_ID', "") == "" for char in d.characters),
             "characters.csv file missing concepticon coding")
 
-    check((d.dir / 'Makefile').exists(), "has a legacy Makefile")
-
-    # is the cldf valid?
-    if (d.dir / 'cldf' / 'Generic-metadata.json').exists():
-        d.cldf_reader().validate()
-    else:
-        check(True, 'CLDF dataset not generated')
+    success &= check((d.dir / 'Makefile').exists(), "has a legacy Makefile")
+    return success
```

### Comparing `phlorest-1.1.0/src/phlorest/commands/merge_characters.py` & `phlorest-1.2.0/src/phlorest/commands/merge_characters.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/src/phlorest/dataset.py` & `phlorest-1.2.0/src/phlorest/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,18 +177,30 @@
         args.writer.add_taxa(self.taxa, args.glottolog.api, args.log)
         if self.raw_dir.joinpath('source.bib').exists():
             args.writer.cldf.sources.add(
                 self.raw_dir.joinpath('source.bib').read_text(encoding='utf8'))
 
     def _cmd_readme(self, args):
         cldfbench.Dataset._cmd_readme(self, args)
+        text = self.dir.joinpath('README.md').read_text(encoding='utf8')
+        text = text.replace('Available online', 'Source available online')
+        pre, header, post = text.partition('## Description')
+        text = pre + header + '\n\n' + self.metadata.text_description + post
+
         if self.dir.joinpath('summary_tree.svg').exists():
-            text = self.dir.joinpath('README.md').read_text(encoding='utf8')
-            text += '\n\n## Summary Tree\n\n![summary](./summary_tree.svg)'
-            self.dir.joinpath('README.md').write_text(text, encoding='utf8')
+            text += '\n\n## Summary Tree\n\n!' \
+                    '[summary](https://raw.githubusercontent.com/phlorest/{}/' \
+                    'main/summary_tree.svg)'.format(self.id)
+        self.dir.joinpath('README.md').write_text(text, encoding='utf8')
+        print('gh repo edit --description "{}" --add-topic "phylogeny"'.format(self.metadata.title))
+        if self.metadata.family:
+            print('gh repo edit --add-topic "language-family-{}"'.format(
+                self.metadata.family.lower().replace(' ', '')))
+        if self.metadata.url:  # pragma: no cover
+            print('gh repo edit --homepage "{}"'.format(self.metadata.url))
 
     def _read_from_etc(self, name):
         if (self.etc_dir / name).exists():
             return list(self.etc_dir.read_csv(name, dicts=True))
         return []
 
     @property
```

### Comparing `phlorest-1.1.0/src/phlorest/metadata.py` & `phlorest-1.2.0/src/phlorest/metadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,20 +26,26 @@
     'centuries': 100,
     'millennia': 1000,
 }
 
 
 @attr.s
 class Metadata(cldfbench.Metadata):
-    name = attr.ib(default=None)
-    author = attr.ib(default=None)
+    name = attr.ib(default=None, metadata=dict(required=True))
+    author = attr.ib(default=None, metadata=dict(required=True))
     year = attr.ib(default=None)
-    scaling = attr.ib(default='none', validator=attr.validators.in_(SCALING))
-    analysis = attr.ib(default='none', validator=attr.validators.in_(ANALYSES))
-    family = attr.ib(default=None)
+    scaling = attr.ib(
+        default='none',
+        validator=attr.validators.in_(SCALING),
+        metadata=dict(required=True))
+    analysis = attr.ib(
+        default='none',
+        validator=attr.validators.in_(ANALYSES),
+        metadata=dict(required=True))
+    family = attr.ib(default=None, metadata=dict(required=True))
     cldf = attr.ib(
         default=None,
         converter=lambda s: 'https://{}'.format(s) if s and s.startswith('github.com') else s)
     data = attr.ib(default=None)
     missing = attr.ib(default=attr.Factory(dict))
 
     def __attrs_post_init__(self):
@@ -70,7 +76,21 @@
         if data:
             res['prov:wasDerivedFrom'] = [{
                 "rdf:about": data,
                 "rdf:type": "prov:Entity",
                 "dc:description": "Dataset underlying the analysis"
             }]
         return res
+
+    @property
+    def text_description(self):
+        res = 'A [Phlorest phylogeny](https://github.com/phlorest)'
+        if self.family:
+            if self.family == 'Multiple':  # pragma: no cover
+                res += ' of multiple language families'
+            else:
+                res += ' of the {} language family'.format(self.family)
+        if self.analysis and self.analysis != 'none':
+            res += ' computed from a {} analysis'.format(self.analysis)
+        if self.scaling and self.scaling != 'none':
+            res += ' scaled by {}'.format(self.scaling)
+        return res + '.'
```

### Comparing `phlorest-1.1.0/src/phlorest/nexuslib.py` & `phlorest-1.2.0/src/phlorest/nexuslib.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml` & `phlorest-1.2.0/src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl` & `phlorest-1.2.0/src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/src/phlorest/phlorest_template/setup.py_tmpl` & `phlorest-1.2.0/src/phlorest/phlorest_template/setup.py_tmpl`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/src/phlorest.egg-info/PKG-INFO` & `phlorest-1.2.0/src/phlorest.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phlorest
-Version: 1.1.0
+Version: 1.2.0
 Summary: A cldfbench plugin to curate language phylogenies
 Home-page: https://github.com/phlorest/phlorest
 Author: Simon Greenhill and Robert Forkel
 Author-email: dlce.rdm@eva.mpg.de
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/phlorest/phlorest/issues
 Keywords: cldf
@@ -95,11 +95,20 @@
 
 The resulting CLDF dataset can be validated running
 ```shell
 pytest
 ```
 
 
+### Release workflow
+
+```shell
+cldfbench makecldf --glottolog-version vX.Y --with-zenodo --with-cldfreadme cldfbench_<id>.py
+pytest
+cldfbench readme cldfbench_<id>.py
+```
+
+
 ## Dependencies
 
 The `run_treeannotator` method of `Dataset` requires the `treeannotator` command from BEAST to be
 installed. For details on how to install `treeannotator` (and `BEAST`), see https://beast.community/index.html
```

### Comparing `phlorest-1.1.0/src/phlorest.egg-info/SOURCES.txt` & `phlorest-1.2.0/src/phlorest.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/phlorest/__init__.py
 src/phlorest/__main__.py
 src/phlorest/beast.py
+src/phlorest/check.py
 src/phlorest/cldfwriter.py
 src/phlorest/dataset.py
 src/phlorest/metadata.py
 src/phlorest/nexuslib.py
 src/phlorest/scaffold.py
 src/phlorest.egg-info/PKG-INFO
 src/phlorest.egg-info/SOURCES.txt
@@ -21,17 +22,19 @@
 src/phlorest.egg-info/top_level.txt
 src/phlorest/commands/__init__.py
 src/phlorest/commands/check.py
 src/phlorest/commands/merge_characters.py
 src/phlorest/phlorest_template/cldfbench_+id+.py_tmpl
 src/phlorest/phlorest_template/setup.cfg
 src/phlorest/phlorest_template/setup.py_tmpl
+src/phlorest/phlorest_template/test.py
 src/phlorest/phlorest_template/.github/workflows/cldf-validation.yml
 src/phlorest/phlorest_template/etc/characters.csv
 src/phlorest/phlorest_template/etc/taxa.csv
 tests/test_beast.py
+tests/test_check.py
 tests/test_cldfwriter.py
 tests/test_cli.py
 tests/test_dataset.py
 tests/test_metadata.py
 tests/test_nexuslib.py
 tests/test_scaffold.py
```

### Comparing `phlorest-1.1.0/tests/test_beast.py` & `phlorest-1.2.0/tests/test_beast.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/tests/test_cldfwriter.py` & `phlorest-1.2.0/tests/test_cldfwriter.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/tests/test_cli.py` & `phlorest-1.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/tests/test_dataset.py` & `phlorest-1.2.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `phlorest-1.1.0/tests/test_nexuslib.py` & `phlorest-1.2.0/tests/test_nexuslib.py`

 * *Files identical despite different names*

