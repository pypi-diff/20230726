# Comparing `tmp/MultiAssayExperiment-0.2.3.tar.gz` & `tmp/MultiAssayExperiment-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MultiAssayExperiment-0.2.3.tar", last modified: Tue Jul 25 06:27:24 2023, max compression
+gzip compressed data, was "MultiAssayExperiment-0.2.4.tar", last modified: Wed Jul 26 03:48:33 2023, max compression
```

## Comparing `MultiAssayExperiment-0.2.3.tar` & `MultiAssayExperiment-0.2.4.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.546064 MultiAssayExperiment-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.518064 MultiAssayExperiment-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.530064 MultiAssayExperiment-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-25 06:27:24.546064 MultiAssayExperiment-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.534064 MultiAssayExperiment-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.538064 MultiAssayExperiment-0.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-25 06:27:24.550064 MultiAssayExperiment-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.518064 MultiAssayExperiment-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.542064 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-25 06:27:24.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-25 06:27:24.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:27:24.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 06:25:51.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-25 06:27:24.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 06:27:24.000000 MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.542064 MultiAssayExperiment-0.2.3/src/multiassayexperiment/
--rw-r--r--   0 runner    (1001) docker     (123)    20347 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/MultiAssayExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.542064 MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/anndata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/mudata.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/src/multiassayexperiment/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.546064 MultiAssayExperiment-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 06:27:24.546064 MultiAssayExperiment-0.2.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   311344 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/data/adata.h5ad
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/test_se_add_expt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/test_se_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/test_se_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/test_se_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tests/test_se_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-25 06:25:38.000000 MultiAssayExperiment-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.816012 MultiAssayExperiment-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.804011 MultiAssayExperiment-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.808011 MultiAssayExperiment-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-26 03:48:33.816012 MultiAssayExperiment-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.808011 MultiAssayExperiment-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.812012 MultiAssayExperiment-0.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-26 03:48:33.816012 MultiAssayExperiment-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.804011 MultiAssayExperiment-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.812012 MultiAssayExperiment-0.2.4/src/MultiAssayExperiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-26 03:48:33.000000 MultiAssayExperiment-0.2.4/src/MultiAssayExperiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-26 03:48:33.000000 MultiAssayExperiment-0.2.4/src/MultiAssayExperiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 03:48:33.000000 MultiAssayExperiment-0.2.4/src/MultiAssayExperiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 03:47:13.000000 MultiAssayExperiment-0.2.4/src/MultiAssayExperiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-26 03:48:33.000000 MultiAssayExperiment-0.2.4/src/MultiAssayExperiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-26 03:48:33.000000 MultiAssayExperiment-0.2.4/src/MultiAssayExperiment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.812012 MultiAssayExperiment-0.2.4/src/multiassayexperiment/
+-rw-r--r--   0 runner    (1001) docker     (123)    20984 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/src/multiassayexperiment/MultiAssayExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/src/multiassayexperiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.812012 MultiAssayExperiment-0.2.4/src/multiassayexperiment/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/src/multiassayexperiment/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/src/multiassayexperiment/io/anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/src/multiassayexperiment/io/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/src/multiassayexperiment/io/mudata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/src/multiassayexperiment/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.816012 MultiAssayExperiment-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 03:48:33.816012 MultiAssayExperiment-0.2.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   311344 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/tests/data/adata.h5ad
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/tests/test_add_expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/tests/test_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/tests/test_with_coldata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-26 03:47:01.000000 MultiAssayExperiment-0.2.4/tox.ini
```

### Comparing `MultiAssayExperiment-0.2.3/.coveragerc` & `MultiAssayExperiment-0.2.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/.github/workflows/pypi-publish.yml` & `MultiAssayExperiment-0.2.4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/.github/workflows/pypi-test.yml` & `MultiAssayExperiment-0.2.4/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/.gitignore` & `MultiAssayExperiment-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/CONTRIBUTING.rst` & `MultiAssayExperiment-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/LICENSE.txt` & `MultiAssayExperiment-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/PKG-INFO` & `MultiAssayExperiment-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiAssayExperiment
-Version: 0.2.3
+Version: 0.2.4
 Summary: Container class to represent multiple experiments and assays performed over a set of samples
 Home-page: https://github.com/BiocPy/MultiAssayExperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/MultiAssayExperiment
 Platform: any
