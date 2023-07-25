# Comparing `tmp/autoray-0.6.4.tar.gz` & `tmp/autoray-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoray-0.6.4.tar", last modified: Tue Jul 25 23:28:47 2023, max compression
+gzip compressed data, was "autoray-0.6.5.tar", last modified: Tue Jul 25 23:31:39 2023, max compression
```

## Comparing `autoray-0.6.4.tar` & `autoray-0.6.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.877347 autoray-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 23:28:26.000000 autoray-0.6.4/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 23:28:26.000000 autoray-0.6.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.861347 autoray-0.6.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.865347 autoray-0.6.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-25 23:28:26.000000 autoray-0.6.4/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-25 23:28:26.000000 autoray-0.6.4/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-25 23:28:26.000000 autoray-0.6.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 23:28:26.000000 autoray-0.6.4/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-25 23:28:26.000000 autoray-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 23:28:26.000000 autoray-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-07-25 23:28:47.877347 autoray-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-07-25 23:28:26.000000 autoray-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.865347 autoray-0.6.4/autoray/
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-25 23:28:26.000000 autoray-0.6.4/autoray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 23:28:47.000000 autoray-0.6.4/autoray/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    59751 2023-07-25 23:28:26.000000 autoray-0.6.4/autoray/autoray.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-25 23:28:26.000000 autoray-0.6.4/autoray/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.869347 autoray-0.6.4/autoray/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:26.000000 autoray-0.6.4/autoray/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-25 23:28:26.000000 autoray-0.6.4/autoray/experimental/complexity_tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)  1265159 2023-07-25 23:28:26.000000 autoray-0.6.4/autoray/experimental/complexity_tracing_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.873347 autoray-0.6.4/autoray/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 23:28:26.000000 autoray-0.6.4/autoray/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48582 2023-07-25 23:28:26.000000 autoray-0.6.4/autoray/lazy/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    25844 2023-07-25 23:28:26.000000 autoray-0.6.4/autoray/lazy/draw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-25 23:28:26.000000 autoray-0.6.4/autoray/lazy/linalg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.869347 autoray-0.6.4/autoray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-07-25 23:28:47.000000 autoray-0.6.4/autoray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-25 23:28:47.000000 autoray-0.6.4/autoray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:28:47.000000 autoray-0.6.4/autoray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 23:28:47.000000 autoray-0.6.4/autoray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 23:28:47.000000 autoray-0.6.4/autoray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.861347 autoray-0.6.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.873347 autoray-0.6.4/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-25 23:28:26.000000 autoray-0.6.4/ci/requirements/py-base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-25 23:28:26.000000 autoray-0.6.4/ci/requirements/py-jax.yml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-25 23:28:26.000000 autoray-0.6.4/ci/requirements/py-tensorflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-25 23:28:26.000000 autoray-0.6.4/ci/requirements/py-torch.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.873347 autoray-0.6.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.873347 autoray-0.6.4/docs/_pygments/
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/_pygments/_pygments_dark.py
--rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/_pygments/_pygments_light.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.877347 autoray-0.6.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    26562 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/_static/autoray-header.png
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/_static/my-styles.css
--rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/automatic_dispatch.md
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/compilation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/development.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.877347 autoray-0.6.4/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    57965 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/images/autoray-readme-pic-0.png
--rw-r--r--   0 runner    (1001) docker     (123)    99582 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/images/autoray-readme-pic-1.png
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)   608532 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/lazy_computation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 23:28:26.000000 autoray-0.6.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-25 23:28:26.000000 autoray-0.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:28:47.877347 autoray-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-25 23:28:26.000000 autoray-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:47.877347 autoray-0.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:28:26.000000 autoray-0.6.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-25 23:28:26.000000 autoray-0.6.4/tests/test_autocompile.py
--rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-07-25 23:28:26.000000 autoray-0.6.4/tests/test_autoray.py
--rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-07-25 23:28:26.000000 autoray-0.6.4/tests/test_lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.169408 autoray-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 23:31:18.000000 autoray-0.6.5/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 23:31:18.000000 autoray-0.6.5/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.157408 autoray-0.6.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.161408 autoray-0.6.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-07-25 23:31:18.000000 autoray-0.6.5/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-25 23:31:18.000000 autoray-0.6.5/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-25 23:31:18.000000 autoray-0.6.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 23:31:18.000000 autoray-0.6.5/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11558 2023-07-25 23:31:18.000000 autoray-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 23:31:18.000000 autoray-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-07-25 23:31:39.169408 autoray-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17484 2023-07-25 23:31:18.000000 autoray-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.161408 autoray-0.6.5/autoray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60207 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/autoray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.161408 autoray-0.6.5/autoray/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/experimental/complexity_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1265159 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/experimental/complexity_tracing_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.165408 autoray-0.6.5/autoray/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48582 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/lazy/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25846 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/lazy/draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-07-25 23:31:18.000000 autoray-0.6.5/autoray/lazy/linalg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.161408 autoray-0.6.5/autoray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18380 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 23:31:39.000000 autoray-0.6.5/autoray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.157408 autoray-0.6.5/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.165408 autoray-0.6.5/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-25 23:31:18.000000 autoray-0.6.5/ci/requirements/py-base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-25 23:31:18.000000 autoray-0.6.5/ci/requirements/py-jax.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-25 23:31:18.000000 autoray-0.6.5/ci/requirements/py-tensorflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-25 23:31:18.000000 autoray-0.6.5/ci/requirements/py-torch.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.165408 autoray-0.6.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.165408 autoray-0.6.5/docs/_pygments/
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/_pygments/_pygments_dark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5435 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/_pygments/_pygments_light.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.169408 autoray-0.6.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    26562 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/_static/autoray-header.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/_static/my-styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10755 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/automatic_dispatch.md
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/compilation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.169408 autoray-0.6.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    57965 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/images/autoray-readme-pic-0.png
+-rw-r--r--   0 runner    (1001) docker     (123)    99582 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/images/autoray-readme-pic-1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)   608532 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/lazy_computation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-25 23:31:18.000000 autoray-0.6.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-25 23:31:18.000000 autoray-0.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 23:31:39.169408 autoray-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-25 23:31:18.000000 autoray-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:39.169408 autoray-0.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:31:18.000000 autoray-0.6.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-07-25 23:31:18.000000 autoray-0.6.5/tests/test_autocompile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23160 2023-07-25 23:31:18.000000 autoray-0.6.5/tests/test_autoray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-07-25 23:31:18.000000 autoray-0.6.5/tests/test_lazy.py
```

### Comparing `autoray-0.6.4/.github/workflows/pypi-release.yml` & `autoray-0.6.5/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/.github/workflows/tests.yml` & `autoray-0.6.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/.gitignore` & `autoray-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/LICENSE` & `autoray-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/PKG-INFO` & `autoray-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoray
-Version: 0.6.4
+Version: 0.6.5
 Summary: Abstract your array operations.
 Home-page: http://github.com/jcmgray/autoray
 Author: Johnnie Gray
 Author-email: johnniemcgray@gmail.com
 License: Apache
 Project-URL: Bug Reports, https://github.com/jcmgray/autoray/issues
 Project-URL: Source, https://github.com/jcmgray/autoray/
