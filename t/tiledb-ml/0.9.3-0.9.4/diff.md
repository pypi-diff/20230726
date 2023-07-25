# Comparing `tmp/tiledb-ml-0.9.3.tar.gz` & `tmp/tiledb-ml-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb-ml-0.9.3.tar", last modified: Tue Apr 18 17:28:20 2023, max compression
+gzip compressed data, was "tiledb-ml-0.9.4.tar", last modified: Tue Jul 25 23:09:09 2023, max compression
```

## Comparing `tiledb-ml-0.9.3.tar` & `tiledb-ml-0.9.4.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.359370 tiledb-ml-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.331370 tiledb-ml-0.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.339370 tiledb-ml-0.9.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.339370 tiledb-ml-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-04-18 17:28:20.359370 tiledb-ml-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.343370 tiledb-ml-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.343370 tiledb-ml-0.9.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/_static/TileDB_Logo_BlueArtboard_1@1.5x.png
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/_static/tiledb-logo_color_no_margin_@4x.png
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/tiledb.ml.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/tiledb.ml.readers.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/docs/tiledb.ml.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.335370 tiledb-ml-0.9.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.335370 tiledb-ml-0.9.3/examples/cloud/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.343370 tiledb-ml-0.9.3/examples/cloud/models/
--rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/models/pytorch_tiledb_cloud_ml_model_array.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/models/sklearn_tiledb_cloud_ml_model_array.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/models/tensorflow_tiledb_cloud_ml_model_array.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.335370 tiledb-ml-0.9.3/examples/cloud/serverless_training/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.343370 tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/data_ingestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/model_load_and_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/model_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.347370 tiledb-ml-0.9.3/examples/models/
--rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/models/pytorch_tiledb_models_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/models/sklearn_tiledb_models_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   172379 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/models/tensorflow_keras_tiledb_models_example.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.347370 tiledb-ml-0.9.3/examples/readers/
--rw-r--r--   0 runner    (1001) docker     (123)    22252 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/readers/pytorch_data_api_tiledb_dense.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23613 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/readers/pytorch_data_api_tiledb_sparse.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19529 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/readers/tensorflow_data_api_tiledb_dense.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/examples/readers/tensorflow_data_api_tiledb_sparse.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-18 17:28:20.359370 tiledb-ml-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.347370 tiledb-ml-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.351370 tiledb-ml-0.9.3/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/models/test_cloud_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/models/test_pytorch_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/models/test_sklearn_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/models/test_tensorflow_keras_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.351370 tiledb-ml-0.9.3/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/test_pytorch_collators.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/test_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/test_tensor_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tests/readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.335370 tiledb-ml-0.9.3/tiledb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.351370 tiledb-ml-0.9.3/tiledb/ml/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.355370 tiledb-ml-0.9.3/tiledb/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/_cloud_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/_file_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10500 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/models/tensorflow_keras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.355370 tiledb-ml-0.9.3/tiledb/ml/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_pytorch_collators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.359370 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/base_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/mapped.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/ragged.py
--rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/sparse_to_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-04-18 17:28:15.000000 tiledb-ml-0.9.3/tiledb/ml/readers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb/ml/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:28:20.359370 tiledb-ml-0.9.3/tiledb_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 17:28:20.000000 tiledb-ml-0.9.3/tiledb_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.558124 tiledb-ml-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.546124 tiledb-ml-0.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.550124 tiledb-ml-0.9.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.550124 tiledb-ml-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-07-25 23:09:09.558124 tiledb-ml-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9288 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.550124 tiledb-ml-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.550124 tiledb-ml-0.9.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/_static/TileDB_Logo_BlueArtboard_1@1.5x.png
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    11823 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/_static/tiledb-logo_color_no_margin_@4x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/tiledb.ml.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/tiledb.ml.readers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/docs/tiledb.ml.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.546124 tiledb-ml-0.9.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.546124 tiledb-ml-0.9.4/examples/cloud/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.550124 tiledb-ml-0.9.4/examples/cloud/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/cloud/models/pytorch_tiledb_cloud_ml_model_array.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/cloud/models/sklearn_tiledb_cloud_ml_model_array.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/cloud/models/tensorflow_tiledb_cloud_ml_model_array.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.546124 tiledb-ml-0.9.4/examples/cloud/serverless_training/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.550124 tiledb-ml-0.9.4/examples/cloud/serverless_training/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/cloud/serverless_training/pytorch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/cloud/serverless_training/pytorch/data_ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/cloud/serverless_training/pytorch/model_load_and_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/cloud/serverless_training/pytorch/model_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.550124 tiledb-ml-0.9.4/examples/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/models/pytorch_tiledb_models_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17586 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/models/sklearn_tiledb_models_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   172379 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/models/tensorflow_keras_tiledb_models_example.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.554124 tiledb-ml-0.9.4/examples/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)    22255 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/readers/pytorch_data_api_tiledb_dense.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23613 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/readers/pytorch_data_api_tiledb_sparse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19531 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/readers/tensorflow_data_api_tiledb_dense.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22020 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/examples/readers/tensorflow_data_api_tiledb_sparse.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-25 23:09:09.558124 tiledb-ml-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.554124 tiledb-ml-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.554124 tiledb-ml-0.9.4/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/models/test_cloud_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/models/test_pytorch_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/models/test_sklearn_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22755 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/models/test_tensorflow_keras_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.554124 tiledb-ml-0.9.4/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/readers/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/readers/test_pytorch_collators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/readers/test_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/readers/test_tensor_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/readers/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tests/readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.546124 tiledb-ml-0.9.4/tiledb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.554124 tiledb-ml-0.9.4/tiledb/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.554124 tiledb-ml-0.9.4/tiledb/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/models/_cloud_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/models/_file_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/models/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/models/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/models/tensorflow_keras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.554124 tiledb-ml-0.9.4/tiledb/ml/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_pytorch_collators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.554124 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/base_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/mapped.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/ragged.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/sparse_to_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-25 23:09:02.000000 tiledb-ml-0.9.4/tiledb/ml/readers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 23:09:09.000000 tiledb-ml-0.9.4/tiledb/ml/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 23:09:09.554124 tiledb-ml-0.9.4/tiledb_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10628 2023-07-25 23:09:09.000000 tiledb-ml-0.9.4/tiledb_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-25 23:09:09.000000 tiledb-ml-0.9.4/tiledb_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:09:09.000000 tiledb-ml-0.9.4/tiledb_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 23:09:09.000000 tiledb-ml-0.9.4/tiledb_ml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-25 23:09:09.000000 tiledb-ml-0.9.4/tiledb_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 23:09:09.000000 tiledb-ml-0.9.4/tiledb_ml.egg-info/top_level.txt
```

### Comparing `tiledb-ml-0.9.3/.github/ISSUE_TEMPLATE/bug_report.md` & `tiledb-ml-0.9.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/.github/ISSUE_TEMPLATE/feature_request.md` & `tiledb-ml-0.9.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/.github/workflows/ci.yml` & `tiledb-ml-0.9.4/.github/workflows/ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,36 @@
 jobs:
   build:
     runs-on: ubuntu-latest
     timeout-minutes: 60
     strategy:
       fail-fast: false
       matrix:
