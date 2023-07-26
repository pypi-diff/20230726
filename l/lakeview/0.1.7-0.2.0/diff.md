# Comparing `tmp/lakeview-0.1.7.tar.gz` & `tmp/lakeview-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakeview-0.1.7.tar", last modified: Fri Mar 17 08:59:43 2023, max compression
+gzip compressed data, was "lakeview-0.2.0.tar", last modified: Wed Jul 26 14:56:05 2023, max compression
```

## Comparing `lakeview-0.1.7.tar` & `lakeview-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:59:43.951935 lakeview-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:59:43.951935 lakeview-0.1.7/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-17 08:57:32.000000 lakeview-0.1.7/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-17 08:57:32.000000 lakeview-0.1.7/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-17 08:57:32.000000 lakeview-0.1.7/.devcontainer/noop.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-17 08:57:32.000000 lakeview-0.1.7/.devcontainer/post_create.sh
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-17 08:57:32.000000 lakeview-0.1.7/.devcontainer/post_start.sh
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-17 08:57:32.000000 lakeview-0.1.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:59:43.943935 lakeview-0.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:59:43.951935 lakeview-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-03-17 08:57:32.000000 lakeview-0.1.7/.github/workflows/deploy_docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-17 08:57:32.000000 lakeview-0.1.7/.github/workflows/lint_with_flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-17 08:57:32.000000 lakeview-0.1.7/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-17 08:57:32.000000 lakeview-0.1.7/.github/workflows/run_pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-17 08:57:32.000000 lakeview-0.1.7/.github/workflows/type_check_with_mypy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-17 08:57:32.000000 lakeview-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-17 08:57:32.000000 lakeview-0.1.7/.gitpod.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-17 08:57:32.000000 lakeview-0.1.7/.gitpod.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:59:43.951935 lakeview-0.1.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-17 08:57:32.000000 lakeview-0.1.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-17 08:57:32.000000 lakeview-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-17 08:57:32.000000 lakeview-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-03-17 08:59:43.951935 lakeview-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-03-17 08:57:32.000000 lakeview-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-17 08:57:32.000000 lakeview-0.1.7/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-03-17 08:57:32.000000 lakeview-0.1.7/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-17 08:57:32.000000 lakeview-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-17 08:57:32.000000 lakeview-0.1.7/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 08:59:43.951935 lakeview-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-17 08:57:32.000000 lakeview-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:59:43.947935 lakeview-0.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:59:43.951935 lakeview-0.1.7/src/lakeview/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/_type_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    69800 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8120 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/region_notation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     5516 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-03-17 08:57:32.000000 lakeview-0.1.7/src/lakeview/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 08:59:43.951935 lakeview-0.1.7/src/lakeview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-03-17 08:59:42.000000 lakeview-0.1.7/src/lakeview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-03-17 08:59:43.000000 lakeview-0.1.7/src/lakeview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 08:59:42.000000 lakeview-0.1.7/src/lakeview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-17 08:59:42.000000 lakeview-0.1.7/src/lakeview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-17 08:59:42.000000 lakeview-0.1.7/src/lakeview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:05.457986 lakeview-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:05.457986 lakeview-0.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-26 14:53:56.000000 lakeview-0.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-26 14:53:56.000000 lakeview-0.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-26 14:53:56.000000 lakeview-0.2.0/.devcontainer/noop.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-26 14:53:56.000000 lakeview-0.2.0/.devcontainer/post_create.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-26 14:53:56.000000 lakeview-0.2.0/.devcontainer/post_start.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-26 14:53:56.000000 lakeview-0.2.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:05.453986 lakeview-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:05.457986 lakeview-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-26 14:53:56.000000 lakeview-0.2.0/.github/workflows/deploy_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-26 14:53:56.000000 lakeview-0.2.0/.github/workflows/lint_with_flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-26 14:53:56.000000 lakeview-0.2.0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-26 14:53:56.000000 lakeview-0.2.0/.github/workflows/run_pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-26 14:53:56.000000 lakeview-0.2.0/.github/workflows/type_check_with_mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-26 14:53:56.000000 lakeview-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-26 14:53:56.000000 lakeview-0.2.0/.gitpod.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-26 14:53:56.000000 lakeview-0.2.0/.gitpod.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:05.457986 lakeview-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-26 14:53:56.000000 lakeview-0.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-26 14:53:56.000000 lakeview-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 14:53:56.000000 lakeview-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-26 14:56:05.457986 lakeview-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-07-26 14:53:56.000000 lakeview-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-26 14:53:56.000000 lakeview-0.2.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-26 14:53:56.000000 lakeview-0.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-26 14:53:56.000000 lakeview-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-26 14:53:56.000000 lakeview-0.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 14:56:05.457986 lakeview-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-26 14:53:56.000000 lakeview-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:05.453986 lakeview-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:05.457986 lakeview-0.2.0/src/lakeview/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/_type_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69711 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31303 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/region_notation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-26 14:53:56.000000 lakeview-0.2.0/src/lakeview/wiggle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:56:05.457986 lakeview-0.2.0/src/lakeview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-26 14:56:04.000000 lakeview-0.2.0/src/lakeview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-26 14:56:05.000000 lakeview-0.2.0/src/lakeview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:56:04.000000 lakeview-0.2.0/src/lakeview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-26 14:56:04.000000 lakeview-0.2.0/src/lakeview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-26 14:56:04.000000 lakeview-0.2.0/src/lakeview.egg-info/top_level.txt
```

### Comparing `lakeview-0.1.7/.devcontainer/Dockerfile` & `lakeview-0.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/.devcontainer/devcontainer.json` & `lakeview-0.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/.github/workflows/deploy_docs.yml` & `lakeview-0.2.0/.github/workflows/deploy_docs.yml`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/.github/workflows/lint_with_flake8.yml` & `lakeview-0.2.0/.github/workflows/lint_with_flake8.yml`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/.github/workflows/pypi_publish.yml` & `lakeview-0.2.0/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/.gitignore` & `lakeview-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/.gitpod.yml` & `lakeview-0.2.0/.gitpod.yml`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/LICENSE` & `lakeview-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/PKG-INFO` & `lakeview-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeview
-Version: 0.1.7
+Version: 0.2.0
 Summary: A Python library for creating publication-quality genome visualisations.
 Author-email: Jia-Yuan Zhang <jiayuan.zhang@ndm.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE
 Project-URL: Homepage, https://jzhang-dev.github.io/lakeview/
 Project-URL: Bug Tracker, https://github.com/jzhang-dev/lakeview/issues
 Keywords: bioinformatics,genomics,visualisation
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Lakeview logo](https://jzhang-dev.github.io/lakeview/_images/logo.svg)
 
 # Lakeview
 
+[![PyPI version](https://badge.fury.io/py/lakeview.svg)](https://badge.fury.io/py/lakeview)
 [![pytest](https://github.com/jzhang-dev/lakeview/actions/workflows/run_pytest.yml/badge.svg)](https://github.com/jzhang-dev/lakeview/actions/workflows/run_pytest.yml)
 [![mypy](https://github.com/jzhang-dev/lakeview/actions/workflows/type_check_with_mypy.yml/badge.svg)](https://github.com/jzhang-dev/lakeview/actions/workflows/type_check_with_mypy.yml)
 
 Lakeview is a Python 3 library for creating publication-quality [IGV](https://software.broadinstitute.org/software/igv/)-style genomic visualizations. Lakeview is based on [Matplotlib](https://matplotlib.org/). 
 
 A quick example:
```

