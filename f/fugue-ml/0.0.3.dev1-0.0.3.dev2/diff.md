# Comparing `tmp/fugue-ml-0.0.3.dev1.tar.gz` & `tmp/fugue-ml-0.0.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fugue-ml-0.0.3.dev1.tar", last modified: Tue Jul 18 07:29:40 2023, max compression
+gzip compressed data, was "fugue-ml-0.0.3.dev2.tar", last modified: Wed Jul 26 07:49:20 2023, max compression
```

## Comparing `fugue-ml-0.0.3.dev1.tar` & `fugue-ml-0.0.3.dev2.tar`

### file list

```diff
@@ -1,90 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.771984 fugue-ml-0.0.3.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-18 07:29:40.771984 fugue-ml-0.0.3.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.755984 fugue-ml-0.0.3.dev1/fugue_ml/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.755984 fugue-ml-0.0.3.dev1/fugue_ml/ann/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/ann/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/ann/indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.755984 fugue-ml-0.0.3.dev1/fugue_ml/ann/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/ann/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/ann/integrations/nmslib.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/api.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/embedding/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/embedding/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/embedding/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/sentence_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/cred.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/knn/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/knn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/knn/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/knn/brute_force.py
--rw-r--r--   0 runner    (1001) docker     (123)    19100 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/knn/indexer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/test/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/test/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/test/embedding/cache_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/fugue_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/iter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.763984 fugue-ml-0.0.3.dev1/fugue_ml/utils/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/numpy/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/params.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml/utils/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.755984 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 07:29:40.000000 fugue-ml-0.0.3.dev1/fugue_ml.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.767984 fugue-ml-0.0.3.dev1/fugue_ml_version/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/fugue_ml_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-18 07:29:40.771984 fugue-ml-0.0.3.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.755984 fugue-ml-0.0.3.dev1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.767984 fugue-ml-0.0.3.dev1/tests/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/embedding/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/embedding/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/embedding/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/embedding/test_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.767984 fugue-ml-0.0.3.dev1/tests/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.767984 fugue-ml-0.0.3.dev1/tests/knn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.767984 fugue-ml-0.0.3.dev1/tests/knn/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/integrations/test_brute_force.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/test_api_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/knn/test_indexer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.771984 fugue-ml-0.0.3.dev1/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:29:40.771984 fugue-ml-0.0.3.dev1/tests/utils/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/numpy/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/test_fugue_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-18 07:25:42.000000 fugue-ml-0.0.3.dev1/tests/utils/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.838749 fugue-ml-0.0.3.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-26 07:49:20.838749 fugue-ml-0.0.3.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.822749 fugue-ml-0.0.3.dev2/fugue_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.822749 fugue-ml-0.0.3.dev2/fugue_ml/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/embedding/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/embedding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/embedding/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.826749 fugue-ml-0.0.3.dev2/fugue_ml/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.826749 fugue-ml-0.0.3.dev2/fugue_ml/integrations/hnswlib/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/hnswlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/hnswlib/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/hnswlib/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.826749 fugue-ml-0.0.3.dev2/fugue_ml/integrations/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/huggingface/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/huggingface/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/huggingface/sentence_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.826749 fugue-ml-0.0.3.dev2/fugue_ml/integrations/openai/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/openai/cred.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/openai/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/integrations/openai/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.826749 fugue-ml-0.0.3.dev2/fugue_ml/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/knn/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/knn/brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27319 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/knn/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.830749 fugue-ml-0.0.3.dev2/fugue_ml/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.830749 fugue-ml-0.0.3.dev2/fugue_ml/testing/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/testing/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/testing/embedding/cache_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.830749 fugue-ml-0.0.3.dev2/fugue_ml/testing/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/testing/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/testing/knn/local_indexer_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.830749 fugue-ml-0.0.3.dev2/fugue_ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/utils/fugue_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/utils/iter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.830749 fugue-ml-0.0.3.dev2/fugue_ml/utils/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/utils/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/utils/numpy/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/utils/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml/utils/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.822749 fugue-ml-0.0.3.dev2/fugue_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-26 07:49:20.000000 fugue-ml-0.0.3.dev2/fugue_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-07-26 07:49:20.000000 fugue-ml-0.0.3.dev2/fugue_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 07:49:20.000000 fugue-ml-0.0.3.dev2/fugue_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-26 07:49:20.000000 fugue-ml-0.0.3.dev2/fugue_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-26 07:49:20.000000 fugue-ml-0.0.3.dev2/fugue_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-26 07:49:20.000000 fugue-ml-0.0.3.dev2/fugue_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.830749 fugue-ml-0.0.3.dev2/fugue_ml_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/fugue_ml_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-26 07:49:20.838749 fugue-ml-0.0.3.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.822749 fugue-ml-0.0.3.dev2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.834749 fugue-ml-0.0.3.dev2/tests/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/embedding/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/embedding/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/embedding/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/embedding/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.834749 fugue-ml-0.0.3.dev2/tests/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.834749 fugue-ml-0.0.3.dev2/tests/integrations/hnswlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/integrations/hnswlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/integrations/hnswlib/test_indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.834749 fugue-ml-0.0.3.dev2/tests/knn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/knn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/knn/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/knn/test_api_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/knn/test_brute_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/knn/test_indexer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.834749 fugue-ml-0.0.3.dev2/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 07:49:20.838749 fugue-ml-0.0.3.dev2/tests/utils/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/utils/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/utils/numpy/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/utils/test_fugue_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/utils/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/utils/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-26 07:44:51.000000 fugue-ml-0.0.3.dev2/tests/utils/test_schema.py
```

### Comparing `fugue-ml-0.0.3.dev1/LICENSE` & `fugue-ml-0.0.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/PKG-INFO` & `fugue-ml-0.0.3.dev2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue-ml
-Version: 0.0.3.dev1
+Version: 0.0.3.dev2
 Summary: Fugue ML
 Home-page: http://github.com/fugue-project/fugue-ml
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue Machine Learning Library
         
@@ -22,7 +22,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: openai
 Provides-Extra: huggingface