+        python-verison: ["3.7"]
         ml-deps:
           - "torch==1.11.0+cpu torchvision==0.12.0+cpu torchdata==0.3.0 tensorflow-cpu==2.8.1"
           - "torch==1.12.1+cpu torchvision==0.13.1+cpu torchdata==0.4.1 tensorflow-cpu==2.9.1"
           - "torch==1.13.0+cpu torchvision==0.14.0+cpu torchdata==0.5.0 tensorflow-cpu==2.10.0"
+          - "torch==1.13.0+cpu torchvision==0.14.0+cpu torchdata==0.5.0 tensorflow-cpu==2.11.0"
+        include:
+          - ml-deps: "torch==1.13.0+cpu torchvision==0.14.0+cpu torchdata==0.5.0 tensorflow-cpu==2.12.0"
+            python-version: "3.9"
+          - ml-deps: "torch==1.13.0+cpu torchvision==0.14.0+cpu torchdata==0.5.0 tensorflow-cpu==2.13.0"
+            python-version: "3.9"
 
     env:
       run_coverage: ${{ github.ref == 'refs/heads/master' }}
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
-        python-version: "3.7"
+        python-version: ${{ matrix.python-version }}
 
     - name: Cache dependencies
       uses: actions/cache@v3
       with:
         path: ~/.cache/pip
         key: ${{ runner.os }}:ml-deps=[${{ matrix.ml-deps }}]
