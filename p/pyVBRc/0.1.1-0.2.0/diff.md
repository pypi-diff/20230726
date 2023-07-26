# Comparing `tmp/pyVBRc-0.1.1.tar.gz` & `tmp/pyVBRc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyVBRc-0.1.1.tar", last modified: Fri Oct 21 01:11:23 2022, max compression
+gzip compressed data, was "pyVBRc-0.2.0.tar", last modified: Wed Jul 26 20:11:39 2023, max compression
```

## Comparing `pyVBRc-0.1.1.tar` & `pyVBRc-0.2.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 01:11:23.478220 pyVBRc-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)      292 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 01:11:23.474220 pyVBRc-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 01:11:23.474220 pyVBRc-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.github/workflows/build-test.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.github/workflows/check-build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.github/workflows/check-manifest.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      557 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.github/workflows/create-release.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.github/workflows/pypi-release.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.github/workflows/style-check.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2361 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-21 01:11:23.478220 pyVBRc-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 01:11:23.474220 pyVBRc-0.1.1/pyVBRc/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/pyVBRc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 01:11:23.478220 pyVBRc-0.1.1/pyVBRc/sample_data/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/sample_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2960 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/sample_data/generate_sample_vbr_struct_file.m
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/sample_data/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 01:11:23.478220 pyVBRc-0.1.1/pyVBRc/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/tests/test_pyVBRc.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/vbr_units.py
--rw-r--r--   0 runner    (1001) docker     (121)     5219 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/pyVBRc/vbrc_structure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-21 01:11:23.478220 pyVBRc-0.1.1/pyVBRc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-10-21 01:11:23.000000 pyVBRc-0.1.1/pyVBRc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-10-21 01:11:23.000000 pyVBRc-0.1.1/pyVBRc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 01:11:23.000000 pyVBRc-0.1.1/pyVBRc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-21 01:11:23.000000 pyVBRc-0.1.1/pyVBRc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-21 01:11:23.000000 pyVBRc-0.1.1/pyVBRc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-21 01:11:23.000000 pyVBRc-0.1.1/pyVBRc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-21 01:11:23.000000 pyVBRc-0.1.1/pyVBRc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/release_history.md
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/release_notes.md
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/requirements_style.txt
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-10-21 01:11:23.478220 pyVBRc-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1483 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      419 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/sync_style_reqs.sh
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-10-21 01:11:13.000000 pyVBRc-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:39.562398 pyVBRc-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:39.554398 pyVBRc-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:39.558398 pyVBRc-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/.github/workflows/build-test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/.github/workflows/check-manifest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/.github/workflows/create-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/.github/workflows/pypi-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-26 20:11:39.562398 pyVBRc-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:39.558398 pyVBRc-0.2.0/pyVBRc/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:39.562398 pyVBRc-0.2.0/pyVBRc/anisotropy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/anisotropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/anisotropy/_stiffness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21549 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/anisotropy/materials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:39.562398 pyVBRc-0.2.0/pyVBRc/anisotropy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/anisotropy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/anisotropy/tests/test_anisotropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/pyVBRc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:39.562398 pyVBRc-0.2.0/pyVBRc/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   422992 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/sample_data/VBRc_sample_LUT.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   253894 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/sample_data/VBRc_sample_LUT_R2021a.mat
+-rw-r--r--   0 runner    (1001) docker     (123)   432816 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/sample_data/VBRc_sample_LUT_v1pt0pt0.mat
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/sample_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/sample_data/generate_sample_vbr_struct_file.m
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/sample_data/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:39.562398 pyVBRc-0.2.0/pyVBRc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/tests/test_pyVBRc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyVBRc/vbrc_structure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 20:11:39.562398 pyVBRc-0.2.0/pyVBRc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-26 20:11:39.000000 pyVBRc-0.2.0/pyVBRc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-26 20:11:39.000000 pyVBRc-0.2.0/pyVBRc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 20:11:39.000000 pyVBRc-0.2.0/pyVBRc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-26 20:11:39.000000 pyVBRc-0.2.0/pyVBRc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-26 20:11:39.000000 pyVBRc-0.2.0/pyVBRc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/release_history.md
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/release_notes.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 20:11:39.562398 pyVBRc-0.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      419 2023-07-26 20:11:22.000000 pyVBRc-0.2.0/sync_style_reqs.sh
```

### Comparing `pyVBRc-0.1.1/.github/workflows/check-build.yml` & `pyVBRc-0.2.0/.github/workflows/check-manifest.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-name: Check Build
-on: pull_request
+name: check MANIFEST.in
+on:
+  pull_request
 
 jobs:
-  twinecheck:
-    name: twinecheck
+  check-manifest:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python
+    - name: Checkout Source
+      uses: actions/checkout@v2
+    - name: Setup Python
       uses: actions/setup-python@v2
       with:
         python-version: 3.9
-    - name: Install dependencies
+    - name: install check-manifest
       run: |
         python -m pip install --upgrade pip
-        python -m pip install -U setuptools setuptools_scm wheel twine
-    - name: Build and check
+        python -m pip install check-manifest
+    - name: install build dependencies
       run: |
-        python setup.py sdist bdist_wheel
-        twine check dist/*
+        python -m pip install wheel
+    - name: Install pyVBRc
+      shell: bash
+      run: |
+        python -m pip install --no-build-isolation .
+    - name: Init submodules
+      uses: snickerbockers/submodules-init@v4
+    - name: run check-manifest
+      run: check-manifest -vvv
```

### Comparing `pyVBRc-0.1.1/.github/workflows/pypi-release.yaml` & `pyVBRc-0.2.0/.github/workflows/pypi-release.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,31 @@
+name: Publish distributions to PyPI
+
 on:
   push:
     # Sequence of patterns matched against refs/tags
     tags:
       - 'v*' # Push events to matching v*, i.e. v1.0, v20.15.10
 
-name: Publish distributions to PyPI
-
 jobs:
   build-and-publish:
     name: Build and Publish
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@master
+    - uses: actions/checkout@v3
     - name: Set up Python 3.9
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v3
       with:
         python-version: 3.9
     - name: Install dependencies
       run: |
           python -m pip install --upgrade pip
-          python -m pip install -U setuptools setuptools_scm wheel twine
+          python -m pip install -U build twine
     - name: Build and check source tarball
-      run: python setup.py sdist bdist_wheel
+      run: python -m build
     - name: Twine check
       run: twine check dist/*
     - name: Publish distribution to PyPI
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `pyVBRc-0.1.1/LICENSE` & `pyVBRc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyVBRc-0.1.1/Makefile` & `pyVBRc-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `pyVBRc-0.1.1/pyVBRc/sample_data/generate_sample_vbr_struct_file.m` & `pyVBRc-0.2.0/pyVBRc/sample_data/generate_sample_vbr_struct_file.m`

 * *Files identical despite different names*

### Comparing `pyVBRc-0.1.1/pyVBRc/tests/test_sample_data.py` & `pyVBRc-0.2.0/pyVBRc/tests/test_sample_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 
 import pytest
+from packaging.version import Version
 
 import pyVBRc.sample_data as sd
 
 _VBRfiles = [
     "VBRc_sample_LUT.mat",
     "VBRc_sample_LUT_R2021a.mat",
+    "VBRc_sample_LUT_v1pt0pt0.mat",
 ]
 
 
 @pytest.mark.parametrize("file", _VBRfiles)
 def test_load_sample_structure(file):
     vbr = sd.load_sample_structure(file)
     assert vbr.input.SV.T_K.ndim == 3
@@ -24,7 +26,17 @@
         assert vbr.input.SV.T_K.ndim == 3
 
 
 def test_get_sample_filename():
     for f in _VBRfiles:
         fullfi = sd.get_sample_filename(f)
         assert os.path.isfile(fullfi)
+
+
+def test_version():
+    vbr = sd.load_sample_structure("VBRc_sample_LUT_v1pt0pt0.mat")
+    assert vbr.vbrc_version == Version("1.0.0")
+
+
+def test_missing_version():
+    vbr = sd.load_sample_structure("VBRc_sample_LUT_R2021a.mat")
+    assert vbr.vbrc_version is None
```