+Provides-Extra: hnswlib
```

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/embedding/api.py` & `fugue-ml-0.0.3.dev2/fugue_ml/embedding/api.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/embedding/base.py` & `fugue-ml-0.0.3.dev2/fugue_ml/embedding/base.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/embedding/cache.py` & `fugue-ml-0.0.3.dev2/fugue_ml/embedding/cache.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/_utils.py` & `fugue-ml-0.0.3.dev2/fugue_ml/integrations/huggingface/_utils.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/integrations/huggingface/sentence_embedding.py` & `fugue-ml-0.0.3.dev2/fugue_ml/integrations/huggingface/sentence_embedding.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/cred.py` & `fugue-ml-0.0.3.dev2/fugue_ml/integrations/openai/cred.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/embedding.py` & `fugue-ml-0.0.3.dev2/fugue_ml/integrations/openai/embedding.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/integrations/openai/registry.py` & `fugue-ml-0.0.3.dev2/fugue_ml/integrations/openai/registry.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/knn/brute_force.py` & `fugue-ml-0.0.3.dev2/fugue_ml/knn/brute_force.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,44 @@
-from typing import Any, Tuple
+from typing import Any, Optional, Tuple
 
 import numpy as np
+import threadpoolctl
 
 from fugue_ml.utils.numpy.distance import knn as compute_knn
 
-from .indexer import KNNLocalIndexer, register_knn_indexer
+from .indexer import LocalKNNIndexer, register_knn_indexer
 
 
 @register_knn_indexer("brute_force")
-class BruteForceKNNIndexer(KNNLocalIndexer):
+class BruteForceKNNIndexer(LocalKNNIndexer):
     """Brute force KNN indexer. It is implemented using Numoy and
     It produces exact (perfect) k nearest neighbors.
     """
 
-    def build_local(self, arr: np.ndarray, **kwargs: Any) -> None:
+    def build_local(
+        self, arr: np.ndarray, worker_nthreads: Optional[int], **kwargs: Any
+    ) -> None:
         self._index = arr
 
     def can_broadcast(self, size_limit: int) -> bool:
         return (
             self._index.nbytes + self._metadata_df.memory_usage(deep=True).sum()
             < size_limit
         )
 
     def search_local(
-        self, queries: np.ndarray, k: int, **kwargs: Any
+        self,
+        query: np.ndarray,
+        k: int,
+        sort_output: bool,
+        worker_nthreads: Optional[int],
+        **kwargs: Any
     ) -> Tuple[np.ndarray, np.ndarray]:
-        return compute_knn(index=self._index, queries=queries, metric=self.metric, k=k)
+        self._dim = query.shape[1]
+        with threadpoolctl.threadpool_limits(limits=worker_nthreads):
+            return compute_knn(
+                index=self._index,
+                query=query,
+                metric=self.metric,
+                k=k,
+                sort_output=sort_output,
+            )
```

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/knn/indexer.py` & `fugue-ml-0.0.3.dev2/fugue_ml/knn/indexer.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Type, Union
 from uuid import uuid4
 
 import fsspec
 import fugue.api as fa
 import numpy as np
 import pandas as pd
-from fugue import AnyDataFrame
+import threadpoolctl
+from fugue import AnyDataFrame, DataFrame
 from triad import Schema, assert_or_throw
 from triad.utils.batch_reslicers import PandasBatchReslicer
 from triad.utils.convert import to_size
 from triad.utils.threading import SerializableRLock
-from fugue_ml.utils.fugue_ext import (
-    deterministic_shard,
-    replicate,
-    deterministic_shard_and_replicate,
-)
+
+from fugue_ml.utils.fugue_ext import deterministic_shard
 from fugue_ml.utils.io import unzip_to_temp, zip_temp
 from fugue_ml.utils.registry import fugue_ml_plugin
 from fugue_ml.utils.schema import is_vec_col
 
+_COLUMN_PREFIX = "_fugue_ml_knn"
 _INDEXERS: Dict[str, Type["KNNIndexer"]] = {}
 _INDEXER_ATTR = "_indexer_name"