```

### Comparing `tiledb-ml-0.9.3/.github/workflows/release.yml` & `tiledb-ml-0.9.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/CODE_OF_CONDUCT.md` & `tiledb-ml-0.9.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/CONTRIBUTING.md` & `tiledb-ml-0.9.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/LICENSE` & `tiledb-ml-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/PKG-INFO` & `tiledb-ml-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-ml
-Version: 0.9.3
+Version: 0.9.4
 Summary: Package supports all machine learning functionality for TileDB Embedded and TileDB Cloud
 Home-page: https://github.com/TileDB-Inc/TileDB-ML
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/TileDB-Inc/TileDB-ML/issues
 Project-URL: Documentation, https://docs.tiledb.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiledb-ml Version: 0.9.3 Summary: Package supports
+Metadata-Version: 2.1 Name: tiledb-ml Version: 0.9.4 Summary: Package supports
 all machine learning functionality for TileDB Embedded and TileDB Cloud Home-
 page: https://github.com/TileDB-Inc/TileDB-ML Author: TileDB, Inc. Author-
 email: help@tiledb.io License: MIT Project-URL: Bug Tracker, https://
 github.com/TileDB-Inc/TileDB-ML/issues Project-URL: Documentation, https://
 docs.tiledb.com Keywords: tiledb,ml Platform: any Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
```

### Comparing `tiledb-ml-0.9.3/README.md` & `tiledb-ml-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/docs/Makefile` & `tiledb-ml-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/docs/_static/TileDB_Logo_BlueArtboard_1@1.5x.png` & `tiledb-ml-0.9.4/docs/_static/TileDB_Logo_BlueArtboard_1@1.5x.png`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/docs/_static/favicon.ico` & `tiledb-ml-0.9.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/docs/_static/tiledb-logo_color_no_margin_@4x.png` & `tiledb-ml-0.9.4/docs/_static/tiledb-logo_color_no_margin_@4x.png`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/docs/conf.py` & `tiledb-ml-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/docs/make.bat` & `tiledb-ml-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/cloud/models/pytorch_tiledb_cloud_ml_model_array.ipynb` & `tiledb-ml-0.9.4/examples/cloud/models/pytorch_tiledb_cloud_ml_model_array.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/cloud/models/sklearn_tiledb_cloud_ml_model_array.ipynb` & `tiledb-ml-0.9.4/examples/cloud/models/sklearn_tiledb_cloud_ml_model_array.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/cloud/models/tensorflow_tiledb_cloud_ml_model_array.ipynb` & `tiledb-ml-0.9.4/examples/cloud/models/tensorflow_tiledb_cloud_ml_model_array.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/README.md` & `tiledb-ml-0.9.4/examples/cloud/serverless_training/pytorch/README.md`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/data_ingestion.py` & `tiledb-ml-0.9.4/examples/cloud/serverless_training/pytorch/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/model_load_and_predict.py` & `tiledb-ml-0.9.4/examples/cloud/serverless_training/pytorch/model_load_and_predict.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/cloud/serverless_training/pytorch/model_training.py` & `tiledb-ml-0.9.4/examples/cloud/serverless_training/pytorch/model_training.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/models/pytorch_tiledb_models_example.ipynb` & `tiledb-ml-0.9.4/examples/models/pytorch_tiledb_models_example.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/models/sklearn_tiledb_models_example.ipynb` & `tiledb-ml-0.9.4/examples/models/sklearn_tiledb_models_example.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/models/tensorflow_keras_tiledb_models_example.ipynb` & `tiledb-ml-0.9.4/examples/models/tensorflow_keras_tiledb_models_example.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/readers/pytorch_data_api_tiledb_dense.ipynb` & `tiledb-ml-0.9.4/examples/readers/pytorch_data_api_tiledb_dense.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999739583333334%*

 * *Differences: {"'cells'": '{14: {\'source\': {insert: [(31, "ctx = tiledb.Ctx({\'sm.mem.total_budget\': '*

 * *            '1024**2})\\n")], delete: [31]}}}'}*

```diff
@@ -450,15 +450,15 @@
                 "\n",
                 "def do_random_noise(img, mag=0.1):\n",
                 "    noise = np.random.uniform(-1, 1,img.shape)*mag\n",
                 "    img = img + noise\n",
                 "    img = np.clip(img,0,1)\n",
                 "    return img\n",
                 "\n",