```

### Comparing `autoray-0.6.4/README.md` & `autoray-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/autoray/__init__.py` & `autoray-0.6.5/autoray/__init__.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/autoray/autoray.py` & `autoray-0.6.5/autoray/autoray.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,15 +399,16 @@
 
             # move any prepended location into the full module path
             #     e.g. 'fn=linalg.eigh' -> ['linalg', 'eigh']
             split_fn = fn.split(".")
             full_location = ".".join([full_location] + split_fn[:-1])
             only_fn = split_fn[-1]
 
-            # try aliases for global (not function specific) modules and submodules
+            # try aliases for global (not function specific) modules and
+            # submodules:
             #     e.g. 'decimal' -> 'math'
             #     e.g. 'cupy.scipy' -> 'cupyx.scipy'
             # we don't do this if the function location has been explicitly
             # give in _SUBMODULE_ALIASES, as that is already a full path
             for k, v in _MODULE_ALIASES.items():
                 if full_location[: len(k)] == k:
                     full_location = full_location.replace(k, v, 1)
@@ -829,15 +830,18 @@
                 return fn
 
             return wrapper
 
     def make_function(self, backend):
         """Make a new function for the specific ``backend``."""
         if self._supply_backend:
-            fn = functools.partial(self._default_fn, backend=backend)
+            # make sure it inherits __name__ etc
+            fn = functools.wraps(self._default_fn)(
+                functools.partial(self._default_fn, backend=backend)
+            )
         else:
             fn = self._default_fn
         self.register(backend, fn)
         return fn
 
     def __call__(self, *args, like=None, **kwargs):
         backend = choose_backend(self._name, *args, like=like, **kwargs)
