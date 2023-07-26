# Comparing `tmp/napari_deeplabcut-0.1.2.tar.gz` & `tmp/napari_deeplabcut-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_deeplabcut-0.1.2.tar", last modified: Fri Apr 21 12:13:50 2023, max compression
+gzip compressed data, was "napari_deeplabcut-0.2.0.tar", last modified: Wed Jul 26 14:53:43 2023, max compression
```

## Comparing `napari_deeplabcut-0.1.2.tar` & `napari_deeplabcut-0.2.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.359644 napari_deeplabcut-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.363644 napari_deeplabcut-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/.github/workflows/plugin_preview.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.363644 napari_deeplabcut-0.1.2/.napari/
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.363644 napari_deeplabcut-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.363644 napari_deeplabcut-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.363644 napari_deeplabcut-0.1.2/src/napari_deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    31059 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/src/napari_deeplabcut/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/assets/lock.svg
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/assets/unlock.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:13:50.367644 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-21 12:13:50.000000 napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-21 12:13:24.000000 napari_deeplabcut-0.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:43.451537 napari_deeplabcut-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:43.443537 napari_deeplabcut-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:43.447537 napari_deeplabcut-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/.github/workflows/plugin_preview.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:43.447537 napari_deeplabcut-0.2.0/.napari/
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-07-26 14:53:43.451537 napari_deeplabcut-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:43.447537 napari_deeplabcut-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-26 14:53:43.455537 napari_deeplabcut-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:43.443537 napari_deeplabcut-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:43.447537 napari_deeplabcut-0.2.0/src/napari_deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:43.451537 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/test_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-26 14:53:43.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38977 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:43.451537 napari_deeplabcut-0.2.0/src/napari_deeplabcut/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/assets/lock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/assets/unlock.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 14:53:43.451537 napari_deeplabcut-0.2.0/src/napari_deeplabcut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-07-26 14:53:43.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-26 14:53:43.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 14:53:43.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-26 14:53:43.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-26 14:53:43.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 14:53:43.000000 napari_deeplabcut-0.2.0/src/napari_deeplabcut.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-26 14:53:19.000000 napari_deeplabcut-0.2.0/tox.ini
```

### Comparing `napari_deeplabcut-0.1.2/.github/workflows/plugin_preview.yml` & `napari_deeplabcut-0.2.0/.github/workflows/plugin_preview.yml`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.2/.github/workflows/test_and_deploy.yml` & `napari_deeplabcut-0.2.0/.github/workflows/test_and_deploy.yml`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools tox tox-gh-actions
 
       # this runs the platform-specific tests declared in tox.ini
       - name: Test with tox
-        uses: GabrielBB/xvfb-action@v1
+        uses: aganders3/headless-gui@v1
         with:
           run: python -m tox
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
         uses: codecov/codecov-action@v2