```

### Comparing `MultiAssayExperiment-0.2.3/README.md` & `MultiAssayExperiment-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/docs/Makefile` & `MultiAssayExperiment-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/docs/conf.py` & `MultiAssayExperiment-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/docs/index.md` & `MultiAssayExperiment-0.2.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/docs/readme.md` & `MultiAssayExperiment-0.2.4/docs/readme.md`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/docs/tutorial.md` & `MultiAssayExperiment-0.2.4/docs/tutorial.md`

 * *Files 4% similar despite different names*

```diff
@@ -85,41 +85,39 @@
     rowData=df_gr.copy(),
     colData=colData_se.copy(),
 )
 ```
 
 Now that we have all the pieces together, we can now create an MAE,
 
-
 ```python
 from multiassayexperiment import MultiAssayExperiment
 
 maeObj = MultiAssayExperiment(
     experiments={"sce": tsce, "se": tse2},
     colData=sample_data,
     sampleMap=sample_map,
     metadata={"could be": "anything"},
 )
 ```
 
-To make your life easier, we also provide methods to naively create sample mapping from experiments. 
+To make your life easier, we also provide methods to naively create sample mapping from experiments.
 
-***This is not a recommended approach, but if you don't have sample mapping, then it doesn't matter.***
+**_This is not a recommended approach, but if you don't have sample mapping, then it doesn't matter._**
 
 ```python
 maeObj = mae.makeMAE(experiments={"sce": tsce, "se": tse2})
 ```
 
-# Import `MuData` and `AnnData` as `MultiAssayExperiment`
+## Import `MuData` and `AnnData` as `MultiAssayExperiment`
 
 If you have a dataset stored as `MuData`, these can be easily converted to an MAE using the `fromMuData` method.
 
 Lets first construct AnnData objects and then an MAE
 
-
 ```python
 import multiassayexperiment as mae
 import numpy as np
 from anndata import AnnData
 
 np.random.seed(1)
 
@@ -162,17 +160,31 @@
 
 ```python
 maeObj.assays
 maeObj.colData
 maeObj.sampleMap
 maeObj.experiments
 maeObj.metadata
+```
+
+## Access experiments
 
+if you want to access a specific experiment
+
+```python
 # access a specific experiment
-maeObj.experiment(experiment name)
+maeObj.experiment(experiment_name)
+```
+
+This does not include the sample data stored in the MAE. If you want to include this information
+
+***Note: This creates a copy of the experiment object.***
+
+```python
+expt_with_sampleData = maeObj.experiment(experiment_name, withSampleData=True)
 ```
 
 # Slice a `MultiAssayExperiment`
 
 `MultiAssayExperiment` allows subsetting by `rows`, `columns`, and `experiments`. Samples are automatically sliced during this operation.
 
 The structure for slicing,
@@ -188,15 +200,14 @@
 
 ```python
 maeObj[1:5, 0:4]
 ```
 
 ## Slice by rows, columns, experiments
 
-
 ```python
 maeObj[1:5, 0:4, ["spatial"]]
 ```
 
 ## Specify slices per experiment
 
 You can specify slices by experiment, rest of the experiments are not sliced.
@@ -219,8 +230,8 @@
 
 ## replicated
 
 replicated identifies biospecimens that have multiple observations per experiment.
 
 ```python
 maeObj.replicated()
-```
+```
```

### Comparing `MultiAssayExperiment-0.2.3/setup.cfg` & `MultiAssayExperiment-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/setup.py` & `MultiAssayExperiment-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/PKG-INFO` & `MultiAssayExperiment-0.2.4/src/MultiAssayExperiment.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiAssayExperiment
-Version: 0.2.3
+Version: 0.2.4
 Summary: Container class to represent multiple experiments and assays performed over a set of samples
 Home-page: https://github.com/BiocPy/MultiAssayExperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/MultiAssayExperiment
 Platform: any
```

### Comparing `MultiAssayExperiment-0.2.3/src/MultiAssayExperiment.egg-info/SOURCES.txt` & `MultiAssayExperiment-0.2.4/src/MultiAssayExperiment.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,13 +33,14 @@
 src/multiassayexperiment/__init__.py
 src/multiassayexperiment/types.py
 src/multiassayexperiment/io/__init__.py
 src/multiassayexperiment/io/anndata.py
 src/multiassayexperiment/io/interface.py
 src/multiassayexperiment/io/mudata.py
 tests/conftest.py
-tests/test_se_add_expt.py
-tests/test_se_create.py
-tests/test_se_io.py
-tests/test_se_methods.py
-tests/test_se_slices.py
+tests/test_add_expt.py
+tests/test_create.py
+tests/test_io.py
+tests/test_methods.py
+tests/test_slices.py
+tests/test_with_coldata.py
 tests/data/adata.h5ad