@@ -1318,22 +1322,30 @@
     """
     return infer_backend_multi(*args)
 
 
 register_dispatch("einsum", einsum_dispatcher)
 
 
-def tensordot_dispatcher(*args, **_):
-    """There are cases when we want to take into account both backends."""
+def binary_dispatcher(*args, **_):
+    """There are cases when we want to take into account both backends of two
+    arguments, e.g. a lazy variable and a constant array.
+    """
     return infer_backend_multi(*args[:2])
 
 
-register_dispatch("tensordot", tensordot_dispatcher)
+register_dispatch("tensordot", binary_dispatcher)
+register_dispatch("matmul", binary_dispatcher)
+register_dispatch("multiply", binary_dispatcher)
+register_dispatch("divide", binary_dispatcher)
+register_dispatch("true_divide", binary_dispatcher)
+register_dispatch("add", binary_dispatcher)
+register_dispatch("subtract", binary_dispatcher)
 
-# TODO: register other binary functions such as add, matmul etc?
+# TODO: register other binary functions?
 
 # --------------- object to act as drop-in replace for numpy ---------------- #
 
 _partial_functions = {}
 
 
 class NumpyMimic:
```

### Comparing `autoray-0.6.4/autoray/compiler.py` & `autoray-0.6.5/autoray/compiler.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/autoray/experimental/complexity_tracing.py` & `autoray-0.6.5/autoray/experimental/complexity_tracing.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,23 +101,28 @@
     "matmul": cost_matmul,
     "einsum": cost_einsum,
     # other cheap ops
     "mul": cost_linear,
     "add": cost_linear,
     "neg": cost_linear,
     "sqrt": cost_linear,
+    "cupy_sqrt": cost_linear,
     "pow": cost_linear,
     "truediv": cost_linear,
     "log10": cost_linear,
+    "cupy_log10": cost_linear,
     "norm": cost_linear,
+    "linalg_norm": cost_linear,
     "reshape": cost_linear,
     "conj": cost_linear,
     "conjugate": cost_linear,
+    "cupy_conjugate": cost_linear,
     "clip": cost_linear,
     "transpose": cost_linear,
+    "torch_transpose": cost_linear,
     "getitem": cost_nothing,
     "None": cost_nothing,
 }
 
 def cost_node(x, allow_missed=True):
     f = x.fn_name
     if f in COSTS:
```

### Comparing `autoray-0.6.4/autoray/experimental/complexity_tracing_example.ipynb` & `autoray-0.6.5/autoray/experimental/complexity_tracing_example.ipynb`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/autoray/lazy/__init__.py` & `autoray-0.6.5/autoray/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/autoray/lazy/core.py` & `autoray-0.6.5/autoray/lazy/core.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/autoray/lazy/draw.py` & `autoray-0.6.5/autoray/lazy/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -807,15 +807,15 @@
 @default_to_neutral_style
 def plot_history_functions(
     self,
     *,
     fn=None,
     log=None,
     colors=None,
-    kind="lines",
+    kind="scatter",
     scatter_size=5,
     scatter_marker="s",
     lines_width=5,
     image_alpha_pow=2 / 3,
     image_aspect=4,
     legend=True,
     legend_ncol=None,
```

### Comparing `autoray-0.6.4/autoray/lazy/linalg.py` & `autoray-0.6.5/autoray/lazy/linalg.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/autoray.egg-info/PKG-INFO` & `autoray-0.6.5/autoray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoray
-Version: 0.6.4
+Version: 0.6.5
 Summary: Abstract your array operations.
 Home-page: http://github.com/jcmgray/autoray
 Author: Johnnie Gray
 Author-email: johnniemcgray@gmail.com
 License: Apache
 Project-URL: Bug Reports, https://github.com/jcmgray/autoray/issues
 Project-URL: Source, https://github.com/jcmgray/autoray/
```

### Comparing `autoray-0.6.4/autoray.egg-info/SOURCES.txt` & `autoray-0.6.5/autoray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/Makefile` & `autoray-0.6.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/_pygments/_pygments_dark.py` & `autoray-0.6.5/docs/_pygments/_pygments_dark.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/_pygments/_pygments_light.py` & `autoray-0.6.5/docs/_pygments/_pygments_light.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/_static/autoray-header.png` & `autoray-0.6.5/docs/_static/autoray-header.png`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/_static/my-styles.css` & `autoray-0.6.5/docs/_static/my-styles.css`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/automatic_dispatch.md` & `autoray-0.6.5/docs/automatic_dispatch.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/compilation.ipynb` & `autoray-0.6.5/docs/compilation.ipynb`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/conf.py` & `autoray-0.6.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/images/autoray-readme-pic-0.png` & `autoray-0.6.5/docs/images/autoray-readme-pic-0.png`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/images/autoray-readme-pic-1.png` & `autoray-0.6.5/docs/images/autoray-readme-pic-1.png`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/index.md` & `autoray-0.6.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/installation.md` & `autoray-0.6.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/lazy_computation.ipynb` & `autoray-0.6.5/docs/lazy_computation.ipynb`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/docs/make.bat` & `autoray-0.6.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/pyproject.toml` & `autoray-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/setup.py` & `autoray-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/tests/test_autocompile.py` & `autoray-0.6.5/tests/test_autocompile.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/tests/test_autoray.py` & `autoray-0.6.5/tests/test_autoray.py`

 * *Files identical despite different names*

### Comparing `autoray-0.6.4/tests/test_lazy.py` & `autoray-0.6.5/tests/test_lazy.py`

 * *Files identical despite different names*