-                "ctx = tiledb.Ctx({'sm.memory_budget': 1024**2})\n",
+                "ctx = tiledb.Ctx({'sm.mem.total_budget': 1024**2})\n",
                 "with tiledb.open(training_images, ctx=ctx) as x, tiledb.open(training_labels, ctx=ctx) as y:\n",
                 "    # Because of this issue (https://github.com/pytorch/pytorch/issues/59451#issuecomment-854883855) we avoid using multiple workers on Jupyter.\n",
                 "    train_loader = PyTorchTileDBDataLoader(\n",
                 "        ArrayParams(x, fn=do_random_noise),\n",
                 "        ArrayParams(y),\n",
                 "        batch_size=128,\n",
                 "        num_workers=0,\n",
```

### Comparing `tiledb-ml-0.9.3/examples/readers/pytorch_data_api_tiledb_sparse.ipynb` & `tiledb-ml-0.9.4/examples/readers/pytorch_data_api_tiledb_sparse.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/examples/readers/tensorflow_data_api_tiledb_dense.ipynb` & `tiledb-ml-0.9.4/examples/readers/tensorflow_data_api_tiledb_dense.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998949579831933%*

 * *Differences: {"'cells'": '{15: {\'source\': {insert: [(4, "ctx = tiledb.Ctx({\'sm.mem.total_budget\': '*

 * *            '1024**2})\\n")], delete: [4]}}}'}*

```diff
@@ -332,15 +332,15 @@
                 }
             ],
             "source": [
                 "from tiledb.ml.readers.tensorflow import TensorflowTileDBDataset, ArrayParams\n",
                 "\n",
                 "model = create_model()\n",
                 "\n",
-                "ctx = tiledb.Ctx({'sm.memory_budget': 1024**2})\n",
+                "ctx = tiledb.Ctx({'sm.mem.total_budget': 1024**2})\n",
                 "with tiledb.open(training_images, ctx=ctx) as x, tiledb.open(training_labels, ctx=ctx) as y:\n",
                 "    tiledb_dataset = TensorflowTileDBDataset(\n",
                 "        ArrayParams(array=x, fields=['features']),\n",
                 "        ArrayParams(array=y, fields=['features']),\n",
                 "        num_workers=2 if os.cpu_count() > 2 else 0,\n",
                 "    )\n",
                 "    tiledb_dataset = tiledb_dataset.batch(64).shuffle(128)\n",
```

### Comparing `tiledb-ml-0.9.3/examples/readers/tensorflow_data_api_tiledb_sparse.ipynb` & `tiledb-ml-0.9.4/examples/readers/tensorflow_data_api_tiledb_sparse.ipynb`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/setup.cfg` & `tiledb-ml-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/setup.py` & `tiledb-ml-0.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tests/models/test_cloud_utils.py` & `tiledb-ml-0.9.4/tests/models/test_cloud_utils.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tests/models/test_pytorch_models.py` & `tiledb-ml-0.9.4/tests/models/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tests/models/test_sklearn_models.py` & `tiledb-ml-0.9.4/tests/models/test_sklearn_models.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tests/models/test_tensorflow_keras_models.py` & `tiledb-ml-0.9.4/tests/models/test_tensorflow_keras_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,24 @@
 
 try:
     from keras.testing_infra.test_utils import (
         get_small_functional_mlp,
         get_small_sequential_mlp,
     )
 except ImportError:
-    from keras.testing_utils import get_small_functional_mlp, get_small_sequential_mlp
+    try:
+        from keras.testing_utils import (
+            get_small_functional_mlp,
+            get_small_sequential_mlp,
+        )
+    except ImportError:
+        from keras.src.testing_infra.test_utils import (
+            get_small_functional_mlp,
+            get_small_sequential_mlp,
+        )
 
 # Suppress all Tensorflow messages
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "3"
 
 batch_get_value = tf.keras.backend.batch_get_value
 
 
@@ -162,16 +171,28 @@
 
         tiledb_model_obj.save(include_optimizer=True if optimizer else False)
         loaded_model = tiledb_model_obj.load(compile_model=True if optimizer else False)
 
         data = np.random.rand(100, 3)
 
         if optimizer:
-            model_opt_weights = batch_get_value(model.optimizer.weights)
-            loaded_opt_weights = batch_get_value(loaded_model.optimizer.weights)
+            if hasattr(model.optimizer, "weights"):
+                model_opt_weights = tf.keras.backend.batch_get_value(
+                    model.optimizer.weights
+                )
+            else:
+                model_opt_weights = [var.numpy() for var in model.optimizer.variables()]
+            if hasattr(loaded_model.optimizer, "weights"):
+                loaded_opt_weights = tf.keras.backend.batch_get_value(
+                    loaded_model.optimizer.weights
+                )
+            else:
+                loaded_opt_weights = [
+                    var.numpy() for var in loaded_model.optimizer.variables()
+                ]
 
             # Assert optimizer weights are equal
             for weight_model, weight_loaded_model in zip(
                 model_opt_weights, loaded_opt_weights
             ):
                 np.testing.assert_array_equal(weight_model, weight_loaded_model)
 
@@ -205,16 +226,28 @@
         model.compile(loss=loss, optimizer=optimizer, metrics=[metrics])
 
         tiledb_uri = os.path.join(tmpdir, "model_array")
         tiledb_model_obj = TensorflowKerasTileDBModel(uri=tiledb_uri, model=model)
         tiledb_model_obj.save(include_optimizer=True)
         loaded_model = tiledb_model_obj.load(compile_model=True)
 
-        model_opt_weights = batch_get_value(model.optimizer.weights)
-        loaded_opt_weights = batch_get_value(loaded_model.optimizer.weights)
+        if hasattr(model.optimizer, "weights"):
+            model_opt_weights = tf.keras.backend.batch_get_value(
+                model.optimizer.weights
+            )
+        else:
+            model_opt_weights = [var.numpy() for var in model.optimizer.variables()]
+        if hasattr(loaded_model.optimizer, "weights"):
+            loaded_opt_weights = tf.keras.backend.batch_get_value(
+                loaded_model.optimizer.weights
+            )
+        else:
+            loaded_opt_weights = [
+                var.numpy() for var in loaded_model.optimizer.variables()
+            ]
 
         # Assert optimizer weights are equal
         for weight_model, weight_loaded_model in zip(
             model_opt_weights, loaded_opt_weights
         ):
             np.testing.assert_array_equal(weight_model, weight_loaded_model)
 
@@ -256,16 +289,28 @@
         model.compile(loss=loss, optimizer=optimizer, metrics=[metrics])
 
         tiledb_uri = os.path.join(tmpdir, "model_array")
         tiledb_model_obj = TensorflowKerasTileDBModel(uri=tiledb_uri, model=model)
         tiledb_model_obj.save(include_optimizer=True)
         loaded_model = tiledb_model_obj.load(compile_model=True)
 
-        model_opt_weights = batch_get_value(model.optimizer.weights)
-        loaded_opt_weights = batch_get_value(loaded_model.optimizer.weights)
+        if hasattr(model.optimizer, "weights"):
+            model_opt_weights = tf.keras.backend.batch_get_value(
+                model.optimizer.weights
+            )
+        else:
+            model_opt_weights = [var.numpy() for var in model.optimizer.variables()]
+        if hasattr(loaded_model.optimizer, "weights"):
+            loaded_opt_weights = tf.keras.backend.batch_get_value(
+                loaded_model.optimizer.weights
+            )
+        else:
+            loaded_opt_weights = [
+                var.numpy() for var in loaded_model.optimizer.variables()
+            ]
 
         # Assert optimizer weights are equal
         for weight_model, weight_loaded_model in zip(
             model_opt_weights, loaded_opt_weights
         ):
             np.testing.assert_array_equal(weight_model, weight_loaded_model)
 
@@ -273,15 +318,15 @@
         timesteps = 1
 
         values_a = np.arange(10, dtype=np.float32)
         indices_a = np.zeros((10, 3), dtype=np.int64)
         indices_a[:, 0] = np.arange(10)
         inputs_a = tf.SparseTensor(indices_a, values_a, (batch_size, timesteps, 1))
 