-_INDEXER_BLOB_COLUMN_NAME = "_indexer_blob"
-_INDEXER_REPLICATES_COLUMN_NAME = "_indexer_rep"
-_INDEXER_SHARD_COLUMN_NAME = "_indexer_shard"
-_TEMP_DIST_COL = "_temp_dist"
+_INDEXER_BLOB_COLUMN_NAME = _COLUMN_PREFIX + "_indexer_blob"
+_INDEXER_METADATA_BLOB_COLUMN_NAME = _COLUMN_PREFIX + "_indexer_metadata_blob"
+_INDEXER_SHARD_COLUMN_NAME = _COLUMN_PREFIX + "_indexer_shard"
+_QUERY_SHARDS_COLUMN_NAME = _COLUMN_PREFIX + "_query_shard"
+_QUERY_BLOB_COLUMN_NAME = _COLUMN_PREFIX + "_query_blob"
+_QUERY_DEDUP_COLUMN_NAME = _COLUMN_PREFIX + "_query_dedup"
+_TEMP_DIST_COL = _COLUMN_PREFIX + "_temp_dist"
 
 
 def register_knn_indexer(name: str) -> Callable:
     def deco(cls: Type) -> Type:
         assert_or_throw(
             issubclass(cls, KNNIndexer),
             TypeError(f"{cls} is not a subtype of KNNIndexer"),
@@ -64,22 +66,30 @@
 
 
 class KNNIndexer(ABC):
     def __init__(self, metric: str):
         self.metric = metric
 
     @abstractmethod  # pragma: no cover
-    def build(self, index: AnyDataFrame, vec_col: str, **kwargs: Any) -> "KNNIndexer":
+    def build(
+        self,
+        index: AnyDataFrame,
+        vec_col: str,
+        worker_nthreads: Optional[int] = None,
+        **kwargs: Any,
+    ) -> "KNNIndexer":
         raise NotImplementedError
 
     @abstractmethod  # pragma: no cover
     def search_local(
         self,
-        queries: np.ndarray,
+        query: np.ndarray,
         k: int,
+        sort_output: bool,
+        worker_nthreads: Optional[int],
         **kwargs: Any,
     ) -> Tuple[np.ndarray, np.ndarray]:
         raise NotImplementedError
 
     @abstractmethod  # pragma: no cover
     def can_broadcast(self, size_limit: int) -> bool:
         raise NotImplementedError
@@ -88,14 +98,18 @@
     def get_metadata_df(self) -> pd.DataFrame:
         raise NotImplementedError
 
     @abstractmethod  # pragma: no cover
     def get_metadata_schema(self) -> Schema:
         raise NotImplementedError
 
+    @abstractmethod  # pragma: no cover
+    def get_dim(self) -> int:
+        raise NotImplementedError
+
     def save(self, path: str) -> None:
         with zip_temp(path) as tmpdir:
             fs, path = fsspec.core.url_to_fs(tmpdir)
             fs.write_bytes(
                 os.path.join(path, "indexer_type.bin"), pickle.dumps(self.__class__)
             )
             params = dict(self.__dict__)
@@ -110,57 +124,63 @@
         return
 
     def load_special_params(self, folder: str) -> Dict[str, Any]:
         return {}
 
     def search(
         self,
-        queries: AnyDataFrame,
+        query: AnyDataFrame,
         k: int,
         vec_col: str,
         dist_col: Optional[str] = None,
         rank_col: Optional[str] = None,
-        index_cache_mem_limit: Any = "1g",
-        queries_chunk_mem_limit: Any = "100m",
-        queries_chunk_row_limit: int = 0,
-        broadcast_limit: Any = "500m",
         drop_vec_col: bool = True,
-        temp_file: Optional[str] = None,
-        index_replicates: Optional[int] = None,
+        index_cache_mem_limit: Any = "1g",
+        index_broadcast_threshold: Any = "500m",
+        query_shards: Optional[int] = None,
+        query_preprocess_mode: str = "direct",
+        query_chunk_mem_limit: Any = "100m",
+        query_chunk_row_limit: int = 0,
+        temp_path: Optional[str] = None,
+        worker_nthreads: Optional[int] = None,
         **kwargs: Any,
     ) -> AnyDataFrame:
         output_schema = self._construct_schema(
-            fa.get_schema(queries),
+            fa.get_schema(query),
             vec_col=vec_col,
             dist_col=dist_col,
             rank_col=rank_col,
             drop_vec_col=drop_vec_col,
         )
-        indexer_ser = _KNNIndexerSerializer(self, to_size(broadcast_limit), temp_file)
+        indexer_ser = _KNNIndexerSerializer(
+            self, to_size(index_broadcast_threshold), temp_path
+        )
 
         def _wrapper(dfs: Iterable[pd.DataFrame]) -> Iterable[pd.DataFrame]:
             indexer = indexer_ser.get_instance(cache_size=index_cache_mem_limit)
             reslicer = PandasBatchReslicer(
-                row_limit=queries_chunk_row_limit, size_limit=queries_chunk_mem_limit
+                row_limit=query_chunk_row_limit, size_limit=query_chunk_mem_limit
             )
             for df in reslicer.reslice(dfs):
                 for res in _search_pd_df(
                     indexer=indexer,
                     df=df,
                     k=k,
                     vec_col=vec_col,
                     dist_col=dist_col,
                     rank_col=rank_col,
                     drop_vec_col=drop_vec_col,
+                    sort_output=rank_col is not None,
+                    worker_nthreads=worker_nthreads,
                     **kwargs,
                 ):
                     yield res[output_schema.names]
 
         return fa.transform(
-            queries, _wrapper, schema=output_schema, partition=index_replicates
+            query, _wrapper, schema=output_schema, partition=query_shards
         )
 
     def get_np_arr(self, df: pd.DataFrame, vec_col: str) -> np.array:
         return np.array(list(df[vec_col]))
 
     def _construct_schema(
         self,
@@ -179,41 +199,55 @@
         if rank_col is not None:
             schema = schema + (rank_col, int)
         if drop_vec_col:
             schema = schema.exclude(vec_col)
         return schema
 
 
-class KNNLocalIndexer(KNNIndexer):
-    def build(self, index: AnyDataFrame, vec_col: str, **kwargs: Any) -> "KNNIndexer":
-        pdf = fa.as_pandas(index).reset_index(drop=True)
-        self._metadata_df = pdf.drop(columns=[vec_col])
-        self._metadata_schema = fa.get_schema(index) - vec_col
-        self.build_local(self.get_np_arr(pdf, vec_col=vec_col), **kwargs)
-        return self
+class LocalKNNIndexer(KNNIndexer):
+    def build(
+        self,
+        index: AnyDataFrame,
+        vec_col: str,
+        worker_nthreads: Optional[int] = None,
+        **kwargs: Any,
+    ) -> "KNNIndexer":
+        with threadpoolctl.threadpool_limits(limits=worker_nthreads):
+            pdf = fa.as_pandas(index).reset_index(drop=True)
+            self._metadata_df = pdf.drop(columns=[vec_col])
+            self._metadata_schema = fa.get_schema(index) - vec_col
+            arr = self.get_np_arr(pdf, vec_col=vec_col)
+            self._dim = arr.shape[1]
+            self.build_local(arr, worker_nthreads=worker_nthreads, **kwargs)
+            return self
 
     def get_metadata_df(self) -> pd.DataFrame:
         return self._metadata_df
 
     def get_metadata_schema(self) -> Schema:
         return self._metadata_schema
 
+    def get_dim(self) -> int:
+        return self._dim
+
     @abstractmethod  # pragma: no cover
-    def build_local(self, arr: np.ndarray, **kwargs: Any) -> None:
+    def build_local(
+        self, arr: np.ndarray, worker_nthreads: Optional[int], **kwargs: Any
+    ) -> None:
         raise NotImplementedError
 
 
-class KNNShardingIndexer(KNNIndexer):
+class DistributedKNNIndexer(KNNIndexer):
     def __init__(
         self,
         metric: str,
         indexer: Any,
         group_cols: Optional[List[str]] = None,
         index_shards: Optional[int] = None,
-        broadcast_limit: Any = "10m",
+        index_broadcast_threshold: Any = "10m",
         save_dir: Optional[str] = None,
         indexer_init_kwargs: Optional[Dict[str, Any]] = None,
     ):
         super().__init__(metric)
 
         self._internal_group_cols: List[str] = []
         if group_cols is not None:
@@ -228,218 +262,320 @@
             self._index_shards = 1
         assert_or_throw(
             len(self._internal_group_cols) > 0,
             ValueError("neither group_cols contains columns nor index_shards>1)"),
         )
 
         self._indexer = indexer
-        self._broadcast_limit = to_size(broadcast_limit)
+        self._index_broadcast_threshold = to_size(index_broadcast_threshold)
         self._save_dir = save_dir
         self._indexer_init_kwargs = indexer_init_kwargs or {}
 
-    def build(self, index: AnyDataFrame, vec_col: str, **kwargs: Any) -> "KNNIndexer":
+    def build(
+        self,
+        index: AnyDataFrame,
+        vec_col: str,
+        worker_nthreads: Optional[int] = None,
+        **kwargs: Any,
+    ) -> "KNNIndexer":
         index = fa.as_fugue_df(index)
-        if self._index_shards > 1:
+        if self._index_shards > 1 and len(self._group_cols) > 0:
+            # only when both index_shards>1 and group_cols is not empty
             index = deterministic_shard(
                 index,
                 self._index_shards,
                 _INDEXER_SHARD_COLUMN_NAME,
                 from_cols=[x for x in fa.get_column_names(index) if x != vec_col],
             )
 
         input_schema = fa.get_schema(index)
         assert_or_throw(
             is_vec_col(input_schema, vec_col),
             ValueError(f"{vec_col} is not a vector column"),
         )
-        output_schema = input_schema.extract(self._internal_group_cols) + (
-            _INDEXER_BLOB_COLUMN_NAME,
-            bytes,
-        )
+        indexer_schema = Schema(
+            [
+                (_INDEXER_BLOB_COLUMN_NAME, bytes),
+                (_INDEXER_METADATA_BLOB_COLUMN_NAME, bytes),
+            ]
+        )
+        if len(self._group_cols) > 0:
+            output_schema = (
+                input_schema.intersect(self._internal_group_cols) + indexer_schema
+            )
+            group_cols = self._internal_group_cols
+        else:
+            output_schema = indexer_schema
+            group_cols = []
 
         def _build_group(df: pd.DataFrame) -> pd.DataFrame:
             indexer = knn_indexer(
                 self._indexer, metric=self.metric, **self._indexer_init_kwargs
             )
-            subdf = df.drop(columns=self._internal_group_cols)
-            indexer.build(subdf, vec_col=vec_col, **kwargs)
-            if self._save_dir is not None:
-                temp_file: Optional[str] = os.path.join(
-                    self._save_dir, str(uuid4()) + ".bin"
-                )
-            else:
-                temp_file = None
+            subdf = df.drop(columns=group_cols)
+            indexer.build(
+                subdf, vec_col=vec_col, worker_nthreads=worker_nthreads, **kwargs
+            )
             ser = _KNNIndexerSerializer(
-                indexer, self._broadcast_limit, temp_file=temp_file
+                indexer, self._index_broadcast_threshold, self._save_dir
             )
-            return df.head(1)[self._internal_group_cols].assign(
-                **{_INDEXER_BLOB_COLUMN_NAME: pickle.dumps(ser)}
+            metablob = (indexer.get_metadata_schema(), indexer.get_dim())
+            return df.head(1)[group_cols].assign(
+                **{
+                    _INDEXER_BLOB_COLUMN_NAME: pickle.dumps(ser),
+                    _INDEXER_METADATA_BLOB_COLUMN_NAME: pickle.dumps(metablob),
+                }
             )[output_schema.names]
 
-        self._index = fa.as_pandas(
-            fa.transform(
-                index,
-                _build_group,
-                schema=output_schema,
-                partition=self._internal_group_cols,
-            ),
-        )
+        if len(group_cols) > 0:
+            self._index = fa.as_pandas(
+                fa.transform(
+                    index,
+                    _build_group,
+                    schema=output_schema,
+                    partition=dict(by=group_cols, algo="even"),
+                ),
+            )
+            if _INDEXER_SHARD_COLUMN_NAME not in self._index.columns:
+                self._index.insert(0, _INDEXER_SHARD_COLUMN_NAME, 0)
+        else:  # must be self._index_shards>1
+            self._index = fa.as_pandas(
+                fa.transform(
+                    index,
+                    _build_group,
+                    schema=output_schema.exclude(_INDEXER_SHARD_COLUMN_NAME),
+                    partition=dict(num=self._index_shards, algo="hash"),
+                ),
+            )
+            self._index.insert(0, _INDEXER_SHARD_COLUMN_NAME, range(len(self._index)))
+
         self._mem_size = int(self._index.memory_usage(deep=True).sum())
-        example = pickle.loads(self._index.iloc[0, -1])
-        self._metadata_schema = example.metadata_schema
+        self._metadata_schema, self._dim = pickle.loads(
+            self._index[_INDEXER_METADATA_BLOB_COLUMN_NAME].iloc[0]
+        )
         return self
 
     def search_local(
-        self, queries: np.ndarray, k: int, **kwargs: Any
+        self,
+        query: np.ndarray,
+        k: int,
+        sort_output: bool,
+        worker_nthreads: Optional[int],
+        **kwargs: Any,
     ) -> Tuple[np.ndarray, np.ndarray]:  # pragma: no cover
         raise NotImplementedError(
-            "search_local is not supported for KNNShardingIndexer"
+            "search_local is not supported for DistributedKNNIndexer"
         )
 
     def can_broadcast(self, size_limit: int) -> bool:
         return self._mem_size < size_limit
 
     def get_metadata_df(self) -> pd.DataFrame:  # pragma: no cover
-        raise NotImplementedError
+        raise NotImplementedError(
+            "get_metadata_df is not supported for DistributedKNNIndexer"
+        )
 
     def get_metadata_schema(self) -> Schema:
         return self._metadata_schema
 
+    def get_dim(self) -> int:
+        return self._dim
+
     def search(  # noqa: C901
         self,
-        queries: AnyDataFrame,
+        query: AnyDataFrame,
         k: int,
         vec_col: str,
         dist_col: Optional[str] = None,
         rank_col: Optional[str] = None,
-        index_cache_mem_limit: Any = "1g",
-        queries_chunk_mem_limit: Any = "100m",
-        queries_chunk_row_limit: int = 0,
-        broadcast_limit: Any = "500m",
         drop_vec_col: bool = True,
-        temp_file: Optional[str] = None,
-        index_replicates: Optional[int] = None,
+        index_cache_mem_limit: Any = "1g",
+        index_broadcast_threshold: Any = "500m",
+        query_shards: Optional[int] = None,
+        query_preprocess_mode: str = "direct",
+        query_chunk_mem_limit: Any = "100m",
+        query_chunk_row_limit: int = 0,
+        temp_path: Optional[str] = None,
+        worker_nthreads: Optional[int] = None,
         **kwargs: Any,
     ) -> AnyDataFrame:
 
-        assert_or_throw(
-            rank_col is None or self._index_shards <= 1,
-            NotImplementedError("rank_col is not supported when index_shards>1"),
-        )
-
         is_dist_temp = False
         if self._index_shards > 1 and dist_col is None:
             # when index is sharded, we must keep a dist_col
             # so that we can merge the results from different shards
             dist_col = _TEMP_DIST_COL
             is_dist_temp = True
 
-        queries_schema = fa.get_schema(queries)
+        input_is_native = not isinstance(query, DataFrame)
+        query = fa.as_fugue_df(query)
+        query_schema = fa.get_schema(query)
+        group_cols = self._internal_group_cols
+        query_sharded = query_shards is not None and query_shards > 1
+        query_shards = max(1, query_shards or 1)
+        index_shards = self._index[_INDEXER_SHARD_COLUMN_NAME].unique()
+
+        if query_preprocess_mode == "direct":
+            query = _process_query_directly(
+                query,
+                index_shards=index_shards,
+                query_shards=query_shards,
+                vec_col=vec_col,
+            )
+        elif query_preprocess_mode == "file":
+            assert_or_throw(
+                temp_path is not None,
+                ValueError("temp_path is required when query_preprocess_mode==`file`"),
+            )
+            query = _cache_query_to_file(
+                query,
+                index_shards=index_shards,
+                query_shards=query_shards,
+                group_cols=self._group_cols,
+                temp_path=temp_path,  # type: ignore
+            )
 
         output_schema = self._construct_schema(
-            queries_schema,
+            query_schema,
             vec_col=vec_col,
             dist_col=dist_col,
             rank_col=rank_col,
             drop_vec_col=drop_vec_col,
         )
-        indexer_ser = _KNNIndexerSerializer(self, to_size(broadcast_limit), temp_file)
-        group_cols = self._internal_group_cols
-        sharded = False
+        indexer_ser = _KNNIndexerSerializer(
+            self, to_size(index_broadcast_threshold), temp_path
+        )
 
-        if index_replicates is not None and index_replicates > 1:
-            if self._index_shards > 1:
-                queries = deterministic_shard_and_replicate(
-                    queries,
-                    index_replicates,
-                    _INDEXER_REPLICATES_COLUMN_NAME,
-                    from_cols=[x for x in fa.get_column_names(queries) if x != vec_col],
-                    replicates=self._index_shards,
-                    replicate_col=_INDEXER_SHARD_COLUMN_NAME,
-                )
-            else:
-                queries = deterministic_shard(
-                    queries,
-                    index_replicates,
-                    _INDEXER_REPLICATES_COLUMN_NAME,
-                    from_cols=[x for x in fa.get_column_names(queries) if x != vec_col],
-                )
-            sharded = True
-        elif self._index_shards > 1:
-            queries = replicate(queries, self._index_shards, _INDEXER_SHARD_COLUMN_NAME)
+        def _extract_df(
+            df: pd.DataFrame, indexer: KNNIndexer
+        ) -> Iterable[Tuple[KNNIndexer, Iterable[pd.DataFrame]]]:
+            if query_preprocess_mode == "direct":
+                idx = indexer._index.merge(df.head(1)[group_cols])  # type: ignore
+                if len(idx) > 0:
+                    indexer = pickle.loads(
+                        idx[_INDEXER_BLOB_COLUMN_NAME].iloc[0]
+                    ).get_instance(cache_size=index_cache_mem_limit)
+                    yield indexer, [df]
+            else:  # query_preprocess_mode == "file"
+                # a bit complex logic to dedup indexer loading
+                for _, gpdf in df.groupby(group_cols, dropna=False):
+                    idx = indexer._index.merge(gpdf.head(1)[group_cols])  # type: ignore
+                    if len(idx) > 0:
+                        indexer = pickle.loads(
+                            idx[_INDEXER_BLOB_COLUMN_NAME].iloc[0]
+                        ).get_instance(cache_size=index_cache_mem_limit)
+
+                        def _get_dfs() -> Iterable[pd.DataFrame]:
+                            for file in gpdf[_QUERY_BLOB_COLUMN_NAME]:
+                                yield pd.read_parquet(file)
+
+                        yield indexer, _get_dfs()
 
         def _wrapper(df: pd.DataFrame) -> Iterable[pd.DataFrame]:
-            if sharded:
-                df = df.drop(columns=[_INDEXER_REPLICATES_COLUMN_NAME])
+            reslicer = PandasBatchReslicer(
+                row_limit=query_chunk_row_limit,
+                size_limit=query_chunk_mem_limit,
+            )
             g_indexer = indexer_ser.get_instance(cache_size=index_cache_mem_limit)
-            has_return = False
-            idx = g_indexer._index.merge(df.head(1)[group_cols])  # type: ignore
-            if len(idx) > 0:  # found the corresponding group
-                indexer = pickle.loads(idx.iloc[0, -1]).get_instance(
-                    cache_size=index_cache_mem_limit
-                )
-                reslicer = PandasBatchReslicer(
-                    row_limit=queries_chunk_row_limit,
-                    size_limit=queries_chunk_mem_limit,
-                )
-                for subdf in reslicer.reslice([df]):
+            for indexer, dfs in _extract_df(df, g_indexer):
+                for subdf in reslicer.reslice(dfs):
                     for res in _search_pd_df(
                         indexer=indexer,
                         df=subdf,
                         k=k,
                         vec_col=vec_col,
                         dist_col=dist_col,
                         rank_col=rank_col,
                         drop_vec_col=drop_vec_col,
+                        # with shards>1, we will merge resort in the end
+                        sort_output=rank_col is not None and len(index_shards) == 1,
+                        worker_nthreads=worker_nthreads,
                         **kwargs,
                     ):
                         if len(res) > 0:
-                            has_return = True
                             yield res[output_schema.names]
-            if not has_return:  # TODO: this is a hack, need to fix Fugue
-                yield pd.DataFrame(columns=output_schema.names)
 
         res = fa.transform(
-            queries,
+            query,
             _wrapper,
             schema=output_schema,
-            partition=group_cols
-            if not sharded
-            else group_cols + [_INDEXER_REPLICATES_COLUMN_NAME],
+            partition=dict(
+                by=group_cols
+                if not query_sharded
+                else group_cols + [_QUERY_SHARDS_COLUMN_NAME],
+                algo="even",
+            ),
         )
 
-        if self._index_shards > 1:
-            res = fa.take(
+        if len(index_shards) > 1:
+            qid_group_cols = query_schema.exclude(vec_col).names
+
+            def _get_n(df: pd.DataFrame) -> int:
+                df = df.head(k)
+                if rank_col is not None:
+                    df = df.assign(**{rank_col: range(len(df))})
+                return df
+
+            def _take(df: pd.DataFrame) -> pd.DataFrame:
+                return (
+                    df.groupby(qid_group_cols, dropna=False, group_keys=False)
+                    .apply(_get_n)
+                    .reset_index(drop=True)
+                )
+
+            res = fa.transform(
                 res,
-                n=k,
-                presort=dist_col,
-                partition=queries_schema.exclude(vec_col).names,
+                _take,
+                schema=output_schema,
+                partition=dict(
+                    by=qid_group_cols, algo="coarse", presort=[(dist_col, True)]
+                ),
             )
 
+            # TODO: ray take is not scalable, also need rank col
+            # TODO: this may be the replacement
+            # res = fa.take(
+            #    res,
+            #    n=k,
+            #    presort=dist_col,
+            #    partition=query_schema.exclude(vec_col).names,
+            # )
+
         if is_dist_temp:
             res = fa.drop_columns(res, [dist_col])
 
-        return res
+        return fa.get_native_as_df(res) if input_is_native else res
 
 
 class _KNNIndexerSerializer:
     def __init__(
         self,
         indexer: KNNIndexer,
         broadcast_size_limit: int,
-        temp_file: Optional[str] = None,
+        temp_path: Optional[str] = None,
     ):
-        if indexer.can_broadcast(broadcast_size_limit):
-            self._indexer_obj: Union[KNNIndexer, str] = indexer
-        else:
-            assert_or_throw(temp_file is not None, ValueError("temp_file is required"))
-            indexer.save(temp_file)  # type: ignore
-            self._indexer_obj = temp_file  # type: ignore
-            # Because of lazy evaluation, this class should not delete the temp file
-        self.metadata_schema = indexer.get_metadata_schema()
+        self._indexer_obj: Union[KNNIndexer, str] = indexer
+        self._broadcast_size_limit = broadcast_size_limit
+        self._temp_file = (
+            None
+            if temp_path is None
+            else os.path.join(temp_path, str(uuid4()) + ".index")
+        )
+
+    def __getstate__(self) -> Any:
+        params = dict(self.__dict__)
+        if isinstance(
+            self._indexer_obj, KNNIndexer
+        ) and not self._indexer_obj.can_broadcast(self._broadcast_size_limit):
+            assert_or_throw(
+                self._temp_file is not None, ValueError("temp_file is required")
+            )
+            self._indexer_obj.save(self._temp_file)  # type: ignore
+            params["_indexer_obj"] = self._temp_file  # type: ignore
+        return params
 
     def get_instance(self, cache_size: Any) -> KNNIndexer:
         if isinstance(self._indexer_obj, str):
             return KNNIndexer.load(self._indexer_obj, cache_size=cache_size)
         else:
             return self._indexer_obj
 
@@ -518,25 +654,132 @@
     indexer: KNNIndexer,
     df: pd.DataFrame,
     k: int,
     vec_col: str,
     dist_col: Optional[str],
     rank_col: Optional[str],
     drop_vec_col: bool,
+    sort_output: bool,
+    worker_nthreads: Optional[int],
     **kwargs: Any,
 ) -> Iterable[pd.DataFrame]:
-    qarr = indexer.get_np_arr(df, vec_col=vec_col)
-    idx, dist = indexer.search_local(qarr, k=k, **kwargs)
-    del qarr
-    df = df.reset_index(drop=True)
-    if drop_vec_col:
-        df = df.drop(columns=[vec_col])
-    for j in range(min(k, idx.shape[1])):
-        meta = indexer.get_metadata_df().iloc[idx[:, j]].reset_index(drop=True)
-        more_cols: Dict[str, Any] = {}
-        if dist_col is not None:
-            more_cols[dist_col] = dist[:, j]
-        if rank_col is not None:
-            more_cols[rank_col] = j
-        if len(more_cols) > 0:
-            df = df.assign(**more_cols)
-        yield pd.concat([df, meta], axis=1)
+    with threadpoolctl.threadpool_limits(limits=worker_nthreads):
+        qarr = indexer.get_np_arr(df, vec_col=vec_col)
+        idx, dist = indexer.search_local(
+            qarr,
+            k=k,
+            sort_output=sort_output,
+            worker_nthreads=worker_nthreads,
+            **kwargs,
+        )
+        del qarr
+        df = df.reset_index(drop=True)
+        if drop_vec_col:
+            df = df.drop(columns=[vec_col])
+        for j in range(min(k, idx.shape[1])):
+            meta = indexer.get_metadata_df().iloc[idx[:, j]].reset_index(drop=True)
+            more_cols: Dict[str, Any] = {}
+            if dist_col is not None:
+                more_cols[dist_col] = dist[:, j]
+            if rank_col is not None:
+                more_cols[rank_col] = j
+            if len(more_cols) > 0:
+                df = df.assign(**more_cols)
+            yield pd.concat([df, meta], axis=1)
+
+
+def _process_query_directly(
+    query: AnyDataFrame,
+    index_shards: np.ndarray,
+    query_shards: int,
+    vec_col: str,
+) -> AnyDataFrame:
+    hash_cols = [x for x in fa.get_column_names(query) if x != vec_col]
+
+    def _wrapper(dfs: Iterable[pd.DataFrame]) -> Iterable[pd.DataFrame]:
+        for df in dfs:
+            sdf = _shard(df, query_shards, hash_cols)
+            for shard in index_shards:
+                yield sdf.assign(**{_INDEXER_SHARD_COLUMN_NAME: shard})
+
+    return fa.transform(
+        query,
+        _wrapper,
+        schema=fa.get_schema(query)
+        + Schema(
+            [
+                (_INDEXER_SHARD_COLUMN_NAME, int),
+                (_QUERY_SHARDS_COLUMN_NAME, int),
+            ]
+        ),
+    )
+
+
+def _cache_query_to_file(
+    query: AnyDataFrame,
+    index_shards: np.ndarray,
+    query_shards: int,
+    group_cols: List[str],
+    temp_path: str,
+) -> pd.DataFrame:
+    has_gp_cols = len(group_cols) > 0
+    input_schema = fa.get_schema(query)
+
+    def _wrapper(df: pd.DataFrame, query_shards: int) -> Iterable[pd.DataFrame]:
+        for rep, subdf in enumerate(np.array_split(df, query_shards)):
+            if len(subdf) > 0:
+                path = os.path.join(temp_path, str(uuid4()) + ".parquet")
+                subdf.to_parquet(path, index=False)
+                res = (
+                    subdf.head(1)
+                    .assign(**{_QUERY_BLOB_COLUMN_NAME: path})
+                    .reset_index(drop=True)
+                )
+                yield res.assign(**{_QUERY_SHARDS_COLUMN_NAME: rep})
+
+    if has_gp_cols:
+        res = fa.as_pandas(
+            fa.transform(
+                query,
+                _wrapper,
+                partition=dict(by=group_cols, algo="hash"),
+                schema=input_schema.extract(group_cols)
+                + Schema(
+                    [
+                        (_QUERY_SHARDS_COLUMN_NAME, int),
+                        (_QUERY_BLOB_COLUMN_NAME, str),
+                    ]
+                ),
+                params={"query_shards": query_shards},
+            )
+        )
+    else:
+        res = fa.as_pandas(
+            fa.transform(
+                query,
+                _wrapper,
+                partition=dict(num=query_shards, algo="hash"),
+                schema=Schema(
+                    [
+                        (_QUERY_SHARDS_COLUMN_NAME, int),
+                        (_QUERY_BLOB_COLUMN_NAME, str),
+                    ]
+                ),
+                params={"query_shards": 1},
+            )
+        )
+        res[_QUERY_SHARDS_COLUMN_NAME] = range(len(res))
+    return pd.concat(
+        [res.assign(**{_INDEXER_SHARD_COLUMN_NAME: shard}) for shard in index_shards]
+    )
+
+
+def _shard(df: pd.DataFrame, query_shards: int, hash_cols: List[str]) -> pd.DataFrame:
+    if query_shards <= 1:
+        return df.assign(**{_QUERY_SHARDS_COLUMN_NAME: 0})
+    return df.assign(
+        **{
+            _QUERY_SHARDS_COLUMN_NAME: pd.util.hash_pandas_object(
+                df[hash_cols], index=False
+            ).mod(query_shards)
+        }
+    )
```

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/test/embedding/cache_suite.py` & `fugue-ml-0.0.3.dev2/fugue_ml/testing/embedding/cache_suite.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/utils/fugue_ext.py` & `fugue-ml-0.0.3.dev2/fugue_ml/utils/fugue_ext.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/utils/io.py` & `fugue-ml-0.0.3.dev2/fugue_ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/utils/iter.py` & `fugue-ml-0.0.3.dev2/fugue_ml/utils/iter.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml/utils/numpy/distance.py` & `fugue-ml-0.0.3.dev2/fugue_ml/utils/numpy/distance.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,27 +68,37 @@
     elif metric == "dot":
         return -compute_dot_product_matrix(vec1, vec2)
     else:
         raise ValueError(f"Unknown metric {metric}")
 
 
 def knn(
-    index: np.array, queries: np.array, metric: str, k: int
+    index: np.array, query: np.array, metric: str, k: int, sort_output: bool = False
 ) -> Tuple[np.array, np.array]:
     """The brute force knn search.
 
     :param index: the set of vectors as index, shape (n1, d)
-    :param queries: the set of vectors as queries, shape (n2, d)
+    :param query: the set of vectors as query, shape (n2, d)
     :param metric: the metric to use, 'l2' or 'cos'
     :param k: top k matches with the smallest distance
+    :param sort_output: whether to sort the output by distance, default False
     :return: the indices and distances of the top k matches for
-        each vector in queries, shape (n2, n)
+        each vector in query, shape (n2, n)
     """
-    dist = compute_distance_matrix(queries, index, metric)
+    dist = compute_distance_matrix(query, index, metric)
     if k == 1:
-        idx = np.argmin(dist, axis=1)[:, None]
+        idx = np.argmin(dist, axis=1, keepdims=True)
+        return idx, np.take_along_axis(dist, idx, axis=1)
     elif k < dist.shape[1]:
         idx = np.argpartition(dist, k, axis=1)[:, :k]
+        dist = np.take_along_axis(dist, idx, axis=1)
+        if not sort_output:
+            return idx, dist
+        new_idx = np.argsort(dist, axis=1)
+        return np.take_along_axis(idx, new_idx, axis=1), np.take_along_axis(
+            dist, new_idx, axis=1
+        )
     else:
+        if not sort_output:
+            return np.tile(np.arange(dist.shape[1]), (dist.shape[0], 1)), dist
         idx = np.argsort(dist, axis=1)
-    res = np.take_along_axis(dist, idx, axis=1)
-    return idx, res
+        return idx, np.take_along_axis(dist, idx, axis=1)
```

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml.egg-info/PKG-INFO` & `fugue-ml-0.0.3.dev2/fugue_ml.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fugue-ml
-Version: 0.0.3.dev1
+Version: 0.0.3.dev2
 Summary: Fugue ML
 Home-page: http://github.com/fugue-project/fugue-ml
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Fugue Machine Learning Library
         
@@ -22,7 +22,8 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: openai
 Provides-Extra: huggingface
+Provides-Extra: hnswlib
```

### Comparing `fugue-ml-0.0.3.dev1/fugue_ml.egg-info/SOURCES.txt` & `fugue-ml-0.0.3.dev2/fugue_ml.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 fugue_ml/py.typed
 fugue_ml.egg-info/PKG-INFO
 fugue_ml.egg-info/SOURCES.txt
 fugue_ml.egg-info/dependency_links.txt
 fugue_ml.egg-info/entry_points.txt
 fugue_ml.egg-info/requires.txt
 fugue_ml.egg-info/top_level.txt
-fugue_ml/ann/__init__.py
-fugue_ml/ann/indexer.py
-fugue_ml/ann/integrations/__init__.py
-fugue_ml/ann/integrations/nmslib.py
 fugue_ml/embedding/__init__.py
 fugue_ml/embedding/api.py
 fugue_ml/embedding/base.py
 fugue_ml/embedding/cache.py
 fugue_ml/integrations/__init__.py
+fugue_ml/integrations/hnswlib/__init__.py
+fugue_ml/integrations/hnswlib/indexer.py
+fugue_ml/integrations/hnswlib/registry.py
 fugue_ml/integrations/huggingface/__init__.py
 fugue_ml/integrations/huggingface/_utils.py
 fugue_ml/integrations/huggingface/registry.py
 fugue_ml/integrations/huggingface/sentence_embedding.py
 fugue_ml/integrations/openai/__init__.py
 fugue_ml/integrations/openai/cred.py
 fugue_ml/integrations/openai/embedding.py
 fugue_ml/integrations/openai/registry.py
 fugue_ml/knn/__init__.py
 fugue_ml/knn/api.py
 fugue_ml/knn/brute_force.py
 fugue_ml/knn/indexer.py
-fugue_ml/test/__init__.py
-fugue_ml/test/embedding/__init__.py
-fugue_ml/test/embedding/cache_suite.py
+fugue_ml/testing/__init__.py
+fugue_ml/testing/embedding/__init__.py
+fugue_ml/testing/embedding/cache_suite.py
+fugue_ml/testing/knn/__init__.py
+fugue_ml/testing/knn/local_indexer_suite.py
 fugue_ml/utils/__init__.py
 fugue_ml/utils/fugue_ext.py
 fugue_ml/utils/io.py
 fugue_ml/utils/iter.py
 fugue_ml/utils/params.py
 fugue_ml/utils/registry.py
 fugue_ml/utils/schema.py
@@ -48,20 +49,21 @@
 fugue_ml_version/__init__.py
 tests/embedding/__init__.py
 tests/embedding/fixtures.py
 tests/embedding/test_api.py
 tests/embedding/test_base.py
 tests/embedding/test_cache.py
 tests/integrations/__init__.py
+tests/integrations/hnswlib/__init__.py
+tests/integrations/hnswlib/test_indexer.py
 tests/knn/__init__.py
 tests/knn/test_api.py
 tests/knn/test_api_distributed.py
+tests/knn/test_brute_force.py
 tests/knn/test_indexer.py
-tests/knn/integrations/__init__.py
-tests/knn/integrations/test_brute_force.py
 tests/utils/__init__.py
 tests/utils/test_fugue_ext.py
 tests/utils/test_io.py
 tests/utils/test_iter.py
 tests/utils/test_schema.py
 tests/utils/numpy/__init__.py
 tests/utils/numpy/test_distance.py
```

### Comparing `fugue-ml-0.0.3.dev1/setup.cfg` & `fugue-ml-0.0.3.dev2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 spark_options = 
 	spark.master: local[*]
 	spark.sql.catalogImplementation: in-memory
 	spark.sql.shuffle.partitions: 4
 	spark.default.parallelism: 4
 	spark.executor.cores: 4
 	spark.sql.execution.arrow.pyspark.enabled: true
-	spark.sql.execution.arrow.enabled: false
 	spark.sql.adaptive.enabled: false
 
 [flake8]
-ignore = E24,E203,W503,B023
+ignore = E24,E203,W503,B023,C408
 max-line-length = 88
 format = pylint
 exclude = .svc,CVS,.bzr,.hg,.git,__pycache__,venv,tests/*,docs/*
 max-complexity = 10
 
 [egg_info]
 tag_build =
```

### Comparing `fugue-ml-0.0.3.dev1/setup.py` & `fugue-ml-0.0.3.dev2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,18 +26,19 @@
     long_description_content_type="text/markdown",
     license="Apache-2.0",
     author="The Fugue Development Team",
     author_email="hello@fugue.ai",
     keywords="fugue machine learning ai",
     url="http://github.com/fugue-project/fugue-ml",
     package_data={"fugue_ml": ["py.typed"]},
-    install_requires=["fugue>=0.8.5", "fsspec>=2023.1.0"],
+    install_requires=["fugue>=0.8.6.dev3", "fsspec>=2023.1.0", "threadpoolctl"],
     extras_require={
         "openai": ["openai", "tiktoken"],
         "huggingface": ["transformers", "sentence-transformers"],
+        "hnswlib": ["hnswlib"],
     },
     classifiers=[
         # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: Apache Software License",
@@ -48,10 +49,11 @@
         "Programming Language :: Python :: 3 :: Only",
     ],
     python_requires=">=3.7",
     entry_points={
         "fugue_ml.plugins": [
             "openai = fugue_ml.integrations.openai.registry[openai]",
             "huggingface = fugue_ml.integrations.huggingface.registry[huggingface]",
+            "hnswlib = fugue_ml.integrations.hnswlib.registry[hnswlib]",
         ],
     },
 )
```

### Comparing `fugue-ml-0.0.3.dev1/tests/embedding/fixtures.py` & `fugue-ml-0.0.3.dev2/tests/embedding/fixtures.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/tests/embedding/test_api.py` & `fugue-ml-0.0.3.dev2/tests/embedding/test_api.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/tests/embedding/test_base.py` & `fugue-ml-0.0.3.dev2/tests/embedding/test_base.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/tests/embedding/test_cache.py` & `fugue-ml-0.0.3.dev2/tests/embedding/test_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from fugue_ml.embedding.cache import (
     EmbeddingCache,
     FileEmbeddingCache,
     PandasEmbeddingCache,
     parse_embedding_cache,
 )
-from fugue_ml.test.embedding.cache_suite import EmbeddingCacheTests
+from fugue_ml.testing.embedding.cache_suite import EmbeddingCacheTests
 
 
 def test_parse_embedding_cache(tmpdir):
     c = parse_embedding_cache("file:" + str(tmpdir.join("x.parquet")))
     assert isinstance(c, FileEmbeddingCache)
     assert parse_embedding_cache(c) is c
     with pytest.raises(ValueError):
```

### Comparing `fugue-ml-0.0.3.dev1/tests/knn/test_api.py` & `fugue-ml-0.0.3.dev2/tests/knn/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,24 +11,24 @@
     arr1 = np.array([[1, 2], [3, 4]])
     arr2 = arr1 + 0.001
     arr = np.concatenate([arr1, arr2], axis=0)
     return pd.DataFrame(dict(idx=range(len(arr)), dummy=10, vec=list(arr)))
 
 
 @fixture
-def queries():
+def query():
     arr1 = np.array([[1, 2], [3, 4]])
     arr3 = arr1 - 0.001
     arr = np.concatenate([arr1, arr3], axis=0)
     return pd.DataFrame(dict(q=range(len(arr)), vec=list(arr)))
 
 
-def test_knn_no_group(index_df, queries):
+def test_knn_no_group(index_df, query):
     res = fa.as_pandas(
-        compute_knn(index_df, queries, 2, vec_col="vec", metric="cos", rank_col="rank")
+        compute_knn(index_df, query, 2, vec_col="vec", metric="cos", rank_col="rank")
     )
 
     actual = set(tuple(x) for x in res[["q", "idx", "dummy", "rank"]].values.tolist())
     assert actual == {
         (0, 0, 10, 0),
         (1, 1, 10, 0),
         (2, 0, 10, 0),
@@ -36,17 +36,17 @@
         (0, 2, 10, 1),
         (1, 3, 10, 1),
         (2, 2, 10, 1),
         (3, 3, 10, 1),
     }
 
 
-def test_knn_with_group(index_df, queries, tmpdir):
+def test_knn_with_group(index_df, query, tmpdir):
     idf = index_df.assign(gg=[0, 0, 1, 1])
-    qdf = pd.concat([queries] * 2).assign(gg=[1, 1, 1, 2, 0, 2, 2, 2], q=range(8))
+    qdf = pd.concat([query] * 2).assign(gg=[1, 1, 1, 2, 0, 2, 2, 2], q=range(8))
 
     res = fa.as_pandas(
         compute_knn(
             idf, qdf, 2, vec_col="vec", partition="gg", metric="cos", rank_col="rank"
         )
     )
 
@@ -70,16 +70,16 @@
             idf,
             qdf,
             2,
             vec_col="vec",
             partition="gg",
             metric="cos",
             rank_col="rank",
-            queries_chunk_mem_limit=1,
-            broadcast_limit=1,
+            query_chunk_mem_limit=1,
+            index_broadcast_threshold=1,
             temp_path=str(tmpdir),
         )
     )
 
     actual = set(
         tuple(x) for x in res[["q", "gg", "idx", "dummy", "rank"]].values.tolist()
     )
```

### Comparing `fugue-ml-0.0.3.dev1/tests/utils/numpy/test_distance.py` & `fugue-ml-0.0.3.dev2/tests/utils/numpy/test_distance.py`

 * *Files 17% similar despite different names*

```diff
@@ -38,49 +38,81 @@
             res[i, j] = 1 - np.dot(a, b) / (np.linalg.norm(a, 2) * np.linalg.norm(b, 2))
     assert np.allclose(res, compute_distance_matrix(v1, v2, metric="cos"))
 
 
 def test_knn_matches():
     v1 = np.array([[1, 2, 3], [4, 5, 6]])
     v2 = np.array([[4.1, 5.1, 6.1], [3, 3, 3], [1.1, 2.1, 3.1]])
-    res = np.zeros((2, 3))
+    # k=1
     idx, res = knn(v2, v1, metric="l2", k=1)
     assert np.allclose(idx, np.array([[2], [0]]))
     assert np.allclose(
         res,
         np.array(
             [[np.linalg.norm(v2[2] - v1[0], 2)], [np.linalg.norm(v2[0] - v1[1], 2)]]
         ),
     )
-    idx, res = knn(v2, v1, metric="l2", k=2)
-    assert np.allclose(idx, np.array([[2, 1], [0, 1]]))
+    idx, res = knn(v2, v1, metric="l2", k=1, sort_output=True)
+    assert np.allclose(idx, np.array([[2], [0]]))
     assert np.allclose(
         res,
         np.array(
-            [
-                [np.linalg.norm(v2[2] - v1[0], 2), np.linalg.norm(v2[1] - v1[0], 2)],
-                [np.linalg.norm(v2[0] - v1[1], 2), np.linalg.norm(v2[1] - v1[1], 2)],
-            ]
+            [[np.linalg.norm(v2[2] - v1[0], 2)], [np.linalg.norm(v2[0] - v1[1], 2)]]
         ),
     )
-    idx, res = knn(v2, v1, metric="l2", k=3)
-    assert np.allclose(idx, np.array([[2, 1, 0], [0, 1, 2]]))
+
+    # 1 < k < number of index (v2)
+    idx, res = knn(v2, v1, metric="l2", k=2, sort_output=True)
+    assert np.allclose(idx, np.array([[2, 1], [0, 1]]))
     assert np.allclose(
         res,
         np.array(
             [
-                [
-                    np.linalg.norm(v2[2] - v1[0], 2),
-                    np.linalg.norm(v2[1] - v1[0], 2),
-                    np.linalg.norm(v2[0] - v1[0], 2),
-                ],
-                [
-                    np.linalg.norm(v2[0] - v1[1], 2),
-                    np.linalg.norm(v2[1] - v1[1], 2),
-                    np.linalg.norm(v2[2] - v1[1], 2),
-                ],
+                [np.linalg.norm(v2[2] - v1[0], 2), np.linalg.norm(v2[1] - v1[0], 2)],
+                [np.linalg.norm(v2[0] - v1[1], 2), np.linalg.norm(v2[1] - v1[1], 2)],
             ]
         ),
     )
 
+    # k >= number of index (v2)
+    for k in [3, 4]:
+        idx, res = knn(v2, v1, metric="l2", k=k)
+        assert np.allclose(idx, np.array([[0, 1, 2], [0, 1, 2]]))
+        assert np.allclose(
+            res,
+            np.array(
+                [
+                    [
+                        np.linalg.norm(v2[0] - v1[0], 2),
+                        np.linalg.norm(v2[1] - v1[0], 2),
+                        np.linalg.norm(v2[2] - v1[0], 2),
+                    ],
+                    [
+                        np.linalg.norm(v2[0] - v1[1], 2),
+                        np.linalg.norm(v2[1] - v1[1], 2),
+                        np.linalg.norm(v2[2] - v1[1], 2),
+                    ],
+                ]
+            ),
+        )
+        idx, res = knn(v2, v1, metric="l2", k=k, sort_output=True)
+        assert np.allclose(idx, np.array([[2, 1, 0], [0, 1, 2]]))
+        assert np.allclose(
+            res,
+            np.array(
+                [
+                    [
+                        np.linalg.norm(v2[2] - v1[0], 2),
+                        np.linalg.norm(v2[1] - v1[0], 2),
+                        np.linalg.norm(v2[0] - v1[0], 2),
+                    ],
+                    [
+                        np.linalg.norm(v2[0] - v1[1], 2),
+                        np.linalg.norm(v2[1] - v1[1], 2),
+                        np.linalg.norm(v2[2] - v1[1], 2),
+                    ],
+                ]
+            ),
+        )
+
     with raises(ValueError):
         knn(v1, v2, metric="unknown", k=1)
```

### Comparing `fugue-ml-0.0.3.dev1/tests/utils/test_fugue_ext.py` & `fugue-ml-0.0.3.dev2/tests/utils/test_fugue_ext.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/tests/utils/test_io.py` & `fugue-ml-0.0.3.dev2/tests/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `fugue-ml-0.0.3.dev1/tests/utils/test_iter.py` & `fugue-ml-0.0.3.dev2/tests/utils/test_iter.py`

 * *Files identical despite different names*