### Comparing `lakeview-0.1.7/README.md` & `lakeview-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ![Lakeview logo](https://jzhang-dev.github.io/lakeview/_images/logo.svg)
 
 # Lakeview
 
+[![PyPI version](https://badge.fury.io/py/lakeview.svg)](https://badge.fury.io/py/lakeview)
 [![pytest](https://github.com/jzhang-dev/lakeview/actions/workflows/run_pytest.yml/badge.svg)](https://github.com/jzhang-dev/lakeview/actions/workflows/run_pytest.yml)
 [![mypy](https://github.com/jzhang-dev/lakeview/actions/workflows/type_check_with_mypy.yml/badge.svg)](https://github.com/jzhang-dev/lakeview/actions/workflows/type_check_with_mypy.yml)
 
 Lakeview is a Python 3 library for creating publication-quality [IGV](https://software.broadinstitute.org/software/igv/)-style genomic visualizations. Lakeview is based on [Matplotlib](https://matplotlib.org/). 
 
 A quick example:
```

### Comparing `lakeview-0.1.7/src/lakeview/_layout.py` & `lakeview-0.2.0/src/lakeview/_layout.py`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/src/lakeview/_type_alias.py` & `lakeview-0.2.0/src/lakeview/_type_alias.py`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/src/lakeview/alignment.py` & `lakeview-0.2.0/src/lakeview/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,14 +312,17 @@
 
         if self._cigartuples is not None:
             self._cigar: _CIGAR = _CIGAR.from_aligned_segment(self)
             "alignment patterns recorded in the CIGAR string"
         else:
             raise ValueError("CIGAR not found.")
 
+    def __getattr__(self, name: str):
+        return getattr(self.wrapped, name)
+
     def has_tag(self, tag: str) -> bool:
         "alias of :external:py:meth:`pysam.AlignedSegment.has_tag`"
         return self.wrapped.has_tag(tag)
 
     def get_tag(self, tag: str):
         "alias of :external:py:meth:`pysam.AlignedSegment.get_tag`"
         return self.wrapped.get_tag(tag)
@@ -573,29 +576,33 @@
         # Check `reference_name`
         reference_names: set[str] = set(alignment_file.references)
         if reference_name not in reference_names:
             raise ValueError(
                 f"Reference name {reference_name!r} is not found. Expecting one of {reference_names!r}"
             )
         # Load segments
+        fetch_kw: dict[str, Any] = dict(contig=reference_name)
+        if interval is not None:
+            fetch_kw['start'], fetch_kw['stop'] = interval
+
         segment_list: list[AlignedSegment] = [
             AlignedSegment(seg)
-            for seg in alignment_file.fetch(region=normalized_region)
-            if seg.is_mapped
+            for seg in alignment_file.fetch(**fetch_kw)
+            if seg.is_mapped # type: ignore # is_mapped is not included in pysam type stub
         ]
         if not segment_list:
             raise ValueError(f"No aligned segments found in {normalized_region!r}.")
         # Load pileup
         pileup_depths: dict[int, int] | None
         pileup_bases: dict[int, collections.Counter[str]] | None
         if load_pileup:
             pileup_depths = {}
             pileup_bases = {}
             pileup_column: pysam.PileupColumn
-            for pileup_column in alignment_file.pileup(region=normalized_region):
+            for pileup_column in alignment_file.pileup(region=normalized_region): # type: ignore # pileup is not correctly typed in pysam type stub
                 position: int = pileup_column.reference_pos
                 query_bases: list[str] = [
                     b.upper() for b in pileup_column.get_query_sequences() if b
                 ]
                 pileup_depths[position] = len(
                     query_bases
                 )  # col.nsegments includes reference skips; use len(query_bases) instead
@@ -870,30 +877,25 @@
             link_identifiers = [link_by(seg) for seg in segments]
         return link_identifiers
 
     def _get_group_identifiers(
         self,
         group_by: Callable[[AlignedSegment], GroupIdentifier]
         | Iterable[GroupIdentifier]
-        | Literal["haplotype", "name", "proper_pair", "strand"]
+        | Literal["name", "proper_pair", "strand"]
         | None,
     ) -> Sequence[GroupIdentifier]:
         segments = self.segments
         group_identifiers: Sequence[GroupIdentifier] = []
         if group_by is None:
             group_identifiers = [0] * len(
                 segments
             )  # Assign all segments into the same group
         if isinstance(group_by, str):
-            if group_by == "haplotype":
-                group_identifiers = [
-                    seg.get_tag("HP") if seg.has_tag("HP") else float("inf")
-                    for seg in segments
-                ]
-            elif group_by == "name":
+            if group_by == "name":
                 group_identifiers = [seg.query_name for seg in segments]
             elif group_by == "proper_pair":
                 group_identifiers = [seg.is_proper_pair for seg in segments]
             elif group_by == "strand":
                 group_identifiers = [
                     "forward" if seg.is_forward else "reverse" for seg in segments
                 ]
@@ -937,15 +939,15 @@
         | None = None,
         link_by: Callable[[AlignedSegment], LinkIdentifier]
         | Iterable[LinkIdentifier]
         | Literal["name", "pair"]
         | None = None,  # TODO: link by pair
         group_by: Callable[[AlignedSegment], GroupIdentifier]
         | Iterable[GroupIdentifier]
-        | Literal["haplotype", "name", "proper_pair", "strand"]
+        | Literal["name", "proper_pair", "strand"]
         | None = None,
         color_by: Callable[[AlignedSegment], Color]
         | Iterable[Color]
         | Literal["proper_pair", "strand"]
         | None = None,
         group_labels: Callable[[GroupIdentifier], str]
         | Mapping[GroupIdentifier, str]
@@ -1073,17 +1075,14 @@
         group_label_dict: dict[GroupIdentifier, str] = {}
         if group_labels is None:
             if group_by == "strand":
                 group_label_dict = {
                     "forward": "Forward strand",
                     "reverse": "Reverse strand",
                 }
-            elif group_by == "haplotype":
-                group_label_dict = {hp: f"Haplotype {hp}" for hp in group_identifiers}
-                group_label_dict[float("inf")] = "Haplotype unknown"
             else:
                 group_label_dict = {g: str(g) for g in unique_group_identifiers}
         elif callable(group_labels):
             group_label_dict = {g: group_labels(g) for g in unique_group_identifiers}
         elif isinstance(group_labels, Mapping):
             group_label_dict = {g: group_labels[g] for g in unique_group_identifiers}
 
@@ -1585,15 +1584,15 @@
     def _draw_links(
         self,
         ax: Axes,
         segments: Sequence[AlignedSegment],
         offsets: Sequence[float],
         link_identifiers: Sequence[LinkIdentifier],
         *,
-        linewidth: float = 1.5,
+        linewidth: float = 1,
         color: Color = "lightgray",
         linestyle: str = "-",
         **kw,
     ) -> None:
         link_ls_dict: dict[LinkIdentifier, _LinkedSegment] = self._link_segments(
             segments, link_identifiers
         )
```

### Comparing `lakeview-0.1.7/src/lakeview/annotation.py` & `lakeview-0.2.0/src/lakeview/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,17 +351,15 @@
             # parent_gene_key = "gene_id"
         elif format_ == "gff3":
             transcript_key = "ID"
             parent_transcript_key = "Parent"
             # gene_key = "ID"
             # parent_gene_key = "Parent"
         else:
-            raise ValueError(
-                f"Invalid value for `format_`: {format!r}."
-            )
+            raise ValueError(f"Invalid value for `format_`: {format!r}.")
 
         instance = cls.from_file(
             file=file,
             region=region,
             format_=format_,
             gene_features=[
                 "gene",
@@ -378,93 +376,103 @@
             parent_transcript_key=parent_transcript_key,
         )
         # Parse gene names
         for transcript in instance.transcripts:
             transcript.gene_name = transcript.attributes.get("gene")
         return instance
 
-    def _parse_runtime_parameters(  # TODO: delete?
+    def _parse_gene_parameters(
         self,
         *,
-        color_by,
-        label_by,
-    ):
+        color_by: Callable[[AnnotationRecord], Color] | Iterable[Color] | None,
+        label_by: Callable[[AnnotationRecord], str] | Iterable[str] | None,
+    ) -> tuple[Sequence[Color], Sequence[str]]:
         genes = self.genes
         # Colors
+        colors: Sequence[Color]
         if color_by is None:
             colors = ["b"] * len(genes)
+        elif callable(color_by):
+            colors = [color_by(g) for g in genes]
         elif isinstance(color_by, Iterable):
             colors = list(color_by)
-        elif isinstance(color_by, Callable):
-            colors = [color_by(g) for g in genes]
+        else:
+            raise ValueError()
+
         # Labels
-        if label_by == None:
+        labels: Sequence[str]
+        if label_by is None:
             labels = [""] * len(genes)
+        elif callable(label_by):
+            labels = [label_by(g) for g in genes]
         elif isinstance(label_by, Iterable):
             labels = list(label_by)
-        elif isinstance(label_by, Callable):
-            labels = [labels(g) for g in genes]
-        return labels, colors
+        else:
+            raise ValueError()
+        return colors, labels
 
-    def draw_genes(  # TODO: delete or update
+    def draw_genes(
         self,
         ax: Axes,
         *,
-        allow_overlaps=False,
-        group_by=None,  # TODO
-        group_labels=None,  # TODO
-        color_by: Union[
-            Callable[[AnnotationRecord], Color],  # TODO: define a color type
-            Iterable[Color],
-            None,
-        ] = None,
-        sort_by=None,  # TODO
-        label_by: Union[
-            Callable[[AnnotationRecord], str],
-            Iterable[str],
-            None,
-        ] = None,  # TODO: support label_by="name"
-        gene_height=None,
-        show_labels=True,
+        color_by: Callable[[AnnotationRecord], Color] | Iterable[Color] | None = None,
+        label_by: Callable[[AnnotationRecord], str] | Iterable[str] | None = None,
+        genes_kw={},
         labels_kw={},
     ):
         genes = self.genes
         intervals = [(g.start, g.end) for g in genes]
-        offsets: Sequence[int]
-        if allow_overlaps:
-            offsets = [0] * len(genes)
-        else:
-            offsets = pack_intervals(intervals)
-        colors, labels = self._parse_runtime_parameters(
+        offsets: Sequence[int] = pack_intervals(intervals)
+        colors, labels = self._parse_gene_parameters(
             color_by=color_by, label_by=label_by
         )
-        self._draw_gene_blocks(ax, genes, offsets, height=5, colors=colors)
-        if show_labels:
+        self._draw_gene_blocks(ax, genes, offsets, height=5, colors=colors, **genes_kw)
+        if not all(label == "" for label in labels):
             self._draw_labels(ax, genes, labels, offsets, colors=colors, **labels_kw)
-        ax.set_ylim(max(offsets) + 0.5, min(offsets) - 0.5)
+        ax.set_ylim(max(offsets) + 0.7, min(offsets) - 0.3)
         ax.set_ylabel("")
 
     def _draw_gene_blocks(self, ax, genes, offsets, height, *, colors, **kw):
         lines = [((g.start, y), (g.end, y)) for g, y in zip(genes, offsets)]
         ax.add_collection(
             LineCollection(
                 lines,
                 linewidths=height,
                 colors=colors[0] if len(set(colors)) == 1 else colors,
                 zorder=0,
                 facecolors="none",
             )
         )
 
-    def _draw_labels(self, ax, annotations, labels, offsets, *, colors, size=8, **kw):
+    def _draw_labels(
+        self,
+        ax,
+        annotations,
+        labels,
+        offsets,
+        *,
+        colors,
+        size=8,
+        horizontalalignment="center",
+        verticalalignment="bottom",
+        clip_on=True,
+        **kw,
+    ):
         for g, l, y, c in zip(annotations, labels, offsets, colors):
             if l:
                 x = (g.start + g.end) / 2
                 ax.text(
-                    x, y + 0.5, l, ha="center", va="bottom", size=size, clip_on=True
+                    x,
+                    y + 0.5,
+                    l,
+                    horizontalalignment=horizontalalignment,
+                    verticalalignment=verticalalignment,
+                    size=size,
+                    clip_on=clip_on,
+                    **kw,
                 )
 
     @staticmethod
     def _pack_transcripts(transcripts: Sequence[AnnotationRecord]) -> np.ndarray:
         intervals = [(t.start, t.end) for t in transcripts]
         return np.array(pack_intervals(intervals), dtype=np.float32)
 
@@ -559,14 +567,15 @@
             sort_keys = [sort_by(t) for t in transcripts]
         elif isinstance(sort_by, Iterable):
             sort_keys = list(sort_by)
 
         if filter_by is not None:
             transcripts = key_filter(transcripts, filter_keys)
             groups = key_filter(groups, filter_keys)
+            colors = key_filter(colors, filter_keys)
             labels = key_filter(labels, filter_keys)
             if sort_by is not None:
                 sort_keys = key_filter(sort_keys, filter_keys)
             if len(transcripts) == 0:
                 warn("All segments removed after filtering.")
 
         if sort_by is not None:
@@ -655,15 +664,15 @@
                 ax_height / (max(offsets) - min(offsets) + 2) * 0.5 * 72,
             )
 
         ax.set_xlim(
             min(t.start for t in transcripts),
             max(t.end for t in transcripts),
         )
-        ax.set_ylim(max(offsets) + 0.5, min(offsets) - 0.5)
+        ax.set_ylim(max(offsets) + 0.7, min(offsets) - 0.3)
         ax.set_yticks([])
 
         self._draw_transcript_backbones(
             ax, transcripts, offsets, colors=colors, **transcripts_kw
         )
         if draw_arrows:
             self._draw_arrows(
```

### Comparing `lakeview-0.1.7/src/lakeview/plot.py` & `lakeview-0.2.0/src/lakeview/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 def get_random_colors(n: int, *, seed=0, cmap="hsv") -> list[Color]:
     """
     Returns ``n`` random colors selected uniformly from ``cmap``.
 
     >>> get_random_colors(3)
     [(0.0, 0.22463448382566054, 1.0, 1.0), (0.4018366371307548, 1.0, 0.0, 1.0), (1.0, 0.2316178786767022, 0.0, 1.0)]
     """
-    rng = np.random.default_rng(seed=0)
-    cmap = plt.get_cmap("hsv")
-    colors = [cmap(rng.random()) for __ in range(n)]
+    rng = np.random.default_rng(seed=seed)
+    _cmap = plt.get_cmap(cmap)
+    colors = [_cmap(rng.random()) for __ in range(n)]
     return colors
 
 
 def draw_rigid_polygon(
     ax: Axes,
     shape: Sequence[Point],
     position: Point,
```

### Comparing `lakeview-0.1.7/src/lakeview/region_notation.py` & `lakeview-0.2.0/src/lakeview/region_notation.py`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/src/lakeview/remote.py` & `lakeview-0.2.0/src/lakeview/remote.py`

 * *Files identical despite different names*

### Comparing `lakeview-0.1.7/src/lakeview/sequence.py` & `lakeview-0.2.0/src/lakeview/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,14 @@
             if sample_fraction == 1 or rng.random() <= sample_fraction:
                 canonical_kmer = canonicalize(kmer)
                 kmer_indices[canonical_kmer].append(index)
         return kmer_indices
 
     # TODO: max_dots
     def draw_dots(
-        self, ax, *, x_offset=0, y_offset=0, s=0.5, max_dots=1e6, edgecolor="none"
+        self, ax, *, x_offset=0, y_offset=0, s=0.5, max_dots=1e6, color=None, edgecolor="none"
     ):
         xs = np.array([dot.x for dot in self.dots]) + x_offset
         ys = np.array([dot.y for dot in self.dots]) + y_offset
-        ax.scatter(xs, ys, s=s, edgecolor=edgecolor)
+        ax.scatter(xs, ys, s=s, color=color, edgecolor=edgecolor)
         ax.set_xlim(x_offset, x_offset + self.x_sequence_size - 1)
         ax.set_ylim(y_offset, y_offset + self.y_sequence_size - 1)
```

### Comparing `lakeview-0.1.7/src/lakeview/widget.py` & `lakeview-0.2.0/src/lakeview/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,24 +83,24 @@
 
     def _zoom(self, scale: float, /) -> None:
         for ax in self.figure.axes:
             old_xlim = ax.get_xlim()
             center = sum(old_xlim) / 2
             radius = (old_xlim[1] - old_xlim[0]) / 2
             new_radius = radius * scale
-            new_xlim = (center - new_radius, center + new_radius)
+            new_xlim = (max(0, center - new_radius), center + new_radius)
             ax.set_xlim(new_xlim)
         self._update_display()
 
     def _shift(self, distance: float, /) -> None:
         for ax in self.figure.axes:
             old_xlim = ax.get_xlim()
             radius = (old_xlim[1] - old_xlim[0]) / 2
             new_xlim = (
-                old_xlim[0] + distance * radius,
+                max(0, old_xlim[0] + distance * radius),
                 old_xlim[1] + distance * radius,
             )
             ax.set_xlim(new_xlim)
         self._update_display()
 
     def _goto(self, start: float, end: float) -> None:
         self.set_xlim(start, end)
@@ -115,15 +115,15 @@
 
     def _reset_xlim(self) -> None:
         self.set_xlim(self._initial_xlim)
         self._update_display()
 
     def _update_region_text(self) -> None:
         start, end = self.get_xlim()
-        self._region_text.value = f"{int(start):,} - {int(end):,}"
+        self._region_text.value = f"{int(start):,}-{int(end):,}"
 
     def _update_display(self):
         self._update_region_text()
         self._center_widget.clear_output(wait=True)
         with self._center_widget:
             display(self.figure)
```

### Comparing `lakeview-0.1.7/src/lakeview.egg-info/PKG-INFO` & `lakeview-0.2.0/src/lakeview.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakeview
-Version: 0.1.7
+Version: 0.2.0
 Summary: A Python library for creating publication-quality genome visualisations.
 Author-email: Jia-Yuan Zhang <jiayuan.zhang@ndm.ox.ac.uk>
 License: GNU GENERAL PUBLIC LICENSE
 Project-URL: Homepage, https://jzhang-dev.github.io/lakeview/
 Project-URL: Bug Tracker, https://github.com/jzhang-dev/lakeview/issues
 Keywords: bioinformatics,genomics,visualisation
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![Lakeview logo](https://jzhang-dev.github.io/lakeview/_images/logo.svg)
 
 # Lakeview
 
+[![PyPI version](https://badge.fury.io/py/lakeview.svg)](https://badge.fury.io/py/lakeview)
 [![pytest](https://github.com/jzhang-dev/lakeview/actions/workflows/run_pytest.yml/badge.svg)](https://github.com/jzhang-dev/lakeview/actions/workflows/run_pytest.yml)
 [![mypy](https://github.com/jzhang-dev/lakeview/actions/workflows/type_check_with_mypy.yml/badge.svg)](https://github.com/jzhang-dev/lakeview/actions/workflows/type_check_with_mypy.yml)
 
 Lakeview is a Python 3 library for creating publication-quality [IGV](https://software.broadinstitute.org/software/igv/)-style genomic visualizations. Lakeview is based on [Matplotlib](https://matplotlib.org/). 
 
 A quick example:
```

### Comparing `lakeview-0.1.7/src/lakeview.egg-info/SOURCES.txt` & `lakeview-0.2.0/src/lakeview.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,12 +28,13 @@
 src/lakeview/annotation.py
 src/lakeview/plot.py
 src/lakeview/py.typed
 src/lakeview/region_notation.py
 src/lakeview/remote.py
 src/lakeview/sequence.py
 src/lakeview/widget.py
+src/lakeview/wiggle.py
 src/lakeview.egg-info/PKG-INFO
 src/lakeview.egg-info/SOURCES.txt
 src/lakeview.egg-info/dependency_links.txt
 src/lakeview.egg-info/requires.txt
 src/lakeview.egg-info/top_level.txt
```