```

### Comparing `napari_deeplabcut-0.1.2/.gitignore` & `napari_deeplabcut-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.2/.napari/DESCRIPTION.md` & `napari_deeplabcut-0.2.0/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.2/.pre-commit-config.yaml` & `napari_deeplabcut-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.2/CODE_OF_CONDUCT.md` & `napari_deeplabcut-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.2/LICENSE` & `napari_deeplabcut-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.2/PKG-INFO` & `napari_deeplabcut-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,7 @@
-Metadata-Version: 2.1
-Name: napari_deeplabcut
-Version: 0.1.2
-Summary: napari + DeepLabCut annotation tool
-Home-page: https://github.com/DeepLabCut/napari-deeplabcut
-Author: Jessy Lauer
-Author-email: jessy.lauer@epfl.ch
-License: BSD-3-Clause
-Project-URL: Bug Tracker, https://github.com/DeepLabCut/napari-deeplabcut/issues
-Project-URL: Documentation, https://github.com/DeepLabCut/napari-deeplabcut#README.md
-Project-URL: Source Code, https://github.com/DeepLabCut/napari-deeplabcut
-Project-URL: User Support, https://github.com/DeepLabCut/napari-deeplabcut/issues
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: napari
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: testing
-License-File: LICENSE
-
 # napari-deeplabcut
 
 
 <img src="https://images.squarespace-cdn.com/content/v1/57f6d51c9f74566f55ecf271/1d409ffe-c9f4-47e1-bde2-3010c1c40455/naparidlc.png?format=750w" width="250" title="napari-deeplabcut" alt="napari+deeplabcut" align="right" vspace = "80">
 
 [![License: BSD-3](https://img.shields.io/badge/License-BSD3-blue.svg)](https://www.gnu.org/licenses/bsd3)
 [![PyPI](https://img.shields.io/pypi/v/napari-deeplabcut.svg?color=green)](https://pypi.org/project/napari-deeplabcut)
@@ -75,26 +45,28 @@
 
 - `2` and `3`, to easily switch between labeling and selection mode
 - `4`, to enable pan & zoom (which is achieved using the mouse wheel or finger scrolling on the Trackpad)
 - `M`, to cycle through regular (sequential), quick, and cycle annotation mode (see the description [here](https://github.com/DeepLabCut/napari-deeplabcut/blob/5a5709dd38868341568d66eab548ae8abf37cd63/src/napari_deeplabcut/keypoints.py#L25-L34))
 - `E`, to enable edge coloring (by default, if using this in refinement GUI mode, points with a confidence lower than 0.6 are marked
 in red)
 - `F`, to toggle between animal and body part color scheme.
+- `V`, to toggle visibility of the selected layer.
 - `backspace` to delete a point.
 - Check the box "display text" to show the label names on the canvas.
 - To move to another folder, be sure to save (Ctrl+S), then delete the layers, and re-drag/drop the next folder.
 
 
 ### Save Layers
 
 Annotations and segmentations are saved with `File > Save Selected Layer(s)...` (or its shortcut `Ctrl+S`).
 Only when saving segmentation masks does a save file dialog pop up to name the destination folder;
 keypoint annotations are otherwise automatically saved in the corresponding folder as `CollectedData_<ScorerName>.h5`.
 - As a reminder, DLC will only use the H5 file; so be sure if you open already labeled images you save/overwrite the H5.
 - Note, before saving a layer, make sure the points layer is selected. If the user clicked on the image(s) layer first, does `Save As`, then closes the window, any labeling work during that session will be lost!
+- Modifying and then saving points in a `machinelabels...` layer will add to or overwrite the existing `CollectedData` layer and will **not** save to the `machinelabels` file.
 
 
 ### Video frame extraction and prediction refinement
 
 Since v0.0.4, videos can be viewed in the GUI.
 
 Since v0.0.5, trailing points can be visualized; e.g., helping in the identification
@@ -129,24 +101,63 @@
     Open *napari* and open an image folder (which needs to contain a `CollectedData_<ScorerName>.h5` file).
     In this case, it is not necessary to open the DLC project's `config.yaml` file, as all necessary metadata is read from the `h5` data file.
 
     Saving works as described in *1*.
 
     ***Note that if a new body part has been added to the `config.yaml` file after having started to label, loading the config in the GUI is necessary to update the dropdown menus and other metadata.***
 
+    ***As `viridis` is `napari-deeplabcut` default colormap, loading the config in the GUI is also needed to update the color scheme.***
+
 3. **Refining labels** – the image folder contains a `machinelabels-iter<#>.h5` file.
 
     The process is analog to *2*.
+    Open *napari* and open an image folder.
+    If the video was originally labeled, *and* had outliers extracted it will contain a `CollectedData_<ScorerName>.h5` file and a `machinelabels-iter<#>.h5` file. In this case, select the `machinelabels` layer in the GUI, and type `e` to show edges. Red indicates likelihood < 0.6. As you navigate through frames, images with labels with edges will need to be refined (moved, deleted, etc). Images with labels without edges will be on the `CollectedData` (previous manual annotations) layer and shouldn't need refining. However, you can switch to that layer and fix errors. You can also right-click on the `CollectedData` layer and select `toggle visibility` to hide that layer. Select the `machinelabels` layer before saving which will append your refined annotations to `CollectedData`.
+
+    If the folder only had outliers extracted and wasn't originally labeled, it will not have a `CollectedData` layer. Work with the `machinelabels` layer selected to refine annotation positions, then save.
+
+    In this case, it is not necessary to open the DLC project's `config.yaml` file, as all necessary metadata is read from the `h5` data file.
+
+    Saving works as described in *1*.
 
 4. **Drawing segmentation masks**
 
     Drop an image folder as in *1*, manually add a *shapes layer*. Then select the *rectangle* in the layer controls (top left pane),
     and start drawing rectangles over the images. Masks and rectangle vertices are saved as described in [Save Layers](#save-layers).
     Note that masks can be reloaded and edited at a later stage by dropping the `vertices.csv` file onto the canvas.
 
+### Workflow flowchart
+
+```mermaid
+%%{init: {"flowchart": {"htmlLabels": false}} }%%
+graph TD
+  id1[What stage of labeling?]
+  id2[deeplabcut.label_frames]
+  id3[deeplabcut.refine_labels]
+  id4[Add labels to, or modify in, \n `CollectedData...` layer and save that layer]
+  id5[Modify labels in `machinelabels` layer and save \n which will create a `CollectedData...` file]
+  id6[Have you refined some labels from the most recent iteration and saved already?]
+  id7["All extracted frames are already saved in `CollectedData...`.
+1. Hide or trash all `machinelabels` layers.
+2. Then modify in and save `CollectedData`"]
+  id8["
+1. hide or trash all `machinelabels` layers except for the most recent.
+2. Select most recent `machinelabels` and hit `e` to show edges.
+3. Modify only in `machinelabels` and skip frames with labels without edges shown.
+4. Save `machinelabels` layer, which will add data to `CollectedData`.
+	- If you need to revisit this video later, ignore `machinelabels` and work only in `CollectedData`"]
+
+  id1 -->|I need to manually label new frames \n or fix my labels|id2
+  id1 ---->|I need to refine outlier frames \nfrom analyzed videos|id3
+  id2 -->id4
+  id3 -->|I only have a `machinelabels...` file|id5
+  id3 ---->|I have both `machinelabels` and `CollectedData` files|id6
+  id6 -->|yes|id7
+  id6 ---->|no, I just extracted outliers|id8
+```
 
 ### Labeling multiple image folders
 
 Labeling multiple image folders has to be done in sequence; i.e., only one image folder can be opened at a time.
 After labeling the images of a particular folder is done and the associated *Points layer* has been saved, *all* layers should be removed from the layers list (lower left pane on the GUI) by selecting them and clicking on the trashcan icon.
 Now, another image folder can be labeled, following the process described in *1*, *2*, or *3*, depending on the particular image folder.
```

### Comparing `napari_deeplabcut-0.1.2/setup.cfg` & `napari_deeplabcut-0.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 	Source Code = https://github.com/DeepLabCut/napari-deeplabcut
 	User Support = https://github.com/DeepLabCut/napari-deeplabcut/issues
 
 [options]
 packages = find:
 install_requires = 
 	dask-image
-	napari==0.4.17
+	napari==0.4.18
 	natsort
 	numpy
 	opencv-python-headless
 	pandas
 	pyyaml
 	qtpy
 	scikit-image
```

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_reader.py` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut/_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,14 +95,19 @@
     params = {
         "name": "images",
         "metadata": {
             "paths": natsorted(filepaths),
             "root": os.path.split(path)[0],
         },
     }
+
+    # https://github.com/soft-matter/pims/issues/452
+    if len(filepaths) == 1:
+        path = glob.glob(path)[0]
+
     return [(imread(path), params, "image")]
 
 
 def _populate_metadata(
     header: misc.DLCHeader,
     *,
     labels: Optional[Sequence[str]] = None,
@@ -121,25 +126,26 @@
         likelihood = np.ones(len(labels))
     label_colors = misc.build_color_cycle(len(header.bodyparts), colormap)
     id_colors = misc.build_color_cycle(len(header.individuals), colormap)
     face_color_cycle_maps = {
         "label": dict(zip(header.bodyparts, label_colors)),
         "id": dict(zip(header.individuals, id_colors)),
     }
+    face_color_prop = "id" if ids[0] else "label"
     return {
         "name": "keypoints",
         "text": "{id}–{label}" if ids[0] else "label",
         "properties": {
             "label": list(labels),
             "id": list(ids),
             "likelihood": likelihood,
             "valid": likelihood > pcutoff,
         },
-        "face_color_cycle": label_colors,
-        "face_color": "id" if ids[0] else "label",
+        "face_color_cycle": face_color_cycle_maps[face_color_prop],
+        "face_color": face_color_prop,
         "face_colormap": colormap,
         "edge_color": "valid",
         "edge_color_cycle": ["black", "red"],
         "edge_width": 0,
         "edge_width_is_relative": False,
         "size": size,
         "metadata": {
@@ -172,14 +178,15 @@
     return [(None, metadata, "points")]
 
 
 def read_hdf(filename: str) -> List[LayerData]:
     layers = []
     for filename in glob.iglob(filename):
         temp = pd.read_hdf(filename)
+        temp = misc.merge_multiple_scorers(temp)
         header = misc.DLCHeader(temp.columns)
         temp = temp.droplevel("scorer", axis=1)
         if "individuals" not in temp.columns.names:
             # Append a fake level to the MultiIndex
             # to make it look like a multi-animal DataFrame
             old_idx = temp.columns.to_frame()
             old_idx.insert(0, "individuals", "")
```

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/conftest.py` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import cv2
 import numpy as np
+import os
+
+os.environ["hide_tutorial"] = "True"
 import pandas as pd
 import pytest
 from napari_deeplabcut import keypoints, _writer
 from skimage.io import imsave
 
 
-@pytest.fixture  # TODO Hack to make this fixture session-scoped
+@pytest.fixture
 def viewer(make_napari_viewer):
     viewer = make_napari_viewer()
     for action in viewer.window.plugins_menu.actions():
         if "deeplabcut" in action.text():
             action.trigger()
             break
     return viewer
@@ -18,20 +21,23 @@
 
 @pytest.fixture
 def fake_keypoints():
     n_rows = 10
     n_animals = 2
     n_kpts = 3
     data = np.random.rand(n_rows, n_animals * n_kpts * 2)
-    cols = pd.MultiIndex.from_product([
-        ["me"],
-        [f"animal_{i}" for i in range(n_animals)],
-        [f"kpt_{i}" for i in range(n_kpts)],
-        ["x", "y"]
-    ], names=["scorer", "individuals", "bodyparts", "coords"])
+    cols = pd.MultiIndex.from_product(
+        [
+            ["me"],
+            [f"animal_{i}" for i in range(n_animals)],
+            [f"kpt_{i}" for i in range(n_kpts)],
+            ["x", "y"],
+        ],
+        names=["scorer", "individuals", "bodyparts", "coords"],
+    )
     df = pd.DataFrame(data, columns=cols, index=range(n_rows))
     return df
 
 
 @pytest.fixture
 def points(tmp_path_factory, viewer, fake_keypoints):
     output_path = str(tmp_path_factory.mktemp("folder") / "fake_data.h5")
@@ -64,30 +70,31 @@
         "scorer": "me",
         "bodyparts": list("abc"),
         "dotsize": 0,
         "pcutoff": 0,
         "colormap": "viridis",
         "video_sets": {
             "fake_video": [],
-        }
+        },
     }
     path = str(tmp_path_factory.mktemp("configs") / "config.yaml")
     _writer._write_config(
-        path, params=cfg,
+        path,
+        params=cfg,
     )
     return path
 
 
 @pytest.fixture(scope="session")
 def video_path(tmp_path_factory):
     output_path = str(tmp_path_factory.mktemp("data") / "fake_video.avi")
     h = w = 50
     writer = cv2.VideoWriter(
         output_path,
-        cv2.VideoWriter_fourcc(*'MJPG'),
+        cv2.VideoWriter_fourcc(*"MJPG"),
         2,
         (w, h),
     )
     for _ in range(5):
         frame = np.random.randint(0, 255, (h, w, 3)).astype(np.uint8)
         writer.write(frame)
     writer.release()
```

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_keypoints.py` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/test_keypoints.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,68 +1,75 @@
 import numpy as np
 from napari_deeplabcut import keypoints
 
 
-def test_store(store, fake_keypoints):
+def test_store_advance_step(store):
     assert store.current_step == 0
     store._advance_step(event=None)
     assert store.current_step == 1
 
+
+def test_store_labels(store, fake_keypoints):
     assert store.n_steps == fake_keypoints.shape[0]
     assert store.labels == list(
         fake_keypoints.columns.get_level_values("bodyparts").unique()
     )
 
+
+def test_store_find_first_unlabeled_frame(store, fake_keypoints):
+    store._find_first_unlabeled_frame(event=None)
+    assert store.current_step == store.n_steps - 1
+    # Remove a frame to test whether it is correctly found
+    ind_to_remove = 2
+    data = store.layer.data
+    store.layer.data = data[data[:, 0] != ind_to_remove]
+    store._find_first_unlabeled_frame(event=None)
+    assert store.current_step == ind_to_remove
+
+
+def test_store_keypoints(store, fake_keypoints):
     annotated_keypoints = store.annotated_keypoints
     assert len(annotated_keypoints) == fake_keypoints.shape[1] // 2
     assert annotated_keypoints[0].id == "animal_0"
     assert annotated_keypoints[-1].id == "animal_1"
     kpt = keypoints.Keypoint(label="kpt_0", id="animal_0")
     next_kpt = keypoints.Keypoint(label="kpt_1", id="animal_0")
     store.current_keypoint = kpt
     assert store.current_keypoint == kpt
     store.next_keypoint()
     assert store.current_keypoint == next_kpt
     store.prev_keypoint()
     assert store.current_keypoint == kpt
     store.next_keypoint()
 
-    store._find_first_unlabeled_frame(event=None)
-    assert store.current_step == store.n_steps - 1
-    # Remove a frame to test whether it is correctly found
-    ind_to_remove = 2
-    data = store.layer.data
-    store.layer.data = data[data[:, 0] != ind_to_remove]
-    store._find_first_unlabeled_frame(event=None)
-    assert store.current_step == ind_to_remove
-
 
 def test_point_resize(viewer, points):
     viewer.layers.selection.add(points)
     layer = viewer.layers[0]
     controls = keypoints.QtPointsControls(layer)
     new_size = 10
     controls.changeSize(new_size)
     np.testing.assert_array_equal(points.size, new_size)
 
 
 def test_add_unnanotated(store):
-    store.layer.metadata["controls"].label_mode = 'loop'
+    store.layer.metadata["controls"].label_mode = "loop"
     ind_to_remove = 0
     data = store.layer.data
     store.layer.data = data[data[:, 0] != ind_to_remove]
     store.viewer.dims.set_current_step(0, ind_to_remove)
     assert not store.annotated_keypoints
     n_points = store.layer.data.shape[0]
     keypoints._add(store, coord=(0, 1, 1))
     assert store.layer.data.shape[0] == n_points + 1
     assert store.current_step == ind_to_remove + 1
 
 
 def test_add_quick(store):
-    store.layer.metadata["controls"].label_mode = 'quick'
+    store.layer.metadata["controls"].label_mode = "quick"
     store.current_keypoint = store._keypoints[0]
     coord = store.current_step, -1, -1
     keypoints._add(store, coord=coord)
     np.testing.assert_array_equal(
-        store.layer.data[store.current_step], coord,
+        store.layer.data[store.current_step],
+        coord,
     )
```

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_reader.py` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/test_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,34 +60,35 @@
     assert dict_["name"].startswith("CollectedData_")
     assert config_path.startswith(dict_["metadata"]["project"])
 
 
 def test_read_hdf_old_index(tmp_path_factory, fake_keypoints):
     path = str(tmp_path_factory.mktemp("folder") / "data.h5")
     old_index = [
-        f"labeled-data/video/img{i}.png"
-        for i in range(fake_keypoints.shape[0])
+        f"labeled-data/video/img{i}.png" for i in range(fake_keypoints.shape[0])
     ]
     fake_keypoints.index = old_index
     fake_keypoints.to_hdf(path, key="data")
     layers = _reader.read_hdf(path)
     assert len(layers) == 1
     image_paths = layers[0][1]["metadata"]["paths"]
     assert len(image_paths) == len(fake_keypoints)
     assert isinstance(image_paths[0], str)
     assert "labeled-data" in image_paths[0]
 
 
 def test_read_hdf_new_index(tmp_path_factory, fake_keypoints):
     path = str(tmp_path_factory.mktemp("folder") / "data.h5")
-    new_index = pd.MultiIndex.from_product([
-        ["labeled-data"],
-        ["video"],
-        [f"img{i}.png" for i in range(fake_keypoints.shape[0])]
-    ])
+    new_index = pd.MultiIndex.from_product(
+        [
+            ["labeled-data"],
+            ["video"],
+            [f"img{i}.png" for i in range(fake_keypoints.shape[0])],
+        ]
+    )
     fake_keypoints.index = new_index
     fake_keypoints.to_hdf(path, key="data")
     layers = _reader.read_hdf(path)
     assert len(layers) == 1
     image_paths = layers[0][1]["metadata"]["paths"]
     assert len(image_paths) == len(fake_keypoints)
     assert isinstance(image_paths[0], str)
```

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_tests/test_widgets.py` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut/_tests/test_widgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import os
 from napari_deeplabcut import _widgets
 from vispy import keys
 
 
 def test_guess_continuous():
-    assert _widgets.guess_continuous(np.array([0.]))
+    assert _widgets.guess_continuous(np.array([0.0]))
     assert not _widgets.guess_continuous(np.array(list("abc")))
 
 
 def test_keypoint_controls(viewer):
     controls = _widgets.KeypointControls(viewer)
     controls.label_mode = "loop"
     assert controls._radio_group.checkedButton().text() == "loop"
@@ -36,40 +36,40 @@
     controls._extract_single_frame()
 
 
 def test_store_crop_coordinates(viewer, images, config_path):
     viewer.layers.selection.add(images)
     _ = viewer.add_shapes(
         np.random.random((4, 3)),
-        shape_type='rectangle',
+        shape_type="rectangle",
     )
     controls = _widgets.KeypointControls(viewer)
     controls._images_meta = {
         "name": "fake_video",
         "project": os.path.dirname(config_path),
     }
     controls._store_crop_coordinates()
 
 
 def test_toggle_face_color(viewer, points):
     viewer.layers.selection.add(points)
     view = viewer.window._qt_viewer
     # By default, points are colored by individual with multi-animal data
     assert points._face.color_properties.name == "id"
-    view.canvas.events.key_press(key=keys.Key('F'))
+    view.canvas.events.key_press(key=keys.Key("F"))
     assert points._face.color_properties.name == "label"
-    view.canvas.events.key_press(key=keys.Key('F'))
+    view.canvas.events.key_press(key=keys.Key("F"))
     assert points._face.color_properties.name == "id"
 
 
 def test_toggle_edge_color(viewer, points):
     viewer.layers.selection.add(points)
     view = viewer.window._qt_viewer
     np.testing.assert_array_equal(points.edge_width, 0)
-    view.canvas.events.key_press(key=keys.Key('E'))
+    view.canvas.events.key_press(key=keys.Key("E"))
     np.testing.assert_array_equal(points.edge_width, 2)
 
 
 def test_dropdown_menu(qtbot):
     widget = _widgets.DropdownMenu(list("abc"))
     widget.update_to("c")
     assert widget.currentText() == "c"
@@ -78,25 +78,25 @@
     qtbot.add_widget(widget)
 
 
 def test_keypoints_dropdown_menu(store):
     widget = _widgets.KeypointsDropdownMenu(store)
     assert "id" in widget.menus
     assert "label" in widget.menus
-    label_menu = widget.menus['label']
+    label_menu = widget.menus["label"]
     label_menu.currentText() == "kpt_0"
     widget.update_menus(event=None)
     label_menu.currentText() == "kpt_2"
     widget.refresh_label_menu("id_0")
     assert label_menu.count() == 0
 
 
 def test_keypoints_dropdown_menu_smart_reset(store):
     widget = _widgets.KeypointsDropdownMenu(store)
-    label_menu = widget.menus['label']
+    label_menu = widget.menus["label"]
     label_menu.update_to("kpt_2")
     widget._locked = True
     widget.smart_reset(event=None)
     assert label_menu.currentText() == "kpt_2"
     widget._locked = False
     widget.smart_reset(event=None)
     assert label_menu.currentText() == "kpt_0"
@@ -115,8 +115,8 @@
     widget = _widgets.ColorSchemeDisplay(None)
     widget._build()
     assert not widget.scheme_dict
     assert not widget._container.layout().count()
     widget.add_entry("keypoint", "red")
     assert widget.scheme_dict["keypoint"] == "red"
     assert widget._container.layout().count() == 1
-    qtbot.add_widget(widget)
+    qtbot.add_widget(widget)
```

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_widgets.py` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut/_widgets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import os
-from collections import defaultdict
+from collections import defaultdict, namedtuple
+from copy import deepcopy
 from datetime import datetime
-from functools import partial
+from functools import partial, cached_property
 from math import ceil, log10
 import pandas as pd
 from pathlib import Path
 from types import MethodType
 from typing import Optional, Sequence, Union
 
 import numpy as np
 from napari._qt.widgets.qt_welcome import QtWelcomeLabel
 from napari.layers import Image, Points, Shapes, Tracks
 from napari.layers.points._points_key_bindings import register_points_action
 from napari.layers.utils import color_manager
+from napari.layers.utils.layer_utils import _features_to_properties
 from napari.utils.events import Event
 from napari.utils.history import get_save_history, update_save_history
-from qtpy.QtCore import Qt, QTimer, Signal, QSize
-from qtpy.QtGui import QPainter, QIcon
+from qtpy.QtCore import Qt, QTimer, Signal, QSize, QPoint, QSettings
+from qtpy.QtGui import QPainter, QIcon, QAction
 from qtpy.QtWidgets import (
     QButtonGroup,
     QCheckBox,
     QComboBox,
+    QDialog,
+    QDialogButtonBox,
     QFileDialog,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QMessageBox,
     QPushButton,
     QRadioButton,
@@ -44,14 +48,97 @@
 from napari_deeplabcut.misc import (
     encode_categories,
     to_os_dir_sep,
     guarantee_multiindex_rows,
 )
 
 
+Tip = namedtuple("Tip", ["msg", "pos"])
+
+
+class Tutorial(QDialog):
+    def __init__(self, parent):
+        super().__init__(parent=parent)
+        self.setParent(parent)
+        self.setWindowTitle("Tutorial")
+        self.setModal(True)
+        self.setStyleSheet("background:#cdb4db")
+        self.setAttribute(Qt.WA_DeleteOnClose)
+        self.setWindowOpacity(0.95)
+        self.setWindowFlags(self.windowFlags() | Qt.FramelessWindowHint)
+
+        self._current_tip = 0
+        self._tips = [
+            Tip(
+                "Load a folder of annotated data\n(and optionally a config file if labeling from scratch)\nfrom the menu File > Open File or Open Folder.\nAlternatively, files and folders of images can be dragged\nand dropped onto the main window.",
+                (0.35, 0.15),
+            ),
+            Tip(
+                "Data layers will be listed at the bottom left;\ntheir visibility can be toggled by clicking on the small eye icon.",
+                (0.1, 0.65),
+            ),
+            Tip(
+                "Corresponding layer controls can be found at the top left.\nSwitch between labeling and selection mode using the numeric keys 2 and 3,\nor clicking on the + or -> icons.",
+                (0.1, 0.2),
+            ),
+            Tip(
+                "There are three keypoint labeling modes:\nthe key M can be used to cycle between them.",
+                (0.65, 0.05),
+            ),
+            Tip(
+                "When done labeling, save your data by selecting the Points layer\nand hitting Ctrl+S (or File > Save Selected Layer(s)...).",
+                (0.1, 0.65),
+            ),
+            Tip(
+                "Read more at <a href='https://github.com/DeepLabCut/napari-deeplabcut#usage'>napari-deeplabcut</a>",
+                (0.4, 0.4),
+            ),
+        ]
+
+        buttons = (
+            QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Abort
+        )
+        self.button_box = QDialogButtonBox(buttons)
+        self.button_box.accepted.connect(self.accept)
+        self.button_box.rejected.connect(self.reject)
+
+        vlayout = QVBoxLayout()
+        self.message = QLabel("💡\n\nLet's get started with a quick walkthrough!")
+        self.message.setTextInteractionFlags(Qt.LinksAccessibleByMouse)
+        self.message.setOpenExternalLinks(True)
+        vlayout.addWidget(self.message)
+        hlayout = QHBoxLayout()
+        self.count = QLabel("")
+        hlayout.addWidget(self.count)
+        hlayout.addWidget(self.button_box)
+        vlayout.addLayout(hlayout)
+        self.setLayout(vlayout)
+
+    def accept(self):
+        if self._current_tip == 0 and "walkthrough" not in self.message.text():
+            self.reject()
+        tip = self._tips[self._current_tip]
+        msg = tip.msg
+        if (
+            self._current_tip < 5
+        ):  # No emoji in the last tip otherwise the hyperlink breaks
+            msg = "💡\n\n" + msg
+        self.message.setText(msg)
+        self.count.setText(f"Tip {self._current_tip + 1}|{len(self._tips)}")
+        self.adjustSize()
+        xrel, yrel = tip.pos
+        geom = self.parent().geometry()
+        p = QPoint(
+            int(geom.left() + geom.width() * xrel),
+            int(geom.top() + geom.height() * yrel),
+        )
+        self.move(p)
+        self._current_tip = (self._current_tip + 1) % len(self._tips)
+
+
 def _get_and_try_preferred_reader(
     self,
     dialog,
     *args,
 ):
     try:
         self.viewer.open(
@@ -74,31 +161,99 @@
     else:
         return False
 
 
 color_manager.guess_continuous = guess_continuous
 
 
+def _paste_data(self, store):
+    """Paste only currently unannotated data."""
+    features = self._clipboard.pop("features", None)
+    if features is None:
+        return
+
+    unannotated = [
+        keypoints.Keypoint(label, id_) not in store.annotated_keypoints
+        for label, id_ in zip(features["label"], features["id"])
+    ]
+    if not any(unannotated):
+        return
+
+    new_features = features.iloc[unannotated]
+    indices_ = self._clipboard.pop("indices")
+    text_ = self._clipboard.pop("text")
+    self._clipboard = {k: v[unannotated] for k, v in self._clipboard.items()}
+    self._clipboard["features"] = new_features
+    self._clipboard["indices"] = indices_
+    if text_ is not None:
+        new_text = {
+            "string": text_["string"][unannotated],
+            "color": text_["color"],
+        }
+        self._clipboard["text"] = new_text
+
+    npoints = len(self._view_data)
+    totpoints = len(self.data)
+
+    if len(self._clipboard.keys()) > 0:
+        not_disp = self._slice_input.not_displayed
+        data = deepcopy(self._clipboard["data"])
+        offset = [
+            self._slice_indices[i] - self._clipboard["indices"][i] for i in not_disp
+        ]
+        data[:, not_disp] = data[:, not_disp] + np.array(offset)
+        self._data = np.append(self.data, data, axis=0)
+        self._shown = np.append(self.shown, deepcopy(self._clipboard["shown"]), axis=0)
+        self._size = np.append(self.size, deepcopy(self._clipboard["size"]), axis=0)
+        self._symbol = np.append(
+            self.symbol, deepcopy(self._clipboard["symbol"]), axis=0
+        )
+
+        self._feature_table.append(self._clipboard["features"])
+
+        self.text._paste(**self._clipboard["text"])
+
+        self._edge_width = np.append(
+            self.edge_width,
+            deepcopy(self._clipboard["edge_width"]),
+            axis=0,
+        )
+        self._edge._paste(
+            colors=self._clipboard["edge_color"],
+            properties=_features_to_properties(self._clipboard["features"]),
+        )
+        self._face._paste(
+            colors=self._clipboard["face_color"],
+            properties=_features_to_properties(self._clipboard["features"]),
+        )
+
+        self._selected_view = list(
+            range(npoints, npoints + len(self._clipboard["data"]))
+        )
+        self._selected_data = set(
+            range(totpoints, totpoints + len(self._clipboard["data"]))
+        )
+        self.refresh()
+
+
 # Hack to save a KeyPoints layer without showing the Save dialog
 def _save_layers_dialog(self, selected=False):
     """Save layers (all or selected) to disk, using ``LayerList.save()``.
     Parameters
     ----------
     selected : bool
         If True, only layers that are selected in the viewer will be saved.
         By default, all layers are saved.
     """
     selected_layers = list(self.viewer.layers.selection)
     msg = ""
     if not len(self.viewer.layers):
         msg = "There are no layers in the viewer to save."
     elif selected and not len(selected_layers):
-        msg = (
-            "Please select one or more layers to save," '\nor use "Save all layers..."'
-        )
+        msg = "Please select a Points layer to save."
     if msg:
         QMessageBox.warning(self, "Nothing to save", msg, QMessageBox.Ok)
         return
     if len(selected_layers) == 1 and isinstance(selected_layers[0], Points):
         self.viewer.layers.save("", selected=True, plugin="napari-deeplabcut")
         self.viewer.status = "Data successfully saved"
     else:
@@ -152,15 +307,15 @@
 
         status_bar = self.viewer.window._qt_window.statusBar()
         self.last_saved_label = QLabel("")
         self.last_saved_label.hide()
         status_bar.addPermanentWidget(self.last_saved_label)
 
         # Hack napari's Welcome overlay to show more relevant instructions
-        overlay = self.viewer.window._qt_viewer._canvas_overlay
+        overlay = self.viewer.window._qt_viewer._welcome_widget
         welcome_widget = overlay.layout().itemAt(1).widget()
         welcome_widget.deleteLater()
         w = QtWelcomeWidget(None)
         overlay._overlay = w
         overlay.addWidget(w)
         overlay._overlay.sig_dropped.connect(overlay.sig_dropped)
 
@@ -181,50 +336,74 @@
         self._images_meta = dict()
 
         # Add some more controls
         self._layout = QVBoxLayout(self)
         self._menus = []
 
         self._video_group = self._form_video_action_menu()
+        self.video_widget = self.viewer.window.add_dock_widget(
+            self._video_group, name="video", area="right"
+        )
+        self.video_widget.setVisible(False)
 
-        vlayout = QHBoxLayout()
+        hlayout = QHBoxLayout()
         trail_label = QLabel("Show trails")
         self._trail_cb = QCheckBox()
         self._trail_cb.setToolTip("toggle trails visibility")
         self._trail_cb.setChecked(False)
         self._trail_cb.setEnabled(False)
         self._trail_cb.stateChanged.connect(self._show_trails)
         self._trails = None
 
         self._view_scheme_cb = QCheckBox("Show color scheme", parent=self)
 
-        vlayout.addWidget(trail_label)
-        vlayout.addWidget(self._trail_cb)
-        vlayout.addWidget(self._view_scheme_cb)
+        hlayout.addWidget(trail_label)
+        hlayout.addWidget(self._trail_cb)
+        hlayout.addWidget(self._view_scheme_cb)
 
-        self._layout.addLayout(vlayout)
+        self._layout.addLayout(hlayout)
 
         self._radio_group = self._form_mode_radio_buttons()
 
         self._display = ColorSchemeDisplay(parent=self)
         self._color_scheme_display = self._form_color_scheme_display(self.viewer)
         self._view_scheme_cb.toggled.connect(self._show_color_scheme)
         self._view_scheme_cb.toggle()
 
         # Substitute default menu action with custom one
-        for action in self.viewer.window.file_menu.actions():
-            if "save selected layer" in action.text().lower():
+        for action in self.viewer.window.file_menu.actions()[::-1]:
+            action_name = action.text().lower()
+            if "save selected layer" in action_name:
                 action.triggered.disconnect()
                 action.triggered.connect(
                     lambda: _save_layers_dialog(
                         self,
                         selected=True,
                     )
                 )
-                break
+            elif "save all layers" in action_name:
+                self.viewer.window.file_menu.removeAction(action)
+
+        # Add action to show the walkthrough again
+        launch_tutorial = QAction("&Launch Tutorial", self)
+        launch_tutorial.triggered.connect(self.start_tutorial)
+        self.viewer.window.view_menu.addAction(launch_tutorial)
+
+        if self.settings.value("first_launch", True) and not os.environ.get(
+            "hide_tutorial", False
+        ):
+            QTimer.singleShot(10, self.start_tutorial)
+            self.settings.setValue("first_launch", False)
+
+    @cached_property
+    def settings(self):
+        return QSettings()
+
+    def start_tutorial(self):
+        Tutorial(self.viewer.window._qt_window.current()).show()
 
     def _move_image_layer_to_bottom(self, index):
         if (ind := index) != 0:
             self.viewer.layers.move_selected(ind, 0)
             self.viewer.layers.select_next()  # Auto-select the Points layer
 
     def _show_color_scheme(self):
@@ -242,31 +421,28 @@
                     tail_length=50,
                     head_length=50,
                     tail_width=6,
                     name="trails",
                     colormap="viridis",
                 )
             self._trails.visible = True
-        else:
+        elif self._trails is not None:
             self._trails.visible = False
 
     def _form_video_action_menu(self):
         group_box = QGroupBox("Video")
         layout = QVBoxLayout()
         extract_button = QPushButton("Extract frame")
         extract_button.clicked.connect(self._extract_single_frame)
-        extract_button.setEnabled(False)
         layout.addWidget(extract_button)
         crop_button = QPushButton("Store crop coordinates")
         crop_button.clicked.connect(self._store_crop_coordinates)
-        crop_button.setEnabled(False)
         layout.addWidget(crop_button)
         group_box.setLayout(layout)
-        self._layout.addWidget(group_box)
-        return extract_button, crop_button
+        return group_box
 
     def _extract_single_frame(self, *args):
         image_layer = None
         points_layer = None
         for layer in self.viewer.layers:
             if isinstance(layer, Image):
                 image_layer = layer
@@ -285,25 +461,26 @@
                 df = _form_df(
                     points_layer.data,
                     {
                         "metadata": points_layer.metadata,
                         "properties": points_layer.properties,
                     },
                 )
-                df = df.iloc[ind:ind + 1]
+                df = df.iloc[ind : ind + 1]
                 df.index = pd.MultiIndex.from_tuples([Path(output_path).parts[-3:]])
-                filepath = os.path.join(image_layer.metadata["root"], "machinelabels-iter0.h5")
+                filepath = os.path.join(
+                    image_layer.metadata["root"], "machinelabels-iter0.h5"
+                )
                 if Path(filepath).is_file():
                     df_prev = pd.read_hdf(filepath)
                     guarantee_multiindex_rows(df_prev)
                     df = pd.concat([df_prev, df])
                     df = df[~df.index.duplicated(keep="first")]
                 df.to_hdf(filepath, key="machinelabels")
 
-
     def _store_crop_coordinates(self, *args):
         if not (project_path := self._images_meta.get("project")):
             return
         for layer in self.viewer.layers:
             if isinstance(layer, Shapes):
                 try:
                     ind = layer.shape_type.index("rectangle")
@@ -415,16 +592,15 @@
         layer.metadata.update(self._images_meta)
 
     def on_insert(self, event):
         layer = event.source[-1]
         if isinstance(layer, Image):
             paths = layer.metadata.get("paths")
             if paths is None:  # Then it's a video file
-                for widget in self._video_group:
-                    widget.setEnabled(True)
+                self.video_widget.setVisible(True)
             # Store the metadata and pass them on to the other layers
             self._images_meta.update(
                 {
                     "paths": paths,
                     "shape": layer.level_shapes[0],
                     "root": layer.metadata["root"],
                     "name": layer.name,
@@ -442,43 +618,56 @@
                 keypoints_menu = self._menus[0].menus["label"]
                 current_keypoint_set = set(
                     keypoints_menu.itemText(i) for i in range(keypoints_menu.count())
                 )
                 new_keypoint_set = set(layer.metadata["header"].bodyparts)
                 diff = new_keypoint_set.difference(current_keypoint_set)
                 if diff:
-                    answer = QMessageBox.question(self, "", "Do you want to display the new keypoints only?")
-                    if answer  == QMessageBox.Yes:
+                    answer = QMessageBox.question(
+                        self, "", "Do you want to display the new keypoints only?"
+                    )
+                    if answer == QMessageBox.Yes:
                         self.viewer.layers[-2].shown = False
 
                     self.viewer.status = f"New keypoint{'s' if len(diff) > 1 else ''} {', '.join(diff)} found."
                     for _layer, store in self._stores.items():
                         _layer.metadata["header"] = layer.metadata["header"]
-                        _layer.metadata["face_color_cycles"] = layer.metadata["face_color_cycles"]
-                        _layer.face_color_cycle = layer.face_color_cycle
                         store.layer = _layer
 
                     for menu in self._menus:
                         menu._map_individuals_to_bodyparts()
                         menu._update_items()
 
-                    self._update_color_scheme()
+                # Always update the colormap to reflect the one in the config.yaml file
+                for _layer, store in self._stores.items():
+                    _layer.metadata["face_color_cycles"] = layer.metadata[
+                        "face_color_cycles"
+                    ]
+                    _layer.face_color = "label"
+                    _layer.face_color_cycle = layer.metadata["face_color_cycles"][
+                        "label"
+                    ]
+                    _layer.events.face_color()
+                    store.layer = _layer
+                self._update_color_scheme()
 
                 # Remove the unnecessary layer newly added
                 QTimer.singleShot(10, self.viewer.layers.pop)
                 return
 
             store = keypoints.KeypointStore(self.viewer, layer)
             self._stores[layer] = store
             # TODO Set default dir of the save file dialog
             if root := layer.metadata.get("root"):
                 update_save_history(root)
             layer.metadata["controls"] = self
             layer.text.visible = False
             layer.bind_key("M", self.cycle_through_label_modes)
+            func = partial(_paste_data, store=store)
+            layer._paste_data = MethodType(func, layer)
             layer.add = MethodType(keypoints._add, store)
             layer.events.add(query_next_frame=Event)
             layer.events.query_next_frame.connect(store._advance_step)
             layer.bind_key("Shift-Right", store._find_first_unlabeled_frame)
             layer.bind_key("Shift-Left", store._find_first_unlabeled_frame)
 
             layer.bind_key("Down", store.next_keypoint, overwrite=True)
@@ -488,14 +677,26 @@
                 self._form_dropdown_menus(store)
             self._images_meta.update(
                 {
                     "project": layer.metadata.get("project"),
                 }
             )
             self._trail_cb.setEnabled(True)
+
+            # Hide the color pickers, as colormaps are strictly defined by users
+            controls = self.viewer.window.qt_viewer.dockLayerControls
+            point_controls = controls.widget().widgets[layer]
+            point_controls.faceColorEdit.hide()
+            point_controls.edgeColorEdit.hide()
+            point_controls.layout().itemAt(9).widget().hide()
+            point_controls.layout().itemAt(11).widget().hide()
+            # Hide out of slice checkbox
+            point_controls.outOfSliceCheckBox.hide()
+            point_controls.layout().itemAt(15).widget().hide()
+
         for layer_ in self.viewer.layers:
             if not isinstance(layer_, Image):
                 self._remap_frame_indices(layer_)
 
     def on_remove(self, event):
         layer = event.value
         n_points_layer = sum(isinstance(l, Points) for l in self.viewer.layers)
@@ -510,16 +711,15 @@
                 menu.destroy()
             self._trail_cb.setEnabled(False)
             self.last_saved_label.hide()
         elif isinstance(layer, Image):
             self._images_meta = dict()
             paths = layer.metadata.get("paths")
             if paths is None:
-                for widget in self._video_group:
-                    widget.setEnabled(False)
+                self.video_widget.setVisible(False)
         elif isinstance(layer, Tracks):
             self._trail_cb.setChecked(False)
             self._trails = None
 
     @register_points_action("Change labeling mode")
     def cycle_through_label_modes(self, *args):
         self.label_mode = next(keypoints.LabelMode)
@@ -614,15 +814,17 @@
     def _populate_menus(self):
         id_ = self.store.ids[0]
         if id_:
             menu = create_dropdown_menu(self.store, list(self.id2label), "id")
             menu.currentTextChanged.connect(self.refresh_label_menu)
             self.menus["id"] = menu
         self.menus["label"] = create_dropdown_menu(
-            self.store, self.id2label[id_], "label",
+            self.store,
+            self.id2label[id_],
+            "label",
         )
 
     def _update_items(self):
         id_ = self.store.ids[0]
         if id_:
             self.menus["id"].update_items(list(self.id2label))
         self.menus["label"].update_items(self.id2label[id_])
@@ -656,15 +858,17 @@
             return
         unannotated = ""
         already_annotated = self.store.annotated_keypoints
         for keypoint in self.store._keypoints:
             if keypoint not in already_annotated:
                 unannotated = keypoint
                 break
-        self.store.current_keypoint = unannotated if unannotated else self.store._keypoints[0]
+        self.store.current_keypoint = (
+            unannotated if unannotated else self.store._keypoints[0]
+        )
 
 
 def create_dropdown_menu(store, items, attr):
     menu = DropdownMenu(items)
 
     def item_changed(ind):
         current_item = menu.itemText(ind)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut/_writer.py` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut/_writer.py`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut/keypoints.py` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut/keypoints.py`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut/misc.py` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut/misc.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,14 +23,48 @@
     map_ = dict(zip(unique_cat, range(len(unique_cat))))
     inds = np.vectorize(map_.get)(categories)
     if return_map:
         return inds, map_
     return inds
 
 
+def merge_multiple_scorers(
+    df: pd.DataFrame,
+) -> pd.DataFrame:
+    n_frames = df.shape[0]
+    header = DLCHeader(df.columns)
+    n_scorers = len(header._get_unique("scorer"))
+    if n_scorers == 1:
+        return df
+
+    if "likelihood" in header.coords:
+        # Merge annotations from multiple scorers to keep
+        # detections with highest confidence
+        data = df.to_numpy().reshape((n_frames, n_scorers, -1, 3))
+        try:
+            idx = np.nanargmax(data[..., 2], axis=1)
+        except ValueError:  # All-NaN slice encountered
+            mask = np.isnan(data[..., 2]).all(axis=1, keepdims=True)
+            mask = np.broadcast_to(mask[..., None], data.shape)
+            data[mask] = -1
+            idx = np.nanargmax(data[..., 2], axis=1)
+            data[mask] = np.nan
+        data_best = data[
+            np.arange(n_frames)[:, None], idx, np.arange(data.shape[2])
+        ].reshape((n_frames, -1))
+        df = pd.DataFrame(
+            data_best,
+            index=df.index,
+            columns=header.columns[: data_best.shape[1]],
+        )
+    else:  # Arbitrarily pick data from the first scorer
+        df = df.loc(axis=1)[: header.scorer]
+    return df
+
+
 def to_os_dir_sep(path: str) -> str:
     """
     Replace all directory separators in `path` with `os.path.sep`.
     Function originally written by @pyzun:
     https://github.com/DeepLabCut/napari-DeepLabCut/pull/13
 
     Raises
```

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut/napari.yaml` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.2/src/napari_deeplabcut.egg-info/SOURCES.txt` & `napari_deeplabcut-0.2.0/src/napari_deeplabcut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_deeplabcut-0.1.2/tox.ini` & `napari_deeplabcut-0.2.0/tox.ini`

 * *Files identical despite different names*