```

### Comparing `MultiAssayExperiment-0.2.3/src/multiassayexperiment/MultiAssayExperiment.py` & `MultiAssayExperiment-0.2.4/src/multiassayexperiment/MultiAssayExperiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import OrderedDict
-from typing import MutableMapping, Optional, Sequence, Tuple, Union
+from copy import deepcopy
+from typing import MutableMapping, Optional, Sequence
 
 import pandas as pd
 from mudata import MuData
 from singlecellexperiment import SingleCellExperiment
 from summarizedexperiment import SummarizedExperiment
 from summarizedexperiment._type_checks import is_bioc_or_pandas_frame, is_list_of_type
 from summarizedexperiment.BaseSE import BaseSE
@@ -200,30 +201,46 @@
             experiments (MutableMapping[str, BaseSE]): new experiments to set.
         """
 
         self._validate_experiments(experiments)
         self._validate_sampleMap_with_Expts(self._sampleMap, experiments)
         self._experiments = experiments
 
-    def experiment(self, name: str) -> BaseSE:
+    def experiment(self, name: str, withSampleData: bool = False) -> BaseSE:
         """Get experiment by name.
 
+        if withSampleData is True, a copy of the experiment object is returned.
+
         Args:
             name (str): experiment name.
+            with_sampleData (bool, optional): include sample data in returned object?
+                Defaults to False.
 
         Raises:
             ValueError: if experiment name does not exist.
 
         Returns:
             BaseSE: experiment.
         """
         if name not in self._experiments:
             raise ValueError(f"Experiment {name} does not exist")
 
-        return self._experiments[name]
+        expt = self._experiments[name]
+
+        if withSampleData is True:
+            expt = deepcopy(self._experiments[name])
+
+            subset_map = self.sampleMap[self.sampleMap["assay"] == name]
+            subset_map = subset_map.set_index("colname")
+
+            expt_colData = expt.colData
+            new_colData = pd.concat([subset_map, expt_colData], axis=1)
+            expt.colData = new_colData
+
+        return expt
 
     @property
     def sampleMap(self) -> pd.DataFrame:
         """Get sample map between experiments and sample metadata.
 
         Returns:
             pd.DataFrame: sample map.
```

### Comparing `MultiAssayExperiment-0.2.3/src/multiassayexperiment/__init__.py` & `MultiAssayExperiment-0.2.4/src/multiassayexperiment/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import sys
 
 if sys.version_info[:2] >= (3, 8):
     # TODO: Import directly (no need for conditional) when `python_requires = >= 3.8`
     from importlib.metadata import (
         PackageNotFoundError,
         version,
-    )  # pragma: no cover
+    )
 else:
     from importlib_metadata import (
         PackageNotFoundError,
         version,
-    )  # pragma: no cover
+    )
 
 try:
     # Change here if project is renamed and does not equal the package name
     dist_name = "MultiAssayExperiment"
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
-from .MultiAssayExperiment import MultiAssayExperiment
-from .io.anndata import readH5AD, fromAnnData
-from .io.mudata import fromMuData
+from .io.anndata import fromAnnData, readH5AD
 from .io.interface import makeMAE
+from .io.mudata import fromMuData
+from .MultiAssayExperiment import MultiAssayExperiment
```

### Comparing `MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/anndata.py` & `MultiAssayExperiment-0.2.4/src/multiassayexperiment/io/anndata.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/interface.py` & `MultiAssayExperiment-0.2.4/src/multiassayexperiment/io/interface.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/src/multiassayexperiment/io/mudata.py` & `MultiAssayExperiment-0.2.4/src/multiassayexperiment/io/mudata.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/src/multiassayexperiment/types.py` & `MultiAssayExperiment-0.2.4/src/multiassayexperiment/types.py`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/tests/data/adata.h5ad` & `MultiAssayExperiment-0.2.4/tests/data/adata.h5ad`

 * *Files identical despite different names*

### Comparing `MultiAssayExperiment-0.2.3/tests/test_se_add_expt.py` & `MultiAssayExperiment-0.2.4/tests/test_with_coldata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-import pytest
+from random import random
 
-from multiassayexperiment import MultiAssayExperiment
-import multiassayexperiment
-from singlecellexperiment import SingleCellExperiment
+import genomicranges
 import numpy as np
-from random import random
 import pandas as pd
-import genomicranges
+from multiassayexperiment import MultiAssayExperiment
+from singlecellexperiment import SingleCellExperiment
 from summarizedexperiment import SummarizedExperiment