-        values_b = np.zeros(10, dtype=np.str)
+        values_b = np.zeros(10, dtype=str)
         indices_b = np.zeros((10, 3), dtype=np.int64)
         indices_b[:, 0] = np.arange(10)
         inputs_b = tf.SparseTensor(indices_b, values_b, (batch_size, timesteps, 1))
 
         # Assert model predictions are equal
         np.testing.assert_array_equal(
             loaded_model.predict({"a": inputs_a, "b": inputs_b}, steps=1),
@@ -306,15 +351,15 @@
         data_x = np.random.normal(size=(32, 4))
         data_y = np.random.randint(0, 3, size=32)
         model.train_on_batch(data_x, data_y)
 
         tiledb_uri = os.path.join(tmpdir, "model_array")
         tiledb_model_obj = TensorflowKerasTileDBModel(uri=tiledb_uri, model=model)
         tiledb_model_obj.save(include_optimizer=True)
-        loaded_model = tiledb_model_obj.load(compile_model=True)
+        loaded_model = tiledb_model_obj.load(compile_model=True, safe_mode=False)
 
         # Assert all evaluation results are the same.
         assert all(
             [
                 a == pytest.approx(b, 1e-9)
                 for a, b in zip(
                     model.evaluate(data_x, data_y),
```

### Comparing `tiledb-ml-0.9.3/tests/readers/test_pytorch.py` & `tiledb-ml-0.9.4/tests/readers/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tests/readers/test_pytorch_collators.py` & `tiledb-ml-0.9.4/tests/readers/test_pytorch_collators.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tests/readers/test_ranges.py` & `tiledb-ml-0.9.4/tests/readers/test_ranges.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tests/readers/test_tensor_schema.py` & `tiledb-ml-0.9.4/tests/readers/test_tensor_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         ("d1", 700_000, {"d1": slice(-10, None), "d0": slice(1000, None)}),
     ],
 )
 @parametrize_fields("d0", "d1", "af8", "af4", "au1")
 def test_max_partition_weight_dense(
     dense_uri, fields, key_dim, memory_budget, dim_selectors
 ):
-    config = {"py.max_incomplete_retries": 0, "sm.memory_budget": memory_budget}
+    config = {"py.max_incomplete_retries": 0, "sm.mem.total_budget": memory_budget}
     with tiledb.open(dense_uri, config=config) as array:
         _test_max_partition_weight(array, fields, key_dim, dim_selectors)
 
 
 @pytest.mark.parametrize(
     "key_dim,memory_budget,dim_selectors",
     [
```

### Comparing `tiledb-ml-0.9.3/tests/readers/test_tensorflow.py` & `tiledb-ml-0.9.4/tests/readers/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tests/readers/utils.py` & `tiledb-ml-0.9.4/tests/readers/utils.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/models/_base.py` & `tiledb-ml-0.9.4/tiledb/ml/models/_base.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/models/_cloud_utils.py` & `tiledb-ml-0.9.4/tiledb/ml/models/_cloud_utils.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/models/_file_properties.py` & `tiledb-ml-0.9.4/tiledb/ml/models/_file_properties.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/models/pytorch.py` & `tiledb-ml-0.9.4/tiledb/ml/models/pytorch.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/models/sklearn.py` & `tiledb-ml-0.9.4/tiledb/ml/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/models/tensorflow_keras.py` & `tiledb-ml-0.9.4/tiledb/ml/models/tensorflow_keras.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,20 +11,47 @@
 import keras
 import tensorflow as tf
 
 import tiledb
 
 from ._base import Meta, TileDBArtifact, Timestamp
 
-SharedObjectLoadingScope = keras.utils.generic_utils.SharedObjectLoadingScope
-FunctionalOrSequential = (keras.models.Functional, keras.models.Sequential)
-TFOptimizer = keras.optimizers.TFOptimizer
-get_json_type = keras.saving.saved_model.json_utils.get_json_type
-preprocess_weights_for_loading = keras.saving.hdf5_format.preprocess_weights_for_loading
-saving_utils = keras.saving.saving_utils
+keras_major, keras_minor, keras_patch = keras.__version__.split(".")
+FunctionalOrSequential = keras.models.Sequential
+# Handle keras <=v2.10
+if int(keras_major) <= 2 and int(keras_minor) <= 10:
+    FunctionalOrSequential = (keras.models.Functional, keras.models.Sequential)
+    TFOptimizer = keras.optimizers.TFOptimizer
+    get_json_type = keras.saving.saved_model.json_utils.get_json_type
+    preprocess_weights_for_loading = (
+        keras.saving.hdf5_format.preprocess_weights_for_loading
+    )
+    saving_utils = keras.saving.saving_utils
+# Handle keras >=v2.11
+elif int(keras_major) <= 2 and int(keras_minor) <= 12:
+    FunctionalOrSequential = (keras.models.Functional, keras.models.Sequential)
+    TFOptimizer = tf.keras.optimizers.legacy.Optimizer
+    get_json_type = keras.saving.legacy.saved_model.json_utils.get_json_type
+    preprocess_weights_for_loading = (
+        keras.saving.legacy.hdf5_format.preprocess_weights_for_loading
+    )
+    saving_utils = keras.saving.legacy.saving_utils
+else:
+    from keras.src.saving.serialization_lib import SafeModeScope
+
+    FunctionalOrSequential = (
+        keras.src.engine.functional.Functional,
+        keras.src.engine.sequential.Sequential,
+    )
+    TFOptimizer = tf.keras.optimizers.legacy.Optimizer
+    get_json_type = keras.src.saving.legacy.saved_model.json_utils.get_json_type
+    preprocess_weights_for_loading = (
+        keras.src.saving.legacy.hdf5_format.preprocess_weights_for_loading
+    )
+    saving_utils = keras.src.saving.legacy.saving_utils
 
 
 class TensorflowKerasTileDBModel(TileDBArtifact[tf.keras.Model]):
     """
     Class that implements all functionality needed to save Tensorflow models as
     TileDB arrays and load Tensorflow models from TileDB arrays.
     """
@@ -56,15 +83,15 @@
         :param callbacks: Callbacks list to store. At the moment only Tensorboard callback is supported.
         """
         if self.artifact is None:
             raise RuntimeError("Model is not initialized")
 
         if not isinstance(self.artifact, FunctionalOrSequential):
             raise RuntimeError(
-                "Subclassed Models (Custom Layers) not supported at the moment."
+                f"Subclassed Models (Custom Layers) for {type(self.artifact)} not supported at the moment."
             )
 
         # Used in this format only when model is Functional or Sequential
         model_weights = pickle.dumps(self.artifact.get_weights(), protocol=4)
 
         # Serialize model optimizer
         if include_optimizer:
@@ -106,14 +133,15 @@
         self,
         *,
         timestamp: Optional[Timestamp] = None,
         compile_model: bool = False,
         custom_objects: Optional[Mapping[str, Any]] = None,
         input_shape: Optional[Tuple[int, ...]] = None,
         callback: bool = False,
+        safe_mode: Optional[bool] = None,
     ) -> tf.keras.Model:
         """
         Load switch, i.e, decide between __load (TileDB-ML<=0.8.0) or __load_v2 (TileDB-ML>0.8.0).
 
         :param callback: Boolean variable if True will store callback data into saved directory. At the moment supports
         only Tensorboard callback.
         :param timestamp: Range of timestamps to load fragments of the array which live
@@ -126,15 +154,15 @@
         """
         with tiledb.open(self.uri, ctx=self.ctx, timestamp=timestamp) as model_array:
             if self._use_legacy_schema(model_array):
                 return self.__load_legacy(
                     model_array, compile_model, callback, custom_objects
                 )
             else:
-                return self.__load(model_array, compile_model, callback)
+                return self.__load(model_array, compile_model, callback, safe_mode)
 
     def __load_legacy(
         self,
         model_array: tiledb.Array,
         compile_model: bool,
         callback: bool,
         custom_objects: Optional[Mapping[str, Any]],
@@ -197,21 +225,33 @@
                         ) as f:
                             f.write(file_bytes)
             except FileNotFoundError:
                 print(f"Array {self.uri}-tensorboard does not exist")
         return model
 
     def __load(
-        self, model_array: tiledb.Array, compile_model: bool, callback: bool
+        self,
+        model_array: tiledb.Array,
+        compile_model: bool,
+        callback: bool,
+        safe_mode: Optional[bool],
     ) -> tf.keras.Model:
         model_config = json.loads(model_array.meta["model_config"])
         model_class = model_config["class_name"]
 
         cls = tf.keras.Sequential if model_class == "Sequential" else tf.keras.Model
-        model = cls.from_config(model_config["config"])
+
+        if int(keras_major) <= 2 and int(keras_minor) >= 13:
+            if safe_mode is not None:
+                with SafeModeScope(safe_mode=safe_mode):
+                    model = cls.from_config(model_config["config"])
+            else:
+                model = cls.from_config(model_config["config"])
+        else:
+            model = cls.from_config(model_config["config"])
         model_weights = self._get_model_param(model_array, "model")
         model.set_weights(model_weights)
 
         if compile_model:
             training_config = json.loads(model_array.meta["training_config"])
 
             # Compile model.
@@ -263,10 +303,13 @@
     def _serialize_optimizer_weights(
         self,
     ) -> bytes:
         """Serialize optimizer weights."""
         assert self.artifact
         optimizer = self.artifact.optimizer
         if optimizer and not isinstance(optimizer, TFOptimizer):
-            optimizer_weights = tf.keras.backend.batch_get_value(optimizer.weights)
+            if hasattr(optimizer, "weights"):
+                optimizer_weights = tf.keras.backend.batch_get_value(optimizer.weights)
+            else:
+                optimizer_weights = [var.numpy() for var in optimizer.variables()]
             return pickle.dumps(optimizer_weights, protocol=4)
         return b""
```

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_pytorch_collators.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_pytorch_collators.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/__init__.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/base.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     @abstractmethod
     def max_partition_weight(self) -> int:
         """
         Determine the maximum partition that can be read without incomplete retries.
 
         What constitutes weight of a partition depends on the array type:
         - For dense arrays, it is the number of unique keys (= number of "rows").
-          It depends on the `sm.memory_budget` config parameter.
+          It depends on the `sm.mem.total_budget` config parameter.
         - For sparse arrays, it is the number of non-empty cells.
           It depends on the `py.init_buffer_bytes` config parameter.
         """
 
     @abstractmethod
     def iter_tensors(
         self, key_ranges: Iterable[InclusiveRange[Any, int]]
```

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/base_sparse.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/base_sparse.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/dense.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/dense.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                 # Move key_dim_index axes first
                 for field, array in field_arrays.items():
                     field_arrays[field] = np.moveaxis(array, key_dim_index, 0)
             yield get_data(field_arrays)
 
     @property
     def max_partition_weight(self) -> int:
-        memory_budget = int(self._array._ctx_().config()["sm.memory_budget"])
+        memory_budget = int(self._array._ctx_().config()["sm.mem.total_budget"])
 
         # The memory budget should be large enough to read the cells of the largest field
         bytes_per_cell = max(dtype.itemsize for dtype in self.field_dtypes)
 
         # We want to be reading tiles following the tile extents along each dimension.
         # The number of cells for each such tile is the product of all tile extents.
         dim_tiles = [self._array.dim(dim).tile for dim in self._all_dims]
```

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/mapped.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/mapped.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/query.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/query.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/ragged.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/ragged.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/ranges.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/ranges.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/sparse.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/sparse.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/_tensor_schema/sparse_to_dense.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/_tensor_schema/sparse_to_dense.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/pytorch.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/pytorch.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/tensorflow.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb/ml/readers/types.py` & `tiledb-ml-0.9.4/tiledb/ml/readers/types.py`

 * *Files identical despite different names*

### Comparing `tiledb-ml-0.9.3/tiledb_ml.egg-info/PKG-INFO` & `tiledb-ml-0.9.4/tiledb_ml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-ml
-Version: 0.9.3
+Version: 0.9.4
 Summary: Package supports all machine learning functionality for TileDB Embedded and TileDB Cloud
 Home-page: https://github.com/TileDB-Inc/TileDB-ML
 Author: TileDB, Inc.
 Author-email: help@tiledb.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/TileDB-Inc/TileDB-ML/issues
 Project-URL: Documentation, https://docs.tiledb.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tiledb-ml Version: 0.9.3 Summary: Package supports
+Metadata-Version: 2.1 Name: tiledb-ml Version: 0.9.4 Summary: Package supports
 all machine learning functionality for TileDB Embedded and TileDB Cloud Home-
 page: https://github.com/TileDB-Inc/TileDB-ML Author: TileDB, Inc. Author-
 email: help@tiledb.io License: MIT Project-URL: Bug Tracker, https://
 github.com/TileDB-Inc/TileDB-ML/issues Project-URL: Documentation, https://
 docs.tiledb.com Keywords: tiledb,ml Platform: any Classifier: Development
 Status :: 4 - Beta Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
```

### Comparing `tiledb-ml-0.9.3/tiledb_ml.egg-info/SOURCES.txt` & `tiledb-ml-0.9.4/tiledb_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