-from anndata import AnnData
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
-
 nrows = 200
 ncols = 6
 counts = np.random.rand(nrows, ncols)
 df_gr = pd.DataFrame(
     {
         "seqnames": [
             "chr1",
@@ -39,51 +35,73 @@
         "score": range(0, 200),
         "GC": [random() for _ in range(10)] * 20,
     }
 )
 
 gr = genomicranges.fromPandas(df_gr)
 
-colData_sce = pd.DataFrame({"treatment": ["ChIP", "Input"] * 3,}, index=["sce"] * 6,)
-
-sample_map_sce = pd.DataFrame(
-    {"assay": ["sce"] * 6, "primary": ["sample1"] * 6, "colname": ["sce"] * 6,}
+colData_sce = pd.DataFrame(
+    {
+        "treatment": ["ChIP", "Input"] * 3,
+    },
+    index=[f"sce_{i}" for i in range(6)],
+)
+colData_se = pd.DataFrame(
+    {
+        "treatment": ["ChIP", "Input"] * 3,
+    },
+    index=[f"se_{i}" for i in range(6)],
 )
 
-sample_coldata_sce = pd.DataFrame({"samples": ["sample1"]}, index=["sample1"])
-
-colData_se = pd.DataFrame({"treatment": ["ChIP", "Input"] * 3,}, index=["se"] * 6,)
+sample_map = pd.DataFrame(
+    {
+        "assay": ["sce", "se"] * 6,
+        "primary": ["sample1", "sample2"] * 6,
+        "colname": [
+            "sce_0",
+            "se_0",
+            "sce_1",
+            "se_1",
+            "sce_2",
+            "se_2",
+            "sce_3",
+            "se_3",
+            "sce_4",
+            "se_4",
+            "sce_5",
+            "se_5",
+        ],
+    }
+)
 
-sample_map_se = pd.DataFrame(
-    {"assay": ["se"] * 6, "primary": ["sample2"] * 6, "colname": ["se"] * 6,}
+sample_data = pd.DataFrame(
+    {"samples": ["sample1", "sample2"]}, index=["sample1", "sample2"]
 )
 
-sample_coldata_se = pd.DataFrame({"samples": ["sample2"]}, index=["sample2"])
+tsce = SingleCellExperiment(
+    assays={"counts": counts}, rowData=df_gr, colData=colData_sce
+)
 
+tse2 = SummarizedExperiment(
+    assays={"counts": counts.copy()},
+    rowData=df_gr.copy(),
+    colData=colData_se.copy(),
+)
 
-def test_MAE_addExpt():
-    tsce = SingleCellExperiment(
-        assays={"counts": counts}, rowData=df_gr, colData=colData_sce
-    )
+mae = MultiAssayExperiment(
+    experiments={"sce": tsce, "se": tse2},
+    colData=sample_data,
+    sampleMap=sample_map,
+    metadata={"could be": "anything"},
+)
 
-    mae = MultiAssayExperiment(
-        experiments={"sce": tsce},
-        colData=sample_coldata_sce,
-        sampleMap=sample_map_sce,
-        metadata={"could be": "anything"},
-    )
 
+def test_access_expt_with_coldata():
     assert mae is not None
-    assert isinstance(mae, MultiAssayExperiment)
 
-    tse2 = SummarizedExperiment(
-        assays={"counts": counts.copy()},
-        rowData=df_gr.copy(),
-        colData=colData_se,
-    )
-
-    mae.addExperiment(
-        name="se", experiment=tse2, sampleMap=sample_map_se, colData=sample_coldata_se
-    )
+    se = mae.experiment("se")
+    assert se.shape == tse2.shape
 
-    assert mae is not None
+    sce = mae.experiment("sce", withSampleData=True)
+    assert sce.shape == tsce.shape
 
+    assert len(sce.colData.columns) >= len(tsce.colData.columns)
```

### Comparing `MultiAssayExperiment-0.2.3/tests/test_se_create.py` & `MultiAssayExperiment-0.2.4/tests/test_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import pytest
+from random import random
 
-from multiassayexperiment import MultiAssayExperiment
-from singlecellexperiment import SingleCellExperiment
+import genomicranges
 import numpy as np
-from random import random
 import pandas as pd
-import genomicranges
+import pytest
+from multiassayexperiment import MultiAssayExperiment
+from singlecellexperiment import SingleCellExperiment
 from summarizedexperiment import SummarizedExperiment
-from mudata import MuData
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 nrows = 200
@@ -38,16 +37,26 @@
         "score": range(0, 200),
         "GC": [random() for _ in range(10)] * 20,
     }
 )
 
 gr = genomicranges.fromPandas(df_gr)
 
-colData_sce = pd.DataFrame({"treatment": ["ChIP", "Input"] * 3,}, index=["sce"] * 6,)
-colData_se = pd.DataFrame({"treatment": ["ChIP", "Input"] * 3,}, index=["se"] * 6,)
+colData_sce = pd.DataFrame(
+    {
+        "treatment": ["ChIP", "Input"] * 3,
+    },
+    index=["sce"] * 6,
+)
+colData_se = pd.DataFrame(
+    {
+        "treatment": ["ChIP", "Input"] * 3,
+    },
+    index=["se"] * 6,
+)
 
 sample_map = pd.DataFrame(
     {
         "assay": ["sce", "se"] * 6,
         "primary": ["sample1", "sample2"] * 6,
         "colname": ["sce", "se"] * 6,
     }
@@ -117,21 +126,22 @@
     tse2 = SummarizedExperiment(
         assays={"counts": counts.copy()},
         rowData=df_gr.copy(),
         colData=colData_sce.copy(),
     )
 
     with pytest.raises(Exception):
-        mae = MultiAssayExperiment(
+        MultiAssayExperiment(
             experiments={"sce": tsce, "se": tse2},
             colData=sample_data,
             sampleMap=sample_map,
             metadata={"could be": "anything"},
         )
 
+
 def test_MAE_save():
     tsce = SingleCellExperiment(
         assays={"counts": counts}, rowData=df_gr, colData=colData_sce
     )
 
     tse2 = SummarizedExperiment(
         assays={"counts": counts.copy()},
@@ -148,8 +158,8 @@
 
     assert mae is not None
     assert isinstance(mae, MultiAssayExperiment)
 
     mdata = mae.toMuData()
 
     assert mdata is not None
-    assert len(mdata.mod.keys()) == 2
+    assert len(mdata.mod.keys()) == 2
```

### Comparing `MultiAssayExperiment-0.2.3/tests/test_se_io.py` & `MultiAssayExperiment-0.2.4/tests/test_io.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import anndata
 import multiassayexperiment as mae
 import numpy as np
 from anndata import AnnData
 from mudata import MuData
-import anndata
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 def test_MAE_fromH5AD():
```

### Comparing `MultiAssayExperiment-0.2.3/tests/test_se_methods.py` & `MultiAssayExperiment-0.2.4/tests/test_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import pytest
+from random import random
 
-from multiassayexperiment import MultiAssayExperiment
+import genomicranges
 import multiassayexperiment
-from singlecellexperiment import SingleCellExperiment
 import numpy as np
-from random import random
 import pandas as pd
-import genomicranges
-from summarizedexperiment import SummarizedExperiment
+import pytest
 from anndata import AnnData
+from multiassayexperiment import MultiAssayExperiment
+from singlecellexperiment import SingleCellExperiment
+from summarizedexperiment import SummarizedExperiment
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 nrows = 200
@@ -39,16 +39,26 @@
         "score": range(0, 200),
         "GC": [random() for _ in range(10)] * 20,
     }
 )
 
 gr = genomicranges.fromPandas(df_gr)
 
-colData_sce = pd.DataFrame({"treatment": ["ChIP", "Input"] * 3,}, index=["sce"] * 6,)
-colData_se = pd.DataFrame({"treatment": ["ChIP", "Input"] * 3,}, index=["se"] * 6,)
+colData_sce = pd.DataFrame(
+    {
+        "treatment": ["ChIP", "Input"] * 3,
+    },
+    index=["sce"] * 6,
+)
+colData_se = pd.DataFrame(
+    {
+        "treatment": ["ChIP", "Input"] * 3,
+    },
+    index=["se"] * 6,
+)
 
 sample_map = pd.DataFrame(
     {
         "assay": ["sce", "se"] * 6,
         "primary": ["sample1", "sample2"] * 6,
         "colname": ["sce", "se"] * 6,
     }
```

### Comparing `MultiAssayExperiment-0.2.3/tests/test_se_slices.py` & `MultiAssayExperiment-0.2.4/tests/test_slices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+import anndata
 import multiassayexperiment as mae
 import numpy as np
 from anndata import AnnData
-from mudata import MuData
-import anndata
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 np.random.seed(1)
 n, d, k = 1000, 100, 10
```

### Comparing `MultiAssayExperiment-0.2.3/tox.ini` & `MultiAssayExperiment-0.2.4/tox.ini`

 * *Files identical despite different names*

